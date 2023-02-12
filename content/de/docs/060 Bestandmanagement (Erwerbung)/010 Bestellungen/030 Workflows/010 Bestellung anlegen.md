---
title: "Bestellung anlegen"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [by-folio, for-anwender, cat-workflows, app-bestellungen]
weight: 10
Description: "
    Quellen: [Folio](https://docs.folio.org/docs/acquisitions/orders/#creating-an-order) & [GBV](https://info.gbv.de/display/FOLIOGBVEXTERN/Folio:+Bestellung+anlegen)
    "
---

Bestellungen enthalten eine Liste von Titeln oder Paketen (physisch oder elektronisch), die von der Bibliothek bei einem Lieferanten bestellt werden.

In FOLIO können entweder Einzelbestellungen oder laufende Bestellungen erstellt werden. Einzelbestellungen sollten für Exemplare verwendet werden, die innerhalb eines Jahres geliefert werden, wie z.B. Monografien. Laufende Bestellungen erstrecken sich in der Regel über mehrere Jahre, und werden in der Regel pro erhaltenem Exemplar bezahlt. Ein Beispiel für laufende Bestellung sind Zeitschriftenabonnements.

Sobald eine Bestellung erstellt wurde, muss der Bestellung [mindestens einen Bestellposten hinzugefügt](https://info.gbv.de/pages/viewpage.action?pageId=851017779) werden, damit die Bestellung geöffnet werden kann und der Erwerbungsvorgang beginnen kann. Die Erstellung einer Bestellung kann auch von der App Katalog aus initiiert werden, indem dort nach einer Instanz gesucht und auf Inventar > Aktionen > Neue Bestellung erstellen geklickt wird.

## Einzelbestellung erstellen

1.  In der Ansicht **Suche & Filter** auf **Bestellungen** klicken.
2.  In der Ansicht **Bestellungen** auf **Aktionen > Neu** klicken.
3.  Im Fenster **Bestellung erstellen** eine Vorlage aus der Dropdown-Liste **Vorlagenname** auswählen, falls verwendet. Die Bestellung wird mit den in der Vorlage konfigurierten Informationen ausgefüllt. Vorlagen werden in der App Einstellungen erstellt. Weitere Informationen sind unter Einstellungen > Bestellungen > Bestellvorlagen zu finden.
4.  **Einmalig** aus der Dropdown-Liste **Bestellungstyp** wählen.
5.  Die restlichen Felder unter Bestellung und Übersicht der Bestellung ausfüllen. Weitere Informationen zu den Feldern und Aktionen, die in diesen Abschnitten verfügbar sind, in den Abschnittsbeschreibungen unten zu finden.
6.  Optional: **Freigegeben** wählen, um die Bestellung zu freizugeben. Anmerkung: Die Bestellung muss nur genehmigt werden, wenn in die Bibliothek die Einstellung
    Freigegeben erforderlich aktiviert ist. Weitere Informationen sind unter [Einstellungen > Bestellungen > Freigaben](https://info.gbv.de/display/FOLIOGBVEXTERN/Einstellungen+%28Bestellungen%29%3A+Freigaben) zu finden.
7.  Auf **Speichern & schließen** klicken. Es erscheint eine Bestätigungsmeldung und die Bestellung wird in der Ansicht Bestellungen angezeigt.

### Bestellung

* **Präfix**. Falls zutreffend, aus der Dropdown-Liste ein Präfix für die Bestellnummer auswählen. Präfixe werden von der Bibliothek in der App Einstellungen konfiguriert. Weitere Informationen sind unter [Einstellungen > Bestellungen > Präfixe](https://info.gbv.de/pages/viewpage.action?pageId=851345594) zu finden.
* **Bestellnummer**. Die Bestellnummer für die Bestellung. Ob die Bestellnummer bearbeitet werde kann, hängt von den Einstellungen der Bibliothek in der Einstellung Bestellnummer bearbeiten ab. Siehe [Einstellungen > Bestellungen > Bearbeiten](https://info.gbv.de/display/FOLIOGBVEXTERN/Einstellungen+%28Bestellungen%29%3A+Bestellnummer+bearbeiten) für weitere Informationen.
* **Suffix**. Gegebenenfalls einen Suffix für die Bestellnummer aus der Dropdown-Liste auswählen. Suffixe werden von der Bibliothek in der App Einstellungen konfiguriert. Weitere Informationen sind unter [Einstellungen > Bestellungen > Suffixe](https://info.gbv.de/display/FOLIOGBVEXTERN/Einstellungen+%28Bestellungen%29%3A+Bestellnummer-Sufffixe) zu finden.
* **Lieferant**. Der mit dieser Bestellung verbundene Lieferant. Auf **Organisationssuche** klicken, um einen Lieferanten auszuwählen. Im Dialogfeld **Organisation wählen** die Organisation mithilfe des Suchfelds und/oder der Filter suchen. Auf die Organisation klicken, um sie auszuwählen. Die Organisation wird zum Feld Lieferant hinzugefügt.
* **Bestellungstyp**. Den Bestellungstyp wählen, der aufgeben werden soll: Einmalig oder Laufend.
* **Erwerbungsteams**. Ist gewünscht, dass die Bestellung für bestimmte Personen innerhalb bestimmter Erwerbungsteams verfügbar ist, die Erwerbungsteams eingeben oder aus der Dropdown-Liste auswählen. Es können mehrere Teams ausgewählt werden. Weitere Informationen zu Erwerbungsteams finden Sie unter [Einstellungen (Erwerbungsteams)](https://info.gbv.de/pages/viewpage.action?pageId=849379720).
* **Zugewiesen an**. Um die Bestellung einer Person zuzuweisen, auf das **+** klicken. Im Dialogfeld **Person auswählen** die Person mithilfe des Suchfelds und/oder der Filter suchen. Auf die Person klicken, um sie auszuwählen. Die Person erscheint im Feld **Zugewiesen an**. Wenn die Person entfernt werden soll, auf das **x** klicken. Wenn der Auftrag einer anderen Person zugewiesen werden soll, auf das **+** klicken und die obigen Schritte wiederholen.
* **Rechnungsadresse**. In der Dropdown-Liste Rechnungsadresse die Rechnungsadresse für die Bestellung auswählen. Sobald eine Adresse ausgewählt wurde, wird die Rechnungsadresse angezeigt. Die Adressen werden in der App Einstellungen konfiguriert. Weitere Informationen sind unter [Einstellungen > Mandant > Adressen](https://info.gbv.de/display/FOLIOGBVEXTERN/Einstellungen+%28Mandant%29%3A+Adressen) zu finden.
* **Lieferadresse**. In der Dropdown-Liste Lieferadresse die Adresse wählen, an die die Exemplare der Bestellung versandt werden sollen. Sobald eine Adresse ausgewählt wurde, wird die Versandadresse angezeigt. Adressen werden in der App Einstellungen konfiguriert. Weitere Informationen sind unter [Einstellungen > Mandant > Adressen](https://info.gbv.de/display/FOLIOGBVEXTERN/Einstellungen+%28Mandant%29%3A+Adressen) zu finden.
* **Manuell**. Wenn die Checkbox Manuell aktiviert ist, werden die Einstellungen für die EDI-Anbindung für diesen Lieferanten ignoriert und nichts aus dieser Bestellung wird an den Lieferanten übermittelt. Diese Checkbox zum Beispiel dann aktivieren, wenn die [EDI-Anbindung](https://info.gbv.de/pages/viewpage.action?pageId=842793035) der Bestellung eingerichtet ist.
* **Erneut belasten**. Die Checkbox Erneut belasten ist standardmäßig aktiviert. Wenn die Checkbox deaktiviert ist, wird damit angeben, dass die Bestellung während des Jahresübergangs nicht erneut belastet werden soll, auch wenn sie die Kriterien für eine erneute Belastung erfüllt. Wenn die Checkbox jedoch aktiviert ist und die Einstellungen für den Jahresübergang zum Ergebnis führen, dass dieser Auftrag die Kriterien für eine erneute Belastung nicht erfüllt, werden die Mittel für diesen Auftrag nicht für das nächste Haushaltsjahr gebunden. Diese Checkbox wird nur berücksichtigt, wenn die Bestellung die Kriterien für den Jahresübergang erfüllt. Wenn die Checkbox aktiviert ist und die Einstellungen für den Jahresübergang zum Ergebnis führen, dass diese Bestellung die Kriterien für eine erneute Belastung erfüllt, werden die Mittel für das nächste Haushaltsjahr für diese Bestellung gebunden.
* **Tags**. Die Tags eingeben oder wählen aus der Dropdown-Liste auswählen, die auf die Bestellung angewendet werden sollen.

### Zusammenfassung der Bestellung

* **Freigegeben**. Um die Bestellung freizugeben, die Checkbox Freigegeben markieren. Anmerkung: Die Bestellung muss nur genehmigt werden, wenn in die Bibliothek die Einstellung Freigegeben erforderlich aktiviert ist. Weitere Informationen sind unter [Einstellungen > Bestellungen > Freigaben](https://info.gbv.de/display/FOLIOGBVEXTERN/Einstellungen+%28Bestellungen%29%3A+Freigaben) zu finden.

## Laufende Bestellung erstellen

1.  In der Ansicht **Suche & Filter** auf **Bestellungen** klicken.
2.  In der Ansicht **Bestellungen** auf **Aktionen > Neu** klicken.
3.  Im Fenster **Bestellung erstellen** eine Vorlage aus der Dropdown-Liste **Vorlagenname** auswählen, falls verwendet. Die Bestellung wird mit den in der Vorlage konfigurierten Informationen ausgefüllt. Vorlagen werden in der App Einstellungen erstellt. Weitere Informationen sind unter [Einstellungen > Bestellungen > Bestellvorlagen](https://info.gbv.de/display/FOLIOGBVEXTERN/Einstellungen+%28Bestellungen%29%3A+Bestellvorlagen) zu finden.
4.  **Laufend** aus der Dropdown-Liste **Bestellungstyp** wählen.
5.  Die restlichen Felder unter Bestellung und Übersicht der Bestellung ausfüllen. Weitere Informationen zu den Feldern und Aktionen, die in diesen Abschnitten verfügbar sind, in den Abschnittsbeschreibungen unten zu finden.
6.  Optional: **Freigegeben** wählen, um die Bestellung zu freizugeben. Anmerkung: Die Bestellung muss nur genehmigt werden, wenn in die Bibliothek die Einstellung  Freigegeben erforderlich aktiviert ist. Weitere Informationen sind unter [Einstellungen > Bestellungen > Freigaben](https://info.gbv.de/display/FOLIOGBVEXTERN/Einstellungen+%28Bestellungen%29%3A+Freigaben) zu finden.
7.  Auf **Speichern & schließen** klicken. Es erscheint eine Bestätigungsmeldung und die Bestellung wird in der Ansicht Bestellungen angezeigt.

### Bestellung

Siehe Bestellung unter "Einzelbestellung erstellen" oben.

### Informationen zur laufenden Bestellung

* **Abonnement**. Wenn es sich bei der laufenden Bestellung um ein Abonnement handelt, die Checkbox Abonnement markieren.
* **Verlängerungsintervall**. Das Intervall für die Verlängerung, in Tagen. Dies ist der Zeitraum in Tagen, in dem die Bibliothek Zugriff auf diese Ressource hat und nach dessen Ablauf die Bibliothek eine weitere Verlängerung vornehmen muss. Dieses Feld kann nur bearbeitet werden und ist erforderlich, wenn Abonnement ausgewählt wurde.
* **Verlängerungsdatum**. Das Datum, bis zu dem die Bibliothek entscheiden muss, ob sie das Abonnement verlängern möchte oder nicht, was manchmal auch als Stornierungsfrist bezeichnet wird. Dieses Feld kann nur bearbeitet werden und ist erforderlich, wenn Abonnement ausgewählt ist.
* **Wiedervorlage-Zeitraum**. Der Zeitraum vor dem Verlängerungsdatum, in dem entschieden werden kann, ob das Abonnement verlängert werden soll. Dieses Feld kann nur bearbeitet werden, wenn Abonnement ausgewählt ist.
* **Manuelle Verlängerung**. Die Checkbox Manuelle Verlängerung markieren, um anzugeben, dass sich an den Lieferanten gewendet werden muss, um das Abonnement um einen weiteren Zeitraum zu verlängern  (der Lieferant erwartet nicht automatisch eine Verlängerung). Dieses Feld kann nur bearbeitet werden, wenn Abonnement ausgewählt ist.
* **Wiedervorlage**. Das Datum für die Überprüfung. Dieses Feld kann nur bearbeitet werden, wenn die Option Abonnement nicht ausgewählt ist.
* **Bemerkungen**. Alle Bemerkungen zur laufenden Bestellung.

### Zusammenfassung der Bestellung

Siehe Zusammenfassung der Bestellung unter "Einzelbestellung erstellen" oben.
