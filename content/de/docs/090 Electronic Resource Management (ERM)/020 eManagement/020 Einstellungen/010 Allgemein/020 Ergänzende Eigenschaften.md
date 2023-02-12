---
title: "Ergänzende Eigenschaften"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [app-e_management, by-folio, cat-einstellungen, for-admin]
weight: 20
Description: "
    Quellen: [Folio](https://docs.folio.org/docs/settings/settings_agreements/settings_agreements/#settings--agreements--supplementary-properties) & [GBV](https://info.gbv.de/pages/viewpage.action?pageId=847085641)
    "
---

Ergänzende Eigenschaften sind eine optionale Möglichkeit, zusätzliche Informationen über die Vereinbarung zu erfassen, die nirgendwo sonst im Datensatz erfasst sind. Zum Beispiel die Authentifizierungsmethode für den Zugriff auf die Ressourcen, die Gegenstand der Vereinbarung sind.

Sind ergänzende Eigenschaften konfiguriert, wird der Abschnitt Ergänzende Eigenschaften in Vertragsdatensätzen angezeigt. Ergänzende Eigenschaften ähneln den Bedingungen von Lizenzverträgen. Es gibt zwei Arten von ergänzenden Eigenschaften, die in FOLIO erstellt werden können: primäre und optionale. Primäre Eigenschaften erscheinen standardmäßig in jedem Vertragsdatensatz. Optionale Eigenschaften können für jede einzelne Vereinbarung hinzugefügt werden.

## Ergänzende Eigenschaft erstellen

1.  Auf **Neu** klicken.
2.  Im Feld **Neue ergänzende Eigenschaft** alle Felder ausfüllen:
    * **Typ**. Einen Eigenschaftstyp aus der Dropdown-Liste wählen: Dezimal, Integer, Text, Auswahlliste, Auswahlliste (Mehrfachauswahl) oder Datum.
    * **Auswahlliste** und **Auswahlliste (Mehrfachauswahl)**. Wird als Eigenschaftstyp Auswahlliste oder Auswahlliste (Mehrfachauswahl) gewählt, wird ein Feld Auswahlliste angezeigt. Die gewünschte **Auswahlliste** aus der Dropdown-Liste wählen. Weitere Informationen zu Auswahllisten sind unter Einstellungen > Vereinbarungen > Auswahllisten zu finden.
    * **Anzeigename**. Der Name der Eigenschaft, der angezeigt wird, wenn Personen in FOLIO die Eigenschaft sehen. Es empfiehlt sich, eine kurze Textzeichenfolge zu erstellen, die die in der Eigenschaft erfassten Informationen klar vermittelt. Wenn die Eigenschaft näher erläutert werden soll, sollte das Feld Beschreibung verwendet werden.
    * **Name**. Wird bei der Ausgabe von Eigenschaftsdaten in einem maschinenlesbaren Format verwendet. Er ist nicht dafür gedacht, Personen (Mitarbeitenden oder anderen Personen) angezeigt zu werden. Es sollte sich um eine kurze Zeichenkette in lateinischen Buchstaben handeln, die von allen externen Systemen oder Programmen verwendet werden kann, die auf die Daten zu den Eigenschaften der Vereinbarung zugreifen. Die Verwendung von camelCase wird empfohlen, ist aber nicht erforderlich. Änderungen am Namen wirken sich auf alle externen Systeme aus, die die Objektdaten der Vereinbarung verwenden, und sollten nicht ohne Rücksprache mit den Verantwortlichen für die entsprechenden externen Systeme und Software vorgenommen werden.
    * **Beschreibung**. Diese Option verwenden, um die Eigenschaft näher zu erläutern. In der App eManagement können die Beschreibung anzeigt werden, indem auf das **Informationssymbol** neben der Bezeichnung der Eigenschaft geklcikt wird.
    * **Kategorie**. (Nicht erforderlich.) Ergänzende Eigenschaften können für Open Access und andere Zwecke kategorisiert werden. Jede Kategorie wird als separates Akkordeon angezeigt, wenn die Vereinbarung angesehen oder bearbeitet wird. Eigenschaften können auch über die Dropdown-Liste **Kategorie** filtern, die alle Kategorien enthält, die den Eigenschaften zugewiesen wurden. Um eine Kategorie hinzuzufügen, auf das Feld **Kategorie** klicken. Es wird eine Liste der vorhandenen Kategorien angezeigt, die bei der Eingabe gefiltert wird. Es können neue Kategorien hinzugefügt werden, indem ein neuer Wert eingegeben und auf die Option **Kontext hinzufügen** geklickt wird. Wenn alle Zuordnungen einer Kategorie über alle Eigenschaften hinweg entfernt werden, wird sie aus der Liste der vorhandenen Kategorien entfernt.
    * **Gewichtung der Reihenfolge**. Um die Reihenfolge festzulegen, in der die Eigenschaften im Vereinbarungsdatensatz erscheinen, eine Zahl eingeben. Wird kein Wert eingeben und die Gewichtung für jede Eigenschaft auf 0 belassen oder alle Eigenschaften die gleiche Zahl enthalten, werden sie alphabetisch sortiert. Bei der alphabetischen Sortierung werden die Großbuchstaben vor den Kleinbuchstaben sortiert. Zum Beispiel: "Zebra" erscheint vor "anfang".
    * **Primäre Eigenschaft**. Auswählen, ob die Eigenschaft eine primäre Eigenschaft ist. Primäre Eigenschaften werden immer in Datensätzen von Vereinbarungen angezeigt. Wird **Nein** gewählt, ist die Eigenschaft optional und sie muss manuell zu einem Vertragsdatensatz hinzugefügt werden, wenn diese Eigenschaft verwendet werden soll.
    * **Veraltet**. Hier kann angegeben werden, ob eine Eigenschaft veraltet sein soll. Wird **Ja** gewählt, bleibt die Eigenschaft in früheren Vereinbarungen erhalten, wird aber nicht mehr in der Liste der verfügbaren Eigenschaften angezeigt, wenn einer Vereinbarung Eigenschaften hinzugefügt werden.
    * **Standardmäßige Sichtbarkeit**. Auswählen, ob die Eigenschaft intern in FOLIO oder extern für die Öffentlichkeit angezeigt werden soll (z.B. wenn Eigenschaften zur Anzeige im  Katalog eingerichtet werden).
3.  Auf **Speichern** klicken. Es erscheint eine Bestätigungsmeldung, und die ergänzende Eigenschaft wird gespeichert und erscheint in der Ansicht Ergänzende Eigenschaften.

## Ergänzende Eigenschaft bearbeiten

1.  Die Eigenschaft suchen, die bearbeitet werden soll und oben in ihrem Eigenschaftsfeld auf **Bearbeiten** klicken.
2.  Die gewünschten Änderungen an der Eigenschaft vornehmen.
3.  Auf **Speichern** klicken. Eine Bestätigungsmeldung wird angezeigt und die Eigenschaft wird aktualisiert.

## Ergänzende Eigenschaft löschen

Anmerkung: Eine Eigenschaft kann nur gelöscht werden, wenn sie keinem Vertragsdatensatz zugewiesen ist.

1.  Die Eigenschaft suchen, die bearbeitet werden soll und oben in ihrem Eigenschaftsfeld auf **Löschen** klicken.
2.  Im Dialogfeld **Ergänzende Eigenschaft löschen** auf **Löschen** klicken. Eine Bestätigungsmeldung erscheint und die Eigenschaft wird gelöscht.

## Ergänzende Eigenschaft suchen

Über das Suchfeld kann nach einer ergänzenden Eigenschaft gesucht werden. Um nach einer Eigenschaft zu suchen, die Eigenschaft in das Suchfeld eingeben und auf **Suchen** klicken.

Eigenschaften können auch nach Kategorie gefiltert werden. Eine Kategorie aus der Dropdown-Liste Kategorie wählen und auf **Suchen** klicken. Die Dropdown-Liste enthält alle Kategorien, die den Eigenschaften zugewiesen wurden.
