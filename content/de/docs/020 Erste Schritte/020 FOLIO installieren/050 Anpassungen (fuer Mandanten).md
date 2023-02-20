---
title: "Anpassungen (für Mandanten)"
linkTitle: "Anpassungen (für Mandanten)"
date: 2023-02-01T00:00:00-00:00
tags: [by-folio, for-entwickler]
weight: 50
Description: "
    Quellen: [Folio](https://docs.folio.org/docs/getting-started/installation/customizations/) <!-- & [GBV](https://info.gebev.de/pages/viewpage.action?pageId=850624536) -->
    "
---

{{% pageinfo %}}
* Siehe auch FAQ bzw. Link zu https://wiki.folio.org/display/Deutsche/FOLIO+Upgrade+-+good+to+know dort - fast identisch zum Handbuch....
{{% /pageinfo %}}

## Branding von Stripes

Stripes verfügt über einige grundlegende Branding-Konfigurationen, die während des Erstellungsprozesses angewendet werden. In der Datei **stripes.config.js** kann das Logo und das Favicon des Mandanten konfiguriert werden. Diese Parameter können unter dem "Branding"-Key am Ende der Datei eingestellt werden. Die neuen Bilder werden in den Ordner tenant-assets eingefügt und in der Konfigurationsdatei mit ihnen verknüpft. Bitte beachten, dass diese Änderungen erst wirksam werden, nach dem Build des Webpack für Stripes ausgeführt wurde.

## Okapi Sicherheit

Es ist sicherzustellen, dass Okapi abgesichert ist, bevor es im Internet bereitgestellt wird. Solange keine Super-Mandanten-Benutzer und kein Passwort für die Okapi-API konfiguriert ist, kann jede Person im Netz privilegierte Anfragen stellen. Die Absicherung von Okapi erfolgt mit dem Skript **secure-supertenant** und wird in den [Server oder PC: Neuinstallation]({{< ref "010 Server oder PC_ Neuinstallation" >}}) erläutert.

Außerdem wird empfohlen, SSL-Zertifikate für Okapi zu konfigurieren, um zu verhindern, dass Daten im Klartext über das Internet gesendet werden. Okapi bietet keine native HTTPS-Unterstützung, aber es kann ein Reverse Proxy (z.B. NGINX) eingerichet werden, der HTTPS-Requests empfängt und an Okapi weiterleitet. Weitere Informationen über HTTPS auf NGINX sind in der NGINX-Dokumentation zu finden. Wird ein Ingress in Kubernetes verwendet, kann auch ein SSL-Zertifikate mit Rancher konfiguriert werden. Weitere Informationen zu diesem Prozess sind in der Rancher-Dokumentation zu finden.

## E-Mail-Konfiguration

Das Modul mod-email bietet die Funktion der Zustellung von Nachrichten über einen SMTP-Server zum Versenden von E-Mails in FOLIO. Es wird für den Versand von Benachrichtigungen und den Neustart von Personen-Passwörtern verwendet.

Das Modul mod-email verwendet mod-configuration, um Verbindungsparameter zu erhalten. Eine detaillierte Liste der Parameter sind in der Dokumentation des Moduls zu finden. Die erforderlichen Konfigurationsoptionen sind die folgenden:

* EMAIL\_SMTP\_HOST
* EMAIL\_SMTP\_PORT
* EMAIL\_USERNAME
* EMAIL\_PASSWORD
* EMAIL\_FROM
* EMAIL\_SMTP\_SSL

Diese Parameter sollten in Okapi durch POST-Requests unter Verwendung des Namens des Moduls gesetzt werden: **SMTP\_SERVER**. Die Host-Konfiguration könnte zum Beispiel so aussehen.

```
curl -X POST \

 http://localhost:9130/configurations/entries \
 -H 'Content-Type: application/json' \
 -H 'X-Okapi-Tenant: <tenant>' \
 -H 'x-okapi-token: <token>' \
 -d
   '{
     "module": "SMTP_SERVER",
     "configName": "smtp",
     "code": "EMAIL_SMTP_HOST",
     "description": "server smtp host",
     "default": true,
     "enabled": true,
     "value": "smtp.googlemail.com"
   }'
```

Bitte beachten, dass diese Konfiguration pro Mandant durchgeführt wird und die Mandant-ID im Header **X-Okapi-Mandant** definiert ist. Außerdem muss man als Superuser des Mandanten eingeloggt sein und das Zugriffstoken im Header **x-okapi-token** angeben. Siehe Beispiel für eine Bestandsanfrage.

Sobald das mod-email Modul konfiguriert ist, sollten weitere Module für die E-Mail-Konfiguration konfiguriert werden: users module und das edge-sip2 Modul. Siehe auch: Bash-Skript zur Automatisierung dieses Vorgangs. Stellen Sie sicher, dass Sie alle für das Skript erforderlichen Umgebungsvariablen ersetzen.

Wird FOLIO in einem Kubernetes-Cluster eingesetzt, kann alternativ ein Kubernetes-Job für diese Aufgabe erstellt werden. Dieses Docker-Projekt https://github.com/folio-org/folio-install/tree/kube-rancher/alternative-install/kubernetes-rancher/TAMU/deploy-jobs/create-email kann ähnlich wie die anderen im Abschnitt über die Kubernetes-Bereitstellung ([Kubernetes-Beispiel]({{< ref "030 Kubernetes-Beispiel" >}})) erwähnten Skripte erstellt, in die Image-Registry übertragen und auf dem Cluster ausgeführt werden.

## Installation und Bereitstellung von Edge-Modulen

Diese Anleitung wurde für eine Einzelserverumgebung geschrieben, in der Okapi auf localhost:9130 läuft.

Wird eine Testinstallation von FOLIO aufgesetzt, müssen überhaupt keine Edge-Module installiert werden. In einer Testumgebung wird ein Edge-Modul nur installiert, wenn getestet werden soll.

Die Edge-Module überbrücken die Lücke zwischen einigen spezifischen Diensten von Drittanbietern und FOLIO (z.B. RTAC, OAI-PMH). In diesen FOLIO-Referenzumgebungen erfolgt der Zugriff auf eine Reihe von Edge-Diensten über Port 8000. In diesem Beispiel wird der Edge-oai-pmh installiert.

Weitere Informationen über die Edge-Module von FOLIO sind im englischsprachigen Wiki zu finden: https://wiki.folio.org/display/FOLIOtips/Edge+APIs.

1.  Institutionellen Benutzer anlegen. Für die Verwendung des Edge-Moduls muss ein institutioneller Benutzer mit den entsprechenden Berechtigungen erstellt werden. Es kann die mitgelieferte Datei create-user.py verwendet werden, um einen Benutzer zu erstellen und Berechtigungen zuzuweisen.

    python3 create-user.py -u instuser -p instpass \\
```
    --permissions oai-pmh.all --tenant diku \\
    --admin-user diku\_admin --admin-password admin
```

Wenn eine Okapi-Instanz angegeben werden muss, die an einem anderen Stelle als http://localhost:9130 läuft, das Flag -okapi-url hinzufügen, um eine andere URL zu übergeben. Wenn mehr als eine Berechtigungsgruppe zugewiesen werden muss, dann eine eine durch Komma getrennte Liste verwenden, d.h. -permissions edge-rtac.all,edge-oai-pmh.all.

2.  Der institutionelle Benutzer wird für jeden Mandanten für die Zwecke der Edge-APIs erstellt. Die Anmeldedaten werden in einem der sicheren Speicher (secure stores) gespeichert und bei Bedarf von der Edge-API abgerufen. Weitere Informationen über sichere Speicher / Secure stores. In diesem Beispiel wird ein einfacher EphemeralStore mit einer **ephemeral.properties**\-Datei verwendet, die Anmeldeinformationen im Klartext speichert. Dies ist nur für Entwicklungs- und Demonstrationszwecke gedacht.

```
sudo mkdir -p /etc/folio/edge
sudo vi /etc/folio/edge/edge-oai-pmh-ephemeral.properties
```

Die Datei mit den ephemeren Propertys sollte wie folgt aussehen.

```
secureStore.type=Ephemeral
# a comma separated list of tenants
tenants=diku
#######################################################
# For each tenant, the institutional user password...
#
# Note: this is intended for development purposes only
#######################################################
# format: tenant=username,password
diku=instuser,instpass
```

3.  Den Edge-Modul-Docker-Container starten. Es wird die auf Okapi verfügbare Version der Edge-Module für den Mandanten benötigt. Es kann eine CURL-Anfrage an Okapi gestellt und die Version des edge-oai-pmh-Moduls abgefragt werden.

```
curl -s http://localhost:9130/_/proxy/tenants/diku/modules | jq -r '.[].id' | grep 'edge-'
```

* Eine Docker-Compose-Datei in /etc/folio/edge/docker-compose.yml erstellen, die jedes Edge-Modul definiert, das als Dienst ausgeführt werden soll. Die compose-Datei sollte wie folgt aussehen.

```
version: '2'
services:
  edge-oai-pmh:
    ports:
      - "9700:8081"
    image: folioorg/edge-oai-pmh:2.2.1
    volumes:
      - /etc/folio/edge:/mnt
    command:
      -"Dokapi_url=http://10.0.2.15:9130"
      -"Dsecure_store_props=/mnt/edge-oai-pmh-ephemeral.properties"
    restart: "always"
```

Sicherstellen, dass Sie die private IP des Servers für die Okapi-URL verwendet wird.

* Die Edge-Modul-Container starten.

```
cd /etc/folio/edge
sudo docker-compose up -d
```

4.  NGINX einrichten.
* Eine neue virtuelle Hostkonfiguration für den Proxy der Edge-Module erstellen. Dies muss innerhalb des Stripes-Containers geschehen. Dazu beim Stripes-Container anmelden, in das nginx-Konfigurationsverzeichnis wechseln und dort eine neue nginx-Konfigurationsdatei erstellen:

```
docker ps --all | grep stripes
docker exec -it <stripes container id> /bin/sh
cd /etc/nginx/conf.d
edit edge-oai.conf
```

Den folgenden Inhalt in die neue Datei edge-oai.conf einfügen:

```
server {
  listen 8130;
  server_name <YOUR_SERVER_NAME>;
  charset utf-8;
  access_log  /var/log/nginx/oai.access.log  combined;
  location /oai {
    rewrite ^/oai/(.*) /$1 break;
    proxy_pass http://<YOUR_SERVER_NAEM>:9700/;
  }
}
```

EIN\_SERVER\_NAME könnte localhost sein. Wird in einer Vagrant-Box gearbeitet, lautet er 10.0.2.15. Den Container beenden und ihn dann neustarten:

```
docker restart <stripes container id>
```

Vielleicht soll auch die Docker-Datei, die den Stripes-Container erstellt, angepasst werden. So kann den Container später oder auf einem anderen Rechner neu erstellt werden. Dazu die Datei edge-oai.conf (mit dem Inhalt wie oben) in das Verzeichnis $HOME/platform-complete/docker/ einfügen und dann eine Zeile in die Dockerdatei $HOME/platform-complete/docker/Dockerfile einfügen:

```
COPY docker/edge-oai.conf /etc/nginx/conf.d/edge-oai.conf
```

Die Änderungen in ein lokales (oder persönliches oder institutionelles) Git-Repository committen.

Jetzt läuft ein OAI-Dienst auf http://server:8130/oai.

5.  Wie folgt vorgehen, um den API-Schlüssel für den Mandanten und den institutionellen Benutzer zu generieren, die in den vorherigen Abschnitten konfiguriert wurden. Derzeit sind die Edge-Module durch API-Schlüssel geschützt.

```
cd ~
git clone https://github.com/folio-org/edge-common.git
cd edge-common
mvn package
java -jar target/edge-common-api-key-utils.jar -g -t diku -u instuser
```

Dies gibt einen API-Schlüssel zurück, der in Requests an Edge-Module vorhanden sein muss. Mit diesem APIKey kann der Zugriff auf das Edge-Modul getestet werden. Eine OAI-Testanfrage würde zum Beispiel so aussehen.

```
curl -s "http://localhost:8130/oai?apikey=APIKEY=&verb=Identify"
```

Die spezifische Methode zur Erstellung einer Bestandsanfrage für ein Edge-Modul ist auf der Website der Entwickler dokumentiert: https://dev.folio.org/source-code/map/ oder es kann das Github-Projekt des jeweiligen Edge-Moduls konsultiert werden.
