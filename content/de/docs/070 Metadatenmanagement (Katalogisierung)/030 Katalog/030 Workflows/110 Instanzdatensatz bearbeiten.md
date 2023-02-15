---
title: "Instanzdatensatz bearbeiten"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [app-katalog, by-folio, cat-workflows, for-anwender]
weight: 110
Description: "
    Quellen: [Folio](https://docs.folio.org/docs/metadata/inventory/#editing-an-instance-record) <!-- & [GBV](https://info.gebev.de/display/FOLIOGBVEXTERN/Folio:+Instanzdatensatz+bearbeiten) -->
    "
---

## Instanzdatensatz bearbeiten

1.  [Die Instanz suchen]({{< ref "090 Datensatz suchen im Katalog" >}}), die bearbeitet werden soll und sie auswählen.
2.  In der Ansicht **Details des Instanzdatensatzes** auf **Aktionen > Bearbeiten** klicken.
3.  Die gewünschten Änderungen an dem Instanzdatensatz vornehmen.
4.  Auf **Speichern und schließen** klicken. Der Instanzdatensatz wird aktualisiert.

## Bearbeiten eines Instanzdatensatzes mit zugrunde liegendem MARC

Siehe Bearbeiten eines MARC-Eintrags mit quickMARC.

## Aktualisieren eines Instanzdatensatzes mit zugrunde liegendem MARC unter Verwendung der Aktion Überlagern des bibliografischen Quellendatensatzes in FOLIO

1.  [Die Instanz suchen]({{< ref "090 Datensatz suchen im Katalog" >}}), die bearbeitet werden soll und sie auswählen.
2.  In der Ansicht **Details des Instanzdatensatzes** auf **Aktionen > Quellbibliographischen Datensatz überlagern** klicken.
3.  Im Dialogfeld **Einzeldatensatz-Import** die Quelle des zu importierenden Datensatzes (z.B. Library of Congress, OCLC WorldCat, BnF) wählen.
4.  Die Datensatznummer ohne Präfixe in das Feld **\[Quellenidentifikator\] eingeben** eingeben.
5.  Auf **Importieren** klicken.

Der ausgewählte Instanzdatensatz und alle zugrunde liegenden Quelldaten werden durch den neu importierten Datensatz ersetzt. Die UUID und HRID der Instanz sowie die manuell konfigurierbaren Administrative Daten wie Nachweis unterdrückt, Status der Instanz, Katalogisierungsdatum und zugewiesene statistische Codes bleiben unverändert. Einige Konfigurationen können lokal an dem für den Einzeldatensatz-Import verwendeten Importprofil vorgenommen werden. Diese Änderungen werden in den Einstellungen für den Datenimport vorgenommen.
