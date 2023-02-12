---
title: "Datensatz suchen im Katalog"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [app-katalog, by-folio, cat-workflows, for-anwender, meta-gemeldet_docsfolioorg]
weight: 90
Description: "
    Quellen: [Folio](https://docs.folio.org/docs/metadata/inventory/#searching-for-a-record) & [GBV](https://info.gbv.de/display/FOLIOGBVEXTERN/Folio:+Datensatz+suchen+im+Katalog)
    "
---

Wenn nach einem Katalogdatensatz gesucht wird, kann zwischen der Suche auf Instanz-, Bestands- oder Exemplar-Ebene umgeschaltet werden. Die Suche nach einem Instanzdatensatz unterstützt die Suche nach bibliographischen Daten. Bei der Suche nach einem Bestandsdatensatz oder einem Exemplar können die Daten des Instanzdatensatzes zusammen mit den bestands- und exemplarspezifischen Datenelementen durchsucht werden.

Nach Instanzen, Beständen oder Exemplaren kann gesucht werden, indem in der Ansicht **Suchen & Filtern** entweder auf **Instanz**, **Bestand** oder **Exemplar** geklickt wird. Die Elemente, die für die Suche und Filterung zur Verfügung stehen, sind je nach Auswahl unterschiedlich, aber die Ergebnisse zeigen immer Instanzdatensätze an.

Um zu suchen, zunächst die Art des Datensatzes auswählen (Instanz, Bestand oder Exemplar); die Suchbegriffe in das Feld eingeben und auf **Suchen** klicken. Die Dropdown-Liste Stichwort (Titel, Mitwirkende/-r, Identifikator wählen), um eine der folgenden Felder zu durchsuchen:

Tab Instanz/Alle

-   **Stichwort (Titel, Mitwirkende/-r, Identifikator)**. Stichwortsuche über die Felder Titel, Mitwirkender und Bezeichner.
-   **Mitwirkende/-r**. Stichwortsuche über alle Mitwirkenden-Felder.
-   **Titel (Alle)**. Stichwortsuche in allen Titelfeldern. Dies beinhaltet die Suche nach dem Äquivalent des eigentlichen Titels, alternativen Titeln (einschließlich einheitlicher Titel) und Serientiteln, aber nicht nach vorangehenden und nachfolgenden Titeln.
-   **Identifikator (alle)**. Durchsucht alle Identifikatortypen. Nicht normalisiert: Die Suche kann trunkiert bleiben, andernfalls muss der gesamte Identifikator, einschließlich eines Präfixes, eingegeben werden.
-   **ISBN**. Sucht die Nummer genau so, wie sie in den Daten erscheint. Wenn die Daten z.B. Bindestriche enthalten, müssen die Bindestriche in die Suche eingegeben werden.
-   **ISSN**. Die Suche sollte Bindestriche enthalten.
-   **OCLC-Nummer, normalisiert**. Sucht nach der OCLC-Nummer mit oder ohne Präfixe.
-   **Instanzanmerkungen (alle)**. Stichwortsuche über alle Instanzanmerkungen; schließt Verwaltungsnotizen ein.
-   **Instanzverwaltungsnotiz**. Stichwortsuche nach Verwaltungsnotizen im Instanzdatensatz.
-   **Schlagwort**. Schlagwortsuche über alle Schlagwortfelder. Dies kann Library of Congress Subjects, FAST und andere Schlagwörter enthalten, einschließlich Genre/Form-Begriffe.
-   **Effektive Signatur (Exemplar), Regalordnung**. Ruft Instanzdatensätze ab, die auf dem Regalordnungselement im Exemplardatensatz basieren.
-   **Titel-HRID**. Von Menschen lesbarer Identifikator für den Instanzdatensatz.
-   **Instanz-UUID**. Universell eindeutiger Bezeichner für den Instanzdatensatz.
-   **Normdaten-UUID.** (Fehlt in Originaldoku?)
-   **Alle**. Durchsucht alle Felder in allen Datensatztypen. Kann die Leistung beeinträchtigen.
-   **CQL-Suche (Experte)**. Eine Suche für fortgeschrittene Personen zur Abfrage nach Eigenschaftsnamen mit CQL.

Tab Browsen (exklusive Felder)

-   Browsen von **Signaturen**. Die Suche nach Signaturnummern basiert auf dem Element Regalordnung im Exemplardatensatz; es werden nur Exemplare mit Exemplardatensätzen abgerufen. Sie umfasst LC-, Dewey Decimal-, NLM-, SuDoc- und lokale Signaturen.
-   Browsen von **Mitwirkenden**. Die Suche nach Mitwirkenden basiert auf dem Feld Mitwirkende in Instanzdatensätzen. Die Namen so eingeben, wie sie im Mitwirkenden-Feld erscheinen.
-   Browsen von **Schlagwörter**. Die Schlagwortsuche basiert auf dem Schlagwort-Feld in Instanzdatensätzen.

Tab Bestand (exklusive Felder)

-   **Signatur, lesbar**. Erfordert die Eingabe der Signatur genau so, wie sie im Bestandsdatensatz erscheint, einschließlich Interpunktion.
-   **Signatur, normalisiert**. Ignoriert alle Zeichen außer Zahlen und Buchstaben, wie z.B. Interpunktionszeichen und Leerzeichen.
-   **Bestandsvormerkungen (alle)**. Stichwortsuche über alle Vormerkungen, einschließlich der Verwaltungsnotizen.
-   **Exemplarverwaltungsnotizen**. Stichwortsuche nach Verwaltungsnotizen zu Bestandsdatensätzen.
-   **Bestands-HRID** . Von Menschen lesbarer Identifikator für den Bestandsdatensatz.
-   **Bestands-UUID**. Universell eindeutiger Identifikator für den Bestandsdatensatz.

Tab Exemplar (exklusive Felder)

-   **Barcode**. Ermöglicht Ihnen das Scannen, Kopieren/Einfügen oder Eingeben eines Barcodes.
-   **Effektive Signatur (Exemplar), lesbar**. Erfordert die Eingabe der Signatur genau so, wie sie im Bestandsdatensatz erscheint, einschließlich der Interpunktion und des Signatur-Präfixes.
-   **Effektive Signatur (Exemplar), normalisiert**. Ignoriert alle Zeichen außer Zahlen und Buchstaben, wie z.B. Interpunktionszeichen und Leerzeichen.
-   **Exemplaranmerkungen(alle)**. Stichwortsuche über alle Exemplare; einschließlich Verwaltungsnotizen, Anmerkungen zur Rückgabe und Ausleihe.
-   **Exemplarverwaltungsnotizen**. Stichwortsuche in den Verwaltungsnotizen des Exemplardatensatzes.
-   **Ausleihanmerkungen**. Stichwortsuche in den Anmerkungen zur Rückgabe und Ausleihe.
-   **Exemplar-HRID**. Von Menschen lesbarer Identifikator für den Exemplardatensatz.
-   **Exemplar-UUID**. Universell eindeutiger Identifikator für den Exemplardatensatz.

Es kann auch nach Instanze, Bestandsdatensätzen oder Exemplaren gesucht werden, indem einer der Filter in der **Ansicht Suchen & Filtern** ausgewählt wird. Außerdem können die Filter nach einer Suche angewendet werden, um die Ergebnisse einzuschränken. Die verfügbaren Filter hängen davon ab, ob nach einer Instanz, einem Bestand oder einem Exemplar-Datensatz gesucht wird. Weitere Informationen sind in den folgenden Abschnitten zu finden.

Wenn Filter verwendet werden, sollte Folgendes beachten werden:

-   Mehrere Filter können kombiniert werden, um die Suche weiter einzuschränken.
-   Mehrere Werte in demselben Filter werden mit "ODER" kombiniert.
-   Mehrere Werte in verschiedenen Filtern werden mit "UND" kombiniert.

Eine Suche, die nach mehreren Standorten gefiltert ist, findet beispielsweise Ressourcen, die mit einem dieser Standorte übereinstimmen. Eine Suche, die nach einem Standort und einer Sprache gefiltert wird, findet jedoch Ressourcen an diesem Standort und in dieser Sprache.

## Tab Instanz/Alle

### Effektiver Standort (Exemplar)

Um nach Instanzen, Beständen oder Exemplaren anhand ihres effektiven Standorts zu suchen, folgendermaßen vorgehen:

1.  In der Ansicht **Suchen & Filtern** unter **Effektiver Standort (Exemplar)** auf die Dropdown-Liste klicken.
2.  Entweder den Standort eingeben oder ihn aus der Liste auswählen.
3.  Schritt 2 wiederholen, um mehr als einen Standort hinzuzufügen. Die Suchergebnisse werden in der Ansicht Katalog angezeigt.

### Sprache

Um nach Instanzen in einer bestimmten Sprache zu suchen, folgendermaßen vorgehen:

1.  In der Ansicht **Suchen & Filtern** auf **Sprache** klicken.
2.  Auf die Dropdown-Liste klicken und entweder die Sprache eingeben oder sie aus der Liste auswählen.
3.  Schritt 2 wiederholen, um mehr als eine Sprache hinzuzufügen. Die Suchergebnisse werden in der Ansicht Katalog angezeigt.

### Ressourcentyp

Um nach Instanzen mit einem bestimmten Ressourcentyp zu suchen, wie folgt vorgehen:

1.  In der Ansicht **Suchen & Filtern** auf **Ressourcentyp** klicken.
2.  Auf die Dropdown-Liste klicken und entweder den Ressourcentyp eingeben oder ihn aus der Liste auswählen.
3.  Schritt 2 wiederholen, um mehr als einen Ressourcentyp hinzuzufügen. Die Suchergebnisse werden in der Ansicht Katalog angezeigt.

### Format

Um nach Instanzen mit einem bestimmten Format zu suchen, folgendermaßen vorgehen:

1.  In der Ansicht **Suchen & Filtern** auf **Format** klicken.
2.  Auf die Dropdown-Liste und klicken entweder das Format eingeben oder es aus der Liste auswählen.
3.  Schritt 2 wiederholen, um mehr als ein Format hinzuzufügen. Die Suchergebnisse werden in der Ansicht Katalog angezeigt.

### Erscheinungsweise

Folgendermaßen vorgehen, um nach Instanzen auf der Grundlage ihrer Erscheinungsweise zu suchen:

1.  In der Ansicht **Suchen & Filtern** auf **Erscheinungsweise** klicken.
2.  Auf die Dropdown-Liste und klicken entweder den Modus eingeben oder ihn aus der Liste auswählen.
3.  Schritt 2 wiederholen, um mehr als einen Modus hinzuzufügen. Die Suchergebnisse werden in der Ansicht Katalog angezeigt.

### Art des Inhalts

Die folgenden Schritte ausführen, um nach Instanzen auf der Grundlage ihrer Art des Inhalts zu suchen:

1.  In der Ansicht **Suchen & Filtern** auf **Art des Inhalts** klicken.
2.  Auf die Dropdown-Liste klicken und entweder die Art des Inhalts eingeben oder sie aus der Liste auswählen.
3.  Schritt 2 wiederholen, um mehr als eine Art von Inhalt hinzuzufügen. Die Suchergebnisse werden in der Ansicht Katalog angezeigt.

### Unterdrückt für Mitarbeitende

Um Instanzen zu suchen, die für Mitarbeiter unterdrückt sind oder nicht, in der Ansicht **Suchen & Filtern** auf **Unterdrückt für Mitarbeitende** klicken und eine der folgenden Möglichkeiten wählen:

-   **Ja**, die Instanz ist für Mitarbeiter unterdrückt.
-   **Nein**. Die Instanz ist für Mitarbeiter nicht unterdrückt.

### Nachweis unterdrückt

Um Instanzen, Bestände oder Exemplare zu suchen, die bei der Suche unterdrückt werden oder nicht, in der Ansicht **Suchen & Filtern** auf Nachweis unterdrückt klicken und eine der folgenden Optionen wählen:

-   **Ja**. Die Instanz, der Betrieb oder das Exemplar wird von der Suche unterdrückt.
-   **Nein**. Die Instanz, der Betrieb oder das Exemplar wird nicht von der Entdeckung ausgeschlossen.

### Statistischer Code

Um nach Instanzen, Beständen oder Exemplaren anhand ihres statistischen Codes zu suchen, wie folgt vorgehen:

1.  In der Ansicht **Suchen & Filtern** auf **Statistischer Code** klicken.
2.  Auf die Dropdown-Liste klicken und den Code/Codenamen eingeben oder ihn aus der Liste auswählen.
3.  Schritt 2 wiederholen, um mehr als einen statistischen Code hinzuzufügen. Die Suchergebnisse werden in der Ansicht Katalog angezeigt.

### Erstellungsdatum

Folgendermaßen vorgehen, um nach Instanzen anhand des Erstellungsdatums zu suchen:

1.  In der Ansicht **Suchen & Filtern** auf **Erstellungsdatum** klicken.
2.  Ein Startdatum in das Feld **Von** und ein Enddatum in das Feld **Bis** eingeben.
3.  Auf **Anwenden** klicken. Die Suchergebnisse werden in der Ansicht Katalog angezeigt.

### Datum der Aktualisierung

Folgendermaßen vorgehen, um nach Instanzen anhand des Datums der letzten Aktualisierung zu suchen:

1.  In der Ansicht **Suchen & Filtern** auf **Aktualisierungsdatum** klicken.
2.  Ein Startdatum in das Feld **Von** und ein Enddatum in das Feld **Bis** eingeben.
3.  Auf **Anwenden** klicken. Die Suchergebnisse werden in der Ansicht Katalog angezeigt.

### Instanzstatus

Folgendermaßen vorgehen, um nach Instanzen auf der Grundlage des Instanzstatus zu suchen:

1.  In der Ansicht **Suchen & Filtern** auf **Instanzstatus** klicken.
2.  Den Status aus der Liste auswählen.
3.  Schritt 2 wiederholen, um mehrere Instanzstatus auszuwählen.
4.  Die Suchergebnisse werden in der Ansicht Katalog angezeigt.

### Quelle

Folgendermaßen vorgehen, um nach Instanzen auf der Grundlage ihrer Quelle zu suchen:

1.  In der Ansicht **Suchen & Filtern** auf **Quelle** klicken.
2.  Die Quelle aus der Liste auswählen.
3.  Schritt 2 wiederholen, um mehrere Quellen auszuwählen.
4.  Die Suchergebnisse werden in der Ansicht Katalog angezeigt.

Anmerkung: Die Quellen können von Institution zu Institution unterschiedlich sein. Im Folgenden sind Beispiele für Quellen, die angezeigt werden können:

-   **FOLIO**. Die Instanz wurde in FOLIO erstellt.
-   **MARC**. Die Instanz wurde durch das Hochladen von MARC-Datensätzen erstellt.

### Tags

Folgendermaßen vorgehen, um nach Instanzen auf der Grundlage von zugewiesenen Tags zu suchen:

-   In der Ansicht **Suchen & Filtern** auf **Tags** klicken.
-   Auf die Dropdown-Liste klicken und entweder das Tag eingeben oder es aus der Liste auswählen.
-   Schritt 2 wiederholen, um mehr als ein Tag hinzuzufügen. Die Suchergebnisse werden in der Ansicht Katalog angezeigt.

## Tab Bestand (exklusive Felder)

### Dauerhafter Standort des Bestandes

Um nach Beständen oder Exemplaren anhand ihres dauerhaften Standorts zu suchen, wie folgt vorgehen:

1.  In der Ansicht **Suchen & Filtern** auf **Dauerhafter Standort von Beständen** klicken.
2.  Auf die Dropdown-Liste klicken und entweder den Dauerhaften Standort des Bestands eingeben oder ihn aus der Liste auswählen.
3.  Schritt 2 wiederholen, wenn mehr als einen Dauerhafter Standort für einen Bestand hinzugefügt werden soll. Die Suchergebnisse werden in der Ansicht Katalog angezeigt.

### Bestandstyp

Folgendermaßen vorgehen, um nach Beständen oder Exemplaren auf der Grundlage ihres Bestandtyps zu suchen:

1.  In der Ansicht **Suchen & Filtern** auf **Bestandstyp** klicken.
2.  Auf die Dropdown-Liste klicken und entweder den Bestandstyp eingeben oder ihn aus der Liste auswählen.
3.  Schritt 2 wiederholen, um mehr als einen Bestandstyp hinzuzufügen. Die Suchergebnisse werden in der Ansicht Katalog angezeigt.

## Tab Exemplar (exklusive Felder)

### Exemplarstatus

Um Exemplare anhand ihres Exemplarstatus zu suchen, folgendermaßen vorgehen:

1.  In der Ansicht **Suchen & Filtern** unter **Exemplarstatus** auf die Dropdown-Liste klicken.
2.  Entweder den Exemplarstatus eingeben oder ihn aus der Liste auswählen.
3.  Schritt 2 wiederholen, um mehr als einen Status hinzuzufügen. Die Suchergebnisse werden in der Ansicht Katalog angezeigt.

### Materialart

Folgendermaßen vorgehen, um nach Ressourcen anhand ihrer Materialart zu suchen:

1.  In der Ansicht **Suchen & Filtern** auf **Materialart** klicken.
2.  Auf die Dropdown-Liste klicken und entweder die Materialart eingeben oder sie aus der Liste auswählen.
3.  Schritt 2 wiederholen, um mehr als eine Materialart hinzuzufügen. Die Suchergebnisse werden in der Ansicht Katalog angezeigt.
