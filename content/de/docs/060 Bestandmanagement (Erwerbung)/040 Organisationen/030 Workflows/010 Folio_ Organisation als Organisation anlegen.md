---
title: "Folio: Organisation als Organisation anlegen"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [app-organisationen, by-folio, cat-workflows, for-anwender]
weight: 10
Description: "
    Quellen: [Folio](https://docs.folio.org/docs/acquisitions/organizations/) & [GBV](https://info.gbv.de/display/FOLIOGBVEXTERN/Folio:+Organisation+als+Organisation+anlegen)
    "
---

Wird eine Organisation angelegt, kann sie entweder als allgemeine Organisation oder speziell als Lieferant anlegt werden. Wenn die Organisation als Lieferant angelegt wird, können zusätzliche lieferantenbezogene Informationen hinzugefügt werden. Weitere Informationen zur Erstellung eines Lieferanten sind unter Erstellen eines Lieferanten zu finden.

1.  In der Ansicht **Organisationen** auf **Neu** klicken.
2.  Im Fenster **Organisation erstellen** die Abschnitte **Übersicht**, **Kontaktinformationen**, **Kontaktpersonen** und **Schnittstelle** ausfüllen. Weitere Informationen zu den Feldern und Aktionen, die in diesen Abschnitten verfügbar sind, sin din den Abschnittsbeschreibungen weiter unten zu finden.
3.  Sobald alle gewünschten Informationen über die Organisation eingegeben sind, auf **Speichern & schließen** klicken. Die Organisation wird gespeichert und der Ansicht Organisationen hinzugefügt.

## Übersicht

-   **Name (erforderlich)**. Der Name der Organisation.
-   **Code (erforderlich)**. Ein eindeutiger Identifikator für die Organisation. Hinweis: Es kann keine doppelten Organisationscodes geben. Die Codes für jede Organisation müssen unterschiedlich sein.
-   **Buchhaltungscode**. Der Buchhaltungscode, der von der Bibliothek in dem Zahlungssystem (z.B. SAP) in Bezug auf die Organisation verwendet wird.
-   **Status (erforderlich)**. Einen Organisationsstatus auswählen: Aktiv, Inaktiv oder Vorläufig. Der hier ausgewählte Status wird von den Apps Bestellungen und Rechnungen ausgewertet. Bestellungen können nur geöffnet und Rechnungen nur bezahlt werden, wenn die Organisation ein Lieferant mit dem Status Aktiv ist. Es kann der Status Vorläufig verwenden werden, um zu signalisieren, dass es sich bei dem Organisationseintrag um einen Entwurf handelt.
-   **Typ**. Einen oder mehrere Organisationstypen auswählen. Weitere Informationen sind unter [Einstellungen > Organisationen > Erstellen eines neuen Typs](https://info.gbv.de/pages/viewpage.action?pageId=842793092) zu finden.
-   **Standardsprache**. Die Standardsprache der Organisation wählen.
-   **Lieferant**. Soll eine Lieferantenorganisation erstellt werden, die Checkbox **Lieferant** markieren. Weitere Informationen sind unter [Lieferanten anlegen](https://info.gbv.de/display/FOLIOGBVEXTERN/Folio%3A+Organisation+als+Lieferanten+anlegen) zu finden.
-   **Erwerbungsteams**. Die Erwerbungsteams wählen, die auf den Organisationsdatensatz angewendet werden sollen. Siehe [Einstellungen > Erwerbungsteams](https://info.gbv.de/pages/viewpage.action?pageId=849379720) für weitere Informationen.
-   **Beschreibung**. Eine Beschreibung der Organisation eingeben.
-   **Alternative Namen**. Alternative Namen, die von der Organisation verwendet werden, wie z.B. Abkürzungen oder frühere Namen.

### Alternativen Namen hinzufügen

Hinweis: Das Hinzufügen eines alternativen Namens ist optional, aber wird auf Alternative Namen hinzufügen geklickt, muss einen Alias eingeben oder der alternativen Namen gelöscht werden, um den Organisationsdatensatz zu speichern.

1.  Auf **Alternative Namen hinzufügen** klicken.
2.  Den **Alias**namen der Organisation in das Feld eingeben.
3.  Optional: In das Feld eine Beschreibung für den Alias eingeben.
4.  Den Vorgang nach Bedarf wiederholen. Der alternative Name wird gespeichert, sobald die Organisation gespeichert wird.

### Alternativen Namen löschen

1.  Den alternativen Namen wählen, der gelöscht werden soll.
2.  Auf das **Mülleimersymbol** klicken. Der alternative Name ist gelöscht und wird aus dem Datensatz entfernt, sobald die Organisation gespeichert wird.

## Kontaktinformationen

Im Bereich Kontaktinformationen werden die Kontaktinformationen der Organisation gespeichert, die sich nicht auf einzelne Personen der Organisation beziehen. Es können Kontaktinformationen für bestimmte Personen im weiter unten beschriebenen Abschnitt Kontaktpersonen hinzugefügt werden.

Kategorien für Kontaktinformationen werden in der App Einstellungen konfiguriert. Wird einer Art von Kontaktinformationen, die in diesem Abschnitt eingeben werden, eine Kategorie zugewiesen, werden die Kontaktinformationen nach dieser Kategorie sortiert, wenn die Organisation angezeigt wird.

-   **Adresse**. Die mit der Organisation verbundenen Adressen. Es können mehrere Adressen hinzugefügt werden.
-   **Telefonnummern**. Die Telefonnummern, die mit der Organisation verbunden sind. Es können mehrere Telefonnummern hinzugefügt werden.
-   **E-Mail Adressen**. Die E-Mail-Adressen, die mit der Organisation verbunden sind. Es können mehrere E-Mail-Adressen hinzugefügt werden.
-   **URLs**. Die URLs, die mit der Organisation verbunden sind. Es können mehrere Websites oder FTP-Verbindungen hinzugefügt werden.

### Adressen

#### Adresse hinzufügen

1.  Auf **Adresse hinzufügen** klicken.
2.  Die Adressdaten eingeben.
3.  Den Vorgang nach Bedarf wiederholen. Die Adresse wird gespeichert, sobald die Organisation gespeichert wird. Hinweis: Werden mehrere Adressen hinzugefügt, die Checkbox **Als primäre Adresse verwenden** wählen. Die primäre Adresse wird in den Rechnungsbelegauszug aufgenommen. Weitere Informationen sind unter Rechnungen > Beleginformationen zu finden.

#### Eine Adresse löschen

1.  Die Adresse suchen, die gelöscht werden soll.
2.  Auf das **Mülleimersymbol**. Die Adresse ist gelöscht und wird aus dem Datensatz entfernt, sobald die Organisation gespeichert wird.

### Telefonnummern

#### Telefonnummer hinzufügen

1.  Auf **Telefonnummer hinzufügen** klicken.
2.  Die Telefonnummer in das Feld eingeben.
3.  Optional: Den **Typ** der Telefonnummer aus der Dropdown-Liste wählen: Büro, Mobil, Fax oder Andere.
4.  Optional: Die **Sprache**, die unter dieser Nummer gesprochen wird, aus der Dropdown-Liste auswählen.
5.  Optional: Aus der Dropdown-Liste alle **Kategorien** auswählen, die die Rufnummer beschreiben.
6.  Die Schritte 1-5 je nach Bedarf wiederholen. Die Telefonnummer wird gespeichert, sobald die Organisation gespeichert wird. Hinweis: Werden mehrere Nummern hinzugefügt, dann die Checkbox **Als primäre Telefonnummer verwenden** wählen.

#### Telefonnummer löschen

1.  Die Telefonnummer suchen, die gelöscht werden soll.
2.  Auf das **Mülleimersymbol** klicken. Die Telefonnummer wird entfernt und gelöscht, sobald die Organisation gespeichert wird.

### E-Mail-Adresse

#### E-Mail-Adresse hinzufügen

1.  Auf **E-Mail hinzufügen** klicken.
2.  Die **E-Mail-Adresse** in das Feld eingeben.
3.  Optional: Eine **Beschreibung** der E-Mail in das Feld eingeben.
4.  Optional: Eine **Sprache** aus der Dropdown-Liste wählen.
5.  Optional: In der Dropdown-Liste die **Kategorien** auswählen, die die E-Mail-Adresse beschreiben.
6.  Die Schritte 1-5 nach Bedarf wiederholen, Die E-Mail-Adresse wird gespeichert, sobald die Organisation gespeichert wird. Hinweis: Werden mehrere E-Mail-Adressen hinzugefügt, die Checkbox **Als primäre E-Mail-Adresse verwenden** wählen.

#### E-Mail-Adresse löschen

1.  Die E-Mail-Adresse suchen, die gelöscht werden soll.
2.  Auf das **Mülleimersymbol** klicken. Die E-Mail-Adresse wird entfernt und ist gelöscht, sobald die Organisation gespeichert wird.

### URLs

#### URL hinzufügen

Die URL kann eine Website oder ein FTP-Link sein.

1.  Auf **URL hinzufügen** klicken.
2.  Die **URL** in das Feld eingeben.
3.  Optional: Eine **Beschreibung** der URL in das Feld eingeben.
4.  Optional: Eine **Sprache** aus der Dropdown-Liste wählen.
5.  Optional: Aus der Dropdown-Liste die Kategorien auswählen, die die URL beschreiben.
6.  Die Schritte 1-5 nach Bedarf wiederholen. Die URL wird gespeichert, sobald die Organisation gespeichert wird. Hinweis: Werden mehrere URLs hinzugefüpt, die Checkbox **Als primäre URL verwenden** verwenden wählen.

#### URL löschen

1.  Die URL suchen, die gelöscht werden soll.
2.  Auf das **Mülleimersymbol** klicken. Die URL wird entfernt und ist gelöscht, sobald die Organisation gespeichert wird.

### Kontaktpersonen

#### Neuen Kontaktperson erstellen

Soll ein neuer Kontaktperson erstellt werden, bitte den Abschnitt [Erstellen eines Kontakts](https://info.gbv.de/pages/viewpage.action?pageId=842793050) lesen.

#### Bestehenden Kontakt hinzufügen

1.  Auf **Kontakt hinzufügen** klicken.
2.  Im Dialog **Kontakte hinzufügen** nach dem Kontakt suchen, der hinzugefügt werden soll.
3.  In den Suchergebnissen die Checkbox neben dem oder den Kontakten aktivieren, die hinzugefügt werden sollen. Es können mehrere Kontakte auf einmal hinzugefügt werden.
4.  Auf **Speichern** klicken. Der/die Kontakt(e) erscheint/erscheinen unter dem Abschnitt Kontaktpersonen.

#### Kontakt Löschen

1.  Den Kontakt suchen, der gelöscht werden soll.
2.  Auf das **x** klicken . Der Kontakt ist gelöscht und wird aus dem Datensatz entfernt, sobald die Organisation gespeichert wird.

### Schnittstellen

Eine Schnittstelle ist eine Website, eine Software oder ein Portal, das zur Verwaltung von Aufträgen oder zur Erfassung von Statistiken aus dem Unternehmen verwendet wird.

#### Neue Schnittstelle erstellen

Weitere Informationen sind unter [Interface erstellen](https://info.gbv.de/pages/viewpage.action?pageId=842793057) zu finden.

#### Bestehenden Schnittstelle hinzufügen

1.  Auf **Schnittstelle hinzufügen** klicken.
2.  Im Dialogfeld **Schnittstellen hinzufügen** nach der Schnittstelle suchen, die hinzufügt werden soll.
3.  In den Suchergebnissen die Checkbox neben der/den Schnittstelle(n) aktivieren, die hinzufügt werden sollen. Es können mehrere Schnittstellen auf einmal hinzugefügt werden.
4.  Auf **Speichern** klicken. Die Schnittstelle(n) wird/werden unter dem Abschnitt Schnittstelle angezeigt.

#### Schnittstelle entfernen

1.  Die Schnittstelle suchen, die gelöscht werden soll.
2.  Auf das **x** klicken. Die Schnittstelle ist gelöscht und wird aus dem Datensatz entfernt, sobald die Organisation gespeichert wird.
