---
title: "Folio: Person löschen"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [app-personen, by-folio, cat-worklfows, for-anwender, topic-datenschutz]
weight: 150
Description: "
    Quellen: [Folio](https://docs.folio.org/docs/users/#deleting-a-user-record-in-the-ui ) & [GBV](https://info.gbv.de/pages/viewpage.action?pageId=841416765)
    "
---

Ein Personendatensatz kann nur gelöscht werden, wenn die Person keine offenen Transaktionen hat. Um einen Personendatensatz zu löschen, zunächst prüfen, ob offene Transaktionen vorliegen. Sobald bestätigt ist, dass die Person keine offenen Transaktionen hat, kann der Personendatensatz gelöscht werden.

Folgendermaßen vorgehen, um in der Benutzeroberfläche nach offenen Transaktionen zu suchen und einen Personendatensatz zu löschen:

1.  Via [Folio: Personen suchen](https://info.gbv.de/display/FOLIOGBVEXTERN/Folio%3A+Personen+suchen), die Personendaten finden, und auswählen.
2.  Im Menü Aktionen die Option **Auf offene Transaktionen prüfen/Personendaten löschen**.
    1.  Wenn es keine offenen Transaktionen für diese Person gibt, erscheint die Meldung _Keine offenen Transaktionen für Benutzer (Nachname, Vorname). Sind Sie sicher, dass Sie diese Personendaten löschen möchten?_ im Fenster Auf offene Transaktionen prüfen/Personendaten löschen.
        1.  Auf Ja klicken, um den Personendatensatz zu löschen. Eine Meldung _Person  (Nachname, Vorname) erfolgreich gelöscht_ bestätigt die Löschung des Personendatensatzes.
        2.  Oder auf Nein klicken, um den Löschvorgang abzubrechen und zum Personendatensatz zurückzukehren.
    2.  Wenn es eine oder mehrere offene Transaktionen für die Person gibt, wird die Meldung _Person (Nachname, Vorname) hat folgende offene Transaktionen. Bitte lösen Sie die Transaktionen auf, um mit dem Löschen dieses Benutzers fortzufahren. Klicken Sie auf OK, um zum Benutzerdatensatz zurückzukehren_ angezeigt.
3.  Wenn die gelöschte Person die Berechtigung hatte, Datensätze zu bearbeiten, wird die im Metadatenverlauf aufgeführte Quelle zu "Unbekannter Benutzer".
