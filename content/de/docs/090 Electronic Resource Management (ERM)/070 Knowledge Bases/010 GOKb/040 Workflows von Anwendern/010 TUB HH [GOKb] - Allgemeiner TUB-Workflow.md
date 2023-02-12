---
title: "TUB HH [GOKb] - Allgemeiner TUB-Workflow"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [app-gokb, by-tubhh, cat-workflows, for-anwender, by-community_einzelbeitrag]
weight: 10
Description: "
    Quellen: [Originalquelle](https://intranet.b.tu-harburg.de/mediawiki/index.php?title=FOLIO/Module/ERM/Workflows/GOKb-Workflow) & [GBV](https://info.gbv.de/display/FOLIOGBVEXTERN/TUB+HH+[GOKb]+-+Allgemeiner+TUB-Workflow)
    "
---

{{% pageinfo %}}
Stand 2023-01
{{% /pageinfo %}}

## Vorab zu klären

### Konsortialpakete

Die Konsortialführenden Bibliotheken sind zu einem großen Teil noch nicht in der GOKb vertreten. Es gibt aber konkrete Planungen zusammen mit der EZB, dass Konsortialpakete aus der EZB heraus in die GOKb überspielt werden sollen, auch wollen weitere Konsortialführer sich an der Pflege der Pakete in der GOKb beteiligen.

Von der TIB und dem heBis haben wir die Rückmeldung bekommen, dass sie die Pflege der Paketdaten in der GOKb zurzeit nicht leisten können.

**Internes Vorgehen (Vorschlag):**

-   Zeitschriften-und eBook-Pakete aus Konsortien erfassen wir vorerst nicht (Vereinbarung in Folio wird mit Tag "nicht-in-GOKb" gekennzeichnet
-   Datenbanken -> sind leicht zu pflegen (keine KBART-Datei), können erfasst werden, kann man aber auch erstmal verschieben

### KBART-Dateien

-   Wir legen ein Paket erst in der GOKb an, wenn eine aktuelle KBART-Datei vorhanden ist.
-   Falls wir die KBART-Datei per Mail vom Anbieter erhalten, wird sie zunächst auf Laufwerk G:/Folio gespeichert
-   Von Vorteil wäre es, wenn die KBART-Datei per Direktlink über die Webseite des Anwenders abrufbar wäre, damit der automatisierte Upload gewählt werden kann
-   Prüfen ob das Feld title\_id in der KBART-Datei anbieterspezifisch ist, oder ob es sich um einen allgemeinen Identifikator, wie z.B. die DOI oder ISSN handelt
-   Die KBART-Datei sollte vorab grob geprüft werden, z.B.
    -   Entspricht der Dateiname dem KBART-Standard? Siehe auch [Einführung in KBART](https://gokb.org/de/documentation/kbart-introduction.html)
    -   sind sowohl die Spalte online\_identifier als auch print\_identifier vorhanden?
    -   ist die Spalte publication\_type vorhanden?
    -   Sind die Felder in der Spalte title\_id belegt?
-   Perspektive: statt der manuellen Prüfung kann zukünftig ggf. die [NISO KBART Validator App](https://niso.cadmoremedia.com/Title/370b7cc4-0753-41f8-a0a2-bc50db9a32cc) helfen (2022 noch in Entwicklung).

### In der GOKb wurde geprüft, ob das Paket vorhanden ist

#### Fall 1: Verwaistes Paket in GOKb

-   Das GOKb-Team anschreiben (gokb@hbz-nrw.de) und das Paket uns als Kurator zuweisen lassen (es sei denn es ist ein Konsortialpaket)
-   Nach Zuweisung die Angaben zum Paket überprüfen und ggf. ergänzen
-   KBART-Datei hochladen, wenn möglich den automatischen Upload verwenden

#### Fall 2: Paket in GOKb mit Kuratorengruppe aber nicht aktuell

-   Den entsprechenden Kurator anschreiben und mitteilen, dass wir das Paket nutzen wollen (E-Mail-Adressen der Kuratorengruppen werden in der GOKb noch nicht angezeigt); Hebis bitte nicht anschreiben, die Hebis-Pakete sind nicht aktuell und werden nicht mehr gepflegt
-   Klären ob der Kurator das Paket weiter pflegen will, (ggf. zeitliche Absprache treffen)
-   Neben der Aktualität ist auch der Listenstatus für uns wichtig (geprüft) da das Paket sonst nicht in Folio übernommen wird

#### Fall 3: Paket nicht in GOKb

-   Siehe nächster Punkt "Anbieter und Plattform"

### Anbieter und Plattform

-   Ist die Entscheidung gefallen, dass ein Paket in der GOKb erfasst werden soll, müssen zunächst der Anbieter und die Plattform geprüft werden

#### Fall 1: Anbieter mit diversen Dubletten vorhanden

-   Wenn zu dem Anbieter mehrere Dubletten vorhanden sind, muss entschieden werden, welche Anbieter ggf. gelöscht werden und welcher erhalten bleiben soll
-   Hängen viele Pakete an den Anbietern, oder es besteht Unsicherheit, soll dies in Absprache mit dem GOKB-Team erfolgen

> **Wer ist der korrekte Anbieter? Dazu folgende Infos aus der GOKb-Inforunde am 10.01.2022**
>
> -   Anbieter (für Pakete) ist in der Regel die Organisation, die die Plattform anbietet, auf der die Daten enthalten sind
> -   Ist dieser Anbieter bibliothekarisch unintuitiv (z.B. Springer Nature Switzerland AG), wird in Absprache mit der GOKb-Redaktion ein präferierter Anbietername gesetzt
> -   Nicht als Anbieter (für Pakete) zählen Verlage, die in der Spalte publisher\_name genannt sind (z.B. J.B. Metzler bei Springer)

#### Fall 2: Anbieter vorhanden, aber Plattform fehlt

-   Siehe Anlegen und Pflege von Anbietern
-   Bei Problemen beim Anlegen der Plattform, Rückfrage an [info@gokb.de](mailto:info@gokb.de)

#### Fall 3: Anbieter und Plattform nicht vorhanden

-   Siehe Anlegen und Pflege von Anbietern
-   Ergänzung zur Anleitung:
    -   Ist die title\_id in der KBART-Datei anbieterspezifisch, muss der Namensraum in der GOKb angelegt werden. Das kann nur das GOKb-Team machen.
    -   Sobald der Namensraum eingerichtet wurde, kann er auch beim Anbieter erfasst werden

> **Aus der GOKb-Infostunde vom 14.2. zum Thema Anbieter-Namensräume:**
>
> -   Wieso gibt es unterschiedliche Anbieter-Namensräume, also Identifikatorsysteme für Anbieter, und nicht nur einfach einen gemeinsamen "Anbieter-ID"?
> -   Unterschiedliche Anbieter-Namensräume existieren, damit es nicht zu falschen Matches über die title\_id kommt. Verschiedene Anbieter identifizieren ihre Titel intern unabhängig voneinander - einige mit Zahlen, einige mit Buchstaben, andere wieder mit Zahlen-Buchstaben-Kombinationen (siehe Beispiel). Hier ist es natürlich möglich, das zwei Anbieter intern z.B. die selbe Zahl für komplett unterschiedliche Titel benutzen. Damit hier in der GOKb keine falsche Übereinstimmung suggeriert wird, müssen sie in verschiedenen Namensräumen gefasst werden, z.B. "Cambridge University Press" und "Springer".

## Pakete anlegen und Pflegen

### Pakete anlegen mit automatischem KBART-Upload

-   Die GOKb-seitige Anleitung zum Anlegen und Pflegen von Paketen, die auch Pflichtfelder der KBART-Datei, sowie eine Anleitung zum automatischen Upload von KBART-Dateien enthält ist sehr ausführlich und muss hier nicht nochmal erfasst werden.
-   Der automatische KBART-Upload bietet sich z.B. an, wenn zu einem e-Book-Paket im Laufe des Jahres weitere Titel hinzukommen aber auch bei laufenden Zeitschriftenpaketen, bei denen neue Titel hinzukommen und Titel ausscheiden können.
-   Der Automatische Upload ist nur möglich, wenn ein Direktlink auf die Datei vorhanden ist
-   der automatische Upload funktioniert aktuell nicht so, wie in der Anleitung beschrieben: Dazu **eine Ergänzung zum automatischen Upload von KBART-Dateien aus der E-Mail von Daniel Rupp vom 1.2.2022:**

> Zurzeit muss der Paketinhalt erstmalig geladen werden, bevor das automatisierte Update mit Platzhaltern läuft. Wir werden das ändern, was aber ggf. etwas dauern dürfte. Als Workaround bietet sich an, die URL zum Paket zunächst einmal ohne Platzhalter anzulegen und den Job nach "Bestätigen" des Pakets einmal durchlaufen zu lassen, in der Folge dann die von Ihnen angegebene URL mit Platzhaltern einzugeben.

### Globale Pakete ohne automatischem KBART-Upload

-   Ist ein automatischer KBART-Upload nicht möglich und wir erwarten, dass, z.B. im Laufe des Jahres weitere E-Book-Titel hinzukommen, muss man sich ggf. einen Termin setzen für einen erneuten KBART-Upload
-   Bei laufenden Zeitschriften-Paketen wäre ein jährlicher KBART-Upload denkbar

### Lokale Pakete anlegen

-   Lokale Pakete müssen wir z.B. anlegen, für
    -   EBS-Festkäufe: KBART-Datei muss ggf. aus KBART-Datei des Gesamtpakets selbst erstellt werden, wenn der Anbieter diese nicht anbietet. Handelt es sich nur um wenige Festkäufe (bis zu 30 Titel), können diese auch direkt in Folio ausgewählt werden, ohne das ein Paket in der GOKb angelegt werden muss
    -   wenn wir nur einen Teil der Zeitschriften eines Paketes beziehen
    -   selbst zusammengestellte Pakete (Pick and choose)
    -   E-Book oder Zeitschriften Einzelkäufe, die zu einem lokalen Paket zusammengefasst, in Folio aufgenommen werden (haben wir noch nicht umgesetzt)
-   Der Zugang und Abgang von Titeln in lokalen Paketen ist über mehrere Wege möglich:
    -   Aktualisierung der KBART-Datei durch Belegen des access\_start\_date und/oder access\_end\_date
    -   Entfernen und Hinzufügen einzelner Titel direkt in der GOKb
    -   Setzen des Datums "Zugreifbar bis" in Folio

## Nach dem Anlegen des Pakets

1.  Auf dem Dashboard überprüfen ob der KBART-Upload erfolgreich war
2.  Nach erfolgreichem KBART-Upload die Anzahl der Titel im Paket überprüfen und Plausibilitätskontrolle durchführen (z.B. Passen die Titel zum Fachgebiet des Pakets?)
3.  Ggf. Prüfanfragen zum Paket und zu den Titeln im Paket bearbeiten
4.  Unter "Paketeigenschaften" den Listenstatus auf "geprüft" setzen, damit das Paket in Folio übernommen werden kann
5.  Gleichzeitig möglichst auch den Bearbeitungsstatus auf "bestätigt" setzen
