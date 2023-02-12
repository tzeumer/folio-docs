---
title: "VZG - Berechtigungskonzepte"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [app-personen, by-vzg, cat-bestpractices, for-admin, cat-berechtigungen, by-community_einzelbeitrag]
weight: 10
Description: "
    Quellen: [GBV](https://info.gbv.de/display/FOLIOGBVEXTERN/VZG+%5BPersonen%5D+-+Berechtigungskonzepte)
    "
---

## Permission Sets - Ständig in Arbeit

* Diese Seite bietet Ihnen eine Vorlage zum Einrichten Ihrer Berechtigungssets, bitte beachten Sie, dass nach jedem Systemupdate auch neue Berechtigungen hinzukommen können. Um eine Übersicht über die neuen Berechtigungen zu erhalten, können Sie die SysAdmin-Kennung (mit allen Berechtigungen) suchen und nach nicht zugewiesenen Berechtigungen Filtern. Daran können Sie dann auch entscheiden, ob die neuen Berechtigungen evtl. anderen Berechtigungssets zugewiesen werden müssen. Sie finden die Information darüber aber auch in den jeweiligen Release Notes.
* In Testbetrieb wird nicht zwischen ERM-Bibliothekar\*innen, Fachreferent\*innen, Abteilungsleitung usw. unterschieden. Es wird ein Permission Set definiert, welches den ERM-Bearbeiter\*innen in der User-Verwaltung zugewiesen wird.
* Zusätzlich gibt es ein Permission Set für Administrative ERM-Aufgaben in den Systemeinstellungen, wie bspw. das Anlegen neuer License Terms oder anderer Kategorien.
* Für die systemweite Administration gibt es ein weitere Permission Set, welches alle verfügbaren Berechtigungen enthält. Dieses Permission Set wird allen Systemverwalter\*innen zugewiesen. **Sofern ein Systemverwalter auch reguläre Aufgaben im System wahrnimmt, sollte dafür ein separater Account ohne "sudo"-Permissions genutzt werden.**

## History

* 2022-12-07: Spalte "Seit Version" ergänzt
* 2022-12-07: [Neue Lotus-Berechtigungen](https://wiki.folio.org/display/REL/Lotus+(R1+2022)+Release+Notes#Lotus(R12022)ReleaseNotes-PermissionsUpdates) ergänzt


|Permission Set Name|Beschreibung (für Description-Feld in Folio)|besteht aus folgenden Berechtigungen|Seit Version|
|:----|:----|:----|:----|
|ERM | lesender Zugriff|Nur Anzeigeberechtigungen|Agreements: Search & view agreements| |
| | |eUsage: Can view, create, edit and delete usage data providers and COUNTER reports| |
| | |Licenses: Search & view licenses| |
| | |Notes: Can view a note| |
| | |Organizations: Interface usernames and passwords: view| |
| | |Organizations: View| |
| | |Settings (My profile): Can change your local password| |
| | |Settings (notes): display list of settings pages| |
| | |UI: ui-notes module is enabled| |
| | |Users: Can view user profile| |
|ERM-Personal| |Agreements: Edit agreements| |
| | |Agreements: Edit e-resources| |
| | |Agreements: Search & view agreements| |
| | |Agreements: Search & view e-resources| |
| | |Agreements: File download| |
| | |ERM Comparisons: Create jobs| |
| | |ERM Comparisons: Delete jobs| |
| | |ERM comparisons: View jobs| |
| | |eUsage: Can view, create, edit and delete usage data providers and COUNTER reports| |
| | |Find License Plugin: Search licenses| |
| | |Licenses: Search & view licenses| |
| | |Licenses: Edit licenses| |
| | |Notes: Can assign and unassign a note| |
| | |Notes: Can create a note| |
| | |Notes: Can delete a note| |
| | |Notes: Can edit a note| |
| | |Notes: Can view a note| |
| | |Orders: Assign acquisition units to new order| |
| | |Orders: Create order lines| |
| | |Orders: Create orders| |
| | |Orders: Delete order lines| |
| | |Orders: Edit order lines| |
| | |Orders: Edit orders| |
| | |Orders: Manage acquisition units| |
| | |Orders: Receive items| |
| | |Orders: Remove orders| |
| | |Orders: Reopen purchase orders| |
| | |Orders: Unopen purchase orders| |
| | |Orders: View order lines| |
| | |Orders: View orders| |
| | |Organizations: Assign acquisition units to new organization| |
| | |Organizations: Manage acquisition units| |
| | |Organizations: Interface usernames and passwords: view, edit, create, delete| |
| | |Organizations: View, edit, create| |
| | |Organizations: View, edit, create| |
| | |Settings (My profile): Can change your local password| |
| | |Settings (notes): display list of settings pages| |
| | |UI: ui-notes module is enabled| |
| | |Users: Can view user profile| |
|ERM-Admin|Berechtigung für den ERM-Admin. Enthält alle Berechtigungen von ERM-Personal und zusätzlich Berechtigungen für Systemeinstellungen.|Agreements: Delete agreements| |
| | |Agreements: Edit agreements| |
| | |Agreements: Edit e-resources| |
| | |Agreements: Search & view agreements| |
| | |Agreements: Search & view e-resources| |
| | |ERM Comparisons: Create jobs| |
| | |ERM Comparisons: Delete jobs| |
| | |ERM comparisons: View jobs| |
| | |eUsage harvester: All permissions for eUsage harvester module| |
| | |Find License Plugin: Search licenses| |
| | |Licenses: Delete licenses| |
| | |Licenses: Edit licenses| |
| | |Local KB admin: Create jobs| |
| | |Local KB admin: Delete jobs| |
| | |Local KB admin: Manage remote KB configuration| |
| | |Notes: Can assign and unassign a note| |
| | |Notes: Can create a note| |
| | |Notes: Can delete a note| |
| | |Notes: Can edit a note| |
| | |Notes: Can view a note| |
| | |Orders: Assign acquisition units to new order| |
| | |Orders: Check-in items| |
| | |Orders: Create order lines| |
| | |Orders: Create orders| |
| | |Orders: Delete order lines| |
| | |Orders: Edit order lines| |
| | |Orders: Edit orders| |
| | |Orders: Manage acquisition units| |
| | |Orders: Receive items| |
| | |Orders: Remove orders| |
| | |Orders: Reopen purchase orders| |
| | |Orders: Unopen purchase orders| |
| | |Orders: View order lines| |
| | |Orders: View orders| |
| | |Organizations: Interface usernames and passwords: view, edit, create, delete| |
| | |Organizations: View, edit, create| |
| | |Organizations: View, edit, delete| |
| | |Settings (Agreements): Can view app settings|Lotus (R1 2022)|
| | |Settings (Agreements): Can view and edit app settings|Lotus (R1 2022)|
| | |Settings (eUsage): Can view and edit settings| |
| | |Settings (Licenses): Can view app settings| |
| | |Settings (Licenses): Can view and edit app settings|Lotus (R1 2022)|
| | |Settings (Licenses): Manage license terms|Lotus (R1 2022)|
| | |Settings (Licenses): Manage pick lists and values| |
| | |Settings (My profile): Can change your local password| |
| | |Settings (notes): display list of settings pages| |
| | |Settings (Orders): Display list of settings for Orders| |
| | |UI: ui-notes module is enabled| |
| | |Users: Can view user profile| |
|Systemverwaltung|Alle Berechtigungen, zur Verwaltung des Systems.|alle Berechtigungen| |


|Ein User mit ERM Lesezugriff soll:|Suche nach App (englisch und deutsch)|Berechtigung auswählen, die diesen Begriff enthält|Berechtigung darf diesen Begriff nicht enthalten|
|:----|:----|:----|:----|
|Anmerkungen/Notizen lesen können|Notiz anzeigen| | |
|Suchen in den ERM-relevanten Apps durchführen können|Organizations/Organisationen Licenses/Lizenzverträge agreements/eManagement Users/Personen|view/anzeigen search/suchen| |
|in den ERM-relevanten Apps lesen/sehen können| | | |
|unter "Mein Profil" sein Passwort ändern können|Mein Profil| | |
