---
title: "Organisation als Lieferanten anlegen"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [app-organisationen, by-folio, cat-workflows, for-anwender]
weight: 20
Description: "
    Quellen: [Folio](https://docs.folio.org/docs/acquisitions/organizations/#creating-a-vendor) & [GBV](https://info.gbv.de/display/FOLIOGBVEXTERN/Folio:+Organisation+als+Lieferanten+anlegen)
    "
---

1.  In der Ansicht **Organisationen** auf **Neu** klicken.
2.  Im Fenster **Organisation erstellen** im Abschnitt **Übersicht** die Checkbox **Lieferant** markieren. Die Abschnitte für Lieferanten werden angezeigt.
3.  Mit dem Ausfüllen des Abschnitts Übersicht fortfahren. Die Abschnitte Kontaktinformationen, Kontaktpersonen, Schnittstelle, Lieferanteninformationen, Lieferantenbedingungen und Konten ausfüllen. Weitere Informationen zu den Feldern und Aktionen, die in diesen Abschnitten verfügbar sind, sind in den Abschnittsbeschreibungen weiter unten zu finden.
4.  Sobald alle gewünschten Informationen über den Lieferanten eingegeben sind, auf **Speichern & schließen** klicken. Der Lieferant wird gespeichert und der Ansicht Organisationen hinzugefügt.
5.  In der Ansicht des neu erstellten Organisationsdatensatzes sind die Akkordeonabschnitte zum Hinzufügen von Notizen und Integrationsdetails zu sehen. Weitere Informationen sind unter [Organisation Anmerkung hinzufügen]({{< ref "090 Organisation Anmerkung hinzufuegen" >}}) und [Organisation (Lieferant) EDI-Verbindung hinzufügen]({{< ref "020 Organisation als Lieferanten anlegen" >}}) zu finden.

## Übersicht

Weitere Informationen unter [Übersicht]({{< ref "010 Organisation als Organisation anlegen" >}}).

## Kontaktinformationen

Weitere Informationen unter [Kontaktinformationen]({{< ref "010 Organisation als Organisation anlegen" >}}).

## Kontaktpersonen

Weitere Informationen unter [Kontaktpersonen]({{< ref "010 Organisation als Organisation anlegen" >}}).

## Schnittstellen

Weitere Informationen unter [Schnittstellen]({{< ref "010 Organisation als Organisation anlegen" >}}).

## Lieferanteninformationen

Die Informationen, die unter Lieferanteninformationen eingegeben werden, legen einige der Standardwerte fest, die angezeigt werden, wenn der Lieferanten für eine Bestellung oder Rechnung verwendet wird.

* **Zahlungsart**. Die Zahlungsart, die als Standardzahlungsart für den Lieferanten auf einer Rechnung angegeben werden soll. Weitere Informationen sind unter Rechnungen > Erweiterte Informationen zu finden.
* **Währungen**. Die von dem Lieferanten akzeptierten Währungen.
* **Erwartetes Aktivierungsintervall**. Der Standard-Aktivierungszeitraum für den Lieferanten, in Tagen. Hinweis: Das Intervall, das hier eingegeben wird, wird im Feld Aktivierungsfrist im Abschnitt E-Ressourcen-Details einer mit dem Lieferanten verbundenen Bestellzeile verwendet. Wenn das Intervall z.B. auf 365 eingestellt wird, wird das Feld Fälligkeit der Aktivierung mit dem Datum gefüllt, das ein Jahr nach dem Erstellungsdatum der Bestellzeile liegt.
* **Erwartetes Rechnungsintervall**. Das Standard-Rechnungsintervall für den Lieferanten, in Tagen. Derzeit wird diese Information nicht auf Rechnungen angezeigt.
* **Forderungsintervall**. Das Standard-Forderungsintervall für den Lieferanten, in Tagen.
* **Erwartetes Eingangsintervall**. Der Standardzeitraum, in dem bestellte Exemplare vom Lieferanten eingehen, in Tagen.
* **Rabatt in Prozent**. Der mit dem Lieferanten ausgehandelte Rabatt als Prozentwert. Wenn eine Bestellzeile für eine Bestellung beim Lieferanten erstellt wird, wird dieser Wert als Standardwert im Feld Rabatt angezeigt.
* **Aktivierungsintervall für Verlängerung**. Das Standardintervall für die Aktivierung der Erneuerung für diesen Lieferanten in Tagen.
* **Abonnementintervall**. Der Standard-Abonnementzeitraum für den Lieferanten in Tagen.
* **An Haushaltssystem exportieren**. Um anzugeben, dass Rechnungen für den Lieferanten Belegsätze für den Export in ein externes Buchhaltungssystem erstellen sollen, die Checkbox An Haushaltssystem exportieren markieren. Beim Erstellen einer Rechnung für den Lieferanten legt der Wert im Datensatz Organisation den Standardwert für das Feld Export in die Buchhaltung fest.

## Steuer

Die Informationen, die unter Steuer eingegeben werden, bestimmen die Standardwerte, die angezeigt werden, wenn der Lieferanten auf eine Bestellung angewendet wird.

1.  **Steuer-ID.** Die Steueridentifikationsnummer für den Lieferanten. Sie wird auch als  Umsatzsteuer-Identifikationsnummer  (USt ID) bezeichnet und dient zur Identifizierung eines Unternehmens.
2.  **Steuersatz**. Der Standardsteuersatz für den Lieferanten. Für Lieferanten, die mehrwertsteuerpflichtig sind, kann der Prozentwert hier als Referenz gespeichert werden.
3.  **Mehrwertsteuerpflichtig** (Umsatzsteuerpflichtig). Um anzugeben, dass der Lieferant mehrwertsteuerpflichtig ist, die Checkbox Mehrwertsteuerpflichtig markieren.

## Lieferantenbedingungen

Lieferantenbedingungen sind die Zusammenfassung einer Vereinbarung mit dem Lieferanten. Die Vereinbarungen können sich auf Erwerbung, Lieferungen oder E-Ressourcen beziehen. Die hier eingegebenen Werte erscheinen nicht in Bestellungen oder Rechnungsdatensätzen.

Hinweis: Das Hinzufügen von Lieferantenbedingungen ist optional, aber wird auf Hinzufügen geklickt, muss ein Namen hinzugefügt oder die Lieferantenbedingungen gelöscht werden, um den Organisationsdatensatz zu speichern.

### Lieferantenbedingungen hinzufügen

1.  Auf **Hinzufügen** klicken.
2.  Den **Namen** der Bedingung in das Feld eingeben.
3.  Optional: In das Feld den **Rabatt %** eingeben oder auswählen.
4.  Optional: Eine **URL** in das Feld eingeben.
5.  Optional: In das Feld **Notizen** zum Vertrag eingeben.
6.  Die Schritte 1-5 je nach Bedarf wiederholen. Die Bedingungen werden gespeichert, sobald der Lieferant gespeichert wird.

### Lieferantenbedingungen löschen

1.  Die Lieferantenbedingungen suchen, die gelöscht werden soll.
2.  Das **Mülleimersymbol** klicken. Der Begriff wird entfernt und ist gelöscht, sobald der  Lieferant gespeichert wird.

## Konten

Der Bereich Konten beschreibt die Konten der Bibliothek bei einem Lieferanten, der für die Bestellung von Materialien verwendet wird.

Hinweis: Das Hinzufügen eines Kontos ist optional, aber wird auf Hinzufügen geklickt, müssen die erforderlichen Felder ausgefüllt oder das Konto gelöscht werden, um den Organisationseintrag zu speichern.

### Konto hinzufügen

1.  Auf **Hinzufügen** klicken.
2.  Den **Namen** in das Feld eingeben.
3.  Die **Kundennummer** in das Feld eingeben. Diese Nummer wird in der Regel vom Lieferanten vergeben. Hinweis: Die hier eingegebene  Kundennummer erscheint als Standardwert auf allen Bestellungen oder Rechnungen für den Lieferanten. Sind in diesem Bereich mehrere Konten eingerichtet, wird die erste Kontonummer als Standardwert auf Bestellungen und Rechnungen angezeigt, aber es kann die entsprechende Nummer aus einer Dropdown-Liste ausgewählt werden, die alle mit dem Lieferanten verbundenen Kontonummern enthält.
4.  Optional: Eine **Beschreibung** des Kontos in das Feld eingeben.
5.  Optional: Den **Buchhaltungscode** in das Feld eingeben.
6.  Optional: Die **Zahlungsart** aus der Dropdown-Liste wählen.
7.  Den **Status** des Kontos aus der Dropdown-Liste wählen.
8.  Optional: Die **Kontakt**\-Informationen in das Feld eingeben.
9.  Optional: Den **Bibliothekscode** in das Feld eingeben. Dies ist der von der Bibliothek vergebene Code für das Konto beim Lieferanten.
10.  Optional: Den **EDI-Code Bibliothek** in das Feld eingeben.
11.  Optional: In das Feld **Notizen** zum Konto eingeben.
12.  Optional: Beliebige **Erwerbungsteams** aus der Dropdown-Liste auswählen. Weitere Informationen zu Erwerbungsteams sind unter [Einstellungen > Erwerbungsteams]({{< ref "010 Einstellungen (Erwerbungsteams)_ Erwerbungsteam erstellen, bearbeiten, loeschen" >}}) zu finden.
13.  Die Schritte 1-13 nach Bedarf wiederholen. Konten werden gespeichert, sobald der Lieferant gespeichert wird.

### Konto löschen

1.  Das Konto suchen, das gelöscht werden soll.
2.  Auf das **Mülleimersymbol** klicken. Das Konto wird entfernt und ist gelöscht, sobald der Lieferant gespeichert wird.
