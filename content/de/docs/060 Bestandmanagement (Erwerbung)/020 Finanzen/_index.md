---
title: "📱Finanzen"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [by-folio, for-anwender, cat-berechtigungen, app-finanzen]
weight: 10
Description: "
    Quellen: [Folio](https://docs.folio.org/docs/acquisitions/finance/) <!-- & [GBV](https://info.gebev.de/pages/viewpage.action?pageId=839188622) -->
    "
---

Mit der App Finanzen können Fondsstrukturen erstellt und Geld verwaltet werden.

Definitionen der Begriffe, die in der App Finanzen verwendet werden:

* **Erwerbungsteams**. Eine zusätzliche Ebene, die zu den Erwerbungsdatensätzen hinzugefügt werden kann und die die Möglichkeit einer Person einschränkt, mit diesen Datensätzen zu interagieren, wenn sie nicht diesem Team zugewiesen wurde. Es können beispielsweise Erwerbungsteams erstellt werden, um die verschiedenen Bibliotheken in dem Bibliothekssystem zu repräsentieren. Die Teams werden von der Bibliothek in der App Einstellungen definiert und festgelegt. Weitere Informationen sind unter [Einstellungen > Erwerbungsteams]({{< ref "010 Einstellungen (Erwerbungsteams)_ Erwerbungsteam erstellen, bearbeiten, loeschen" >}}) zu finden.
* **Zugewiesener Betrag**. Der Geldbetrag, der einem Fonds zu Beginn eines Haushaltsjahres zugewiesen wird. Zusätzliches Geld kann auch während des Jahres zugewiesen werden.
* **Budget**. Ein Finanzdatensatz, der den für ein Haushaltsjahr innerhalb eines Fonds verfügbaren Geldbetrag beschreibt und eine Definition des zulässigen Ausgaben- und des zulässigen Prozentsatzes für die Bindung enthält. Transfers und Zuweisungstransaktionen werden gegen ein Budget durchgeführt. Einem Budget können Kostenarten zugewiesen werden.
* **Bindung**. Ein Geldbetrag, den die Bibliothek an einen Lieferanten aus dem Budget eines Fonds für bestellte Ressourcen, die in der Zukunft in Rechnung gestellt werden, zu zahlen verpflichtet ist.
* **Kostenart**. Eine fiskalische Einheit, die verwendet wird, um Transaktionen für einen bestimmten Zweck oder eine bestimmte Funktion innerhalb eines Fonds zu verfolgen. Optional, mandantenabhängig und kann einem oder mehreren Fonds zugewiesen werden. Wird bei der Fondsverteilung auf Auftrags- und Rechnungszeilen angewendet. Jeder Fonds kann mehrere Kostenarten unterstützen.
* **Haushaltsjahr**. Der zwölfmonatige Zeitraum, den die Bibliothek für die Verwaltung der Finanzen verwendet.
* **Fonds**. Eine fiskalische Einheit, die dazu dient, Transaktionen für einen allgemeinen Zweck oder eine Funktion innerhalb eines Etats zu verfolgen. Fonds sind nur mit einem einzigen Etat verbunden. Die Fondsinformationen bleiben von Jahr zu Jahr erhalten, da jedes Jahr neue Budgets für den Fonds erstellt werden.
* **Gruppe**. Eine Sammlung von einem oder mehreren Fonds, die in einer Gruppe zusammengefasst sind.
* **Etat**. Eine Sammlung von Fonds, die fiskalisch von der Sammlung von Fonds eines anderen Etats getrennt gehalten werden muss. Alle Fonds innerhalb eines Etats haben ein gemeinsames Verfahren beim Jahresübergang für das kommende Haushaltsjahr.
* **Netto-Transfers**. Geld, das während eines Haushaltsjahres zwischen Fonds übertragen wird.

## Berechtigungen

Die unten aufgeführten Berechtigungen ermöglichen die Interaktion mit der App Finanzen und legt fest, was in der App getan werden kann und was nicht. Personen können in der App Personen Berechtigungen zugewiesen werden. Wenn einer Person keine dieser Berechtigungen zugewiesen ist, kann sie die App Finanzen und alle damit verbundenen Informationen nicht sehen.

Finanzen-Berechtigungen:

* **Finanzen: Erwerbungsteams einem neuen Datensatz zuweisen**. (Finance: Assign acquisition units to new record)
    Mit dieser Berechtigung kann die Person einem Datensatz Erwerbungsteams zuweisen, wenn sie einen neuen Datensatz erstellt.
* **Finanzen: Zuweisungen erstellen**. (Finance: Create allocations)
    Mit dieser Berechtigung können Personen Zuweisungstransaktionen gegen Budgets erstellen. Muss die Berechtigung zum Anzeigen und Bearbeiten von Fonds und Budgets enthalten.
* **Finanzen: Transfers erstellen**. (Finance: Create transfers)
    Mit dieser Berechtigung können Personen Transfertransaktionen gegen Budgets erstellen. Muss die Berechtigung zum Anzeigen und Bearbeiten von Fonds und Budgets enthalten.
* **Finanzen: Jahresübergang durchführen**. (Finance: Execute fiscal year rollover)
    Diese Berechtigung erlaubt es Personen, einen Jahresübergang durchzuführen.
* **Finanzen: Finanzdatensätze exportieren**. (Finance: Export finance records)
    Diese Berechtigung ermöglicht es dem Personen, einen Export von Finanzdatensätzen für ein Etat durchzuführen.
* **Finanzen: Erwerbungsteams verwalten**. (Finance: Manage acquisition units.)
    Mit dieser Berechtigung können Personen bei der Bearbeitung eines Datensatzes die Zuordnung von Erwerbungsteams für den Datensatz ändern.
* **Finanzen: Bindung manuell auflösen**. (Finance: Manually release encumbrance)
    Mit dieser Berechtigung können Personen eine Bindung aus einem Fonds über die Aktion Bindung freigeben im Budgettransaktionsprotokoll freigeben.
* **Finanzen: Haushaltsjahr anzeigen**.  (Finance: View fiscal year)
    Mit dieser Berechtigung können Haushaltsjahr-Datensätze gesucht und angezeigt werden.
* **Finanzen: Fonds und Budget anzeigen**. (Finance: View fund and budget)
    Mit diesem Recht können Personen Fonds und Budgets durchsuchen und anzeigen.
* **Finanzen: Gruppe anzeigen**. (Finance: View group)
    Mit diesem Recht kann die Person Gruppen suchen und anzeigen.
* **Finanzen: Etat anzeigen**. (Finance: View ledger)
    Diese Berechtigung ermöglicht es Personen, Etats zu suchen und einzusehen.
* **Finanzen: Haushaltsjahr anzeigen und bearbeiten**. (Finance: View, edit fiscal year)
    Mit dieser Berechtigung kann die Person Haushaltsjahre anzeigen und bearbeiten.
* **Finanzen: Fonds und Budget anzeigen und bearbeiten**. (Finance: View, edit fund and budget)
    Mit dieser Berechtigung können Personen Fonds und Budgets anzeigen und bearbeiten.
* **Finanzen: Gruppe anzeigen und bearbeiten**. (Finance: View, edit group)
    Mit diesem Recht kann die Person Gruppen anzeigen und bearbeiten.
* **Finanzen: Etat anzeigen und bearbeiten**. (Finance: View, edit ledger)
    Mit dieser Berechtigung können Personen Etats anzeigen und bearbeiten.
* **Finanzen: Haushaltsjahr anzeigen, bearbeiten, erstellen**. (Finance: View, edit, create fiscal year)
    Mit dieser Berechtigung kann die Person Haushaltsjahre anzeigen, bearbeiten und erstellen.
* **Finanzen: Fonds und Budget anzeigen, bearbeiten und erstellen**. (Finance: View, edit, create fund and budget)
    Mit dieser Berechtigung kann die Person Fonds und Budgets anzeigen, bearbeiten und erstellen.
* **Finanzen: Gruppe anzeigen, bearbeiten, erstellen**. (Finance: View, edit, create group)
    Mit diesem Recht kann die Person Gruppen anzeigen, bearbeiten und erstellen.
* **Finanzen: Etat anzeigen, bearbeiten und erstellen**. (Finance: View, edit, create ledger)
    Mit diesem Recht kann die Person Etats anzeigen, bearbeiten und erstellen.
* **Finanzen: Haushaltsjahr anzeigen, bearbeiten, löschen**. (Finance: View, edit, delete fiscal year.)
    Mit dieser Berechtigung kann die Person das Haushaltsjahr anzeigen, bearbeiten und löschen.
* **Finanzen: Fonds und Budget anzeigen, bearbeiten und löschen**. (Finance: View, edit, delete fund and budget)
    Mit dieser Berechtigung kann die Person Fonds und Budgets anzeigen, bearbeiten und löschen.
* **Finanzen: Gruppe anzeigen, bearbeiten, löschen**. (Finance: View, edit, delete group)
    Mit diesem Recht kann die Person Gruppen anzeigen, bearbeiten und löschen.
* **Finanzen: Etat anzeigen, bearbeiten und löschen**. (Finance: View, edit, delete ledger)
    Mit dieser Berechtigung kann die Person die Etats ansehen, bearbeiten und löschen.
