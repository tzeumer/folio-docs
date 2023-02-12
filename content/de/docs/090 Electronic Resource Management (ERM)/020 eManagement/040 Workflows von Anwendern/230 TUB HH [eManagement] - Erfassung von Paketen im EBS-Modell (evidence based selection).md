---
title: "TUB HH [eManagement] - Erfassung von Paketen im EBS-Modell (evidence based selection)"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [app-e_management, by-tubhh, cat-workflows, for-anwender, by-community_einzelbeitrag]
weight: 230
Description: "
    Quellen: [Originalquelle](https://intranet.b.tu-harburg.de/mediawiki/index.php/FOLIO/Module/ERM/Workflows/Erfassung_EBS-Modell) & [GBV](https://info.gbv.de/pages/viewpage.action?pageId=855343296)
    "
---

{{% pageinfo %}}
Stand 2023-01
{{% /pageinfo %}}

## E-Management-App

* Es wird eine Vereinbarung für das laufende EBS-Paket erstellt, sowie eine Vereinbarung für die anschließend aus diesem Paket gekauften E-Books
* Es gibt die Möglichkeit die erste Vereinbarung oder Teile der Vereinbarung zu duplizieren, damit nicht alles neu eingegeben werden muss, was in beiden Vereinbarungen gleich ist.
* Im Akkordeon "zugehörige Vereinbarung" werden die beiden Vereinbarungen miteinander verknüpft
* Die Verknüpfungen werden mit den Beziehungen "tracks demand-driven acquisition for" und "has demand-driven acquisitions in" beschrieben.

### Vereinbarung für EBS-Paket

* Als Startdatum der einzelnen Vereinbarungsperiode kann z.B. das Datum verwendet werden an dem unser Lieferant die Bestellung oder die Verlängerung des Pakets bestätigt hat.
* Solange sich das Lizenzmodell nicht ändert, wird die Vereinbarung bei Verlängerung des EBS-Modells weiter genutzt und um die nächste Vereinbarungsperiode erweitert
* Wenn wir das Paket selbst in der GOKb pflegen, müssen die Paketdaten, wenn möglich durch den automatischen Upload laufend aktualisiert werden. Ist ein automatischer Upload nicht möglich, weil z.B. kein entsprechender Link zur Verfügung steht, sollte regelmäßig eine neue KBART-Datei beim Verlag angefordert werden und die Aktualisierung des Pakets manuell durchgeführt werden. Das Workflow-Gitlab kann dafür genutzt werden die Aktualisierung des Pakets zu terminieren.
* "Dauerhafter Zugriff" muss auf "nein" gesetzt werden

#### Verlängerung des EBS-Modells

* Bei einer Verlängerung wird die Vereinbarung weitergeführt:
    * Das Paket muss in der GOKb weiter aktualisiert werden
    * Es wird eine neue Vereinbarungsperiode hinzugefügt

### Vereinbarung für ausgewählte Festkäufe

* Prüfen, ob über den jeweiligen Admin-Account auch KBART-Dateien für die Festkäufe zur Verfügung gestellt werden (Beispiel Cambridge)
* Ggf. Absprachen mit dem Verlag/Anbieter treffen, ob KBART-Dateien für die Festkäufe geliefert/bereitgestellt werden können (ggf. fehleranfällig)
* Alternativ die KBART-Datei anhand unserer ausgewählten Festkäufe, die als Excel-Datei gespeichert wurden selbstbauen
* Die Vereinbarung des laufenden EBS-Pakets kann dubliziert werden, sodass nur die Angaben bezüglich der Festkäufe ergänzt bzw. korrigiert werden müssen
* Die Vereinbarungsperiode beginnt nachdem die Festkäufe getätigt und vom Anbieter bestätigt wurden. Das Enddatum wird nicht besetzt da auf die Titel ein dauerhafter Zugriff besteht
* Die Vereinbarung wird mit der Vereinbarung des laufenden EBS-Pakets verknüpft

### Lizenzverträge bei EBS-Festkäufen

* Gelten für die Festkäufe die gleichen Bedingungen (und es gibt nur einen Vertrag), wie für das laufende EBS-Paket, kann der gleiche Vertrag auch mit der Vereinbarung für die Festkäufe verknüpft werden
* Gibt es ein Amendment in dem die Festkäufe aufgeführt werden, wird dieses Dokument ebenfalls in Folio im Vertrag gespeichert
* Bei veränderten Bedingungen muss ggf. ein zweiter Vertrag angelegt werden
* [f](https://info.gbv.de/label/FOLIOGBVEXTERN/for-anwender)
