---
title: "📱eManagement"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [app-e_management, by-folio, cat-berechtigungen, for-anwender, meta-uebersetzungsproblem]
weight: 10
Description: "
    Quellen: [Folio](https://docs.folio.org/docs/erm/agreements/ ) & [GBV](https://info.gbv.de/pages/viewpage.action?pageId=839188710)
    "
---

{{% pageinfo %}}
* Berechtigungen sind manchmal noch "Vereinbarungen:" statt "eManagement:"
* Rot:Fehlende offizielle Übersetzungen. ("Agreements: File download.", "eUsage reports: charts may be viewed.")
{{% /pageinfo %}}

Mit der App eManagement (englisch: Agreements) können die Vereinbarungen der Bibliothek erstellt und verwaltet werden. Die Vereinbarungen, die hier erstellt werden, können mit Lizenzen in der App Lizenzverträge verknüpft werden.

Definition von Begriffen im Zusammenhang mit der App eManagement:

1.  **Vereinbarungen**. Eine Vereinbarung ist ein Ort, an dem die Inhalte verwaltet werden können, auf die die Bibliothek zugreifen kann (auf der Grundlage von Ressourcen, die in einer Knowledgebase beschrieben sind), und an dem diese Inhalte mit Lizenzierungs- und Erwerbungsinformationen verknüpft werden können.
2.  **Externe Knowledgebase**. Eine Knowledgebase (siehe Definition in dieser Liste), die sich außerhalb des FOLIO-Systems befindet. Zum Beispiel die GOKb oder die EBSCO Knowledgebase.
3.  **Lokale Knowledgebase**. Die Verwaltung der Knowledgebase der Bibliothek innerhalb von FOLIO.
4.  **Knowledgebase (KB)**. Eine Knowledgebase (gelegentlich auch deutsch: Wissensdatenbank) ist eine umfangreiche Datenbank, die von einem Anbieter von Wissensdatenbanken verwaltet wird und Informationen über elektronische Ressourcen wie Titellisten, Abdeckungszeiträume usw. enthält. Knowledgebases gliedern die von einem Contentprovider bereitgestellten Ressourcen in der Regel in Sammlungen oder Datenbanken, die bestimmte Angebote des Contentproviders widerspiegeln, z.B. Pakete von elektronischen Zeitschriften, E-Books oder anderen Materialien.
5.  **Lizenz**. Eine Lizenz erklärt, was mit den Inhalten, auf die die Bibliothek zugreifen kann, getan werden darf. Der Vertrag oder die Nutzungsbestimmungen bilden die Lizenz.

Bibliotheken, die FOLIO nutzen, können eine externe Knowledgebase wie die GOKb oder EBSCO verwenden oder die lokale Knowledgebase von FOLIO nutzen. Anmerkung: Je nachdem, ob die Bibliothek eine externe oder lokale Knowledgebase nutzt, unterscheiden sich einige Anleitungen.

## Berechtigungen

Die unten aufgeführten Berechtigungen ermöglichen die Interaktion mit der App eManagement und legen fest, was innerhalb der App getan werden kann und was nicht. Es können Personen in der App Personen Berechtigungen zugwiesen werden. Wenn einer Person keine dieser Berechtigungen zugewiesen ist, kann sie die App Vereinbarungen und alle damit verbundenen Informationen nicht sehen.

Die folgenden Berechtigungen gelten für alle Bibliotheken, die die App Vereinbarungen verwenden:

* **eManagement: Vereinbarungen suchen und anzeigen**. (Agreements: Search & view agreements)
    Mit dieser Berechtigung kann die Person bestehende Vereinbarungen suchen und anzeigen. Außerdem kann die Person die App für eManagement im FOLIO Interface sehen und darauf zugreifen.
* **Vereinbarungen: Vereinbarungen bearbeiten**. (Agreements: Edit agreements)
    Diese Berechtigung erlaubt der Person, Vereinbarungen zu bearbeiten, einschließlich der Möglichkeit, Vertragszeilen hinzuzufügen und zu bearbeiten, Dokumente hinzuzufügen und zu bearbeiten und Tags zu einer Vereinbarung anzuzeigen, hinzuzufügen und zu bearbeiten. Sie gewährt außerdem alle Berechtigungen, die unter "eManagement: Vereinbarungen suchen & anzeigen" enthalten sind.
* **Vereinbarungen: Vereinbarungen löschen**. (Agreements: Delete agreements)
    Diese Berechtigung erlaubt es der Person, Vereinbarungen zu löschen. (Dies beinhaltet nicht die Möglichkeit, Vereinbarungen zu bearbeiten, sondern nur, sie zu löschen.) Es gewährt außerdem alle Berechtigungen, die unter "eManagement: Vereinbarungen suchen und anzeigen" enthalten sind.
* **Agreements: File download**. (Agreements: File download)
    (ui-agreements.agreements.file.download) Diese Berechtigung gewährt die Berechtigung zum Herunterladen von Dokumenten, unabhängig vom Hochladen von Dokumenten.

Die folgenden Berechtigungen sind nur anwendbar, wenn Ihre Bibliothek die Lokale KB verwendet:

* **eManagement: E-Ressourcen suchen und anzeigen**. (Agreements: Search & view e-resources)
    Mit dieser Berechtigung kann die Person eRessourcen (Pakete und Titel in diesen Paketen) in der internen KB suchen und anzeigen. Dies beinhaltet die Berechtigung, die App Vereinbarungen im FOLIO Interface zu sehen und darauf zuzugreifen.
* **Vereinbarungen: E-Ressourcen bearbeiten**. (Agreements: Edit e-resources)
    Diese Berechtigung erlaubt es der Person, die eRessourcen zu bearbeiten. Sie gewährt auch alle Rechte, die in "eManagement: E-Ressourcen suchen und anzeigen" enthalten sind.
* **eManagement: Plattformen suchen und anzeigen**. (Agreements: Search & view platforms)
    Diese Berechtigung ermöglicht es der Person, Plattformen in der internen KB zu suchen und anzuzeigen. Dazu gehört auch die Berechtigung, die App für Vereinbarungen im FOLIO Interface zu sehen und darauf zuzugreifen.
* **eManagement: Plattformen bearbeiten**. (Agreements: Edit platforms)
    Diese Berechtigung ermöglicht es der Person, die Eigenschaften von Plattformen zu bearbeiten. Es gewährt auch alle Rechte, die in "eManagement: E-Ressourcen suchen und anzeigen" enthalten sind.

Wenn Daten in einem Vereinbarungsdatensatz eUsagen verwendet werden sollen, werden außerdem die folgende eUsage-Berechtigung benötigt:

* **eUsage reports: charts may be viewed**. (eUsage reports: charts may be viewed)
    Diese Berechtigung fügt dem Datensatz einer Vereinbarung in der App "Vereinbarungen" ein Akkordeon hinzu, das Diagramme und Grafiken zu eUsage-Daten für die mit einer Vereinbarung verbundenen Titel anzeigt.

Fehlte in der Originaldoku noch, sind aber beim FOLIO-System zu finden; evtl. weggefallen

* Einstellungen (eManagement): Auswahllisten und Werte verwalten
* Einstellungen (eManagement): Ergänzende Vereinbarungseigenschaften verwalten
* Einstellungen (eManagement): Kann allgemeine Einstellungen anzeigen und bearbeiten
* eManagement Plugin: Vereinbarungen suchen
