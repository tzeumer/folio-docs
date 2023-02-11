---
title: "Instanzabgleich"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [by-folio, for-admin, cat-einstellungen, app-bestellungen, meta-fehler_inhalt, meta-gemeldet_docsfolioorg]
weight: 10
Description: "
    Quellen: [Folio](https://docs.folio.org/docs/settings/settings_orders/settings_orders/ ) & [GBV](https://info.gbv.de/display/FOLIOGBVEXTERN/Einstellungen+(Bestellungen):+Instanzabgleich)
    "
---

Wenn der Instanzabgleich aktiv ist, werden Bestellposten, die laut Einstellung eine Instanz erstellen sollen, aber nicht manuell mit einem Instanzdatensatz verknüpft sind, als Instanz angezeigt. Zuerst werden die Instanzen durchsucht, um eine Übereinstimmung mit einer oder mehreren der Produkt-IDs zu finden, die im Bestellposten angegeben sind. Wenn eine Produkt-ID gefunden wird, wird diese Instanz mit dem Bestellposten verknüpft und das System erstellt KEINE neue Instanz für diesen Bestellposten. Wenn keine Übereinstimmungen gefunden werden, erstellt das System einen neuen Instanzdatensatz und verknüpft den Bestellposten mit dieser Instanz.

**Instanzabgleich deaktivieren** wählen, wenn gewünscht.
