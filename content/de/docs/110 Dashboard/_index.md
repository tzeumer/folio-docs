---
title: "📱Dashboard"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [app-dashboard, by-folio, cat-berechtigungen, for-anwender]
weight: 110
Description: "
    Quellen: [Folio](https://docs.folio.org/docs/dashboard/) & [GBV](https://info.gbv.de/pages/viewpage.action?pageId=839188640)
    "
---

Die Dashboard-App wurde entwickelt, um eine personalisierte Ansicht der wichtigsten Informationen aus allen FOLIO-Apps auf einen Blick zu ermöglichen. In der ersten Version (die in der Juniper Flower-Version enthalten ist) bietet das Dashboard die Möglichkeit, Informationen aus den Apps [📱eManagement](https://info.gbv.de/pages/viewpage.action?pageId=839188710) und [📱Lizenzverträge (geplant)](https://info.gbv.de/pages/viewpage.action?pageId=839188719) anzuzeigen.

Informationen für Entwickler, die die Dashboard-Funktionalität für ihre eigenen Apps nutzen möchten, sind auf der FOLIO-Wiki-Seite [Dashboard-Dokumentation](https://wiki.folio.org/display/ERM/Dashboard+Documentation) verfügbar.

Definition von Begriffen im Zusammenhang mit der App Dashboard:

* **Dashboard**. Ein Dashboard ist ein Bildschirm, der Widgets anzeigen kann. Eine Person kann innerhalb der App Dashboard Zugriff auf ein oder mehrere Dashboards haben. Ein Dashboard verfügt über eine Reihe von konfigurierten Widgets und auch über eine Zugriffsliste für Personen.
* **Widget**. Um Informationen auf einem Dashboard anzuzeigen, müssen Widgets hinzugefügt werden. Widgets können Informationen aus FOLIO-Anwendungen oder anderen Quellen abrufen und anzeigen. Es gibt verschiedene Arten von Widgets, die je nach Art der Informationen, die angezeigt werden sollen, verwendet werden.

Widgets sind oft von der Person konfigurierbar, so dass dieselbe Art von Widget mehrfach hinzugefügt werden kann, aber mit einer anderen Konfiguration, um eine andere Art von Informationen anzuzeigen. Personen können entscheiden, welche Widgets auf ihrem Dashboard angezeigt werden und in welcher Reihenfolge sie angezeigt werden. Jeder Person steht ein eigenes Dashboard zur Verfügung, so dass jede Person die Widgets, die sie benötigt, in einer für sie geeigneten Weise konfigurieren kann.

* **Personenzugriffsliste**. Auf Dashboards kann von einer oder mehreren Personen zugegriffen werden. Welche Personen auf ein Dashboard zugreifen können, wird über die Personenzugriffsliste für das Dashboard gesteuert. Nur Personen auf dieser Liste können auf das Dashboard zugreifen. Personen können der Personenzugriffsliste hinzugefügt oder von ihr entfernt werden. In der Personenzugriffsliste gibt es drei Zugangsebene, die einer Person gewährt werden können: Anzeigen, Bearbeiten, Verwalten.

Berechtigungen

Es gibt zwei Ebenen der Berechtigungskontrolle für Dashboards. Erstens die Berechtigungen für die App Dashboard, die festlegen, auf welche Funktionen die Personen innerhalb der App Dashboard Zugriff haben. Zweitens bestimmt die Zugangsebene der Person auf jedes Dashboard, die durch die Benutzerzugriffsliste des Dashboards gewährt wird, was die Person in Bezug auf ein bestimmtes Dashboard tun kann.

## Dashboard App Berechtigungen

Die unten aufgeführten Berechtigungen ermöglichen die Interaktion mit der App Dashboard und legen fest, was innerhalb der App getan werden kann und was nicht. Personen können in der App Personen Berechtigungen zugewiesen werden. Wenn einer Person keine dieser Berechtigungen zugewiesen ist, kann sie die App Dashboard und alle damit verbundenen Informationen nicht sehen.

Im Folgenden sind die Dashboard-Berechtigungen aufgelistet:

* **Dashboard: Dashboard verwalten**. (Dashboard: Manage dashboard)
    Dies beinhaltet die Berechtigung, die App Dashboard im FOLIO Interface zu sehen und darauf zuzugreifen, und ermöglicht der Person:  Dashboards zu erstellen, bearbeiten und löschen**.** Widgets auf Dashboards hinzufügen, bearbeiten, entfernen und neu anordnen.Personen zur Benutzerzugriffsliste für ein Dashboard hinzufügen und aus dieser entfernen. Aktualisieren der Zugangsebene für eine Person in der Benutzerzugriffsliste für ein Dashboard.
* **Dashboard: Dashboard-Administrator**. (Dashboard: Dashboard Administrator)
    Mit dieser Berechtigung kann die Person auf alle Dashboards im System zugreifen und Änderungen daran vornehmen, als ob sie die Zugangsebene 'Verwalten' für das Dashboard erhalten hätte.

## Dashboard-Zugangsebene

Die Zugangsebene bestimmen, welche Aktionen eine Person in Bezug auf ein bestimmtes Dashboard durchführen kann.

Wenn die Person keine Zugangsebene für ein Dashboard hat, kann sie nicht auf dieses Dashboard zugreifen (es sei denn, sie hat die Anwendungsberechtigung "Dashboard: Dashboard-Administrator.").

Anmerkung: Um auf Dashboards zugreifen zu können, muss die Person über die Anwendungsberechtigung "Dashboard: Dashboard verwalten" sowie eine Zugangsebene für das Dashboard erhalten haben.

Im Folgenden sind die Personen aufgeführt, die auf ein Dashboard zugreifen können:

* **Anzeigen**. Damit kann die Person das Dashboard, einschließlich der Widgets auf dem Dashboard und der Benutzerzugriffsliste für das Dashboard, anzeigen, aber keine Änderungen am Namen oder der Beschreibung des Dashboards, den Widgets auf dem Dashboard oder der Benutzerzugriffsliste für das Dashboard vornehmen.
* **Bearbeiten**. Damit erhält die Person dieselben Rechte zur Anzeige des Dashboards wie bei der Zugangsebene Anzeigen und kann zusätzlich den Namen und die Beschreibung des Dashboards bearbeiten sowie Widgets auf dem Dashboard hinzufügen, entfernen oder bearbeiten. Die Person kann jedoch keine Änderungen an der Benutzerzugriffsliste für das Dashboard vornehmen.
* **Verwalten**. Ermöglicht dem Benutzer dieselben Ansichts- und Bearbeitungsrechte wie die Zugangsebene Bearbeiten und erlaubt der Person zusätzlich, Personenzugriffsliste für das Dashboard hinzuzufügen, zu entfernen und zu bearbeiten sowie das Dashboard zu löschen.
