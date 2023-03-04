---
title: "Library Data Platform"
linkTitle: ""
date: 2023-03-04T00:00:00-00:00
tags: [app-ldp, by-folio, for-admin, topic-datenschutz]
weight: 10
Description: "
    Quellen: [Folio](https://docs.folio.org/docs/reporting/library-data-platform/) <!-- & [GBV](https://info.gebev.de/display/FOLIOGBVEXTERN/Library+Data+Platform) -->
    "
---

{{% pageinfo %}}
**Anmerkung: Diese Präsentation  vom WOLFcon 2021 gibt einen Überblick über die Library Data Platform.**
{{% /pageinfo %}}

Damit die LDP-Software eine Verbindung zu FOLIO herstellen kann, benötigt sie Lesezugriff auf Okapi und die FOLIO-Datenbank. Die LDP kann lokal von den eigenen Mitarbeitenden einer Institution gehostet und verwaltet werden oder durch die Vergabe von Hosting-Diensten an einen Drittanbieter. Die spezifischen Systemanforderungen sind in der LDP-Dokumentation zu finden.

## Installieren und Konfigurieren der LDP

FOLIO Reporting - Komponentenmatrix

|Folio Release|LDP version|ldpmarc|FOLIO Analytics*|
|:----|:----|:----|:----|
|Nolana|1.8.0 or later|v1.5.0 or later|v1.5.0|
|Morning Glory|1.8.0 or later|v1.5.0 or later|v1.4.0|
|Lotus|1.8.0 or later|v1.5.0 or later|v1.3.0|
|Kiwi|1.8.0 or later|v1.5.0 or later|v1.2.0|
|Juniper|1.8.0 or later|v1.5.0 or later|v1.2.0|
|Iris|1.8.0 or later|v1.5.0 or later|v1.1.1|
|Honeysuckle|1.8.0 or later|-|v1.0|


\* Die FOLIO Analytics Version ist an eine bestimmte Version gebunden. Die neueste Version ist im [Releases](https://github.com/folio-org/folio-analytics#releases) Bereich des folio-analytics Repository zu finden.

Ausführliche Informationen zur Einrichtung und Konfiguration der LDP sind in den unten verlinkten Anleitungen zu finden, die im LDP-Repository verfügbar sind. Dort sind auch die neuesten Versionen und Korrekturen der LDP zu finden.

### Leitfaden zur Administrations

* [Overview](https://github.com/library-data-platform/ldp/blob/1.8.2/doc/Admin_Guide.md#1-overview): kurze Einführung und Zusammenfassung
* [System requirements](https://github.com/library-data-platform/ldp/blob/1.8.2/doc/Admin_Guide.md#2-system-requirements): Software- und Hardwarevoraussetzungen
* [Installation](https://github.com/library-data-platform/ldp/blob/1.8.2/doc/Admin_Guide.md#3-installation): Installation der Voraussetzungen und Aufbau von LDP
* [Database configuration](https://github.com/library-data-platform/ldp/blob/1.8.2/doc/Admin_Guide.md#4-database-configuration): Einrichten und Konfigurieren der Datenbank
* [Server configuration](https://github.com/library-data-platform/ldp/blob/1.8.2/doc/Admin_Guide.md#5-ldp-configuration): Einrichten, Konfigurieren, Starten und Aktualisieren des LDP
* [Data privacy](https://github.com/library-data-platform/ldp/blob/1.8.2/doc/Admin_Guide.md#6-data-privacy): Optionen zur Anonymisierung persönlicher Daten (Datenschutz)
* [Optional columns](https://github.com/library-data-platform/ldp/blob/1.8.2/doc/Admin_Guide.md#7-optional-columns): Festlegen optionaler FOLIO-Spalten, die immer in LDP-Tabellen erscheinen sollen
* [Historical data](https://github.com/library-data-platform/ldp/blob/1.8.2/doc/Admin_Guide.md#8-historical-data): Beschreibung der Funktion Historische Daten und Anleitung zur Deaktivierung
* [User accounts](https://github.com/library-data-platform/ldp/blob/1.8.2/doc/Admin_Guide.md#9-user-accounts): Einrichtung von Benutzerkonten und Aktivierung von LDP zum Setzen von Berechtigungen
* [Reference](https://github.com/library-data-platform/ldp/blob/1.8.2/doc/Admin_Guide.md#reference): Referenz für die Konfigurationsdatei: ldpconf.json

## Abgeleitete Tabellen einrichten

Damit Personen die von der Community entwickelten [Berichtsabfragen]({{< ref "030 FOLIO Analytics" >}}) in vollem Umfang nutzen können und einen guten Ausgangspunkt für [Ad-hoc-Abfragen]({{< ref "030 FOLIO Analytics" >}}) haben, wird dringend empfohlen, eine nächtliche Aktualisierung der [abgeleiteten Tabellen](https://github.com/folio-org/folio-analytics/tree/release-1.5/sql/derived_tables) einzurichten. Bitte beachten, dass die Verwendung von Views und materialisierten Views in LDP-Datenbanken nicht unterstützt wird und dazu führen kann, dass die LDP-Software keine Datenaktualisierungen durchführen kann.

Eine Anleitung zur Einrichtung von [FOLIO Reporting Derived Tables](https://github.com/folio-org/folio-analytics/blob/release-1.5/sql/derived_tables/README.md) ist auf Github zu finden.

## Datenschutz

Die LDP ist so konzipiert, dass sie GDPR und andere Datenschutzanforderungen unterstützt. Administratoren können eine vordefinierte Gruppe von Tabellen ausschließen.

Im [Anonymisierungsleitfaden](https://github.com/library-data-platform/ldp/blob/1.8.2/doc/Admin_Guide.md#7-data-privacy) sind Informationen zur Aktivierung und Konfiguration dieser Funktionen zu finden.

Auf den unten verlinkten Seiten sind Attribute aufgeführt, die potenziell personenbezogene Daten enthalten:

* [User module](https://wiki.folio.org/display/RPT/Potential+personal+data%3A+List+of+FOLIO+attributes?src=contextnavpagetreemode): Tabellen, die nicht in LDP geladen werden, wenn die Anonymisierung aktiviert ist
* [Organizations module](https://wiki.folio.org/display/RPT/Potential+personal+data+in+mod-organizations-storage?src=contextnavpagetreemode): Potenzielle personenbezogene Daten im Modul Organisationen

## Lokalen Daten hinzufügen

Wie im [Benutzerleitfaden](https://github.com/library-data-platform/ldp/blob/1.8.2/doc/User_Guide.md#4-local-tables) beschrieben, ist es auch möglich, lokale Daten in die LDP zu laden und zu erstellen. Neben der Verwendung des lokalen Schemas können auch separate Schemas für verschiedene Personengruppen oder Zwecke eingerichtet werden.

### Verwendung von Schemata

Das Konzept der Schemata ermöglicht es, Tabellen und Berechtigungen innerhalb einer Datenbank zu organisieren. In LDP gibt es zunächst vier relevante Schemata:

* public: enthält alle extrahierten Tabellen und ihre aktuellen Daten aus dem angebundenen FOLIO-Mandanten
* [history](https://github.com/library-data-platform/ldp/blob/1.8.2/doc/User_Guide.md#5-historical-data): speichert Daten, die in der Vergangenheit aktualisiert wurden oder möglicherweise nicht mehr existieren
* [folio\_reporting](https://github.com/folio-org/folio-analytics/blob/release-1.5/sql/derived_tables/README.md): enthält alle [abgeleiteten Tabellen](https://github.com/folio-org/folio-analytics/tree/release-1.5/sql/derived_tables), die von der Community erstellt und unterstützt werden
* [local](https://github.com/library-data-platform/ldp/blob/1.8.2/doc/User_Guide.md#4-local-tables): gemeinsamer Bereich für Personen, die Berichte erstellen oder eigene Daten importieren

Neben den bestehenden Schemas können weitere Schemas für lokale Bedürfnisse erstellt werden (z.B. um Daten für verschiedene Fachbereiche bereitzustellen oder um sensible Daten zu trennen und zu schützen).

Mehr über das Schemakonzept und die Konfiguration von Schemas ist in der [Postgres’s Schema Documentation](https://www.postgresql.org/docs/13/ddl-schemas.html#DDL-SCHEMAS-PRIV) zu lesen.

Für eine granulare Einrichtung von Berechtigungen auch die integrierten [Rollen](https://www.postgresql.org/docs/13/user-manag.html)\- und [Privilegien](https://www.postgresql.org/docs/13/ddl-priv.html)\-Konzepte von Postgres beachten.

### Verschieben und Laden von Daten

Das Laden und Verschieben von Daten in LDP ist genauso einfach wie bei Datenbanken im Allgemeinen.

Für Postgres gibt es zwei gängige Ansätze:

* [COPY](https://www.postgresql.org/docs/13/sql-copy.html): SQL-Befehl zum Verschieben von Tabellendaten über csv-Dateien
* [pg\_dump](https://www.postgresql.org/docs/13/app-pgdump.html) / [pg\_restore](https://www.postgresql.org/docs/13/app-pgrestore.html): Postgres Kommandozeilen-Tools zum Importieren und Exportieren von Daten

## FOLIO-Datenabdeckung in der LDP

Die LDP nutzt die FOLIO-APIs, um die meisten ihrer Inhalte zu erhalten. Weitere Einzelheiten zu den APIs sind in der FOLIO Developers [API documentation](https://dev.folio.org/reference/api/) zu finden (siehe auch [Schnittstellen (API) (geplant)]({{< ref "060 Schnittstellen (API)" >}})).

Ab [Version 1.8.2](https://github.com/library-data-platform/ldp/tree/1.8.2) bezieht die LDP Daten aus den folgenden FOLIO-Modulen:

* mod-audit
    * /audit-data/circulation/logs
* mod-circulation-storage
    * /cancellation-reason-storage/cancellation-reasons
    * /check-in-storage/check-ins
    * /fixed-due-date-schedule-storage/fixed-due-date-schedules
    * /loan-policy-storage/loan-policies
    * /loan-storage/loans
    * /loan-storage/loan-history
    * /patron-action-session-storage/patron-action-sessions
    * /patron-notice-policy-storage/patron-notice-policies
    * /request-policy-storage/request-policies
    * /request-preference-storage/request-preference
    * /request-storage/requests
    * /scheduled-notice-storage/scheduled-notices
    * /staff-slips-storage/staff-slips
* mod-configuration
    * /configurations/entries
* mod-courses
    * /coursereserves/copyrightstatuses
    * /coursereserves/courselistings
    * /coursereserves/courses
    * /coursereserves/coursetypes
    * /coursereserves/departments
    * /coursereserves/processingstatuses
    * /coursereserves/reserves
    * /coursereserves/roles
    * /coursereserves/terms
* mod-email
    * /email
* mod-feesfines
    * /accounts
    * /comments
    * /feefines
    * /feefineactions
    * /lost-item-fees-policies
    * /manualblocks
    * /overdue-fines-policies
    * /owners
    * /payments
    * /refunds
    * /transfer-criterias
    * /transfers
    * /waives
* mod-finance-storage
    * /finance-storage/budgets
    * /finance-storage/expense-classes
    * /finance-storage/fiscal-years
    * /finance-storage/fund-types
    * /finance-storage/funds
    * /finance-storage/group-fund-fiscal-years
    * /finance-storage/groups
    * /finance-storage/ledgers
    * /finance-storage/transactions
* mod-inventory-storage
    * /alternative-title-types
    * /call-number-types
    * /classification-types
    * /contributor-name-types
    * /contributor-types
    * /electronic-access-relationships
    * /holdings-note-types
    * /holdings-storage/holdings\*
    * /holdings-types
    * /identifier-types
    * /ill-policies
    * /instance-formats
    * /instance-note-types
    * /instance-relationship-types
    * /instance-statuses
    * /instance-storage/instance-relationships
    * /instance-storage/instances\*
    * /instance-types
    * /item-damaged-statuses
    * /item-note-types
    * /item-storage/items\*
    * /location-units/campuses
    * /location-units/institutions
    * /location-units/libraries
    * /loan-types
    * /locations
    * /material-types
    * /modes-of-issuance
    * /nature-of-content-terms
    * /service-points
    * /service-points-users
    * /statistical-code-types
    * /statistical-codes
* mod-invoice-storage
    * /invoice-storage/invoice-lines
    * /invoice-storage/invoices
    * /voucher-storage/voucher-lines
    * /voucher-storage/vouchers
* mod-notes
    * /notes
* mod-orders-storage
    * /acquisitions-units-storage/memberships
    * /acquisitions-units-storage/units
    * /orders-storage/alerts
    * /orders-storage/order-invoice-relns
    * /orders-storage/order-templates
    * /orders-storage/pieces
    * /orders-storage/po-lines
    * /orders-storage/purchase-orders
    * /orders-storage/receiving-history
    * /orders-storage/reporting-codes
* mod-organizations-storage
    * /organizations-storage/addresses
    * /organizations-storage/categories
    * /organizations-storage/contacts
    * /organizations-storage/emails
    * /organizations-storage/interfaces
    * /organizations-storage/organizations
    * /organizations-storage/phone-numbers
    * /organizations-storage/urls
* mod-source-record-storage
    * srs::marc\_records\_lb\*
    * srs::records\_lb\*
* mod-users
    * /addresstypes
    * /departments
    * /groups
    * /proxiesfor
    * /users
