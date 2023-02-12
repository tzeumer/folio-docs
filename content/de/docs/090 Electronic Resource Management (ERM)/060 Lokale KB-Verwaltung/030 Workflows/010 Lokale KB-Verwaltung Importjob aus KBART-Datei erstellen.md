---
title: "Lokale KB-Verwaltung Importjob aus KBART-Datei erstellen"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [app-lokale_kb_verwaltung, by-folio, cat-workflows, for-anwender]
weight: 10
Description: "
    Quellen: [Folio](https://docs.folio.org/docs/erm/local-kb-admin/#creating-a-kbart-import-job) & [GBV](https://info.gbv.de/display/FOLIOGBVEXTERN/Folio:+Lokale+KB-Verwaltung+Importjob+aus+KBART-Datei+erstellen)
    "
---

1.  In der **Lokalen KB-Verwaltung** auf **Aktionen > KBART-Importjob** klicken
2.  Im Fenster Neuer KBART-Job die Pflichtfelder ausfüllen. Weitere Informationen zu den Feldern sind in den Abschnittsbeschreibungen unten zu finden.
3.  Die KBART-Datei **in den Upload-Bereich ziehen** oder auf die Schaltfläche "**oder Datei wählen**" klicken, um die KBART-Datei im Dateisystem auszuwählen.
4.  Sind alle Informationen über den Auftrag eingegeben, auf **Speichern & schließen** klicken. Der Auftrag ist gespeichert und wird im Hintergrund verarbeitet.

## Felder

* **Paketname**. Der Name des Pakets, der in der App eManagement im Bereich E-Ressourcen angezeigt wird, wenn die lokale KB von der Bibliothek verwendet wird.
* **Paketquelle**. Angabe der Quelle der Paketliste.
* **Paketreferenz**. Die Paketreferenz, z.B. eine Paket-ID.
* **Paketanbieter**. Der Name des Anbieters, auf dessen Plattform der Paketinhalt verfügbar ist. Wenn der eingegebene Anbieter nicht existiert, wird ein neuer in der lokalen Knowledgebase in der App eManagement erstellt.
* **Diesem Job als Quelle für Titelinstanz-Metadaten vertrauen**. Wenn diese Checkbox aktiviert ist, überschreiben die Daten in der KBART-Datei alle vorhandenen Titeldaten, die während des Importvorgangs abgeglichen werden. Auf diese Weise kann z.B. den Namen einer E-Ressource aktualisiert werden, die bereits in der lokalen KB existiert. Wenn die Checkbox nicht aktiviert ist, werden die Daten in der KBART-Datei keine vorhandenen Titeldaten überschreiben.

Die Felder Quelle und Referenz werden zusammen als eindeutiger Bezeichner für Pakete verwendet. Wenn ein Paket mit der angegebenen Quelle+Referenz bereits existiert, wird es aktualisiert, andernfalls wird ein neues Paket erstellt.
