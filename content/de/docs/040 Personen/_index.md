---
title: "📱 Personen"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [app-personen, by-folio, for-anwender, cat-berechtigungen, meta-uebersetzungsproblem]
weight: 40
Description: "
    Quellen: [Folio](https://docs.folio.org/docs/users/) & [GBV](https://info.gbv.de/pages/viewpage.action?pageId=839188597)
    "
---

Mit der App "Personen" können Sie Benutzerinformationen für Benutzer und Bibliotheksmitarbeiter verwalten. Sowohl die Benutzer als auch die Mitarbeiter der Bibliothek werden in der App "Personen" gespeichert. Es gibt kein separates Verzeichnis oder eine App für Bibliotheksmitarbeiter. Der Unterschied zwischen einem Benutzer des Bibliothekspersonals und einem Bibliotheksnutzendem besteht darin, dass dem Datensatz des Bibliothekspersonals FOLIO-Berechtigungen, ein Benutzername und ein Passwort zugewiesen sind.

Definition von Begriffen im Zusammenhang mit der App Personen:

-   **Person**. Jede Person, die mit FOLIO interagiert oder dort Aufgaben ausführt.
-   **Personen-Datensatz**. Enthält Kontaktinformationen und Identifikatoren für einen einzelnen Personen. Personendatensätze gibt es sowohl für Bibliotheksnutzende als auch für Bibliotheksmitarbeiter. Eine Liste aller Informationen, die in einem Personendatensatz enthalten sind, finden Sie unter [Folio: Personen anzeigen](https://info.gbv.de/display/FOLIOGBVEXTERN/Folio%3A+Personen+anzeigen)..
-   **Berechtigung**. Einer Person zugewiesener Wert, der den Zugriff auf FOLIO-Datensätze gewährt oder es erlaubt, bestimmte Aufgaben in FOLIO auszuführen.
-   **Berechtigungsgruppe**. Eine Gruppe von Berechtigungen, die es einem Person erlaubt, eine bestimmte Gruppe von Aufgaben auszuführen. Sie können zum Beispiel bestimmte Berechtigungen gruppieren, um berufsspezifische Berechtigungsgruppen zu erstellen. Berechtigungsgruppen werden von Ihrer Bibliothek unter [Einstellungen > Personen > Berechtigungsgruppen](https://info.gbv.de/display/FOLIOGBVEXTERN/Einstellungen+%28Personen%29%3A+Berechtigungsgruppen) definiert.

## Berechtigungen

Die unten aufgeführten Berechtigungen ermöglichen die Interaktion mit der Personen-App und bestimmen, was in der App gemacht werden kann und was nicht. Wenn ein Benutzer keine dieser Berechtigungen zugewiesen hat, kann die App "Personen" und alle damit verbundenen Informationen nicht angezeigt werden.

Hinweis: Informationen zum Zuweisen von Berechtigungen an Personen finden Sie unter Zuweisen von Berechtigungen an einen Personendatensatz.

Im Folgenden sind alle Personenberechtigungen aufgeführt:
-   **Benutzerimport - Alle Berechtigungen.** (User import - all permissions)
    Diese Berechtigung erlaubt es der Person, Personendatensätze zu importieren.
-   **Personen: Kann Exemplarsperren umgehen** (User: Can override item blocks)
    Mit dieser Berechtigung kann die Person eine  Exemplarsperre in der Ausleihe außer Kraft setzen.
-   **Personen: Kann Kontosperren umgehen** (User: Can override patron blocks)
    Mit dieser Berechtigung kann die Person eine Sperre für die Ausleihe, Bestandsanfrage oder Verlängerung eines Exemplars in der Ausleihe außer Kraft setzen.
-   **Personen: Kann Personen Berechtigungen zuweisen und entziehen** (Users: Can assign and unassign permissions to users)
    Mit dieser Berechtigung kann die Person einem anderen Personen Berechtigungen zuweisen oder die Zuweisung aufheben.
-   **Personen: Kann Personen Servicestellen zuweisen und entziehen** (Users: Can assign and unassign service points to users)
    Mit dieser Berechtigung kann die Person Servicestellen, die Personen zugewiesen wurden, anzeigen und bearbeiten. Die Person kann auch grundlegende Datenelemente von Personen anzeigen und bearbeiten.
-   **Personen: Kann offene Transaktionen öffnen** (Users: Can check open transactions)
    Diese Berechtigung erlaubt es der Person, den Personendatensatz auf offene Vorgänge zu überprüfen. Wenn keine offenen Vorgänge vorhanden sind, kann der Personendatensatz gelöscht werden.
-   **Personen: Kann eine neue Person anlegen** (Users: Can create new user)
    Diese Berechtigung ermöglicht es der Person, einen neuen Personendatensatz anzulegen und diesem Personendatensatz Personeninformationen, erweiterte Informationen und Kontaktinformationen hinzuzufügen.
-   **Personen: Kann Forderungen erstellen, bearbeiten und entfernen** (Users: Can create, edit and remove fees/fines)
    Mit dieser Berechtigung kann die Person Gebühren/Gebühren erstellen, bearbeiten, entfernen und anzeigen.
-   **Personen: Kann Kontosperren erstellen, bearbeiten und entfernen** (Users: Can create, edit and remove patron blocks)
    Mit dieser Berechtigung kann die Person den Abschnitt Gönnersperren im Personendatensatz sehen und Sperren anzeigen, bearbeiten und erstellen.
-   **Personen: kann Vollmachtnehmer/innen erstellen, bearbeiten und entfernen** (Users: Can create, edit and remove proxies)
    Mit dieser Berechtigung kann die Person die einer Person zugewiesenen Proxys anzeigen und bearbeiten. Die Person kann außerdem grundlegende Datenelemente der Person anzeigen und bearbeiten.
-   **Personen: Kann Konto löschen, wenn die Person keine offenen Transaktionen hat** (Users: Can delete user profile if user does not have any open transactions)
    Mit dieser Berechtigung kann ein Personenprofil über die Benutzeroberfläche gelöscht werden, wenn die Person keine offenen Vorgänge hat. Diese Berechtigung muss zusammen mit Personen verwendet werden: **Personen: Kann offene Transaktionen öffnen**.
-   **Personen: Kann das Konto bearbeiten** (Users: Can edit user profile)
    Mit dieser Berechtigung kann die Person die folgenden Abschnitte in einem Personendatensatz bearbeiten und anzeigen: Benutzerinformationen, Erweiterte Informationen und Kontaktinformationen.
-   **Users: Can process lost items requiring actual cost**. (Users: Can process lost items requiring actual cost)
    Mit dieser Berechtigung kann die Person die Bestellung von verlorenen Exemplaren, für die Istkosten anfallen, verwenden. Tatsächliche Kosten werden in Nolana nicht vollständig implementiert sein. Es wird empfohlen, mit der Verwendung der Istkostenbearbeitung bis Orchid zu warten.
-   **Personen: Kann Forderungen ansehen** (Users: Can view fees/fines and loans)
    Mit dieser Berechtigung können Personen die Gebühren/Gebühren und Ausleihen eines Benutzers einsehen.
-   **Personen: Kann Berechtigungen sehen, die Personen zugewiesen sind** (Users: Can view permissions assigned to users)
    Mit diesem Recht kann die Person die einem anderen Benutzer zugewiesenen Rechte einsehen.
-   **Personen: Kann Bevollmächtigungen sehen, die Personen zugewiesen sind** (Users: Can view proxies assigned to users)
    Mit dieser Berechtigung kann die Person den Abschnitt Proxies sehen, aber keine einem Personen zugewiesenen Proxies bearbeiten. Diese Berechtigung umfasst auch die Möglichkeit, Personendatensätze zu suchen und anzuzeigen (nur grundlegende Benutzerfelder).
-   **Personen: Kann Servicestellen anzeigen, die Personen zugewiesen sind** (Users: Can view service points assigned to users)
    Mit dieser Berechtigung kann die Person den Abschnitt Servicestellen sehen, aber keine Servicestellen bearbeiten, die einem Personen zugewiesen sind. Diese Berechtigung umfasst auch die Möglichkeit, Personendatensätze zu suchen und anzuzeigen (nur grundlegende Personenfelder).
-   **Personen: Kann das Konto ansehen** (Users: Can view user profile)
    Mit dieser Berechtigung kann die Person nach Personendatensätzen suchen und die folgenden Abschnitte eines Personendatensatzes anzeigen: Benutzerinformationen, Erweiterte Informationen und Kontaktinformationen.
-   **Personen: Bericht zum Kassenabschluss erstellen und herunterladen** (Users: Create and download Cash drawer reconciliation report)
    Mit dieser Berechtigung kann die Person einen Kassenladenabstimmungsbericht erstellen und herunterladen.
-   **Personen: Bericht "Finanztransaktionen" erstellen und herunterladen** (Users: Create and download Financial transaction detail report)
    Personen: Detailbericht zu Finanzvorgängen erstellen und herunterladen. Mit dieser Berechtigung kann die Person einen Detailbericht zu Finanzvorgängen erstellen und herunterladen.
-   **Personen: Erstellen und Herunterladen von Erstattungsberichten zur manuellen Bearbeitung** (Users: Create and download Refunds to process manually report)
    Mit dieser Berechtigung können Personen einen Bericht über manuell zu bearbeitende Rückerstattungen erstellen und herunterladen.
-   **Personen: Passwort erstellen/zurücksetzen** (Users: Create/reset password)
    Mit dieser Berechtigung kann die Person eine E-Mail zum Zurücksetzen des Kennworts an eine Person senden oder den Link zum Zurücksetzen des Kennworts kopieren, um ihn mit einer Person zu teilen, die die Funktion zum Zurücksetzen des Kennworts nutzt.
-   **Personen: Ausleihen anonymisieren** (Users: User loans anonymize)
    Mit dieser Berechtigung kann die Person alle Angaben zu Personen aus einer Ausleihe entfernen.
-   **Personen: Fälligkeitsdatum bei Ausleihen ändern** (Users: User loans change due date)
    Diese Berechtigung erlaubt es der Person, das Fälligkeitsdatum einer Ausleihe im Datensatz einer anderen Person zu ändern.
-   **Personen: Ausleihen für angeblich zurückgegeben erklären** (Users: User loans claim returned)
    Mit dieser Berechtigung kann die Person den Status von ausgeliehenen Exemplaren in angeblich zurückgegeben ändern.
-   **Personen: Ausleihen für verloren erklären** (Users: User loans declare lost)
    Mit dieser Berechtigung kann die Person den Status der ausgeliehenen Exemplare in Verloren erklärt ändern.
-   **Users: User loans mark claimed returned missing**. (Users: User loans mark claimed returned missing)
    Diese Berechtigung erlaubt es Personen, den Status von Ausleihen auf angeblich zurückgegebenen zu ändern.
-   **Personen: Ausleihen verlängern** (Users: User loans renew)
    Mit dieser Berechtigung kann die Person Ausleihen verlängern, soweit es die Ausleihrichtlinie zulässt.
-   **Personen: Ausleihen mit spezieller Zustimmung verlängern** (Users: User loans renew through override)
    Diese Berechtigung erlaubt es der Person, fehlgeschlagene Verlängerungen zu übersteuern.
-   **Personen: Ausleihen anzeigen** (Users: User loans view)
    Diese Berechtigung erlaubt es der Person, die Rubrik Ausleihen in einem Personendatensatz, die Bestellung und die Ausleihdetails einzusehen.
-   **Personen: Ausleihen ansehen, bearbeiten, alle verlängern** (Users: User loans view, change due date, renew)
    Mit dieser Berechtigung kann die Person die Rubrik Ausleihen in einem Personendatensatz anzeigen, das Fälligkeitsdatum einer Ausleihe ändern und Ausleihen verlängern.
-   **Personen: Bestandsanfragen anzeigen** (Users: View requests)
    Mit dieser Berechtigung kann die Person den Abschnitt Bestandsanfragen in einem Personendatensatz anzeigen. Diese Berechtigung umfasst auch die Möglichkeit, Personendatensätze zu suchen und anzuzeigen (nur grundlegende Benutzerfelder).
