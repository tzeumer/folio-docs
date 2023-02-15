---
title: "FOLIO-Systeminformationen (Installationsdetails)"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [app-einstellungen, by-folio, cat-einstellungen, for-admin]
weight: 10
Description: "
    Quellen: [Folio](https://docs.folio.org/docs/settings/system_software_versions/system_software_versions/ ) <!-- & [GBV](https://info.gebev.de/pages/viewpage.action?pageId=841809973) -->
    "
---

Auf der Seite mit den Installationsdetails werden alle Komponenten aufgelistet, die für den aktuellen Mandanten ausgeführt werden. Wenn einen Fehler gemeldet werden soll, sollte die Version des betroffenen Moduls angegeben werden, um den Support- und Entwicklungsteams zu helfen.

## Berechtigungen

Es gibt keine explizite Berechtigung zum Anzeigen von Einstellungen > Installationsdetails. Wenn ein FOLIO-Benutzer Zugriff auf einen beliebigen Bereich der Einstellungen hat, kann sie auch Einstellungen > Installationsdetails > Software-Versionen sehen.

## Aufbau der Seite

Die Seite ist dreispaltig.

* Benutzeroberfläche: Informationen über Stripes (das FOLIO UI-Framework) und die damit verbundene Infrastruktur
    * Basis
    * Appmodule
    * Pluginmodule
    * Module für Einstellungen
    * Handler Module
* Okapi: Informationen über Okapi (das FOLIO API-Gateway) und die zugehörige Infrastruktur
    * Okapi
    * Module
    * Interfaces
* Abhängigkeiten: Informationen über Abhängigkeiten zwischen verschiedenen Bereichen der FOLIO-Infrastruktur
    * Basis
    * Appmodule
    * Pluginmodule
    * Module für Einstellungen
    * Handler-Module

## "Blumen"-Releases (Softwareversionen)

Suchen Sie nach diesen Modulen, um herauszufinden, welche FOLIO Flower-Version auf dem System läuft. Dies ist ein guter Indikator dafür, ob der offizielle plattformübergreifende Satz von Modulen installiert wurde und keine individuellen Änderungen vorgenommen wurden.

|mod-configuration|mod-inventory-storage|mod-login-saml|release|
|:----|:----|:----|:----|
|05.09.00|25.0.3|02.05.00|[Nolana R3-2022-GA](https://github.com/folio-org/platform-complete/blob/R3-2022-GA/install.json)|
|05.08.00|24.01.00|02.04.09|[Morning Glory R2-2022-GA](https://github.com/folio-org/platform-complete/blob/R2-2022-GA/install.json)|
|05.07.09|23.0.5|02.04.09|[Lotus R1-2022-hotfix-3](https://github.com/folio-org/platform-complete/blob/R1-2022-hotfix-3/install.json)|
|05.07.09|23.0.5|02.04.08|[Lotus R1-2022-hotfix-2](https://github.com/folio-org/platform-complete/blob/R1-2022-hotfix-2/install.json)|
|05.07.08|23.0.5|02.04.05|[Lotus R1-2022-hotfix-1](https://github.com/folio-org/platform-complete/blob/R1-2022-hotfix-1/install.json)|
|05.07.06|23.0.2|02.04.04|[Lotus R1-2022-GA](https://github.com/folio-org/platform-complete/blob/R1-2022-GA/install.json)|
|05.07.07|22.0.4|02.04.05|[Kiwi R3-2021-hotfix-3](https://github.com/folio-org/platform-complete/blob/R3-2021-hotfix-3/install.json)|
|05.07.05|22.0.4|02.04.02|[Kiwi R3-2021-hotfix-2](https://github.com/folio-org/platform-complete/blob/R3-2021-hotfix-2/install.json)|
|05.07.04|22.0.4|02.04.02|[Kiwi R3-2021-hotfix-1](https://github.com/folio-org/platform-complete/blob/R3-2021-hotfix-1/install.json)|
|05.07.03|22.0.4|02.03.02|[Kiwi R3-2021-GA](https://github.com/folio-org/platform-complete/blob/R3-2021-GA/install.json)|
|05.07.04|21.0.10|02.04.01|[Juniper R2-2021-hotfix-6](https://github.com/folio-org/platform-complete/blob/R2-2021-hotfix-6/install.json)|
|05.07.04|21.0.10|02.03.02|[Juniper R2-2021-hotfix-5](https://github.com/folio-org/platform-complete/blob/R2-2021-hotfix-5/install.json)|
|05.07.02|21.0.9|02.02.01|[Juniper R2-2021-hotfix-4](https://github.com/folio-org/platform-complete/blob/R2-2021-hotfix-4/install.json)|
|05.07.01|21.0.9|02.02.01|[Juniper R2-2021-hotfix-3](https://github.com/folio-org/platform-complete/blob/R2-2021-hotfix-3/install.json)|
|05.07.00|21.0.3|02.02.01|[Juniper R2-2021-hotfix-2](https://github.com/folio-org/platform-complete/blob/R2-2021-hotfix-2/install.json)|
|05.07.00|21.0.3|02.02.01|[Juniper R2-2021-hotfix-1](https://github.com/folio-org/platform-complete/blob/R2-2021-hotfix-1/install.json)|
|05.07.00|21.0.3|02.02.01|[Juniper R2-2021-GA](https://github.com/folio-org/platform-complete/blob/R2-2021-GA/install.json)|
