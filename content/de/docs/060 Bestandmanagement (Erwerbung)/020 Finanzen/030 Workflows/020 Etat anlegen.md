---
title: "Etat anlegen"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [app-finanzen, by-folio, cat-workflows, by-folio]
weight: 20
Description: "
    Quellen: [Folio](https://docs.folio.org/docs/acquisitions/finance/#creating-a-ledger) <!-- & [GBV](https://info.gebev.de/display/FOLIOGBVEXTERN/Folio:+Etat+anlegen) -->
    "
---

Ein Etat ist eine Sammlung von Fonds, die fiskalisch von der Sammlung von Fonds eines anderen Etats getrennt gehalten werden muss. Einem Haushaltsjahr können mehrere Etats zugeordnet werden, und jeder Etat kann in zukünftigen Haushaltsjahren fortbestehen. Ein Fonds kann nur mit einem einzigen Etat verknüpft werden.

1.  In der Ansicht **Suche & Filter** auf **Etat** klicken.
2.  In der Ansicht **Etat** auf **Neu** klicken.
3.  Im Fenster **Etat erstellen** alle erforderlichen Informationen für das Etat eingeben. Weitere Informationen zu den Feldern und Aktionen, die in diesem Bereich verfügbar sind, sind in den Beschreibungen unten zu finden.
4.  Auf **Speichern & Schließen** klicken. Das Etat wird gespeichert.

Informationen zum Etat

1.  **Name (erforderlich)**. Name des Etats. Zum Beispiel: Jurabibliothek.
2.  **Code (erforderlich)**. Von der Person erstellt, basierend auf dem Namen.
3.  **Haushaltsjahr 1 (erforderlich)**. Das erste Haushaltsjahr für den Etat. Etats können weiterhin für mehrere Haushaltsjahre verwendet werden. Wenn das Haushaltsjahr nicht in der Liste erscheint, kann auf **Neues Haushaltsjahr** geklickt werden, um ein neues anzulegen.
4.  **Status (erforderlich)**. Den Status des Etats wählen: Aktiv, Gesperrt oder Inaktiv. Aktiv bedeutet, dass das Etat läuft, gesperrt bedeutet, dass das die Verwendung des Etats pausiert wurde, und inaktiv bedeutet, dass das Etat nicht mehr verwendet wird.
5.  **Erwerbungsteams**. Ist gewünscht, dass nur bestimmte Personen innerhalb bestimmter Erwerbungsteams den Etat bearbeiten können, die Erwerbungsteams eingeben oder diese aus der Dropdown-Liste auswählen. Es können mehrere Teams ausgewählt werden. Wenn das Feld leer ist, können alle Personen, die über die entsprechenden Berechtigungen verfügen, die Informationen des Etats bearbeiten. Weitere Informationen finden Sie unter [Einstellungen > Erwerbungsteams]({{< ref "010 Einstellungen (Erwerbungsteams)_ Erwerbungsteam erstellen, bearbeiten, loeschen" >}}).
6.  **Bindungen nicht beschränken**. Dieses Feld ist standardmäßig markiert. Dieses Kästchen markiert lassen, wenn gewünscht ist, dass das System alle Bindungen gegen Fonds, die mit diesem Etat verbunden sind, ablehnt, die den verfügbaren Betrag des aktuellen Budgets überschreiten würden. Dieses Kontrollkästchen deaktivieren, wenn die Bindung von Beträgen an das Budget des laufenden Jahres ohne Einschränkungen zulassen möchten.
7.  **Ausgaben nicht beschränken**. Dieses Feld ist standardmäßig markiert. Dieses Feld markiert lassen, wenn gewünscht ist, dass das System alle Ausgaben für Fonds, die mit diesem Etat verbunden sind, ablehnt, die den verfügbaren Betrag des aktuellen Budgets überschreiten würden. Dieses Kontrollkästchen deaktivieren, um Ausgabenbeträge für das Budget des laufenden Jahres ohne Einschränkungen zuzulassen.
8.  **Beschreibung**. Eine Beschreibung des Etats.
