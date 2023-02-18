---
title: "📱Bestandsanfragen"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [by-folio, for-anwender, app-bestandsanfragen, cat-berechtigungen, topic-exemplarstatus]
weight: 10
Description: "
    Quellen: [Folio](https://docs.folio.org/docs/access/requests/requests/) <!-- & [GBV](https://info.gebev.de/pages/viewpage.action?pageId=8391886) -->
    "
---

Mit der Bestandsanfragen-App werden Bestandsanfragen erstellt und verwaltet.

FOLIO unterstützt zwei Arten von Bestandsanfragen - auf Exemplarebene und auf Titelebene.

Bestandsanfragen auf Exemplarebene beziehen sich auf einen einzelnen Exemplardatensatz und sind die Standardform von Anfragen in FOLIO.

Bestandsanfragen auf Titelebene werden auf Instanzebene gestellt. FOLIO wählt das Exemplar aus den Beständen dieser Instanz aus, um die Anfrage zu erfüllen, unabhängig davon, ob das Exemplar sofort verfügbar ist oder erst bei der Rückgabe des Exemplars verfügbar wird.

Bibliotheken können Bestandsanfragen auf Titelebene unter [Einstellungen > Ausleihe > Bestandsanfragen auf Titelebene einschalten]({{< ref "030 Bestandsanfragen auf Titelebene" >}}).

Bibliotheken, die Bestandsanfragen auf Titelebene verwenden möchten, sollten dies berücksichtigen:

* Ist die Bestandsanfrage auf Titelebene erst einmal aktiviert, können Bestandsanfragen auf Titelebene nicht mehr deaktiviert werden, ohne dass diese Bestandsanfragen aus dem FOLIO-System entfernt werden.
* Offene Bestandsanfragen im System aus früheren Versionen von FOLIO sollten geschlossen werden, bevor Titelanfragen aktiviert werden, um Probleme mit der Reihenfolge in der Warteschlange zu vermeiden.
* Bestandsanfragen auf Titelebene können für jede Instanz im System erstellt werden, unabhängig von den Ausleihregeln. Die Ausleihregeln werden an dem Punkt überprüft, an dem eine Bestandsanfrage auf Titelebene mit einem Exemplar verknüpft werden würde. Wenn die Ausleihregeln das Stellen einer Bestandsanfrage nicht zulassen, verbleibt die Anfrage in der Bestandsanfragen-App mit dem Status Offen - noch nicht erledigt.
* Bestandsanfragen auf Titelebene werden für mehrbändige Werke noch nicht unterstützt - z.B. "ein beliebiges Exemplar von Band D der Longman Anthology of World Literature". Diese Bestandsanfragen müssen weiterhin als Anfragen auf Exemplarebene behandelt werden.
* Wenn ein Exemplar neu in FOLIO ist und über die App für die Inventarisierung oder den Datenimport hinzugefügt wurde, gibt es keinen Hinweis darauf, dass das Exemplar für eine offene Titelanfrage verwendet werden könnte. Das Exemplar muss zurückgegeben werden, damit eine Bestandsanfrage bearbeitet werden kann.

## Berechtigungen

Die unten aufgeführten Berechtigungen ermöglichen die Interaktion mit der Bestandsanfragen-App und legen fest, was innerhalb der App getan werden kann und was nicht. Personen können in der App Personen Berechtigungen zugewiesen werden. Wenn einer Personen keine dieser Berechtigungen zugewiesen sind, kann sie die Bestandsanfragen-App oder damit verbundene Informationen nicht sehen.

Im Folgenden sind alle Bestandsanfragen-Berechtigungen aufgeführt:

* **Bestandsanfragen: Alle Berechtigungen**. (Requests: All permissions)
    Mit dieser Berechtigung kann die Person alle Bestandsanfragen durchführen.
* **Bestandsanfragen: Verschieben zu neuem Exemplar, Warteliste neu anordnen**. (Requests: Move to new item, reorder queue)
    Mit dieser Berechtigung kann die Person Bestandsanfragen von einem Exemplar auf ein anderes umhängen (abhängig von den Anfragerichtlinien).
* **Bestandsanfragen: Warteliste neu anordnen**. (Requests, Reorder queue)
    Mit dieser Berechtigung können Personen auf die spezielle Seite für Bestandsanfragen zugreifen und diese nachbestellen. Sie wird nur für Personen benötigt, die die Warteschlange neu ordnen müssen. Sie benötigen diese Berechtigung nicht, um die Warteschlange einzusehen.
* **Bestandsanfragen: Anzeigen**. (Requests: View)
    Mit dieser Berechtigung können Personen Bestandsanfragen suchen und anzeigen.
* **Bestandsanfragen: Anzeigen, erstellen**. (Requests: View, create)
    Mit dieser Berechtigung kann die Person neue Bestandsanfragen erstellen und vorhandene Datensätze anzeigen.
* **Bestandsanfragen: Anzeigen, bearbeiten, stornieren**. (Requests: View, edit, cancel)
    Mit dieser Berechtigung können Personen Bestandsanfragen anzeigen, bearbeiten und stornieren.

## Bestandsanfragen: Typen und Status

Bestandsanfragen werden einem von drei Anfragetypen zugeordnet:

* **Vormerkung** (_hold_). Exemplare, die derzeit nicht verfügbar sind, aber bei Verfügbarkeit gewünscht werden.
* **Bestellung** (_page_). Exemplare, die aus dem Regal entnommen werden können.
* **Rückruf** (_recall_). Exemplare, die derzeit nicht verfügbar sind, aber sofort benötigt werden.

Bitte beachten, dass FOLIO den Rückruf von Exemplaren in einigen Status erlaubt, auch wenn sie nicht an eine Person ausgeliehen sind. In den FOLIO-Arbeitsabläufen gibt es jedoch derzeit keinen Unterschied zwischen einem Rückruf und einer Bestellung, wenn dies der Fall ist. Wenn eine Ausleihe zurückgerufen wird, kann die ursprüngliche Leihfrist verkürzt werden.

Offene Bestandsanfragen haben einen der folgenden Status:

* **Offen - Warten auf Lieferung** (_Awaiting delivery_): Die Bestandsanfrage wurde mit einem Exemplar verknüpft und befindet sich in der Auslieferung, aber das Exemplar ist noch nicht an die Person ausgeliehen worden. In der Regel bedeutet dies, dass es ein Problem mit der Bereitstellungsanfrage gibt.
* **Offen - Im Abholregal stehend** (_Awaiting pickup_): Zu der Bestandsanfrage gehört ein Exemplar, das sich derzeit am gewünschten Abholort befindet und darauf wartet, dass die Person es abholt.
* **Offen - In Transport** (_In transit_): Die Bestandsanfrage wurde mit einem Exemplar verknüpft, das gerade an die von der Person gewünschte Servicestelle geliefert wird.
* **Offen - Noch nicht erfüllt** (_Not yet filled_): Die Anfrage wurde noch nicht mit einem Exemplar verknüpft und das Ablaufdatum der Bestandsanfrage liegt, falls vorhanden, in der Zukunft.

Geschlossene Bestandsanfragen haben einen der folgenden Status:

* **Geschlossen - Storniert** (_Cancelled_): Die Anfrage wurde entweder storniert, bevor ein Exemplar zur Abholung verfügbar war, oder nachdem das Exemplar zur Abholung verfügbar war, aber bevor die Abholung abgelaufen ist.
* **Geschlossen - Erfüllt** (_Filled_): Die Bestandsanfrage wurde mit einem Exemplar verknüpft, das Exemplar wurde für die Person vorgemerkt und die Person hat das Exemplar ausgecheckt.
* **Geschlossen - Abgelaufen** (_Pickup expired_): Die Bestandsanfrage war mit einem Exemplar verknüpft, das Exemplar wurde für die Person in die Warteschleife gelegt, aber die Person hat das Exemplar nicht abgeholt, bevor das Ablaufdatum des Abholregals abgelaufen ist.
* **Geschlossen - Unerfüllt** (_Unfilled_): Die Bestandsanfrage wurde nicht mit einem Exemplar verknüpft, bevor das Ablaufdatum der Bestandsanfrage abgelaufen ist. Wenn das Feld Ablaufdatum der Bestandsanfrage leer ist, wird die Anfrage nie in diesen Status verschoben.

