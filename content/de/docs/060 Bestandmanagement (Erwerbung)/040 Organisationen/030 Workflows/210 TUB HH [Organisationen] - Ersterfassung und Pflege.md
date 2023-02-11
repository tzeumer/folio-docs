---
title: "TUB HH [Organisationen] - Ersterfassung und Pflege"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [app-organisationen, by-tubhh, cat-workflows, for-anwender, by-community_einzelbeitrag]
weight: 10
Description: "
    Originalquelle ([by-TUB Hamburg](https://info.gbv.de/display/FOLIOGBVEXTERN/by-TUB+Hamburg); Stand 2023-01) & [GBV](https://info.gbv.de/display/FOLIOGBVEXTERN/TUB+HH+[Organisationen]+-+Ersterfassung+und+Pflege)
    "
---

{{% pageinfo %}}
Das ist lange nicht mehr aktualisiert worden. Reines Copy & Paste des Workflows hier derzeit.
{{% /pageinfo %}}

## Zu nutzende Quellen für einen Organisations-Datensatz in Folio

-   E-Mail-Verkehr im E-Medien Account (Kontaktpersonen)
-   Daten aus Lieferanten-Datensatz im ACQ (Kopf, Kontaktinformationen)
-   aktuelle Lizenzverträge und Rechnungen (Kontaktinformationen)
-   Pakete-Seiten im Wiki (Kontaktpersonen)
-   Admin-Zugangsdaten im Wiki (Interfaces)
-   Webseiten der Lieferanten/Anbieter/Verlage (Kontaktpersonen, Kontaktinformationen)

## Einpflegen von ACQ-Lieferanten

-   Für das ERM sind noch nicht alle Akkordeons und Felder in Folio relevant
-   Wenn Angaben im ACQ, Feldern in Folio zuzuordnen sind, übernehmen wir diese. Die Angaben müssen noch nicht vollständig sein.
-   Eine Vervollständigung der Angaben erfolgt ggf. sobald auch die Erwerbung über Folio läuft
-   Die Angaben aus dem ACQ werden bei Übernahme in Folio mit aktuellen, vorliegenden Dokumenten abgeglichen und ggf. ergänzt oder korrigiert (z.B. aktuellem E-Mail-Verkehr, Lizenzverträgen, Rechnungen etc.)

## Kopf

-   Pflichtfelder im Kopf sind Name, Code und Status
**Code**

-   Ist die Organisation schon im ACQ als Lieferant vorhanden, übernehmen wir den Code
-   Legen wir eine neue Organisation an, vergeben wir eine Buchstabenkombination, die wir vom Namen der Organisation ableiten
**Status**

-   Der Status der Organisation hat keinen Einfluss auf die ERM-Apps
-   Der Status wird zukünftig von den Apps "Bestellungen" und "Finanzen" ausgewertet. So können Bestellungen nur geöffnet und Rechnungen nur bezahlt werden, wenn die Organisation ein Lieferant mit dem Status Aktiv ist.
-   Der Status "vorläufig" kann genutzt werden, um einen Organisations-Datensatz als "Entwurf" zu kennzeichnen. Sobald die Organisation in einer ERM-App genutzt wird, sollte der Status aber geändert werden
**Häkchen bei Lieferant**

Wird das Häkchen bei "Lieferant" gesetzt, werden folgende zusätzliche Akkordeons freigeschaltet:

-   Lieferanteninformationen
-   Lieferantenbedingungen
-   EDI-Informationen
-   Konten
**Erwerbungsteams** Im Feld Erwerbungsteams ist keine Auswahlliste hinterlegt, da wir das Feld nicht nutzen

## Akkordeon Kontaktinformationen

-   In 4 Unterfeldern können die Adresse, Telefonnummer, E-Mail-Adresse und URL der Organisation angelegt werden
-   Es kann jeweils eine Kategorie ausgewählt werden. Diese haben wir selbst definiert.
-   Bei mehreren verwendeten Kategorien, werden die Kontaktinformationen nach Kategorien angezeigt
-   Die Kontaktinformationen sind nicht personenbezogen. Deshalb werden hier hauptsächlich die Adresse/n, Hotlines, allgemeine Webseiten etc. angegeben. Da wir bei den meisten Organisationen Ansprechpartner haben, werden die meisten Kontaktinformationen unter Kontaktpersonen verwaltet.

## Akkordeon Kontaktpersonen

-   Um eine neue Kontaktperson anlegen zu können, müssen zunächst alle vorher im Organisationen-Datensatz vorgenommenen Änderungen gespeichert, bzw. eine neu angelegte Organisation erst einmal gespeichert werden.
-   Die Personendaten werden in einer Hintergrund-App gespeichert. Vor dem Anlegen einer neuen Person kann die Hintergrund-App nach dieser Person durchsucht werden. Bei uns wird dies kaum vorkommen, da es eigentlich keine Personen gibt, die bei 2 Organisationen arbeiten. Somit kann die Person beim ersten Anlegen einer Organisation auch noch nicht vorhanden sein.
-   Bestandteile eines Personen-Datensatzes:
    -   Status: Aktiv/Inaktiv. Personen, die nicht mehr als Ansprechpartner fungieren oder nicht mehr bei einer Organisation arbeiten, werden auf "inaktiv" gesetzt
    -   Sprache: Die Sprache, die die Person spricht
    -   Kategorien: Es können die gleichen Kategorien vergeben werden, wie bei den Kontaktinformationen
    -   E-Mail-Adresse, Telefonnummer, URL, Adresse: Diese Informationen werden nur aufgenommen, wenn sie sich auf die jeweilige Person beziehen. Pro Information kann nochmal die Sprache und die Kategorie vergeben werden (keine Pflichtfelder)

## Interfaces

-   Unter "Interfaces" nehmen wir Webseiten mit Kennung und Zugang auf, die bisher im Wiki auf der Seite ERM: Administration Zugangskennungen verwaltet wurden.
-   Vor der Übernahme der Daten wird überprüft ob sie noch aktuell sind und bei älteren Angaben, ob sie überhaupt noch genutzt werden.
-   Die Angaben zu UStat werden nicht übernommen, da sie nicht mehr benötigt werden.
-   Im Media-Wiki wird nach Übernahme der Daten in die Organisationen-App beim jeweiligen Eintrag das Folio-Logo eingefügt (aus Vorlage übernommen).
-   Zusätzlich zu den Zugangsdaten können Informationen zu Statistiken hinzugefügt werden, wie z.B. Art der Bereitstellung und Angaben zum Format
-   Wir erfassen hier auch Webseiten, auf denen KBART-Dateien bereitgestellt werden (auch wenn hierfür keine Kennung notwendig ist)

## Lieferanteninformationen

**noch nicht relevant**

## Lieferantenbedingungen (erfassen wir noch nicht)

-   Hier kann ein Link zu den Lieferantenbedingungen des Lieferanten angegeben werden, sowie der Rabatt der grundsätzlich gewährt wird. Vorerst geben wir hier aber noch keinen Rabatt an. Sobald die Erwerbung über Folio läuft, müssen diverse Daten, die die Erwerbung betreffen in der Organisationen-App ergänzt werden.

## Edi-Informationen

-   Diese Informationen sind für das ERM nicht relevant. Bei Übernahme der Daten aus dem ACQ können aber Angaben übernommen werden, wenn diese den entsprechenden Feldern in Folio zugeordnet werden können

## Konten

-   Mit Konten sind Kundenkonten gemeint. Hier kann z.B. die Kundennummer erfasst werden.
