---
title: "Datensatz einen Bestand hinzufügen"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [app-katalog, by-folio, cat-workflows, for-anwender]
weight: 30
Description: "
    Quellen: [Folio](https://docs.folio.org/docs/metadata/inventory/#adding-holdings-to-a-record) & [GBV](https://info.gbv.de/pages/viewpage.action?pageId=852492467)
    "
---

## MARC-Bestandsdatensatz hinzufügen

1.  [Den Instanzdatensatz suchen](https://info.gbv.de/display/FOLIOGBVEXTERN/Folio%3A+Datensatz+suchen+im+Katalog), zu dem ein Bestand hinzugefügt werden soll und ihn auswählen.
2.  In der Ansicht **Details des Instanzdatensatzes** im Abschnitt **Bestand** auf **MARC-Bestandsdatensatz hinzufügen** klicken.
3.  Den neuen Datensatz gemäß den Anweisungen unter Bearbeiten eines MARC-Datensatzes mit quickMARC hinzufügen.
4.  Sobald alle gewünschten Informationen in den Bestandsdatensatz aufgenommen wurden, auf **Speichern & schließen** klicken**.** Der Datensatz wird gespeichert.

## FOLIO-Bestandsdatensatzes hinzufügen

1.  [Den Instanzdatensatz suchen](https://info.gbv.de/display/FOLIOGBVEXTERN/Folio%3A+Datensatz+suchen+im+Katalog), zu dem ein Bestand hinzugefügt werden soll und ihn auswählen.
2.  In der Ansicht **Details des Instanzdatensatzes** im Abschnitt **Bestand** auf **Bestand hinzufügen** klicken.
3.  Im Fenster **Bestandsdatensatz** die Abschnitte Administrative Daten, Standort, Details zum Bestand, Anmerkungen zum Bestand, Elektronischer Zugriff, Inventarisierung und Inventarisierungsverlauf ausfüllen. Weitere Informationen zu den Feldern und Aktionen, die in diesen Abschnitten verfügbar sind, sind in den Abschnittsbeschreibungen weiter unten zu finden.
4.  Sobald alle gewünschten Informationen in den Bestandsdatensatz aufgenommen wurden, auf **Speichern & schließen** klicken. Der Datensatz wird gespeichert.

### Administrative Daten

Der Abschnitt Administrative Daten enthält technische Informationen zu den Beständen.

-   **Nachweis unterdrückt**. Wenn der Datensatz in dem Discoverysystem unterdrückt werden soll, die Checkbox Nachweis unterdrücken markieren.
-   **Bestands-HRID**. Die Human Readable ID ("Augenlesbare ID"). Eine vom System zugewiesene fortlaufende ID, die der Bestands-ID zugeordnet ist.
-   **Quelle**. Format des Bestandsdatensatzes, wenn ein Quelldatensatz vorhanden ist. Zum Beispiel FOLIO, wenn es sich um einen in Katalog erstellten Datensatz handelt, MARC, wenn es sich um einen in MARCcat erstellten MARC-Datensatz handelt, oder EPKB, wenn es sich um einen Datensatz aus eHoldings handelt.
-   **Frühere Bestands-ID**. Frühere Bestands-ID
-   **Bestandstyp**. Gibt die Art des bibliografischen Formats des Bestandsdatensatzes an. Zum Beispiel, gedruckt oder elektronisch. Konfiguriert in [Einstellungen > Katalog > Bestandstypen](https://info.gbv.de/display/FOLIOGBVEXTERN/Einstellungen+%28Katalog%29%3A+Bestandstypen).
-   **Statistischer Code**. Statistische Codes (z.B. ASER; Name: Active serial; Typ: SERM (Serienverwaltung) oder Bücher; Name: Buch, Druck (Bücher); Typ ARL (Sammlungsstatistik) usw.). Wird in den Einstellungen konfiguriert.

#### Frühere Bestands-ID hinzufügen

1.  Auf **Frühere Bestands-ID hinzufügen** klicken.
2.  Die **Vorherige Bestands-ID** in das Feld eingeben.
3.  Die Schritte 1-2 je nach Bedarf wiederholen. Die ID des früheren Bestandes wird gespeichert, sobald der Bestandsdatensatz gespeichert wird.

#### Statistischen Codes hinzufügen

1.  Auf **Statistischen Code hinzufügen** klicken.
2.  Den statistischen Code aus der Dropdown-Liste auswählen.
3.  Die Schritte 1-2 je nach Bedarf wiederholen. Der statistische Code wird gespeichert, sobald der Bestandsdatensatz gespeichert wird.

#### Löschen einer früheren Bestands-ID oder eines statistischen Codes

1.  Die frühere Bestands-ID oder den statistischen Code suchen, der gelöscht werden soll.
2.  Auf das **Mülleimersymbol** neben der ID oder dem Code klicken. Die ID oder der Code wird aus dem Datensatz entfernt und gelöscht, sobald der Bestandsdatensatz gespeichert wird.

### Standort

Der Abschnitt Standort enthält Informationen über den physischen oder elektronischen Standort des Bestands.

-   **Dauerhafter Standort (erforderlich)**. Der Standardstandort der Ressource, der ein physischer Standort oder ein Online-Standort sein kann, an dem die Ressource gespeichert ist. Der dauerhafte Standort wird auf der Ebene des Bestands zugewiesen, kann aber bei Bedarf auf der Ebene des Exemplars überschrieben werden. Einen Dauerhaften Standort aus der Dropdown-Liste auswählen oder auf Standortsuche klicken, um einen Standort auszuwählen.
-   **Vorläufiger Standort**. Ein Vorläufiger Standort für die Ressource, der ein physischer Standort oder ein Online-Standort sein kann, an dem die Ressource gespeichert ist. Vorläufige Standorte können auf der Ebene der Bestände zugewiesen und bei Bedarf auf der Ebene der Exemplare überschrieben werden. Einen Vorläufigen Standort aus der Dropdown-Liste auswählen oder auf Standortsuche klicken, um einen Standort auszuwählen.
-   **Regalordnung**. Eine vom System generierte Normalisierung der Signatur, die eine Sortierung der Signatur in Berichten und in Suchergebnissen ermöglicht.
-   **Regaltitel**. Beschriftung des Regals.
-   **Exemplarnummer**. Die Exemplarnummer des Bestandes.
-   **Signaturtyp**. Das für die Signatur verwendete Klassifikationssystem. Den **Signaturtyp** aus der Dropdown-Liste wählen. Konfiguriert unter Einstellungen > Katalog > Signaturtypen.
-   **Signatur-Präfix**. Präfix der Signatur auf der Bestandsebene. Zum Beispiel: FIC.
-   **Signatur**. Die Signatur ist eine einem Exemplar zugewiesene Kennung, die normalerweise auf einem am Exemplar angebrachten Etikett steht. Die Signatur wird verwendet, um die physische Position des Exemplars in einer Regalreihenfolge zu bestimmen (z.B. K1 .M44)
-   **Signatur-Suffix**. Suffix der Signatur auf der Bestandsebene. Zum Beispiel das Jahr (2001).

### Details zum Bestand

Der Abschnitt Bestandsdetails enthält zusätzliche Angaben zu den Beständen.

-   **Exemplarzahl**. Anzahl der Exemplare des Bestands
-   **Bestandsangaben**. Gibt den genauen Inhalt an, auf den die Bibliothek Zugriff hat, typischerweise für fortlaufende Publikationen.
-   **Richtlinie zur Fernleihe**. Eine Liste von Werten auswählen, die die Verleihrichtlinien der Bibliothek definieren, die Fernleih-Richtlinien. Zum Beispiel: Wird ausgeliehen, Wird nicht ausgeliehen, Wird vervielfältigt, Wird nicht vervielfältigt, usw. Konfiguriert unter [Einstellungen > Katalog > Fernleihrichtlinien](https://info.gbv.de/display/FOLIOGBVEXTERN/Einstellungen+%28Katalog%29%3A++Fernleihrichtlinien).
-   **Richtlinie zur Digitalisierung**. Anmerkungen zu den Digitalisierungsrichtlinien.
-   **Richtlinie zur Aufbewahrung**. Anmerkungen zu den Aufbewahrungsrichtlinien.

#### Bestandsangaben hinzufügen

1.  Auf **Bestandsangaben hinzufügen** klicken.
2.  Optional: Eine **Bestandsangabe** eingeben.
3.  Optional**:** Eine **Bestandsangabe öffentliche Anmerkung** eingeben. Bibliografische öffentliche Anmerkung, die mit der Bestandsübersicht verknüpft ist.
4.  Optional: Eine **Bestandsangabe interne Anmerkung** eingeben. Bibliografische Anmerkung des Personals, die mit der Bestandsübersicht verknüpft ist.
5.  Die Schritte 1-4 nach Bedarf wiederholen. Der Bestandsangaben wird gespeichert, sobald der Bestandsdatensatz gespeichert wird.

#### Bestandsangabe für Supplemente hinzufügen

Gibt den genauen Inhalt der  Supplemente an, auf die die Bibliothek Zugriff hat, in der Regel für fortlaufende Publikationen.

1.  Auf **Bestandsangabe für Supplemente hinzufügen** klicken.
2.  Optional: Eine **Bestandsangabe für Supplemente** eingeben.
3.  Optional: Eine **Bestandsangabe für Supplemente öffentliche Anmerkung** eingeben.
4.  Optional: Eine **Bestandsangabe für Supplemente interne Anmerkung** eingeben.
5.  Die Schritte 1-4 je nach Bedarf wiederholen. Die Bestandsmitteilung wird gespeichert, sobald der Bestandsdatensatz gespeichert wird.

#### Bestandsangabe für Indizes hinzufügen

Gibt den genauen Inhalt von Indizes an, auf die die Bibliothek Zugriff hat, typischerweise für fortlaufende Publikationen.

1.  Auf **Bestandsangabe für Indizes hinzufügen** klicken.
2.  Optional: Eine **Bestandsangabe für Indizes** eingeben.
3.  Optional: Eine **Bestandsangabe für Indizes öffentliche Anmerkung** eingeben.
4.  Optional: Eine **Bestandsangabe für Indizes interne Anmerkung** eingeben.
5.  Die Schritte 1-4 je nach Bedarf wiederholen. Die Bestandsanweisung wird gespeichert, sobald der Bestandsdatensatz gespeichert wird.

#### Bestandsangabe löschen

1.  Die Bestandsangabe suchen, die gelöscht werden soll.
2.  Auf das **Mülleimersymbol** neben der Bestandsangabe klicken. Die Bestandsangabe wird aus dem Datensatz entfernt und gelöscht, sobald der Bestandsdatensatz gespeichert wird.

### Anmerkungen zum Bestand

Der Abschnitt Anmerkungen zum Bestand enthält alle Anmerkungen zu den Beständen.

#### Anmerkung hinzufügen

1.  Auf **Anmerkung hinzufügen** klicken.
2.  Den Anmerkungstyp aus der Dropdown-Liste auswählen. Konfiguriert unter [Einstellungen > Katalog > Anmerkungstypen der Instanz](https://info.gbv.de/display/FOLIOGBVEXTERN/Einstellungen+%28Katalog%29%3A+Anmerkungstypen+der+Instanz).
3.  Eine **Anmerkung** in das Feld eingeben.
4.  Optional: Wenn die Anmerkung nur für Mitarbeitende sichtbar sein soll, die über die entsprechenden Berechtigungen verfügen, die Checkbox Nur Personal markieren.
5.  Die Schritte 1-4 je nach Bedarf wiederholen. Die Anmerkung wird gespeichert, sobald der Bestandsdatensatz gespeichert wird.

#### Anmerkung entfernen

1.  Die Anmerkung suchen, die gelöscht werden soll.
2.  Auf das **Mülleimersymbol** neben der Anmerkung klicken. Die Anmerkung wird aus dem Datensatz entfernt und gelöscht, sobald der Bestandsdatensatz gespeichert wird.

### Elektronischer Zugang

Im Bereich Elektronischer Zugang können Informationen zum Online-Zugang für die Ressource hinzugefügt werden.

#### Elektronischen Zugang hinzufügen

Anmerkung: Das Hinzufügen eines elektronischen Zugangs ist optional, aber wenn auf **Elektronischen Zugang hinzufügen** geklickt wird, muss ein URI eingeben oder der elektronischen Zugang gelöscht werden, um die Instanz zu speichern.

1.  Auf **Elektronischen Zugang hinzufügen** klicken.
2.  Optional: Eine **Beziehung** aus der Dropdown-Liste auswählen.
3.  Optional: Eine **URI** in das Feld eingeben.
4.  Optional: Einen **Linktext** in das Feld eingeben.
5.  Optional: Die **Aufgeführten Materialien** in das Feld eingeben.
6.  Optional: Eine **URL öffentliche Anmerkung** in das Feld eingeben.
7.  Die Schritte 1-6 je nach Bedarf wiederholen. Der elektronische Zugang wird gespeichert, sobald Sie den Bestandsdatensatz speichern.

#### Elektronischen Zugang löschen

1.  Den elektronischen Zugang suchen, der gelöscht werden soll.
2.  Auf das **Mülleimersymbol** neben dem elektronischen Zugang klicken. Der elektronische Zugang wird aus dem Datensatz entfernt und ist gelöscht, sobald der Bestandsdatensatz gespeichert wird.

### Erwerbung

Der Abschnitt Erwerb enthält Informationen über den Erwerb von Beständen.

-   **Erwerbungsmethode**. Die Methode, mit der der Bestand erworben wurde.
-   **Bestellungsformat**. Das Bestellformat des Bestands. Zum Beispiel: DVD oder Monographie.
-   **Inventarisierungsstatus**. Der Inventarisierungsstatus. Zum Beispiel: Ausstehend, Inventarisierung erwartet, Teilweise inventarisiert, Vollständig inventarisiert, Inventarisierung nicht erforderlich und Storniert.

### Inventarisierungsverlauf

Die Inventarisierung wird für Serien und fortlaufende Ressourcen verwendet. Zeigt die Ressourcen an, die bereits inventarisiert wurden.

#### Inventarisierungsverlauf hinzufügen

1.  Auf **Inventarisierungsverlauf hinzufügen** klicken.
2.  Optional: Wenn der  Inventarisierungsverlauf und die Chronologie öffentlich angezeigt werden sollen, die Checkbox **Öffentliche Anzeige** markieren.
3.  Optional: Die Zählung eingeben.
4.  Optional: Die Chronologie eingeben.
5.  Die Schritte 1-4 nach Bedarf wiederholen. Die Empfangshistorie wird gespeichert, sobald der Bestandsdatensatz gespeichert wird.

 Inventarisierungsverlauf löschen

-   Den  Inventarisierungsverlauf suchen, der gelöscht werden soll.
-   Auf das **Mülleimersymbol** neben dem  Inventarisierungsverlauf klicken. Der  Inventarisierungsverlauf wird aus dem Datensatz entfernt und gelöscht, sobald der Bestandsdatensatz gespeichert wird.
