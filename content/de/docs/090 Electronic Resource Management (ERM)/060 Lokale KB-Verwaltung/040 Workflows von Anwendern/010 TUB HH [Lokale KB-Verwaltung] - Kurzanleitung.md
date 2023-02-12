---
title: "TUB HH [Lokale KB-Verwaltung] - Kurzanleitung"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [app-lokale_kb_verwaltung, by-tubhh, cat-workflows, for-anwender, by-community_einzelbeitrag]
weight: 700
Description: "
    Quellen: [Folio](xxx) & [GBV](xxx)
    "
---

## Zweck der App

Die App ermöglicht die direkte Einspielung von Paketen in Folio per KBART-Datei, ohne diese in der GOKb zu erfassen.

## Wann nutzt man diese App?

Grundsätzlich sollten Pakete in der GOKb erfasst und gepflegt werden und werden auf diesem Weg in die interne Knowledgebase von Folio eingespielt und nicht über direkte Einspielung in Folio. Möchte man ein Paket aber nicht in der GOKb pflegen, kann die lokale KB-Verwaltung genutzt werden. Ein möglicher Grund hierfür wäre ein geplanter Vergleich von Paketen in der App "eVergleich".

## Durchführung eines KBART-Imports

1.  In der App "Lokale KB-Verwaltung" oben rechts auf "Aktionen" klicken
2.  "KBART-Importjob auswählen
3.  Die Pflichtfelder ausfüllen:
    * Paketname: Der Name sollte eindeutig sein und den Paketnamen in der GOKb entsprechen, da das Paket der internen Knowledgebase in Folio hinzugefügt wird
    * Paketquelle: Bei Paketen aus der GOKb ist hier "GOKb" angegeben. Bei lokal eingespielten Paketen würde ich "Lokale KB" angeben, damit zu erkennen ist, dass das Paket nicht aus der GOKb stammt
    * Paketreferenz: Sollte dem Pakettitel entsprechen, nur dass die einzelnen Wörter mit Unterstrich getrennt werden, z.B.: Springer\_Mathematics\_and\_Statistics\_eBooks\_2022\_English/International\_2
    * Außerdem muss ein Häkchen gesetzt werden bei "Diesem Job als Quelle für Titelinstanz-Metadaten vertrauen"
    * Weiterhin sollte der Paketanbieter erfasst werden, auch wenn dies kein Pflichtfeld ist
4.  Die Datei hochladen durch Drag & Drop oder durch Auswählen der Datei
5.  Auf "Speichern und schließen" klicken
6.  Der Importjob wird nun in der Ergebnisliste der lokalen KB-Verwaltung angezeigt ![](/img/de/../../../attachments/070TUB~1_2023-02-10-17-59-25.png)
8.  Sobald der Job beendet ist, wird er nur noch angezeigt, wenn man in der Such- und Filterspalte ein Häkchen beim Status "beendet" setzt
9.  Weitere Informationen zum ausgeführten Importjob erhält man im Datensatz in den Akkordeons "Fehlerprotokoll" und "Infoprotokoll"
10. Das Paket wurde der internen Knowledgebase hinzugefügt und ist jetzt in der eManagement-App im Reiter E-Ressourcen auffindbar

## Löschen eines Importjobs

Das Löschen eines Importjobs ist möglich. Allerdings wird damit nur die Dokumentation des KBART-Imports gelöscht, aber nicht das Paket in der internen Knowledgebase. Ein über die App eingespieltes Paket kann derzeit nicht aus der internen Knowledgebase gelöscht werden.
