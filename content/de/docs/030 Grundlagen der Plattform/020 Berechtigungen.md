---
title: "Berechtigungen"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [app-personen, by-folio, for-admin, cat-berechtigungen]
weight: 20
Description: "
    Quellen: [Folio](https://docs.folio.org/docs/platform-essentials/permissions/) <!-- & [GBV](https://info.gebev.de/display/FOLIOGBVEXTERN/Berechtigungen) -->
    "
---

{{% pageinfo %}}
Siehe auch

* [FOLIO Wiki: Guides to FOLIO Permissions](https://wiki.folio.org/display/FOLIOtips/Guides+to+FOLIO+Permissions)
* [Folio: Person Rechte zuweisen]({{< ref "080 Person Rechte zuweisen" >}})
* [Folio: Person Rechte entziehen]({{< ref "090 Person Rechte entziehen" >}})
{{% /pageinfo %}}

FOLIO verfügt über ein System von Benutzerrechten, mit dem sich genau steuern lässt, worauf Benutzer in FOLIO zugreifen können.

Jede App definiert ihre eigenen Berechtigungen für die Frontend- und Backend-Module, die sie verwendet.

Standardmäßig bietet eine FOLIO-Installation keine Rollen oder Berechtigungen für Bibliotheksmitarbeiter. Stattdessen können FOLIO-Administratoren eigene Gruppen von Berechtigungen, sogenannte **Berechtigungsgruppen**, erstellen, die ihren lokalen Anforderungen entsprechen. Diese Berechtigungsgruppen können sie dann den Benutzern über die App Personen zuweisen.

## Was ist eine Berechtigung?

Eine Berechtigung ist ein Objekt in FOLIO, das verwendet werden kann, um den Zugriff auf FOLIO-Apps, -Workflows und -Daten zu steuern.

Eine Berechtigung kann eine Reihe verschiedener Attribute haben, je nachdem, ob Sie die Berechtigung im FOLIO-Code betrachten oder ob Sie die Berechtigungen für einen Benutzer in einem FOLIO-Mandanten betrachten. Attribute können sein:

* **permissionName**. Dies ist der eindeutige Name der Berechtigung.
* **displayName**. Dies ist ein von Menschen lesbarer Name für die Berechtigung, der in der Regel dem Namen entspricht, der in der Benutzeroberfläche angezeigt wird. Zu beachten ist, dass es sich bei der Anzeige in der FOLIO-Benutzeroberfläche um eine übersetzte Bezeichnung für den Berechtigungsnamen handelt; die Übersetzungen werden für die unterstützten Sprachen in jedem FOLIO-Modul gespeichert. Der displayName wurde in früheren Versionen von FOLIO verwendet, erfüllt aber in der FOLIO-Benutzeroberfläche keinen Zweck mehr.
* **id**. Die id ist ein eindeutiger Bezeichner für die Berechtigung auf Mandantenebene, der erstellt wird, wenn das entsprechende FOLIO-Modul installiert wird.
* **Description**. Eine Beschreibung der Berechtigung, wie sie vom Entwickler bereitgestellt wurde. Dieses Feld ist optional.
* **subPermissions**. Viele Berechtigungen sind eigentlich eine Gruppierung von spezifischeren Berechtigungen - wenn dies der Fall ist, werden diese spezifischeren Berechtigungen unter subPermissions aufgeführt.
* **childOf**. Wenn eine Berechtigung eine Unterberechtigung für eine andere Berechtigung ist, wird diese "übergeordnete" (=parent) Berechtigung aufgelistet.
* **grantedTo**. Wenn die Berechtigung einem FOLIO-Benutzer erteilt wurde, wird dessen Benutzer-ID für die Berechtigung aufgelistet.
* **mutable**. Eine Berechtigung kann entweder veränderbar oder unveränderbar sein; standardmäßig sind Berechtigungen unveränderbar. Wenn eine Berechtigung als "mutable" : false definiert ist, kann sie nicht geändert werden, ohne den zugehörigen Modulcode zu ändern und das Modul neu zu starten. Wenn eine Berechtigung als "mutable" : true definiert ist, kann sie in der Benutzeroberfläche geändert werden, ohne dass das zugehörige Modul angehalten und neu gestartet werden muss.
* **visible**. Eine Berechtigung kann entweder sichtbar oder unsichtbar sein. Standardmäßig ist eine Berechtigung unsichtbar. Wenn eine Berechtigung als "visible" : true definiert ist, dann ist sie in der FOLIO-Benutzeroberfläche sichtbar. Wenn eine Berechtigung als "visible" : false definiert ist, dann ist sie standardmäßig in der FOLIO-Benutzeroberfläche nicht sichtbar.
* deprecated **moduleName** und **moduleVersion**. Diese Felder erscheinen nur, wenn man sich eine FOLIO-Installation direkt ansieht, sie sind nicht im Code enthalten. Diese Felder geben Auskunft darüber, welches Modul die Berechtigungsdefinition bereitgestellt hat und welche Version dieses Moduls läuft.

## Namenskonvention

Berechtigungen werden benannt, um anzugeben, was ein FOLIO-Benutzer mit dieser Berechtigung innerhalb der App tun kann.

Berechtigungsnamen folgen im Allgemeinen einem von zwei Formaten:

1.  \[Appname\]: \[Was der Benutzer tun kann\]
2.  Einstellungen (\[Bereich der Einstellungen oder Appname\]): \[Was der Benutzer tun kann\]

### Beispiele

* Vereinbarungen: Vereinbarungen bearbeiten
    * Mit dieser Berechtigung können FOLIO-Benutzer Datensätze von Vereinbarungen in der App für Vereinbarungen bearbeiten.
* Einstellungen (Katalog): Materialarten erstellen, bearbeiten, löschen
    * Mit dieser Berechtigung können FOLIO-Benutzer auf die Einstellungen im Katalog zugreifen und Materialarten hinzufügen, ändern oder löschen.

## Schlüsselbegriffe

* **Gruppenberechtigung**. Eine Gruppenberechtigung in FOLIO besteht aus einer oder mehreren Unterberechtigungen.
    * Gruppenberechtigungen können im FOLIO-System von einem Entwickler erstellt werden.
    * Gruppenberechtigungen können auch von einzelnen Bibliotheken unter Einstellungen → Personen erstellt werden.
* **CRUD**. CRUD steht für "Erstellen, Lesen, Aktualisieren und Löschen" (Create, Read, Update and Delete). In Diskussionen über Berechtigungen wird dieser Begriff oft als Abkürzung verwendet. Die meisten FOLIO-Berechtigungen erlauben "CRUD"-Funktionalität - sie geben die Möglichkeit, FOLIO-Datensätze zu erstellen, zu lesen, zu aktualisieren und/oder zu löschen.
    * Eine Berechtigung, die den Zugriff auf das Erstellen, Aktualisieren oder Löschen eines Datensatzes erlaubt, beinhaltet in der Regel auch die Möglichkeit, den Datensatz anzusehen. Zum Beispiel beinhaltet die Berechtigung "Benutzer: Kann Benutzerprofil bearbeiten" eine Unterberechtigung für die Anzeige von Benutzerprofilen enthalten. Sie müssen einem FOLIO-Benutzer nicht beide Berechtigungen erteilen, um das Anzeigen und Bearbeiten von Benutzerdatensätzen zu ermöglichen.
* **Sichtbare Berechtigung**. Eine sichtbare Berechtigung ist eine Berechtigung, die Sie in der Liste der Berechtigungen in der Benutzeroberfläche sehen können. Sie können Benutzern direkt zugewiesen werden und/oder Sie können sie einer Gruppenberechtigung über Einstellungen → Personen → Allgemein → Gruppenberechtigungen hinzufügen.
* **Unsichtbare Berechtigung**: Eine unsichtbare Berechtigung ist in der FOLIO-Benutzeroberfläche verborgen und wird normalerweise nicht direkt einem FOLIO-Benutzer zugewiesen. Unsichtbare Berechtigungen sind in der Regel Teil eines Backend-Moduls. Sie bieten einen sehr spezifischen, begrenzten Zugriff auf Funktionen in FOLIO.

## Allgemeine Workflows

Gängige Berechtigungs-Workflows umfassen:

* Folio: Zuweisung von Berechtigungen und Berechtigungsgruppen zu einem Benutzerdatensatz
* Folio: Eigene Berechtigungsgruppen erstellen

## Sichtbare versus unsichtbare Berechtigungen

FOLIO-Berechtigungen können entweder "sichtbar" oder "unsichtbar" sein.

Berechtigungen, die Sie in der App Personen oder unter Einstellungen > Personen > Berechtigungsgruppen sehen, sind sichtbare Berechtigungen. Entwickler erstellen sichtbare Berechtigungen, indem sie eine Reihe sehr granularer, spezifischer Berechtigungen definieren, die in ihrer Gesamtheit eine bestimmte Funktion erfüllen. Sie haben einen aussagekräftigen Anzeigenamen, der erklärt, was ein FOLIO-Benutzer mit der Berechtigung tun kann.

Unsichtbare Berechtigungen erscheinen nicht standardmäßig in der Personen App. Sie werden von Entwicklern in einem Backend-Modul erstellt und sind nicht dazu gedacht, Benutzern direkt zugewiesen zu werden. In der Regel sind sie sehr granular und steuern eine bestimmte Aktion - zum Beispiel die Möglichkeit, einen bestimmten Typ von Datensätzen in einer App anzuzeigen. Sie haben weniger benutzerfreundliche Anzeigenamen wie "addresstypes collection get".

### Warum sollte ich etwas über unsichtbare Berechtigungen wissen wollen?

Wenn Sie in FOLIO arbeiten, müssen Sie sich im Idealfall nie mit unsichtbaren Berechtigungen befassen, da der Entwicklungsprozess zur Erstellung sichtbarer Berechtigungen geführt hat, die alle von Ihnen benötigten Funktionen bieten.

Gelegentlich treten jedoch Fehler bei den Berechtigungen auf, oder eine Funktion ist nur teilweise entwickelt. In diesem Fall müssen FOLIO-Administratoren möglicherweise einem Benutzer direkt eine unsichtbare Berechtigung zuweisen, um einen benötigten Workflow zu aktivieren.

### Wie kann ich unsichtbare Berechtigungen in der FOLIO Benutzeroberfläche sehen?

Die Möglichkeit, unsichtbare Berechtigungen zu sehen, wird von Benutzer zu Benutzer festgelegt. Der eingeloggte Benutzer muss Zugriff auf Einstellungen → Entwickler haben.

1.  Gehen Sie zu Einstellungen > Entwickler > Konfiguration.
2.  Aktivieren Sie das Kontrollkästchen "Unsichtbare" Berechtigungen in den Menüs für Zusatzberechtigungen auflisten?
3.  Speichern Sie Ihre Änderungen.

Es wird nicht empfohlen, diese Einstellung dauerhaft zu aktivieren; es gibt Tausende von Berechtigungen in FOLIO, wenn man sichtbare und unsichtbare Berechtigungen zusammenzählt, und die Anzeige unsichtbarer Berechtigungen verlangsamt die Arbeitsabläufe der Berechtigungsverwaltung erheblich.

### Wie sollte ich FOLIO für die Verwendung von unsichtbare Berechtigungen konfigurieren, wenn ich in der Lage sein muss, sie an Mitarbeitende zu vergeben?

Sie sollten Berechtigungsgruppen verwenden.

Der allgemeine Ansatz ist:

Melden Sie sich als Benutzer mit entsprechenden Berechtigungen an und aktivieren Sie die Auflistung unsichtbarer Berechtigungen in FOLIO.
Gehen Sie zu Einstellungen>Personen> Berechtigungsgruppen und erstellen Sie eine neue Berechtigungsgruppe mit nur den unsichtbaren Berechtigungen, die Sie zuweisen können müssen.
Deaktivieren Sie die Möglichkeit, unsichtbare Berechtigungen zu sehen.
Weisen Sie die von Ihnen erstellte Berechtigungsgruppe den Benutzern zu, die die unsichtbare Berechtigung benötigen.

Der Grund, warum dieses Verfahren verwendet werden sollte, anstatt sich einfach als entsprechender Administrator anzumelden und den Mitarbeitern die unsichtbare Berechtigung zuzuweisen, ist, dass andere Benutzer nach der Zuweisung der unsichtbaren Berechtigung das Konto des Mitarbeiters bearbeiten und die Änderungen des Administrators überschreiben könnten.

Ein Beispiel:

Angenommen, Jameca Jones, ein FOLIO-Administratorin, beschließt, dass Jeanne Dupont, ein FOLIO-Benutzer, die unsichtbare Berechtigung "circulation-rules.storage.get" benötigt, um bei der Behebung von Lieferproblemen in FOLIO zu helfen.

1.  Jameca meldet sich bei FOLIO an und aktiviert die unsichtbare Berechtigungsoption unter Einstellungen > Entwickler.
2.  Jameca geht zur Personen App und findet Jeannes Profil.
3.  Jameca weist Jeanne die unsichtbare Berechtigung zu und speichert ihre Änderungen.
4.  Jameca deaktiviert die Option für die unsichtbare Berechtigung.

Ein paar Tage später stellt Max Mustermann fest, dass Jeanne die sichtbare Berechtigung "Kurse: Alle lesen" benötigt. Max ist ein Manager, aber kein FOLIO-Administrator.

1.  Max geht in die Personen und sieht sich Jeannes Eintrag an.
2.  Wenn Max Jeannes Konto anschaut, sieht er die Berechtigung "circulation-rules.storage.get" auf Jeannes Konto nicht, weil diese Option für sein Konto in den Einstellungen nicht aktiviert ist.
3.  Max fügt die Berechtigung "Kurse: Alle lesen" hinzu und speichert seine Änderungen.

Wenn Max den Datensatz von Jeanne speichert, speichert FOLIO eine komplett neue Kopie von Jeannes Berechtigungen, **die nur die Berechtigungen enthält, die Max einsehen konnte,** wodurch die von Jameca vorgenommenen Änderungen überschrieben werden.

Nehmen wir dagegen an, dass Jameca Berechtigungsgruppen verwendet, um Jeanne Zugriff zu gewähren.

1.  Jameca geht zu Einstellungen > Entwickler und aktiviert unsichtbare Berechtigungen.
2.  Sie geht zu Einstellungen > Personen > Berechtigungsgruppen und erstellt eine Berechtigungsgruppe mit dem Namen "Fehlerbehebung - Ausleihregelberechtigungen".
3.  Jameca fügt die unsichtbare Berechtigung "circulation-rules.storage.get" zu der von ihr erstellten Berechtigungsgruppe hinzu und speichert ihre Änderungen.
4.  Jameca geht in die App "Personen", sucht Jeannes Datensatz und weist Jeanne die Berechtigungsgruppe "Fehlerbehebung - Ausleihregelberechtigungen" zu.

Ein paar Tage später stellt Max fest, dass Jeanne auch die Berechtigung "Kurse: Alle lesen" benötigt.

1.  Max geht zur App "Personen" und sieht sich Jeannes Eintrag an.
2.  Max weiß nicht, wozu die Berechtigung "Fehlerbehebung - Ausleihregelberechtigungen" dient, aber er weiß, dass Administratoren Berechtigungsgruppen zur Fehlerbehebung verwenden, und lässt sie Jeanne zugewiesen.
3.  Max fügt die Berechtigung "Kurse: Alle lesen" zu Jeannes Konto hinzu und speichert seine Änderungen.

Wenn Max seine Änderungen speichert, speichert FOLIO eine völlig neue Kopie von Jeannes Berechtigungen, die **immer noch** nur die Berechtigungen enthält, die Max einsehen konnte. Da Max jedoch **die von Jameca erstellte Berechtigungsgruppe sehen konnte,** wird sie erneut in Jeannes Konto gespeichert, und sie verliert nicht den Zugriff, den sie benötigt.
