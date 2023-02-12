---
title: "TUB HH [Personen] - Benutzerkonten anlegen"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [app-personen, by-tubhh, for-anwender, cat-workflows, by-community_einzelbeitrag]
weight: 190
Description: "
    Quellen: [Originalquelle TUBHH](https://intranet.b.tu-harburg.de/mediawiki/index.php/FOLIO/Module/ERM/Workflows/Benutzer-Accounts_anlegen) & [GBV](https://info.gbv.de/display/FOLIOGBVEXTERN/TUB+HH+[Personen]+-+Benutzerkonten+anlegen)
    "
---

{{% pageinfo %}}
Hinweis: Mit [VZG (Personen): Berechtigungskonzepte](https://info.gbv.de/display/FOLIOGBVEXTERN/VZG+%28Personen%29%3A+Berechtigungskonzepte?src=contextnavpagetreemode) ist mindesten Schritt 3 schon als spezifischer Punkt überflüssig. Einige andere werden sicher auch standardisiert(er) werden (Personengruppen). Schritt 6 ist wahrscheinlich obsolet, wenn [Folio: Person Passwortrücksetzungs-E-Mail senden](https://info.gbv.de/pages/viewpage.action?pageId=840859873) funktioniert (noch nicht probiert). Kurz, der Workflow ist leicht antik und evtl. eher überflüssig.
{{% /pageinfo %}}

# Workflow

## 1\. Schritt: Personengruppe anlegen

Da die Benutzer einer Personengruppe zugeordnet werden, muss diese, wenn noch nicht vorhanden, vorher angelegt werden. Siehe [GBV FOLIO Dokumentation > Personen > Einstellungen (Personen): Personengruppen](https://info.gbv.de/display/FOLIOGBVEXTERN/Einstellungen+%28Personen%29%3A+Personengruppen)

Unser (alter, redundante Workflow)

* App "Einstellungen">Personen>Allgemein>Personengruppen
* Es muss ein Name und ggf. eine Beschreibung eingegeben werden

## 2\. Schritt: Adresstyp

Wird beim Benutzer auch eine Adresse hinterlegt, müssen vorher Adresstypen erstellt werden, wenn noch nicht vorhanden. Siehe [GBV FOLIO Dokumentation > Personen > Einstellungen (Personen): Adresstypen](https://info.gbv.de/display/FOLIOGBVEXTERN/Einstellungen+%28Personen%29%3A+Adresstypen)

* App "Einstellungen>Personen>Allgemein>Adresstyp
* Beispiele:
    * Dienstanschrift
    * Privatanschrift

## 3\. Schritt: Berechtigungsgruppe erstellen

Wir verwenden die Berechtigungsgruppen, die im Verbund gemeinsam definiert wurden. Falls Bedarf an neuen besteht, sollte dies dort abgeklärt werden. Siehe [GBV FOLIO Dokumentation > Personen > Best Practice (Personen) > VZG (Personen): Berechtigungskonzepte](https://info.gbv.de/display/FOLIOGBVEXTERN/VZG+%28Personen%29%3A+Berechtigungskonzepte).

[Standardworkflow: GBV FOLIO Dokumentation > Personen > Einstellungen (Personen): Berechtigungsgruppen](https://info.gbv.de/display/FOLIOGBVEXTERN/Einstellungen+%28Personen%29%3A+Berechtigungsgruppen)

Unser (alter, redundante Workflow)

* App "Einstellungen">Personen>Allgemein>Berechtigungsgruppen
* Neu
* Der Berechtigungsgruppe einen Namen vergeben und eine passende Beschreibung
* Auf "Berechtigung hinzufügen" klicken
* Filter für "Berechtigungen" anwenden
* Die gewünschten Berechtigungen auswählen und speichern
* Die Berechtigungsgruppe speichern

## 4\. Schritt: Benutzer anlegen

In der Personen-App mit dem "+" einen neuen Benutzer anlegen. Siehe [GBV FOLIO Dokumentation > Personen > Workflows Personen > Folio: Person anlegen](https://info.gbv.de/display/FOLIOGBVEXTERN/Folio%3A+Person+anlegen)

Minimal auszufüllen sind folgende Felder:

* Personeninformationen
    * Nachname
    * Personengruppe (für Folio-Nutzer die Gruppe "TUHH-Mitarbeiter"
    * Status: Aktiv
    * Benutzername (Wir verwenden die Kerberos-Kennung)
* Kontaktinformationen:
    * E-Mail
    * Bevorzugte Kontaktmöglichkeit

## 5\. Schritt: Berechtigungsgruppe zuweisen

Siehe [GBV FOLIO Dokumentation > Personen > Workflows Personen > Folio: Person Rechte zuweisen](https://info.gbv.de/display/FOLIOGBVEXTERN/Folio%3A+Person+Rechte+zuweisen)

* Nach dem Speichern, die Person im Bearbeitungs-Modus nochmal öffnen
* Im Akkordeon _Systemberechtigungen_ eine oder mehrere Berechtigungen (Berechtigungsgruppen) vergeben

## 6\. Schritt: Passwort für den Benutzer erstellen

Der offizielle Weg ist [GBV FOLIO Dokumentation > Personen > Workflows Personen > Folio: Person Passwortrücksetzungs-E-Mail senden](https://info.gbv.de/pages/viewpage.action?pageId=840859873). Da der nicht funktionierte (bzw. aktuell zu testen, ob es geht), gab es auch den alternativen Weg über Einstellungen > Entwickler, wie folgt:

* In der App "Einstellungen", "Entwickler" öffnen und die Einstellung "Passwd. anklicken
* Bei Systemkennung den Benutzernamen eingeben
* Neues Passwort vergeben und zur Bestätigung nochmal eingeben
* erstelltes "Standardpasswort" an Benutzer weiterleiten.
* Neues Passwort kann vom Nutzer nach dem Einloggen oben rechts vergeben werden.
