---
title: "Rechnung freigeben"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [app-rechnungen, by-folio, cat-workflows, for-anwender]
weight: 90
Description: "
    Quellen: [Folio](https://docs.folio.org/docs/acquisitions/invoices/#approving-an-invoice) & [GBV](https://info.gbv.de/display/FOLIOGBVEXTERN/Folio:+Rechnung+freigeben)
    "
---

Rechnungen müssen genehmigt werden, bevor die Zahlungsbeträge als zur Zahlung erwartet gelten und damit Belege erstellt werden können. Das Freigeben einer Rechnung ist möglich, wenn:

-   Der Rechnungsstatus ist Offen oder Überprüft.
-   Der Rechnung sind ein oder mehrere Rechnungsposten hinzugefügt worden.
-   Das Benutzerkonto die **Berechtigung Rechnung freigeben** enthält.
-   Wird ein **Gesamtsumme fixieren-**Wert eingegeben, müssen alle Rechnungsposten und Zusatzkosten diesem "Gesamtsumme fixieren"-Betrag entsprechen. Siehe Informationen zur [Rechnung > Gesamtsumme fixieren](https://info.gbv.de/display/FOLIOGBVEXTERN/Folio%3A+Rechnung+erstellen) für Informationen über die Gesamtsumme fixieren.

Das Freigeben einer Rechnung löst die folgenden Systemaktionen aus:

-   Sobald eine oder mehrere Rechnungen, die mit einem Bestellposten verbunden sind, "Freigegeben" wurden, wird der Zahlungsstatus des Bestellpostens auf "Teilweise bezahlt" geändert.
-   Es werden Belege und Vorgänge für ausstehende Zahlungen erstellt. Belege sind ein Mechanismus zur Bereitstellung der für die Zahlung von Rechnungen erforderlichen Informationen und können in ein externes Zahlungssystem exportiert werden. Jede Rechnung erzeugt einen einzigen Beleg, auf dem alle Fondsgebühren nach der externen Kontonummer des Fonds gruppiert sind. Weitere Informationen zum Exportieren von Belegen sind unter [Exportieren von Belegen](https://info.gbv.de/display/FOLIOGBVEXTERN/Folio%3A+Export+von+Belegen) zu finden.

Um eine Rechnung freizugeben, folgendermaßen vorgehen:

-   [Die Rechnung suchen](https://info.gbv.de/display/FOLIOGBVEXTERN/Folio%3A+Rechnung+suchen), die freigegeben werden soll und sie auswählen.
-   In der Ansicht **Rechnungsnummer des Lieferanten** auf **Aktionen > Freigeben** klicken.
-   Im Dialogfeld **Rechnung genehmigen** auf **Freigegeben** klicken. Es wird eine Bestätigungsmeldung angezeigt und die Rechnung wird freigegeben.
