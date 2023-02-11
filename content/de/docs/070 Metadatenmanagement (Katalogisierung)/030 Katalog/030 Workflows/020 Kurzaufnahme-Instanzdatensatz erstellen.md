---
title: "Kurzaufnahme-Instanzdatensatz erstellen"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [app-katalog, by-folio, cat-workflows, for-anwender]
weight: 20
Description: "
    Quellen: [Folio](https://docs.folio.org/docs/metadata/inventory/#creating-a-fast-add-instance-record) & [GBV](https://info.gbv.de/display/FOLIOGBVEXTERN/Folio:+Kurzaufnahme-Instanzdatensatz+erstellen)
    "
---

Eine Kurzaufnahme kann verwendet werden, um einen Instanzdatensatz mit einer begrenzten Anzahl von Informationen zu erstellen, die höchstwahrscheinlich benötigt werden. Die vollständige Liste der Informationen, die dem Datensatz hinzugefügt werden können, sind unter [Folio: Instanzdatensatz manuell in FOLIO erstellen](https://info.gbv.de/display/FOLIOGBVEXTERN/Folio%3A+Instanzdatensatz+manuell+in+FOLIO+erstellen), [Bestände zu einem Datensatz hinzufügen](https://info.gbv.de/pages/viewpage.action?pageId=852492467) und [Exemplar zu einem Datensatz hinzufügen](https://info.gbv.de/pages/viewpage.action?pageId=852492470) zu finden.

1.  In der Ansicht **Katalog** auf **Aktionen > Neue Kurzaufnahme** klicken.
2.  In Neue Kurzaufnahme die Abschnitte Instanz, Bestand und Exemplar ausfüllen. Weitere Informationen zu den Feldern und Aktionen, die in diesen Abschnitten verfügbar sind, sind in den Abschnittsbeschreibungen unten zu finden.
3.  Sobald alle gewünschten Informationen in den Instanzdatensatz eingegeben wurden, auf **Speichern & schließen** klicken. Der Instanzdatensatz wird gespeichert.

## Instanz

Der Abschnitt Instanzen enthält ausgewählte Felder des Instanzdatensatzes. Alle Felder, die in einem Instanzdatensatz verfügbar sind, sind unter [Folio: Instanzdatensatz manuell in FOLIO erstellen](https://info.gbv.de/display/FOLIOGBVEXTERN/Folio%3A+Instanzdatensatz+manuell+in+FOLIO+erstellen) zu finden.

-   **Nachweis unterdrückt**. Kurzaufnahme-Datensätze werden im Discoverysystem standardmäßig unterdrückt. Wenn der Datensatz in der Discoverysystem-Ebene angezeigt werden soll, die Checkbox Nachweis unterdrücken deaktivieren.
-   **Instanz-Statusbegriff**. Den Typ des Instanzstatus wählen, der dem Datensatz zugewiesen werden soll. Der Instanzstatus kann z.B. sein: katalogisiert, nicht katalogisiert, Batch-Import oder noch nicht zugewiesen. Die Instanz-Statusbegriffe werden von der Bibliothek in der App Einstellungen konfiguriert. Weitere Informationen sind unter Einstellungen > Katalog > Instanz-Statusbegriffezu finden.
-   **Ressourcentitel (erforderlich)**. Der primäre Titel (oder die Bezeichnung), der mit der Ressource verbunden ist.
-   **Erscheinungsdatum**. Das Jahr der Veröffentlichung, Verbreitung usw.
-   **ISBN**. Internationale Standardbuchnummer.
-   **ISSN**. Internationale Standard-Seriennummer.
-   **Ressourcentyp (erforderlich)**. Ein eindeutiger Begriff für die Ressource, der aus der Liste der RDA-Inhaltsbegriffe zugewiesen oder lokal definiert werden kann. Wird unter [Einstellungen > Katalog > Ressourcentypen](https://info.gbv.de/display/FOLIOGBVEXTERN/Einstellungen+%28Katalog%29%3A+Ressourcentypen) konfiguriert.
-   **Mitwirkende**. Alle Personen, die zu der Instanz beigetragen haben.

### Mitwirkende hinzufügen

Anmerkung: Das Hinzufügen eines Mitwirkenden ist optional, aber wenn auf **Mitwirkende/-n hinzufügen** geklickt wird, muss ein Namen und einen Namenstyp eingeben  oder der Mitwirkenden gelöscht werden, um den Instanzdatensatz zu speichern.

1.  Auf **Mitwirkende/-n hinzufügen** klicken.
2.  Den **Namen** in das Feld eingeben.
3.  Den **Namenstyp** aus der Dropdown-Liste auswählen.
4.  Optional: Den **Typ** des Mitwirkenden aus der Dropdown-Liste wählen.
5.  Optional: Auf **Primär** klicken, um den Mitwirkenden zum primären Mitwirkenden zu machen.
6.  Die Schritte 1-4 je nach Bedarf wiederholen. Der Mitwirkende wird gespeichert, sobald die Instanz gespeichert wird.

### Mitwirkende löschen

1.  Den Mitwirkenden suchen, der gelöscht werden soll.
2.  Auf das **Mülleimersymbol** neben dem Mitwirkenden klicken. Der Mitwirkende wird aus dem Datensatz entfernt und gelöscht, sobald die Instanz gespeichert wird.

## Bestand

Der Bereich Bestand enthält ausgewählte Felder für Bestandsdatensätze. Alle Felder, die in einem Bestandsdatensatz verfügbar sind, unter [Erstellen eines Bestandsdatensatzes](https://info.gbv.de/display/FOLIOGBVEXTERN/Folio%3A+Instanzdatensatz+manuell+in+FOLIO+erstellen) zu finden.

-   **Dauerhafter Standort (erforderlich)**. Der Standardstandort der Ressource, der ein physischer Standort sein kann, an dem die Ressource gespeichert ist, oder ein Online-Standort. Der Dauerhafte Standort wird auf der Bestandsebene zugewiesen, kann aber bei Bedarf auf der Ebene des Exemplars überschrieben werden. Einen Dauerhaften Standort aus der Dropdown-Liste auswählen oder auf Standortsuche klicken, um einen Standort auszuwählen.
-   **Vorläufiger Standort**. Ein vorläufiger Standort für die Ressource. Das kann der ein physischer Standort oder ein Online-Standort sein, an dem die Ressource gespeichert ist. Vorläufige Standorte können auf der Ebene des Bestandes zugewiesen und bei Bedarf auf der Ebene der Exemplare überschrieben werden. Einen Vorläufigen Standort aus der Dropdown-Liste aus oder auf Standortsuche klicken, um einen Standort auszuwählen.
-   **Signaturtyp**. Das für die Signatur verwendete Klassifikationssystem. Den Typ der Signatur aus der Dropdown-Liste auswählen. Konfiguriert unter [Einstellungen > Katalog > Signaturtypen](https://info.gbv.de/display/FOLIOGBVEXTERN/Einstellungen+%28Katalog%29%3A+Signaturtypen).
-   **Signatur-Präfix**. Präfix der Signatur auf der Bestandsebene. Zum Beispiel: FIC.
-   **Signatur**. Die Signatur ist eine einem Exemplar zugewiesene Kennung, die normalerweise auf einem am Exemplar angebrachten Etikett steht. Die Signatur wird verwendet, um die physische Position der Ressource in einer Regalreihenfolge zu bestimmen. Zum Beispiel: K1 .M44.
-   **Signatur-Suffix**. Suffix der Signatur auf der Bestandsebene. Zum Beispiel, das Jahr (2001).

## Exemplar

Der Abschnitt Exemplar enthält ausgewählte Felder des Exemplardatensatzes. Alle Felder, die in einem Exemplardatensatz verfügbar sind, sind unter [Hinzufügen eines Exemplars zu einem Datensatz](https://info.gbv.de/pages/viewpage.action?pageId=852492470) zu finden.

-   **Barcode**. In der Regel eine Zahlenfolge, die an der Ressource angebracht ist und mit einem Barcode-Scanner überprüft wird. Muss ein eindeutiger Wert sein.
-   **Materialart (erforderlich)**. Beschreibt die materielle Beschaffenheit eines bestimmten Exemplars, mit der Absicht, spezifischere Informationen als nur den Ressourcentyp zu ermöglichen. Wird unter Einstellungen > Katalog > Materialarten konfiguriert.
-   **Dauerhafter Ausleihtyp (erforderlich)**. Die Standard-Ausleihart für ein bestimmtes Exemplar. Zum Beispiel: Ausleihbar, Reservierte Exemplare, Lesesaal, Ausgewählt, usw. Konfiguriert unter [Einstellungen > Katalog > Ausleihtypen](https://info.gbv.de/display/FOLIOGBVEXTERN/Einstellungen+%28Katalog%29%3A++Ausleihtypen).
-   **Anmerkungen zum Exemplar (erforderlich)**. Alle Anmerkungen zu dem Exemplar, die dem Personal bei der Rückgabe oder Ausleihe angezeigt werden sollen.
-   **Elektronischer Zugriff**. Online-Zugriffsinformationen für das Exemplar.

### Ausleih-/Rückgabeanmerkung

#### Ausleih-/Rückgabeanmerkung hinzufügen

Eine Anmerkung bei der Rückgabe oder Ausleihe ist standardmäßig erforderlich.

1.  Den **Anmerkungstyp** aus der Dropdown-Liste wählen. Konfiguriert unter [Einstellungen > Katalog > Anmerkungstypen des Exemplars](https://info.gbv.de/display/FOLIOGBVEXTERN/Einstellungen+%28Katalog%29%3A++Anmerkungstypen+des+Exemplars).
2.  Eine **Anmerkung** in das Feld eingeben.
3.  Optional: Wenn die Anmerkung nur für Mitarbeitende sichtbar sein soll, die über die entsprechenden Berechtigungen verfügen, die Checkbox Nur Personal markieren.
4.  Um eine weitere Anmerkung hinzuzufügen, auf Ausleih-/Rückgabeanmerkung hinzufügen klicken und die Schritte 1-3 wiederholen. Die Anmerkung wird gespeichert, sobald der Kurzaufnahme-Datensatz gespeichert wird.

#### Ausleih-/Rückgabeanmerkung entfernen

1.  Die Anmerkung suchen, die gelöscht werden soll.
2.  Auf das **Mülleimersymbol** neben der Anmerkung klicken. Die Anmerkung wird aus dem Datensatz entfernt und gelöscht, sobald der Kurzaufnahme-Datensatz gespeichert wird.

### Elektronischen Zugang

#### Elektronischen Zugang hinzufügen

1.  Auf **Elektronischen Zugang hinzufügen** klicken.
2.  Optional: Eine **Beziehung** aus der Dropdown-Liste auswählen.
3.  Optional: Eine **URI** in das Feld eingeben.
4.  Optional: Einen **Linktext** in das Feld eingeben.
5.  Optional: Die **Aufgeführten Materialien** eingeben.
6.  Optional: Eine **URL** **öffentliche Anmerkung** in das Feld eingeben.
7.  Die Schritte 1-6 je nach Bedarf wiederholen. Der elektronische Zugang wird gespeichert, sobald der Kurzaufnahme-Datensatz gespeichert wird.

#### Elektronischen Zugang entfernen

1.  Den elektronischen Zugang suchen, der gelöscht werden soll.
2.  Auf das **Mülleimersymbol** neben dem elektronischen Zugang klicken. Der elektronische Zugang wird aus dem Datensatz entfernt und gelöscht, sobald der Kurzaufnahme-Datensatz gespeichert wird.
