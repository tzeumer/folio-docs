---
title: "Einstellungen (OAI-PMH)"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [app-einstellungen, by-folio, cat-berechtigungen, cat-einstellungen, for-admin, meta-uebersetzungsproblem]
weight: 10
Description: "
    Quellen: [Folio](https://docs.folio.org/docs/settings/settings_oaipmh/settings_oaipmh/) <!-- & [GBV](https://info.gebev.de/pages/viewpage.action?pageId=850002078) -->
    "
---

{{% pageinfo %}}
Fehlende Übersetzungen. ("Einstellungen (OAI-PMH): Liste der Einstellungsseiten anzeigen.", "Einstellungen (OAI-PMH): Kann Einstellungen anzeigen und bearbeiten.")
{{% /pageinfo %}}

Im Abschnitt OAI-PMH der App Einstellungen kann das Verhalten des OAI-PMH-Feeds von FOLIO konfiguriert werden. Mehr über die OAI-PMH-Spezifikation erfahren: [OAI-PMH Specification at the Open Archives website](http://www.openarchives.org/OAI/openarchivesprotocol.html).

FOLIO unterstützt derzeit drei Metadatenformate:

* marc21
* oai\_dc
* marc21\_withholdings

Diese Liste kann mit dem [**ListMetadataFormats** verb](http://www.openarchives.org/OAI/openarchivesprotocol.html#ListMetadataFormats) eingesehen werden.

## Berechtigungen

Um mit den OAI-PMH-Einstellungen zu interagieren, muss einer Person die folgende Berechtigung zugewiesen werden:

* **Einstellungen (OAI-PMH): Liste der Einstellungsseiten anzeigen**.  (Settings (OAI-PMH): Can view)
    Diese Berechtigung ermöglicht es der Person, alle OAI-PMH-Einstellungen anzuzeigen, aber die Schaltfläche "Speichern" ist deaktiviert. Personen erhalten die Meldung "Ihnen fehlen die erforderlichen Berechtigungen zum Bearbeiten der OAI-PMH-Einstellungen. Bitte wenden Sie sich an den Systemadministrator."
* **Einstellungen (OAI-PMH): Kann Einstellungen anzeigen und bearbeiten**. (Settings (OAI-PMH): Can view and edit settings)
    Diese Berechtigung erlaubt der Person, die OAI-PMH-Einstellungen anzuzeigen und zu bearbeiten.
