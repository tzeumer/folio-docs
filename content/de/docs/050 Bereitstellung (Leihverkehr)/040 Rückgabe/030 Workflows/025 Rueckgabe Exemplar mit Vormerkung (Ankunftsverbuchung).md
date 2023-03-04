---
title: "Rückgabe Exemplar mit Vormerkung (Ankunftsverbuchung)"
linkTitle: ""
date: 2023-03-04T00:00:00-00:00
tags: [by-folio, for-anwender, app-rückgabe, cat-workflows]
weight: 25
Description: "
    Quellen: [Folio](https://docs.folio.org/docs/access/check-in/checkin/#checking-in-an-item-with-a-request-hold-shelf-fulfillment)
    "
---

Wenn eine Person eine Bestandsanfrage stellt, löst das Einchecken des Exemplars an der gewünschten Abholservicestelle die Vormerkungsankunftsverbuchung aus.

1. Entweder den Barcode des Exemplars scannen, oder den Barcode eingeben und auf **Eingabe** klicken. Es erscheint ein Dialog "Bestandsanfrage ins Abholregal hinterlegen" mit dem Hinweis, dass das Exemplar zur Abholung bereitsteht, und einer Auflistung der Servicestelle, an der es abgeholt werden soll.
2. Wenn kein Vormerkungszettel ausgedruckt werden soll, die Checkbox **Zettel drucken** deaktivieren, sofern sie markiert ist.
3. Auf **Schließen** klicken, um das Fenster zu schließen und einen Vormerkungszettel auszudrucken, sofern ausgewählt. Das Exemplar erscheint in der Tabelle Gescannte Objekte und sein Status ändert sich in Im Abholregal. FOLIO setzt automatisch das Ablaufdatum/die Ablaufzeit des Abholregals auf die Bestandsanfrage, entsprechend den Einstellungen für die Datumsverwaltung der Abholservicestelle. Falls in der Benachrichtigungsrichtlinie konfiguriert, wird der Person nach Beendigung der Rückgabe eine Abholbenachrichtigung zugesandt.
