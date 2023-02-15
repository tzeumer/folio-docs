---
title: "Rechnung stornieren"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [app-rechnungen, by-folio, cat-workflows, for-anwender]
weight: 130
Description: "
    Quellen: [Folio](https://docs.folio.org/docs/acquisitions/invoices/#paying-an-invoice) & [GBV](https://info.gbv.de/display/FOLIOGBVEXTERN/Folio:+Rechnung+stornieren)
    "
---

Das Stornieren einer Rechnung ist möglich, während sie sich im Status Freigegeben oder Bezahlt befindet und wenn das Personenkonto **Berechtigung Rechnung: Rechnung stornieren** hat. Das Stornieren einer Rechnung löst die folgenden Systemaktionen aus:

* Alle Vorgänge gegen Fonds, die sich auf die Rechnung beziehen, werden storniert.
* Der Status des Rechnungsbelegs wird auf Storniert gesetzt.
* Personen können die Rechnung nach dem Stornieren weder öffnen noch freigeben oder bezahlen. Um eine Rechnung zu stornieren, folgendermaßen vorgehen:
    1.  [Die Rechnung suchen]({{< ref "030 Rechnung suchen" >}}), die storniert werden soll und sie auswählen.
    2.  In der Ansicht **Rechnungsnummer des Lieferanten** auf **Aktionen > Stornieren** klicken.
    3.  Im Dialog **Rechnung stornieren** optional eine **Anmerkung zur Stornierung** eingeben. Die Anmerkung zur Stornierung wird in dem Akkordeon Informationen zur Rechnung angezeigt.
    4.  Auf **Absenden** klicken.
