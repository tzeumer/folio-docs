---
title: "Konfigurationen"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [app-einstellungen, by-folio, cat-einstellungen, for-admin, meta-uebersetzungsproblem]
weight: 10
Description: "
    Quellen: [Folio](https://docs.folio.org/docs/settings/settings_remotestorage/remotestorage/#settings–configurations) & [GBV](https://info.gbv.de/display/FOLIOGBVEXTERN/Einstellungen+(Fernmagazin):+Konfigurationen)
    "
---

{{% pageinfo %}}
Fehlende offizielle Übersetzungen. ("Anmeldeinformationen (Credential properties)")
{{% /pageinfo %}}

Für jedes Fernmagazin muss ein Konfigurationseintrag erstellt werden. Die Vorgehensweise ist für Dematic EMS (API), StagingDirector (TCP/IP) und CAIASoft unterschiedlich.

## Konfigurationen

### Konfiguration für Dematic EMS (API) erstellen

1.  Auf **Neu** klicken.
2.  Auf dem Bildschirm **Konfiguration erstellen** den **Namen des Fernmagazins**, den **Anbieter** und die **URL (Domain)** angeben.
3.  Auf **Speichern & schließen** klicken.

### Konfiguration für StagingDirector (TCP/IP) erstellen

1.  Auf **Neu** klicken.
2.  Auf dem Bildschirm **Konfiguration erstellen** den **Namen des Fernmagazins**, den **Anbieter**, die **URL (Domain)** und die **Status-URL** angeben.
3.  Bei den **Einstellungen des Datenabgleichs**, kann ein Intervall von Minute(n), Stunde(n), Tag(en), Woche(n) oder Monat(en) gewählt werden, das bestimmt, wie oft FOLIO und das Fernmagazin Daten synchronisieren sollen.
4.  Auf **Speichern & schließen** klicken.

### Konfiguration für CAIASoft erstellen

1.  Auf **Neu** klicken.
2.  Auf dem Bildschirm **Konfiguration erstellen** den **Namen des Fernmagazins**, den **Anbieter**, die **URL (Domain)** und die **Anmeldeinformationen (Credential properties)** angeben.
3.  Für die **Einstellungen zum Aufnahmeworkflow** eine der beiden Optionen wählen:
    -   **Dauerhafter Standort ändern**: Wenn ein Exemplar in CAIASoft akzessioniert wird und der dauerhafte Standort des Bestandes nicht mit dem neuen entfernten Standort des Exemplars übereinstimmt, wird der dauerhafte Standort des Bestandes geändert.
    -   **Bestand duplizieren**: Wenn ein Exemplar in CAIASoft aufgenommen wird und ein Bestandsdatensatz für den neuen entfernten Standort noch nicht existiert, wird der nicht entfernte Bestandsdatensatz dupliziert, der Standort im neuen Bestandsdatensatz wird auf den Standort des Exemplars geändert und das Exemplar wird in diesen neuen Bestandsdatensatz verschoben.
4.  Für die **Einstellungen zum Rücknahmeworkflow** eine von zwei Optionen wählen:
    -   **Exemplare im Fernmagazin eingetroffen und gescannt in FOLIO**: Wenn diese Option gewählt wird, geht FOLIO davon aus, dass ein Exemplar direkt in FOLIO gescannt wird, und FOLIO sendet eine Aktualisierung an CAIASoft, die anzeigt, dass das Exemplar voraussichtlich gelagert wird, und setzt den FOLIO-Status des Exemplars auf Verfügbar.
    -   **Exemplar im Fernmagazin eingetroffen und gescannt in CaiaSoft**: Wenn diese Option ausgewählt ist, erwartet FOLIO, dass die Exemplare für die Rückgabe in CAIASoft gescannt werden. Wenn Exemplare in CAIASoft gescannt werden, sendet CAIASoft Informationen an FOLIO. Wenn FOLIO offene Bestandsanfragen zu dem Exemplar findet, verschiebt CAIASoft das Exemplar sofort in den Anforderungsworkflow. Wenn das Exemplar nicht angefordert wird, bucht FOLIO das Exemplar ein und ändert den Status des Exemplars in Verfügbar.
5.  Auf **Speichern & schließen** klicken.

## Konfiguration bearbeiten

1.  Aus der Liste der Konfigurationen diejenige auswählen, die bearbeitet werden soll. Sie wird in einer vierten Ansicht geöffnet.
2.  In der vierten Ansicht auf **Aktionen > Bearbeiten** klicken.
3.  In der Ansicht die gewünschten Änderungen vornehmen.
4.  Auf **Speichern & schließen** klicken.

## Konfiguration löschen

Eine Konfiguration kann nicht gelöscht werden, wenn Standorte auf der FOLIO-Instanz mit dieser Konfiguration verknüpft sind.

1.  In der Liste der Konfigurationen diejenige auswählen, die gelöscht werden soll. Sie wird in einer vierten Ansicht geöffnet.
2.  In der vierten Ansicht auf **Aktionen > Löschen** klicken.
3.  Im Popup-Fenster zur Bestätigung auf **Löschen** klicken.
