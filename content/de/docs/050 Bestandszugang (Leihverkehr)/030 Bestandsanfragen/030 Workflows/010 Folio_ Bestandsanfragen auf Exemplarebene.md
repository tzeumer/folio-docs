---
title: "Folio: Bestandsanfragen auf Exemplarebene"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [by-folio, for-anwender, app-bestandsanfragen, cat-workflows, meta-feedback]
weight: 10
Description: "
    Quellen: [Folio](https://docs.folio.org/docs/access/requests/requests/#item-level-requesting) & [GBV](https://info.gbv.de/display/FOLIOGBVEXTERN/Folio:+Bestandsanfragen+auf+Exemplarebene)
    "
---

## Bestandsanfrage auf Exemplarebene erstellen

Bibliotheksmitarbeitende erstellen Bestandsanfragen in der Bestandsanfragen-App. Die Bestandsanfrage können auch von einem Personendatensatz in Personen oder einem Exemplardatensatz in Katalog aus gestartet werden. Diese Apps leiten dann zur Bestandsanfragen-App weiter, um die Anfrage zu erstellen.

Bestandsanfragen werden durch Ausleihregeln und Exemplarstatus gesteuert. Einige Exemplarstatus können überhaupt nicht angefordert werden; einige Exemplarstatus erlauben nur Vormerkungen und Rückrufe. Weitere Informationen sind unter [Grundlagen der Plattform > Exemplarstatus](https://info.gbv.de/display/FOLIOGBVEXTERN/Exemplarstatus) zu finden.

1.  In der Ansicht **Bestandsanfrage** die Option **Aktionen > Neu** wählen.
2.  Im Feld **Exemplarinformationen** entweder den Barcode des angeforderten Exemplars scannen oder den Barcode eingeben und auf **Eingabe** klicken. Das Exemplar wird der Bestandsanfrage hinzugefügt und die Informationen zum Exemplar werden angezeigt.
3.  Den **Bestandsanfragetyp** wählen. Welche Optionen angezeigt werden, hängt vom Status des Exemplars ab, das angefragt wird.
4.  Optional: Ein **Ablaufdatum Bestandsanfrage** eingeben. Wenn die Bestandsanfrage zum gewählten Datum noch offen ist, wird sie geschlossen und ihr Status ändert sich in Geschlossen - unerfüllt.
5.  Optional: Einen **Kommentar Benutzer/-in** eingeben. Wenn die Person das Exemplar zum Beispiel sofort benötigt, kann dies hier vermerkt werden. Die Kommentare werden im CSV-Bericht und auf den Entnahmezetteln angezeigt.
6.  Im Feld **Informationen über Benutzer/in** entweder den Barcode der Person scannen oder den Barcode eingeben und auf **Eingabe** klicken.
7.  Wenn der Barcode der Person nicht verfügbar ist, auf **Personensuche** klicken, um nach der Person zu suchen:
    1.  Im Dialogfeld **Person auswählen** nach der Person suchen.
    2.  Wenn die Person gefunden wurde, diese aus der Ergebnisliste der Personensuche auswählen. Sie wird auf in der Bestandsanfrage angewendet und  ihre Informationen werden angezeigt.
8.  Die **Bereitstellungspräferenz** wählen.
9.  Die **Abholservicestelle** oder die **Lieferadresse** wählen, je nachdem, was im vorherigen Schritt ausgewählt wurde.
10.  Auf **Speichern & schließen** klicken. Die Bestandsanfrage wird gespeichert und die Ansicht mit den Details der Anfrage wird angezeigt. Die Person erhält eine E-Mail-Benachrichtigung, dass ihre Bestandsanfrage bei der Bibliothek eingegangen ist, sofern diese Benachrichtigung konfiguriert wurde.

## Bestandsanfrage auf Exemplarebene bearbeiten

Es können nur offene Bestandsanfragen bearbeitet werden. Sobald eine Bestandsanfrage geschlossen ist, kann sie nicht mehr bearbeitet werden.

1.  [Die Bestandsanfrage suchen](https://info.gbv.de/display/FOLIOGBVEXTERN/Folio%3A+Bestandsanfragen+suchen), die bearbeitet werden soll.
2.  In der Ansicht **Bestandsanfrage** die **Aktionen > Bearbeiten** wählen.
3.  Die Bestandsanfrage bearbeiten.
4.  Auf **Speichern & schließen** klicken. Die Bestandsanfrage wird aktualisiert.

## Bestandsanfrage auf Exemplarebene duplizieren

Jede offene Bestandsanfrage kann dupliziert werden, solange die Anfrage, die durch die Duplizierung erstellt wird, eine andere anfordernden Person hat.

1.  [Die Bestandsanfrage suchen](https://info.gbv.de/display/FOLIOGBVEXTERN/Folio%3A+Bestandsanfragen+suchen), die duplizieren werden soll.
2.  In der Ansicht **Bestandsanfrage** die **Aktionen > Duplizieren** wählen. Es erscheint ein Fenster **Neue Anfrage** mit denselben Exemplarinformationen, Bestellinformationen und Informationen zur anfordernden Person der Anfrage, die duplizieren werden soll.
3.  Die Bestandsanfrage bearbeiten, bevor die Anfrage abgeschickt wird.
4.  Eine **Abholservicestelle** auswählen.
5.  Auf **Speichern & schließen** klicken. Die duplizierte Anfrage wird in der Ansicht Bestandsanfrage angezeigt.

## Bestandsanfrage auf Exemplarebene auf ein anderes Exemplar der selben Instanz umhängen

Eine Bestandsanfrage kann von einem Exemplar auf ein anderes Exemplar auf derselben Instanz umgehängt werden. Dies kann gewünscht sein, wenn ein Exemplar einer Bestandsanfrage verloren geht oder wenn die Warteschlangen für Anfragen optimiert werden sollen.

Hinweis: Wenn eine Bestandsanfrage auf ein Exemplar umgehängt wird, das zuvor nicht zurückgerufen wurde, wird die Ausleihe zurückgerufen - die Person erhält eine Rückrufbenachrichtigung, sofern konfiguriert, und das Fälligkeitsdatum der Ausleihe wird je nach Ausleihrichtlinie verkürzt oder verlängert.

1.  [Die Bestandsanfrage suchen](https://info.gbv.de/display/FOLIOGBVEXTERN/Folio%3A+Bestandsanfragen+suchen), die verschoben werden soll.
2.  In der Ansicht **Bestandsanfrage** die **Aktionen > Anfrage** verschieben wählen.
3.  Im Fenster **Exemplar auswählen** das Exemplar wählen, in das die Anfrage umgehängt werden soll. Wenn der aktuelle Anfragetyp nicht zulässig ist, erscheint das Dialogfeld Aktueller Anfragetyp für ausgewähltes Exemplar nicht zulässig.
4.  Auf **Bestätigen** klicken, damit die Bestandsanfrage umgehängt werden kann. Es erscheint eine Bestätigungsmeldung und die Anfrage wird unter dem ausgewählten Exemplar angezeigt.

