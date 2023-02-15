---
title: "Organisation (Lieferant) EDI-Verbindung hinzufügen"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [app-organisationen, by-folio, cat-workflows, for-anwender, topic-edi, meta-uebersetzungsproblem]
weight: 100
Description: "
    Quellen: [Folio](xxx) & [GBV](xxx)
    "
---

{{% pageinfo %}}
* "EDI-Verbindung" ist eine neue Übersetzung (de-discuss in Lokalise)
* Bei Organisationen > Konten ist Account number mit Kundennummer übersetzt
- 	Diverses rot (GBV)
{{% /pageinfo %}}

Dieser Abschnitt ermöglicht den Export von Bestellungen an Lieferanten im EDIFACT-Format. Um Informationen über eine oder mehrere EDI-Verbindung für eine Lieferantenorganisation hinzuzufügen, wie folgt vorgehen:

1.  Die [Organisation suchen](https://info.gbv.de/display/FOLIOGBVEXTERN/Folio%3A+Organisation+suchen) und auswählen, der eine EDI-Verbindung hinzugefügt werden soll.
2.  In der Ansicht **Organisationsdetails** auf das Akkordeon **EDI-Verbindung** klicken.
3.  Auf **EDI-Verbindung hinzufügen** klicken. Das Fenster **EDI-Verbindung erstellen** wird geöffnet.
4.  Informationen zu den Abschnitten Informationen, EDI-Konfiguration, FTP-Details und Zeitplanung hinzu. Weitere Informationen zu den Feldern und Aktionen, die in diesen Abschnitten verfügbar sind, finden Sie in den Abschnittsbeschreibungen unten.
5.  Auf **Speichern & schließen** klicken. Die EDI-Verbindung wird gespeichert und erscheint im Abschnitt EDI-Verbindungen in der Ansicht Organisation.

## Informationen zur EDI-Verbindung

1.  **Name der EDI-Verbindung (erforderlich)**. Der Name für diese EDI-Verbindung.
2.  **Beschreibung**. Eine Beschreibung dieser EDI-Verbindung.
3.  **Standard-EDI-Verbindung**. Diese Checkbox aktivieren, wenn für den Lieferant keine Konten verwendet werden. Dies bedeutet, dass jede für die Übermittlung markierte Bestellung, die sich nicht auf ein bestimmtes Konto für diesen Lieferanten bezieht, dieser Standardkonfiguration verwenden soll.

## EDI-Konfiguration

* **Kundennummer (erforderlich)**. Es werden alle Kundennummern aufgelistet, die im Abschnitt Konten des Lieferanten angelegt wurden. Auf alle Lieferantenkundennummer klicken, die in diese EDI-Konfiguration aufgenommen werden sollen. Um mehrere Kundennummern für diese Konfiguration auszuwählen, Umschalt+Klick verwenden. Wird de Cursor in ein anderes Feld bewegt, bleibt die Markierung auf der/den ausgewählten Kundennummer(n) bestehen.
* **Auftragsexport für Erwerbungsarten automatisieren**. Es werden alle  Erwerbungsarten aufgelistet. Wenn Bestellungen für diesen Lieferanten automatisch für bestimmten  Erwerbungsarten übermittelt werden sollen, auf den Namen der  Erwerbungsart klicken. Bei der Erstellung von Bestellungen kann dieses Standardverhalten außer Kraft gesetzt werden, indem die Checkbox Manuell auf der Bestellung aktivieren wird. Um mehrere Erwerbungsarten für den automatischen Export auszuwählen, Umschalt+Klick verwenden. Wird de Cursor in ein anderes Feld bewegt, bleibt die Markierung der ausgewählten  Erwerbungsarten weiterhin bestehen.
* **EDI-Kennung des Lieferanten (erforderlich)**. Die Kennung des Lieferanten für EDI-Transaktionen.
* **EDI-Typ des Lieferant**. Einen der Lieferanten-EDI-Typen auswählen, der den Typ der Kennung angibt, die als EDI-Kennung des Lieferanten verwendet wird: 014/EAN, 31B/US-SAN, 091/Lieferant zugewiesen oder 092/Kunde zugewiesen.
* **EDI-Kennung der Bibliothek (erforderlich)**. Der Bibliotheksidentifikator für EDI-Transaktionen.
* **EDI****\-Typ der** **Bibliothek**. Wählen Sie einen der Bibliotheks-EDI-Typen aus, der die Typ der Kennung angibt, die als EDI-Kennung der Bibliothek verwendet wird: 014/EAN, 31B/US-SAN, 091/Lieferant-zugeordnet oder 092/Kunde-zugeordnet.
* **EDI-Namenskonvention**. Die Namenskonvention für die ausgehenden FOLIO EDI-Dateien, wie z.B. das Präfix oder die Dateierweiterung. Beispiel: .edu Hinweis: Bei der Definition der Namenskonvention kann Text oder eines der folgenden Token verwendet werden. Die Token werden durch die entsprechenden Informationen aus dem Exportauftrag ersetzt. Mögliche Token sind organizationCode, integrationName, exportJobEndDate, jobID, numberSequence
* **Kundennummer senden**. Wenn die Kundennummer mit Bestellungen oder Rechnungen mitgeschickt werden soll, diese Checkbox aktivieren. Wenn dieses Kontrollkästchen aktivieren ist, ist die Kundennummer für die PO/POL (Bestellpostennummer?) erforderlich und wird in die EDI-Bestelldatei aufgenommen.
* **Welche Nachrichten werden für diesen Lieferanten erwartet?** Wenn die Bibliothek erwartet, EDI-Bestellungen an den Lieferanten zu senden, markieren Sie die Checkbox **Bestellungen**. Wenn Ihre Bibliothek erwartet, EDI-Rechnungen von dem Lieferanten zu erhalten, markieren Sie die Checkbox **Rechnungen**.
* **Anmerkungen**. Hinweise zu den Details der EDI-Verbindung für diesen Lieferanten.

## FTP-Details

* **Verbindungstyp**. Den FTP-Verbindungstyp auswählen, mit dem die Bibliothek die Transaktionen mit dem Lieferanten durchführen möchte: SFTP oder FTP.
* **Übertragungsmodus**. Den Übertragungsmodus, den die Bibliothek mit dem Lieferanten verwenden möchte: ASCII oder Binär.
* **Server-Adresse**. Die Adresse des FTP-Servers des Lieferanten.
* **FTP-Verbindungsmodus**. Den Verbindungsmodus auswählen: Aktiv oder Passiv.
* **Benutzername**. Der FTP-Benutzername, wenn ein Login-Benutzername für diesen Lieferanten erforderlich ist. Weitere Informationen zu den Berechtigungen für die Anzeige und Bearbeitung von EDI-Verbindungen sind unter [Berechtigungen für Organisationen](https://info.gbv.de/display/FOLIOGBVEXTERN/Organisationen) zu finden.
* **Kennwort**. Das FTP-Kennwort, wenn für diesen Lieferanten ein Anmeldekennwort erforderlich ist. Das Kennwort wird automatisch ausgeblendet. Auf **Anzeigen**, klicken um das Kennwort anzuzeigen. Auf **Ausblenden** klicken, um die Anzeige des Passworts zu beenden.
* **Port (erforderlich)**. Die Nummer des FTP-Ports.
* **Bestellverzeichnis**. Das Unterverzeichnis, in dem Bestellungen abgelegt werden sollen, wenn es sich vom FTP-Hauptverzeichnis für diesen Lieferanten unterscheidet. Beispiel: /Verzeichnis.
* **Rechnungsverzeichnis**. Das Unterverzeichnis, in dem die Rechnungen abgerufen werden sollen, wenn es sich vom FTP-Hauptverzeichnis für diesen Lieferanten unterscheidet. Bsp: /Verzeichnis.
* **Anmerkungen**. Hinweise zu den FTP-Details für diese EDI-Verbindung.

## Zeitplanung

* **Zeitplan**. Wenn die EDI zeitgesteuert konfiguriert werden soll, die Checkbox Zeitplan markieren.
* **Zeitraum festlegen**. Der Zeitraum zwischen den automatischen Übermittlungen an den Lieferanten. Zwischen Täglich und Wöchentlich wählen. Diese Version von FOLIO enthält aufgrund eines bekannten Problems, das in der nächsten Version behoben wird, keine Optionen für stündliche oder monatliche Zeiträume. Wenn einer dieser Werte zuvor auf einen Lieferanten angewendet wurde, kann es sein, dass der Export bei Verwendung von stündlichen oder monatlichen Zeitplänen nicht zum gewünschten Zeitpunkt erfolgt.
* **Datum**. Wenn unter Zeitraum festlegen "Täglich" gewählt wird, wird das Datumsfeld angezeigt. Die Kalenderfunktion verwenden, um das Startdatum für diesen Zeitplan auszuwählen.
    **Häufigkeit festlegen**. Wird eine Zeitraum von Täglich oder Wöchentlich gewählt, erscheint das Feld  Häufigkeit, Den numerischen Wert für die stündliche oder tägliche Häufigkeit dieser geplanten EDI-Verbindung eingeben.
* **Zeit**. Wird eine Zeitraum von Täglich oder Wöchentlich gewählt, erscheint das Feld Zeit. Auf dieses Feld klicken, um eine Auswahlliste mit Stunden und Uhrzeiten anzuzeigen. Die geplante Zeit für diesen automatischen Export wählen.
* **S M D M D F S.** Wird als Zeitraum Wöchentlich gewählt, werden die Checkboxen für den Wochentag angezeigt. Die Tage für diesen wöchentlichen automatischen Export wählen.
