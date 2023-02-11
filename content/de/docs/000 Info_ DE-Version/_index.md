---
title: "Info: DE-Version"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: []
weight: 10
Description: "
    Quellen: [Folio](https://docs.folio.org/docs/) & [GBV](https://info.gbv.de/display/FOLIOGBVEXTERN/GBV+FOLIO+Dokumentation)
    "
---

## Deutsch
### Stand der Übersetzung
2023-02-11. Die Vollständigkeit ist in der Konkordanzseite zu sehen (siehe [Handbuchseiten-Konkordanz der übersetzen Dokumentation]({{< ref "Handbuchseiten-Konkordanz der übersetzen Dokumentation" >}}))

### Hintergrund
* Diese Übersetzung der offiziellen FOLIO-Dokumentation ist eine laienhaft und inoffizielle Freizeitübersetzung von [tzeumer@verweisunsgform.de](mailto:tzeumer@verweisunsgform.de)
* Übersetzt wurde mit DeepL (siehe [Englisch-Deutsch (DeepL)-Glossar]({{< ref "Englisch-Deutsch (DeepL)" >}})). Persönliche Ansprachen ("Sie") wurden neutral umformuliert.
* Live gegengeprüft wurde jeweils via https://folio-snapshot.dev.folio.org
* Sie wurde zuerst ins [GBV-Confluence](https://info.gbv.de/display/FOLIOGBVEXTERN/GBV+FOLIO+Dokumentation) eingetragen. Die Seite ist frei zugänglich, aber aus technischen Gründen musste ein Login vorgeschaltet werden. Die Zugangsdaten sind: info_folio / folio.
* Sie wurde ab 2023-02 in die Hugo-Struktur übernommen. Tools (https://www.pastetomarkdown.com/ & https://markdown-convert.com/en/tool/table & https://tableconvert.com/excel-to-markdown)

### Änderungen zur offiziellen FOLIO-Dokumentation
* Config-Dateien aus der Original-Version, die angepasst oder gelöscht/deaktivert wurden, liegen mit der  Dateierweiterung ".folio-official" nochmal in diesem Branch
* Die Deutsche Version setzt stärker auf Unterseiten, statt sehr langen Seiten zu einzelnen Apps. 
* Es wurden Tags vergeben

### Todo
Der erste Lauf zielt auf Vollständigkeit. Einige Dinge, die für zukünftige Verbesserungen zu bedenken sind, sind hier notiert.

* Replace "-   " mit "* "
* Dateinamen nochmal überlegen
  * Interne Links (info.gbv.de) anpassen
* Bilder aus _moved_from_wrong_pasting nochmal schön einordnen ggf.
* Die Originaldoku hat Hugo/Docsy ziemlich beschnitten. Damit die DE-Struktur klappt, wurde daher vielfach wieder die Docsy-Defaults genommen. Checken.
* `date: 2023-02-01T00:00:00-00:00` ggf. entfernen? Autogenerieren aus Git(hub) wie in layouts\partials\page-meta-lastmod.html ?
* C:\ProgrammePortable\__NoSync\Seafile\Filesafe\Programme\UniServerZ\www\_gitRep\tub_dd\_folio\folio-docs\docs.folio.org_de-branched\content\de\docs\110 Dashboard\030 Workflows\080 TUB HH [Dashboard] - Widgets erstellen (Kurzanleitung).md 
  * Bilder

## English
### Status of translation
2023-02-11. For completeness, see the concordance page (see [manual page concordance of translated documentation]({{< ref "Handbuchseiten-Konkordanz der übersetzen Dokumentation" >}})).

### Background
* This translation of the official FOLIO documentation is an amateurish and unofficial recreational translation of [tzeumer@verweisunsgform.de](mailto:tzeumer@verweisunsgform.de)
* Translated using DeepL (see [English-German (DeepL) glossary]({{< ref "Englisch-Deutsch (DeepL)" >}})). Personal addresses (Sie/"you") were rephrased neutrally.
* Live cross-checking was done via https://folio-snapshot.dev.folio.org in each case.
* It was first entered into the [GBV-Confluence](https://info.gbv.de/display/FOLIOGBVEXTERN/GBV+FOLIO+Documentation). The page is freely accessible, but for technical reasons, a login had to be set up beforehand. The login details are: info_folio / folio.
* It has been incorporated into the Hugo structure as of 2023-02. Tools (https://www.pastetomarkdown.com/ & https://markdown-convert.com/en/tool/table & https://tableconvert.com/excel-to-markdown)

### Changes to the official FOLIO documentation
* Config files from the original version, which were adapted or deleted/deactivated, are again in this branch with the file extension ".folio-official".
* The German version relies more on subpages instead of very long pages for individual apps. 
* Tags were assigned

### Todo
The first run aims at completeness. Some things to consider for future improvements are noted here.

* Replace "- " with "* "
* Reconsider file names
  * Adapt internal links (info.gbv.de)
* Arrange pictures from _moved_from_wrong_pasting again nicely if necessary.
* The original docu has Hugo/Docsy quite trimmed. So to make the DE structure work, many times the Docsy defaults were taken again. Check.
* Remove `date: 2023-02-01T00:00:00-00:00` if necessary? Autogenerate from Git(hub) as in layouts\partials\page-meta-lastmod.html ??
* C:\ProgramsPortable\__NoSync\Seafile\Filesafe\Programs\UniServerZ\www\_gitRep\tub_dd\folio\folio-docs\docs.folio.org_en-branched\content\de\docs\110 Dashboard\030 Workflows\080 TUB HH [Dashboard] - Create Widgets (Quick Start Guide).md 
  * Images
