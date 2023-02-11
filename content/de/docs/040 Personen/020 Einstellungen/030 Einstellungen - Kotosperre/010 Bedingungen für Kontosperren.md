---
title: "Bedingungen für Kontosperren"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [by-folio, for-admin, cat-einstellungen, app-personen]
weight: 10
Description: "
    Quellen: [Folio](https://docs.folio.org/docs/settings/settings_users/settings_users/#settings--users--conditions) & [GBV](https://info.gbv.de/pages/viewpage.action?pageId=841809962)
    "
---

Automatische Personensperren ermöglichen es der Bibliothek, Sperrgrenzen festzulegen, die automatisch durchgesetzt werden. Die Sperrgrenzen werden in Echtzeit angewendet und in denselben Bereichen wie manuelle Kontosperren angezeigt. Personen können automatisch für das Ausleihen, Verlängern und/oder Bestandsanfragen gesperrt werden.

Automatische Personensperren werden in der App "Personen" im Abschnitt "Kontosperren" eines Personendatensatzes angezeigt. Je nachdem, welche Aktionen gesperrt sind, werden die Sperren auch in Apps angezeigt. In der App Ausleihe nach der Eingabe des Barcodes einer Person oder der Suche nach einer Person oder nach dem Scannen eines Barcodes für ein Exemplar. In der App Ausleihe für Personen, wenn Sie ein Exemplar verlängern möchten. Und in der App Bestandsanfragen nach der Suche nach einem Barcode einer Person.

Die Sperre wird automatisch aufgehoben, sobald die Person das Limit unterschreitet.

Hinweis: Damit die automatische Personensperren funktioniert, müssen Bedingungen und Grenzwerte festgelegt werden.

Die Bedingungen legen fest, welche Aktionen Personen nicht mehr erlaubt sind, sobald sie die für ihre Personengruppe unter [Einstellungen > Personen > Grenzwerte für Kontosperren](https://info.gbv.de/pages/viewpage.action?pageId=841809967) festgelegten Grenzen erreicht haben.

Dies sind alle Kategorien, für die Bedingungen und Grenzen festlgelehgt werden können:

-   Maximale Anzahl der ausgeliehener Exemplare
    -   (Ausleihmaximum)
-   Maximale Anzahl verlorener Exemplare
    -   (Verlustmaximum)
-   Maximale Anzahl überfälliger Exemplare
    -   (Ausleihfristüberschreitungen)
-   Maximale Anzahl überfälliger Vormerkungen
    -   (Ausleihfristüberschreitungen (Vormerkungen))
-   Maximale ausstehende Forderungen
    -   (Forderungslimit)
-   Maximalzahl überfällige Tage bei Vormerkungen

## Kontosperrbedingungen konfigurieren

1.  Im Bereich **Bedingungen für Kontosperren** die Bedingung auswählen, die konfigurieren werden soll.
2.  Im ausgewählten Bedingungsfenster die Aktion(en) auswählen, die bei Überschreitung der definierten Grenzwerte erfolgen soll(en): **Ausleihen sperren** und/oder **Verlängerungen sperren** und/oder **Bestandsanfragen sperren**.
3.  Eine **Nachricht, die angezeigt werden soll** eingeben (erforderlich).
4.  Auf **Speichern** klicken. Eine Bestätigungsmeldung wird angezeigt, und die Sperrbedingung wird gespeichert.

## Kontosperrbedingungen bearbeiten

1.  Im Bereich **Bedingungen für Kontosperren** die Bedingung auswählen, die bearbeitet werden soll.
2.  Im ausgewählten Bedingungsfenster Änderungen an der Bedingung vornehmen.
3.  Auf **Speichern** klicken. Es wird eine Bestätigungsmeldung angezeigt, und die Sperrbedingung wird gespeichert.

## Kontosperrbedingungen entfernen

1.  Im Bereich **Bedingungen für Kontosperren** die Bedingung auswählen, die entfernt werden soll.
2.  Im Bereich der ausgewählten Bedingung alle Sperren und Meldungen entfernen.
3.  Auf **Speichern** klicken. Es wird eine Bestätigungsmeldung angezeigt, und die Sperrbedingung wird gespeichert.
