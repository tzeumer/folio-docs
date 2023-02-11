---
title: "📱Lokale KB-Verwaltung"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [app-lokale_kb_verwaltung, by-folio, cat-berechtigungen, for-anwender]
weight: 60
Description: "
    Quellen: [Folio](https://docs.folio.org/docs/erm/local-kb-admin/ ) & [GBV](https://info.gbv.de/pages/viewpage.action?pageId=839188721)
    "
---

{{% pageinfo %}}
-   Siehe auch [Knowledge Bases](https://info.gbv.de/display/FOLIOGBVEXTERN/Knowledge+Bases)
{{% /pageinfo %}}

Mit der App Lokale KB-Verwaltung können Daten im KBART- und JSON-Format in die lokale Knowledgebase (KB) von FOLIO importiert und Importjobs aus externen Quellen von E-Ressourcen-Metadaten überwacht werden. Diese können unter [Einstellungen > Lokale KB-Verwaltung > Externe Datenquellen](https://info.gbv.de/display/FOLIOGBVEXTERN/Einstellungen+%28Lokale+KB-Verwaltung%29%3A+Externe+Datenquelle+verbinden) konfiguriert werden. Bei diesen Daten handelt es sich um einzelne E-Ressourcen, die in Paketen organisiert sind. Sie sind nach dem Import in der App eManagement > E-Ressourcen (Registerkarte ) verfügbar und können als Vereinbarungskomponenten mit Vereinbarungen verknüpft werden. Wird die App eHoldings verwendet, die auf die Knowledgebase von EBSCO zurückgreift, ist die Verwendung der Lokalen KB-Verwaltung optional. Die Lokale KB kann ausblendet werden, indem die Checkbox "Interne Vereinbarungs-Knowledgebase unterdrücken" unter [Einstellungen > eManagement > Anzeigeeinstellungen](https://info.gbv.de/display/FOLIOGBVEXTERN/Einstellungen+%28eManagement%29%3A+Anzeigeeinstellungen) aktivieren.

Definition von Begriffen im Zusammenhang mit der App Lokale KB-Verwaltung:

-   **E-Ressource**. Eine elektronische Ressource. Dies bezieht sich im Allgemeinen auf Pakete und Titel.
-   **Anbieter** (Provider). Der Anbieter der E-Ressource, z. B. der Lieferant oder der Verlag.
-   **Paket** (Package). Eine Sammlung von elektronischen Ressourcen, die zu einer Einheit gebündelt sind.
-   **Titel**. Eine einzelne E-Ressource, z.B. ein E-Book, eine E-Zeitschrift oder eine Datenbank, unabhängig davon, in welchem Paket sie enthalten ist.
-   **Paket-Titel**. Ein Titel innerhalb eines Pakets mit einer bestimmten Paket/Plattform-Kombination, z.B. Titel "Handelsprofile" im Paket "WTO iLibrary journals" auf der Plattform "WTO iLibrary".
-   **Knowledgebase (KB)**. Eine Knowledgebase (gelegentlich auch deutsch: Wissensdatenbank) ist eine umfangreiche Datenbank, die von einem Anbieter von Wissensdatenbanken verwaltet wird und Informationen über elektronische Ressourcen wie Titellisten, Abdeckungszeiträume usw. enthält. Knowledgebases gliedern die von einem Contentprovider bereitgestellten Ressourcen in der Regel in Sammlungen oder Datenbanken, die bestimmte Angebote des Contentproviders widerspiegeln, z.B. Pakete von elektronischen Zeitschriften, E-Books oder anderen Materialien.
-   **Lokale Knowledgebase**. Die Verwaltung der Knowledgebase der Bibliothek innerhalb von FOLIO.
-   **Proxy-Server**. Ein Dienst, der Bestandsanfragen für E-Ressourcen durchleitet, so dass eine Person mit minimalen Authentifizierungs-/Autorisierungsproblemen auf die E-Ressource zugreifen kann.
-   **Plattform**. Eine Plattform ist die Infrastruktur eines Anbieters, über die auf eRessourcen zugegriffen werden kann.

## Berechtigungen

Die unten aufgeführten Berechtigungen ermöglichen die Interaktion mit der App Lokale KB-Verwaltung und legt fest, was innerhalb der App getan werden kann und was nicht. Es können Personen in der App Personen Berechtigungen zugewiesen werden. Wenn einer Person keine dieser Berechtigungen zugewiesen ist, kann sie die App Lokale KB-Verwaltung nicht sehen.

Die folgenden Berechtigungen gelten für alle Bibliotheken, die die App Lokale KB-Verwaltung verwenden:

-   **Lokale KB-Verwaltung: Jobs erstellen**. (Local KB admin: Create jobs.)
    Diese Berechtigung erlaubt es der Person, neue Importjobs hinzuzufügen.
-   **Lokale KB-Verwaltung: Jobs löschen**. (Local KB admin: Delete jobs)
    Mit dieser Berechtigung kann die Person bestehende Importjobs löschen.
-   **Lokale KB-Verwaltung: Verwalten der Proxyserverkonfiguration**. (Local KB admin: Manage proxy server configuration)
    Mit dieser Berechtigung kann die Person unter Einstellungen > Lokaler KB-Admin Proxy-Server-Einstellungen erstellen, bearbeiten und löschen.
-   **Lokale KB-Verwaltung: Verwalten der KB-Konfiguration**. (Local KB admin: Manage remote KB configuration)
    Mit dieser Berechtigung kann die Person unter Einstellungen > Lokaler KB-Admin externe Datenquellen erstellen, bearbeiten und löschen.
-   **Lokale KB-Verwaltung: Jobs anzeigen**. (Local KB admin: View jobs)
    Diese Berechtigung ermöglicht es der Person, bestehende Aufträge einzusehen. Außerdem kann die Person die App Lokale KB-Verwaltung im Interface von FOLIO sehen und darauf zugreifen.
