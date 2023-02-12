---
title: "Exportmanager Aufträge suchen und filtern"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [app-exportmanager, by-folio, cat-workflows, for-anwender, meta-uebersetzungsproblem]
weight: 20
Description: "
    Quellen: [Folio](https://docs.folio.org/docs/export-manager/#searching-and-filtering-jobs) & [GBV](https://info.gbv.de/pages/viewpage.action?pageId=845709339)
    "
---

{{% pageinfo %}}
Fehlende offizielle Übersetzungen. ("Bursar", "Zahlmeister")
{{% /pageinfo %}}

In der Ansicht **Suchen & Filtern** kann nach Aufträgen gesucht werden. Um einen Auftrag nach Auftrags-ID zu suchen, die Suchbegriffe in das Feld eingeben.

Nach Protokollen suchen, indem einer der Filter in der Ansicht Suchen & Filtern ausgewählt wird. Außerdem können die Filter nach der Suche angewendet werden, um die Ergebnisse einzuschränken. Weitere Informationen sind in den folgenden Abschnitten zu finden.

## Status

Um nach Status zu filtern, einen Filter wählen:

-   **Geplant**. Dieser Export wurde geplant, aber noch nicht ausgeführt.
-   **In Bearbeitung**. Dieser Export wird gerade ausgeführt.
-   **Erfolgreich**. Dieser Export wurde bis zum Ende ausgeführt.
-   **Fehlgeschlagen**. Dieser Export konnte nicht durchgeführt werden. Auf  die Zeilen mit diesem Status klicken um Fehlerdetails zu erhalten.

## Jobtyp

Um nach Jobtyp zu filtern, einen Filter wählen:

-   **Bursar**. Dieser Export enthält Gebühren und/oder Erstattungen, die an den Zahlmeister überwiesen wurden. Das Ausgabeformat ist .dat.
-   **Ausleihprotokoll**. Dieser Export enthält Suchergebnisse aus dem Ausleihprotokoll. Das Ausgabeformat ist .csv.
-   **eHoldings**. Dieser Export enthält Paket- und Titeldetails aus eHoldings. Das Ausgabeformat ist .csv.
-   **Massenbearbeitung**. Dieser Export enthält heruntergeladene Informationen aus der Massenbearbeitung. Das Ausgabeformat ist .csv.

## System

Um danach zu filtern, ob der Auftrag vom System generiert wurde oder nicht, eine der folgenden Optionen wählen:

-   **Ja**. Der Export wurde automatisch initiiert.
-   **Nein**. Der Export wurde von einer Person manuell ausgelöst.

## Quelle

So wird nach Protokollen basierend auf der Person gesucht, die den Export initiiert hat: In der Ansicht **Suchen & Filtern** auf **Quelle** klicken. Auf **Person finden** klicken. Im Dialogfeld **Person auswählen** nach der Person suchen. Die Person wählen, nach gefiltert werden soll.

## Startzeit

So wird nach Protokollen anhand des Datums gesucht, an dem sie zu laufen begonnen haben:

In der Ansicht **Suchen & Filtern** auf **Startzeit** klicken. Ein Startdatum in das Feld **Von** und ein Enddatum in das Feld **Bis** eingeben. Auf **Anwenden** klicken. Die Suchergebnisse werden in der Ansicht **Exportjob** angezeigt.

## Endzeit

So wird nach Protokollen anhand des Datums gesucht, an dem sie beendet wurden:

In der Ansicht **Suchen & Filtern** auf **Endzeit** klicken. Ein Startdatum in das Feld **Von** und ein Enddatum in das Feld **Bis** eingeben. Auf **Anwenden** klicken. Die Suchergebnisse werden in der Ansicht Exportaufträge angezeigt.

## Exportmethode

Dieser Filter ist nur in der Ansicht Organisationen verfügbar. So wird nach Exporten nach Exportmethode gesucht:

In der Ansicht **Suchen & Filtern** auf **Exportmethode** klicken. Die Exportmethode aus der Dropdown-Liste auswählen.

Die Suchergebnisse werden in der Ansicht **Exportjob** angezeigt.

## Organisationen

Dieser Filter ist nur in der Ansicht Organisationen verfügbar.

So wird nach Exporten gesucht, die mit einer bestimmten Organisation verbunden sind:

In der Ansicht **Suchen & Filtern** auf **Organisation** klicken. Auf **Organisationssuche** klicken. Im Dialogfeld **Organisation wählen** nach der Organisation suchen. Die Organisation wählen, nach der gefiltert werden soll. Die Suchergebnisse werden in der Ansicht **Exportjob** angezeigt.
