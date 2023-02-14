---
title: "VZG [Lizenzverträge] - Feldbeschreibung"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [app-lizenzverträge, by-vzg, cat-bestpractices, for-anwender, by-community_einzelbeitrag]
weight: 30
Description: "
    Quellen: [GBV](https://info.gbv.de/pages/viewpage.action?pageId=650608732)
    "
---

| |Feldbezeichnung|Beschreibung|Pflichtfeld|Wiederholbar|Typ|Gültige Werte|Ergänzende Informationen|
|:----|:----|:----|:----|:----|:----|:----|:----|
|2|Name|Ein von der Einrichtung vergebener Name für die Lizenz|Ja|Nein|String| |Beliebige Zeichenkette mit bis zu 255 Zeichen|
|3|Typ|Art der Lizenz|Ja|Nein|Auswahlliste| |Auswahlliste komplett pro Mandant konfigurierbar|
|4|Status|Aktueller Status der Lizenz|Ja|Nein|Auswahlliste| |Auswahlliste teilweise pro Mandant konfigurierbar|
|5|Startdatum|Datum, an dem die Lizenzvertragslaufzeit beginnt|Nein|Nein|Datum| |Beliebiges Datum|
|6|Enddatum|Datum, an dem die Lizenzvertragslaufzeit endet|Nein|Nein|Datum| |Beliebiges Datum nach dem Startdatum|
|7|Unbefristet|Wird verwendet, um anzuzeigen, dass die Lizenz unbefristet ist (hat kein festgelegtes Enddatum)|Nein|Nein|Boolean (true/false)|angehakt/abgehakt (wahr/falsch)|Ein Enddatum kann nicht gesetzt werden, wenn das Kontrollkästchen "unbefristet" aktiviert ist (true)|
|8|Beschreibung|Beschreibung für die von der Einrichtung erstellte Lizenz|Nein|Nein|String| |Bis zu 1Gb Text|
|9|Interne Kontakte|Zur Erfassung von Kontakten innerhalb der Bibliothek, die eine Verantwortung oder Rolle in Bezug auf die Lizenz haben|Nein|Ja|Interne Kontakte s. Reihen 10-11| |Siehe Definition eines internen Kontakts|
|10|Person|Eine Personr mit einer Beziehung zur Lizenz|Ja|Nein|Person in der Folio-Personen-App| |Jede Folio-Person|
|11|Rolle|Die Rolle/Beziehung, die die Person zur Lizenz hat|Ja|Nein|Auswahlliste| |Auswahlliste vollständig pro Mandant konfigurierbar|
|12|Organisation|Um Organisationen zu erfassen, die eine Verantwortung oder Rolle in Bezug auf die Lizenz haben|Nein|Ja|Organisationslink s. Reihen 13-14| |Siehe Definition eines Organisationslinks|
|13|Organisation (Orgnaisationslink)|Eine Organisation, die eine Beziehung zur Lizenz hat|Ja|Nein|Organisation in der Folio-Organisationen-App| |Beliebige Folio-Organisation|
|14|Rolle (Organisationslink)|Die Rolle/Beziehung, die die Organisation zur Lizenz hat|Ja|Nein|Auswahlliste| |Auswahlliste teilweise pro Mandant konfigurierbar|

# Links
[Feldbeschreibungen aller Apps (Link zum Google Dokument)](https://docs.google.com/spreadsheets/d/1ZpB3-SZwD07E71OVMR1TLie2CZ8wbEq_q1AF-gSGLXo/edit#gid=1148873991)
