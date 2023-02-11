---
title: "Kalender mit Ausnahmen versehen"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [app-einstellungen, by-folio, cat-einstellungen, for-admin]
weight: 60
Description: "
    Quellen: [Folio](https://docs.folio.org/docs/settings/settings_calendar/settings_calendar/#add-exceptions-to-a-calendar) & [GBV](https://info.gbv.de/display/FOLIOGBVEXTERN/Einstellungen+(Kalender):+Kalender+mit+Ausnahmen+versehen)
    "
---

Bibliotheken haben oft Standardöffnungszeiten, die für einen längeren Zeitraum gelten, z. B. für ein akademisches Semester. Sie wünschen sich aber auch die Möglichkeit, ihre Öffnungszeiten für bestimmte Daten wie lokale Feiertage oder Prüfungszeiten zu ändern. Ausnahmen bieten eine Möglichkeit, die regulären Öffnungszeiten einer Servicestelle außer Kraft zu setzen.

Eine Bibliothek kann Ausnahmen nutzen, um eine Servicestelle komplett zu schließen oder die Öffnungszeiten einer Servicestelle zu ändern. Zum Beispiel kann eine Bibliothek während des akademischen Jahres von Sonntag bis Samstag von 9 Uhr bis Mitternacht geöffnet sein, während der Frühjahrsferien jedoch nur von Montag bis Freitag von 9 Uhr bis 17 Uhr. Ausnahmen würden es ermöglichen, den Zeitplan von 9 Uhr morgens bis 17 Uhr abends einzurichten und ihn auf eine bestimmte Woche anzuwenden.

Es gibt zwei Arten von Ausnahmen:

1.  **Schließungen**: Außergewöhnliche Schließungen schließen eine Servicestelle vom Start- bis einschließlich zum Enddatum. Diese können auf einen oder mehrere Kalendertage angewendet werden.
2.  **Öffnungen**: Bei außergewöhnlichen Öffnungen können mehrere Datums- und Zeitspannen angeben werden, so dass die Öffnungs- und Schließzeiten an einem Tag geändert werden können.

So wird eine Ausnahme zu einem Kalender hinzugefügt:

1.  Unter dem Akkordeon **Ausnahmen** auf **Zeile hinzufügen** klicken.
2.  Einen **Namen** für den Zeitraum der Ausnahme eingeben.
3.  Unter **Status** die Option **Geöffnet** wählen, um einen außergewöhnlichen Öffnungszeitraum zu erstellen, oder **Geschlossen** wählen, um einen außergewöhnlichen Schließungszeitraum zu erstellen.
4.  Das **Startdatum** wählen, an dem der Zeitraum der Ausnahme beginnt.
    Anmerkung: Im Gegensatz zu den Öffnungszeiten wird hier ein bestimmtes Datum angeben und nicht einen allgemeinen Wochentag.
5.  Wenn der Status der Zeile **Geöffnet** ist, eine **Startzeit** festlegen.
6.  Das **Enddatum** wählen, an dem der Zeitraum endet.
7.  Wenn der Status der Zeile **Geöffnet** ist, eine Abschlusszeit festlegen.
8.  Wenn die Ausnahme den Status Geöffnet hat, können der Ausnahme weitere Datums-/Zeiträume hinzugefügt werden, indem auf das + in der Spalte Aktionen geklickt wird.

## Beispiel mit Kalenderausnahmen: Schließung wegen des chinesischen Neujahrsfestes.

Angenommen, eine Universitätsbibliothek hat während des Frühjahrssemesters an sieben Tagen in der Woche von 9 Uhr morgens bis Mitternacht geöffnet, wird aber während des chinesischen Neujahrsfestes von Samstag, den 21. Januar 2023 bis Sonntag, den 29. Januar 2023 an einigen Tagen geschlossen und an anderen Tagen für kürzere Zeiten geöffnet sein.

Für die Hauptservicestelle der Bibliothek könnten sie folgendes tun:

1.  Erstellen eines Kalenders mit dem Namen "Frühling 2023 Öffnungszeiten der Hauptbibliothek".
2.  Ein Startdatum für den ersten Unterrichtstag im Januar und ein Enddatum für den letzten Unterrichtstag im Mai festlegen.
3.  Den Kalender der Servicestelle "Hauptbibliothek" zuweisen.
4.  Unter **Öffnungszeiten** eine Zeile für jeden Kalendertag mit dem Status "Geöffnet", einer Startzeit von 9 Uhr und einer Endzeit von 23:59 Uhr erstellen.
5.  Unter **Ausnahmen** eine Ausnahme mit dem Namen "Chinesisches Neujahrsfest - Erstes Wochenende" erstellen. Den Status auf "Geschlossen" setzen, mit einem Startdatum am 21. Januar 2023 und einem Enddatum am 22. Januar 2023. Damit wäre die Bibliothek am ersten Wochenende geschlossen.
6.  Eine zweite Ausnahme mit dem Namen "Feiertag zum chinesischen Neujahr - Wochentag" erstellen. Den Status auf "Geöffnet" setzen. Für die erste Zeile das Start- und Enddatum auf den 23. Januar 2023 festlegen, mit einer Startzeit von 9 Uhr und einer Endzeit von 16 Uhr. Dann eine zweite Zeile hinzufügen, indem auf das + Zeichen unter Aktionen geklickt wird und das Start- und Enddatum auf den 24. Januar 2023 mit einer Startzeit von 9 Uhr und einer Endzeit von 16 Uhr festlegt wird. Diesen Vorgang wiederholen, um für jeden der fünf Tage in dieser Woche eine Zeile hinzuzufügen.
7.  Eine dritte Ausnahme mit dem Namen "Chinesisches Neujahrsfest - Zweites Wochenende" erstellen. Den Status auf "Geschlossen" setzen, mit einem Startdatum am 28. Januar 2023 und einem Enddatum am 29. Januar 2023.
8.  Auf **Speichern und schließen** klicken, um den Kalender zu speichern.

Sobald dieser Kalender erstellt ist, kann er in zukünftigen Jahren wiederverwendet werden, indem der Kalender dupliziert und die Daten geändert werden, anstatt den Zeitplan erneut von Grund auf zu erstellen.
