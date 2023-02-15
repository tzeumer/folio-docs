---
title: "Bestellposten mit anderer Instanz verknüpfen"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [by-folio, for-anwender, cat-workflows, app-bestellungen, meta-uebersetzungsproblem]
weight: 260
Description: "
    Quellen: [Folio](https://docs.folio.org/docs/acquisitions/orders/#changing-an-instance-connection ) & [GBV](https://info.gbv.de/pages/viewpage.action?pageId=851345487)
    "
---

Folgendermaßen vorgehen, um die Verbindung der Katalog-Instanz für einen Bestellposten zu ändern:

1.  [Nach dem Bestellposten suchen]({{< ref "230 Bestellposten suchen" >}}), der geändert werden soll und ihn auswählen.
2.  In der Ansicht **Details zum Bestellposten** auf **Aktionen > Instanz-Verknüpfung ändern** klicken. Das Fenster **Instanz auswählen** wird geöffnet.
3.  Den Titel mit Hilfe des Suchfeldes und/oder der Filter suchen. Auf den Titel klicken, um ihn auszuwählen. Das Fenster **Titel ändern** wird geöffnet: "Die Titelinformationen dieser Bestellpostens wurden von (VON) nach (ZU) geändert. Alle zugehörigen Exemplardatensätze werden in die neue Instanz verschoben. Wie sollen die zugehörigen Bestände adressiert werden?"
4.  Auf die Dropdown-Liste **So werden Bestände aktualisiert** klicken und **Transferieren**, **Finde oder erstelle neu** oder **Neu erstellen** wählen.
5.  Sollen neue Bestände angelegt oder anhand des aktuellen Standorts der Exemplare passende Bestände gefunden werden, fragt FOLIO, ob die aufgegebenen Bestände nach Möglichkeit gelöscht werden sollen. In einem Popup-Fenster wird angezeigt: "Dieses Stück ist mit Datensätzen im Katalog verbunden. Es gibt keine weiteren Exemplare, die mit diesen Bestandsdatensätzen verbunden sind. Möchten Sie nach dem Löschen des Stückes, dass FOLIO die Bestandsdatensätze löscht?" **Absenden** wählen, um die Änderung der Instanzverknüpfung abzuschließen. Entweder **Bestand behalten** oder **Bestand löschen** wählen, um fortzufahren.
6.  Die Bestätigungsmeldung "**Verknüpfung der Instanz der Bestellung wurde erfolgreich aktualisiert**" wird angezeigt.
