---
title: "Allgemein"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [app-einstellungen, by-folio, cat-einstellungen, for-admin, meta-uebersetzungsproblem]
weight: 10
Description: "
    Quellen: [Folio](https://docs.folio.org/docs/settings/settings_oaipmh/settings_oaipmh/#settings--oai-pmh--general) <!-- & [GBV](https://info.gebev.de/display/FOLIOGBVEXTERN/Einstellungen+(OAI-PMH):+Allgemein) -->
    "
---

{{% pageinfo %}}
Englische Originalfassung. ("Time granularity", "Administrator E-Mail(s)")
{{% /pageinfo %}}

Allgemeine Einstellungen, um zu konfigurieren, wie das [**Identify** verb](http://www.openarchives.org/OAI/openarchivesprotocol.html#Identify) antwortet.

## OAI-Dienst aktivieren

Checkbox, um OAI-Dienste global zu aktivieren oder zu deaktivieren.

## Repository-Name

Legt den Inhalt des XML-Elements `respositoryName` in der Identify-Response fest.

## Basis-URL

Legt den Inhalt des XML-Elements `baseURL` in der Identify-Response fest. Dieser Wert erscheint auch im Inhalt des XML-Elements `response` des ListRecords verb.

## Time granularity

Legt den Inhalt des XML-Elements `granularity` in der Identify-Response fest.

## Administrator E-Mail(s)

Legt den Inhalt des XML-Elements `adminEmail` der Identify-Response fest.
