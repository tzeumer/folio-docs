---
title: "📱Katalog"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [app-katalog, by-folio, cat-berechtigungen, for-anwender]
weight: 10
Description: "
    Quellen: [Folio](https://docs.folio.org/docs/metadata/inventory/) <!-- & [GBV](https://info.gebev.de/pages/viewpage.action?pageId=839188638) -->
    "
---

Mit der App Katalog werden (physischen und/oder virtuellen) Sammlungen verwaltet. Der Katalog speichert bibliographische, Bestands- und Exemplardaten in Form von Instanz-, Bestands- und Exemplardatensätzen. Instanzdatensätze können in FOLIO erstellt oder aus Datensätzen im Source Record Storage (SRS) generiert werden. Die Daten im Katalog sind mit anderen Apps wie Bestellungen, Rückgabe, Ausleihe und Bestandsanfragen verbunden.

Definition von Begriffen im Zusammenhang mit der App Katalog:

* **Instanzdatensatz**. Ein Datensatz, der bibliografische und administrative Informationen über eine bestimmte Ressource enthält. Der Instanzdatensatz ist der so genannte bibliografische Datensatz. Sie werden meist aus vollständigen bibliografischen Datensätzen (in MARC oder anderen Formaten) abgeleitet und sollen Bibliotheksmitarbeitenden Informationen zur Identifizierung und Auswahl von Datensätzen liefern, um Arbeiten an zugehörigen Beständen und Exemplaren durchzuführen.
* **Bestandsdatensatz**. Ein Datensatz, der Informationen wie Standort, Signatur und vorgehaltene Bände enthält und es Bibliotheksmitarbeitenden ermöglicht, den Bestand an Ressourcen aller Formate zu finden und zu verwalten. Ein Bestandsdatensatz muss mit einem Instanzdatensatz verknüpft sein.
* **Exemplardatensatz**. Ein Datensatz, der Informationen enthält, die zur Identifizierung und Nachverfolgung eines einzelnen Exemplars oder Teils erforderlich sind. Der Exemplardatensatz enthält Daten, die sich auf einen einzelnen Band oder ein einzelnes Teil beziehen, z.B. Barcode und Ausleihstatus. Ein Exemplardatensatz muss mit einem Bestandsdatensatz verknüpft sein.
* **HRID**. Human readable identifier. "Augenlesbare ID".
* **UUID**. Universally unique identifier (Universell eindeutige ID).
* **SRS**. Source Record Storage ("Quelldatenspeicher"). Eine Speicherebene in FOLIO. Wenn einer Instanz ein MARC-Datensatz zugrunde liegt, wird dieser Datensatz im SRS gespeichert.
* **Arbeitsdatensatz** (englisch: intellectual item). Dieser Status kann für einen Exemplardatensatz verwendet werden, der nicht mit einem einzelnen, eindeutigen physischen Objekt übereinstimmt. Kann auch als "Dummy-Datensatz" bezeichnet werden.

## Berechtigungen

Die unten aufgeführten Berechtigungen ermöglichen Ihnen die Interaktion mit der App Katalog und legen fest, was Sie innerhalb der App tun können und was nicht. Sie können Personen in der App Personen Berechtigungen zuweisen.

Im Folgenden finden Sie alle Berechtigungen für den Katalog:

* **Katalog: Alle Berechtigungen**. (Inventory: All permissions)
    Diese Berechtigung erlaubt es der Person, alle Aktionen im Katalog durchzuführen.
* **Katalog: Bestellung aus Instanz erstellen**. (Inventory: Create order from instance)
    Diese Berechtigung erlaubt es der Person, die Erstellung einer neuen Bestellung oder eines neuen Bestellpostens (in der App Bestellungen) von einem Instanzdatensatz in Katalog aus zu veranlassen.
* **Katalog: Einzelne bibliografische Datensätze importieren**. (Inventory: Import single bibliographic records)
    Diese Berechtigung erlaubt es der Person, Instanzdatensätze aus externen Quellen zu importieren und zu überlagern. Externe Quellen müssen in den Einstellungen konfiguriert werden.
* **Katalog: Exemplare als in Bearbeitung markieren**. (Inventory: Mark items in process)
    Mit dieser Berechtigung kann die Person den Status eines Exemplardatensatzes auf In Bearbeitung aktualisieren.
* **Katalog: Exemplare als in Bearbeitung markieren (nicht bestellbar)**. (Inventory: Mark items in process (non-requestable))
    Mit dieser Berechtigung kann der Benutzer den Status eines Exemplardatensatzes auf In Bearbeitung (nicht bestellbar) aktualisieren.
* **Katalog: Exemplare als Arbeitsdatensatz markieren**. (Inventory: Mark items intellectual item)
    Mit dieser Berechtigung kann die Person den Exemplarstatus eines Exemplardatensatzes auf Arbeitsdatensatz aktualisieren.
* **Katalog: Exemplare als lange vermisst markieren**. (Inventory: Mark items long missing)
    Mit dieser Berechtigung kann die Person den Exemplarstatus eines Exemplardatensatzes auf Lang vermisst aktualisieren.
* **Katalog: Exemplare als beschränkt markieren**. (Inventory: Mark items restricted)
    Mit dieser Berechtigung kann die Person den Exemplarstatus eines Exemplardatensatzes auf Beschränkt aktualisieren.
* **Katalog: Exemplare als nicht verfügbar markieren**. (Inventory: Mark items unavailable)
    Mit dieser Berechtigung kann die Person den Exemplarstatus eines Exemplardatensatzes auf Nicht verfügbar aktualisieren.
* **Katalog: Exemplare als unbekannt markieren**. (Inventory: Mark items unknown)
    Mit dieser Berechtigung kann die Person den Exemplarstatus eines Exemplardatensatzes auf Unbekannt aktualisieren.
* **Katalog: Exemplare als ausgesondert markieren**. (Inventory: Mark items withdrawn)
    Mit dieser Berechtigung kann die Person den Exemplarstatus eines Exemplardatensatzes auf Ausgesondert aktualisieren. Die Person kann auch Exemplare anzeigen und bearbeiten.
* **Katalog: Bestandsdatensätze verschieben**. (Inventory: Move holdings)
    Mit dieser Berechtigung kann die Person Bestandsdatensätze von einem Instanzdatensatz in einen anderen verschieben. Die Person kann außerdem Instanzen, Bestände und Exemplare suchen und anzeigen.
* **Katalog: Exemplare verschieben**. (Inventory: Move items)
    Mit dieser Berechtigung können Personen einen Exemplardatensatz von einem Bestandsdatensatz in einen anderen verschieben. Die Person kann außerdem Instanzen, Bestände und Exemplare durchsuchen und anzeigen.
* **Katalog: Für das Personal unterdrückte Instanzdatensätze anzeigen**. (Inventory: View instance records being suppressed for staff)
    Mit dieser Berechtigung kann die Person Instanzdatensätze, die für Mitarbeitende unterdrückt sind, suchen und anzeigen. (Derzeit nicht implementiert; standardmäßig können alle Personen, die Datensätze einsehen können, die für Mitarbeitende unterdrückten Datensätze einsehen).
* **Katalog: Instanzen, Bestände und Exemplare anzeigen**. (Inventory: View instances, holdings, and items)
    Mit dieser Berechtigung kann die Person Instanzen, Bestände und Exemplare anzeigen.
* **Katalog: Bestandsdatensätze anzeigen, erstellen**. (Inventory: View, create holdings)
    Mit dieser Berechtigung kann die Person neue Bestandsdatensätze erstellen. Die Person kann auch Bestände anzeigen.
* **Katalog: Instanzen anzeigen, erstellen**. (Inventory: View, create instances)
    Mit dieser Berechtigung kann die Person neue Instanzdatensätze erstellen. Die Person kann auch Instanzen anzeigen.
* **Katalog: Exemplare anzeigen, erstellen**. (Inventory: View, create items)
    Mit dieser Berechtigung können Personen neue Exemplardatensätze erstellen. Die Person kann auch Exemplare ansehen.
* **Katalog: Bestandsdatensätze anzeigen, erstellen, bearbeiten**. (Inventory: View, create, edit holdings)
    Mit dieser Berechtigung kann die Person bestehende Bestandsdatensätze bearbeiten. Die Person kann außerdem Bestände anzeigen und erstellen.
* **Katalog: Instanzen anzeigen, erstellen, bearbeiten**. (Inventory: View, create, edit instances)
    Mit dieser Berechtigung kann die Person bestehende Instanzdatensätze bearbeiten. Die Person kann auch Instanzen anzeigen und erstellen.
* **Katalog: Exemplare anzeigen, erstellen, bearbeiten**. (Inventory: View, create, edit items)
    Mit dieser Berechtigung kann die Person vorhandene Exemplare zu bearbeiten. Die Person kann außerdem Exemplare anzeigen und erstellen.
* **Katalog: Bestandsdatensätze anzeigen, erstellen, bearbeiten, löschen**. (Inventory: View, create, edit, delete holdings)
    Mit dieser Berechtigung kann die Person Bestandsdatensätze löschen. Die Person kann außerdem Bestände anzeigen und bearbeiten.
* **Katalog: Exemplare anzeigen, erstellen, bearbeiten, löschen**. (Inventory: View, create, edit, delete items)
    Mit dieser Berechtigung kann die Person Exemplare löschen. Die Person kann außerdem Exemplare anzeigen und bearbeiten.
* **Katalog: Exemplare anzeigen, erstellen, bearbeiten, fehlende Exemplare kennzeichnen**. (Inventory: View, create, edit, mark missing items)
    Mit dieser Berechtigung kann die Person den Status eines Exemplardatensatzes auf Vermisst aktualisieren. Die Person kann auch Exemplare anzeigen und bearbeiten.

Anmerkung: Einige Aktionen im Katalog erfordern Berechtigungen in anderen Apps. So erfordert z.B. die **Quelle anzeigen** eine Berechtigung in quickMARC.
