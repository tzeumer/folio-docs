---
title: "📱eUsage"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [app-e_usage, by-folio, cat-berechtigungen, for-anwender, meta-fehler_inhalt, meta-uebersetzungsproblem]
weight: 10
Description: "
    Quellen: [Folio](https://docs.folio.org/docs/erm/eusage/) <!-- & [GBV](https://info.gebev.de/pages/viewpage.action?pageId=839188717) -->
    "
---

{{% pageinfo %}}
Rot: Fehlende offizielle Übersetzungen. (vieles)
{{% /pageinfo %}}

Mit der App eUsage können Sie über die Nutzungsdaten von elektronischen Ressourcen verwaltet werden.

Die App ermöglicht das automatische Sammeln von COUNTER-Standardnutzungsberichten über SUSHI und das manuelle Hochladen von Standard- und Nicht-Standardstatistiken. Auf die in eUsage verwalteten Nutzungsdatenquellen kann über die App eManagement zugegriffen werden.

Definition von Bedingungen im Zusammenhang mit der App eUsage:

* **Aggregator**. Ein Dienst, der Statistik-Rohdaten für mehrere Statistikanbieter aggregiert und einen Zugang zum Herunterladen der Berichte bietet. eUsage ermöglicht es, Statistiken für einen Nutzungsdatenanbieter entweder direkt vom Anbieter über SUSHI oder von einem Aggregator zu beziehen. Der einzige Aggregator-Dienst, der derzeit von FOLIO unterstützt wird, ist der deutsche Nationale Statistikserver.
* **COUNTER und SUSHI**. Standardformat und Protokoll für Statistiken zur Nutzung elektronischer Ressourcen. Ausführliche Informationen finden Sie unter [Projekt COUNTER](https://www.projectcounter.org/).
* **Bericht**. Die Nutzungsdaten für einen bestimmten Satz elektronischer Ressourcen innerhalb eines bestimmten Zeitraums für einen bestimmten Typ.
* **Datenquelle** (Usage data provider). Der Anbieter, der Nutzungsstatistiken für eine Reihe von elektronischen Ressourcen bereitstellt. Höchstwahrscheinlich handelt es sich dabei um einen Lieferanten oder einen Plattformanbieter. Die Datensätze des Anbieters von Nutzungsdatenquellen sind die Grundlage in eUsage für die Verwaltung aller zugehörigen Berichte und Sammelprozesse.

## Themen, die noch in der Dokumentation behandelt werden müssen...

(Topics still to be covered by documentation…)

* Starten des Abruf für alle Datenquellen
* Einrichten des periodischen Harvestings
* Einrichten eines Aggregators
* Manuelles Hochladen eines COUNTER-Berichts
* Markieren eines COUNTER-Berichts als manuell geändert
* Hochladen eines Nicht-COUNTER-Berichts
* Herunterladen eines COUNTER-Berichts
* Herunterladen eines Nicht-COUNTER-Berichts
* Löschen von mehreren Berichten
* Löschen eines einzelnen Berichts
* Verknüpfen einer Datenquelle mit einer Vereinbarung

## Berechtigungen

Die unten aufgeführten Berechtigungen ermöglichen die Interaktion mit der App eUsage und legen fest, was innerhalb der App getan werden kann und was nicht. Es können Personen in der App Personen Berechtigungen zugewiesen werden. Wenn einer Person keine dieser Berechtigungen zugewiesen ist, kann sie die App eUsage und alle damit verbundenen Informationen nicht sehen.

Im Folgenden sind alle eUsage Berechtigungen aufgeführt:

* **eUsage: Alle Berechtigungen**. (eUsage: All permissions)
    Diese Berechtigung umfasst alle anderen eUsage-Berechtigungen.
* **eUsage: Kann Datenquellen und COUNTER-Berichte einsehen/herunterladen**. (eUsage: Can view usage data providers and view/download usage reports)
    Dies ist die eUsage Leseberechtigung, die es der Person erlaubt, die Datenquellen der Nutzungsdaten einzusehen und die zugehörigen Berichte über die Nutzung einzusehen und herunterzuladen.
* **eUsage: Kann Datenquellen und COUNTER-Berichte anzeigen und bearbeiten**. (eUsage: Can create and edit usage data providers)
    Diese Berechtigung erlaubt es der Person, UDP-Datensätze (UDP: Usage Data Provider) zu erstellen und zu bearbeiten. Sie umfasst nicht den Upload von Nutzungsberichten zum Anbieter.
* **eUsage: Kann Datenquellen löschen**. (Can delete usage data providers)
    Diese Berechtigung erlaubt es der Person, UDP-Datensätze zu löschen. Sie beinhaltet nicht das Löschen der zugehörigen Nutzungsberichte.
* **eUsage: Kann Nutzungsberichte hochladen**. (Can upload usage reports)
    Diese Berechtigung ermöglicht es der Person, COUNTER- und Nicht-CUNTER-Nutzungsberichte hochzuladen.
* **eUsage: Kann das Harvesting für einen einzelnen Anbieter starten**. (Can start harvesting for a single provider)
    Diese Berechtigung erlaubt es der Person, den Harvesterdienst für einen UDP zu starten.
* **eUsage: Kann Nutzungsberichte löschen**. (eUsage: Can delete usage reports)
    Diese Berechtigung erlaubt es der Person, COUNTER- und Nicht-CUNTER-Nutzungsberichte zu löschen.
* **Einstellungen (eUsage): Kann Einstellungen anzeigen und bearbeiten**. (Settings (eUsage): Can view and edit settings)
    Mit dieser Berechtigung kann die Person die eUsage-Einstellungen anzeigen und bearbeiten. Sie umfasst auch das Starten des Harvesters für alle Nutzungsdatenquellen im Mandanten.

Dies sind weitere Berechtigungen aus Lotus, die in der Originaldoku nicht vorkommen

1.  eUsage: Kann Datenquellen und COUNTER-Berichte anzeigen
2.  eUsage: Kann Datenquellen und COUNTER-Berichte anzeigen und erstellen
3.  eUsage: Kann Datenquellen und COUNTER-Berichte anzeigen, erstellen und bearbeiten
4.  eUsage: Kann Datenquellen und COUNTER-Berichte anzeigen, erstellen, bearbeiten und löschen

und

* eUsage Abruf: Alle Berechtigungen für das eUsage Abruf-Modul
* eUsage Abruf: Nur lesende Berechtigungen für eUsage Abruf-Modul
* eUsage reports: charts may be viewed
* eUsage reports: title matches may be viewed and edited
