---
title: "Kubernetes-Beispiel"
linkTitle: "Kubernetes-Beispiel"
date: 2023-02-01T00:00:00-00:00
tags: [by-folio, for-entwickler]
weight: 30
Description: "
    Quellen: [Folio](https://docs.folio.org/docs/getting-started/installation/kubernetesex/) <!-- & [GBV](https://info.gebev.de/pages/viewpage.action?pageId=850624532) -->
    "
---

Die Rancher/Kubernetes-Lösung ermöglicht das Hinzufügen neuer Mandanten und Hardware-Ressourcen nach Bedarf. Sie ist ideal, wenn die FOLIO-Instanz in Zukunft skalierbar sein muss. Dieser Leitfaden beschreibt eine Rancher/Kubernetes-Installation.

![](/img/de/030%20Kubernetes-Beispiel/030%20Kubernetes-Beispiel_2023-02-20-19-40-27.png)

## Deployment: Umgebungen für die Bereitstellung

FOLIO ist ein System, das auf Microservices basiert. Es ist für eine Multi-Mandanten-Cloud-Umgebung konzipiert. Dennoch werden einige Institutionen FOLIO auch vor Ort einsetzen. Die Community kann mit einer Vielzahl von Bereitstellungsumgebungen und -mechanismen aufwarten. In diesem Leitfaden werden einige der Probleme beschrieben, die in einer Rancher/Kubernetes-Umgebung verstanden werden müssen, sowie die Möglichkeiten, die sich daraus ergeben. Wenn möglich, werden wir auch angeben, was wir für die besten Praktiken halten.

### Öffentliche Cloud vs. vor Ort

Ein produktionsfähiger FOLIO-Einsatz benötigt eine angemessene Infrastruktur für einen zuverlässigen Service. Die Institution muss entscheiden, wo und wie sie FOLIO einsetzen will. Die Entscheidung für eine öffentliche Cloud oder eine Vor-Ort-Installation bestimmt eine Reihe von Optionen für Technologie und Tools. Wenn sich eine Einrichtung beispielsweise für die Bereitstellung in AWS entscheidet, stehen ihr eine Reihe von Werkzeugen und Technologien zur Verfügung, die vor Ort nicht verfügbar sind. Möglicherweise werden auch proprietäre Lösungen wie RDS verwendet. Der Bereitstellungsprozess wird an die Besonderheiten der jeweiligen Organisation angepasst.

### Virtuell vs. physisch

Die Virtualisierung hat sich in Rechenzentren aufgrund der bequemen Verwaltung virtueller Umgebungen zu einer gängigen Praxis entwickelt. Einige Institutionen ziehen jedoch aus verschiedenen Gründen physische Server vor. Die Entscheidung für virtuelle oder physische Server muss nicht zwangsläufig mit der Entscheidung für die Cloud oder für den eigenen Standort zusammenhängen. Es kann zum Beispiel VMware in AWS betrieben werden. Glücklicherweise ist der Bereitstellungsprozess für eine FOLIO-Instanz in beiden Szenarien praktisch derselbe.

### Überlegungen zur Datenbank

FOLIO wurde mit PostgreSQL als Standard-Datenbank-Engine konzipiert und entwickelt. Obwohl die Verwendung von PostgreSQL nicht zwingend erforderlich ist, wird sie für die meisten Anwendungsfälle empfohlen. Die wichtigsten Überlegungen zu PostgreSQL und FOLIO sind, ob:

* ein Cloud-Service wie Amazon RDS oder Amazon Aurora verwendet wird.
* ein dedizierter Datenbankserver oder -cluster eingerichtet wird.
* PostgreSQL-as-a-Service mit Kubernetes eingerichtet wird.
* ein unabhängiger PostgreSQL-Server für die Komponenten von FOLIO verwendet wird.

Diese Entscheidungen hängen von den Ansprüchen der einzelnen Organisationen ab. Aus Sicht der FOLIO-Bereitstellung wird jedoch nur ein verfügbarer PostgreSQL-Dienst benötigt.

### Orchestrierungs-Tools

Es gibt viele Orchestrierungs-Tools sowohl für On-Premise- als auch für Cloud-Lösungen, einschließlich, aber nicht beschränkt auf: Kubernetes, OpenShift, Docker Swarm oder ECS (Amazon). Theoretisch können Sie aufgrund der Microservice-Architektur von FOLIO jedes dieser Tools verwenden, aber die Rancher/Kubernetes-Lösung ist in der FOLIO-Community am weitesten verbreitet und wird daher in diesem Handbuch behandelt.

## Rancher-Server bereitstellen

Es wird ein Rancher-Server für die Verwaltung des Kubernetes-Clusters für FOLIO benötigt. Dieser Server sollte für alle Kubernetes-Knoten in dem Cluster zugänglich sein. Wird AWS verwendet, müssen ein VPC, Subnetze und Routentabellen konfiguriert werden.

Ein Beispiel für die Konfiguration und Bereitstellung sind unter https://github.com/folio-org/folio-install/tree/tamu-r2-2021/alternative-install/kubernetes-rancher/TAMU zu finden.
