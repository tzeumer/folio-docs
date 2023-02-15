---
title: "Datensatz ein Exemplar hinzufügen"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [app-katalog, by-folio, cat-workflows, for-anwender]
weight: 40
Description: "
    Quellen: [Folio](https://docs.folio.org/docs/metadata/inventory/#adding-an-item-to-a-record) <!-- & [GBV](https://info.gebev.de/pages/viewpage.action?pageId=852492470) -->
    "
---

1.  [Den Datensatz suchen]({{< ref "090 Datensatz suchen im Katalog" >}}), zu dem ein Exemplar hinzugefügt werden soll und es auswählen.
2.  In der Ansicht **Details des Instanzdatensatz** im Bereich Bestand auf **Exemplar hinzufügen** klicken.
3.  Im Fenster **Exemplardatensatz** die Abschnitte Administrative Daten, Exemplardaten, Daten zur Zählung, Zustand, Anmerkungen zum Exemplar, Ausleihe und Verfügbarkeit, Standort und Elektronischer Zugriff ausfüllen. Weitere Informationen zu den Feldern und Aktionen, die in diesen Abschnitten verfügbar sind, sind in den Abschnittsbeschreibungen weiter unten zu finden.
4.  Sobald alle gewünschten Informationen in den Exemplardatensatz aufgenommen wurden, auf **Speichern & schließen** klicken. Der Exemplardatensatz wird gespeichert.

## Administrative Daten

* **Datensatz zuletzt aktualisiert**. Datum und Uhrzeit, zu der der Datensatz zuletzt aktualisiert wurde. Auf **Datensatz Zuletzt aktualisiert** klicken, um die nächsten drei Felder anzuzeigen.
    * **Quelle**. Name der Person, die den Datensatz zuletzt aktualisiert hat.
    * **Datensatz erstellt**. Datum und Uhrzeit, zu der der Datensatz erstellt wurde.
    * **Quelle**. Name der Person, die den Datensatz erstellt hat.
* **Nachweis unterdrücken**. Wenn gewünscht ist, dass der Datensatz im Discoverysystem unterdrückt wird, die Checkbox **Nachweis unterdrücken** markieren.
* **Exemplar-HRID**. Die menschenlesbare ID. Eine vom System zugewiesene sequenzielle ID, die der Exemplar-ID zugeordnet ist.
* **Barcode**. In der Regel eine numerische Sequenz, die an der Ressource angebracht und mit einem Barcode-Scanner überprüft wird. Muss ein eindeutiger Wert sein.
* **Zugangsnummer**. Eine eindeutige Nummer, die einem Exemplar in der Reihenfolge zugewiesen wird, in der es in eine Bibliothekssammlung aufgenommen wird. Die meisten Bibliotheken vergeben Zugangsnummern in einer fortlaufenden numerischen Reihenfolge, aber einige verwenden ein Codesystem, um zusätzlich zur Reihenfolge des Zugangs die Art der Ressource und/oder das Jahr des Zugangs anzugeben. Auch Inventarnummer genannt.
* **Exemplaridentifikator**. Nummer zur Identifizierung des Exemplars. Zum Beispiel aus dem Verbundkatalog importiert (nur lesen).
* **Ehemaliger Identifikator**. Frühere Identifikatoren, die dem Exemplar zugewiesen wurden.
* **Statistischer Code**. Statistische Codes (z.B. ASER; Name: Active serial; Typ: SERM (Serienverwaltung) oder Bücher; Name: Buch, Druck (Bücher); Typ ARL (Sammlungsstatistik) usw.)

### Ehemaligen Identifikator hinzufügen

* Auf **Ehemaligen Identifikator hinzufügen** klicken.
* Einen **ehemaligen Identifikator** in das Feld eingeben.
* Die Schritte 1-2 je nach Bedarf wiederholen. Der ehemalige Identifikator wird gespeichert, sobald das Exemplar gespeichert wird.

### Statistischen Code hinzufügen

1.  Auf **Statistischen Code hinzufügen** klicken.
2.  Den statistischen Code aus der Dropdown-Liste auswählen.
3.  Die Schritte 1-2 je nach Bedarf wiederholen. Der statistische Code wird gespeichert, sobald das Exemplar gespeichert wird.

### Ehemaligen Identifikators oder statistischen Code löschen

1.  Den Ehemaligen Identifikator oder statistischen Code suchen, der gelöscht werden soll.
2.  Auf das **Mülleimersymbol** neben dem Identifikator oder Code klicken. Der Identifikator oder Code wird aus dem Exemplar entfernt und gelöscht, sobald das Exemplar gespeichert wird.

## Exemplardaten

Der Abschnitt Artikeldaten enthält zusätzliche Informationen über das Exemplar.

* **Materialart (erforderlich)**. Beschreibt die materielle Beschaffenheit eines bestimmten Exemplars, mit der Absicht, spezifischere Informationen als nur den Ressourcentyp zu ermöglichen. Wird unter [Einstellungen > Katalog > Materialarten]({{< ref "030 Materialarten" >}}) konfiguriert.
* **Exemplarnummer**. Die Exemplarnummer ist die Kennung des Teils. Die Exemplarnummer gibt an, ob die Bibliothek ein (oder mehrere) Exemplare einer einbändigen Monographie besitzt; ein (oder mehrere) Exemplare eines mehrbändigen Werkes, (z.B. Exemplar 1 oder C.7.)
* **Signaturtyp**. Das Klassifikationssystem, das für die Signatur verwendet wird. Den Signaturtyp aus der Dropdown-Liste auswählen. Wird unter [Einstellungen > Katalog > Signaturtypen]({{< ref "010 Signaturtypen" >}}) konfiguriert.
* **Signatur-Präfix**. Präfix der Signatur auf der Ebene des Exemplars.
* **Signatur**. Die Signatur ist eine einem Exemplar zugewiesene Kennung, die in der Regel auf einem am Exemplar angebrachten Etikett steht. Die Signatur wird verwendet, um die physische Position der Ressource in einer Regalreihenfolge zu bestimmen. Zum Beispiel: K1 .M44.
* **Signatur-Suffix**. Suffix der Signatur auf der Ebene des Exemplars.
* **Anzahl der Teile**. Anzahl der Teile. Wird verwendet, wenn ein Exemplar ausgeliehen oder zurückgegeben wird, um zu überprüfen, ob alle Teile vorhanden sind (z.B. 7 CDs in einem Set).
* **Beschreibung der Teile**. Beschreibung der Teile. Zum Beispiel 500 Teile eines Puzzles.

## Daten zur Zählung

Der Abschnitt Daten zur Zählung enthält Zählungsinformationen für alle Serien oder mehrteiligen Monographien.

* **Zählung**. Die beschreibenden Informationen für das Nummerierungsschema einer Serie, die in der Regel durch eine Ebene und eine beschreibende Überschrift gekennzeichnet sind. Zum Beispiel: Stufe 0 = v. und Stufe 1 = no. Das bedeutet, dass jede Ausgabe der Reihe einen Band und eine Ausgabenummer hat, die erscheinen würde (v.71:no.2-4).
* **Chronologie**. Die beschreibenden Informationen für das Datierungsschema einer Serie, die normalerweise durch die Ebene identifiziert werden. Zum Beispiel: Ebene 0 = Jahr Ebene 1 = Monat. Das bedeutet, dass jede Ausgabe der Serie einen Monat und ein Jahr enthält (1985:Juli-Dez.)
* **Band**. Band ist für mehrteilige Monographien gedacht. Zum Beispiel eine Biographie von George Bernard Shaw in drei Bänden.
* **Jahr, Bezeichnung**. In mehrteiligen Monographien wird eine Bezeichnung verwendet, um eine chronologische Ebene zu kennzeichnen. Zum Beispiel, Jahr 1985.

### Jahr, Bezeichnung hinzufügen

* Auf **Jahr, Bezeichnung hinzufügen** klicken.
* Eine **Jahr, Bezeichnung** in das Feld eingeben.
* Die Schritte 1-2 je nach Bedarf wiederholen. Jahr, Bezeichnung wird gespeichert, sobald das Exemplar gespeichert wird.

### Jahr, Bezeichnung löschen

* Das Jahr, Bezeichnung suchen, das gelöscht werden soll.
* Auf das **Mülleimersymbol** neben der Jahr, Bezeichnung klicken. Jahr, Bezeichnung wird aus dem Datensatz entfernt und gelöscht, sobald das Exemplar gespeichert wird.

## Zustand

Der Abschnitt Zustand enthält Informationen über den Zustand des Exemplars.

* **Anzahl der fehlenden Teile**. Anzahl der fehlenden Teile
* **Fehlende Teile**. Beschreibung der fehlenden Teile.
* **Datum**. Datum, an dem das/die Teil(e) vermisst wurde(n).
* **Schadensbeschreibung des Exemplars**. Ob das Exemplar beschädigt oder nicht beschädigt ist.
* **Datum**. Datum, an dem die Teile beschädigt wurden.

## Anmerkungen zum Exemplar

Der Abschnitt Anmerkungen zum Exemplar enthält alle Anmerkungen zum Exemplar.

### Anmerkung hinzufügen

1.  Auf **Anmerkung hinzufügen** klicken.
2.  Den **Anmerkungstyp** aus der Dropdown-Liste wählen. Konfiguriert unter [Einstellungen > Katalog > Anmerkungstypen des Exemplars]({{< ref "010 Anmerkungstypen des Exemplars" >}}).
3.  Eine **Anmerkung** in das Feld eingeben.
4.  Optional: Wenn die Anmerkung nur für Mitarbeitende sichtbar sein soll, die über die entsprechenden Berechtigungen verfügen, die Checkbox Nur Personal markieren.
5.  Die Schritte 1-4 je nach Bedarf wiederholen. Die Anmerkung wird gespeichert, sobald das Exemplar gespeichert wird.

### Anmerkung löschen

1.  Die Anmerkung suchen, die gelöscht werden soll.
2.  Auf das **Mülleimersymbol** neben der Anmerkung klicken. Die Anmerkung wird aus dem Exemplar entfernt und gelöscht, sobald das Exemplar gespeichert wird.

## Ausleihe und Verfügbarkeit

Der Bereich Ausleihe und Verfügbarkeit enthält Informationen über den Ausleihstatus des Exemplars.

* **Dauerhafter Ausleihtyp (erforderlich)**. Die Standardausleihart für das Exemplar. Zum Beispiel: Ausleihbar, Reservierte Exemplare, Lesesaal, Ausgewählt, usw. Wird unter [Einstellungen > Katalog > Ausleihtypen]({{< ref "020 Ausleihtypen" >}}) konfiguriert.
* **Temporärer Ausleihtyp**. Ein temporärer Ausleihtyp für das Exemplar. Zum Beispiel: Kann ausgeliehen werden, Semesterapparate, Lesesaal, Ausgewählt, usw. Konfiguriert unter [Einstellungen > Katalog > Ausleihtypen]({{< ref "020 Ausleihtypen" >}}).
* **Status**. Bezeichnung für den Status des Exemplars. Zum Beispiel: Verfügbar, Ausgeliehen, Im Transport, Im Abholregal, Auf Bestellung, usw. Standardmäßig ist der Status des Exemplars auf Verfügbar eingestellt.
* **Ausleih-/Rückgabeanmerkungen**. Alle Anmerkungen zu dem Exemplar, die dem Personal bei der Rückgabe oder Ausleihe angezeigt werden sollen.

### Ausleih-/Rückgabeanmerkungen hinzufügen

Eine Anmerkung bei der Rückgabe oder Ausleihe ist standardmäßig erforderlich.

1.  Den **Anmerkungstyp** aus der Dropdown-Liste wählen. Konfiguriert unter [Einstellungen > Katalog > Anmerkungstypen des Exemplars]({{< ref "010 Anmerkungstypen des Exemplars" >}}).
2.  Eine **Anmerkung** in das Feld eingeben.
3.  Optional: Wenn die Anmerkung nur für Mitarbeitende sichtbar sein soll, die über die entsprechenden Berechtigungen verfügen, die Checkbox Nur Personal markieren.
4.  Um eine weitere Anmerkung hinzuzufügen, auf Ausleih-/Rückgabeanmerkung hinzufügen klicken und die Schritte 1-3 wiederholen. Die Anmerkung wird gespeichert, sobald das Exemplar gespeichert wird.

### Ausleih-/Rückgabeanmerkung entfernen

1.  Die Anmerkung suchen, die gelöscht werden soll.
2.  Auf das **Mülleimersymbol** neben der Anmerkung klicken. Die Anmerkung wird aus dem Datensatz entfernt und gelöscht, sobald das Exemplar gespeichert wird.

## Standort

Der Abschnitt Standort enthält Informationen über den physischen oder elektronischen Standort des Exemplars.

* **Dauerhafter Standort (erforderlich)**. Der Standardstandort der Ressource, der ein physischer Standort sein kann, an dem die Ressource gespeichert ist, oder ein Online-Standort. Der Dauerhafte Standort wird auf der Bestandsebene zugewiesen, kann aber bei Bedarf auf der Ebene des Exemplars überschrieben werden. Einen Dauerhaften Standort aus der Dropdown-Liste auswählen oder auf Standortsuche klicken, um einen Standort auszuwählen.
* **Vorläufiger Standort**. Ein vorläufiger Standort für die Ressource. Das kann der ein physischer Standort oder ein Online-Standort sein, an dem die Ressource gespeichert ist. Vorläufige Standorte können auf der Ebene des Bestandes zugewiesen und bei Bedarf auf der Ebene der Exemplare überschrieben werden. Einen Vorläufigen Standort aus der Dropdown-Liste aus oder auf Standortsuche klicken, um einen Standort auszuwählen.

## Elektronischer Zugang

Im Bereich Elektronischer Zugang können Informationen zum Online-Zugriff für die Ressource hinzugefügt werden.

### Elektronischen Zugang hinzufügen

Anmerkung: Das Hinzufügen eines elektronischen Zugangs ist optional, aber wenn auf **Elektronischen Zugang hinzufügen** geklickt wird, muss ein URI eingeben oder der elektronischen Zugang gelöscht werden, um das Exemplar zu speichern.

1.  Auf **Elektronischen Zugang hinzufügen** klicken.
2.  Optional: Eine **Beziehung** aus der Dropdown-Liste auswählen.
3.  Optional: Eine **URI** in das Feld eingeben.
4.  Optional: Einen **Linktext** in das Feld eingeben.
5.  Optional: Die **Aufgeführten Materialien** eingeben.
6.  Optional: Eine **URL** **öffentliche Anmerkung** in das Feld eingeben.
7.  Die Schritte 1-6 je nach Bedarf wiederholen. Der elektronische Zugang wird gespeichert, sobald der Kurzaufnahme-Datensatz gespeichert wird.

### Elektronischen Zugang entfernen

1.  Den elektronischen Zugang suchen, der gelöscht werden soll.
2.  Auf das **Mülleimersymbol** neben dem elektronischen Zugang klicken. Der elektronische Zugang wird aus dem Datensatz entfernt und gelöscht, sobald der Kurzaufnahme-Datensatz gespeichert wird.
