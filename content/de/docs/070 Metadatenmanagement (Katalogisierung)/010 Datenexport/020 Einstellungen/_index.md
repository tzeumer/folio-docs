---
title: "Einstellungen"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [app-datenexport, by-folio, cat-berechtigungen, cat-einstellungen, for-admin]
weight: 10
Description: "
    Quellen: [Folio](https://docs.folio.org/docs/settings/settings_data_export/settings_data_export/) & [GBV](https://info.gbv.de/pages/viewpage.action?pageId=849379672)
    "
---

Im Abschnitt Datenexport der App Einstellungen können die Jobprofile konfiguriert werden, die beim Datenexport verwendet werden. Jobprofile bestimmen, wie die Informationen in die MARC-Datei exportiert werden, die als Ergebnis des Exports erzeugt wird.

Die App Datenexport wird mit einem Standard Jobprofil geliefert, das nur bibliografische Daten exportiert. Zusätzliche Profile, die Informationen aus den Instanz-, Bestandsdatensätzen und/oder Exemplaren liefern, können nach Bedarf erstellt werden. Mit den Feldmappingprofilen können die Daten, die im Jobprofil verwendet werden, individuell angepasst werden.

Die Feldmapping- und Jobprofile erhöhen die Flexibilität des Datenexports und bieten eine einfache Möglichkeit, einen anderen Exporttyp für denselben Datensatz oder denselben Exporttyp für verschiedene Datensätze auszuführen. Beispielsweise kann ein Personen nur bibliografische Daten exportieren und ein anderer Personen können Instanzen mit angehängten Elementen der Bestandsdatensätze und Exemplare mit demselben Datensatz exportieren.

## Berechtigungen

Um mit den Einstellungen für den Datenexport interagieren zu können, muss einer Person die folgende Berechtigung zugewiesen werden:

-   **Einstellungen (Datenexport): Liste der Einstellungsseiten anzeigen**. (Settings (data-export): display list of settings pages)
    Mit dieser Berechtigung kann die Person Datenexportprofile einrichten.
