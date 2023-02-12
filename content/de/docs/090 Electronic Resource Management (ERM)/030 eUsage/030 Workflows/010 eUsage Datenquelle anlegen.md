---
title: "eUsage Datenquelle anlegen"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [app-e_usage, by-folio, cat-workflows, for-anwender]
weight: 10
Description: "
    Quellen: [Folio](https://docs.folio.org/docs/erm/eusage/#creating-a-usage-data-provider ) & [GBV](https://info.gbv.de/display/FOLIOGBVEXTERN/Folio:+eUsage+Datenquelle+anlegen)
    "
---

{{% pageinfo %}}
Achtung "Vendor ID". "Customer ID" sind tatsächlich und absichtlich auf Englisch belassen worden in AG Übersetzung 
{{% /pageinfo %}}

Wenn eine Datenquelle erstellt wird, wird dazu aufgefordert, die Konfigurationsdetails für das automatische Harvesting einzugeben. Wenn der Anbieter nur das manuelle Herunterladen von Daten unterstützt, muss dennoch ein Anbieterdatensatz erstellt werden, um Berichte manuell zu diesem Anbieter hochladen zu können. Weitere Informationen zum manuellen Hochladen von Berichten sind unter Berichte manuell Hochladen zu finden.

1.  In der Ansicht **Datenquellen** auf **Neu** klicken.
2.  Im Fenster **Datenquelle anlegen** die Abschnitte **Informationen zur Datenquelle** und **Abrufeinstellungen** ausfüllen. Weitere Informationen zu den Feldern und Aktionen, die in diesen Abschnitten verfügbar sind, sind in den Abschnittsbeschreibungen unten zu finden.
3.  Sobald alle gewünschten Informationen über die Datenquelle eingegeben wurden, auf **Speichern & schließen** klicken. Die Datenquelle wird gespeichert und der Ansicht  Datenquellen hinzugefügt.

## Informationen zur Datenquelle

* **Name (erforderlich)**. Den Namen des Anbieters der Datenquelle eingeben.
* **Beschreibung**. Eine Beschreibung der Datenquelle. Dieses Feld kann verwendet werden, um zusätzliche Informationen zur Identifizierung des Anbieters oder andere Daten zur Datenquelle oder der Berichte einzugeben, die an prominenter Stelle im Datensatz angezeigt werden sollen.

## Abrufeinstellungen

* **Abrufstatus (erforderlich)**. Einen Abrufstatus wählen: Aktiv oder Inaktiv. Der Status, der hier auswählt wird, legt fest, ob die Berichte der Datenquelle im Rahmen der automatisierten oder manuell ausgelösten Harvesting-Prozesse abgerufen werden.
* **Abrufart (erforderlich)**. Auswählen, wie die Statistiken gesammelt werden sollen: Aggregator oder Sushi. Anmerkung: Der einzige Aggregator, der derzeit von FOLIO unterstützt wird, ist der Deutsche Statistikserver.
* **Aggregator (erforderlich)**. Wurde sich dafür entschieden, die Statistiken über einen Aggregator zu sammeln, den Aggregator auswählen, der für die Sammlung der Statistiken verwendet werden soll. Anmerkung: Der einzige derzeit von FOLIO unterstützte Aggregator ist der Deutsche Statistikserver.
* **Vendor Code**. Wurde sich dafür entschieden, Statistiken über einen Aggregator zu sammeln, den Code eingeben, mit dem der Aggregator den Zulieferer identifiziert, für den die Statistiken angefordert werden. Der Deutsche Statistikserver benötigt die Namen der Lieferanten, wie sie in der Benutzeroberfläche des Servers angezeigt werden.
* **Servicetyp (erforderlich)**. Wurde sich dafür entschieden, Statistiken über ein SUSHI-Protokoll zu sammeln, die Implementierung des SUSHI-Servicetyps auswählen, die vom Harvester verwendet werden soll: Counter-Sushi 4.1 oder Counter-Sushi 5.0. Der Servicetyp entspricht normalerweise der angeforderten Berichtsversion.
* **Service-URL (erforderlich)**. Wurde sich dafür entschieden, Statistiken über ein SUSHI-Protokoll zu sammeln, die URL für den Zugriff auf den SUSHI-Dienst eingeben. Die URL ist normalerweise auf den Backend-Informationsseiten des Anbieters aufgeführt.
    Anmerkung: Nur die Basis-URL zum Dienst eingeben, nicht die vollständige URL für eine API-Anfrage. Wenn der Anbieter z.B. die URL [https://usage.catsanddogs.org/sushi/reports/tr\_b1](https://usage.catsanddogs.org/sushi/reports/tr_b1) aufführt, nur den Teil vor (und ohne) "reports" eingeben: [https://usage.catsanddogs.org/sushi](https://usage.catsanddogs.org/sushi). Alles andere wird vom Harvester hinzugefügt.
* **Berichtsversion (erforderlich)**. Eine Berichtsversion wählen: COUNTER 4 oder COUNTER 5. Anmerkung: Die Unterstützung von Version 5 des Counter-Standards ist für Counter-konforme Datenquellen ab Januar 2019 obligatorisch. FOLIO unterstützt nicht das gleichzeitige Harvesting von Berichten beider Versionen für eine Datenquelle. Wenn nachträglich COUNTER 4-Berichte abgerufen werden sollen, zunächst den Anbieter für COUNTER 4 konfigurieren und die gewünschten Berichte abrufen. Dann die Nutzungsdatenquelle bearbeiten und sie für die Abfrage von COUNTER 5 konfigurieren.
* **Angeforderter Bericht (erforderlich)**. Die Berichtstypen hinzufügen, die für die Datenquelle abgeholt werden sollen. Weitere Informationen sind unter Berichtstyp hinzufügen zu finden.
* **Abruf ab (erforderlich)**. Den ersten Monat für die Berichte eingeben, die abgerufen werden sollen.
* **Abruf bis**. Den letzten Monat für die Berichte eingeben, die abgerufen werden sollen. Anmerkung: Es sollte einen Endmonat hinzugefügt werden, für den Fall, dass keine weiteren Ressourcen von einem Anbieter lizenziert werden, ein Anbieter die Unterstützung von Nutzungsstatistiken einstellt oder aus einem anderen Grund keine fortlaufende Erfassung gewünscht ist. Wenn kein Ende für das Harvesting konfiguriert ist, werden die Berichte kontinuierlich abgerufen, bis der Harvesting-Status auf Inaktiv geändert wird.
* **Customer ID (erforderlich für SUSHI)**. Wurde sich dafür entschieden, Statistiken über ein SUSHI-Protokoll zu sammeln, die vom Anbieter zugewiesene Customer-ID eingeben. Diese Information ist normalerweise auf den Backend-Informationsseiten des Anbieters aufgeführt.
* **Requestor-ID**. Die vom Anbieter zugewiesene Requestor-ID eingeben. Falls erforderlich, ist diese Informationen in der Regel auf den Backend-Informationsseiten des Anbieters zu finden. Nicht alle SUSHI-Dienste erfordern eine Requestor-ID.
* **API-Schlüssel**. Den vom Anbieter zugewiesenen API-Schlüssel eingeben. Falls erforderlich, ist diese Information in der Regel auf den Backend-Informationsseiten des Anbieters zu finden. Nicht für alle SUSHI-Dienste ist ein API-Schlüssel erforderlich.
* **Plattform**. Die Plattform eingeben, für die Berichte angefordert werden. Falls erforderlich, ist diese Informationen in der Regel auf den Backend-Informationsseiten des Anbieters zu finden. Die meisten SUSHI-Dienste sind standardmäßig auf allen Plattformen verfügbar, für die ein Kunde Ressourcen lizenziert hat.
* Requestor name. Den vom Anbieter zugewiesenen Requestor name eingeben. Falls erforderlich, ist diese Information normalerweise auf den Backend-Informationsseiten des Anbieters zu finden. Nicht alle SUSHI-Dienste erfordern einen Requestor name.
* **Requestor mail**. Geben Sie die vom Anbieter zugewiesene Requestor mail eingeben. Falls erforderlich, ist diese Information in der Regel auf den Backend-Informationsseiten des Anbieters zu finden. Nicht für alle SUSHI-Dienste ist eine Requestor mail erforderlich.

## Berichtstyp hinzufügen

1.  Auf **Berichtstyp hinzufügen** klicken.
2.  Einen Berichtstyp aus der Liste der verfügbaren Berichtstypen für die gewählte Berichtsversion auswählen. Die Liste kann gefiltert werden.
3.  Den Vorgang nach Bedarf wiederholen. Der Berichtstyp wird gespeichert, sobald die Datenquelle gespeichert wird.

## Berichtstyp löschen

1.  Die Berichtsart suchen, die gelöscht werden soll.
2.  Auf das Mülleimersymbol klicken. Die Berichtsart ist gelöscht und wird aus dem Datensatz entfernt, sobald die Datenquelle gespeichert wird.
