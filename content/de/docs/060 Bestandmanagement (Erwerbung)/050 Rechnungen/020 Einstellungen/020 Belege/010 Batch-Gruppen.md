---
title: "Batch-Gruppen"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [app-rechnungen, by-folio, cat-einstellungen, for-admin]
weight: 10
Description: "
    Quellen: [Folio](https://docs.folio.org/docs/settings/settings_invoices/settings_invoices/#settings--invoices--batch-groups) & [GBV](https://info.gbv.de/display/FOLIOGBVEXTERN/Einstellungen+(Rechnungen):+Batch-Gruppen)
    "
---

## Einstellungen > Rechnungen > Batch-Gruppen

Diese Einstellung wird verwendet, um Batch-Gruppen zu erstellen, zu bearbeiten und zu löschen. Batch-Gruppen dienen dazu, Rechnungen für den Export als Belege in ein externes Zahlungssystem zu organisieren.

### Batch-Gruppe erstellen

1.  Auf **Neu** klicken.
2.  Einen **Namen** in das Feld eingeben.
3.  Optional: Eine **Beschreibung** in das Feld eingeben.
4.  Auf **Speichern** klicken. Die Batch-Gruppe wird gespeichert.

### Batch-Gruppe bearbeiten

1.  Die Batch-Gruppe suchen, die bearbeitet werden soll und auf das **Bleistiftsymbol** klicken.
2.  Die **Batch-Gruppe** bearbeiten.
3.  Auf **Speichern** klicken.

### Batch-Gruppe löschen

1.  Die Batch-Gruppe suchen, die bearbeitet werden soll und auf das **Mülleimersymbol** klicken.
2.  In der Dialogbox **Batch-Gruppe löschen** auf **Löschen** klicken. Es erscheint eine Bestätigungsmeldung und die Batch-Gruppe wird gelöscht.

## Einstellungen > Rechnungen > Batch-Gruppe konfigurieren

Diese Einstellung wird verwendet, um die Exporte von Belegen der Batch-Gruppe zu konfigurieren. Mit dieser Konfiguration können automatische Exporte von Dateien eingerichtet werden, die alle Rechnungsbelege enthalten, die seit dem letzten Export erstellt wurden. Weitere Informationen darüber, wie Belege erstellt werden, finden sind unter [Rechnungen > Freigeben einer Rechnung]({{< ref "090 Rechnung freigeben" >}}) zu finden. Alle Belege, bei denen die Checkbox An Haushaltssystem exportieren aktiviert ist und die seit dem letzten Export für die Batch-Gruppe erstellt wurden, werden in eine Datei exportiert. Weitere Informationen über das Kontrollkästchen An Haushaltssystem exportieren sind unter [Rechnungen > Erweiterte Informationen]({{< ref "010 Rechnung erstellen" >}}) zu finden. Jede Rechnung erzeugt einen einzigen Beleg, auf dem alle Fondsgebühren nach der externen Kontonummer des Fonds gruppiert sind.

### Konfigurieren einer Batch-Gruppe

1.  Eine **Batch-Gruppe** wählen.
2.  Einen **Export planen**. Wird **Täglich** gewählt, dann eine Uhrzeit eingeben. Wird **Wöchentlich** gewählt, dann die Tage und die Uhrzeit auswählen, an denen der Export automatisch ausgeführt werden soll.
3.  Einen **Upload-Speicherort** eingeben. Wenn dieses Feld leergelassen wird, lädt der Export die Datei auf den lokalen Computer herunter.
4.  Ein **Format** wählen: JSON oder XML.
5.  Bei Bedarf eine **Kennung** für den Standort eingeben, an dem die Datei hochgeladen werden soll.
6.  Ein **Passwort** eingeben, falls dies für den Upload-Speicherort erforderlich ist.
7.  Auf **Speichern** klicken.

Auf **Anmeldedaten anzeigen**/**Anmeldedaten ausblenden** klicken, um das Passwort ein- oder auszublenden. Wenn die Verbindung mit dem den Upload-Standort getestet werden soll, auf **Verbindung testen**
