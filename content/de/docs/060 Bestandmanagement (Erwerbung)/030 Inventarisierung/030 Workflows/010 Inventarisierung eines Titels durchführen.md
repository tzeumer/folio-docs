---
title: "Inventarisierung eines Titels durchführen"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [app-inventarisierung, by-folio, cat-workflows, for-anwender]
weight: 10
Description: "
    Quellen: [Folio](https://docs.folio.org/docs/acquisitions/receiving/#creating-a-receiving-title) & [GBV](https://info.gbv.de/pages/viewpage.action?pageId=851935415)
    "
---

Normalerweise besteht eine Bestellung aus einem zu inventarisierenden Titel, der aus ein oder mehrere Teile bestehen kann. Wenn z.B. eine Zeitschrift bestellt wurde, wäre der zu inventarisierende Titel der Name der Zeitschrift und die angehängten Teile wären die einzelnen Ausgaben der Zeitschrift.

Bestellposten können auch zur Darstellung von Paketen verwendet werden. Ein Bestellposten für ein Paket wird in der App Bestellungen als einzelner Bestellposten angelegt, kann aber in der Inventarisierung nicht gefunden oder inventarisiert werden, da er den Erwerb mehrerer Titel darstellt (z.B. einen monographischen Dauerauftrag). Um die in einem Paket enthaltenen Titel zu inventarisieren, müssen die zu inventarisierenden Titel in der App Inventarisierung angelegt und mit dem Bestellposten für das Paket verknüpft werden. In dieser Version von FOLIO müssen die zu inventarisierenden Titel mit einer Instanz in der App Inventarisierung und einem Bestellposten verbunden sein.

Mit der Aktion **Neu** können die zu inventarisierenden Titel in einem Paket erstellt werden, damit sie von der Bibliothek inventarisiert werden können. Mit dieser Aktion können auch vorhandene Instanzen mit einem Bestellposten-Paket verknüpft werden, wenn eine Beziehung zwischen der Instanz und der Bestellung hergestellt werden soll. In diesem Fall ist der zu inventarisierende Titel anhand der zugehörigen Bestellpostennummer durchsuchbar.

1.  Auf **Neu** klicken.
2.  Im Fenster **Neuer Titel** im Abschnitt Bestellpostendetails auf **Bestellpostennummersuche** klicken.
3.  Im Dialog **Bestellposten auswählen** im Feld **Suche & Filter** die Bestellpostennummer des Pakets eingeben.
4.  Optional: Die Ergebnisse mit Hilfe der Filter im Dialog **Bestellposten auswählen** filtern.
5.  Auf **Suchen** klicken und das Paket aus den Suchergebnissen auswählen. Der Bestellposten für das Paket wird mit dem neuen Titel verknüpft.
6.  Einen **Titel** für das Exemplar im Paket eingeben.
7.  Die restlichen Felder unter Exemplardetails und Bestellpostendetails ausfüllen. Weitere Informationen zu den Feldern und Aktionen, die in diesen Abschnitten verfügbar sind, sind in den Abschnittsbeschreibungen unten zu finden.
8.  Auf **Speichern & schließen** klicken. Es wird eine Bestätigungsmeldung angezeigt, und der neue zu inventarisierende Titel wird erstellt und in der Ansicht Inventarisierung angezeigt. Er kann nun bearbeitet werden und erwartete Teile können hinzugefügt und inventarisiert werden. Der Titel kann gefunden werden, indem nach der Bestell- oder Bestellpostennummer, dem Paketnamen oder dem Titelgesucht wird.

## Exemplardetails

-   **Titel**. Der Titel der Ressource, die inventarisiert werden soll. Anmerkung: Bei Bestellposten, die nicht zum Paket gehören, wird der zu inventarisierende Titel automatisch erstellt. Bei Bestellposten für Pakete die **Titelsuche** verwenden, um eine Inventarinstanz mit dem Bestellposten für Pakete zu verknüpfen und einen inventarisierenden Titel erfolgreich hinzuzufügen.
-   **Verlag**. Verlag der Ressource.
-   **Erscheinungsdatum**. Datum, an dem die Ressource veröffentlicht wurde.
-   **Ausgabe**. Ausgabe der Ressource.
-   **Abonnement von**. Datum des Beginns des Abonnements (falls zutreffend).
-   **Abonnement bis**. Enddatum des Abonnements (falls zutreffend).
-   **Abonnementintervall**. Anzahl der Tage, in der das Abonnement erscheint (falls zutreffend).
-   **Mitwirkender**. Mitwirkende der Ressource.
-   **Produkt-ID**. Eine Identifikationsnummer, wie ISBN oder DOI.

### Mitwirkende

#### Mitwirkende hinzufügen

Anmerkung: Das Hinzufügen von Mitwirkenden ist optional, aber wenn auf **Mitwirkende hinzufügen** geklickt wird, müssen **Mitwirkende** und eine **Mitwirkenden-ID-Typ** eingeben werden oder der Eintrag gelöscht werden, um den Titel zu speichern.

1.  Auf **Mitwirkende hinzufügen** klicken.
2.  Den/die **Mitwirkende** eingeben.
3.  Einen **Mitwirkenden-ID-Typ** aus der Dropdown-Liste wählen. Der/die Mitwirkende wird hinzugefügt, sobald alle Änderungen gespeichert sind.

#### Mitwirkende löschen

1.  Den Mitwirkendeneintrag suchen, der gelöscht werden soll.
2.  Auf das **Mülleimersymbol** klicken. Der Mitwirkendeneintrag wird entfernt und gelöscht, sobald die Änderungen gespeichert sind.

### Produkt-ID und -Typ

#### Produkt-ID und Produkt-ID-Typ hinzufügen

Anmerkung: Das Hinzufügen einer Produkt-ID und eines Typs ist optional, aber wenn auf Produkt-ID und Produkt-ID-Typ hinzufügen geklickt wird, müssen eine Produkt-ID und ein Produkt-ID-Typ eingeben werden oder die Produkt-ID und den Typ gelöscht werden, um den Titel zu speichern.

1.  Auf **Produkt-ID und Produkt-ID-Typ hinzufügen** klicken.
2.  Die **Produkt-ID** eingeben.
3.  Optional: Eine Bedingung eingeben. Zum Beispiel könnte _Paperback_ als Bedingung für eine ISBN hinzufügt werden.
4.  Den Produkt-ID-Typ aus der Dropdown-Liste wählen. Die Produkt-ID wird hinzugefügt, sobald alle Änderungen gespeichert sind.

#### Produkt-ID und -Typ löschen

1.  Die Produkt-ID suchen, die gelöscht werden soll.
2.  Auf das **Mülleimersymbol** klicken. Die Produkt-ID wird entfernt und gelöscht, sobald die Änderungen gespeichert sind.

## Bestellpostendetails

-   **Bestellpostennummer**. Die Nummer des Bestellpostens. Diese kann nur mit Hilfe der Bestellpostennummersuche eingegeben werden. Weitere Informationen sind weiter oben in dieser Seite zu finden.
-   **Erwartetes Eingangsdatum**. Das Datum, an dem die Ressource voraussichtlich eintreffen wird. Dieses Datum wird automatisch mit Informationen aus Bestellungen gefüllt und kann nicht geändert werden.
-   **Inventarisierungsnotiz**. Anmerkungen zum Erhalt der Ressource. Dieses Feld wird automatisch mit Informationen aus den Bestellungen gefüllt und kann nicht geändert werden.
-   **Inventarisierungsnotiz bestätigen**. Wenn diese Checkbox aktiviert ist, wird das Dialogfeld Inventarisierung angezeigt, sobald versucht wird, die Ressource zu inventarisieren. Es muss auf Weiter geklickt werden, um die Ressource zu inventarisieren.

### Bestehenden Titels mit zu inventarisierenden Titeln verknüpfen

1.  Im Fenster **Neuer Titel** auf **Titelsuche** klicken.
2.  Im Dialog **Instanz auswählen** im Feld **Suche & Filter** den Titel eingeben, der mit dem Paket verknüpft werden soll.
3.  Optional: Die Ergebnisse mit Hilfe der Filter im Dialogfeld **Instanz auswählen** filtern.
4.  Auf **Suche** klicken und den Titel aus den Suchergebnissen auswählen. Dadurch werden alle Felder ausgefüllt, die bereits für den vorhandenen Titel ausgefüllt wurden.
5.  Den Rest der Felder unter Exemplardetails ausfüllen. Weitere Informationen sind unter Exemplardetails oben zu finden.
6.  Auf **Bestellpostennummersuche** klicken.
7.  Im Dialog **Bestellposten auswählen** im Feld **Suche & Filter** die Bestellpostennummer des Pakets eingeben.
8.  Optional: Die Ergebnisse mit Hilfe der Filter im Dialogfeld **Bestellposten auswählen** filtern.
9.  Auf **Suchen** klicken und das Paket aus den Suchergebnissen auswählen.
10.  Auf **Speichern & schließen** klicken. Der vorhandene Titel ist nun mit dem Paket-Bestellposten verknüpft. Es kann über die Suche nach dem Titel, der ursprünglichen Bestellpostennummer, der Bestellposten-Nummer des Pakets oder dem Namen des Pakets gefunden werden.
