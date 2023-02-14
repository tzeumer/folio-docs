---
title: "TUB HH [Lizenzverträge] - Ersterfassung"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [app-lizenzverträge, by-tubhh, cat-workflows, for-anwender, by-community_einzelbeitrag, topic-fernleihe, app-e_management]
weight: 100
Description: "
    Quellen: [Originalquelle](https://intranet.b.tu-harburg.de/mediawiki/index.php/FOLIO/Module/ERM/Workflows/Lizenzvertr%C3%A4ge) & [GBV](https://info.gbv.de/pages/viewpage.action?pageId=718307483)
    "
---

{{% pageinfo %}}
Stand 2023-01
{{% /pageinfo %}}

## Erstes Eingabefenster/Kopfbereich

### Pflichtfelder

* Die Felder Name, Typ und Status sind Pflichtfelder. Start- und Enddatum, sowie das Beschreibungsfeld sind optional.

### Name

* Bei der Schreibweise des Namens müssen doppelte Leerzeichen vermieden werden, da sonst die alphabetische Sortierung verändert wird.
* Bei der Vergabe des Namens sind die Angaben im Vertrag zu beachten
* Bei verschiedenen Verträgen eines Verlages, ist darauf zu achten, die Lizenzverträge so zu benennen, dass sie voneinander zu unterscheiden sind. Beispiele:
    * Springer Verträge:
        * Springer eBook Collections
        * Springer Access and Select - Basic
        * Springer Nature Publish and Read
        * Springer Publish and Read
    * ACM:
        * ACM Books Collection I
        * ACM Digital Library
* Gibt es unterschiedliche Beschreibungen für den Vertrag, kann ein weiterer Name als "Alternativer Name" hinzugefügt werden
* Der Lizenzzeitraum (oder wenn Ende nicht bekannt, das Start-Jahr) wird zusätzlich zum Start- und Enddatum im Titel angegeben

### Start- und Enddatum

* Es werden Start- und Enddatum des Lizenzvertrages erfasst, unabhängig davon für welchen Zeitraum eine Vereinbarung getroffen wurde. Läuft ein **Konsortialvertrag** beispielsweise von 2019-2021, wir sind aber erst 2020 beigetreten, wird dennoch der 1.1.2019 als Startdatum und der 31.12.2021 als Enddatum eingegeben.
* Ist das Enddatum des Vertrages nicht definiert, muss ein Häkchen bei "Offenes Ende" gesetzt werden, damit man die eingegebenen Daten abschicken kann.
* Enthält ein Vertrag ein Enddatum, ist aber über dieses Datum hinaus für Medien mit dauerhaftem Zugriff gültig, wird es dennoch erfasst (Vertrag bleibt aber weiter "aktiv".

### Status

Der Status muss manuell verändert werden, z.B. sobald:

* ein noch nicht aktiver Vertrag, aktiv wird
* ein aktiver Vertrag abgelaufen ist, es sei denn der Vertrag ist weiterhin für den dauerhaften Zugriff gültig - dann bleibt auch der Status "aktiv" dauerhaft erhalten
* eine Vertragsverhandlung abgeschlossen ist

### Beschreibung

* Das Feld muss nicht ausgefüllt werden, kann aber genutzt werden um Informationen (z.B. aus dem Wiki) zu erfassen, die an keiner anderen Stelle abgebildet werden können.
* Bei mehreren Verträgen eines Verlages, die schwer voneinander zu unterscheiden sind, kann der Vertrag hier näher definiert werden.
* Angaben zum Konsortialvertrag sind an anderen Stellen erfasst, können hier aber zusammengefasst abgebildet werden. (Kein Muss)

## Interne Kontakte

* Die internen Kontakte werden genutzt um das zuständige Fachreferat zu erfassen
* Die Fachreferenten werden vorerst nicht namentlich erfasst.
* Unter "Interne Kontakte" ist aus Fachreferat 2-6 auszuwählen. (Diese sind in der Personen-App bereits erfasst)
* Die Fachreferate werden in beiden Apps erfasst (eManagement und Lizenzverträge)
* Ist ein Lizenzvertrag für diverse Pakete gültig und es sind alle Fachreferate daran beteiligt, müssen diese im Lizenzvertrag nicht erfasst werden.
* Abgesehen von den Fachreferaten erfassen wir keine internen Kontakte

## Organisationen

* In der Lizenzverträge-App verknüpfen wir die Organisationen, die direkt mit dem Lizenzvertrag im Zusammenhang stehen, also in erster Linie Lizenzgeber und Lizenznehmer. Weitere Organisationen werden in der eManagement-App erfasst (z.B. Rechnungssteller).
* **Wir nutzen nur die Rollen Lizenzgebende Organisation und Konsortialführung** (Die Werte "Konsortium" und "Lizenznehmende Organisation" gehören zu den Referenzwerten, die sich nicht löschen lassen).
* Bei einem "Konsortialvertrag" vergeben wir "Konsortialführung" für die konsortialführende Bibliothek und "Lizenzgebende Organisation" für den Vertragspartner
* Bei vorliegenden Unterlagen, wie z.B. Angeboten, Zusagen, Lizenzverträgen gleichen wir die dort angegebenen Kontaktdaten mit denen in Folio (wenn schon angelegt) ab und ergänzen oder korrigieren diese
* Ergänzende Informationen siehe Workflow "Pflege der Organisationen"

## Hauptdokumente

* Unter "Hauptdokumente" laden wir den Lizenzvertrag und ggf. Ergänzungen zum Lizenzvertrag hoch
* Die Dokumente werden gleichzeitig auf Laufwerk J gespeichert
* Die Felder "Physischer Standort" und "URL" belegen wir. Hier wird der Pfad zum Dokument hinterlegt.

## Bedingungen

### Primärbedingungen/Optionalbedingungen

* Die Primärbedingungen wurden so ausgewählt, dass diese grundsätzlich ausgefüllt werden können und sollen.
* Alle benötigten optionalen Bedingungen (wenn diese im Vertrag enthalten sind) werden zusätzlich aus der Auswahlliste ausgewählt.

### Sichtbarkeit

* Vorerst ist bei allen Lizenzbedingungen die Sichtbarkeit auf "intern" voreingestellt und wird bei der Erfassung auch nicht geändert. Definition:
    * intern: Die Bedingung wird nur intern in Folio angezeigt
    * öffentlich (nutzen wir noch nicht): Die Bedingung wird in einem, an Folio angebundenen System angezeigt

### Interne Notiz

* Im Feld "Interne Notiz" erfassen wir ggf. ergänzende Informationen die im "Wert" nicht abgebildet werden können.

### Paragraphen aus dem Lizenzvertrag

* in das Feld "Interne Notiz" geben wir nach einem Semikolon den entsprechenden Paragraphen aus dem Vertrag ein. Dieser wird voraussichtlich später in ein neues Feld "Paragraph" übernommen.

### Öffentliche Notiz

* Dieses Feld nutzen wir aktuell nicht
* Sobald Lizenzbedingungen auch in einem externen System angezeigt werde (K10Plus, Discovery-System), kann dieses Feld genutzt werden, um ergänzende Informationen zum Bedingungs-Wert zu erfassen.

### Bedarf für zusätzliche Bedingungen

* Wird eine im Vertrag genannte Bedingung nicht in Folio abgebildet, die uns aber wichtig erscheint, vermerken wir diese zunächst im Gitlab-Board. Ggf.ergänzen wir diese dann in den Einstellungen als zusätzliche Bedingung.

### Lizenzbedingungen zum Zweitveröffentlichungsrecht

* Vorerst setzen wir das Tag "Zweitveröffentlichungsrecht" wenn der Vertrag Angaben zum Zweitveröffentlichungsrecht erhält und erfassen noch keine Bedingungen hierzu.

### Lizenzbedingungen zur Fernleihe

* die Primärbedingung zur Fernleihe muss ausgefüllt werden
* die optionalen Bedingungen zur Fernleihe werden nur erfasst, wenn die entsprechenden Angaben aus dem Vertrag hervorgehen (nicht aus einer anderen Quelle)

[Lizenzen (Fernleih-Bedingungen)](https://intranet.b.tu-harburg.de/folio/folio-api-queries/rest-php/index.php?tub_query=get_licenses) zum schnellen Abgleich vorhandener und fehlender Fernleihangaben. Via Link in der Rechten Spalte lässt sich prüfen, was andere Pilotbibliotheken im KXP für ein Sigel an FL-Rechten für ein Paketsigel gesetzt haben.

## Ergänzende Dokumente

Wie die Hauptdokumente, werden auch die ergänzenden Dokumente sowohl in Folio als auch auf Laufwerk J gespeichert und der Pfad wird hinterlegt.

**Mögliche Dokumente:**

* Konsortiale Autorisierungserklärung
* Produktdatenblatt
* Zusätzliche Informationen

## Sonstiges

### Abgelaufene Lizenzverträge eines zu einer aktuellen Vereinbarung

* Bei der Ersterfassung, wird der aktuelle Vertrag vollständig erfasst und mit dem Status "wirkend" in der Vereinbarung verknüpft.
* Die vorherigen Verträge werden ebenfalls erfasst, aber ohne Bedingungen. Sie werden mit dem Status "abgelaufen" in der eManagement-App verknüpft
* In der Beschreibung im Kopf wird Folgendes vermerkt: Ersterfassung ohne Bedingungen, da Vertrag abgelaufen

## Speichern von Verträgen

* Wir speichern die Lizenzverträge sowohl in der Lizenzverträge-App in Folio, als auch auf Laufwerk J
* Der Original-Vertrag (ohne Unterschrift) wird durchsuchbar gemacht und erhält den Zusatz "durchsuchbar" im Namen (auch bei Namensvergabe in Folio beachten)
* Der unterschriebene Vertrag muss nicht durchsuchbar sein und erhält den Zusatz "TU Unterschrift" nach dem er von der tub unterschrieben wurde. Sind alle Unterschriften auf dem Vertrag, erhält er den Zusatz "mit Unterschriften" und der Vertrag mit den tub-Unterschriften wird gelöscht.
**Fall 1: Vertrag ist nicht durchsuchbar**

* Der Vertrag wird an Mr. X weitergeben, um ihn mit Adobe Premium durchsuchbar zu machen
**Fall 2: Vertrag ist schreibgeschützt**

* PDF24 öffnen
* Auf "PDF Passwortschutz entfernen" klicken
* Datei auswählen
* Auf "Passwort entfernen" klicken
* Datei unter neuem Namen abspeichern
* Überprüfen ob durchsuchen und kopieren möglich ist
**Fall 3: Vertrag lässt sich nicht bearbeiten und ist mit DocuSign unterschrieben**

* Libre Office öffnen
* Vom Vertragspartner per DocuSign erstellte Signatur markieren und mit 'Entfernen' löschen
* Nicht Speicheroption wählen, sondern im Datei-Menü den Punkt 'Exportieren als (pdf)' wählen und an beliebigen Ort zwischenspeichern
* Dokument kann nun mit Adobe Premier durchsuchbar gemacht und im entsprechenden Verzeichnis auf Laufwerk J mit dem Namenszusatz "durchsuchbar" gespeichert werden

## Jährliche Lizenzverträge

## Jährliche Lizenzverträge zu Jahres-Paketen (Beispiel Springer)

### Lizenzverträge-App

Erhalten wir zu Jahrespaketen auch jährlich einen neuen Lizenzvertrag, können die Verträge in Folio zu einem einzigen Vertrag zusammengefasst werden, insofern es keine gravierenden Änderungen gibt. Der neue Lizenzvertrag wird mit dem im Vorjahr (bzw. in den Vorjahren) erfassten Lizenzbedingungen in Folio abgeglichen:

**Fall 1: Keine Änderungen gegenüber dem Vorjahr**:

* Der Name des Vertrags wird um das aktuelle Jahr erweitert
* Der aktuelle Vertrag wird im Akkordeon Hauptdokumente mit Angabe des aktuellen Jahres gespeichert
* In der Beschreibung wird erfasst: "Die Lizenzbedingungen der Verträge von .... bis .... stimmen überein" (oder so ähnlich)
**Fall 2: Geringfügige Änderungen gegenüber dem Vorjahr** (z.B. Änderung von Formulierungen, Verschiebung der Paragraphen-Nummern):

* Der Name des Vertrags wird um das aktuelle Jahr erweitert
* Es wird eine Vertragsänderung angelegt
* In der Vertragsänderung werden alle Bedingungen erfasst (inkl. Vertragstext), die Änderungen gegenüber dem Vorjahr aufweisen.
* Die Vertragsänderung erhält als Startdatum das Startdatum der Vertragslaufzeit. Das Enddatum bleibt offen.
* Der neue Vertrag wird in der Vertragsänderung gespeichert.
* Hinweis in der Beschreibung erfassen: "Vertrag von .... enthält geringfügige Änderungen, siehe Vertragsänderung"
**Fall 3: Änderungen gegenüber dem Vorjahr mit Auswirkungen** (z.B. etwas ist jetzt erlaubt, was vorher nicht erlaubt war, oder der Vertrag enthält eine neue Bedingung, die wir ebenfalls in Folio erfassen):

* Der Vertrag aus den Vorjahren wird dupliziert und ein neuer Vertrag angelegt und entsprechend angepasst.
* Der Vertrag des Vorjahres wird auf "abgelaufen" gesetzt

### eManagement-App

**Fall 1: Verträge wurden in einem Lizenzvertrag in Folio zusammengefasst**:

* Alle Jahrespakete deren Lizenzverträge in Folio zu einem zusammengefasst wurden, können gesammelt in einer Vereinbarung mit mehreren Vereinbarungskomponenten erfasst werden, da der "Folio-Lizenzvertrag für alle Pakete "wirkend" ist.
**Fall 2: Verträge wurden in einem Lizenzvertrag in Folio zusammengefasst und enthalten eine Vertragsänderung**:

* Die "geringfügigen" Änderungen in der Vertragsänderung beziehen sich auf alle in der Vereinbarung enthaltenen Pakete (nicht auf die Pakete ab einem bestimmten Jahr
* Da die Änderungen nicht gravierend sind, können weitere Pakete zur Vereinbarung hinzugefügt werden
**Fall 3: Es wurde ein neuer Lizenzvertrag mit "gravierenden" Änderungen erstellt**:

* Ab dem Jahr, für das ein neuer Lizenzvertrag erfasst wurde, müssen die Jahrespakete ebenfalls in einer neuen Vereinbarung erfasst werden. Dafür kann die Vereinbarung aus den Vorjahren dupliziert und angepasst werden.

## Jährliche Lizenzverträge zu einem laufenden Paket/einer laufenden Vereinbarung

* Gibt es z.B. zu einem laufenden Zeitschriften-Paket jährlich oder zumindest regelmäßig einen neuen Lizenzvertrag, kann dieser auch jährlich in Folio als neuer Vertrag erfasst werden, da an der Vereinbarung nur eine Vereinbarungskomponente hängt, für die entsprechend nur ein wirkender Lizenzvertrag vorhanden ist
* es bietet sich an, den Lizenzvertrag zu duplizieren, die im Vorjahr erfassten Lizenzbedingungen mit dem neuen Vertrag abzugleichen und den Vertrag entsprechend anzupassen.

[Checkliste für Paketverlängerung](https://collaborating.tuhh.de/tub/dd/applications/folio/workflow-erm-paketaufnahme/-/blob/master/.gitlab/issue_templates/Pakete_Verl%C3%A4ngerung_Folio.md) als Template im GitLab
