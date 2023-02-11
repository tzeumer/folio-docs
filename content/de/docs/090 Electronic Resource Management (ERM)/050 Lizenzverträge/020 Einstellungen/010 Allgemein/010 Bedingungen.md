---
title: "Bedingungen"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [app-lizenzverträge, by-folio, cat-einstellungen, for-admin]
weight: 10
Description: "
    Quellen: [Folio](https://docs.folio.org/docs/settings/settings_licenses/settings_licenses/#settings--licenses--terms) & [GBV](https://info.gbv.de/pages/viewpage.action?pageId=847085665)
    "
---

Bedingungen sind die Nutzungsbedingungen, die festlegen, was mit den Ressourcen, die mit dem Lizenzvertrag verbunden sind, getan werden kann und was nicht.

Es gibt zwei Arten von Bedingungen, die in FOLIO erstellt werden können: primäre und optionale Bedingungen. Primäre Bedingungen erscheinen standardmäßig in jedem Lizenzvertrag. Optionale Bedingungen können für jeden einzelnen Lizenzvertrag hinzugefügt werden.

## Bedingung erstellen

1.  Auf **Neu** klicken.
2.  Im Feld **Neue Lizenzbedingung** alle Felder ausfüllen:
    -   **Typ**. Einen Bedingungstyp aus der Dropdown-Liste wählen: Dezimal, Integer, Text, Text, Auswahlliste, Auswahlliste (Mehrfachauswahl) oder Datum. Anmerkung: Dies kann nicht mehr geändert werden, sobald die Bedingung erstellt ist.
    -   **Auswahlliste** und **Auswahlliste (Mehrfachauswahl).** Wenn die Bedingung Auswahlliste oder Auswahlliste (Mehrfachauswahl) ist, wird ein Auswahllistenfeld angezeigt. Dort die gewünschte Auswahlliste aus der Dropdown-Liste auswählen. Weitere Informationen zu Auswahllisten sind unter Einstellungen > Lizenzverträge > Auswahllisten zu finden.
    -   **Anzeigename**. Der Name der Bedingung, der angezeigt wird, wenn Personen in FOLIO und in anderen Systemen, die Lizenzverträge für Personen anzeigen, die Bedingung angezeigt wird. Es empfiehlt sich, einen kurzen Text zu erstellen, der die in der Bedingung enthaltenen Informationen klar und deutlich wiedergibt. Wenn die Bedingung näher erläutert werden muss, sollte das Feld Beschreibung verwendet werden.
    -   **Name**. Wird verwendet, wenn die Daten zu den Bedingungen in einem maschinenlesbaren Format ausgeben werden. Er ist nicht dafür gedacht, Personen (Mitarbeitenden oder anderen Personen) angezeigt zu werden. Es sollte sich um eine kurze Zeichenkette in lateinischen Buchstaben handeln, die von allen externen Systemen oder Programmen verwendet werden kann, die auf die Daten der Lizenzbedingungen zugreifen. Die Verwendung von camelCase wird empfohlen, ist aber nicht erforderlich. Änderungen an den Bedingungen des Lizenzvertrags wirken sich auf alle externen Systeme aus, die auf die Daten der Lizenzverträge zugreifen, und sollten nicht ohne Rücksprache mit den Verantwortlichen für die entsprechenden externen Systeme und Software vorgenommen werden.
    -   **Beschreibung**. Diese Option verwenden, um die Bedingung näher zu erläutern. In der App Lizenzverträge können die Beschreibung angezeigt werden, indem auf das **Informationssymbol** neben der Bezeichnung der Bedingung geklickt wird.
    -   **Kategorie**. Bedingungen können in Kategorien eingeteilt werden. Jede Kategorie wird als separates Akkordeon angezeigt, wenn der Lizenzvertrag angezeigt oder bearbeitet wird. Die Bedingungen können auch in der Dropdown-Liste **Kategorie** nach Kategorien gefiltert werden, die alle Bedingungen enthält, denen die Kategorie zugewiesen wurde. Um eine Kategorie hinzuzufügen, auf das Feld **Kategorie** klicken. Es wird eine Liste der vorhandenen Kategorien angezeigt, die bei der Eingabe gefiltert wird. Es können neue Kategorien hinzugefügt werden, indem ein neuer Wert eingeben und auf die Option **Kontext hinzufügen** geklickt wird. Wenn alle Zuweisungen einer Kategorie über alle Bedingungen hinweg entfernt wurden, wird sie aus der Liste der vorhandenen Kategorien gestrichen.
    -   **Gewichtung der Reihenfolge**. Um die Reihenfolge festzulegen, in der die Bedingungen im Lizenzvertrag erscheinen, eine Zahl eingeben. Wenn kein Wert festlegt und die Gewichtung für jede Bedingung auf 0 belassen wird oder alle Bedingungen die gleiche Zahl enthalten, werden sie alphabetisch sortiert. Bei der alphabetischen Sortierung werden die Großbuchstaben vor den Kleinbuchstaben sortiert. Zum Beispiel: "Zebra" erscheint vor "anfang".
    -   **Primäre Bedingung**. Auswählen, ob es sich bei der Bedingung um einen primäre Bedingung handelt. Primäre Bedingungen werden im Lizenzvertrag immer zur Auswahl angezeigt. Wird **Nein** gewählt, ist die Bedingung optional und sie muss manuell zum Lizenzvertrag hinzugefügt werden, wenn die Bedingung verwendet werden soll.
    -   **Veraltet**. Hier kann angegeben werden, ob eine Bedingung veraltet sein soll. Wird **Ja** gewählt, bleibt die Bedingung in früheren Lizenzverträgen erhalten, wird aber nicht mehr in der Liste der verfügbaren Bedingungen angezeigt, wenn Bedingungen zu einem Lizenzvertrag hinzugefügt werden.
    -   **Standardmäßige Sichtbarkeit**. Auswählen, ob die Bedingung intern in FOLIO oder extern für die Öffentlichkeit angezeigt werden soll (z.B. wenn Eigenschaften zur Anzeige im Katalog eingerichtet werden).
3.  Auf **Speichern** klicken. Es wird eine Bestätigungsmeldung angezeigt, und die Bedingung wird gespeichert und in der Ansicht Bedingungen angezeigt.

## Bedingung bearbeiten

Anmerkung: Der Begriffstyp kann nicht mehr bearbeitet werden, sobald der Begriff erstellt ist.

1.  Die Bedingung suchen, die bearbeitet werden soll und oben im Feld für die Bedingungen auf **Bearbeiten** klicken.
2.  Die gewünschten Änderungen an der Bedingung vornehmen.
3.  Auf **Speichern** klicken. Eine Bestätigungsmeldung wird angezeigt und die Bedingung wird aktualisiert.

## Bedingung löschen

Anmerkung: Eine Bedingung kann nur gelöscht werden, wenn sie keinem Lizenzvertrag zugewiesen ist.

1.  Die Bedingung suchen, die bearbeitet werden soll und oben im Feld für die Bedingungen auf **Löschen** klicken.
2.  Im Dialogfeld **Bedingung löschen** auf **Löschen** klicken. Eine Bestätigungsmeldung wird angezeigt und die Bedingung wird gelöscht.

## Bedingung suchen

Über das Suchfeld kann nach einer Bedingung gesucht werden. Um nach einer Bedingung zu suchen, den Begriff in das Suchfeld eingeben und auf **Suchen** klicken.

Bedingungen können auch nach **Kategorien** gefiltert werden. Eine Kategorie aus der Dropdown-Liste Kategorie wählen und auf **Suchen** klicken. Die Dropdown-Liste enthält alle Kategorien, die den Bedingungen zugewiesen wurden.
