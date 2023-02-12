---
title: "Massenbearbeitung Exemplardatensätze"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [app-massenbearbeitung, by-folio, cat-workflows, for-anwender]
weight: 20
Description: "
    Quellen: [Folio](https://docs.folio.org/docs/bulk-edit/#item-records) & [GBV](https://info.gbv.de/pages/viewpage.action?pageId=845709326)
    "
---

## Datensätzen für die Massenbearbeitung identifizieren

Die App **Massenbearbeitung** akzeptiert nur CSV-Dateien zum Hochladen. Es können nur Dateien mit einer Spalte mit Datensatzidentifikatoren hochgeladen werden.

1.  In der Ansicht **Kriterien einstellen** sicherstellen, dass Datensatztypen auf **Katalog - Exemplare** eingestellt ist.
2.  In der Ansicht **Kriterien festlegen** den **Datensatzidentifikator** aus der Dropdown-Liste auswählen. Der ausgewählte Datensatzidentifikator, sollte mit dem Typ des Datensatzidentifikators in der hochgeladenen CSV-Datei übereinstimmen.
3.  Die CSV-Datei per Drag & Drop in das Feld ziehen oder auf "**Datei wählen**, um die Datei von Ihrem Computer hochzuladen" klicken.

## Übereinstimmende Datensätze mit der Vorschau anzeigen lassen

Sobald nach einem Exemplardatensatz gesucht wurde, werden die folgenden Informationen in der Ansicht Vorschau der übereinstimmenden Datensätze angezeigt:

-   **Barcode**. Eine Zahlenfolge, die an das Exemplar angehängt und mit einem Barcode-Scanner überprüft wurde.
-   **Status**. Der Status des Exemplars.
-   **Tatsächlicher Standort des Exemplars**. Der tatsächliche Standort des Exemplars.
-   **Effektive Signatur**. Die effektive Signatur des Exemplars.
-   **Exemplar-HRID**. Der von Menschen lesbare Identifikator (HRID) des Exemplars.
-   **Materialart**. Die Materialart der Ressource des Exemplars. Die Materialart ist die materielle Beschaffenheit eines bestimmten Exemplars und soll spezifischere Informationen als die Ressourcenart allein ermöglichen.
-   **Art der Dauerausleihe**. Die Art der Dauerausleihe des Exemplars.
-   **Temporärer Ausleihtyp**. Die Art der vorübergehenden Ausleihe des Exemplars.
-   **Exemplar UUID**. Der universell eindeutige Identifikator (UUID) des Exemplars.
-   **Früherer Identifikator**. Frühere Identifikatoren, die dem Exemplar zugewiesen wurden.
-   **Zugangsnummer**. Die Zugangsnummer eines Exemplars. Die Zugangsnummer ist eine eindeutige Nummer, die einem Exemplar in der Reihenfolge zugewiesen wird, in der es in eine Bibliothekssammlung aufgenommen wird.
-   **Dauerhafter Standort des Exemplars**. Der dauerhafte Standort des Exemplars.
-   **Temporärer Standort des Exemplars**. Der temporäre Standort des Exemplars.
-   **Exemplarnummer**. Die Exemplarnummer des Exemplars. Die Exemplarnummer gibt an, ob die Bibliothek ein (oder mehrere) Exemplare einer einbändigen Monographie besitzt.
    Aufzählung. Die mit dem Exemplar verbundene Aufzählung. Bei den Aufzählungsdaten des Exemplars handelt es sich um die beschreibenden Informationen für das Nummerierungsschema einer Reihe.
-   **Chronologie**. Die mit dem Exemplar verknüpfte Chronologie. Die Chronologie ist die beschreibende Information für das Datierungsschema einer Serie.
-   **Band**. Die Bandnummer des Exemplars.

Wenn eine oder mehrere dieser Spalten in der Ansicht fehlen, auf die Schaltfläche **Aktionen** klicken und aus dem Dropdown-Menü auswählen.

## Fehlern verstehen

Wenn bei der Suche nach den übereinstimmenden Datensätzen Fehler gefunden wurden, werden diese im Akkordeon "Fehler" angezeigt.

Es werden zwei Spalten angezeigt:

1.  **Datensatzidentifikator**. Der Datensatzidentifikator für den Datensatz, bei dem der Fehler aufgetreten ist
2.  **Fehlergrund**. Der Grund, warum die Suche nicht zu einem passenden Datensatz geführt hat.

## Massenbearbeitung ausführen

1.  Auf die Schaltfläche **Aktionen** klicken.
2.  Aus dem Dropdown-Menü **Massenbearbeitung starten** wählen.
3.  Unter Optionen auf die Dropdown-Liste klicken und das Feld wählen, das bearbeitet werden soll.
4.  Unter **Aktionen** auf **Aktion auswählen** klicken und die Aktion wählen, die auf die Exemplardatensätze angewendet werden soll.
5.  Um ein weiteres Feld während desselben Auftrags der Massenbearbeitung zu bearbeiten, auf das Pluszeichen am Ende der Zeile klicken. Eine weitere Zeile wird unter der/den vorhandenen Zeile(n) angezeigt.
6.  Um eine Zeile zu löschen, auf das Mülleimersymbol am Ende der Zeile klicken, die gelöscht werden soll. Die Zeile wird gelöscht.
7.  Auf **Änderungen bestätigen** klicken. Es erscheint ein neues Fenster mit einer Vorschau der ersten 10 zu ändernden Datensätze.
8.  Um zur Massenbearbeitung zurückzukehren, auf **Bearbeitung fortsetzen** klicken. Das Fenster wird geschlossen und es kann mit der Bearbeitung fortgefahren werden.
9.  Um eine Vorschau der gesamten Liste der Datensätze zu sehen, auf **Vorschau herunterladen** klicken. Eine CSV-Datei wird auf das lokales Gerät heruntergeladen.
10.  Um den Auftrag zur Massenbearbeitung auszuführen, auf **Speichern & schließen** klicken. Das Fenster wird geschlossen und das Banner oben in der Ansicht Massenbearbeitung zeigt die Anzahl der erfolgreich geänderten Datensätze an.
11.  Um die Liste der geänderten Datensätze herunterzuladen, auf die Schaltfläche **Aktionen** oben rechts in der Ansicht klicken.
12.  **Geänderte CSV-Datensätze herunterladen** klicken. Die CSV-Datei wird auf das lokales Gerät heruntergeladen.

## Temporären Standort für Exemplare bearbeiten

1.  Unter **Optionen** die Option **Temporärer Standort für Exemplare** aus der Dropdown-Liste wählen.
2.  Auf **Aktionen** klicken, um **Ersetzen durch** oder **Feld leeren** auszuwählen.
3.  Für **Ersetzen durch** auf **Standort auswählen** klicken und den temporären Standort des Exemplars aus der Dropdown-Liste auswählen oder die **Standortsuche** verwenden.
4.  Für **Feld leeren**, mit Schritt 5 fortfahren.
5.  Auf **Änderungen bestätigen** klicken.
6.  Die **Vorschau der zu ändernden Datensätze** wird angezeigt mit den Optionen **Bearbeitung fortsetzen**, **Vorschau herunterladen** oder **Änderungen übernehmen**.
7.  Die Änderungen werden auf die Exemplardatensätze angewendet, sobald auf **Änderungen übernehmen** geklickt wird.

## Dauerhaften Standorts eines Exemplars bearbeiten

1.  Unter **Optionen** die Option **Dauerhafter Standort für Exemplare** aus der Dropdown-Liste wählen.
2.  Auf **Aktionen** klicken, um **Ersetzen durch** oder **Feld leeren** auszuwählen.
3.  Für **Ersetzen durch** auf **Standort auswählen** klicken und den temporären Standort des Exemplars aus der Dropdown-Liste auswählen oder die **Standortsuche** verwenden.
4.  Für **Feld leeren**, mit Schritt 5 fortfahren.
5.  Auf **Änderungen bestätigen** klicken.
6.  Die **Vorschau der zu ändernden Datensätze** wird angezeigt mit den Optionen **Bearbeitung fortsetzen**, **Vorschau herunterladen** oder **Änderungen übernehmen**.
7.  Die Änderungen werden auf die Exemplardatensätze angewendet, sobald auf **Änderungen übernehmen** geklickt wird.

## Exemplarstatus bearbeiten

1.  Unter **Optionen** die Option **Exemplarstatus** aus der Dropdown-Liste wählen.
2.  Aus der Dropdown-Liste den Exemplar-Status auswählen, der angewendet werden soll.
3.  Auf **Änderungen bestätigen** klicken. Der neue  Exemplarstatus wird auf die Exemplardatensätze angewandt.
4.  Die **Vorschau der zu ändernden Datensätze** wird angezeigt mit den Optionen **Bearbeitung fortsetzen**, **Vorschau herunterladen** oder **Änderungen übernehmen**.
5.  Die Änderungen werden auf die Exemplardatensätze angewendet, sobald auf **Änderungen übernehmen** geklickt wird.

## Bearbeitung des Zeitweisen Ausleihtyps

1.  Unter **Optionen** die Option **Zeitweisen Ausleihtyp** aus der Dropdown-Liste wählen.
2.  Auf **Aktionen** klicken, um **Ersetzen durch** oder **Feld leeren** auszuwählen.
3.  Für **Ersetzen durch** auf **Ausleihtyp auswählen** klicken und den Zeitweisen Ausleihtyp auswählen.
4.  Für **Feld leeren**, mit Schritt 5 fortfahren.
5.  Auf **Änderungen bestätigen** klicken.
6.  Die **Vorschau der zu ändernden Datensätze** wird angezeigt mit den Optionen **Bearbeitung fortsetzen**, **Vorschau herunterladen** oder **Änderungen übernehmen**.
7.  Die Änderungen werden auf die Exemplardatensätze angewendet, sobald auf **Änderungen übernehmen** geklickt wird.

## Dauerhafter Ausleihtyp bearbeiten

1.  Unter **Optionen** die Option **Dauerhafter Ausleihtyp** aus der Dropdown-Liste wählen.
2.  Aus der Dropdown-Liste den Ausleihtyp auswählen, der angewendet werden soll.
3.  Auf **Änderungen bestätigen** klicken.
4.  Die **Vorschau der zu ändernden Datensätze** wird angezeigt mit den Optionen **Bearbeitung fortsetzen**, **Vorschau herunterladen** oder **Änderungen übernehmen**.
5.  Die Änderungen werden auf die Exemplardatensätze angewendet, sobald auf **Änderungen übernehmen** geklickt wird.

## Abgeglichene Datensätze herunterladen (CSV)

1.  Auf die Schaltfläche **Aktionen** klicken.
2.  Aus dem Dropdown-Menü **Abgeglichene Datensätze herunterladen (CSV)** wählen.
3.  Die Datei auf dem lokalen Gerät öffnen.
4.  Die Datensätze bearbeiten und die Datei auf dem lokalen Gerät speichern. Sicherstellen, dass die Datei im CSV-Format gespeichert wird.
