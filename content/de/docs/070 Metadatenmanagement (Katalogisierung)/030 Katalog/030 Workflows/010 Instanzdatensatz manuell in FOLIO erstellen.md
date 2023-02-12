---
title: "Instanzdatensatz manuell in FOLIO erstellen"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [app-katalog, by-folio, cat-workflows, for-anwender, meta-uebersetzungsproblem]
weight: 10
Description: "
    Quellen: [Folio](https://docs.folio.org/docs/metadata/inventory/#creating-an-instance-record-manually-in-folio) & [GBV](https://info.gbv.de/display/FOLIOGBVEXTERN/Folio:+Instanzdatensatz+manuell+in+FOLIO+erstellen)
    "
---

1.  In der Ansicht Katalog auf **Aktionen > Neu** klicken.
2.  Im Fenster **Neue Instanz** die Administrative Daten, Titeldaten, Identifikator, Mitwirkende/-r, Beschreibende Daten, Anmerkungen zur Instanz, Elektronischer Zugang, Schlagwort, Klassifikation, Instanz-Beziehung (analytisch und Konvolut) und Verwandte Instanzen aus. Weitere Informationen zu den Feldern und Aktionen, die in diesen Abschnitten verfügbar sind, sind in den Abschnittsbeschreibungen weiter unten zu finden.
3.  Sobald alle gewünschten Informationen in den Instanzdatensatz aufgenommen wurden, auf **Speichern & schließen** klicken. Der Instanzdatensatz wird gespeichert.

## Administrative Daten

Der Abschnitt Verwaltungsdaten enthält technische Informationen über den Instanzdatensatz.

* **Nachweis unterdrücken**. Wenn gewünscht ist, dass der Datensatz im Discoverysystem unterdrückt wird, die Checkbox **Nachweis unterdrücken** markieren.
* **Unterdrückt für Mitarbeitende**. Wenn der Datensatz und die zugehörigen Bestandsdatensätze und Exemplardatensätze für Mitarbeitern unterdrückt werden sollen, die nicht über die entsprechenden Berechtigungen zum Anzeigen des Datensatzes verfügen, die Checkbox **Unterdrückt für Mitarbeitende** markieren. Wenn dieses Kontrollkästchen aktiviert wird, müssen Mitarbeitende die Berechtigung "Katalog: Für das Personal unterdrückte Instanzdatensätze anzeigen." besitzen, um den Datensatz anzeigen zu können.
* **Zuvor in Besitz**. Wenn die Ressource bereits im Besitz der Bibliothek war, die Checkbox **Zuvor in Besitz** markieren. Eine Bibliothek kann die Checkbox Zuvor in Besitz wählen, wenn die Bibliothek die im Instanzdatensatz beschriebene bibliografische Ressource nicht mehr besitzt, den Datensatz aber aus verwaltungstechnischen Gründen im Katalog beibehalten und den früheren Besitz angeben möchte. So kann z.B. die Erlaubnis für Personen, Exemplare in einer Konsortialsammlung einzusehen oder zu benutzen, den Nachweis erfordern, dass die Bibliothek zu irgendeinem Zeitpunkt Eigentümerin dieser Exemplare war.
* **Titel-HRID**. Der Human Readable Identifier ("Menschenlesbare ID"), eine vom System zugewiesene sequentielle ID.
* **Metadatenquelle (erforderlich)**. Format des Instanzdatensatzes, wenn ein Quelldatensatz vorhanden ist. Zum Beispiel FOLIO, wenn es sich um einen in Katalog erstellten Datensatz handelt, MARC, wenn es sich um einen in MARCcat erstellten MARC-Datensatz handelt, oder EPKB, wenn es sich um einen Datensatz aus eHoldings handelt. Das System ordnet die Quelle automatisch zu.
* **Katalogisierungsdatum**. Datum, an dem eine Instanz als "katalogisiert" gilt.
* **Instanz-Statustyp**. Wählen Sie den Typ des Instanzstatus, der dem Datensatz zugewiesen werden soll. Der Instanzstatus kann z.B. sein: katalogisiert, nicht katalogisiert, per Batch eingespielt oder noch nicht zugewiesen. Die Instanz-Statusbegriffe werden von der Bibliothek in der App Einstellungen konfiguriert. Weitere Informationen sind unter [Einstellungen > Katalog > Instanz-Statustyp](https://info.gbv.de/display/FOLIOGBVEXTERN/Einstellungen+%28Katalog%29%3A+Instanz-Statustypen) zu finden.
* **Erscheinungsweise**. Eine bibliografische Kategorisierung, die angibt, ob eine Ressource in einem oder mehreren Teilen ausgegeben wird, wie sie aktualisiert wird und ob ihr Abschluss festgelegt ist oder nicht. Die Werte, die in der Dropdown-Liste unter Einstellungen > Katalog > Erscheinungsweisen erscheinen, können konfiguriert werden. Für in FOLIO erstellte Datensätze kann ein Wert zugewiesen werden, aber für Instanzdatensätze mit einem zugrundeliegenden MARC-Datensatz in der SRS-Datenbank wird der Wert anhand der festen MARC-Feldwerte bestimmt.
* **Statistischer Code**. Statistische Codes sind lokal zugewiesene Werte, die zum Filtern und Sortieren von Datensätzen verwendet werden. Einem Datensatz können mehrere statistische Codes hinzugefügt werden. Statistische Codes werden von der Bibliothek in der App Einstellungen konfiguriert. Siehe [Einstellungen > Katalog > Statistische Codes](https://info.gbv.de/display/FOLIOGBVEXTERN/Einstellungen+%28Katalog%29%3A+Statistische+Codes) für weitere Informationen.
* **Verwaltungsnotizen**. Verwaltungsnotizen sind Freitextfelder, in denen Informationen über den Instanzdatensatz oder die damit durchgeführten Aktionen erfasst werden können.

### Statistische Codes

#### Statistischen Code hinzufügen

1.  Auf **Statistischen Code hinzufügen** klicken.
2.  Den statistischen Code aus der Dropdown-Liste auswählen.
3.  Die Schritte 1-2 je nach Bedarf wiederholen. Der statistische Code wird gespeichert, sobald die Instanz gespeichert wird.

#### Statistischen Code löschen

1.  Den statistischen Code suchen, der gelöscht werden soll.
2.  Auf das **Mülleimersymbol** neben dem Code klicken. Der Code wird aus dem Datensatz entfernt und ist gelöscht, sobald die Instanz gespeichert wird.

### Verwaltungsnotiz

#### Verwaltungsnotiz hinzufügen

1.  Auf **Verwaltungsnotiz hinzufügen** klicken.
2.  Den Text eingeben.
3.  Die Schritte 1-2 je nach Bedarf wiederholen. Die Verwaltungsnotiz wird gespeichert, sobald die Instanz gespeichert wird.

#### Verwaltungsnotiz löschen

1.  Auf das Mülleimersymbol neben der administrativen Anmerkung klicken, die gelöscht werden soll. Die Notiz wird aus dem Datensatz entfernt und gelöscht, sobald die Instanz gespeichert wird.

## Titeldaten

Der Abschnitt Titeldaten enthält Informationen über den Titel der Ressource.

1.  **Ressourcentitel (erforderlich)**. Der primäre Titel (oder die Bezeichnung), der mit der Ressource verbunden ist.
2.  **Alternative Titel**. Ein alternativer Titel für die Ressource. Zum Beispiel der Titel der originalen Sprachversion eines Films. Es können mehrere alternative Titel zu einem Datensatz hinzugefügt werden.
3.  **Indextitel**. Ein Titel, der für das Browsen und die Suche auf der Grundlage des Titels ohne Artikel (der, die, das etc.) am Anfang normalisiert wurde.
4.  **Gesamttitelangaben**. Ein Reihentitel, der mit der Ressource verknüpft ist. Zum Beispiel Harry Potter oder Lecture Notes in Mathematics.
5.  **Vorgängertitel**. Der unmittelbar vorangehende Titel, mit dem die Ressource früher identifiziert wurde. Es können mehrere Vorgängertitel zu einem Datensatz hinzugefügt werden. So kann es beispielsweise mehrere Vorgängertitel geben, die zu dem einen aktuellen Titel zusammengeführt wurden.
6.  **Nachfolgetitel**. Der unmittelbar nachfolgende Titel der Ressource. Es können mehrere Nachfolgetitel zu einem Datensatz hinzugefügt werden. So kann es beispielsweise mehrere Nachfolgetitel geben, wenn die aktuelle Veröffentlichung in mehrere Nachfolgepublikationen aufgeteilt wird.

### Alternativen Titel hinzufügen

1.  Auf **Alternativen Titel hinzufügen** klicken.
2.  Den **Typ** des alternativen Titels aus der Dropdown-Liste wählen. Alternative Titeltypen werden von der Bibliothek in der App Einstellungen konfiguriert. Weitere Informationen sind unter [Einstellungen > Katalog > Alternative Titelarten](https://info.gbv.de/display/FOLIOGBVEXTERN/Einstellungen+%28Katalog%29%3A+Alternative+Titelarten) zu finden.
3.  Den **alternativen Titel** in das Feld eingeben.
4.  Die Schritte 1-3 je nach Bedarf wiederholen. Der alternative Titel wird gespeichert, sobald die Instanz gespeichert wird.

### Gesamttitelangabe hinzufügen

1.  Auf **Gesamttitel hinzufügen** klicken.
2.  Den Gesamttitel in das Feld eingeben.
3.  Bei Bedarf die Schritte 1-2 wiederholen. Die Gesamttitelangabe wird gespeichert, sobald die Instanz gespeichert wird.

### Vorgängertitel hinzufügen

Anmerkung: Das Hinzufügen eines Vorgängertitels ist optional, aber wenn auf Vorgängertitel hinzufügen geklickt wird, muss ein Titel eingeben oder den Vorgängertitel gelöscht werden, um den Instanzdatensatz zu speichern.

1.  Auf **Vorgängertitel hinzufügen** klicken.
2.  Den **Titel** in das Feld eingeben oder die folgenden Schritte ausführen, um den Vorgängertitel mit einer anderen Instanz in dem Katalog zu verbinden:
    1.  Auf das **+** klicken.
    2.  Im Dialog **Instanz auswählen** in der Ansicht **Suchen & Filtern** den gesamten oder einen Teil des Titels in das Suchfeld eingeben und auf **Suchen** klicken.
    3.  Optional: Die Ergebnisse nach Sprache, Ressourcentyp oder Standort filtern.
    4.  In der Ansicht der **Suchergebnisse** auf den Titel klicekn, um ihn auszuwählen. Der Titel ist mit dem Instanzdatensatz als Vorgängertitel verknüpft. Die Felder "Titel", "Instanz-HRID", "ISBN" und "ISSN" werden automatisch mit den Informationen aus dem Datensatz gefüllt, und "Nicht verbunden" ändert sich in "Verbunden".
3.  Optional: Wenn der Titel nicht mit einer anderen Instanz verknüpft wurde, die ISBN oder ISSN in die entsprechenden Felder eingeben.
4.  Die Schritte 1-3 je nach Bedarf wiederholen. Der vorhergehende Titel wird gespeichert, sobald die Instanz gespeichert wird.

### Nachfolgetitel hinzufügen

Anmerkung: Das Hinzufügen eines Nachfolgetitels ist optional, aber wenn auf Nachfolgetitel hinzufügen geklickt wird, muss einen Titel eingeben oder den Nachfolgetitel gelöscht werden, um den Instanzdatensatz zu speichern.

1.  Auf **Nachfolgetitel hinzufügen** klicken.
2.  Den **Titel** in das Feld eingeben oder die folgenden Schritte ausführen, um eine Verbindung zu dem Nachfolgetitel herzustellen, der durch eine andere Instanz in dem Katalog repräsentiert wird:
    1.  Auf das **+** klicken.
    2.  Im Dialog **Instanz auswählen** in der Ansicht **Suchen & Filtern** den gesamten oder einen Teil des Titels in das Suchfeld eingeben und auf **Suchen** klicken.
    3.  Optional: Die Ergebnisse nach Sprache, Ressourcentyp oder Standort filtern.
    4.  In der Ansicht der Suchergebnisse auf den Titel klicken, um ihn auszuwählen. Der Titel wird als Nachfolgetitel mit dem Instanzdatensatz verbunden. Die Felder "Titel", "Instanz-HRID", "ISBN" und "ISSN" werden automatisch mit den Informationen aus dem Datensatz gefüllt, und "Nicht verbunden" ändert sich in "Verbunden".
3.  Optional: Wenn der Titel nicht mit einer anderen Instanz verknüpft wurde, die ISBN oder ISSN in die entsprechenden Felder eingeben.
4.  Die Schritte 1-3 je nach Bedarf wiederholen. Der Nachfolgetitel wird gespeichert, sobald die Instanz gespeichert wird.

### Löschen eines alternativen Titels, eines Vorgängertitels, eines Nachfolgetitels oder einer Gesamttitelangabe

1.  Den alternativen Titel, den Vorgängertitel, den Nachfolgetitel oder die Gesamttitelangaben suchen, die gelöscht werden sollen.
2.  Auf das **Mülleimersymbol** neben dem alternativen Titel, Vorgängertitel, Nachfolgetitel oder den Gesamttitelangaben klicken. Der alternative Titel, der Vorgängertitel, der Nachfolgetitel oder die Gesamttitelangabe wird aus dem Datensatz entfernt und gelöscht, sobald Sie Instanz gespeichert wird.

## Identifikator

Ein erweiterbarer Satz von Name-Wert-Paaren von Identifikatoren, die mit der Ressource verbunden sind.

### Identifikator hinzufügen

Anmerkung: Das Hinzufügen eines Identifikators ist optional, aber wenn ein Identifikator hinzufügen geklickt wird, muss ein Typ eingeben oder der Identifikator gelöscht werden, um den Instanzdatensatz zu speichern.

1.  Auf **Identifikator hinzufügen** klicken.
2.  Den **Typ** aus der Dropdown-Liste wählen. Die Identifikatortypen werden von der Bibliothek in der App Einstellungen konfiguriert. Weitere Informationen sind unter [Einstellungen > Katalog > Ressourcen-Identifikatorentypen](https://info.gbv.de/display/FOLIOGBVEXTERN/Einstellungen+%28Katalog%29%3A+Ressourcen-Identifikatorentypen) zu finden.
3.  Den Identifikator in das Feld eingeben.
4.  Die Schritte 1-3 je nach Bedarf wiederholen. Der Identifikator wird gespeichert, sobald die Instanz gespeichert wird.

### Identifikator löschen

1.  Den Identifikator suchen, der gelöscht werden soll.
2.  Auf das **Mülleimersymbol** neben dem Identifikator klicken. Der Identifikator wird aus der Anzeige des Bearbeitungsdatensatzes entfernt und dauerhaft gelöscht, sobald die Instanz gespeichert wird.

## Mitwirkende/-r

Mitwirkende sind Personen, die einen Beitrag zur bibliografischen Ressource geleistet haben.

### Mitwirkende hinzufügen

Anmerkung: Das Hinzufügen eines Mitwirkenden ist optional, aber wenn auf **Mitwirkende/-n hinzufügen** geklickt wird, muss ein Namen und einen Namenstyp eingeben  oder der Mitwirkenden gelöscht werden, um den Instanzdatensatz zu speichern.

1.  Auf **Mitwirkende/-n hinzufügen** klicken.
2.  Den **Namen** in das Feld eingeben.
3.  Den **Namenstyp** aus der Dropdown-Liste auswählen.
4.  Optional: Den **Typ** des Mitwirkenden aus der Dropdown-Liste wählen. Die Typen der Mitwirkenden werden von der Bibliothek in der App Einstellungen konfiguriert. Weitere Informationen sind unter [Einstellungen > Katalog > Typen von Mitwirkenden](https://info.gbv.de/display/FOLIOGBVEXTERN/Einstellungen+%28Katalog%29%3A+Typen+von+Mitwirkenden) zu finden.
5.  Optional: Einen Rollentyp in das Feld **Typ, Freitext** eingeben.
6.  Optional: Auf **Primär** klicken, um den Mitwirkenden zum primären Mitwirkenden zu machen.
7.  Die Schritte 1-6 je nach Bedarf wiederholen. Der Mitwirkende wird gespeichert, sobald die Instanz gespeichert wird.

### Mitwirkende löschen

1.  Den Mitwirkenden suchen, der gelöscht werden soll.
2.  Auf das **Mülleimersymbol** neben dem Mitwirkenden klicken. Der Mitwirkende wird aus dem Datensatz entfernt und gelöscht, sobald die Instanz gespeichert wird.

## Beschreibende Daten

Beschreibende Daten enthalten deskriptive Informationen über die Ressource.

* **Erscheinungsvermerk**. Daten über die Ressource, die sich auf ihre Veröffentlichung, Verbreitung, Herstellung usw. beziehen.
* **Ausgabevermerk**. Die Angabe zur Ausgabe.
* **Physische Beschreibungen**. Physische Beschreibung der beschriebenen Ressource, einschließlich ihres Umfangs, ihrer Abmessungen und anderer physischer Details.
* **Ressourcentyp (erforderlich)**. Ein eindeutiger Begriff für die Ressource, der aus der Liste der RDA-Inhaltsbegriffe zugewiesen oder lokal definiert werden kann. Wird unter Einstellungen > Katalog > Ressourcentypen konfiguriert.
* **Art des Inhalts**. Die Art des Inhalts ist eine RDA-Kategorisierung.
* **Formate**. Ein eindeutiger Zeitraum für das Format, der aus der RDA-Trägerbegriffsliste ("RDA carrier term list") zugewiesen oder lokal definiert werden kann. Konfiguriert unter [Einstellungen > Katalog > Formate](https://info.gbv.de/display/FOLIOGBVEXTERN/Einstellungen+%28Katalog%29%3A+Formate).
* **Sprachen**. Die von der Ressource verwendete Sprachen.
* **Erscheinungsweise**. Das Intervall, in dem Serienausgaben veröffentlicht werden oder eine integrierende Ressource ("integrating resource") aktualisiert wird. Zum Beispiel täglich, wöchentlich, monatlich, vierteljährlich, usw.
* **Veröffentlichungszeitraum**. Fortlaufenden Bezeichnung/Chronologie der Veröffentlichung, oder Datumsbereich.

### Erscheinungsvermerk hinzufügen

Anmerkung: Das Hinzufügen von Erscheinungsvermerken ist optional, aber wenn Erscheinungsvermerk hinzufügen geklickt wird, muss ein Verlags-, Orts- oder Erscheinungsdatum eingeben oder der Erscheinungsvermerk gelöscht werden, um den Instanzdatensatz zu speichern.

1.  Auf **Erscheinungsvermerk hinzufügen** klicken.
2.  Optional: Einen **Verlag** in das Feld eingeben.
3.  Optional: Eine **Verlagsrolle** in das Feld eingeben.
4.  Optional: Einen **Erscheinungsort** in das Feld eingeben.
5.  Optional: Ein **Erscheinungsdatum** in das Feld eingeben.
6.  Die Schritte 1-5 je nach Bedarf wiederholen. Die Erscheinungsvermerke werden gespeichert, sobald die Instanz gespeichert wird.

### Ausgabevermerk hinzufügen

1.  Auf **Ausgabevermerk hinzufügen** klicken.
2.  Die **Ausgabe** in das Feld eingeben.
3.  Die Schritte 1-2 je nach Bedarf wiederholen. Die Angabe der Ausgabe wird gespeichert, sobald die Instanz gespeichert wird.

### Physische Beschreibung hinzufügen

1.  Auf **Beschreibung hinzufügen** klicken.
2.  Eine **physische Beschreibung** in das Feld eingeben.
3.  Die Schritte 1-2 je nach Bedarf wiederholen. Die physische Beschreibung wird gespeichert, sobald die Instanz gespeichert wird.

### Art des Inhalts hinzufügen

1.  Auf **Art des Inhalts hinzufügen** klicken.
2.  Die  **Art des Inhalts (Begriff)** aus der Dropdown-Liste wählen.
3.  Die Schritte 1-2 je nach Bedarf wiederholen. Die Art des Inhalts wird gespeichert, sobald die Instanz gespeichert wird.

### Format hinzufügen

1.  Auf **Format hinzufügen** klicken.
2.  Das **Format** aus der Dropdown-Liste wählen.
3.  Die Schritte 1-2 je nach Bedarf wiederholen. Das Format wird gespeichert, sobald die Instanz gespeichert wird.

### Sprache hinzufügen

Anmerkung: Das Hinzufügen einer Sprache ist optional, aber wenn auf **Sprache hinzufügen** geklickt wird, muss eine Sprache eingeben oder die Sprache gelöscht werden, um den Instanzdatensatz zu speichern.

1.  Auf **Sprache hinzufügen** klicken.
2.  Die **Sprache** aus der Dropdown-Liste wählen.
3.  Die Schritte 1-2 je nach Bedarf wiederholen. Die Sprache wird gespeichert, sobald die Instanz gespeichert wird.

### Erscheinungsweise hinzufügen

1.  Auf **Erscheinungsweise hinzufügen** klicken.
2.  Die Erscheinungsweise in das Feld eingeben.
3.  Die Schritte 1-2 je nach Bedarf wiederholen. Die Erscheinungsweise wird gespeichert, sobald die Instanz gespeichert wird.

### Veröffentlichungszeitraum hinzufügen

1.  Auf **Veröffentlichungszeitraum hinzufügen** klicken.
2.  Den **Veröffentlichungszeitraum** in das Feld eingeben.
3.  Die Schritte 1-2 je nach Bedarf wiederholen. Der Veröffentlichungszeitraum wird gespeichert, sobald die Instanz gespeichert wird.

### Löschen eines Erscheinungsvermerk, eines Ausgabevermerk, einer physischen Beschreibung, einer Art des Inhalts, eines Formats, einer Sprache, eines Erscheinungsweises, eines Veröffentlichungszeitraums

1.  Erscheinungsvermerk, Ausgabevermerk, physischen Beschreibung, Art des Inhalts, Format, Sprache, Erscheinungsweise oder Veröffentlichungszeitraum suchen
2.  Auf das **Mülleimersymbol** neben dem Erscheinungsvermerk, Ausgabevermerk, physischen Beschreibung, Art des Inhalts, Format, Sprache, Erscheinungsweise oder Veröffentlichungszeitraum klicken. Der Inhalt wird aus dem Datensatz entfernt und gelöscht, sobald die Instanz gespeichert wird.

## Anmerkungen zur Instanz

Im Bereich Anmerkungen zur Instanz können beliebige Anmerkungen zum Instanzdatensatz hinzugefügt werden.

### Anmerkung hinzufügen

Anmerkung: Das Hinzufügen einer Anmerkung ist optional, aber wenn auf **Anmerkung hinzufügen** geklickt wird, muss eine Anmerkung eingeben oder die Anmerkung gelöscht werden, um den Instanzdatensatz zu speichern.

1.  Auf **Anmerkung hinzufügen** klicken.
2.  Den **Anmerkungstyp** aus der Dropdown-Liste auswählen. Die Werte, die in der Dropdown-Liste erscheinen, können unter [Einstellungen > Katalog > Anmerkungstypen der Instanz](https://info.gbv.de/display/FOLIOGBVEXTERN/Einstellungen+%28Katalog%29%3A+Anmerkungstypen+der+Instanz) konfiguriert werden.
3.  Eine **Anmerkung** in das Feld eingeben.
4.  Optional: Wenn die Anmerkung nur für Mitarbeitende mit der Berechtigung "Katalog: Für das Personal unterdrückte Instanzdatensätze anzeigen" angezeigt werden soll, die Checkbox Nur Personal markieren.
5.  Die Schritte 1-4 nach Bedarf wiederholen. Die Anmerkung wird gespeichert, sobald die Instanz gesüpeichert wird.

### Anmerkung löschen

1.  Die Anmerkung suchen, die gelöscht werden soll.
2.  Auf das **Mülleimersymbol** neben der Anmerkung klicken. Die Anmerkung wird aus dem Datensatz entfernt und gelöscht, sobald die Instanz gespeichert wird.

## Elektronischer Zugang

Im Abschnitt Elektronischer Zugang können Informationen zum Online-Zugang für die Ressource hinzugefügt werden.

### Elektronischen Zugang hinzufügen

Anmerkung: Das Hinzufügen eines elektronischen Zugangs ist optional, aber wenn auf **Elektronischen Zugang hinzufügen** geklickt wird, muss ein URI eingeben oder der elektronischen Zugang gelöscht werden, um die Instanz zu speichern.

1.  Auf **Elektronischen Zugang hinzufügen** klicken.
2.  Optional: Eine **Beziehung** aus der Dropdown-Liste auswählen.
3.  Optional: Eine **URI** in das Feld eingeben.
4.  Optional: Einen **Linktext** in das Feld eingeben.
5.  Optional: Die **Aufgeführten Materialien** in das Feld eingeben.
6.  Optional: Eine **URL öffentliche Anmerkung** in das Feld eingeben.
7.  Die Schritte 1-6 je nach Bedarf wiederholen. Der elektronische Zugang wird gespeichert, sobald die Instanz gespeichert wird.

### Elektronischen Zugang löschen

1.  Den elektronischen Zugang suchen, der gelöscht werden soll.
2.  Auf das **Mülleimersymbol** neben dem elektronischen Zugang klicken. Der elektronische Zugang wird aus dem Datensatz entfernt und ist gelöscht, sobald die Instanz gespeichert wird.

## Schlagwort

Im Abschnitt Schlagwort können alle Schlagwörter hinzugefügt werden, die sich auf die Ressource beziehen.

### Schlagwort hinzufügen

1.  Auf **Schlagwort hinzufügen** klicken.
2.  Das **Schlagwort** in das Feld eingeben.
3.  Die Schritte 1-2 je nach Bedarf wiederholen. Das Schlagwort wird gespeichert, sobald die Instanz gespecihert wird.

### Schlagwort entfernen

1.  Das Schlagwort suchen, das gelöscht werden soll.
2.  Auf das **Mülleimersymbol** neben dem Schlagwort klicken. Das Schlagwort wird aus dem Datensatz entfernt und gelöscht, sobald die Instanz gespeichert wird.

## Klassifikation

Im Abschnitt Klassifikation können Informationen zur Klassifikation der Ressource hinzufügt werden.

### Klassifikation hinzufügen

Anmerkung: Das Hinzufügen einer Klassifikation ist optional, aber wenn Sie auf Klassifikation hinzufügen klicken, müssen Sie einen Klassifikationsidentifikatortyp und eine Klassifikation eingeben oder die Klassifikation löschen, um den Instanzdatensatz zu speichern.

1.  Auf **Klassifikation hinzufügen** klicken.
2.  Einen **Klassifikations-Identifikatorentyp** aus der Dropdown-Liste wählen. Konfiguriert in [Einstellungen > Katalog > Klassifikations-Identifikatorentypen](https://info.gbv.de/display/FOLIOGBVEXTERN/Einstellungen+%28Katalog%29%3A+Klassifikations-Identifikatorentypen).
3.  Eine **Klassifikation** in das Feld eingeben.
4.  Die Schritte 1-3 je nach Bedarf wiederholen. Die Klassifikation wird gespeichert, sobald die Instanz gespeichert wird.

### Klassifikation löschen

1.  Die Klassifikation suchen, die gelöscht werden soll.
2.  Auf das **Mülleimersymbol** neben der Klassifikation klicken. Die Klassifikation wird aus dem Datensatz entfernt und gelöscht, sobald die Instanz gespeichert wird.

## Instanz-Beziehung (analytisch und Konvolut)

Im Abschnitt Instanzbeziehung können beliebige Beziehungen zwischen der Instanz und anderen Instanzen hinzugefügt werden.

* **Übergeordnete Instanzen**. Die übergeordnete Instanz ist der Datensatz, der als primärer Datensatz ausgewählt wurde und mit dem alle anderen untergeordneten Datensätze verknüpft sind. Informationen über übergeordnete Instanzen (Titel, Instanz-HRID, Verlag, Erscheinungsdatum, ISBN, ISSN) einschließlich eines Links zum entsprechenden übergeordneten Instanzdatensatz werden in den Datensätzen der untergeordneten Instanzen angezeigt.
* **Untergeordnete Instanzen**. Ein untergeordneter Instanzdatensatz ist jeder Datensatz, der mit einem übergeordneten Datensatz verknüpft wurde. Informationen über untergeordnete Instanzen (Titel, Instanz-HRID, Verlag, Erscheinungsdatum, ISBN, ISSN) einschließlich eines Links zu jedem entsprechenden untergeordneten Instanzdatensatz werden im übergeordneten Instanzdatensatz angezeigt.

### Übergeordneten Instanz hinzufügen

Anmerkung: Das Hinzufügen einer übergeordneten Instanz ist optional, aber wenn auf **Übergeordnete Instanz hinzufügen** geklickt wird, müssen ein **Titel** und **Art der Beziehung** eingeben oder die übergeordnete Instanz gelöscht (siehe unten) werden, um den Instanzdatensatz zu speichern.

1.  Auf **Übergeordnete Instanz hinzufügen** klicken.
2.  Die **Titel** in das Feld eingeben.
3.  Die **Art der Beziehung** aus der Dropdown-Liste wählen.
4.  Die Schritte 1-3 je nach Bedarf wiederholen. Die übergeordnete Instanz wird gespeichert, sobald die Instanz gespeichert wird.

### Untergeordnete Instanz hinzufügen

Anmerkung: Das Hinzufügen einer untergeordneten Instanz ist optional, aber wenn auf **Untergeordnete Instanz hinzufügen** geklickt wird, müssen ein **Titel** und **Art der Beziehung** eingeben oder die untergeordnete Instanz gelöscht (siehe unten) werden, um den Instanzdatensatz zu speichern.

1.  Auf **Untergeordnete** **Instanz hinzufügen** klicken.
2.  Die **Titel** in das Feld eingeben.
3.  Die **Art der Beziehung** aus der Dropdown-Liste wählen.
4.  Die Schritte 1-3 je nach Bedarf wiederholen. Die untergeordnete Instanz wird gespeichert, sobald die Instanz gespeichert wird.

### Übergeordnete oder untergeordnete Instanz entfernen

1.  Die übergeordnete oder untergeordnete Instanz suchen, die gelöscht werden soll.
2.  Auf das **Mülleimersymbol** neben der übergeordneten oder untergeordneten Instanz klicken. Die über- oder untergeordnete Instanz wird aus dem Datensatz entfernt und gelöscht, sobald die Instanz gespeichert wird.

## Verwandte Instanzen

Der Abschnitt Verwandte Instanzen zeigt alle verknüpften über- oder untergeordneten Instanzen an.
