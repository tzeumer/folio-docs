---
title: "Bestellung öffnen"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [by-folio, for-anwender, cat-workflows, app-bestellungen]
weight: 70
Description: "
    Quellen: [Folio](https://docs.folio.org/docs/acquisitions/orders/#opening-an-order) & [GBV](https://info.gbv.de/pages/viewpage.action?pageId=851017752)
    "
---

Nachdem eine Bestellung erstellt wurde, hat sie den Status Ausstehend, bis sie geöffnet wird. Sobald eine Bestellung geöffnet wird, finden die folgenden Aktionen statt:

-   Es werden Bindungsvorgänge erstellt. Anmerkung: Bindungsvorgänge werden nur erstellt, wenn eine Fondsverteilung zu einem Bestellposten hinzugefügt wurde.
-   Es werden Katalogeinträge erstellt. Wenn **Im Katalog erstellen** auf der Bestellposten-Zeile auf "Instanz/Bestand/Exemplar" eingestellt ist, wird ein Exemplar mit dem Exemplarstatus "im Erwerbungsvorgang" erstellt. Weitere Informationen zum Artikelstatus sind unter [Exemplarstatus](https://info.gbv.de/display/FOLIOGBVEXTERN/Exemplarstatus) zu finden. Katalogeinträge werden nicht erstellt, wenn **Im Katalog erstellen** in der Bestellposten-Zeile auf Keine eingestellt ist. Weitere Informationen zum Thema Katalogeintrag erstellen sind in den Abschnitten [E-Ressourcen-Details](https://info.gbv.de/pages/viewpage.action?pageId=851017779) und [Physische Details](https://info.gbv.de/pages/viewpage.action?pageId=851017779) weiter unten zu finden.
-   Das Öffnungsdatum wird auf das aktuelle Datum gesetzt.
-   Das Freigabedatum wird auf das aktuelle Datum gesetzt, wenn die Bestellung noch nicht von einer Person freigegeben wurde.
-   Wenn auf der Grundlage der Werte für Titel und Produkt-ID mögliche Duplikate gefunden werden, wird ein Modal mit einer Liste möglicher doppelter Bestellungen angezeigt. Dort Fortsetzen oder Stornieren wählen. Diese Dublettenprüfung kann in den Einstellungen deaktiviert werden. Siehe Einstellungen > Bestellungen > Öffnen von Bestellungen.
-   Bestellposten können nicht hinzugefügt werden, nachdem die Bestellung geöffnet wurde, es sei denn, es wird [Öffnen rückgängig machen](https://info.gbv.de/pages/viewpage.action?pageId=851017754) ausgeführt.
-   Felder wie Bestellungstyp, Titel, Erwerbungsarten und Bestellformat können nicht mehr bearbeitet werden, sobald eine Bestellung geöffnet ist. Um diese Felder zu bearbeiten, muss [Öffnen rückgängig machen](https://info.gbv.de/pages/viewpage.action?pageId=851017754) ausgeführt werden.
1.  [Nach der Bestellung suchen](https://info.gbv.de/display/FOLIOGBVEXTERN/Folio%3A+Bestellungen+suchen+und+exportieren), die geöffnet werden soll und sie auswählen.
2.  In der Ansicht **Bestellung** auf **Aktionen > Öffnen** klicken.
3.  Im Dialog **Öffnen - Bestellung** auf **Absenden** klicken. Es wird eine Bestätigungsmeldung angezeigt und der Status des Bestellungsworkflows ändert sich in Offen.

