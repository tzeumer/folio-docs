---
title: "Folio: Vereinbarung anlegen"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [app-e_management, by-folio, cat-workflows, for-anwender]
weight: 10
Description: "
    Quellen: [Folio](https://docs.folio.org/docs/erm/agreements/#creating-an-agreement) & [GBV](https://info.gbv.de/display/FOLIOGBVEXTERN/Folio:+Vereinbarung+anlegen)
    "
---

1.  In der Ansicht **Vereinbarungen** auf **Neu** klicken.
2.  Im Fenster **Neue Vereinbarung** die Abschnitte Primäre Felder, Vereinbarungszeiträume, Interne Kontakte, Vereinbarungskomponenten, Informationen des Lizenzvertrags, Organisationen, Ergänzende Eigenschaften, Ergänzende Dokumente, Nutzungsdatenquelle und Zugehörige Vereinbarungen ausfüllen. Weitere Informationen zu den Feldern und Aktionen, die in diesen Abschnitten verfügbar sind, sind in den Abschnittsbeschreibungen weiter unten zu finden.
3.  Sobald alle gewünschten Informationen zur Vereinbarung eingegeben wurden, auf **Speichern & schließen** klicken. Die Vereinbarung wird gespeichert und der Ansicht Vereinbarungen hinzugefügt.

## Grundlegende Felder

-   **Name (erforderlich)**. Der Titel des Vereinbarungsdatensatzes.
-   **Beschreibung**. Eine Beschreibung der Vereinbarung eingeben.
-   **Status (erforderlich)**. Aus der Dropdown-Liste den Status der Vereinbarung auswählen. Zum Beispiel: Aktiv oder Geschlossen. Die Werte, die in der Dropdown-Liste erscheinen, können unter [Einstellungen > eManagement > Auswahllistenwerte](https://info.gbv.de/display/FOLIOGBVEXTERN/Einstellungen+%28eManagement%29%3A+Auswahllistenwerte) konfiguriert werden.
-   **Grund für die Schließung**. Diese Option ist nur verfügbar, wenn in der Dropdown-Liste Status die Option Geschlossen ausgewählt wurde. Dann in der Dropdown-Liste auswählen, warum die Vereinbarung geschlossen wurde. Die Werte, die in der Dropdown-Liste erscheinen, können unter Einstellungen > Vereinbarungen > Werte der Auswahlliste konfiguriert werden.
-   **Verlängerungspriorität**. Aus der Dropdown-Liste den Stand des Interesses an der Verlängerung der Vereinbarung wählen. Die Werte, die in der Dropdown-Liste erscheinen, können unter [Einstellungen > eManagement > Auswahllistenwerte](https://info.gbv.de/display/FOLIOGBVEXTERN/Einstellungen+%28eManagement%29%3A+Auswahllistenwerte) konfiguriert werden.
-   **Dauerhafter Zugriff**. Wenn die Vereinbarung einen unbefristeten Zugriff auf die gekauften Ressourcen vorsieht, **Ja** wählen. Die Werte, die in der Dropdown-Liste erscheinen, können unter [Einstellungen > eManagement > Auswahllistenwerte](https://info.gbv.de/display/FOLIOGBVEXTERN/Einstellungen+%28eManagement%29%3A+Auswahllistenwerte) konfiguriert werden.
-   **Alternativer Name**. Alternative Namen für den Datensatz der Vereinbarung.

### Alternativen Namen hinzufügen

Anmerkung: Das Hinzufügen eines alternativen Namens ist optional, aber wird **Alternative Namen hinzufügen** geklickt, muss ein alternativer Name eingeben werden oder den alternativen Namen muss gelöscht werden, um den Datensatz der Vereinbarung zu speichern.

1.  Auf **Alternative Namen hinzufügen** klicken.
2.  Den **alternativen Namen** für den Datensatz der Vereinbarung in das Feld eingeben.
3.  Den Vorgang nach Bedarf wiederholen. Der alternative Name wird gespeichert, sobald die Vereinbarung gespeichert wird.

### Alternativen Namen löschen

1.  Den alternativen Namen suchen, der gelöscht werden soll.
2.  Auf das **Mülleimersymbol** klicken. Der alternative Name ist gelöscht und wird aus dem Datensatz entfernt, sobald die Vereinbarung gespeichert wird.

## Vereinbarungszeiträume

Mit den Vereinbarungszeiträumen können die Zeitspannen erfasst und verwalten werden, in denen die Vereinbarung aktiv ist.

Werden Vereinbarungszeiträume hinzufügt, sollten Folgendes beachtet werden:

-   Jeder Datensatz muss mindestens einen Vereinbarungszeitraum haben.
-   Wenn nur ein einziger Vereinbarungszeitraum verwendet wird, werden keine weiteren Informationen in Bezug auf Zeiträume angezeigt.
-   Werden dem Datensatz mehrere Zeiträume hinzugefügt, dürfen sich deren Daten nicht überschneiden.
-   Jeder Zeitraum muss ein Startdatum haben.
-   Das früheste Startdatum des Zeitraums wird als Startdatum der Vereinbarung behandelt.
-   Enddaten sind optional, aber nur ein Zeitraum in einem Satz kann ohne Enddatum bleiben. Dies wird als unbefristeter Zeitraum bezeichnet, der zwar ein Startdatum hat, bei dem aber davon ausgegangen wird, dass er auf unbestimmte Zeit läuft.
-   Das späteste Enddatum des Zeitraums wird als Enddatum der Vereinbarung behandelt, oder wenn es ein leeres Enddatum für den Zeitraum gibt, wird die Vereinbarung so behandelt, als hätte sie kein Enddatum.
-   Es kann zwischen vergangenen, aktuellen und zukünftigen Zeiträumen navigiert werden, indem auf die Schaltflächen Vorherige, Aktuelle oder Nächste geklickt wird.

### Vereinbarungszeitraum hinzufügen

1.  Das **Startdatum** des Zeitraums der Vereinbarung eingeben.
2.  Die übrigen Felder ausfüllen. Siehe unten für weitere Informationen. Der Zeitraum der Vereinbarung wird gespeichert, sobald die Vereinbarung gespeichert wird.
3.  Sollen mehrere Zeiträume eingegeben werden, auf **Vereinbarungszeitraum hinzufügen** klicken und die Schritte 1-2 wiederholen.
-   **Startdatum (erforderlich)**. Das Datum, an dem die Vereinbarung beginnt.
-   **Enddatum**. Das Datum, an dem die Vereinbarung endet.
-   **Stornierungsfrist**. Das Datum, bis zu dem die Vereinbarung storniert werden muss, wenn die Ressource, die Gegenstand der Vereinbarung ist, nicht verlängert werden soll.
-   **Bemerkungen zum Zeitraum**. Alle zusätzlichen Informationen über den Zeitraum der Vereinbarung.

### Vereinbarungszeitraum löschen

1.  Den Zeitraum der Vereinbarung suchen, der gelöscht werden soll.
2.  Auf das **Mülleimersymbol** klicken. Der Zeitraum der Vereinbarung ist gelöscht und wird aus dem Datensatz entfernt, sobald die Vereinbarung gesichert wird.

## Interne Kontakte

Interne Kontakte sind in der Regel die Personen innerhalb der Bibliothek, die bei Fragen zu der Vereinbarung kontaktiert werden müssen. Beispielsweise den ERM-Bibliothekar, der für Verlängerungen zuständig ist, den Unterschriftsberechtigten für Vereinbarungen oder den Fachreferenten, der für die Überprüfung von Inhalten im Vorfeld von Verlängerungen verantwortlich ist. Einem Datensatz können mehrere Kontakte zugewiesen werden, aber jeder Kontakt, der hinzugefügt wird, muss einen Personendatensatz in der App Personen haben.

### Internen Kontakt hinzufügen

1.  Auf **Internen Kontakt hinzufügen** klicken.
2.  Auf **Person verknüpfen** klicken.
3.  Im Dialog **Person auswählen** den Namen oder einen Teil des Namens der Person in das Suchfeld in der Ansicht **Personensuche** eingeben und auf **Suche** klicken. Die Ergebnisse der Benutzersuche werden angezeigt.
4.  (Optional) Die Ergebnisse nach Status oder nach Personengruppe filtern.
5.  Auf die Person klicken, die ausgewählt werden soll. Die Person wird dem Datensatz der Vereinbarung als interner Kontakt hinzugefügt.
6.  Die Rolle des internen Kontakts aus der Dropdown-Liste wählen. Die Werte, die in der Dropdown-Liste erscheinen, können unter [Einstellungen > eManagement > Auswahllistenwerte](https://info.gbv.de/display/FOLIOGBVEXTERN/Einstellungen+%28eManagement%29%3A+Auswahllistenwerte) konfiguriert werden.
7.  Die Schritte 1-6 je nach Bedarf wiederholen. Die internen Kontakte werden gespeichert, sobald die Vereinbarung gespeichert wird.

### Internen Kontakt entfernen

1.  Den internen Kontakt suchen, der entfernt werden soll.
2.  Auf das **Mülleimersymbol** klicken. Der interne Kontakt wird aus dem Datensatz entfernt, sobald die Vereinbarung gespeichert wird.

## Vereinbarungskomponenten

Eine Vereinbarungskomponente steht für die Ressource, die von der Vereinbarung abgedeckt wird, z.B. ein Paket oder ein Titel. Soll eine Vereinbarungskomponente hinzugefügt werden, sollte der Fortschritt in dem von erstellten Vereinbarungsdatensatz gesichert oder gewartet werden, bis alle Vereinbarungsinformationen abgeschlossen und gesichert sind, bevor mit dem Prozess der Vereinbarungskomponenten begonnen wird. Anweisungen zum Hinzufügen von Vereinbarungskomponenten zu einem Datensatz sind unter [Folio: Vereinbarungskomponente hinzufügen](https://info.gbv.de/pages/viewpage.action?pageId=845250582) zu finden.

## Informationen des Lizenzvertrags

Im Abschnitt Informationen des Lizenzvertrags kann der Vereinbarungssdatensatz mit einem Lizenzdatensatz verknüpft werden. Es gibt zwei Arten von Lizenzen, die in diesem Abschnitt hinzufügt werden können: in der App Lizenzverträge erstellte Lizenzdatensätze oder externe Lizenzdatensätze (z.B. von einem Konsortium verwaltete Lizenzen).

Anmerkung: Es können mehrere Lizenzverträge zu einem Vereinbarungsdatensatz hinzugefügt werden, aber nur einer kann der wirkende Lizenzvertrag sein. Alle anderen Lizenzverträge müssen als historisch oder zukünftig gekennzeichnet sein. Weitere Informationen sind in Schritt 6 unter [Lizenzvertrag (aus App: Lizenzverträge) hinzufügen zu einer Vereinbarung](https://info.gbv.de/display/FOLIOGBVEXTERN/Folio%3A+Vereinbarung+anlegen) zu finden.

### Bemerkungen zur Lizenz hinzufügen

-   Oben im Abschnitt Informationen des Lizenzvertrags können in das Feld **Bemerkungen** eben solche eingegeben werden.

### Lizenzvertrag (aus App: Lizenzverträge) hinzufügen zu einer Vereinbarung

Anmerkung: Wenn der Lizenzvertrag, der mit der Vereinbarung verknüpft werden soll, Änderungen enthält, werden diese ebenfalls angezeigt, sobald der Lizenzvertrag verknüpft wird. Er muss außerdem einen Status in Bezug auf den Vereinbarungssatz haben. Dies ist wichtig, da die Kombination aus den anwendbaren (kontrollierenden) Lizenzverträgen und den Änderungen die für die Vereinbarung geltenden Bedingungen bestimmt.

1.  Auf **Lizenzvertrag hinzufügen** klicken.
2.  Auf **Lizenzvertrag verknüpfen** klicken.
3.  Im Dialog **Lizenzverträge auswählen** den Namen des Lizenzvertrags oder einen Teil des Namens in das Suchfeld in der Ansicht **Suchen & Filtern** eingeben und auf **Suchen** klicken. Die Suchergebnisse werden in der Ansicht Lizenzverträge angezeigt.
4.  (Optional) Die Ergebnisse mit Hilfe der Filter in der Ansicht **Suchen & Filtern** filtern.
5.  Auf den gewünschten Lizenzvertrag klicken. Der Lizenzvertrag wird dem Vereinbarungsdatensatz hinzugefügt.
6.  Den Status (dieser Vereinbarung) aus der Dropdown-Liste wählen: Wirkend, Zukünftig oder Abgelaufen. Anmerkung: Nur eine Lizenz kann gleichzeitig den Status Wirkend in Bezug auf die Vereinbarung haben. Wirkend bedeutet, dass die Bedingungen des Lizenzvertrags jetzt auf die Vereinbarungen angewendet werden. Die Bedingungen des Wirkenden Lizenzvertrags werden als Lizenzbedingungen der Vereinbarung in der Ansicht Details der Vereinbarung angezeigt. Zukünftig bedeutet, dass der Lizenzvertrag irgendwann in der Zukunft wirkend wird. Abgelaufen bedeutet, dass der Lizenzvertrag zu einem bestimmten Zeitpunkt in der Vergangenheit der wirkende Lizenzvertrag war.
7.  (Optional) Im Feld **Bemerkungen** Anmerkungen zum Lizenzvertrag eingeben.
8.  Die Schritte 1-7 nach Bedarf wiederholen. Die Lizenz wird gespeichert, sobald die Vereinbarung gespeichert wird.

### Externen Lizenzvertrag hinzufügen zu einer Vereinbarung

Externe Lizenzverträge sind alle Lizenzverträge, die nicht über die App Lizenzverträge verfügbar sind.

1.  Auf **Externen Lizenzvertrag hinzufügen** klicken.
2.  Einen **Namen** in das Feld eingeben.
3.  (Optional): Geben Sie eine **Notiz** zum Lizenzvertrag ein.
4.  Es muss mindestens einer der folgenden Schritte ausgeführt werden:
    -   Eine Datei in den Lizenzdatensatz hochladen, indem die Datei per **Drag & Drop** in das Feld Hochladen gezogen wird oder eine **Datei ausgewählt** wird.
    -   **Physischer Standort** des Lizenzvertrags in das Feld eingeben.
    -   Die **URL** des Lizenzvertrags in das Feld eingeben.
5.  Die Schritte 1-5 je nach Bedarf wiederholen. Die externe Lizenz wird gespeichert, sobald der Datensatz der Vereinbarung gespeichert wird.

### Lizenzvertrag entfernen

1.  Den Lizenzvertrag suchen, der entfernt werden soll.
2.  Auf das **Mülleimersymbol** klicken. Die Lizenz wird aus dem Datensatz entfernt, sobald die Vereinbarung gespeichert wird.

### Lizenzvertrag ersetzen

1.  Den Lizenzvertrag suchen, der ersetzt werden soll.
2.  Auf **Lizenzvertrag ersetzen** klicken.
3.  Die Schritte 3-7 unter "Lizenzvertrag (aus App: Lizenzverträge) hinzufügen zu einer Vereinbarung" wiederholen.

## Organisationen

Organisationen sind alle Institutionen, mit denen die Bibliothek in Verbindung steht. Zum Beispiel kann ein Lieferant oder ein Konsortium mit der Vereinbarung verbunden werden. Es können mehrere Organisationen zu einem Datensatz hinzugefügt werden, aber die Organisationen müssen zunächst in der App Organisationen erstellt werden. Um eine Organisation als Hauptorganisation festzulegen, das Feld **Als primäre Organisation festlegen** markieren.

### Organisation hinzufügen

1.  Auf **Organisation hinzufügen** klicken.
2.  Im Feld Organisation auf **Organisation verknüpfen** klicken.
3.  Im Dialog **Organisation wählen** im Suchfeld der Ansicht **Suche & Filter** den Namen der Organisation eingeben oder die Dropdown-Liste Alle verwenden, um nach bestimmten Organisationsparametern zu suchen, und auf **Suchen** klicken. Die Suchergebnisse werden in der Ansicht Organisationen angezeigt.
4.  (Optional) Die Ergebnisse mit Hilfe der Filter in der Ansicht **Suche & Filter** filtern.
5.  Auf die Organisation klicken, die ausgewählt werden soll. Die Organisation wird zum Datensatz der Vereinbarung hinzugefügt.
6.  Die **Rolle** der Organisation aus der Dropdown-Liste wählen. Die Werte, die in der Dropdown-Liste erscheinen, können unter [Einstellungen > eManagement > Auswahllistenwerte](https://info.gbv.de/display/FOLIOGBVEXTERN/Einstellungen+%28eManagement%29%3A+Auswahllistenwerte) konfiguriert werden.
7.  (Optional) Im Feld **Notiz** Anmerkungen zu der Organisation eingeben.
8.  Die Schritte 1-7 nach Bedarf wiederholen. Die Organisation wird gespeichert, sobald die Vereinbarung gespeichert wird.

### Organisation entfernen

1.  Die Organisation suchen, die entfernt werden soll.
2.  Auf das **Mülleimersymbol** klicken. Die Organisation wird aus dem Datensatz entfernt, sobald die Vereinbarung gespeichert wird.

### Organisation ersetzen

1.  Die Organisation suchen, die ersetzt werden soll.
2.  Auf **Organisation ersetzen** klicken.
3.  Die Schritte 3-7 unter "Organisation hinzufügen" wiederholen.

## Ergänzende Eigenschaften

Ergänzende Eigenschaften sind eine optionale Möglichkeit, zusätzliche Informationen über die Vereinbarung zu erfassen, die nirgendwo sonst im Datensatz enthalten sind. Zum Beispiel die Authentifizierungsmethode, die für den Zugriff auf die von der Vereinbarung abgedeckte Ressourcen verwendet wird.

Anmerkung: Dieser Abschnitt wird nur angezeigt, wenn zusätzliche Eigenschaften in der App Einstellungen konfiguriert sind. Weitere Informationen zum Einrichten von Eigenschaften sind unter [Einstellungen > eManagement > Ergänzende Eigenschaften](https://info.gbv.de/pages/viewpage.action?pageId=847085641) zu finden.

### Primär-Eigenschaften ausfüllen

Wenn eine Eigenschaft in der App Einstellungen als primär definiert ist, erscheint sie immer als Option in einem Vertragsdatensatz. Das Feld Wert einer primären Eigenschaft kann leer gelassen werden oder die Option Nicht festgelegt gewählt werden, aber primäre Eigenschaften können nicht aus dem Datensatz einer Vereinbarung entfernt werden.

1.  Das Feld **Wert** ausfüllen, indem entweder Text eingeben, mit den Auf- und Abwärtspfeilen eine ganze Zahl festlegt oder eine Option aus der Dropdown-Liste auswählt wird. Der Wert ist die Definition bzw. die Antwort auf die Eigenschaft.
2.  (Optional) Eine **Interne Notiz** in das Feld eingeben. Jeder Text, der hier eingegeben wird, wird intern für Personen in FOLIO angezeigt.
3.  Die **Sichtbarkeit** der Eigenschaft aus der Dropdown-Liste wählen. Die Sichtbarkeit gibt an, ob die Eigenschaft intern (nur innerhalb von FOLIO) oder extern für die Öffentlichkeit, z.B. in dem Katalog, angezeigt werden soll.
4.  (Optional) Eine **Öffentliche Notiz** in das Feld eingeben. Jeder Text, der hier eingegeben wird, wird extern für die Öffentlichkeit angezeigt.
5.  Die Schritte 1-4 für so viele primäre Eigenschaften wie gewünscht wiederholen. Die Eigenschaften werden gespeichert, sobald die Vereinbarung gespeichert wird.

### Optionale Eigenschaften hinzufügen

Eine Eigenschaft ist optional, wenn sie in der App Einstellungen nicht als primär definiert ist. Optionale Eigenschaften werden nicht automatisch in einem Vertragsdatensatz angezeigt.

1.  Auf **Eigenschaft hinzufügen** klicken.
2.  Den **Namen** der Eigenschaft aus der Dropdown-Liste wählen.
3.  Die Schritte 1-4 unter "Primär-Eigenschaften ausfüllen" ausführen.
4.  So viele optionale Eigenschaften wie nötig hinzufügen. Die Eigenschaften werden gespeichert, sobald die Vereinbarung gespeichert wird.

### Optionale Eigenschaften entfernen

1.  Die optionale Eigenschaft suchen, die entfernt werden soll.
2.  Auf das **Mülleimersymbol** klicken. Die optionale Eigenschaft wird aus dem Datensatz entfernt, sobald die Vereinbarung gespeichert wird.

## Ergänzende Dokumente

Ein ergänzendes Dokument ist jedes zusätzliche Dokument, das für den Datensatz der Vereinbarung relevant ist.

### Ergänzendes Dokumente hinzufügen

1.  Auf **Ergänzendes Dokumente hinzufügen** klicken.
2.  Einen **Namen** in das Feld eingeben.
3.  Eine **Kategorie** aus der Dropdown-Liste wählen. Die Werte, die in der Dropdown-Liste erscheinen, können unter [Einstellungen > eManagement > Auswahllistenwerte](https://info.gbv.de/display/FOLIOGBVEXTERN/Einstellungen+%28eManagement%29%3A+Auswahllistenwerte) konfiguriert werden.
4.  (Optional) Eine Notiz zu dem Ergänzenden Dokumente eingeben.
5.  Es muss mindestens einer der folgenden Schritte ausgeführt werden:
    -   Eine Datei in den Datensatz der Vereinbarung hochladen, indem die Datei per **Drag & Drop** in das Feld Hochladen gezogen wird oder eine **Datei ausgewählt** wird.
    -   **Physischer Standort** des Dokuments in das Feld eingeben.
    -   Die **URL** des Dokuments in das Feld eingeben.
6.  Die Schritte 1-5 je nach Bedarf wiederholen. Das Zusatzdokument wird gespeichert, sobald die Vereinbarung gespeichert wird.

### Ergänzendes Dokumente entfernen

1.  Das ergänzende Dokument suchen, das entfernt werden soll.
2.  Auf das **Mülleimersymbol** klicken. Das ergänzende Dokument wird aus dem Datensatz entfernt, sobald die Vereinbarung gespeichert wird.

## Nutzungsdatenquelle

Ein Anbieter von Nutzungsdaten ist jede Organisation, die der Bibliothek Nutzungsdaten für E-Ressourcen zur Verfügung stellt. Es können mehrere Nutzungsdatenanbieter zu einem Datensatz hinzugefügt werden, aber die Nutzungsdatenanbieter müssen zunächst in der eUsage App erstellt werden.

### Nutzungsdatenquelle hinzufügen

1.  Auf **Nutzungsdatenquelle hinzufügen** klicken.
2.  Im Feld **Nutzungsdatenquelle** auf **Nutzungsdatenquelle verknüpfen** klicken.
3.  Im Dialog **Datenquelle auswählen** den Namen des Anbieters oder einen Teil des Namens in das Suchfeld in der Ansicht **Suchen & Filtern** eingeben und auf **Suchen** klicken. Die Suchergebnisse werden in der Ansicht Nutzungsdatenquellen angezeigt.
4.  (Optional) Die Ergebnisse mit Hilfe der Filter in der Ansicht **Suchen & Filtern** filtern.
5.  Auf den auszuwählenden Nutzungsdatenquellen-Anbieter klicken. Der Anbieter wird dem Datensatz der Vereinbarung hinzugefügt.
6.  (Optional) Eine **Bemerkung** zu dem Nutzungsdatenanbieter eingeben.
7.  Die Schritte 1-6 nach Bedarf wiederholen. Die Nutzungsdatenquelle wird gespeichert, sobald die Vereinbarung gespeichert wird.

### Nutzungsdatenquelle entfernen

1.  Den Anbieter der Nutzungsdatenquelle suchen, die entfernt werden soll.
2.  Auf das **Mülleimersymbol** klicken. Die Nutzungsdatenquelle wird aus dem Datensatz entfernt, sobald die Vereinbarung gespeichert wird.

### Nutzungsdatenquelle ersetzen

1.  Den Anbieter der Nutzungsdatenquelle suchen, die ersetzt werden soll.
2.  Auf **Nutzungsdatenquelle ersetzen** klicken.
3.  Die Schritte 3-6 unter "Nutzungsdatenquelle hinzufügen" wiederholen.

## Zugehörige Vereinbarungen

Eine zugehörige Vereinbarung ist eine Vereinbarung, die für die aktuelle Vereinbarung relevant ist. In diesem Abschnitt können Vereinbarungen miteinander verknüpft werden, um Beziehungen zwischen ihnen herzustellen. Es kann hier zum Beispiel eine Vereinbarung nach einer Stornierung hinzugefügt werden.

### Zugehörige Vereinbarungen hinzufügen

1.  Auf **Zugehörige Vereinbarung hinzufügen** klicken.
2.  Im Feld  **Zugehörige Vereinbarung** auf **Vereinbarung verknüpfen** klicken.
3.  Im Dialogfeld **Vereinbarung auswählen** den Namen der Vereinbarung oder einen Teil des Namens in das Suchfeld in der Ansicht **Suchen & Filtern** eingeben und auf **Suchen** klicken. Die Suchergebnisse werden in der Ansicht Vereinbarungen angezeigt.
4.  (Optional) Die Ergebnisse mit Hilfe der Filter in der Ansicht **Suchen & Filtern** filtern.
5.  Auf die Vereinbarung klicken, die ausgewählt werden soll. Die Vereinbarung wird zum Datensatz der Vereinbarung hinzugefügt.
6.  Aus der Dropdown-Liste die Beziehung der verknüpften Vereinbarung zu der zu bearbeitenden Vereinbarung auswählen. Anmerkung: Die Beziehungen sind direktional. Wenn z.B. die Vereinbarung A eine Rückverknüpfung mit der Vereinbarung B hat, dann hat automatisch die Vereinbarung B eine Vorverknüpfung mit der Vereinbarung A. Diese Beziehungen können von beiden Seiten aus festgelegt werden (d.h. es kann mit der Verknüpfung der Vereinbarung A mit B oder B mit A begonnen werden).
7.  (Optional) Eine **Bemerkung** zu der zugehörigen Vereinbarung eingeben.
8.  Die Schritte 1-6 nach Bedarf wiederholen. Die zugehörige Vereinbarung wird gespeichert, sobald die Hauptvereinbarung gespeichert wird.

### Zugehörige Vereinbarungen entfernen

1.  Die Zugehörige Vereinbarung suchen, die entfernt werden soll.
2.  Auf das **Mülleimersymbol** klicken. Die zugehörige Vereinbarung wird aus dem Datensatz entfernt, sobald die Vereinbarung gespeichert wird.

### Zugehörige Vereinbarungen ersetzen

1.  Die zugehörige Vereinbarung suchen, die ersetzt werden soll.
2.  Auf **Vereinbarung ersetzen** klicken.
3.  Die Schritte 3-6 unter "Zugehörige Vereinbarungen hinzufügen" wiederholen.
