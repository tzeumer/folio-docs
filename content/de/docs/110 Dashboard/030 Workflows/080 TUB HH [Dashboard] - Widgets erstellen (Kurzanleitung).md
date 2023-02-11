---
title: "TUB HH [Dashboard] - Widgets erstellen (Kurzanleitung)"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [app-dashboard, by-tubhh, cat-workflows, for-anwender, by-community_einzelbeitrag]
weight: 80
Description: "
    Quellen: [Originalquelle](https://intranet.b.tu-harburg.de/mediawiki/index.php/FOLIO/Module/ERM/Workflows/Erstellung_von_Dashboard_Widgets) & [GBV](https://info.gbv.de/pages/viewpage.action?pageId=749207653)
    "
---

{{% pageinfo %}}
* Stand 2023-01
* Das wird ab Nolana eher hinfällig und ist so auch nur sehr begrenzt genutzt worden. Erst mal reines Copy & Paste, ohne weitere Prüfung auf Korrektheit/Aktualität.
{{% /pageinfo %}}

## Dashboard allgemein

Das Dashboard in Folio dient dazu, den Überblick über einzelne Vorgänge in Folio nicht zu verlieren. Bisher können im Dashboard Daten aus der Lizenzverträge-App und der eManagement-App abgerufen und dargestellt werden. Jeder Folio-Nutzer kann sich selbst "Widgets" erstellen, in dem er Filter verwendet und Regeln erstellt.

## Ein neues Widget anlegen

1.  Das Dashboard aufrufen
2.  Auf "Aktionen" und dann auf "Neu" klicken
3.  Im Feld "Widget-Name" einen Namen vergeben:
    -   Der Name sollte möglichst genau beschreiben, was im Widget dargestellt wird, damit man auch nach mehreren Wochen noch nachvollziehen kann, welche Daten abgerufen werden, z.B.:
        -   "Alle AKTIVEN Lizenzverträge, die in den nächsten 3 Monaten ablaufen"
        -   "Alle Vereinbarungen, die bis 31.12.2022 ablaufen"
        -   "Alle Vereinbarungen mit einer eingetragenen Stornierungsfrist im Jahr 2022"
        -   "Alle Vereinbarungen, an denen das Fachreferat 3 beteiligt ist"
4.  Im Feld Widget-Definition ist die App auszuwählen aus der Daten ins Widget übernommen werden sollen (ERM-Agreement = eManagement-App)
5.  Nach Auswahl der App öffnen sich mehrere Akkordeons
6.  Im Akkordeon Filter ein Feld aus dem Vereinbarungsformular auswählen, nach dem man filtern möchte und eine entsprechende Regel aufstellen.
    -   Hier einige Beispiele anhand von Screenshots:
        -   Ich möchte eine Liste aller aktiven Vereinbarungen, die "Springer" im Namen haben:
            [![Widgets1.png](https://intranet.b.tu-harburg.de/mediawiki/images/thumb/1/1f/Widgets1.png/1005px-Widgets1.png)](https://intranet.b.tu-harburg.de/mediawiki/index.php/Datei:Widgets1.png)

        -   Ich möchte alle Vereinbarungen angezeigt bekommen, bei denen die Stornierungsfrist ab dem heutigen Tag innerhalb der nächsten 3 Monate abläuft:
            [![Widgets2.png](https://intranet.b.tu-harburg.de/mediawiki/images/e/ea/Widgets2.png)](https://intranet.b.tu-harburg.de/mediawiki/index.php/Datei:Widgets2.png)
        -   Ich möchte alle Vereinbarungen angezeigt bekommen an denen das Fachreferat 3 beteiligt ist - hierfür wird ein Suchfenster in der Personen-App geöffnet, um die Person bzw. das Fachreferat auszuwählen:

            [![Widgets3.png](https://intranet.b.tu-harburg.de/mediawiki/images/thumb/8/83/Widgets3.png/1005px-Widgets3.png)](https://intranet.b.tu-harburg.de/mediawiki/index.php/Datei:Widgets3.png)

7.  Akkordeon Ergebnisanzeige
    -   Anzahl der Zeilen: Auswählen wieviele Zeilen/Treffer im Widget gleichzeitig dargestellt werden sollen
    -   Sortieren nach: Auswählen, nach welcher Eigenschaft/ welchem Feld die Zeilen im Widget sortiert werden sollen
    -   Sortierrichtung: absteigend oder aufsteigend
    -   Spalten hinzufügen: Welche Felder, z.B. aus einer Vereinbarung sollen pro Treffer im Widget angezeigt werden, z.B. der Name der Vereinbarung, der Status, sowie das Enddatum. Die Anzeige würde dann so aussehen:
        [![Widgets4.png](https://intranet.b.tu-harburg.de/mediawiki/images/b/b8/Widgets4.png)](https://intranet.b.tu-harburg.de/mediawiki/index.php/Datei:Widgets4.png)
8.  Auf "Speichern & schließen" klicken. Das Widget wurde nun erstellt.

## Widget anlegen, das eine Suche beinhaltet

-   Im Akkordeon "Suche" während der Erstellung eines Widgets kann ein Suchbegriff eingegeben werden
-   Es kann nach dem Namen der Vereinbarung, nach dem Alternativen Namen und nach der Beschreibung gesucht werden
-   z.B. alle Titel mit Springer im Namen:

[![Widgets5.png](https://intranet.b.tu-harburg.de/mediawiki/images/thumb/8/8e/Widgets5.png/1005px-Widgets5.png)](https://intranet.b.tu-harburg.de/mediawiki/index.php/Datei:Widgets5.png)

-   Das Suchergebnis wird dann nach dem Speichern im Widget selbst angezeigt

## Widgets bearbeiten oder Löschen

Jedes Widget lässt sich bearbeiten und löschen. Dazu klickt man auf die 3 Punkte oben rechts im Widget. Es öffnet sich ein Auswahl-Menü mit den Funktionen "bearbeiten" und "löschen"

## Ein Widget aktualisieren

Widgets werden automatisch regelmäßig aktualisiert. Man kann sie aber auch manuell aktualisieren, in dem man im Widget unten links auf den runden Pfeil klickt

## Besonderheiten

-   Bei der Filterung nach Tags muss man den genauen Namen des Tags wissen und diesen manuell im Feld "Wert" eingeben
-   Möchte man nach einer bestimmten Verlängerungspriorität filtern, muss man den entsprechenden Wert zum Label kennen. Diesen erhält man nur über die Einstellungen der eManagement-App. Dort wählt man "Auswahllistenwerte" aus und die Auswahlliste "SubscriptionAgreement.RenewalPriority". Dort bekommt man die entsprechenden Werte angezeigt.
-   [a](https://info.gbv.de/label/FOLIOGBVEXTERN/app-dashboard)
