---
title: "Standorte"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [by-folio, for-admin, for-anwender]
weight: 40
Description: "
    Quellen: [Folio](https://docs.folio.org/docs/platform-essentials/locations/locations/) & [GBV](https://info.gbv.de/display/FOLIOGBVEXTERN/Standorte)
    "
---

In FOLIO werden Standorte verwendet, um zu beschreiben, wo sich Exemplare in der Bibliothek befinden.

Standorte sind für jede Bibliothek erforderlich, die Bestands- oder Exemplardaten in der Katalog-App verwenden möchte. Standorte werden in Workflows mit Servicestellen, der Ausleihe und Rückgabe von Artikeln, der Erhebung von Gebühren, der Anforderung von Artikeln, der Bereitstellung von Fernspeichern und dem Datenexport für Bestände und Exemplare verwendet.

Die Standorteinrichtung besteht aus vier hierarchischen Elementen - jede Ebene der Hierarchie muss mindestens einen Wert aufweisen, damit ein Wert auf der nächsten, spezifischeren Ebene erstellt werden kann.

-   **Institution**. Eine Institution ist die höchste Ebene der FOLIO-Standorthierarchie. Eine Institution repräsentiert in der Regel Entitäten wie ein Institut oder eine Universität, wobei dies keine Vorgabe von FOLIO ist. Sie können eine oder mehrere Institutionen erstellen.
-   **Campus**. Ein Campus ist die zweithöchste Ebene der FOLIO-Standorthierarchie. Ein Campus repräsentiert typischerweise verschiedene Teile einer Institution, wie einen physischen oder einen Zweigcampus oder Online-Programme, wobei dies keine Vorgabe von FOLIO ist.
-   **Bibliothek**. Eine Bibliothek ist die dritte Ebene der FOLIO-Standorthierarchie. Eine Bibliothek repräsentiert typischerweise physische Gebäude auf einem Campus oder Dienstbereiche auf einem virtuellen Campus, wobei dies keine Vorgabe von FOLIO ist.
-   **Standort**. Ein Standort ist die vierte und detaillierteste Ebene der FOLIO-Standorthierarchie. Ein Standort repräsentiert in der Regel bestimmte Regalbereiche, wie z. B. die Magazine, Lehrbücher oder bestimmte Sprachsammlungen, wobei dies keine Vorgabe von FOLIO ist.

In der Praxis stellen die meisten Bibliotheken physische Standorte in ihrem Standortbaum dar, aber FOLIO schreibt dies nicht vor. Bibliotheken können Standorte auf verschiedene Weise darstellen.

-   Eine Bibliothek könnte sich dafür entscheiden, ihre Sammlung durch den physischen Standort der Bestände zu beschreiben, z. B. 3. Stock, N-Seite, Gang 1, Seite A.
-   Eine Bibliothek kann ihre Standorte nach der Verwaltungsstruktur gruppieren, z. B. eine Institution mit zwei Standorten, einer für wissenschaftliche Mitarbeitende und einer für Studierende.
-   Eine Bibliothek könnte sich dafür entscheiden, ihre elektronischen Exemplare in ihre Standortstruktur einzubeziehen und eine Institution für physische Exemplare und eine Institution für elektronische Exemplare zu haben, wobei jede Institution ihren eigenen Campus, ihre eigene Bibliothek und ihre eigene Standortstruktur hat.

## Dauerhafte, temporäre und tatsächliche Standorte

Im Katalog können Sie in einem Bestands- und/oder Exemplardatensatz Werte für den dauerhaften und den temporären Standort festlegen. Für einen Bestand muss ein Wert für den dauerhaften Standort festgelegt sein.

Anhand der Werte in den Feldern für den dauerhaften und den temporären Standort berechnet FOLIO zwei effektive Standorte - einen im Bestandsdatensatz und einen im Exemplardatensatz. Tatsächliche Standorte unterstützen Arbeitsabläufe wie OAI-PMH-Harvesting, das Vormerken von Exemplaren und das Ausleihen von Exemplaren an Benutzer.

### Beispiele

Temporäre Standorte können zur Unterstützung verschiedener Bibliotheksabläufe verwendet werden.

#### Beispiel 1: Unterstützung eines Neuerscheinungsbereich in der Bibliothek

Die Smith University Library kauft ein Exemplar von The Midnight Library von Matt Haig, ein beliebtes neues Buch. Die Midnight Library soll drei Monate lang am Standort "Smith Neuzugänge" aufbewahrt werden, bevor sie an ihren dauerhaften Standort "Smith Hauptbestand" geschickt wird.

Bei der Bestellung des Exemplars setzen die Bibliotheksmitarbeiter den Standort in der Bestellzeile auf "Smith Hauptbestand". Dies ist dann der dauerhafte Standort für die Midnight Library.
Mithilfe von Datenimport- oder Katalog-Workflows setzen die Mitarbeiter dann den temporären Standort des Exemplars für The Midnight Library auf "Smith Neuzugänge". FOLIO setzt dann den tatsächlichen Standort des Exemplars auf "Smith Neuzugänge", und dieser Standort wird von FOLIO verwendet, wenn das Buch im Umlauf ist.
Nachdem die Mitternachtsbibliothek drei Monate lang im Umlauf war, entfernen die Bibliotheksmitarbeiter den temporären Standort des Exemplars mithilfe der Workflows für den Katalog oder den Datenimport. Dadurch wird der Tatsächliche Standort des Exemplars in "Smith Hauptbestand" geändert, und FOLIO verwendet diesen Standort, um das Exemplar in Zukunft auszuleihen.

#### Beispiel 2: Unterstützung der Renovierungsmaßnahmen einer Bibliothek

Das Pacific College renoviert seine Arts Library. Während der neunmonatigen Renovierung müssen die Mitarbeiter 5.000 Exemplare aus der Arts Library in die Undergraduate Library umziehen.

Die Bibliotheksmitarbeiter verwenden Datenimport-Workflows, um für die 5.000 Exemplare den temporären Standort "Undergrad Stacks" festzulegen und die Exemplare dann physisch zu verschieben.
Dadurch wird der Tatsächliche Standort für alle 5.000 Exemplare auf "Undergrad Stacks" geändert, und FOLIO verwendet diesen Standort, wenn sie im Umlauf sind.
Wenn die Renovierung abgeschlossen ist und die Exemplare in die Kunstbibliothek zurückgebracht werden, entfernen die Bibliotheksmitarbeiter mit Hilfe von Datenimport-Workflows den temporären Standort aller 5.000 Exemplare, wodurch sich deren tatsächlicher Standort wieder auf "Kunstbibliothek" ändert. FOLIO verwendet diesen Standort, um die Exemplare in Zukunft zu verteilen.

## Konfigurieren von Standorten

Der Standortbaum wird unter [Einstellungen > Mandant > Standort einrichten](https://info.gbv.de/display/FOLIOGBVEXTERN/Einstellungen+%28Mandant%29%3A+Standorte) konfiguriert.

## Tatsächliche Standorte von Beständen und Exemplaren

FOLIO unterstützt einen Tatsächlichen Standort von Beständen und Exemplaren. Beide Felder werden von FOLIO automatisch ermittelt.

### Tatsächlicher Standort des Bestandes

Der Tatsächliche Standort wird verwendet, um Informationen über den Standort von Beständen bereitzustellen, die nicht immer einzeln aufgeführt sind, wie z. B. Zeitschriften, Mikrofilme oder in Bearbeitung befindliche Sonderbestände. Er wird nicht in Workflows für die Ausleihe verwendet.

Im Bestandsdatensatz gibt es drei Standortfelder:

-   Dauerhafter Standort des Bestandes (erforderlich)
-   Temporärer Standort des Bestandes (optional)
-   Tatsächlicher Standort des Bestandes ( ermittelter Wert, von FOLIO festgelegt)

FOLIO setzt den tatsächlichen Standort des Bestands auf den ersten Wert, den es in der folgenden Liste findet:

1.  Temporärer Standort des Betriebs
2.  Dauerhafter Standort des Bestandes

Wenn die Bibliothek SRS für MARC-Bestände verwendet, kann das Feld für den dauerhaften Standort im Katalog nicht bearbeitet werden, sondern nur in quickMARC. Allerdings kann ein temporärer Standort für Bestände festgelegt werden.

### Tatsächlicher Standort eines Exemplars

Der Tatsächliche Standort eines Exemplars wird von FOLIO verwendet, um den aktuellen Standort eines Exemplars zu kennen, und damit Mitarbeiter und Benutzer wissen, wo ein Exemplar in der Bibliothek zu finden ist.

Der tatsächliche Standort eines Exemplars wird in mehreren Apps verwendet, darunter Ausleihe, Rückgabe, Bestellung und Personen (bei der Anzeige von Ausleihen und Gebühren/Geldbußen).

Im Exemplardatensatz gibt es drei Standortfelder:

-   Dauerhafter Standort des Exemplars (optional)
-   Temporärer Standort des Exemplars (optional)
-   Tatsächlicher Standort des Exemplars (berechneter Wert, von FOLIO festgelegt)

FOLIO setzt den tatsächlichen Standort des Exemplars auf den ersten Wert, den es in der folgenden Liste findet:

1.  Exemplar temporärer Standort
2.  Dauerhafter Standort des Exemplars
3.  Temporärer Standort
4.  Dauerhafter Standort
