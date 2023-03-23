---
title: "Info: DE-Version"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: []
weight: 10
Description: "
    Quellen: Keine <!-- [Folio](https://docs.folio.org/docs/) & [GBV](https://info.gebev.de/display/FOLIOGBVEXTERN/GBV+FOLIO+Dokumentation) -->
    "
---

## Deutsch
### Stand der Übersetzung
2023-03-04. Die Vollständigkeit ist in der Konkordanzseite zu sehen (siehe [Handbuchseiten-Konkordanz der übersetzen Dokumentation]({{< ref "Handbuchseiten-Konkordanz der uebersetzen Dokumentation" >}}))

### Hintergrund
* Diese Übersetzung der offiziellen FOLIO-Dokumentation ist eine laienhaft und inoffizielle Freizeitübersetzung von [tzeumer@verweisunsgform.de](mailto:tzeumer@verweisunsgform.de)
* Übersetzt wurde mit DeepL zwischen 2022-12 und 2023-01 (siehe [Englisch-Deutsch (DeepL)-Glossar]({{< ref "Englisch-Deutsch (DeepL)" >}})). Persönliche Ansprachen ("Sie") wurden neutral umformuliert.
* Live gegengeprüft wurde jeweils via https://folio-snapshot.dev.folio.org
* Sie wurde zuerst ins [GBV-Confluence](https://info.gbv.de/display/FOLIOGBVEXTERN/GBV+FOLIO+Dokumentation) eingetragen und ist dann 2023-02 als Fork der Hugo-Version der offiziellen Dokumentation hierhin umgezogen. Tools (https://www.pastetomarkdown.com/ & https://markdown-convert.com/en/tool/table & https://tableconvert.com/excel-to-markdown)
* Siehe auch [siehe FOLIO-Wiki zum Thema Dokumentation und Konventionen](https://wiki.folio.org/display/SS/FOLIO+Documentation)

### Änderungen zur offiziellen FOLIO-Dokumentation
* Config-Dateien aus der Original-Version, die angepasst oder gelöscht/deaktiviert wurden, liegen mit der  Dateierweiterung ".folio-official" nochmal in diesem Branch
* Die deutsche Version setzt stärker auf Unterseiten ("Workflows"-Abschnitt unter jeder App), statt sehr langen Seiten zu einzelnen Apps. 
* In der englischen Dokumentation sind die Einstellungen aller Apps unter "Einstellungen" zu finden. Die deutsche Version hat diese Inhalt direkt unter die jeweilige App sortiert und nur Inhalte ohne eindeutige App-Zuordnung unter "Einstellungen" behalten
* Apps haben ggf. noch "Best Practice" und "Worfklows von Anwendern" als Unterabschnitte (siehe Abschnitt Struktur weiter unten)
* Jede Seite linkt zur englischen Originalquelle ("Quellen: Folio" am Seitenanfang)
* Letzte/Nächste Seite über TOC verlinkt (sofern vorhanden)
* Es wurden Tags vergeben

Im ersten Schritt (und wahrscheinlich zugleich letzten) ging es nicht um Perfektion, d.h. es wurde nur wenig Zeit auf grammatikalisch "schönere" Sätze gelegt. Zum Teil klingt es etwas steif, da die englische Version sowohl in Folio selbst als auch in der Dokumentation aktive Anrede verwendet, währen die die [Folio-Fachgruppe D-Übersetzung](https://wiki.folio.org/pages/viewpage.action?pageId=33947726) sich auf passive Formulierungen festgelegt hat ("Wenn Sie einen weiteren Typ anlegen wollen, dann klicken Sie auf den Button" wird "Soll einer neuer Typ angelegt wird, dann auf den Button klicken"). Gendern ist weitgehend schon durch die Übersetzungen der AG Übersetzung abgedeckt, An wenigen Stellen kann das aber noch unzureichend übersetzt sein.

### Lizenz und Version
Diese Übersetzung ist ein [Fork des FOLIO-Doc-Repositorys](https://github.com/folio-org/docs). Dort zu entnehmen: "This software is distributed under the terms of the Apache License, Version 2.0. See the file '[LICENSE](https://github.com/folio-org/docs/blob/main/LICENSE)' for more information.". 

Der Copyright-Hinweis im Footer der offiziellen Dokumentation wurde am 2023-02-20 mit dem Commit [Use CC-By 4.0 license and FOLIO project](https://github.com/folio-org/docs/commit/f51249ae7d0626ff2a3cdf201cdeb3407721a2ed) geändert.

### Quellen
Bedeutsame Quellen sind
* [Offizielle FOLIO-Dokumentation](https://docs.folio.org/)
* [Folio-Wiki: Information and User Guides for FOLIO Apps](https://wiki.folio.org/display/FOLIOtips/Information+and+User+Guides+for+FOLIO+Apps)
* [Beiträge der Anwenderbibliotheken in diesem Wiki](https://info.gbv.de/display/FOLIOGBVEXTERN/by-Community)
* [FOLIO- Project: DACH-Fachgruppen](https://wiki.folio.org/display/Deutsche/D-A-CH+-Fachgruppen?src=contextnavpagetreemode) (insbesondere Ausleihe, Erwerbung, Metadaten Management und Übersetzung)

### Struktur
Die Struktur der Dokumentation orientiert sich an der Struktur der offiziellen Doku (siehe auch [FOLIO Wiki: About Documentation> Content standards](https://wiki.folio.org/display/SS/FOLIO+Documentation)). Sie hat also Einleitung, Anhang und Hauptblöcke zu den großen Themen-/Aufgabenbereichen in Bibliotheken, wie Bestandszugang (Leihverkehr), Bestandmanagement (Erwerbung), Metadatenmanagement (Katalogisierung) und Electronic Resource Management (ERM). Die einzelnen FOLIO-Apps sind darunter zusammengefasst und beschrieben.

An vielen Stelle des Handbuchs, insbesondere unter den App-Seiten, gibt es eine Unterseite "Best Practises" und/oder "Workflows" und "Workflows von Anwendern". Diese Seiten haben jeweils Unterseiten. Bei "Workflows von Anwendern" nach dem Schema "Einstellende Einrichtung: App/Thema + Aktion" (Beispiel: "TUB HH: Lizenzverträge Ersterfassung"). Die Workflows aus dem Original-Foliohandbuch sind alle unter " Workflows" mit der Reihenfolge der Originaldokumentation.

Zusätzlich werden den Seiten (ehemals Confluence-)Labels vergeben, womit sich dann Übersichten und Filterungen generieren lassen, die auch unabhängig von der (primären) hierarchischen Dokumentationsstruktur. Siehe dazu insbesondere die Übersichtslisten aus Tags im [Index](https://info.gbv.de/display/FOLIOGBVEXTERN/Index). Dort ist jeweils auch die Verwendung eines einzelnen Tags nochmal näher erläutert.

Beispiel folgen hier drunter, solange es nur Vorschlagscharakter hat und es noch keine Extraseite gibt. Die Labels könnten ggf. noch spezifischer gewählt werden, lassen sich aber später auch noch (relativ) leicht anpassen. Es gibt folgende Labelkategorien, die bei den meisten Beitrag (fast) alle vergeben werden sollten

* [by-](https://info.gbv.de/pages/viewpage.action?pageId=849379549)
    * Vom wem stammt der Beitrag. Zum Beispiel [by-ag\_folio](https://info.gbv.de/display/FOLIOGBVEXTERN/by-AG+Folio), [by-folio](https://info.gbv.de/display/FOLIOGBVEXTERN/by-Folio), [by-tubhh](https://info.gbv.de/display/FOLIOGBVEXTERN/by-TUB+Hamburg), [by-vzg](https://info.gbv.de/display/FOLIOGBVEXTERN/by-VZG), [by-zbw](https://info.gbv.de/display/FOLIOGBVEXTERN/by-ZBW)
    * Besonders: by-community\_x für gemeinschaftlich gepflegte/ergänzte Dokumente. Um diese einfach für Übersichten filtern zu können, aufgeteilt in zwei Tags:
        * [by-community\_einzelbeitrag](https://info.gbv.de/display/FOLIOGBVEXTERN/by-Community_Einzelbeitrag): immer zusammen mit by-NAME\_DER\_EINRICHTUNG wie die Beispiele im ersten Spiegelstrich
        * [by-community\_gemeinsam](https://info.gbv.de/display/FOLIOGBVEXTERN/by-Community_Gemeinsam): Dokumente, die wirklich von vielen Einrichtungen direkt ergänzt werden (ein gutes Beispiel sind die [Lizenbedingungen für Lizenverträge](https://info.gbv.de/pages/viewpage.action?pageId=661979189)).
* [for-](https://info.gbv.de/pages/viewpage.action?pageId=849379622)
    * Für welche Zielgruppe ist der Beitrag? Derzeit [for-anwender](https://info.gbv.de/display/FOLIOGBVEXTERN/for-Anwender) für z.B. Workflows in den Apps selbst und [for-admin](https://info.gbv.de/display/FOLIOGBVEXTERN/for-Admin) für Workflows bei den App-Einstellungen.
    * In Testphase: [for-entwickler](https://info.gbv.de/display/FOLIOGBVEXTERN/for-Entwickler) (sinngemäß auch für SIGs).
* [cat-](https://info.gbv.de/pages/viewpage.action?pageId=849379568)
    * Typ des Beitrag. Zum Beispiel [cat-bestpractises](https://info.gbv.de/display/FOLIOGBVEXTERN/cat-Best+Practises) (von Anwendern), [cat-workflows](https://info.gbv.de/display/FOLIOGBVEXTERN/cat-Workflows) (von Folio und von Anwendern), [cat-einstellungen](https://info.gbv.de/display/FOLIOGBVEXTERN/cat-Einstellungen) (von Folio), sowie [cat-berechtigungen](https://info.gbv.de/display/FOLIOGBVEXTERN/cat-Berechtigungen) (meist zugleich Beschreibung der app selbst)
    * cat- meint eher starre, wiederkehrende Strukturelement der Dokumentation. Topic- (siehe unten) hingegen können mehr und freier gewählt werden
* [app-](https://info.gbv.de/pages/viewpage.action?pageId=849379634)
    * Name der beteiligten Folio-App(s). Zum Beispiel app-personen, app-organisationen
    * Sonderfall "app-einstellungen". Da Einstellungen zu spezifischen Apps werden mit app-NAME und cat-einstellung gettagt. Globale Einstellungen werden mit app-einstellungen getaggt. Das ist nicht unbedingt logisch oder am sinnvollsten, aber Konvention für den Moment. Um weiterhin Filterungen zu erlauben, gibt es zusätzlich auch cat-eisntellungen.
    * In Testphase (Sonderfall): [app-gokb](https://info.gbv.de/display/FOLIOGBVEXTERN/app-GOKb) und app-laser, weil es sich gut ins Schema (by-x und for-x und app-x und cat-x) einfügt. Wird aber eventuell noch geändert.
* [topic-](https://info.gbv.de/pages/viewpage.action?pageId=849379639)
    * Manche Dinge sollen übergreifend auffindbar sein. Beispiele [topic-passwort](https://info.gbv.de/display/FOLIOGBVEXTERN/topic-Passwort), [topic-tags](https://info.gbv.de/display/FOLIOGBVEXTERN/topic-Tags), [topic-datenschutz](https://info.gbv.de/display/FOLIOGBVEXTERN/topic-Datenschutz), [topic-edi](https://info.gbv.de/display/FOLIOGBVEXTERN/topic-Edi), [topic-exemplarstatus](https://info.gbv.de/display/FOLIOGBVEXTERN/topic-Exemplarstatus), [topic-sip2](https://info.gbv.de/display/FOLIOGBVEXTERN/topic-SIP2), [topic-kbart](https://info.gbv.de/display/FOLIOGBVEXTERN/topic-KBART) und eben viele mehr potentiell.
* [meta-](https://info.gbv.de/pages/viewpage.action?pageId=849379630)
    * Tags, die die Bearbeitung dieser Dokumentation unterstützen. Zum Beispiel [meta-Dokumentation](https://info.gbv.de/display/FOLIOGBVEXTERN/meta-Dokumentation) (Alles Festlegungen etc. rund um die Dokumentation) und [meta-Entwurf](https://info.gbv.de/display/FOLIOGBVEXTERN/meta-Entwurf) (unfertige aber ggf. veröffentlichte Seiten)
    * [dev-bug](https://info.gbv.de/pages/createpage.action?spaceKey=FOLIOGBVEXTERN&title=dev-Bugs&linkCreation=true&fromPageId=839909381) (wurde übersprünglich benutzt, soll aber durch ein meta-fehler o.ä. abgelöst werden ggf.)
        * Gelegentlich fallen beim Schreiben/Übersetzen Fehler auf, die aber nicht sofort gemeldet werden können oder ggf. nochmal geprüft werden müssen. Um die wiederzufinden, ist dieser spezielle Tag vergeben.

### Todo
Der erste Lauf zielt auf Vollständigkeit. Einige Dinge, die für zukünftige Verbesserungen zu bedenken sind, sind hier notiert.

* Dateinamen nochmal überlegen
* Bilder aus _moved_from_wrong_pasting nochmal schön einordnen ggf.
* Die Originaldoku hat Hugo/Docsy ziemlich beschnitten. Damit die DE-Struktur klappt, wurde daher vielfach wieder die Docsy-Defaults genommen. Checken.
* `date: 2023-02-01T00:00:00-00:00` ggf. entfernen? Autogenerieren aus Git(hub) wie in layouts\partials\page-meta-lastmod.html ?
* C:\ProgrammePortable\__NoSync\Seafile\Filesafe\Programme\UniServerZ\www\_gitRep\tub_dd\_folio\folio-docs\docs.folio.org_de-branched\content\de\docs\110 Dashboard\030 Workflows\080 TUB HH [Dashboard] - Widgets erstellen (Kurzanleitung).md 
  * Bilder
* "pane" ist mit "Ansicht" übersetzt. Könnte auch "Spalte mit dem Titel" o.ä. sein
* Neue Workflows
	* https://info.gbv.de/display/FOLIOGBVEXTERN/ZBW+%5BeManagement%5D%3A+Paketeintritt+und+Paketaustritt+von+E-Ressourcen?src=mail&src.mail.product=confluence-server&src.mail.timestamp=1676978404877&src.mail.notification=com.atlassian.confluence.plugins.confluence-content-notifications-plugin%3Apage-created-notification&src.mail.recipient=412e702f46c73d930146c741df94006e&src.mail.action=view
	* https://info.gbv.de/pages/viewpage.action?pageId=871530571&src=mail&src.mail.product=confluence-server&src.mail.timestamp=1676978187043&src.mail.notification=com.atlassian.confluence.plugins.confluence-content-notifications-plugin%3Apage-created-notification&src.mail.recipient=412e702f46c73d930146c741df94006e&src.mail.action=view
	* https://info.gbv.de/display/FOLIOGBVEXTERN/ZBW+%5BeManagement%5D%3A+Paketeintritt+und+Paketaustritt+von+E-Ressourcen?focusedCommentId=873037834&src=mail&src.mail.product=confluence-server&src.mail.timestamp=1677136800431&src.mail.notification=com.atlassian.confluence.plugins.confluence-notifications-batch-plugin%3Abatching-notification&src.mail.recipient=412e702f46c73d930146c741df94006e&src.mail.action=view#comment-873037834

## English
### Status of translation

2023-03-04. completeness can be seen in the concordance page (see [manual page concordance of translated documentation]({{< ref "Handbuchseiten-Konkordanz der uebersetzen Dokumentation" >}})). As of march 2023 only the pages "Single server or PC: fresh install", " Single server with containers", "quickMARC", "eHoldings" and "GOBI integration" are not translated.

### Background

- This translation of the official FOLIO documentation is an amateurish and unofficial recreational translation of [tzeumer@verweisunsgform.de](mailto:tzeumer@verweisunsgform.de)
- Translated with DeepL between 2022-12 and 2023-01 (see [English-German (DeepL)-Glossary]({{< ref "Englisch-Deutsch (DeepL)" >}})). Personal addresses ("you can...") were rephrased neutrally ("it can...").
- Live cross-checking was done in each case via [https://folio-snapshot.dev.folio.org](https://folio-snapshot.dev.folio.org/).
- It was first entered into the [GBV-Confluence](https://info.gbv.de/display/FOLIOGBVEXTERN/GBV+FOLIO+Documentation) and then moved here in 2023-02 as a fork of the Hugo version of the official documentation. Tools ([https://www.pastetomarkdown.com/](https://www.pastetomarkdown.com/) & [https://markdown-convert.com/en/tool/table](https://markdown-convert.com/en/tool/table) & [https://tableconvert.com/excel-to-markdown](https://tableconvert.com/excel-to-markdown))
- See also [see FOLIO wiki for documentation and conventions](https://wiki.folio.org/display/SS/FOLIO+Documentation).

### Changes to the official FOLIO documentation

- Config files from the original version, which were adapted or deleted/deactivated, are again in this branch with the file extension ".folio-official".
- The German version relies more on subpages ("Workflows" section fo each app) instead of very long pages for single apps.
- In the English documentation, the settings of all apps can be found under "Settings" (Einstellungen). The German version has this content sorted directly under the respective app and only keeps content without a clear app relationship  under "Settings" (Einstellungen).
- Apps may have "Best Practice" and "Worfklows from Users" as subsections (see section "Structure" further down).
- Each page links to the original English source ("Quelle: Folio" at the top of the page)
- Last/next page linked via TOC (if available)
- Tags were assigned

The first step (and probably at the same time last) was not about perfection, i.e. little time was spent on grammatically "nicer" sentences. In part it sounds a bit stiff, since the English version uses active forms of address both in Folio itself and in the documentation, while the [DACH-SIG D-Übersetzung](https://wiki.folio.org/pages/viewpage.action?pageId=33947726) (DE-Translation) has settled on passive formulations ("A license explains what you can do with the content your library can access." becomes "A license explains what can be done with the content that the library can access."). Gendering is largely already covered by the translations of D-Übersetzung, but in a few places it may still be insufficiently translated.

### License and version

This translation is a [fork of the FOLIO doc repository](https://github.com/folio-org/docs). According to it: "This software is distributed under the terms of the Apache License, Version 2.0. See the file '[LICENSE](https://github.com/folio-org/docs/blob/main/LICENSE)' for more information."

The copyright notice in the footer of the official documentation was changed on 2023-02-20 with the commit [Use CC-By 4.0 license and FOLIO project](https://github.com/folio-org/docs/commit/f51249ae7d0626ff2a3cdf201cdeb3407721a2ed).

### Sources

Significant sources are

- [Official FOLIO Documentation](https://docs.folio.org/)
- [Folio Wiki: Information and User Guides for FOLIO Apps](https://wiki.folio.org/display/FOLIOtips/Information+and+User+Guides+for+FOLIO+Apps)
- [User Libraries Contributions to this Wiki](https://info.gbv.de/display/FOLIOGBVEXTERN/by-Community)
- [FOLIO- Project: DACH Subject Groups](https://wiki.folio.org/display/Deutsche/D-A-CH+-subject-groups?src=contextnavpagetreemode) (especially lending, acquisitions, metadata management, and translation).

### Structure

The structure of the documentation is based on the structure of the official documentation (see also [FOLIO Wiki: About Documentation> Content standards](https://wiki.folio.org/display/SS/FOLIO+Documentation)). Thus, it has introduction, appendix, and main blocks on the major topic/task areas in libraries, such as collection access (circulation), collection management (acquisitions), metadata management (cataloging), and electronic resource management (ERM). The individual FOLIO apps are summarized and described below.

In many places in the manual, especially under the app pages, there is a "Best Practices" and/or "Workflows" and "User Workflows" subpage. These pages each have subpages. In the case of "Workflows from users" according to the scheme "Contributing institution: App/Topic + Action" (example: "TUB HH: License agreements initial entry"). The workflows from the original folio manual are all under " Workflows" with the order of the original documentation.

In addition, (formerly Confluence) labels are assigned to the pages, which can then be used to generate overviews and filters that are also independent of the (primary) hierarchical documentation structure. See in particular the overview lists from tags in the [Index](https://info.gbv.de/display/FOLIOGBVEXTERN/Index). There the use of a single tag is explained in more detail.

Example follow hereunder, as long as it has only suggestion character and there is no extra page yet. The labels could be chosen more specific if necessary, but can be adapted (relatively) easily later. There are the following label categories, which should be assigned (almost) all for most contributions

- [by-](https://info.gbv.de/pages/viewpage.action?pageId=849379549)
    - From whom the contribution originates. For example [by-ag\_folio](https://info.gbv.de/display/FOLIOGBVEXTERN/by-AG+Folio), [by-folio](https://info.gbv.de/display/FOLIOGBVEXTERN/by-Folio), [by-tubhh](https://info.gbv.de/display/FOLIOGBVEXTERN/by-TUB+Hamburg), [by-vzg](https://info.gbv.de/display/FOLIOGBVEXTERN/by-VZG), [by-zbw](https://info.gbv.de/display/FOLIOGBVEXTERN/by-ZBW)
    - Special: by-community\_x for collaboratively maintained/added documents. To easily filter these for overviews, split into two tags:
        - [by-community\_individual_contribution](https://info.gbv.de/display/FOLIOGBVEXTERN/by-Community_Einzelbeitrag): always together with by-NAME\_Organization like the examples in the first indent.
        - [by-community\_common](https://info.gbv.de/display/FOLIOGBVEXTERN/by-Community_Gemeinsam): Documents that are really directly supplemented by many institutions (a good example is the [license terms for license agreements](https://info.gbv.de/pages/viewpage.action?pageId=661979189)).
- [for-](https://info.gbv.de/pages/viewpage.action?pageId=849379622)
    - What is the target audience for the contribution? Currently [for-users](https://info.gbv.de/display/FOLIOGBVEXTERN/for-Anwender) for e.g. workflows in the apps themselves and [for-admin](https://info.gbv.de/display/FOLIOGBVEXTERN/for-Admin) for workflows in app settings.
    - In test phase: [for-developer](https://info.gbv.de/display/FOLIOGBVEXTERN/for-Entwickler) (analogously also for SIGs).
- [cat-](https://info.gbv.de/pages/viewpage.action?pageId=849379568)
    - Type of contribution. For example, [cat-bestpractises](https://info.gbv.de/display/FOLIOGBVEXTERN/cat-Best+practises) (from users), [cat-workflows](https://info.gbv.de/display/FOLIOGBVEXTERN/cat-Workflows) (from Folio and from users), [cat-settings](https://info.gbv.de/display/FOLIOGBVEXTERN/cat-Einstellungen) (from Folio), and [cat-permissions](https://info.gbv.de/display/FOLIOGBVEXTERN/cat-Berechtigungen) (usually also description of the app itself).
    - cat- means rather rigid, recurring structural elements of the documentation. Topic- (see below) on the other hand can be chosen more and more freely
- [app-](https://info.gbv.de/pages/viewpage.action?pageId=849379634)
    - Name of the folio app(s) involved. For example, app-persons, app-organizations.
    - Special case "app-settings". Since settings to specific apps are tagged with app-NAME and cat-setting. Global settings are tagged with app-settings. This is not necessarily logical or most useful, but convention for now. To still allow filtering, there is also cat-settings.
    - In testing (special case): [app-gokb](https://info.gbv.de/display/FOLIOGBVEXTERN/app-GOKb) and app-laser, because it fits well into the scheme (by-x and for-x and app-x and cat-x). But will be changed eventually.
- [topic-](https://info.gbv.de/pages/viewpage.action?pageId=849379639)
    - Some things should be findable across the board. Examples [topic-password](https://info.gbv.de/display/FOLIOGBVEXTERN/topic-Passwort), [topic-tags](https://info.gbv.de/display/FOLIOGBVEXTERN/topic-Tags), [topic-data-protection](https://info.gbv.de/display/FOLIOGBVEXTERN/topic-Datenschutz), [topic-edi](https://info.gbv.de/display/FOLIOGBVEXTERN/topic-Edi), [topic-exemplar-status](https://info.gbv.de/display/FOLIOGBVEXTERN/topic-Exemplarstatus), [topic-sip2](https://info.gbv.de/display/FOLIOGBVEXTERN/topic-SIP2), [topic-kbart](https://info.gbv.de/display/FOLIOGBVEXTERN/topic-KBART) and many more potentially.
- [meta-](https://info.gbv.de/pages/viewpage.action?pageId=849379630)
    - Tags that support editing this documentation. For example, [meta-documentation](https://info.gbv.de/display/FOLIOGBVEXTERN/meta-Dokumentation) (All specifications etc. around the documentation) and [meta-draft](https://info.gbv.de/display/FOLIOGBVEXTERN/meta-Entwurf) (unfinished but possibly published pages).
    - [dev-bug](https://info.gbv.de/pages/createpage.action?spaceKey=FOLIOGBVEXTERN&title=dev-Bugs&linkCreation=true&fromPageId=839909381) (was originally used, but should be replaced by a meta-bug or similar if necessary)
        - Occasionally errors are found while writing/translating, but cannot be reported immediately or may need to be rechecked. To find them again, this special tag is assigned.

### Todo

The first run aims at completeness. Some things to consider for future improvements are noted here.

- Reconsider file names
- Reorder images from \_moved\_from\_wrong\_pasting again nicely if necessary.
- Hugo/Docsy has trimmed the original doc quite a bit. So to make the DE structure work, many times the Docsy defaults were taken again. Check.
- Remove `date: 2023-02-01T00:00:00-00:00` if necessary? Autogenerate from Git(hub) as in layouts\partials\page-meta-lastmod.html ?
- C:\ProgramsPortable\_\_NoSync\\Seafile\Filesafe\Programs\UniServerZ\\www\_gitRep\tub\_dd\_folio\folio-docs\\docs.folio. org\_en-branched\\content\\de\docs\\110 Dashboard\\030 Workflows\\080 TUB HH \[Dashboard\] - Creating Widgets (Quick Start Guide).md
    - pane
- "pane" translates to "view". Could also be "column with the title" or similar.
