---
title: "Kalender erstellen"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [app-einstellungen, by-folio, cat-einstellungen, for-admin]
weight: 50
Description: "
    Quellen: [Folio](https://info.gbv.de/display/FOLIOGBVEXTERN/Einstellungen+(Kalender):+Kalender+erstellen) & [GBV](https://docs.folio.org/docs/settings/settings_calendar/settings_calendar/#create-a-new-calendar)
    "
---

So wird ein neuer Kalender erstellt:

1.  Zu **Alle Kalender** gehen.
2.  **Aktionen > Neu** wählen.
3.  Einen **Kalendernamen** eingeben.
4.  Ein **Startdatum** und ein Enddatum eingeben.
5.  Eine oder mehrere Servicestellen wählen, denen der Kalender zugewiesen werden soll. Diese Option kann auch leer gelassen werden und der Kalender später einer Servicestelle zugewiesen werden.

Als Nächstes werden Öffnungszeiten hinzugefügt.

Die Öffnungszeiten werden im Kalender in Form einer Tabelle dargestellt, wobei jede Zeile für einen Zeitraum von **Öffnungszeiten** steht - einen Zeitraum, in dem die Servicestelle für den Service geöffnet und dann geschlossen ist.

Wenn eine Servicestelle an einem Tag öffnet und dann erst an einem späteren Tag schließt, können der **Starttag** und der **Endtag** einer bestimmten Zeile unterschiedliche Tage sein. Dies kann beispielsweise der Fall sein, wenn eine Bibliothek über Nacht für Studierende geöffnet bleibt, die für Abschlussprüfungen lernen.

Wenn die Standardöffnungszeiten einer Bibliothek einen Tag vorsehen, an dem sie komplett geschlossen ist, sollten trotzdem eine Zeile für diesen Tag angelegt werden und den Status als geschlossen gekennzeichnet werden. Wenn zum Beispiel eine Servicestelle sonntags immer geschlossen ist, würde dieser Tag mit einer Zeile mit dem Status **Geschlossen**, dem **Starttag** Sonntag und dem **Endtag** Sonntag abgebildet werden.

So werden Öffnungszeiten hinzugefügt:

1.  Unter **Status** die Option **Geöffnet** oder **Geschlossen** wählen.
2.  Den **Starttag** für die Öffnungszeit wählen.
3.  Die **Startzeit** wählen, zu der die Servicestelle geöffnet ist. Wenn der Status der Zeile Geschlossen ist, wird keine Startzeit festgelegt.
4.  Den **Endtag** wählen, an dem die Servicestelle schließt. Wenn die Bibliothek nach 23:59 Uhr geöffnet bleibt, ist der Endtag ein anderer als der Starttag.
5.  Die **Endzeit** wählen, zu der die Servicestelle schließt. Wenn der Status der Zeile **Geschlossen** ist, muss keine Endzeit festgelegt werden.
6.  Auf **Zeile hinzufügen** klicken, um bei Bedarf weitere Zeilen hinzuzufügen.
7.  Wenn das Hinzufügen der Öffnungszeiten abgeschlossen ist, unten auf **Speichern und schließen** klicken, um den Kalender zu speichern.

Unterläuft bei einer Kalenderzeile ein Fehler, auf den **Mülleimer** unter Aktionen klicken, um sie zu entfernen und ein neues Zeitfenster hinzuzufügen. Wenn die Änderungen gespeichert werden, sortiert FOLIO die Zeilen so, dass sie in einer Standard-Wochenreihenfolge angezeigt werden.
