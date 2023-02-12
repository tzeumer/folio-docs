---
title: "Standort einrichten"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [app-einstellungen, by-folio, cat-einstellungen, for-admin]
weight: 20
Description: "
    Quellen: [Folio](https://docs.folio.org/docs/settings/settings_tenant/settings_tenant/#settings--tenant--location-setup) & [GBV](https://info.gbv.de/display/FOLIOGBVEXTERN/Einstellungen+(Mandant):+Standort+einrichten)
    "
---

{{% pageinfo %}}
* [Standorte](https://info.gbv.de/display/FOLIOGBVEXTERN/Standorte) auch beachten bei Erste Schritte - teils eventuell etwas redundant und besser zusammenzuführen
{{% /pageinfo %}}

Diese Einstellungen unter Standort einrichten verwenden, um die vier Teile des Hierarchie für den Standort eines Exemplars zu konfigurieren. Standorte müssen konfiguriert werden, um Bestände und Exemplare im Katalog anzulegen, um Exemplare über die Apps Ausleihe und Rückgabe zu verbuchen und um Exemplare über die App Bestandsanfragen anzufordern.

Die Einrichtung der Standorte besteht aus vier Elementen, die hierarchisch miteinander verbunden sind, und zwar von oben nach unten: Institutionen > Campus > Bibliotheken > Standorte.

## Tatsächlicher Standort

In FOLIO haben Exemplare einen tatsächlichen Standort, der anhand der Standortwerte in den Bestands- und Exemplardatensätzen berechnet wird. Die Ausleihregeln verwenden den tatsächlichen Standort eines Exemplars, wenn sie Geschäftslogik auf Ausleihtransaktionen anwenden.

Vormerkungen müssen einen Wert für einen dauerhaften Standort haben. Ein Bestand kann auch einen Wert für einen temporären Standort haben. Exemplare können auch einen Wert für einen dauerhaften Standort und/oder einen Wert für einen temporären Standort haben. Der tatsächlichen Standortwert eines Exemplars ist der erste Wert, den es in dieser Reihenfolge findet:

1.  Exemplar Temporärer Standort
2.  Exemplar Dauerhafter Standort
3.  Bestand Temporärer Standort
4.  Bestand Dauerhafter Standort

## Tipps für Systemverwaltende

* In FOLIO ist es nicht erforderlich, dass die Elemente der Standorthierarchie der Geografie eines Campus entsprechen. Es kann hilfreich sein zu überlegen, ob eine bestimmte Bibliothek oder mehrere Bibliotheken in einem System besser als Campus modelliert werden sollten oder ob für einen bestimmten Arbeitsablauf zusätzliche Campus oder Institutionen benötigt werden.
* Da die Standorthierarchie eine Hierarchie aufweist, sollten die Werte in der Reihenfolge der Hierarchie erstellt werden: Institutionen, Campus, Bibliotheken und dann Standorte.
* Standorte müssen mindestens eine zugehörige Servicestelle haben. Es sollten Servicestellen angelegt sein, bevor die Standorthierarchie erstellt wird.
* Die vier Teile der Standorthierarchie können zusammen mit Personengruppen, Materialtypen und Ausleiharten Teil von Ausgaberegeln sein. Beim Einrichten der Standorte sollte die Strategie für die Ausgaberegeln berücksichtigt werden.
