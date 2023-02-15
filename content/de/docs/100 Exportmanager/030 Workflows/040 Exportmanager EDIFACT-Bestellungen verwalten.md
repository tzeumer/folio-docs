---
title: "Exportmanager EDIFACT-Bestellungen verwalten"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [app-exportmanager, by-folio, cat-workflows, for-anwender, topic-edi]
weight: 40
Description: "
    Quellen: [Folio](https://docs.folio.org/docs/export-manager/#managing-edifact-orders-export-jobs) <!-- & [GBV](https://info.gebev.de/display/FOLIOGBVEXTERN/Folio:+Exportmanager+EDIFACT-Bestellungen+verwalten) -->
    "
---

Ein FOLIO Mandant kann so konfiguriert werden, dass der Export von EDIFACT-Bestellungen an einen Lieferanten unterstützt wird. Dies erfordert die Konfiguration der Details zur Anbindung an den Datensatz der Organisation. Alle Exporte werden aufgezeichnet und sind in der App Exportmanager in der Ansicht Organisationen zugänglich. Die Datei steht in FOLIO zum Download bereit und hat kein Verfallsdatum. Wenn eine Bibliothek eine neue Kopie der erstellten EDIFACT-Datei benötigt, muss sie die Optionen zum Herunterladen oder erneuten Senden in der App des Exportmanagers verwenden. Die Aktion Erneut senden sendet eine neue Kopie der zuvor exportierten EDIFACT-Datei an den FTP-Server der Organisation, wo die Bibliothek und der Lieferant erneut auf die Datei zugreifen können.

## Einen Exportauftrag für EDIFACT-Bestellungen erneut senden

Um einen Export erneut zu senden: In der **Ansicht Suchen & Filtern** auf **Organisation** klicken. Den Export suchen, der erneut versendet werden soll und auf die Zeile klicken, um den Exportdatensatz aufzurufen. Auf **Aktionen > Erneut senden** klicken. Es erscheint eine grüne Meldung, die anzeigt, dass der Datei-Upload erfolgreich gestartet wurde.

## Erneutes Ausführen eines EDIFACT-Bestellungsexportauftrags

Wird ein Exportauftrag wiederholt, wird ein neuer Exportauftrag ausgelöst, der eine neue Datei mit neuen Bestellungen erzeugt. Der Auftrag verwendet dieselbe Konfiguration, aber die Ergebnisse werden anders sein.

Um einen Export zu wiederholen: In der Ansicht **Suchen & Filtern** auf **Organisation** klicken. Den Export suchen, der erneut ausgeführt werden soll und auf die Zeile klicken, um den Exportdatensatz aufzurufen. Auf **Aktionen > Erneut ausführen** klicken. Der wiederholte Export wird oben in den Exportprotokollen angezeigt. Die Datei kann heruntergeladen werden, indem auf den neuen Exportdatensatz geklickt und dann auf **Aktionen > Download** geklickt wird.
