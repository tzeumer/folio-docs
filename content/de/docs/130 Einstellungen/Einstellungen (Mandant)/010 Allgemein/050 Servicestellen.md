---
title: "Servicestellen"
linkTitle: ""
date: 2023-03-04T00:00:00-00:00
tags: [app-einstellungen, by-folio, cat-einstellungen, for-admin]
weight: 50
Description: "
    Quellen: [Folio](https://docs.folio.org/docs/settings/settings_tenant/settings_tenant/#settings--tenant--service-points) <!-- & [GBV](https://info.gebev.de/display/FOLIOGBVEXTERN/Einstellungen+(Mandant):+Servicestellen) -->
    "
---

{{% pageinfo %}}
`Closed library date management for hold shelf expiration date calculation` ist noch nicht offiziell übersetzt. Verwendet `Ablaufdatumsberechnung des Abholregals bei geschlossener Bibliothek` 
{{% /pageinfo %}}

Closed library date management for hold shelf expiration date calculation

Diese Einstellung verwenden, um die Servicestellen der Bibliothek zu konfigurieren. In FOLIO ist ein Servicepunkt ein Arbeitsort für Bibliotheksmitarbeiter.

Ein Servicepunkt wird benötigt, wenn mindestens einen der folgenden Dienste an diesem Ort angeboten werden:

* Exemplare ausleihen.
* Exemplare zurückgeben.
* Bestandsanfrage für die Lieferung von Exemplaren an Personen.
* Bestandsanfrage zur Abholung durch eine Person.
* Exemplare an einen anderen Standort transportieren lassen.
* Forderungen für Transaktionen erheben, die an diesem Standort stattgefunden haben.

Jeder Standort, der über physische Materialien verfügt, benötigt einen zugehörigen primären Servicepunkt, um diese Materialien zu verwalten. Daher sollten die gewünschten Servicestellen angelegt werden, bevor die Standorthierarchie erstellt wird.

Mitarbeitenden, die die Apps Ausleihe, Rückgabe, Bestandsanfrage und Personen verwenden, muss in ihren Personendatensatz ein Servicepunkt zugewiesen sein.

Es ist nicht erforderlich, dass ein Servicestelle ein Ort ist, der Personen Dienstleistungen anbietet. Für Bibliotheken kann es hilfreich sein, interne Servicestellen für Bereiche wie Regale, Bestandserhaltung oder Sammlungsentwicklung einzurichten.

Alle Servicestellen sollten mit einem Forderungseigentümer/-in in den Einstellungen > Personen verknüpft werden, auch wenn nicht davon ausgegangen wird, dass Forderungen an Personen gestellt werden. Durch die Einrichtung der Verbindung wird sichergestellt, dass die Vorgänge nicht unerwartet fehlschlagen, wenn die Bibliothek doch beginnt, Forderungen zu erheben (manuell oder automatisch).
 
## Servicestelle erstellen

1.  In der Ansicht **Servicestellen** auf **Neu** klicken.
2.  Im Fenster **Neuer Servicestelle** einen Namen für die Servicestelle ein. Der Name muss für den FOLIO-Mandanten eindeutig sein.
3.  Einen **Code** eingeben. Der Code ist der maschinenlesbare Name der Servicestelle und muss für Ihren FOLIO-Mandanten eindeutig sein.
4.  Einen **Anzeigename im Discovery** eingeben. Dieser Name wird in Discovery verwendet, um die Servicestelle für Personen zu identifizieren. Er muss nicht eindeutig sein.
5.  (Optional): Eine **Beschreibung** für die Servicestelle eingeben. Die Beschreibung wird nur in den Einstellungen angezeigt.
6.  (Optional): Die **Regalverzögerungszeit (Minuten)** für den Standort eingeben. Mit dieser Zahl wird festgelegt, wie lange es dauern soll, bis die an diese Servicestelle zurückgegebenen Materialien wieder ins Regal gestellt werden.
7. (Optional): Auswählen, ob es sich bei der Servicestelle um einen **Abholstandort** handelt. Wenn es sich bei der Servicestelle um einen Abholstandort handelt, wird er in der Bestandsanfragen-App und der App Personen als Standort für Abholungen angezeigt.
8. (Erforderlich, wenn die Servicestelle ein **Abholstandort** ist): Einen **Abholregal-Ablaufdatums** eingeben, das bestimmt, wie lange die Bestandsanfrage im Status **Offen - Im Abholregal** verbleibt.
9. (Erforderlich, wenn es sich bei der Servicestelle um einen **Abholstandort** handelt): Die **Ablaufdatumsberechnung des Abholregals bei geschlossener Bibliothek** angeben. Damit wird FOLIO mitgeteilt, was mit dem Ablaufdatum des Abholregals geschehen soll, wenn es in eine Zeit fällt, in der die Servicestelle geschlossen ist.
    * Wenn der Zeitraum für das Abholregal in **Minuten** oder **Stunden** berechnet wird, kann gewählt werden, ob das ursprüngliche Ablaufdatum/die ursprüngliche Uhrzeit beibehalten, das Ablaufdatum/die Uhrzeit auf den Zeitpunkt zu dem die Servicestelle geschlossen wird verschoben, oder das Ablaufdatum/die Uhrzeit auf den Beginn der nächsten offenen Stunden verschoben werden soll.
    * Wenn der Zeitraum für das Abholregal in **Tagen**, **Wochen** oder **Monaten** berechnet wird, kann gewählt werden, ob das ursprüngliche Ablaufdatum beibehalten, das Ablaufdatum auf das Ende des letzten offenen Tages oder auf das Ende des nächsten offenen Tages verschobene werden soll.
10. (Optional): Die Checkboxen **Vormerkung**, **Entnahmezettel**, **Bestandsanfrage** und/oder **Transport** aktivieren, um festzulegen, welche Belegzettel für diese Servicestelle standardmäßig gedruckt werden.
11.  Auf Speichern & schließen klicken. Eine Bestätigungsmeldung wird angezeigt und die Servicestelle wird erstellt.

Das Akkordeon **Zugewiesene Standorte** wird aktualisiert, wenn die Servicestelle einem Standort im Standortbaum zugewiesen wird.

## Servicestelle bearbeiten

1.  In der Ansicht **Servicestellen** die Servicestelle auswählen, die bearbeitet werden soll.
2.  In der Ansicht **Servicestellen-Details** auf **Bearbeiten** klicken.
3.  Im Fenster **Bearbeiten** die gewünschten Änderungen vornehmen.
4.  Auf **Speichern & schließen** klicken. Es wird eine Bestätigungsmeldung angezeigt und die Servicestelle wird aktualisiert.

## Servicestelle löschen

Eine Servicestelle kann nicht über die FOLIO Benutzeroberfläche gelöscht werden.
