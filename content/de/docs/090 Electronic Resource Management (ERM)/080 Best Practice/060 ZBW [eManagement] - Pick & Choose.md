---
title: "ZBW [eManagement] - Pick & Choose"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [by-zbw, cat-bestpractices, for-anwender, by-community_einzelbeitrag, topic-fernleihe]
weight: 60
Description: "
    Quellen: [GBV](https://info.gbv.de/pages/viewpage.action?pageId=839909385)
    "
---

{{% pageinfo %}}
Version: Lotus

Berechtigung: role-erm-admin
{{% /pageinfo %}}

Pick & Choose ist eine Erwerbungsart für elektronische Medien (E-Journals und E-Books), bei der die gewünschten Titel _einzeln_ lizenziert werden (im Gegensatz zu Paketlizenzen).

![(Info)](https://info.gbv.de/s/-yuig8a/8803/369q8t/_/images/icons/emoticons/information.svg) Grundsätzlich muss jede Bibliothek prüfen, ob sich der **Aufwand für die Verwaltung von Einzellizenzen im FOLIO-ERM-Modul** lohnt, da durch den Erwerbungsworkflow (ACQ oder FOLIO) i.d.R. bereits viele Anforderungen abgedeckt werden: Metadaten kommen i.d.R. in den Katalog, indem ein Bestellexemplar in K10plus angelegt wird, Verlängerungen erfolgen im Rahmen der Verwaltung von Fortsetzungen im ACQ usw..

Wann das ERM-Modul für Einzellizenzen genutzt werden sollte:

* Nutzung des FOLIO-ERM-Lizenzmoduls: Verknüpfung von Lizenzinformationen mit Titeldaten (z.B. Infos zur elektronischen Fernleihe).
* FOLIO-ERM als Datenquelle für Zielsysteme (z.B. Discovery).

### Recherche und Datenimport: Einzeltitel in Paketen

Für Ressourcen, die im Modul **eManagement** verwaltet werden sollen, müssen Informationen zu Titel, Identifiern und Plattform in der lokalen Knowledgebase des **FOLIO-ERM-Moduls** vorhanden sein.  Alle Ressourcen sind Bestandteile von **Paketen** \- wenn es wirklich nur einen Titel auf einer Plattform gibt, dann muss dafür trotzdem ein Paket (mit  einem einzigen Titel) angelegt und in die lokale Knowledgebase übernommen werden.

Es wird davon ausgegangen, dass die **GOKb** als externe Datenquelle aktiviert ist. Dadurch stehen aktuell alle in **GOKb** vorhandenen Pakete und die enthaltenen Titel in den lokalen FOLIO-ERM-Instanzen zur Verfügung.

![](/img/de/_moved_from_wrong_pasting/060%20ZBW%20[eManagement]%20-%20Pick%20&%20Choose_2023-02-10-18-22-36.png)

1.   Recherche: Ist der Titel bereits in der lokalen FOLIO-ERM-Knowledgebase vorhanden?
    1.  Im Modul **eManagement** → _Search & Filter_ → Tab _E-Ressourcen_
    2.  Empfohlen: Filtern nach _Publikationstyp (engl. Type)_
        (![(Info)](https://info.gbv.de/s/-yuig8a/8803/369q8t/_/images/icons/emoticons/information.svg) Das Filtern nach _Typ: Journal_ ergibt für eine GOKb-basierte Knowledgebase fast identische Ergebnisse wie _Publikationstyp: Serial_)
    3.  Suche mit Identifier oder Titel: Diese Identifier werden für das Matching genutzt:
        P-ISSN, P-ISBN, DOI, ZDB-Id, DOI (daher bekommt man z.B. bei Suchen mit der E-ISSN keine Treffer, obwohl der Titel in der Knowledgebase vorhanden ist. Zur Sicherheit sollte mit dem Titel gesucht werden, wenn die Recherche mit Identifier ergebnislos ist.

![](/img/de/_moved_from_wrong_pasting/060%20ZBW%20[eManagement]%20-%20Pick%20&%20Choose_2023-02-10-18-23-00.png)

2.  Der Titel ist vorhanden:
    1.  Optionen für den Erwerb dieser E-Ressource: Eine geeignete Option für den Titel (Zeilen mit Bestandsangabe:  laufende Subskription =  offener Bestandsverlauf) auswählen und _Titel hinzufügen_ klicken;
        der Titel wird in den Warenkorb eingefügt. Jeder Titel erzeugt eine eigene _Vereinbarungskomponente_ und kann dadurch unabhängig von den anderen Titeln in der Vereinbarung verändert oder gelöscht werden.  Bei Nutzung des Erwerbungsmodul kann jede Komponente mit ihrer Bestellung verknüpft werden.
    2.  ![(Warnung)](https://info.gbv.de/s/-yuig8a/8803/369q8t/_/images/icons/emoticons/warning.svg) Wenn man 10 oder mehr Titel für eine Vereinbarung auswählt, ist das Verfahren über die Recherche der Einzeltitel erst einmal aufwändig. Ab einer  bestimmten Anzahl von Einzellizenzen kann es sich lohnen, in **GOKb** ein lokales bibliotheksspezifisches Paket anzulegen und dieses als Grundlage einer _Vereinbarung_ mit nur einer _Vereinbarungskomponente_ zu nutzen. Neue Käufe werden einfach dem lokalen Paket hinzugefügt. Bei Nutzung des Erwerbungsmodul kann nur das Paket mit einer oder mehrerer Bestellungen verknüpft werden.
3.  Der Titel ist nicht vorhanden:
    Der Titel muss in der GOKb angelegt werden (bitte auf GOKb-Seiten weiterlesen), damit er über die automatische Synchronisierung mit den FOLIO-Instanzen in die FOLIO-ERM-Knowledgebase importiert wird. Während Zeitschriften die Abdeckung durch die Anbindung der EZB vermutlich weitgehend komplett ist, können E-Books hier einen erhöhten Aufwand verursachen, da hier die Pakete wesentlich größer und dynamischer sind, d.h. man ist u.U. gezwungen, ein lokales Paket  für einen Titel anzulegen, der in GOKb  noch nicht vorhanden ist (oder für die GOKb-Community ein Paket mit zehntausenden Titeln).

Beispiel _ABI-Technik_: Die Suche mit der ISSN 0720-6763 ergibt keine Treffer,  ZDB-ID 2598795-1 und ISSN 2191-4664 funktionieren. Der Titel _Rundbrief Fotografie_  (ZDB-Id  3115029-9) war am 15.12.22 noch nicht in der FOLIO-ERM-Knowledgebase enthalten und muss in der GOKb angelegt werden, damit er nach der Synchronisierung in FOLIO-ERM genutzt werden kann.

![(Info)](https://info.gbv.de/s/-yuig8a/8803/369q8t/_/images/icons/emoticons/information.svg) Es ist auch möglich, KBART-Dateien direkt über das Modul Lokale KB-Verwaltung einzuspielen, da es aber vom Aufwand her keinen Unterschied zur Arbeit in der GOKb macht, wird dies für GOKb-Anwender im GBV nicht empfohlen.

![](https://info.gbv.de/download/attachments/839909385/image2022-12-14_18-5-43.png?version=1&modificationDate=1671037543347&api=v2)

![](https://info.gbv.de/download/attachments/839909385/image2022-12-14_18-49-53.png?version=1&modificationDate=1671040193537&api=v2)

### Verwaltung von Pick & Choose in Vereinbarungen:  Einzeltitel als neue Vereinbarungskomponente
![](/img/de/_moved_from_wrong_pasting/060%20ZBW%20[eManagement]%20-%20Pick%20&%20Choose_2023-02-10-18-23-42.png)

Mit dem Inhalt des Warenkorbs (i.d.R. nur ein  Titel) kann jetzt entweder eine neue _Vereinbarung_ erstellt werden, oder der Titel wird als neue _Vereinbarungskomponente_ an eine vorhandene Vereinbarung gehängt.
![(Info)](https://info.gbv.de/s/-yuig8a/8803/369q8t/_/images/icons/emoticons/information.svg) Vorteil ist, dass in der Vereinbarungskomponente über die Aktion _Bestellposten hinzufügen_ eine Verknüpfung  mit der Bestellung im Modul FOLIO-Bestellungen möglich ist.

Alternativen:

*  ![(Haken)](https://info.gbv.de/s/-yuig8a/8803/369q8t/_/images/icons/emoticons/check.svg) für jeden Titel eine eigene Vereinbarung zu erzeugen = jedesmal, wenn ein neuer Titel dazukommt, wird eine eigene Vereinbarung mit genau einer Vereinbarungskomponente erzeugt.
    Vorteil: Verlängerungen können über die Felder _Vereinbarungszeiträume →Enddatum_ und _→ Stornierungsfrist_ gesteuert werden, z.B. über das **Dashboard-Modul**;
    Beispiel: Für _ABI-Technik und Rundbrief Fotografie_ wird jeweils eine eigene Vereinbarung erstellt
    Nachteil: Die Anzahl der Vereinbarungen wird aufgebläht;

*   ![(Haken)](https://info.gbv.de/s/-yuig8a/8803/369q8t/_/images/icons/emoticons/check.svg) ![(Haken)](https://info.gbv.de/s/-yuig8a/8803/369q8t/_/images/icons/emoticons/check.svg) Titel mit gemeinsamen Eigenschaften (z.B. alle de Gruyter-Einzellizenzen) jeweils in Vereinbarungen zu clustern = jedesmal, wenn ein neuer Titel dazukommt, wird die zugehörige Vereinbarung um eine neue Vereinbarungskomponente erweitert.
    Nachteil: Keine Verwaltung der Vereinbarungszeiträume je Titel ; _Vereinbarungszeiträume → Startdatum_ ist Pflichtfeld und muss daher belegt werden (z.B. Tagesdatum); für alle Titel gelten die selben Bedingungen aus dem ERM-Lizenzmodul.
    Beispiel: _ABI-Technik und Rundbrief Fotografie_ werden als jeweils eigene Vereinbarungskomponenten in einer gemeinsamen Vereinbarung (für de Gruyter-Einzelsubskriptionen) verwaltet.
    Andere Möglichkeiten der inhaltlichen Gruppierung:  Proquest-E-Book-Einzelkäufe mit 1-Nutzer-Lizenz, die 2022 erworben wurden ![](/img/de/_moved_from_wrong_pasting/060%20ZBW%20[eManagement]%20-%20Pick%20&%20Choose_2023-02-10-18-24-05.png)
*  ![(Fehler)](https://info.gbv.de/s/-yuig8a/8803/369q8t/_/images/icons/emoticons/error.svg) beliebige Titel in einer Sammel-Vereinbarung zu verwalten = jedesmal, wenn ein neuer Titel dazukommt, wird die SammelVereinbarung um eine neue Vereinbarungskomponente erweitert = möglich, aber wenig sinnvoll
    Nachteil: Der  heterogenen Titelgruppe kann keine gemeinsame Lizenz aus dem **ERM-Lizenzen-Modul** zugewiesen werden.
* Beispiel: _ABI-Technik und Rundbrief Fotografie_ werden als neue Vereinbarungskomponenten einer bestehenden Vereinbarung zugewiesen, die bereits Einzelabos von Elsevier, OUP und weiteren Verlagen enthält. ![](/img/de/_moved_from_wrong_pasting/060%20ZBW%20[eManagement]%20-%20Pick%20&%20Choose_2023-02-10-18-24-21.png)
**Einzellizenzen eines Anbieters in einer Vereinbarung: eine Vereinbarungskomponente je Titel**

Belegung der Felder:

|Name|beliebig; empfohlen wird Konvention wie z.B. Verlagsname -Medientype -Erwerbungsart - (Jahr) z.B.  De Gruyter Journals Pick & choose|
|:----|:----|
|Beschreibung|optional, empfohlen: Beschreibung der gemeinsamen Eigenschaften, z.B. Einzelabos Print & Online bei de Gruyter|
|Status Dauerhafter Zugriff|aktiv laufende Zeitschriftenabos = leer, E-Books = yes  |
|Vereinbarungszeiträume Startdatum    Enddatum   Stornierungsfrist|(= Angaben zum Subskriptionsverlauf) Startdatum des Lizenzzeitraums (bei E-Books i.d.R. aktuelles Tagesdatum bzw. Tag der Freischaltung)  Beispiel: Startdatum = 1.1.2023 → der Titel wird bei einem Export (z.B. für den Recherchekatalog) am 1.12.22 nicht berücksichtigt, in der Exportdatei am 2.1.23 ist er dagegen enthalten.  bleibt leer; Kauf E-Books haben kein Enddatum,  für E-Journals  kann zwar bei der üblichen jährlichen Verlängerung eine Vereinbarungskomponente für jedes Lizenzjahr angelegt werden, bei mehreren Vereinbarungskomponenten in einer Vereinbarung wird das aber schnell unübersichtlich. optional (wenn die Verwaltung der Verlängerungen nicht im Erwerbungsmodul erfolgt (z.B. bei ACQ)|
|Vereinbarungskomponente  Aktiv ab / bis|(= Angaben zur Verfügbarkeit der Inhalte) Datum, ab dem/bis wann die Lizenz gültig ist/Datum der Freischaltung   Lizenzen können sofort bei Vertragsabschluss im FOLIO-ERM-Modul angelegt werden.  Das Datum wird beim Export der Vereinbarung mitgeliefert und kann z.B. für die Anzeige in Katalogen ausgewertet werden.|
|Benutzerdefinierte Abdeckung|nur E-Journals: Vom Erscheinungsverlauf der eingespielten Daten abweichende freigeschaltete Jahrgänge|

Alle weiteren Schritte entsprechen dem Anlegen von Vereinbarungen für Pakete.

![(Warnung)](https://info.gbv.de/s/-yuig8a/8803/369q8t/_/images/icons/emoticons/warning.svg) Ergänzende Dokumente, die spezifische für Einzeltitel sind (soweit vorhanden)  lassen sich leider nur der Vereinbarung, nicht den einzelnen Vereinbarungskomponenten zuordnen.

![](https://info.gbv.de/download/attachments/839909385/image2022-12-14_19-0-3.png?version=1&modificationDate=1671040803569&api=v2)

![](https://info.gbv.de/download/attachments/839909385/image2022-12-14_18-58-58.png?version=1&modificationDate=1671040738569&api=v2)

![](https://info.gbv.de/download/attachments/839909385/image2022-12-14_18-57-12.png?version=1&modificationDate=1671040632709&api=v2)

#### Titel entfernen
![](/img/de/_moved_from_wrong_pasting/060%20ZBW%20[eManagement]%20-%20Pick%20&%20Choose_2023-02-10-18-24-37.png)

Wenn das subskribierte E-Journal abbestellt wird oder in Open Access transformiert wird, reicht es,  im Akkordeon _Vereinbarungskomponente_ das Enddatum _Aktiv bis_ zu setzen.  Die Ressource taucht nach diesem Datum im Filter _Unter diese Vereinbarung fallende E-Ressourcen_ der Liste der in der Vereinbarung enthaltenen Ressourcen als _Weggefallen_ auf und wird nicht mehr exportiert. Auch wenn der Titel in einer anderen Vereinbarung (z.B. als Open Access) weitergeführt wird, kann er zur Dokumentation der Bestellgeschichte als inaktive _Vereinbarungskomponente_ bestehen bleiben.

![](https://info.gbv.de/download/thumbnails/839909385/image2022-12-15_18-5-41.png?version=1&modificationDate=1671123941978&api=v2)

