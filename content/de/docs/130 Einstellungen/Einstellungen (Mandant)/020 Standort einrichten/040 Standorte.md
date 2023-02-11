---
title: "Standorte"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [app-einstellungen, by-folio, cat-einstellungen, for-admin]
weight: 40
Description: "
    Quellen: [Folio](https://docs.folio.org/docs/settings/settings_tenant/settings_tenant/#settings--location-setup--locations) & [GBV](https://info.gbv.de/display/FOLIOGBVEXTERN/Einstellungen+(Mandant):+Standorte)
    "
---

Diese Einstellung verwenden, um die Standorte zu konfigurieren. Ein Standort ist die vierte und detaillierteste Ebene der FOLIO-Standorthierarchie und steht in der Regel für bestimmte Regalbereiche, wie z.B. die Magazine, Vormerkregale oder bestimmte Sprachsammlungen.

## Standorte und Servicestellen

Jedem Standort muss mindestens eine Servicestelle zugeordnet sein, die als primär bezeichnet wird. Standorte können auch über zusätzliche Servicestellen verfügen, die nicht primär sind. Nicht-primäre Servicestellen sind nicht erforderlich.

Wenn ein Exemplar an einer anderen Servicestelle abgegeben wird, die nicht mit dem Standort verbunden ist, wird es zum Transport an die primäre Servicestelle gebracht. Wenn ein Exemplar an einer nicht primären Servicestelle eines Standorts abgegeben wird, wird es nicht in den Transport zur primären Servicestelle gebracht.

Der häufigste Anwendungsfall für einen nicht-primären Servicestelle ist, wenn die Bibliothek mehrere Servicestellen im selben Gebäude hat oder beschließt, zusätzlich zu einer Servicestelle für eine Person, die sich an der Ausleihtheke befindet, eine Servicestelle für Mitarbeitende einzurichten, die "hinter den Kulissen" arbeiten. In diesen Fällen kann eine Servicestelle die primäre Servicestelle für Standorte in diesem Gebäude sein, und die anderen Servicestellen wären keine primäre Servicestellen für diese Standorte. Auf diese Weise können die Mitarbeiter an diesen nicht primären Servicestellen Exemplare für die Bibliothek zurückgeben und ausleihen, ohne dass sie zum Hauptservicepunkt transportiert werden müssen.

## Standort erstellen

1.  In der Ansicht **Standorte** die **Institution** wählen, unter der der Standort erstellt werden soll.
2.  Den **Campus** auswählen, unter dem der Standort erstellt werden soll.
3.  Die **Bibliothek** auswählen, unter der der Standort erstellt werden soll.
4.  Auf **Neu** klicken.
5.  Einen **FOLIO-Namen** für den Standort eingeben. Der Name muss für den FOLIO-Mandanten eindeutig sein. Der Name und der Code werden an anderen Stellen wie dem Katalog angezeigt.
6.  Auswählen, ob der Standort als **Fernmagazin** verwendet werden soll.
7.  Einen **Code** eingeben. Der Code ist der maschinenlesbare Name und muss für den FOLIO-Mandanten eindeutig sein.
8.  Einen **Anzeigename im Discovery** eingeben. Dieser Name wird im Discovery verwendet, um den Standort für Personen zu identifizieren. Er muss nicht eindeutig sein.
9.  Eine primäre **Servicestelle** für den Standort aus der Dropdown-Liste auswählen.
10.  Optional: Um dem Standort eine nicht primäre Servicestelle hinzuzufügen, auf **Servicestelle hinzufügen** klicken und die **Servicestelle** aus der Dropdown-Liste wählen. Den Vorgang nach Bedarf wiederholen. Um eine Servicestelle zu entfernen, klicken Sie auf das **Mülleimersymbol**.
11.  Optional: Den **Status** des Standorts wählen. In der Standardeinstellung sind alle Standorte aktiv.
12.  Optional: Eine **Beschreibung** für den Standort eingeben.
13.  Auf **Speichern & schließen** klicken. Der Standort wird erstellt.

## Standort bearbeiten

1.  In der Ansicht **Standorte** die **Institution** wählen, unter der sich der Standort befindet.
2.  Den **Campus** wählen, unter dem sich der Standort befindet.
3.  Die **Bibliothek** auswählen, unter der sich der Standort befindet.
4.  Den Standort wählen, der bearbeitet werden soll.
5.  In der Ansicht mit den **Standortdetails** auf **Aktionen > Bearbeiten** klicken.
6.  Die gewünschten Änderungen vornehmen.
7.  Auf **Speichern & schließen** klicken. Der Standort wird aktualisiert.

## Standort duplizieren

1.  In der Ansicht **Standorte** die **Institution** wählen, unter der sich der Standort befindet.
2.  Den **Campus** wählen, unter dem sich der Standort befindet.
3.  Die **Bibliothek** auswählen, unter der sich der Standort befindet.
4.  Den Standort wählen, der dupliziert werden soll.
5.  In der Ansicht mit den **Standortdetails** auf **Aktionen > Duplizieren** klicken.
6.  Die gewünschten Änderungen vornehmen.
7.  Auf **Speichern & schließen** klicken. Der Standort wird erstellt.

## Standort löschen

Hinweis: Wenn der Standort von mindestens einem Datensatz im Katalog verwendet wird, kann der Standort nicht gelöscht werden. In diesen Fällen empfiehlt es sich, den Standort zu bearbeiten und den Status auf **Inaktiv** zu setzen. Dadurch wird der Standort zwar nicht aus den Dropdown-Menüs der Standorte im Katalog entfernt, aber die Mitarbeitenden erhalten eine Dialogmeldung, wenn sie einen inaktiven Standort auswählen.

1.  In der Ansicht **Standorte** die **Institution** wählen, unter der sich der Standort befindet.
2.  Den **Campus** wählen, unter dem sich der Standort befindet.
3.  Die **Bibliothek** auswählen, unter der sich der Standort befindet.
4.  Den Standort wählen, der gelöscht werden soll.
5.  In der Ansicht mit den **Standortdetails** auf **Aktionen > Löschen** klicken.
6.  Die gewünschten Änderungen vornehmen.
7.  Auf **Speichern & schließen** klicken. Der Standort wird erstellt.
8.  Im Dialog **Standort löschen** auf **Löschen**. Es wird eine Bestätigungsmeldung angezeigt und der Standort wird gelöscht.

