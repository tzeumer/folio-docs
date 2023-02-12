---
title: "Person Ausleihen anpassen"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [app-personen, by-folio, cat-worklfows, for-anwender]
weight: 160
Description: "
    Quellen: [Folio](https://docs.folio.org/docs/users/#managing-loans-and-feefines-for-patrons) & [GBV](https://info.gbv.de/display/FOLIOGBVEXTERN/Folio:+Person+Ausleihen+anpassen)
    "
---

Im Ausleihbereich einer Person können Mitarbeitende mit den entsprechenden Berechtigungen eine Ausleihe für eine Person verlängern, das Fälligkeitsdatum ändern, die Rückgabe des Exemplars markieren oder das Exemplar für verloren erklären.

## Ausleihen verlängern

Um eine oder mehrere Ausleihen für ein Person zu verlängern:

1.  Im Bereich **Personendatensatz** bei Bedarf das Akkordeon **Ausleihen** erweitern.
2.  Auf **Aktuelle Ausleihen** klicken.
3.  Die Checkbox auf der linken Seite des Ausleihfensters verwenden, um die entsprechende(n) Ausleihe(n) auszuwählen.
4.  Auf die Schaltfläche **Verlängern** in der oberen rechten Ecke des Fensters Ausleihen klicken.

Wenn die Verlängerung erfolgreich war, erscheint eine grüne Erfolgsmeldung in der unteren rechten Ecke. Das neue Fälligkeitsdatum kann früher als zu erwarten sein, wenn das normale Fälligkeitsdatum nach dem Ablauf des Kontos einer Person liegt. Wenn die Verlängerung nicht erfolgreich war, erscheint eine Pop-up-Meldung. Mit der entsprechenden Berechtigungen, kann im Pop-up-Fenster **Verlängern durch spezielle Zustimmung** gewählt werden, um die Ausleihe trotzdem zu verlängern.

Alternativ können Ausleihen auch verlängert werden, indem in der Spalte **Aktionen** auf **Verlängern** geklickt wird.

## Fälligkeitsdatum ändern

Fälligkeitsdaten einer oder mehrerer Ausleihen für eine Person ändern:

1.  Im Bereich **Personendatensatz** bei Bedarf das Akkordeon **Ausleihen** erweitern.
2.  Auf **Aktuelle Ausleihen** klicken.
3.  Die Checkbox auf der linken Seite des Ausleihfensters verwenden, um die entsprechende(n) Ausleihe(n) auszuwählen.
4.  Auf die Schaltfläche **Fälligkeitsdatum ändern** klicken in der oberen rechten Ecke des Ausleihfensters.
5.  Im Pop-up-Fenster ein neues Fälligkeitsdatum und eine neue Fälligkeitszeit eingeben oder aus der Dropdown-Liste im Kalender auswählen.
6.  Auf **Speichern und schließen** klicken.

Mit der entsprechenden Berechtigungen, kann das Fälligkeitsdatum/die Fälligkeitszeit einer Ausleihe auf einen Zeitpunkt in der Vergangenheit geändert werden; FOLIO gibt eine Warnmeldung aus, lässt die Änderung aber zu.

## Angeblich zurückgegeben für Exemplar setzen

Gelegentlich teilen Personen der Bibliothek mit, dass sie Exemplare zurückgegeben haben, die noch als ausgeliehen aufgeführt sind. Die Bibliothek hat die Möglichkeit, das Exemplar als "angeblich zurückgegeben" zu kennzeichnen. Dadurch werden alle damit verbundenen Forderungen ausgesetzt, während die Bibliothek Arbeitsgänge ausführen kann, um das Exemplar zu suchen.

Exemplar als angeblich zurückgegeben setzen:

1.  Im Bereich **Personendatensatz** bei Bedarf das Akkordeon **Ausleihen** erweitern.
2.  Auf **Aktuelle Ausleihen** klicken.
3.  Die Checkbox auf der linken Seite des Ausleihfensters verwenden, um die entsprechende(n) Ausleihe(n) auszuwählen.
4.  Auf die Schaltfläche **Angeblich zurückgegeben** in der oberen rechten Ecke des Fensters Ausleihe klicken.
5.  In dem daraufhin angezeigten Pop-up-Fenster zusätzliche Informationen zur Meldung der Person eingeben.
6.  Auf **Bestätigen** klicken.

Die Ausleihe verbleibt in der Liste der aktuellen Ausleihen der Person, aber der Status des Exemplars zeigt an, dass das Exemplar als angeblich zurückgegeben gemeldet ist.

Wenn die Bibliothek das zurückgeforderte Exemplar nicht finden kann, muss sie entscheiden, ob sie der Person das Exemplar in Rechnung stellt oder es als verloren markiert, ohne Forderungen zu erheben. In FOLIO wird diese Aktion als Forderung auflösen (englisch: "resolving a claim") bezeichnet.

Forderung für ein Exemplar auflösen

1.  Auf die entsprechende Ausleihe klicken, um das Fenster Ausleihdetails zu öffnen.
2.  In der obersten Zeile auf die Schaltfläche **Forderung auflösen** klicken.
3.  Wenn der Person das Exemplar in Rechnung gestellt werden soll, die Option "Für verloren erklärt" wählen. Wenn der Person das Exemplar nicht in Rechnung stellen wollen, wählen Sie "Vermisst".
4.  In dem daraufhin erscheinenden Pop-up-Fenster zeigt FOLIO eine Meldung an, in der die gewünschte Aktion bestätigt werden muss. Dort alle zusätzlichen Informationen über die Reklamation der Person eingeben (erforderlich).
5.  Auf **Bestätigen** klicken.

Wenn dafür entscheiden wird, das Exemplar auf "Für verloren erklärt" zu setzen, prüft FOLIO die zugehörige Forderungsrichtlinie für verlorene Exemplare für die Ausleihe und erhebt die in dieser Richtlinie konfigurierten Forderung.

## Für verloren erklären eines Exemplars

FOLIO verfügt über zwei Optionen, um anzuzeigen, dass ein Exemplar ausgeliehen und nicht zurückgegeben wurde - "Verloren erklärt (Aged to lost)" und "Für verloren erklärt (Declared lost)". "Verloren erklärt" ist ein automatischer Status, den FOLIO einem Exemplar gibt, wenn das Exemplar nicht bis zu dem in der Richtlinie für verlorene Exemplare angegebenen Datum zurückgegeben wird. "Für verloren erklärt" ist ein manueller Status, den das Bibliothekspersonal verwenden kann, wenn eine Person der Bibliothek mitteilt, dass sie das Exemplar nicht zurückgeben kann, weil sie es nicht mehr finden kann oder weil es versehentlich beschädigt wurde.

Es kann jeweils in einem Schritt nur eine Ausleihe als ""Für verloren erklärt" markiert werden. Dazu:

1.  Auf die entsprechende Ausleihe klicken, um das Fenster Ausleihdetails zu öffnen.
2.  Oben auf **Für verloren erklärt** klicken.
3.  In dem erscheinenden Pop-up-Fenster zusätzliche Informationen zu den Umständen der Ausleihe eingeben (erforderlich)
4.  Auf **Bestätigen** klicken.
