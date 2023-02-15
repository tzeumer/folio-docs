---
title: "Massenbearbeitung Personendatensätze"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [app-massenbearbeitung, by-folio, cat-workflows, for-anwender]
weight: 10
Description: "
    Quellen: [Folio](https://docs.folio.org/docs/bulk-edit/#user-records) <!-- & [GBV](https://info.gebev.de/pages/viewpage.action?pageId=845709324) -->
    "
---

## Massenbearbeitung einer Datei vorbereiten

Die App Massenbearbeitung akzeptiert nur CSV-Dateien zum Hochladen. Die Datei darf nur eine Spalte mit Datensatzidentifikatoren enthalten.

In der Ansicht **Kriterien festlegen**:

1.  **Personen** unter **Datensatztypen** wählen.
2.  Den Datensatzidentifikatortyp in der Datei aus dem Dropdown-Menü **Datensatzidentifikator** wählen.
3.  Die CSV-Datei per Drag & Drop in das Feld ziehen oder auf "**Datei wählen**, um die Datei von Ihrem Computer hochzuladen" klicken.

## Übereinstimmende Datensätze mit der Vorschau anzeigen lassen

Sobald die CSV-Datei hochgeladen ist, wird die Anzahl der übereinstimmenden Datensätze oben in der Ansicht Massenbearbeitung angezeigt. In der Vorschau werden die ersten zehn gefundenen Ergebnisse angezeigt.

Die folgenden Informationen werden in der Ansicht Vorschau der übereinstimmenden Datensätze angezeigt:

* **Status**. Der Status der Person.
* **Nachname**. Der Nachname der Person.
* **Vorname**. Der Vorname der Person.
* **Barcode**. Der Barcode aus dem Personendatensatz.
* **Personengruppe**. Die Personengruppe, zu der die Person gehört.
* **Kennung**. Die Kennung der Person.
* **E-Mail**. Die E-Mail Adresse der Person.
* **Ablaufdatum**. Das Ablaufdatum des Personendatensatzes.

Wenn eine oder mehrere dieser Spalten in der Ansicht fehlen, auf die Schaltfläche **Aktionen** klicken und sie aus dem Dropdown-Menü auswählen.

## Fehlern verstehen

Wenn bei der Suche nach den übereinstimmenden Datensätzen Fehler gefunden wurden, werden diese im Akkordeon "Fehler" angezeigt.

Es werden zwei Spalten angezeigt:

* **Datensatzidentifikator**. Der Datensatzidentifikator für den Datensatz, bei dem der Fehler aufgetreten ist
* **Fehlergrund**. Der Grund, warum die Suche nicht zu einem passenden Datensatz geführt hat.

## Änderungen vornehmen

### Bearbeitete Datensätze zu FOLIO hochladen

1.  Auf die Schaltfläche **Aktionen** klicken.
2.  Aus dem Dropdown-Menü **Massenbearbeitung starten (CSV)** wählen.
3.  Die CSV-Datei per Drag & Drop in das Feld ziehen oder auf "**Datei wählen**, um die Datei von Ihrem Computer hochzuladen" klicken.
4.  Wenn die Datei erfolgreich hochgeladen wurde, wird eine Bestätigungsmeldung ausgegeben.

### Änderungen bestätigen

1.  Sobald die Datei hochgeladen ist, auf **Weiter** klicken.
2.  Um die Datensätze zu aktualisieren, auf **Änderungen übernehmen** klicken. Das Fenster schließt sich, und die bearbeiteten Datensätze werden in der Ansicht Vorschau der geänderten Datensätze angezeigt.

### Massenbearbeitung ausführen

1.  In der Ansicht **Kriterien festlegen** sicherstellen, dass **Datensatztypen** auf **Personen** eingestellt ist.
2.  In der Ansicht **Kriterien festlegen** die Dropdown-Liste **Datensatzidentifikator auswählen** verwenden, um den Typ des Datensatzidentifikators in der CSV-Datei auszuwählen.
3.  Auf die Schaltfläche **Aktionen** klicken.
4.  Aus dem Dropdown-Menü **Massenbearbeitung starten** wählen.
5.  Unter Optionen auf die Dropdown-Liste klicken und das Feld wählen, das bearbeitet werden soll.
6.  Die zu bearbeitenden Daten eingeben.
7.  Um ein weiteres Feld während desselben Auftrags der Massenbearbeitung zu bearbeiten, auf das Pluszeichen am Ende der Zeile klicken. Eine weitere Zeile wird unter der/den vorhandenen Zeile(n) angezeigt.
8.  Um eine Zeile zu löschen, auf das Mülleimersymbol am Ende der Zeile klicken, die gelöscht werden soll. Die Zeile wird gelöscht.
9.  Auf **Änderungen bestätigen** klicken. Es erscheint ein neues Fenster mit einer Vorschau der ersten 10 zu ändernden Datensätze.
10.  Um die Massenbearbeitung zu beenden, auf **Bearbeitung fortsetzen** klicken. Das Fenster wird geschlossen und die Bearbeitung kann fortgesetzt werden.
11.  Um eine Vorschau der gesamten Liste der Datensätze zu sehen, auf **Vorschau herunterladen** klicken. Eine CSV-Datei wird auf das lokales Gerät heruntergeladen.
12.  Um den Auftrag zur Massenbearbeitung auszuführen, auf **Speichern & schließen** klicken. Das Fenster wird geschlossen und das Banner oben in der Ansicht Massenbearbeitung zeigt die Anzahl der erfolgreich geänderten Datensätze an.
13.  Um die Liste der geänderten Datensätze herunterzuladen, auf die Schaltfläche **Aktionen** oben rechts in der Ansicht klicken.
14.  **Geänderte CSV-Datensätze herunterladen** klicken. Die CSV-Datei wird auf das lokales Gerät heruntergeladen.

### E-Mail bearbeiten

1.  Unter **Optionen** die Option **E-Mail** aus der Dropdown-Liste wählen.
2.  Auf **E-Mail** klicken.
3.  Die einzige verfügbare Aktion ist **Suchen/Ersetzen mit**. Die Daten eingeben, die gesucht und ersetzt werden sollen.
4.  Auf **Änderungen bestätigen** klicken. Die Änderungen an der E-Mail werden auf die Personendatensätze angewendet.

### Ablaufdatum bearbeiten

1.  Unter **Optionen** die Option **Ablaufdatum** aus der Dropdown-Liste wählen.
2.  Die einzige verfügbare Aktion ist **Ersetzen durch**.
3.  Das neue Datum im Format MM/TT/JJJJ eingeben oder auf den Kalender klicken, um das neue Datum auszuwählen.
4.  Auf **Änderungen bestätigen** klicken. Das neue Ablaufdatum wird auf die Personendatensätze angewendet.

### Personengruppe bearbeiten

1.  Unter **Optionen** die Option **Personengruppe** aus der Dropdown-Liste wählen.
2.  Die einzige verfügbare Aktion ist **Ersetzen durch**.
3.  Auf **Personengruppe** klicken und die Personengruppe aus der Dropdown-Liste wählen.
4.  Auf **Änderungen bestätigen** klicken. Die neue Personengruppe wird auf die Personendatensätze angewendet.

### Fehlern verstehen

Wenn bei der Suche nach den übereinstimmenden Datensätzen Fehler gefunden wurden, werden diese im Akkordeon "Fehler" angezeigt.

Es werden zwei Spalten angezeigt:

1.  **Datensatzidentifikator**. Der Datensatzidentifikator für den Datensatz, bei dem der Fehler aufgetreten ist
2.  **Fehlergrund**. Der Grund, warum die Suche nicht zu einem passenden Datensatz geführt hat.

### Massenbearbeitung ausführen (CSV)

1.  In der Ansicht **Kriterien festlegen** sicherstellen, dass **Datensatztypen** auf **Personen** eingestellt ist.
2.  In der Ansicht **Kriterien festlegen** die Dropdown-Liste **Datensatzidentifikator auswählen** verwenden, um den Typ des Datensatzidentifikators in der CSV-Datei auszuwählen.
3.  Auf die Schaltfläche **Aktionen** klicken.
4.  Die CSV-Datei per Drag & Drop in das Feld ziehen oder auf "**Datei wählen**, um die Datei von Ihrem Computer hochzuladen" klicken.
5.  Sobald die CSV-Datei hochgeladen ist, wird die Anzahl der übereinstimmenden Datensätze oben in der Ansicht Massenbearbeitung angezeigt. In der Vorschau werden die ersten zehn gefundenen Ergebnisse angezeigt. Wenn bei der Suche nach den übereinstimmenden Datensätzen Fehler gefunden wurden, werden diese im Akkordeon "Fehler" angezeigt.
6.  Aus dem Dropdown-Menü die Option **Übereinstimmende Datensätze herunterladen (CSV)** wählen.
7.  Die CSV-Datei wird auf das lokales Gerät heruntergeladen.
8.  Die CSV-Datei öffnen und die Änderungen an den gewünschten Feldern vornehmen. Je nach dem Programm, das zum Anzeigen und Bearbeiten von CSV-Dateien verwendet wird, muss möglicherweise geprüft werden, ob alle Felder als "Text" verarbeitet werden, um sicherzustellen, dass die Änderungen von der App für **Massenbearbeitung** korrekt verarbeitet werden.
9.  Die CSV-Datei auf dem lokalen Rechner speichern.
10.  In der App **Massenbearbeitung** auf die Schaltfläche **Aktionen** klicken.
11.  **Massenbearbeitung (CSV) starten** wählen.
12.  Die CSV-Datei mit den bearbeiteten Datensätzen per Drag & Drop in das Feld ziehen oder auf "**Datei wählen**, um die Datei von Ihrem Computer hochzuladen" klicken.
13.  Auf **Weiter** klicken.
14.  Ein Dialogfeld wird angezeigt, in dem die Anzahl der Datensätze angegeben wird, die aktualisiert werden, sobald die Änderungen bestätigt sind.
15.  Auf **Änderungen übernehmen** klicken.
16.  Sobald die Änderungen bestätigt sind, wird die Anzahl der geänderten Datensätze oben in der Ansicht Massenbearbeitung angezeigt. In der Vorschau werden die ersten zehn gefundenen Ergebnisse angezeigt. Wenn beim Aktualisieren der Personendatensätze Fehler gefunden wurden, werden diese im Akkordeon Fehler angezeigt.
17.  Um alle geänderten Datensätze anzuzeigen, auf **Aktionen > Geänderte Datensätze herunterladen (CSV)** klicken.
18.  Um alle Datensätze anzuzeigen, bei denen Fehler gefunden wurden, auf **Aktionen > Fehler herunterladen (CSV)** klicken.
