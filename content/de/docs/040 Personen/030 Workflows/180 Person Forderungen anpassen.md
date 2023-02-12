---
title: "Person Forderungen anpassen"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [app-personen, by-folio, cat-worklfows, for-anwender, meta-Workflow-Sammlung]
weight: 180
Description: "
    Quellen: [Folio](https://docs.folio.org/docs/users/#managing-loans-and-feefines-for-patrons) & [GBV](https://info.gbv.de/display/FOLIOGBVEXTERN/Folio:+Person+Forderungen+anpassen)
    "
---

{{% pageinfo %}}
Hinweis: Es sind eigentlich mehrere einzelne Workflows. Ob einzeln oder wie hier zusammengefasst besser ist, ist noch unentschieden.
{{% /pageinfo %}}

Mitarbeitende mit den entsprechenden Berechtigungen können Forderungen für die Konten von Personen verwalten. Dies umfasst die Anzeige von Forderungsinformationen, die Erstellung manueller Forderungen, die Annahme von Zahlungen, den Erlass einer Forderung und die Rückerstattung einer Forderung.

## Forderung anlegen

Eine Bibliothek muss die Forderungseinstellungen konfigurieren, bevor sie Forderungen von Personen erheben kann. Weitere Informationen sind unter [Einstellungen > Personen > Forderungseigentümer/-in](https://info.gbv.de/pages/viewpage.action?pageId=841809942) und [Einstellungen > Personen > Manuelle Kosten](https://info.gbv.de/display/FOLIOGBVEXTERN/Einstellungen+%28Personen%29%3A+Manuelle+Kosten).

1.  Via [Folio: Personen suchen](https://info.gbv.de/display/FOLIOGBVEXTERN/Folio%3A+Personen+suchen), die Personendaten finden, und auswählen.
2.  Im Bereich **Personendatensatz** bei Bedarf das Akkordeon **Forderungen** erweitern.
3.  Auf **Forderung erstellen** klicken.
4.  Im Fenster **Neue Forderung** den **Forderungseigentümer/-in** wählen.
5.  **Art der Forderung** wählen.
6.  Im Feld **Forderungsbetrag** kann eine von drei Möglichkeiten gewählt werden:
    1.  Beibehalten des Standardforderungsbetrags, wenn einer für die Art der Forderung eingetragen ist.
    2.  Anpassung des Standardforderungsbetrags, wenn er für die Art der Forderung eingetragen ist. Wenn dieser nicht ausgefüllt wurde, einen Forderungsbetrag angeben,
7.  Optional: Um die Forderung mit einem Exemplar zu verknüpfen, den Barcode des Exemplars scannen oder ihn in das Feld **Exemplarinformationen** eingeben und auf **Eingabe** klicken.
8.  Optional: **Zusätzliche Informationen für das Personal** in das Feld eingeben.
9.  Auf **Nur einbuchen** klicken, um die Forderung auf das Konto der Person anzuwenden. Mitarbeitende mit den entsprechenden Berechtigungen können die Forderung erstellen und sofort die Zahlung akzeptieren, indem sie auf **Einbuchen und bezahlen** klicken.

## Forderung begleichen

1.  Via [Folio: Personen suchen](https://info.gbv.de/display/FOLIOGBVEXTERN/Folio%3A+Personen+suchen), die Personendaten finden, und auswählen.
2.  Im Bereich **Personendatensatz** bei Bedarf das Akkordeon **Forderungen** erweitern.
3.  **(Anzahl) offener Forderungen** wählen, um die offenen Forderungen der Person anzuzeigen.
4.  Das Modal "**Forderungen**" wird geöffnet. Auf die Forderung klicken, für die die Zahlung akzeptiert werden soll.
5.  Das Modal **Forderungsdetails** wird geöffnet. Auf **Aktionen > Bezahlen** klicken.
6.  Das Modal "**Forderungen begleichen**" wird geöffnet. Den Zahlungsbetrag eingeben (erforderlich). FOLIO kann vollständige und teilweise Zahlungen verarbeiten. Wird eine Teilzahlung akzeptiert, berechnet das Modal den verbleibenden Betrag.
7.  Die **Zahlungsmethode** wählen (erforderlich).
8.  **Transaktionsinformationen** und zusätzliche Informationen für das Personal eingeben. Das Feld **Zusätzliche Informationen für das Personal** kann erforderlich sein, wenn die Bibliothek diese Option konfiguriert hat.
9.  Auf **Bezahlen** und dann auf **Bestätigen** klicken .

Das Modal wird geschlossen, und die Seite mit den **Forderungsdetails** wird mit aktualisiert.

## Forderung erlassen

Mitarbeitende mit entsprechenden Berechtigungen können eine Forderung teilweise oder vollständig erlassen (oder: ausbuchen).

1.  Via [Folio: Personen suchen](https://info.gbv.de/display/FOLIOGBVEXTERN/Folio%3A+Personen+suchen), die Personendaten finden, und auswählen.
2.  Im Bereich **Personendatensatz** bei Bedarf das Akkordeon **Forderungen** erweitern.
3.  **(Anzahl) offener Forderungen** wählen, um die offenen Forderungen der Person anzuzeigen.
4.  Das Modal "**Forderungen**" wird geöffnet. Auf die Forderung klicken, für die die Zahlung erlassen werden soll.
5.  Das Modal **Forderungsdetails** wird geöffnet. Auf **Aktionen > Erlassen** klicken.
6.  Das Modal "**Forderungen erlassen**" wird geöffnet. Den zu erlassenden Betrag eingeben (erforderlich). Es können einen Teil oder den gesamten Betrag der Forderung erlassen werden. Wird nur ein Teil erlassen, berechnet das Modal den verbleibenden Betrag.
7.  Den Grund für den Verzicht wählen (erforderlich) und zusätzliche Informationen für das Personal eingeben. Das Feld **Zusätzliche Informationen für das Personal** kann erforderlich sein, wenn die Bibliothek diese Option konfiguriert hat.
8.  Auf **Verzicht** und dann auf **Bestätigen** klicken.

Das Modal wird geschlossen, und die Seite mit den **Forderungsdetails** wird mit aktualisiert.

## Forderung erstatten

Mitarbeitende mit entsprechender Berechtigung können eine Forderung ganz oder teilweise erstatten. Die Zahlungsmethode muss Erstattungen zulassen.

1.  Via [Folio: Personen suchen](https://info.gbv.de/display/FOLIOGBVEXTERN/Folio%3A+Personen+suchen), die Personendaten finden, und auswählen.
2.  Im Bereich **Personendatensatz** bei Bedarf das Akkordeon **Forderungen** erweitern.
3.  **Alle Forderungen anzeigen** wählen, um die offenen Forderungen der Person anzuzeigen.
4.  Das Modal "**Forderungen**" wird geöffnet. Auf die Forderung klicken, für die die Zahlung erstattet werden soll. Sie kann offen oder geschlossen sein.
5.  Das Modal **Forderungsdetails** wird geöffnet. Auf **Aktionen > Rückerstattung** klicken.
6.  Das Modal "**Forderungen zurückerstatten**" wird geöffnet. Den zu erstattenden Betrag eingeben (erforderlich). Es können einen Teil oder den gesamten Betrag der Forderung erstattet werden. Wird nur ein Teil erstattet, berechnet das Modal den verbleibenden Betrag.
7.  Den **Erstattungsgrund** wählen (erforderlich) und zusätzliche Informationen für das Personal eingeben. Das Feld **Zusätzliche Informationen für das Personal** kann erforderlich sein, wenn die Bibliothek diese Option konfiguriert hat.
8.  Auf **Erstattung** und dann auf **Bestätigen** klicken.

Das Modal wird geschlossen, und die Seite mit den **Forderungsdetails** wird mit aktualisiert.

## Forderung stornieren

Mitarbeitende mit den entsprechenden Berechtigungen können eine Forderung als Fehler kennzeichnen; dies hat die Stornierung der Forderung zur Folge.

Eine Stornierung kann nur auf eine Forderung im Status "Ausstehend" angewendet werden. Die Kennzeichnung einer Forderung als Fehler ist für den Fall gedacht, dass die Forderung aufgrund eines Personal- oder Systemfehlers erhoben wurde und daher nicht bezahlt werden sollte.

1.  Via [Folio: Personen suchen](https://info.gbv.de/display/FOLIOGBVEXTERN/Folio%3A+Personen+suchen), die Personendaten finden, und auswählen.
2.  Im Bereich **Personendatensatz** bei Bedarf das Akkordeon **Forderungen** erweitern.
3.  **Alle Forderungen anzeigen** wählen, um die offenen Forderungen der Person anzuzeigen.
4.  Das Modal "**Forderungen**" wird geöffnet. Auf die Forderung klicken, für die die Zahlung storniert werden soll. Sie kann offen oder geschlossen sein.
5.  Das Modal **Forderungsdetails** wird geöffnet. Auf **Aktionen > Fehler** klicken.
6.  Das Modal "**Bestätigung der Stornierung**" wird geöffnet.
7.  Den **Stornierung****sgrund** wählen (erforderlich) und zusätzliche Informationen für das Personal eingeben. Das Feld **Zusätzliche Informationen für das Personal** kann erforderlich sein, wenn die Bibliothek diese Option konfiguriert hat.
8.  Auf **Bestätigen** klicken.

Das Modal wird geschlossen, und die Seite mit den **Forderungsdetails** wird mit aktualisiert.
