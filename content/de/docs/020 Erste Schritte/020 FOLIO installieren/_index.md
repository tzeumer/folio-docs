---
title: "FOLIO installieren"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [by-folio, for-entwickler]
weight: 10
Description: "
    Quellen: [Folio](https://docs.folio.org/docs/getting-started/installation/)
    "
---

## Arten von Installationen und Bereitstellungen

FOLIO kann auf verschiedene Arten installieren und eingesetzt werden:

* Vorgefertigte Vagrant-Boxen
* Bereitstellung auf einem einzelnen Server
* Kubernetes-Bereitstellung

### Vorgefertigte Vagrant-Boxen

Wenn FOLIO nur ausprobiert werden soll, ohne es zu installieren, kann eine der vorgefertigten Vagrant-Boxen verwendet werden. Es dauert nur ein paar Minuten, um eine virtuelle Maschine mit einer FOLIO-Instanz und Beispieldaten herunterzuladen, auszuführen und sie sofort zu verwenden.

Siehe [Vagrant]({{< ref "040 Vagrant" >}}) für weitere Informationen.

### Server (Standalone)

FOLIO kann lokal gehostet und betrieben werden. In diesem Szenario wird die Installation von FOLIO selbst verwaltet und erfolgt auf einem einzelnen Server ohne die Verwendung von Software-Orchestrationslösungen wie Kubernetes. Diese Konfiguration empfiehlt sich, wenn es nur einen einzigen Mandanten gibt oder die Anzahl der Mandanten und Ressourcen, die die FOLIO-Instanz verwalten wird, im Voraus abgeschätzt werden kann; andernfalls sollte eine Kubernetes-Bereitstellung in Betracht gezogen werden.

Eines der Ziele von FOLIO ist die Erweiterbarkeit. Bibliotheken und Lieferanten können auf bestehenden Apps aufbauen oder neue Apps entwickeln, die die Bibliothek in Bereiche wie Campus-ERP, Forschungsdatenverwaltung und mehr erweitern. Zusätzlich zu dem softwarecode und Testtools wird ein Entwickler wahrscheinlich das gesamte FOLIO-System kennenlernen wollen und benötigt dazu eine lokale Instanz. In der Regel handelt es sich dabei um eine virtuelle Maschine mit einer Single-Server-Installation von FOLIO.

Siehe [Server mit Containern]({{< ref "020 Server mit Containern" >}}) für weitere Informationen.

### Kubernetes

Die in FOLIO integrierten Multi-Mandanten-Fähigkeiten erlaubt einfache Skalierbarkeit und damit die Effizienz von Bibliotheken zu verbessern. In diesem Szenario wird FOLIO auf einem Server-Cluster eingesetzt, der Kubernetes für die Orchestrierung verwendet. Diese Konfiguration ermöglicht das Hinzufügen neuer Mandanten und Hardwareressourcen nach Bedarf und ist ideal, wenn die FOLIO-Instanz in Zukunft skalierbar sein muss.

Siehe [Kubernetes-Beispiel]({{< ref "030 Kubernetes-Beispiel" >}}) für weitere Informationen.

## Voraussetzungen

### Speicher

Es werden mindestens 24 GB Arbeitsspeicher benötigt, um das offiziellen "platform-complete"-Paket von FOLIO-Modulen zu betreiben.

### PostgreSQL

FOLIO benötigt PostgreSQL 12 oder eine neuere Version.

`pg_hba.conf` muss für die md5-Passwortauthentifizierung konfiguriert sein. Einige PostgreSQL-Distributionen verwenden standardmäßig die `scram-sha-256`\-Passwortauthentifizierung, wodurch die FOLIO-Installation mit dieser Fehlermeldung fehlschlägt:

```
Opening SQLConnection failed: com/ongres/scram/common/stringprep/StringPreparation
java.lang.NoClassDefFoundError: com/ongres/scram/common/stringprep/StringPreparation
```
