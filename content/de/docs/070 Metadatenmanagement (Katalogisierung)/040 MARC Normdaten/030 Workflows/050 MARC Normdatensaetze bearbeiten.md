---
title: "MARC Normdatensätze bearbeiten"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [app-marc_normdaten, by-folio, cat-workflows, for-anwender]
weight: 50
Description: "
    Quellen: [Folio](https://docs.folio.org/docs/metadata/inventory/marcauthority/#editing-marc-authority-records) & [GBV](https://info.gbv.de/pages/viewpage.action?pageId=854294555)
    "
---

## MARC Normdatensätzen über [📱Datenimport]({{< ref "020 Datenimport" >}}) aktualisieren.

##
MARC-Normdatensätzen über quickMARC bearbeiten

Den MARC-Normdatensatz anzeigen, der bearbeitet werden soll und oben rechts auf **Bearbeiten** klicken. Der Datensatz wird im Bearbeitungsmodus geöffnet. Im Fenster MARC Normdatensatz bearbeiten können die folgenden Aktionen durchgeführt werden:

* **Ein Feld hinzufügen**. Um ein Feld hinzuzufügen, auf das **+** klicken.  Das neue Feld wird darunter angezeigt.
* **Ein Feld löschen**. Um ein Feld zu löschen, auf das **Mülleimersymbol** klicken. Das Feld wird gelöscht.
* **Ein Feld nach oben verschieben**. Um ein Feld nach oben zu verschieben, auf den **Pfeil nach oben** in der Zeile des Feldes, das verschoben werden soll klicken. Das Feld wird eine Zeile nach oben verschoben.
* **Ein Feld nach unten verschieben**. Um ein Feld nach unten zu verschieben, auf den **Abwärtspfeil** in der Zeile des Feldes klicken, das verschoben werden soll. Das Feld wird um eine Zeile nach unten verschoben.
* **Text innerhalb eines Feldes bearbeiten**. In ein Feld klicken, um Änderungen am Text vorzunehmen. Sobald die gewünschten Änderungen vorgenommen wurden, auf **Speichern & schließen** klicken. Ein Bestätigungsdatensatz wird angezeigt und der Datensatz wird aktualisiert.

Validierungen und Einschränkungen

Ein Unterfeld wird durch ein $ (Dollarzeichen) definiert.
Tags müssen aus 3 numerischen Zeichen bestehen.
Indikatoren müssen aus einzelnen Zeichen bestehen.

Es gelten die folgenden Validierungsregeln und Einschränkungen:

* Die Felder 001 und 999ff werden vom System bereitgestellt und können nicht bearbeitet oder gelöscht werden.
* Die LDR kann nicht bearbeitet werden.
* 1xx ist erforderlich und nicht wiederholbar.
* Es wird keine weitere Validierung durchgeführt.
