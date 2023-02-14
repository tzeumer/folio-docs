---
title: "Erwartetes Teil hinzufügen"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [app-inventarisierung, by-folio, cat-workflows, for-anwender]
weight: 60
Description: "
    Quellen: [Folio](https://docs.folio.org/docs/acquisitions/receiving/#adding-an-expected-piece) & [GBV](https://info.gbv.de/pages/viewpage.action?pageId=851935460)
    "
---

Ein erwartetes Teil ist ein Teil einer Bestellung, die voraussichtlich erhalten wird. Wenn zum Beispiel ein Zeitschriftenabonnement bestellt wurde, ist zu erwarten, dass im Laufe des Jahres 12 verschiedene Teile erhalten. Wenn ein Buch bestellt wurde, das mit zusätzlichen Ressourcen wie einer CD oder einer Karte geliefert wird, ist zu erwarten, dass mehrere Teile mit der Bestellung erhalten werden. In der Bestellung wird zunächst nicht jedes Teil angezeigt, das mit der Bestellung geliefert wird. Werden einer Bestellung erwartete Teile hinzugefügt, kann verfolgt werden, welche Teile der Bestellung bereits inventarisiert wurden und welche noch erwartet werden.

Erwartete Teile sind im Abschnitt Erwartet in einem Datensatz der App Inventarisierung zu finden. Die erwarteten Teile können auch über diesen Abschnitt inventarisiert werden. Weitere Informationen sind unter Schnelles Empfangen zu finden.

Anmerkung: Damit ein erwartetes Teil in der Inventarisierung hinzugefügt werden kann, muss der [Workflow der Inventarisierung](https://info.gbv.de/pages/viewpage.action?pageId=851017779) auf der Bestellung auf "Unabhängige Bestell- und Eingangsmenge" eingestellt sein, wenn die Bestellung geöffnet wird.

1.  [Den zu inventarisierenden Titel suchen](https://info.gbv.de/display/FOLIOGBVEXTERN/Folio%3A+Inventarisierten+Titel+suchen), dem ein Teil hinzugefügt werden soll und ihn auswählen.
2.  In der Sektion **Erwartet** auf **Aktion** klicken. Im Aktionsmenü die Option **Teil hinzufügen** wählen.
3.  Im Dialogfeld **Teil hinzufügen** Informationen über das Teil hinzufügen. Weitere Informationen zu den einzelnen Feldern sind weiter unten zu finden.
4.  Wenn ein weiteres Teil hinzugefügt werden soll, nachdem dieses Teil gespeichert oder schnell inventarisiert wurde, auf **Weitere erstellen** klicken. Nachdem das Teil gespeichert und geschlossen oder schnell empfangen wurde, wird das Dialogfeld **Teil hinzufügen** mit den Details aus dem vorherigen Formular ausgefüllt.
5.  Um das Teil zu speichern und zu inventarisieren, auf **Schnell inventarisieren** klicken. Der neue Teil wird gespeichert und im Bereich Inventarisiert aufgelistet.
6.  Um zu speichern, ohne ein weiteres Teil hinzuzufügen, auf **Speichern & schließen** klicken. Das neue Teil wird gespeichert und im Abschnitt Erwartet aufgelistet.

## Teil hinzufügen

* **Bezeichnung**. Ein Wort, eine Phrase oder eine Abkürzung, die die Teile angibt, in die der Verlag die Serie unterteilt hat, z. B. "Band", "Teil" oder "Band".
* **Exemplarnummer**. Die Nummer des Exemplars des Teils.
* **Zählung**. Die Zählung des Teils, die die fortlaufende numerische und/oder alphabetische Bezeichnung angibt, die von einem Verlag verwendet wird, um die einzelnen bibliografischen oder physischen Teile zu identifizieren und die Beziehung jedes Teils zur bibliografischen Einheit als Ganzes aufzuzeigen.
* **Chronologie**. Die Chronologie des Teils, z. B. "Jahr", "Monat".
* **Stückformat**. Das Format der Bestellung, wie in Bestellungen ausgewählt. Dieses Feld ist nicht bearbeitbar.
* **Erwartetes Eingangsdatum**. Das Datum, an dem das Teil voraussichtlich inventarisiert wird.
* **Kommentar**. Kommentare oder Anmerkungen zu dem Teil.
* **Bestellposten Standorte**. Eine Liste der Standorte, die auf dem Bestellposten ausgewählt wurden.
* **Bestand auswählen**. In der Dropdown-Liste den Bestand für dieses Teil auswählen. Der Standort kann geändert werden, indem auf **Neue Bestände für Standort anlegen** geklickt wird.
* **Exemplar erstellen**. Die Checkbox **Artikel erstellen** markieren, um das neue Teil mit einer Instanz im Katalog zu verknüpfen. Diese Option steht nur für Teile zur Verfügung, die mit einer Bestellung verknüpft sind, bei der der Bestellposten **Im Katalog erstellen** auf "Instanz/Bestand/Exemplar" eingestellt ist. . Anmerkung: Um ein Exemplar im Katalog erstellen zu können, müssen in den Einstellungen bereits ein Standard-Instanzstatus, ein Instanztyp und ein Ausleihtyp eingerichtet sein. Siehe [Einstellungen > Bestellungen](https://info.gbv.de/pages/viewpage.action?pageId=851345510) für weitere Informationen.
* **Ergänzung**. Die Checkbox Ergänzung markieren, um anzugeben, dass es sich bei dem Teil um eine ergänzende Ressource wie eine CD oder eine Karte handelt.
* **Anzeige**. Die Checkbox **Anzeige** markieren, um anzugeben, dass Informationen zu diesem Teil in der App Katalog im Abschnitt Erwerbungen des Bestandsdatensatzes angezeigt werden sollen. Weitere Informationen sind unter Katalog > Erwerbung zu finden.

### Neuen Bestand für Standort anlegen

Anmerkung: Wenn der Standort für ein bestimmtes Teil geändert wird und noch kein Bestand für diesen Standort existiert, wird ein neuer Bestand angelegt.

1.  Im Dialogfeld **Stück hinzufügen** auf **Bestande auswählen** klicken.
2.  Im Dialog Dauerhafter Standort auswählen eine **Institution**, einen **Campus**, eine **Bibliothek** und einen **Standort** auswählen.
3.  Auf **Speichern und schließen** klicken. Die Änderungen werden im Feld **Bestand auswählen** des Dialogs **Stück hinzufügen** angezeigt. Der Standort wird bestätigt, sobald das Teil gespeichert ist.
