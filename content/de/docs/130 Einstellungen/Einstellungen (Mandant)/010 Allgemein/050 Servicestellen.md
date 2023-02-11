---
title: "Servicestellen"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [app-einstellungen, by-folio, cat-einstellungen, for-admin]
weight: 50
Description: "
    Quellen: [Folio](https://docs.folio.org/docs/settings/settings_tenant/settings_tenant/#settings--tenant--service-points) & [GBV](https://info.gbv.de/display/FOLIOGBVEXTERN/Einstellungen+(Mandant):+Servicestellen)
    "
---

Diese Einstellung verwenden, um die Servicestellen der Bibliothek zu konfigurieren. In FOLIO ist ein Servicepunkt ein Arbeitsort für Bibliotheksmitarbeiter.

Ein Servicepunkt wird benötigt, wenn mindestens einen der folgenden Dienste an diesem Ort angeboten werden:

-   Exemplare ausleihen.
-   Exemplare zurückgeben.
-   Bestandsanfrage für die Lieferung von Exemplaren an Personen.
-   Bestandsanfrage zur Abholung durch eine Person.
-   Exemplare an einen anderen Standort transportieren lassen.
-   Forderungen für Transaktionen erheben, die an diesem Standort stattgefunden haben.

Jeder Standort, der über physische Materialien verfügt, benötigt einen zugehörigen primären Servicepunkt, um diese Materialien zu verwalten. Daher sollten die gewünschten Servicestellen angelegt werden, bevor die Standorthierarchie erstellt wird.

Mitarbeitenden, die die Apps Ausleihe, Rückgabe, Bestandsanfrage und Personen verwenden, muss in ihren Personendatensatz ein Servicepunkt zugewiesen sein.

Es ist nicht erforderlich, dass ein Servicestelle ein Ort ist, der Personen Dienstleistungen anbietet. Für Bibliotheken kann es hilfreich sein, interne Servicestellen für Bereiche wie Regale, Bestandserhaltung oder Sammlungsentwicklung einzurichten.

## Servicestelle erstellen

1.  In der Ansicht **Servicestellen** auf **Neu** klicken.
2.  Im Fenster **Neuer Servicestelle** einen Namen für die Servicestelle ein. Der Name muss für den FOLIO-Mandanten eindeutig sein.
3.  Einen **Code** eingeben. Der Code ist der maschinenlesbare Name der Servicestelle und muss für Ihren FOLIO-Mandanten eindeutig sein.
4.  Einen **Anzeigename im Discovery** eingeben. Dieser Name wird in Discovery verwendet, um die Servicestelle für Personen zu identifizieren. Er muss nicht eindeutig sein.
5.  (Optional): Eine **Beschreibung** für die Servicestelle eingeben. Die Beschreibung wird nur in den Einstellungen angezeigt.
6.  (Optional): Die **Regalverzögerungszeit (Minuten)** für den Standort eingeben. Mit dieser Zahl wird festgelegt, wie lange es dauern soll, bis die an diese Servicestelle zurückgegebenen Materialien wieder ins Regal gestellt werden.
7.  (Optional): Auswählen, ob es sich bei der Servicestelle um einen **Abholstandort** handelt. Wenn es sich bei der Servicestelle um eine Abholstelle handelt, wird sie in der Bestandsanfrage und der App für Personen als Abholstandort angezeigt. Wird **Ja** gewählt, muss eine **Ablaufzeitraum für das Abholregal** eingeben, die festlegt, wie lange die Materialien im Abholregal zur Abholung bereitstehen.
8.  (Optional): Die Checkboxen **Vormerkung**, **Entnahmezettel**, **Bestandsanfrage** und/oder **Transport** aktivieren, um festzulegen, welche Belegzettel für diese Servicestelle standardmäßig gedruckt werden.
9.  Auf Speichern & schließen klicken. Eine Bestätigungsmeldung wird angezeigt und die Servicestelle wird erstellt.

Das Akkordeon **Zugewiesene Standorte** wird aktualisiert, wenn die Servicestelle einem Standort im Standortbaum zugewiesen wird.

## Servicestelle bearbeiten

1.  In der Ansicht **Servicestellen** die Servicestelle auswählen, die bearbeitet werden soll.
2.  In der Ansicht **Servicestellen-Details** auf **Bearbeiten** klicken.
3.  Im Fenster **Bearbeiten** die gewünschten Änderungen vornehmen.
4.  Auf **Speichern & schließen** klicken. Es wird eine Bestätigungsmeldung angezeigt und die Servicestelle wird aktualisiert.

## Servicestelle löschen

Eine Servicestelle kann nicht über die FOLIO Benutzeroberfläche gelöscht werden.
