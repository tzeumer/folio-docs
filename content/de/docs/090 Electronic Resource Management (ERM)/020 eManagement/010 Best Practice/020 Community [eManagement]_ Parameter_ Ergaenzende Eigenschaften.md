---
title: "Community [eManagement]: Parameter: Ergänzende Eigenschaften"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [app-e_management, cat-bestpractices, for-admin, by-community_gemeinsam, by-tubhh, by-vzg]
weight: 20
Description: "
    Quellen: [GBV](https://info.gbv.de/pages/viewpage.action?pageId=676167734)
    "
---

## Bedingungen
|Annzeigename|Name|Beschreibung|Primäre Eigenschaft|Reihenfolge |Standardmäßige Sichtbarkeit |Typ|Auswahlliste|Name der ergänzenden Einrichtung|Verwendet von|
|:----|:----|:----|:----|:----|:----|:----|:----|:----|:----|
|Fakultät|Fakultaet|Fakultät, für die die Ressource erworben wird|Ja| |Intern|Auswahlliste|Fakultäten|VZG| |
|Ressourcentyp|RessourcenTyp|Welche Ressourcen werden verwaltet?|Ja| |Intern|Auswahlliste|Ressource.Typ|VZG| |
|ACQ-Bestell-Nr. |acqBestellnummer|Aktuell gültige Bestellnummer eines laufenden Pakets in ACQ|ja|1|Intern|Text| |TUBHH|TUBHH|
|DBIS-ID|dbisId|DBIS-Zugangsnummer für Datenbanken|Ja|1|Intern|Text| |TUBHH|TUBHH|
|SFX-Target|sfxTarget|Für den SFX-Linkresolver|ja|1|Intern|Text| |TUBHH|TUBHH|
|Ressourcen-Typ|resourceType|Welche Ressourcen-Arten enthält das Paket?|ja|3|Intern|Auswahlliste|resource.type|TUBHH|TUBHH|
|Rechnungsstellung|rechnung|Angaben zur Rechnungsstellung. Wann wird die Rechnung zugestellt?|ja|4|Intern|Text| |TUBHH|TUBHH|
|Link zum Paket|paketlink|Link zum Paket, z.B. für die Ermittlung der Bandanzahl eines E-Book-Pakets|Ja|5|Intern|Text| |TUBHH|TUBHH|
|EZB Anker|ezbAnchor|Welcher Anker wird für den Paketinhalt in der EZB verwendet?|Nein|0|Intern|Text| |TUBHH|TUBHH|
|EZB-Readme|ezbReadme|Direkt-Link zum EZB-Readme|Nein|0|Intern|Text| |TUBHH|TUBHH|
|Produktsigel aus ZDB (ISIL)|zdbProduktsigel|Für e-Book-Pakete: Welches Produktsigel ist in der ZDB für dieses Paket hinterlegt? Bzw. über welches Produktsigel werden hier durch den Verbund Exemplare erzeugt (über EBM-Tool)?|Nein|0|Intern|Text| |TUBHH|TUBHH|
|K10Plus|k10plus|Hinweise zu den Paketen/Paket-Titeln im K10Plus|Nein|5|Intern|Text| |TUBHH|TUBHH|
|Metadaten|metadaten|Hinweise zu Metadaten, z.B. aktuell nicht verfügbaren, oder angeforderten Daten|Nein|5|Intern|Text| |TUBHH|TUBHH|
|Abrufzeichen 8600|ablolr|Ist in den Datensätzen die durch das EBM-Tool angelegt werden in der 8600 enthalten und dient der Auffindbarkeit der lizenzierten Titel. Suchbar im CBS mit f abl ... Bei Belegung in Af- oder Av-Sätzen erfolgt eine entsprechende Kennzeichnung auch in Ac-/Ab-/Ad-Aufnahmen|Nein|1|Intern|Text| |TUBHH|TUBHH|
