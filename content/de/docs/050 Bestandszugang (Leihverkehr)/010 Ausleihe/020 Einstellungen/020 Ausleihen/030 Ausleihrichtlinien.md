---
title: "Ausleihrichtlinien"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [by-folio, for-admin, cat-einstellungen, app-ausleihe]
weight: 30
Description: "
    Quellen: [Folio](https://docs.folio.org/docs/settings/settings_circulation/settings_circulation/#settings--circulation--loan-policies) & [GBV](https://info.gbv.de/display/FOLIOGBVEXTERN/Einstellungen+(Ausleihe):+Ausleihrichtlinien)
    "
---

Die Ausleihrichtlinien bestimmen, wie ein Exemplar behandelt wird, wenn es ausgeliehen, verlängert oder angefordert wird. Ausleihrichtlinien umfassen eine Vielzahl von Konfigurationsoptionen und werden in den Ausleihregeln verwendet.

Das Verhalten der Ausleihrichtlinien hängt von der Zeiteinheit ab, die für die Leihfrist verwendet wird. Wenn ein Exemplar für Minuten oder Stunden ausgeliehen wird, gilt die Ausleihe als "Kurzausleihe". Wird ein Exemplar für Tage, Wochen oder Monate ausgeliehen, gilt die Ausleihe als "langfristige Ausleihe".

## Überlegungen zur Umsetzung

Es kann von Hilfreich sein, die derzeitigen Ausleihrichtlinien und Ausleihregeln zu prüfen und Richtlinien zu erstellen, die das typische Ausleihverhalten der Bibliothek widerspiegeln. Ausleihrichtlinien sind in Ausleihregeln wiederverwendbar, so dass nicht mehrere Richtlinien desselben Typs erstellt werden müssen, um sie z. B. auf verschiedene Personengruppen anzuwenden.

Bevor mit der Konfiguration der Ausleihrichtlinien begonnen wird, sollte sichergestellt sein, dass Zeitpläne für feste Fälligkeitstermine eingerichtet sind, wenn Zeitpläne in den Richtlinien verwendet werden.

Nachdem die Ausleihrichtlinien erstellt wurden, sollten sie getestet werden, um sicherzustellen, dass sie wie erwartet funktionieren.

## Ausleihrichtlinie erstellen

1.  In der Ansicht **Ausleihrichtlinien** auf **Neu** klicken.
2.  Im Fenster **Ausleihrichtlinie erstellen** einen **Name der Ausleihrichtlinie** in das Feld eingeben.
3.  Optional: In das Feld eine **Beschreibung** der Richtlinie eingeben.
4.  Die Informationen in den folgenden Abschnitten nutzen, um sich bei der Erstellung von Ausleihrichtlinien zu orientieren. Je nachdem, welche Optionen in der Richtlinie ausgewählt sind, sind unterschiedliche Felder verfügbar.
5.  Auf **Speichern und schließen** klicken. Die Richtlinie wird gespeichert und zur Liste der Ausleihrichtlinien hinzugefügt.

### Ausleihen

**Ausleihbar**. Um eine Ausleihrichtlinie zu erstellen, die nicht ausleihbar ist, die Checkbox deaktivieren. Wird die Checkbox deaktiviert, werden alle anderen Felder ausgeblendet. Da Ausleihrichtlinien wiederverwendbar sind, muss nur eine einzige nicht -Ausleihbar-Richtlinie erstellt werden.

**Ausleihprofil**. Die Art des Ausleihprofils wählen. Je nach Auswahl werden unterschiedliche Felder angezeigt.

-   **Festgelegt** wählen, wenn Exemplare, die während eines bestimmten Zeitraums ausgeliehen werden, ein festes Enddatum haben sollen. Dies ist zum Beispiel für Exemplare zu verwenden, die bis zum Ende des Semesters ausgeliehen werden.
-   **Rollend** wählen, wenn die Ausleihe für einen bestimmten Zeitraum erfolgt, einschließlich Kurzausleihen. Diese Option z. B. für Exemplare verwenden, die für 28 Tage ausgeliehen werden.

Je nachdem, welches Ausleihprofil gewählt wurde, werden unterschiedliche Felder angezeigt.

Wurde **Festgelegt** gewählt, werden die folgenden Felder angezeigt:

**Fester Fälligkeitszeitplan (Fälligkeitsbegrenzung)**. Einen festen Fälligkeitsplan wählen, wie unter [Einstellungen > Ausleihe > Feste Fälligkeitspläne](https://info.gbv.de/pages/viewpage.action?pageId=844267627) konfiguriert. Der ausgewählte Zeitplan bestimmt das Fälligkeitsdatum für das Exemplar. Anmerkung: Feste Fälligkeitszeitpläne gelten nur für Ausleihen, die länger als 24 Stunden dauern, und das Fälligkeitsdatum/die Fälligkeitszeit wird automatisch auf 23:59 Uhr am Fälligkeitstag gesetzt.

**Verwaltung des Fälligkeitsdatums bei geschlossenen Öffnungszeiten**. Legt fest, wann das Exemplar fällig ist, wenn das berechnete Fälligkeitsdatum eines Exemplars in die Schließungszeit der Servicestelle fällt.

-   Wenn das Ausleihintervall eines Exemplars in Minuten oder Stunden angegeben ist, richtet sich das Fälligkeitsdatum nach der in der Ausleihrichtlinie angegebenen Auswahl.
-   Wenn das Ausleihintervall eines Exemplars in Tagen, Wochen oder Monaten angegeben ist, richtet sich das Fälligkeitsdatum nur dann nach der Ausleihrichtlinie, wenn die Servicestelle an dem Tag, an dem das Exemplar fällig wäre, vollständig geschlossen ist. Bei der Erstellung der Ausleihe prüft FOLIO den [Kalender](https://info.gbv.de/pages/viewpage.action?pageId=844890129) der Servicestelle; ist die Servicestelle an dem Tag, an dem das Exemplar fällig ist, zu einem beliebigen Zeitpunkt geöffnet, setzt FOLIO den Fälligkeitszeitpunkt auf 23:59 Uhr an diesem Tag.

Kulanzfrist. Eine Schonfrist für überfällige Exemplare eingeben. Wenn eine Kulanzfrist gewählt wird, ist das Exemplar erst nach dem Fälligkeitsdatum/der Fälligkeitszeit der Ausleihe plus der Kulanzfrist überfällig. Wenn die Kulanzfrist abläuft und das Exemplar nicht zurückgegeben wurde, wird die Kulanzfrist bei der Berechnung einer Forderung für überfälligen oder verlorenen Exemplare berücksichtigt. Das Hinzufügen einer Kulanzfrist zu einem Fälligkeitsdatum folgt der gleichen Logik, die für die Verwaltung des Fälligkeitsdatums bei geschlossenen Öffnungszeiten gewählt ist, wenn die Kulanzfrist in eine Schließzeit der Servicestelle fällt.

**Exemplarlimit**. Ein Limit für Exemplare eingeben, die im Rahmen dieser Richtlinie ausgeliehen werden können.

Wurde **Rollend** ausgewählt, werden die folgenden Felder angezeigt:

**Ausleihdauer**. Eine Zeitspanne für die Ausleihfrist wählen.

**Fester Fälligkeitszeitplan (Fälligkeitsbegrenzung)**. Einen festen Fälligkeitsplan, wie unter [Einstellungen > Ausleihe > Feste Fälligkeitspläne](https://info.gbv.de/pages/viewpage.action?pageId=844267627) konfiguriert wählen. Der Zeitplan wird verwendet, um eine Begrenzung für automatische/fortlaufende Verlängerungen zu erzwingen. Es kann zum Beispiel Studenten erlaubt werden, Exemplare alle vier Wochen zu verlängern, aber die Verlängerungen sollen spätestens am Ende des Semesters enden.

**Verwaltung des Fälligkeitsdatums bei geschlossenen Öffnungszeiten**. Legt fest, wann das Exemplar fällig ist, wenn das berechnete Fälligkeitsdatum eines Exemplars in die Schließungszeit der Servicestelle fällt.

-   Wenn das Ausleihintervall eines Exemplars in Minuten oder Stunden angegeben ist, richtet sich das Fälligkeitsdatum nach der in der Ausleihrichtlinie angegebenen Auswahl.
-   Wenn das Ausleihintervall eines Exemplars in Tagen, Wochen oder Monaten angegeben ist, richtet sich das Fälligkeitsdatum nur dann nach der Ausleihrichtlinie, wenn die Servicestelle an dem Tag, an dem das Exemplar fällig wäre, vollständig geschlossen ist. Bei der Erstellung der Ausleihe prüft FOLIO den Kalender der Servicestelle; ist die Servicestelle an dem Tag, an dem das Exemplar fällig ist, zu einem beliebigen Zeitpunkt geöffnet, setzt FOLIO den Fälligkeitszeitpunkt auf 23:59 Uhr an diesem Tag.
**Kulanzfrist**. Eine Kulanzfrist für überfällige Exemplare eingeben. Wird sich für eine Kulanzfrist entschieden, ist das Exemplar erst nach dem Fälligkeitsdatum/der Fälligkeitszeit der Ausleihe plus dem Zeitraum der Kulanzfrist überfällig. Wenn die Kulanzfrist abläuft und das Exemplar nicht zurückgegeben wurde, wird die Kulanzfrist bei der Berechnung einer überfälligen oder verlorenen Forderung berücksichtigt. Das Hinzufügen einer Kulanzfrist zu einem Fälligkeitsdatum folgt der gleichen Logik, die für die Verwaltung des Fälligkeitsdatums bei geschlossenen Öffnungszeiten gewählt wurde, wenn die Kulanzfrist in eine Schließzeit der Servicestelle fällt

**Exemplarlimit**. Ein Limit für Exemplare eingeben, die im Rahmen dieser Richtlinie ausgeliehen werden.

### Verlängerungen

**Verlängerbar**. Wenn keine Verlängerungen unter dieser Police gewünscht sind, die Checkbox deaktivieren. Wird die Checkbox deaktiviert, werden alle anderen Felder ausgeblendet und die Exemplare sind nicht verlängerbar.

**Unbegrenzte Verlängerungen**. Die Checkbox markieren, wenn unbegrenzte Verlängerungen zugelassen werden sollen.

**Anzahl der erlaubten Verlängerungen**. Wenn Unbegrenzte Verlängerungen nicht ausgewählt wurden, die Anzahl der zulässigen Verlängerungen eingeben.

**Verlängern von**. Auswählen, ob ein Exemplar ab dem **Aktuellen Fälligkeitsdatum** oder dem **Systemdatum** verlängert werden soll.

**Verlängerungszeitraum abweichend von der ursprünglichen Ausleihe**. Die Checkbox markieren, wenn für verlängerte Exemplare eine andere Leihfrist als die ursprüngliche Leihfrist gewünscht ist. Ist dieses Feld markiert, werden die nächsten beiden Optionen angezeigt.

**Abweichende Ausleihdauer für Verlängerungen**. Die abweichende Leihfrist für Verlängerungen eingeben.

**Abweichender fester Fälligkeitszeitplan (Fälligkeitsbegrenzung) für Verlängerungen**. Ein festen Fälligkeitsplan wählen, wie unter Einstellungen > Ausleihe > Feste Fälligkeitspläne konfiguriert. Der Zeitplan wird verwendet, um eine Begrenzung für fortlaufende Verlängerungen zu erzwingen.

### Verwaltung von Bestandsanfragen

Festlegen, ob Rückrufe und/oder Vormerkungen zugelassen werden sollen.

Alle Felder in diesem Abschnitt sind optional. Anmerkung: Wenn diese Felder leer gelassen werden, sind Rückrufe und Vormerkungen nicht zulässig.

### Rückrufe

**Rückruf-Rückgabe-Intervall**. Eine Zeitspanne für das Rückrufintervall eingeben. Dies ist die Zeitspanne, in der die Person ein zurückgerufenes Exemplar zurückgeben muss, bevor es überfällig wird.

**Garantierte Mindestausleihdauer für zurückgerufene Exemplare**. Eine Zeitspanne für die garantierte Mindestausleihfrist für zurückgerufene Exemplare eingeben. Wenn der Rückruf eines Exemplars zugelassen wird, aber keine garantierte Mindestausleihfrist festlegen ist, wird das Rückruf-Rückgabe-Intervall effektiv zur garantierten Mindestausleihfrist für zurückgerufene Exemplare.

**Rückrufe zur Verlängerung von Fälligkeitsterminen für überfällige Ausleihen erlauben**. Wenn dieses Kontrollkästchen aktivieren wird, wird sichergestellt, dass Personen, die ein überfälliges Exemplar haben, dass zurückgerufen wird, nicht plötzlich mit unerwarteten Forderungen konfrontiert werden, obwohl sie davon ausgingen, dass das Exemplar lediglich überfällig ist.

### Vormerkungen

**Abweichende Ausleihdauer bei der Ausleihe für Exemplare mit einer aktiven, ausstehenden Vormerkung**. Um die Leihfrist für ein Exemplar mit einer Bestandsanfrage-Warteliste zu verkürzen, eine Zeitspanne eingeben. Wenn ein Exemplar ausgeliehen ist und keine Warteliste hat, wird die reguläre Leihfrist angewendet.

**Verlängerung von Exemplaren mit einer aktiven, ausstehenden Vormerkung erlauben**. Wenn Verlängerungen für ein ausgechecktes Exemplar mit Bestandsanfragen zugelassen werden soll, das Kontrollkästchen markieren. Wenn Verlängerungen erlaubt sind, können Personen das Exemplar weiterhin gemäß den Einstellungen im Abschnitt Verlängerungen verlängern.

**Abweichende Ausleihdauer bei Verlängerungen für Exemplare mit einer aktiven, ausstehenden Vormerkung**. Wenn Verlängerungen für Exemplare mit einer aktiven, ausstehenden Vormerkung zugelassen sind und die Leihfrist für die Verlängerung verkürzt werden soll, eine Zeitspanne eingeben.

## Ausleihrichtlinie duplizieren

1.  In der Ansicht **Ausleihrichtlinien** die Ausleihrichtlinie auswählen, die duplizieren werden soll.
2.  In der **Detailansicht der Ausleihrichtlinie** auf Aktionen > **Duplizieren** klicken. Es wird ein Fenster Ausleihrichtlinie erstellen mit denselben Informationen angezeigt wie die der Ausleihrichtlinie, die dupliziert werden soll.
3.  Die Informationen bearbeiten und dann die Richtline speichern.
4.  Auf **Speichern und schließen** klicken. Die duplizierte Ausleihrichtlinie wird gespeichert und erscheint in der Ansicht Ausleihrichtlinie.

## Ausleihrichtlinie bearbeiten

1.  In der Ansicht **Ausleihrichtlinien** die Ausleihrichtlinie auswählen, die bearbeitet werden soll.
2.  In der **Detailansicht der Ausleihrichtlinie** auf Aktionen > **Bearbeiten** klicken.
3.  Die Ausleihrichtlinie bearbeiten.
4.  Auf **Speichern und schließen** klicken. Die Richtlinie wird aktualisiert.

## Ausleihrichtlinie löschen

1.  In der Ansicht **Ausleihrichtlinien** die Ausleihrichtlinie auswählen, die gelöscht werden soll.
2.  In der **Detailansicht der Ausleihrichtlinie** auf Aktionen > **Löschen** klicken.
3.  Im Dialog **Ausleihrichtlinie löschen** auf **Löschen** klicken. Die Richtlinie wird gelöscht und eine Bestätigungsmeldung wird angezeigt.
