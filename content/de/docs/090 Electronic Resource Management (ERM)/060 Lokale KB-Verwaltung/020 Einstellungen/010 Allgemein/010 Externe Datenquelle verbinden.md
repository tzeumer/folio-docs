---
title: "Externe Datenquelle verbinden"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [app-lokale_kb_verwaltung, by-folio, cat-einstellungen, for-admin]
weight: 10
Description: "
    Quellen: [Folio](https://docs.folio.org/docs/erm/local-kb-admin/#connecting-an-external-kb) & [GBV](https://info.gbv.de/display/FOLIOGBVEXTERN/Einstellungen+(Lokale+KB-Verwaltung):+Externe+Datenquelle+verbinden)
    "
---

Die App Lokale KB-Verwaltung bietet die Möglichkeit, externe Datenquellen zu konfigurieren, die dann in regelmäßigen Abständen auf Änderungen der Metadaten abgefragt werden. Die externe Quelle wird dadurch in der lokalen KB synchron gehalten und kann als Grundlage für Vereinbarungskomponenten in der App eManagement dienen. Um dem System eine externe Datenquelle hinzuzufügen, folgendermaßen vorgehen

1.  [Einstellungen > Lokale KB-Verwaltung > Externe Datenquellen](https://info.gbv.de/display/FOLIOGBVEXTERN/Einstellungen+%28Lokale+KB-Verwaltung%29%3A+Externe+Datenquelle+verbinden) öffnen.
2.  In der Ansicht **Externe Datenquellen** auf **Neu** klicken, um eine neue Datenquelle zum System hinzuzufügen.
3.  Die Pflichtfelder ausfüllen. Weitere Informationen zu den Feldern sind in den Abschnittsbeschreibungen unten zu finden.
4.  Sobald alle Informationen über die externe Datenquelle eingegeben wurden, auf **Speichern** klicken. Der Harvester wird bei seinem nächsten Lauf Daten aus der neuen Quelle abrufen.

## Felder

-   **Name**. Der Name der externen Quelle, wie er in eManagement > E-Ressourcen (Registerkarte) > Filter Externe Datenquelle angezeigt wird.
-   **Typ**. Der Adaptertyp, z.B. für die Verbindung mit GOKb
    `org.olf.kb.adapters.GOKbOAIAdapter`
-   **Datensatz-Typ**. Der Datensatztyp, der zum Starten des Abrufvorgangs verwendet wird. Wenn er auf Paket gesetzt ist, holt der Harvester alle Pakete und die in diesen Paketen enthaltenen Titel ab.
-   **URI**. URL, die auf den OAI-Zugang verweist.
-   **Vertrauenswürdig für Titelinstanz-Metadaten**. Wenn diese Checkbox aktiviert ist, überschreiben die Daten im OAI-Stream alle vorhandenen Titeldaten, die während des Importvorgangs abgeglichen werden. Auf diese Weise kann z.B. den Namen einer E-Ressource aktualisiert werden, die bereits in der lokalen KB vorhanden ist. Wenn die Checkbox nicht aktiviert ist, werden die Daten im OAI-Stream keine vorhandenen Titeldaten überschreiben.
-   **Ist aktiv**. Wenn diese Checkbox aktiviert ist, wird die Datenquelle in das Harvesting einbezogen.
-   **Unterstützt das Harvesting**. (Derzeit nicht funktionsfähig). Zeigt an, ob die Datenquelle das Harvesting von Daten unterstützt
-   **Aktivierung eingeschaltet**. (Derzeit nicht funktionsfähig). Zeigt an, ob die Datenquelle Aktivierungs-/Auswahlinformationen für Ressourcen unterstützt.
-   **Listprefix**. Für Datenquellen, die mit dem OAI-PMH (Open Access Initiative Protocol for Metadata Harvesting) gesammelt wurden, kann hier das Metadatenpräfix für die ListRecords-Methode angegeben werden. Dies kann je nach dem für die Quelle angegebenen Adaptertyp erforderlich sein
-   **Fullprefix**. Für Datenquellen, die mit dem OAI-PMH (Open Access Initiative Protocol for Metadata Harvesting) gesammelt wurden, kann dies verwendet werden, um das Metadatenpräfix für die Fullprefix-Methode anzugeben. Dies kann je nach dem für die Quelle angegebenen Adaptertyp erforderlich sein
-   **Kundenkennung**: Die Konto-ID für die externe KB.
-   **Credentials**: Der API-Schlüssel für die externe KB.
