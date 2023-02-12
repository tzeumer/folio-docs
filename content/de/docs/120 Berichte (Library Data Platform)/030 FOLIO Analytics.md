---
title: "FOLIO Analytics"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [app-ldp, by-folio, for-admin, topic-datenschutz]
weight: 30
Description: "
    Quellen: [Folio](https://docs.folio.org/docs/reporting/folio-analytics/) & [GBV](https://info.gbv.de/display/FOLIOGBVEXTERN/FOLIO+Analytics)
    "
---

## Was ist das FOLIO Analytics-Repository?

Das FOLIO Analytics Repository enthält Berichte und andere Analysen, die für FOLIO entwickelt wurden und auf der Library Data Platform laufen sollen. Die für FOLIO entwickelten Berichte werden als Code gespeichert, der in Structured Query Language (SQL) geschrieben ist. Die SQL-Abfragen können in einer Datenbankabfragesoftware geöffnet werden, um Daten aus der LDP abzurufen.

Eine Einführung in das Repository kann in der übergreifenden [README-Datei](https://github.com/folio-org/folio-analytics/blob/release-1.5/README.md) auf GitHub gelesen werden. Die Datei beschreibt Folgendes:

* Die beiden Arten von SQL-Abfragen, die im Repository zu finden sind:
    * **Berichtsabfragen**, die kopiert und eingefügt werden können, um sie in dem jeweiligen LDP auszuführen.
    * **Abfragen für abgeleitete Tabellen**, die Berichtsabfragen vereinfachen und beschleunigen. Eine abgeleitete Tabelle ist einfach eine Tabelle, die mit Daten aus einer oder mehreren anderen Tabellen erstellt wird. Diese Abfragen werden hinter den Kulissen über die LDP-Verwaltung verwaltet, so dass sie automatisch ausgeführt werden und die abgeleiteten Tabellen in der Datenbank erzeugen.
* Dokumentation für die Abfragen.
* Beispiele für die Software, in der Abfragen ausgeführt werden können.
* Wie die Abfragen im Repository organisiert sind.

Der erste Abschnitt unten beschreibt, wie die Berichtsabfragen im FOLIO Analytics-Repository genutzt werden können, um Berichte über FOLIO-Daten zu erstellen. Andere Abschnitte der Dokumentation behandeln die [Verwaltung von abgeleiteten Tabellen](https://docs.folio.org/docs/reporting/library-data-platform/#setting-up-derived-tables) und die [Verwendung von abgeleiteten Tabellen für Ad-hoc-Abfragen](https://docs.folio.org/docs/reporting/folio-analytics/#ldp-specific-query-guidance).

## Verwendung von Abfragen aus dem FOLIO Analytics Repository

**Die Versionen von FOLIO Analytics sind an eine bestimmte Flower-Version gebunden. Bitte die Versionsmatrix für die Kompatibilität beachten.**

Die Berichtsabfragen im FOLIO Analytics Repository sind in einer bestimmten Struktur aufgebaut, die es leicht machen, die verschiedenen Bereiche zu finden, die benötigt werden, während eigene SQL-Kenntnisse ausgebaut werden.

* **Einleitende Kommentare**. Abfragen können mit einem kurzen Textblock beginnen, der nicht Teil der Abfrage ist. Diese Kommentare beschreiben oft grundlegende Komponenten der Abfrage und geben eine kurze Beschreibung des Zwecks.
* **Parameter**. Um der Person die Arbeit zu erleichtern, enthalten Abfragen in der Regel einen Parameter-Abschnitt am Anfang, in dem die für die Filterung eines Feldes benötigten Werte einfach angeben werden können.
* **Unterabfragen (Subquery)**. Abfragen können mehrere Gruppen von kleineren Abfragen enthalten, die als Unterabfragen bezeichnet werden. Diese Unterabfragen helfen, verschiedene Teile der Datenbank zu vereinfachen und neu anzuordnen, um die endgültige Abfrage zu erleichtern. (Anmerkung: Die offizielle Bezeichnung für diese Teile der Abfrage ist Common Table Expressions oder CTEs. Die Bezeichnung Unterabfragen soll die Rolle unterstreichen, die sie in der größeren Abfrage spielen).
* **Hauptabfrage (Main query)**. Die Hauptabfrage bestimmt das endgültige Aussehen des Berichts. Unter dem Stichwort SELECT ist eine Liste der Felder zu sehen, die im endgültigen Bericht auftauchen werden. Nach dem Schlüsselwort FROM folgt eine Liste der Tabellen, aus denen die Felder stammen. Das Stichwort WHERE gibt die Filter an, die zur Begrenzung der Zeilen im Bericht angewendet werden sollen. Nach dem Schlüsselwort WHERE können weitere Schlüsselwörter erscheinen, um die Ausgabe des Berichts weiter anzupassen. Kommentare können in der Abfrage erscheinen, um Anweisungen oder Klarstellungen zu geben.

### Standort von Abfragen im Repository

Berichtsabfragen werden im Ordner sql/report\_queries des Repositorys gespeichert. Um einen Überblick über die Berichtsabfragen im Repository zu erhalten, bitte die README-Datei im Ordner report\_queries lesen. Es können auch die Unterverzeichnisse im Ordner sql/report\_queries durchsucht werden. Jedes Unterverzeichnis enthält eine oder mehrere SQL-Abfragen zusammen mit einer Dokumentation, die den Zweck und die Ausgabe der Abfragen beschreibt.

### Ausführen von Abfragen in einem Datenbankabfragetool

Sobald eine gewünschten Berichtsabfrage gefunden ist, werden die folgenden Schritte durchgeführt, um die Abfrage auszuführen und einen Bericht zu erstellen:

1.  Den Abfragecode von GitHub kopieren.
2.  Ein Datenbankabfragetool öffnen.
3.  Sich mit der LDP verbinden.
4.  Den SQL-Abfragecode in eine lokale Datei einfügen.
5.  Die SQL-Abfrage ausführen.
6.  Die Abfrageergebnisse im gewünschten Format exportieren.

Der folgende Abschnitt demonstriert diesen Arbeitsablauf anhand von [DBeaver](https://dbeaver.io/), einem Datenbankabfragetool, das über eine kostenlose Community-Version verfügt und für die Betriebssysteme Windows, Mac OSX und Linux verfügbar ist.

#### Beispiel für die Ausführung einer Abfrage mit DBeaver

##### Den Abfragecode von GitHub kopieren

1.  Im Ordner **sql** des [FOLIO Analytics Repository](https://github.com/folio-org/folio-analytics/tree/release-1.5/sql) auf den Ordner **report\_queries** klicken.
2.  Auf den Unterordner für den Bericht klicken, an dem Interesse besteht. Für dieses Beispiel wird die Abfragedatei ACRL Circulation geöffnet, indem zuerst auf den Unterordner **acrl** und dann auf den Unterordner **circulation** geklickt und schließlich auf die Datei **acrl\_circulation**.sql geklickt wird.
3.  Um die Abfragedatei direkt zu öffnen, auf die Schaltfläche **raw** in der oberen rechten Ecke des Dateivorschaufensters klicken.
4.  Um den Abfragecode zu kopieren, Strg-A (Cmd-A auf Mac) drücken, um den gesamten Text zu markieren, gefolgt von Strg-C (Cmd-C auf Mac), um den Text zu kopieren.

###### Ein Datenbankabfragetool öffnen

1.  Die [DBeaver Community-Version](https://dbeaver.io/download/) für das entsprechende Betriebssystem installieren.
2.  DBeaver öffnen.
3.  (Auf Deutsch stellen: In Window > Preferences > User Intferface bei Language German wählen)

###### Verbinden Sie sich mit dem LDP

1.  Um eine LDP-Verbindung hinzuzufügen, auf die Schaltfläche **Neue Datenbankverbindung** im oberen Bereich der Registerkarte Datenbank-Navigator klicken. Sie sollte wie ein elektrischer Stecker mit einem Pluszeichen aussehen.
2.  Im Fenster **Wählen Sie Ihre Datenbank aus**, das sich öffnet, auf das **PostgreSQL**\-Symbol und dann auf **Weiter** klicken.
3.  Den **Verbindungsdatendialog** ausfüllen:
    * Es müssen die folgenden Informationen vom lokalen LDP-Administrator erhalten worden sein:
        * Host (sieht normalerweise wie eine URL aus, z.B. [ldp.institution.edu](http://ldp.institution.edu/))
        * Port (typischerweise 5432)
        * Name der Datenbank
        * Benutzername und Passwort
        * SSL-Modus (wird wahrscheinlich erforderlich sein)
    * Anmerkung: Eine gehostete LDP-Berichtsdatenbank ist derzeit für die FOLIO-Community verfügbar. Sie bietet Zugriff auf Daten aus der FOLIO Referenzumgebung folio-snapshot und wird stündlich aktualisiert. Informationen zur Anmeldung sind in der [Wiki-Dokumentation der Reporting SIG](https://wiki.folio.org/display/RPT/FOLIO+Reporting+Reference+Environment) zu finden.
4.  Zusätzlich zur ersten Seite der Verbindungsdetails muss auf die Registerkarte SSL geklickt und unter SSL-Modus die Option "erforderlich" ausgewählt werden.
5.  Schließlich die Verbindungseinstellungen in der Seitenleiste auf der linken Seite erweitern und die Unterrubrik Initialisierung wählen. Sicherstellen, dass in den Einstellungen auf der rechten Seite, das Kontrollkästchen **Auto-commit** aktiviert ist.
6.  Wenn die Einrichtung der Verbindung abgeschlossen ist, auf der Registerkarte Datenbank-Navigator auf den Verbindungsnamen doppelklicken, um eine Verbindung zur Datenbank herzustellen.

###### Einfügen des SQL-Abfragecodes in eine lokale Datei

1.  Um eine neue Skriptdatei zu erstellen, entweder auf die Schaltfläche **Neuer SQL-Editor** in der Symbolleiste klicken (sie sieht aus wie ein Dokument mit einem Pluszeichen) oder **Neues SQL-Skript** aus dem Menü SQL-Editor wählen.
2.  Wenn mehrere Datenbanken verfügbar sind, wird von DBeaver möglicherweise aufgefordert, die Datenbank auszuwählen, die abgefragt werden soll. Die richtige Datenbank wählen und auf **Auswählen** klicken. Das neue Skript-Fenster sollte auf der rechten Seite angezeigt werden, mit dem Skript-Editor oben und dem Ergebnisfenster (derzeit leer) unten.
3.  Den kopierten Abfragecode von GitHub in den Skript-Editor einfügen. (Sobald die Kopie des Skripts eingefügt wurde, kann sie nach Belieben geändert werden. Dies ist die eigene Kopie der SQL-Abfrage. Weiter unten ist mehr über das Anpassen von Abfragen zu finden und bitte auch dem Abschnitt "Parameter" in der Abfrage besondere Aufmerksamkeit schenken).
4.  Um die Abfrage zu speichern, im Menü Datei die Option Speichern unter wählen und zu dem gewünschten Verzeichnis navigieren, wobei ein Dateinamen mit der Erweiterung ".sql" verwendet werden sollte.

###### Ausführen der SQL-Abfrage

1.  Um die Abfrage auszuführen, entweder auf die Schaltfläche **SQL-Skript ausführen** auf der linken Seite des Skripteditors klicken (es sollte die dritte Schaltfläche von oben sein und wie ein Dokument mit einem "Abspiel"-Symbol darin aussehen) oder **SQL-Skript ausführen** aus dem Menü des SQL-Editors wählen.
2.  Die Ergebnisse werden dann hoffentlich im Ergebnisbereich unterhalb des Skripts angezeigt. Anmerkung: Bei der Abfrage von Teilen der Datenbank mit vielen Daten, wie z.B. den Katalog-Tabellen, kann es zu einer langen Verzögerung kommen, bevor die Ergebnisse zurückgegeben werden.

###### Die Abfrageergebnisse als CSV-Datei exportieren

1.  Um die Ergebnisse zu exportieren, mit der rechten Maustaste in die Ergebnistabelle klicken und **Daten exportieren...** wählen.
2.  Den Datenexport-Assistenten abschließen:
    1.  CSV als Zieltyp für den Datentransfer wählen und auf **Weiter >** klicken.
    2.  Die Einstellungen für den Datentransfer anpassen und auf **Weiter >** klicken.
    3.  Die Ausgabeeinstellungen an (z.B. Ausgabeverzeichnis, Dateinamensmuster) und auf **Weiter >** klicken.
    4.  Die Einstellungen bestätigen und auf **Start** klicken, um die Datei zu exportieren.

##### Abfragen anpassen

Bei vielen Abfragen können die korrekten Werte für Berichtsfilter angeben werden, indem die "Parameter"-Abschnitte oben in der Abfrage bearbeitet werden. **Die Parameter sollten immer überprüft und aktualisiert werden, bevor Abfrage ausgeführt werden.** Wenn die Werte im Abschnitt "Parameter" nicht angepasst werden, werden die Standardwerte verwendet, die in vielen Fällen für die Daten in Ihrer LDP ungeeignet sein können.

Um die Parameterwerte zu bearbeiten, muss nur der gewünschte Wert zwischen den einfachen Anführungszeichen am Anfang einer oder mehrerer Parameterzeilen eingegebn werden. Die Werte müssen genau so eingegeben werden, wie sie in der Datenbank erscheinen. Mögliche Werte werden in den Abfragekommentaren vorgeschlagen (obwohl diese Beispiele in der jeweiligen Institution möglicherweise nicht verwendet werden). Wenn keine Filterung der Daten gewünscht ist, kann alles zwischen den einfachen Anführungszeichen entfernt werden.

Um die Abfrage weiter anzupassen, die Einleitung zu dieser Seite lesen, um die verschiedenen Abschnitte zu identifizieren, die überprüft und geändert werden können. Eine Anpassung, die möglicherweise gewünscht ist, ist das Hinzufügen der eigenen Kommentare, um sich und anderen eine Orientierungshilfe zu geben. Der Kommentartext wird (in DBeaver) grau dargestellt und hat keinen Einfluss auf die Ausführung der Abfrage. Es gibt zwei Möglichkeiten, Kommentare zu erstellen. Wird -- eingeben, wird ein Kommentar aus dem Rest der betreffenden Zeile der Datei erstellt. Um einen Kommentar zu erstellen, der sich über mehrere Zeilen erstreckt, /\* am Anfang des Kommentars und \*/ am Ende des Kommentars verwenden.

Eine weitere Anpassung, die möglicherweise gewünscht ist, ist das Entfernen eines Feldes aus dem Bericht. Dazu im Hauptabschnitt der Abfrage nach dem Stichwort SELECT  suchen (hier ist normalerweise die längste Liste von Feldnamen zu finden). In der Liste der Felder nach dem Schlüsselwort SELECT können die Zeilen gelöscht werden, in denen die Felder aufgeführt sind, die nicht gewünscht sind. Aber darauf achten, dass dem letzten Eintrag in der Liste, der direkt vor dem Schlüsselwort FROM steht, kein Komma folgt.

Weitere fortgeschrittene Techniken zum Schreiben von Abfragen sind in der Dokumentation über Ad-hoc-Abfragen mit LDP-Tabellen unten zu finden.

##### Fehlersuche bei Abfragen

###### Was getan werden kann, wenn keine Ergebnisse erhalten werden

* Prüfen, ob der Berichtserstellende einen Parameter eingegeben hat, der nicht zutrifft. Wenn dies nicht der Fall ist, hier oder in der lokalen (oder weltweite) FOLIO-Community nach zusätzlichen Schulungen suchen.

###### Was tun, wenn Fehler auftreten?

* Prüfen, ob die Fehlermeldung darauf hinweist, dass eine abgeleitete Tabelle fehlt. Diese abgeleiteten Tabellen sind in einem Schema namens folio\_reporting gespeichert, so dass dieser Schemaname gefolgt von einem Tabellennamen in der Fehlermeldung erscheinen kann. Wenn eine abgeleitete Tabelle fehlt, dann an den eigenen LDP-Administrator wenden.
* Wenn die Abfrage bearbeitet wurde, sicherstellen, dass kein Komma am Ende einer Liste steht, wie z.B. in der Liste der Felder nach dem Schlüsselwort SELECT.
* Wenn die Fehlerursache nicht festgestellt werden kann, an den lokalen LDP-Administrator oder entweder an die lokale oder die weltweite [FOLIO Reporting Community](https://docs.folio.org/docs/reporting/support) wenden.

## Ad-hoc-Abfragen mit LDP-Tabellen

Wenn die gemeinsam genutzten Abfragen den Anforderungen nicht genügen, können auch eigenen "Ad-hoc"-Abfragen (oder Abfragen nach Bedarf) entwickelt werden, um Daten aus der LDP zu ziehen. Es können nicht nur Abfragen mit anderen Feldern und Tabellenverbindungen als in den geteilten Abfragen erstellt werden, sondern FOLIO auch mit anderen benutzerdefinierten Tabellen verbunden werden, die in dem lokalen LDP verfügbar sind. Da die LDP auf standardmäßiger relationaler Datenbanksoftware basiert, können Ad-hoc-LDP-Abfragen auf die gleiche Weise erstellt werden, wie Abfragen für jede andere Datenbank erstellt werden würde. indem eine SQL-Abfrage geschrieben und ein Datenbankabfragetool zur Ausführung der Abfrage verwendt wird.

### SQL lernen

Um Ad-hoc-Abfragen zu entwickeln, müssen die Abfrageskripte mit der Structured Query Language (SQL) geschrieben werden. In der folgenden Tabelle sind einige Ressourcen zum Erlernen von SQL zu finden. (Nur Englischsprachig)

|Training Resource|Beschreibung|
|:----|:----|
|The Data School: Learn Introductory SQL Concepts|An interactive tutorial with an approachable style. The tutorial has built-in SQL evaluation, so you don’t need to set up a separate database tool to try the exercises.|
|Select Star SQL|An interactive book that teaches SQL concepts using real-world datasets and problems. The book has built-in SQL evaluation, so you don’t need to set up a separate database tool to try the exercises.|
|SQL Murder Mystery|The SQL Murder Mystery is designed to be both a self-directed lesson to learn SQL concepts and commands and a fun game for experienced SQL users to solve an intriguing crime. They also have a walkthrough for SQL beginners.|
|CodeAcademy: Learn SQL course SQL Commands|A course called Learn SQL and a list of SQL Commands. Without a Pro account, course features are limited.|
|Linked In Learning|Linked In Learning provides access to several courses on SQL at many levels of expertise. Requires a paid subscription.|

### LDP-spezifische Abfrageanleitungen

Nachdem gelernt wurde, wie SQL verwendet wird, gibt es einige Ressourcen, die die Besonderheiten der Organisation von FOLIO-Daten durch LDP beschreiben.

* **[The LDP User Guide](https://github.com/library-data-platform/ldp/blob/1.8.2/doc/User_Guide.md).** Dieses Handbuch enthält Einzelheiten zum Schreiben von SQL, das für das LDP-Datenmodell funktioniert. Insbesondere die Abschnitte beachten, die das Datenmodell, JSON-Abfragen und die Unterschiede zwischen den relationalen Attributen und JSON-Feldern beschreiben. Der Leitfaden enthält auch einen Abschnitt, in dem die Funktion für historische Daten innerhalb der LDP beschrieben wird, mit der Personen Abfragen erstellen können, die untersuchen, wie sich FOLIO-Datensätze im Laufe der Zeit verändern.
* **[SchemaSpy](https://d1f3dtrg62pav.cloudfront.net/ldp/schema/public/index.html)**. Diese SchemaSpy-Installation ist mit der LDP-Referenzumgebung verbunden, die Daten aus der FOLIO-Snapshot-Referenzumgebung abruft. SchemaSpy liefert eine übersichtliche Liste der LDP-Tabellen und -Felder und kann bei der Entwicklung von Abfragen hilfreich sein, wenn die lokale LDP dieselbe Softwareversion wie die LDP-Referenzumgebung verwendet.
* **[FOLIO Schema Parser](https://docs.google.com/spreadsheets/d/1m_Cq_GmZX37gJPEjVWt9eOLXskUjSLUb-8KapWj0SIw/edit#gid=1511890017)**. Dieser leichtgewichtige FOLIO Schema Parser füllt automatisch eine Kalkulationstabelle aus, indem er die Datenschema-Dokumentation von FOLIO verwendet und FOLIO-Felder mit LDP-Tabellen und -Feldern verbindet. Er kann hilfreich sein, um schnell herauszufinden, welche Felder in FOLIO Apps verfügbar sind und welche LDP-Tabellen diese Felder enthalten.
* **[FOLIO Analytics shared derived tables](https://github.com/folio-org/folio-analytics/tree/release-1.5/sql/derived_tables).** Die für die LDP entwickelten abgeleiteten Tabellen (zu finden im **folio\_reporting** Schema der LDP) dienen oft als besserer Ausgangspunkt für Ad-hoc-Abfragen als die FOLIO Tabellen im **öffentlichen** Schema. Die abgeleiteten Tabellen kombinieren und vereinfachen die ursprünglichen FOLIO-Tabellen auf eine Weise, die die Entwicklung von Abfragen erheblich erleichtert. Es sollte mit dem lokalen LDP-Administrator zusammengearbeitet werden, um herauszufinden, wie die lokale LDP abgeleitete Tabellen verwendet (z.B. welche FOLIO Analytics-Version verwendet wird, wie häufig die abgeleiteten Tabellen aktualisiert werden).

### Gemeinsame Nutzung von Ad-hoc-Abfragen

Wenn eine Ad-hoc-Abfrage für andere Institutionen von Nutzen sein könnte, empfehlen wir, sie an das folio-analytics Repository zu senden. Unsere [Richtlinien für Beiträge](https://github.com/folio-org/folio-analytics/blob/release-1.5/CONTRIBUTING.md) beschreiben die Anforderungen für neue Beiträge zum Repository.

### Tipps für die Verwendung von DBeaver zum Schreiben einer Ad-hoc-Abfrage

Die Entwicklung von Ad-hoc-Abfragen mit DBeaver folgt einem ähnlichen Arbeitsablauf wie der obige Beispiel-Workflow. Es kann entweder mit einer bestehenden Berichtsabfrage oder einer abgeleiteten Tabellenabfrage begonnen und diese für die eigenen Zwecke modifiziert werden oder der SQL-Code wird von Grund auf neu geschrieben.

Ein Beispiel für eine einfache Ad-hoc-Abfrage ist:

```
SELECT
    group_name,
    COUNT(user_id) AS num_users
FROM
    folio_reporting.users_groups
GROUP BY
    group_name
;
```

Dieser Code gibt an, dass der Bericht zwei Spalten enthalten soll: **group\_name** und eine Spalte, die eine Berechnung der Anzahl der Werte in der Spalte **user\_id** speichert, die in der Abfrage mit der Bezeichnung "num\_users" erscheinen soll. Der Code gibt dann an, dass diese Spalten aus der abgeleiteten Tabelle **folio\_reporting.users\_groups** stammen. Schließlich gibt er an, dass die Daten aus der Originaltabelle mit Hilfe der Werte aus der Spalte **group\_name** in separate Gruppen aufgeteilt werden sollen, so dass die Berechnung von **num\_users** für jede Gruppe separat durchgeführt wird. Das Ergebnis ist eine Tabelle, in der jeder Wert von **group\_name** mit der Anzahl der Personen in dieser Gruppe abgeglichen wird.

Wenn ein Abfrage in DBeaver geschrieben wird, kann es hilfreich sein, die LDP mit Hilfe der Registerkarte [Datenbank-Navigator](https://dbeaver.com/docs/wiki/Database-Navigator/) zu durchsuchen. Es können zum Beispiel die Verbindung, dann die **Schemas**, dann das Schema **folio\_reporting** und schließlich die Tabellen erweitert werden, um die verfügbaren abgeleiteten Tabellen zu sehen. Jede Tabelle kann erweitert werden, um ihre verfügbaren Spalten zu sehen. Um die Daten in einer Tabelle zu durchsuchen, mit der rechten Maustaste auf eine Tabelle klicken und **Daten anzeigen** wählen. Auf die gleiche Weise vorgehen, um die im öffentlichen Schema verfügbaren Tabellen und Spalten zu durchsuchen.
