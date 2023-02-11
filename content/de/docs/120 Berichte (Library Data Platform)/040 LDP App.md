---
title: "📱LDP App"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [app-ldp, by-folio, cat-berechtigungen, cat-einstellungen, for-admin, meta-uebersetzungsproblem]
weight: 40
Description: "
    Quellen: [Folio](https://docs.folio.org/docs/reporting/ldp-app/) & [GBV](https://info.gbv.de/pages/viewpage.action?pageId=839188652)
    "
---

Die LDP App bietet ein FOLIO Interface für die Interaktion mit einer LDP Datenbank. Die App besteht aus zwei Teilen: dem Abfragegenerator und den gespeicherten Abfragen. Mit dem Abfragegenerator können Abfragen erstellt und für eine spätere Verwendung gespeichert werden. Mit Gespeicherte Abfragen können frühere Abfrage in den Abfragegenerator geladen werden, um sie zu bearbeiten oder auszuführen.

## Berechtigungen

Mit den unten aufgeführten Berechtigungen werden Personen Berechtigungen für die Interaktion mit der LDP App erteilt. Personen können in der App Personen Berechtigungen zugewiesen werden. Wenn einer Person keine dieser Berechtigungen zugewiesen ist, kann sie die LDP App oder damit verbundene Informationen nicht sehen.

Im Folgenden sind alle Berechtigungen für die LDP-App zu finden:

-   **UI: LDP-Modul ist aktiviert**. (UI: LDP module is enabled)
    Ermöglicht es der Person, die App zu sehen und den Abfragegenerator und die Gespeicherten Abfragen zu verwenden.
-   **LDP: alle Berechtigungen**. (LDP: All permissions)
    Diese Berechtigung erlaubt es der Person, die LDP App zu sehen und zu verwenden.
-   **Einstellungen (LDP): Kann die Einstellungen sehen**. (Settings (LDP): Can view settings)
-   **Einstellungen (LDP): Kann die Verbindungsdetails der LDP-Datenbank ändern**. (Settings (LDP): Can modify LDP database connection details)
-   **Einstellungen (LDP): Kann Standarddatensatzlimits ändern**. (Settings (LDP): Can modify default record limits)
-   **Einstellungen (LDP): Kann Konfigurationsdetails für gespeicherte Abfragen ändern**. (Settings (LDP): Can modify saved-query configuration details)
-   **Einstellungen (LDP): Kann auswählen, welche Tabellen für die Suche verfügbar sind**. (Settings (LDP): Can select which tables are available to search)

### Schema

Schemata können sich als die "Behälter" vorgestellt werden, in denen sich die Datentabellen befinden. Im Dropdown-Menü Schema kann jeweils ein Schema ausgewählt werden, das in einer Abfrage verwendet werden soll. Es stehen drei Schemata zur Verfügung: public, folio\_reporting und local. Eine ausführlichere Erklärung der Schemas und Beispiele für einige der enthaltenen Standardeinstellungen sind unter [Library Data Platform - Using schemas](https://docs.folio.org/docs/reporting/library-data-platform/#using-schemas) zu finden.

### Tabelle

Über das Dropdown-Menü Tabelle kann eine Datentabelle aus dem von gewählten Schema ausgewählt werden, die in einer Abfrage verwendet werden soll. Tabellen sind der Ort, an dem verwandte Daten gespeichert werden. Tabellen gehören zu einem bestimmten Schema. Wenn das Schema und die Tabelle ausgewählt wurden, werden die anderen Felder freigeschaltet und je nach Auswahl aktualisiert.

## Nach Spalte filtern

Mit dem Dropdown-Menü Nach Spalte filtern können die Ergebnisse verfeinert werden, indem eine Spalte ausgewählt und Beschränkungen angewendet werden. Es können mehrere Filter erstellt werden, indem die Schaltfläche Filter hinzufügen verwendet wird. Wenn mehrere Filter verwendet werden, werden die Ergebnisse mit dem Operator AND verknüpft. Sobald eine Spalte zum Filtern ausgewählt wurde, können Gleichheits- und Ungleichheitsoperationen in Kombination mit einem numerischen Wert (z.B. einem Datum oder einer Anzahl), TRUE oder FALSE ausgewählt werden. Die Operatoren umfassen:

-   gleich (=)
-   nicht gleich (<>)
-   kleiner als (<)
-   kleiner als oder gleich (<=)
-   größer als (>)
-   größer als oder gleich (>=)
-   WARH (Groß-/Kleinschreibung wird nicht beachtet)
-   FALSCH (Groß-/Kleinschreibung wird nicht beachtet)

Hier sind einige Beispiele für die Filterung nach Spalten:

-   find where previously\_held = TRUE
-   find where \_version > 1

Bei der Eingabe von Datumsbereichen werden sowohl YYYY-MM-DD als auch MM/DD/YYYY unterstützt. Die Operatoren LIKE und ILIKE, die einen Musterabgleich innerhalb zeichenbasierter Spaltendaten ermöglichen, werden in einer zukünftigen Version enthalten sein. Bei LIKE wird die Groß-/Kleinschreibung beachtet, während bei ILIKE die Groß-/Kleinschreibung keine Rolle spielt.

### Spalten anzeigen

Über das Dropdown-Menü **Spalten anzeigen** können ein oder mehrere Felder aus dem Schema und der Tabelle ausgewählt werden, die in den Abfrageergebnissen angezeigt werden sollen. Standardmäßig werden alle Spalten angezeigt. Die Liste der Spalten, die einbeziehen werden sollen, wird aufgebaut, wenn die einzelnen Spalten aus dem Dropdown-Menü ausgewählt werden.

Um die Liste einzuschränken, einfach auf das Dropdown-Menü **Spalten anzeigen** klicken und auf die aufgeführten Felder klicken. Um hinzugefügte Felder zu entfernen, kann entweder auf das **x** neben dem Feldnamen im Feld geklickt werden oder in der Dropdown-Liste erneut auf das Feld geklickt werden, um es abzuwählen.

### Nach Spalte sortieren

Es kann auf die Schaltfläche **Sortierkriterium hinzufügen** geklickt werden, um eine oder mehrere Spalten hinzuzufügen, nach denen die Ergebnisse geordnet werden sollen. Optionen wie **Aufsteigend** im nächsten Feld rechts erscheinen in einem Dropdown-Menü, das mit zusätzlichen Optionen wie **Nullen am Ende** im dritten Feld rechts kombiniert werden können. Wenn nach mehreren Spalten sortiert werden soll, kann erneut auf die Schaltfläche **Sortierkriterium hinzufügen** geklickt werden. Um eine Spaltensortierung zu entfernen, auf das **Mülleimersymbol** klicken.

### Anzahl der Ergebnisse begrenzen

Mit dem Dropdown-Menü Anzahl der Ergebnisse begrenzen kann die Anzahl der Zeilen, die in den Abfrageergebnissen zurückgegeben werden, auf 1, 10, 100 oder 1000 beschränkt werden. Dies ist nützlich, wenn nur einen Ausschnitt der gesamten Ergebnismenge angezeigt werden soll, insbesondere wenn erwartet wird, dass die Anzahl der zurückgegebenen Zeilen sehr groß ist.

### Speichersymbol

Mit dem Speichersymbol  oben rechts im Abfragegenerator können Abfragen gespeichert werden, nachdem sie erstellt wurden. Nach dem Speichern werden die Abfragen in der Liste im Abschnitt Gespeicherte Abfragen der LDP App angezeigt.

### Gespeicherte Abfragen

Im Abschnitt **Gespeicherte Abfragen** der LDP-App werden Abfragen aufgelistet, die von Personen gespeichert wurden, die auf das Speichersymbol im Abschnitt **Abfrageerstellung** der LDP-App geklickt haben. Jeder, der Zugriff auf die LDP-App hat, kann auf die Abfragen in der Liste Gespeicherte Abfragen klicken und sie ausführen. Abfragen können aus dieser Liste entfernt werden, indem auf das **Mülleimersymbol** neben der einzelnen Abfrage am rechten Ende der Liste geklickt wird.

## Was in der App Einstellungen geändert werden kann

Die App Einstellungen kann verwendet werden, um globale Einstellungen für die LDP-App zu konfigurieren. Um zu den LDP-Einstellungen zu gelangen, im Menü Apps die Option Einstellungen und dann LDP wählen.

### Datensatzlimits

Mit der Einstellung **Datensatzlimits** kann die Standard- und Höchstzahl der Datensätze festlegt werden, die in den Abfrageergebnissen einer Person angezeigt werden sollen. Es kann auch die Anzahl der Datensätze einschränkt werden, die eine Person exportieren kann, indem die Einstellung **Maximal zu exportierende Anzahl** verwendet wird.

-   Standardmäßig anzuzeigende Anzahl
-   Maximal anzuzeigende Anzahl
-   Maximal zu exportierende Anzahl

### Verfügbarkeit von Tabellen

Die Einstellung Verfügbarkeit von Tabellen

-   zeigt das Schema und die Tabellen in der verbundenen Datenbank an und ermöglicht es, die Abfrage von Tabellen zu deaktivieren, so dass Personen sie nicht in Abfragen einbeziehen können. Dies ist nützlich für Tabellen, die möglicherweise beschränkte Daten enthalten, wie z.B. PII (Personally Identifiable Information).
**Derzeit zur Deaktivierung empfohlen: Es wird derzeit empfohlen, folgende Tabellen zu deaktivieren: srs\_marc, srs\_marctab, srs\_records. Derzeit unterstützt die App die Indizierung bestimmter Spalten nicht. Wenn sie aktiviert gelassen wird, kann dies zu Leistungsproblemen und zusätzlicher Belastung der Datenbank führen.**

### Datenbankkonfiguration

Die Einstellung **Datenbankkonfiguration** wird verwendet, um die Verbindung von der FOLIO-Anwendungsinstanz zur LDP-Berichtsdatenbankinstanz festzulegen. Hier werden auch die Kennung und das Passwort festgelegt, die von der LDP App für die Abfrage der LDP Berichtsdatenbank verwendet werden sollen.

### Konfiguration gespeicherter Abfragen (experimentelle Funktion)

Mit der Konfigurationseinstellung Gespeicherte Abfragen kann einen Standort für ein GitHub-Repository für die Abfragen konfiguriert werden, in das die Personen speichern, wenn sie das Speichersymbol verwenden, um Abfragen zu speichern, die sie mit dem  Abfragegenerator erstellt haben. Der Besitzer des GitHub-Repository, der Repository-Name, der Branch und das OAuth-Token für den Zugriff auf das Repository müssen hier angegeben werden.
