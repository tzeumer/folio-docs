---
title: "Person anlegen"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [app-personen, by-folio, cat-worklfows, for-anwender, topic-passwort]
weight: 10
Description: "
    Quellen: [Folio](https://docs.folio.org/docs/users/#creating-a-user-record-manually) & [GBV](https://info.gbv.de/display/FOLIOGBVEXTERN/Folio:+Person+anlegen)
    "
---

1.  Im Bereich der **Personensuche** auf **Aktionen > Neu** klicken
2.  Im Fenster **Benutzer/-in anlegen** die Felder **Personeninformationen**, **Erweiterte Informationen** und **Kontaktinformationen** ausfüllen. Die Abschnitte mit den **benutzerdefinierten Feldern** ausfüllen, falls diese konfiguriert wurden. Weitere Informationen zu den Feldern und Aktionen, die in diesen Abschnitten verfügbar sind, sind in den Abschnittsbeschreibungen unten zu finden.
3.  Wenn Sie alle gewünschten Informationen über den Benutzer eingegeben haben, klicken Sie auf **Speichern & schließen**. Der Benutzerdatensatz wird gespeichert.

## Personeninformationen

* **Nachname (erforderlich)**. Der Nachname der Person.
* **Vorname**. Der Vorname der Person.
* **Mittlerer Name**. Der zweite Vorname der Person.
* **Bevorzugter Vorname**. Der Name, mit dem die Person bevorzugt angesprochen werden möchte. Wenn ein bevorzugter Vorname angegeben wird, wird er im Personendatensatz anstelle des Vornamens angezeigt.
* **Personengruppe (erforderlich)**. Wählen Sie eine Personengruppe aus, die der Person zugeordnet werden soll. Personengruppe sind Klassen von Bibliotheksbenutzenden, die in der App "Einstellungen" konfiguriert werden. Siehe [Einstellungen > Personen > Personengruppen](https://info.gbv.de/display/FOLIOGBVEXTERN/Einstellungen+%28Personen%29%3A+Personengruppen) für weitere Informationen.
* **Status (erforderlich)**. Einen Status für die Person auswählen: Aktiv oder Inaktiv. Der Status einer Person ist an das Ablaufdatum in des Personendatensatzes gebunden. Der Status "aktiv" zeigt an, dass die Person derzeit in der Institution der Bibliothek beschäftigt oder eingeschrieben ist. Der inaktive Status zeigt an, dass das Ablaufdatum des Personendatensatzes überschritten wurde und die Person nicht mehr zugehörig, angestellt oder eingeschrieben ist. Wenn eine Personengruppe ausgewählt wird, ist der Status automatisch auf "Aktiv" voreingestellt.
* **Ablaufdatum**. Die Zeitspanne, die festgelegt wird, bevor der Personendatensatz abläuft und die Person nicht mehr über aktive Berechtigungen verfügt oder keine Exemplare mehr ausleihen kann. Das Ablaufdatum bestimmt, wann der Status einer Person von Aktiv zu Inaktiv wechselt. Nachdem eine Benutzergruppe ausgewählt wurde, wird dazu aufgefordert, das Standardablaufdatum für diese Personengruppe zu verwenden. Klicken Sie im Popup-Fenster Ablaufdatum einstellen auf Einstellen, um das Standardablaufdatum für die Personengruppe zu akzeptieren. Andernfalls, wenn Sie das Ablaufdatum anpassen möchten, klicken Sie auf Abbrechen und geben das Datum in das Feld Ablaufdatum ein oder klicken auf das Kalendersymbol, um ein Datum auszuwählen. Sie können das Feld auch leer lassen.
* **Barcode**. Die Barcode-Nummer für den Bibliotheksausweis der Person.

## Erweiterte Informationen

* **Erfassungsdatum**. Das Datum, an dem eine Person an der Institution eingeschrieben ist. Dieses Feld wird automatisch ausgefüllt, wenn es in Daten enthalten ist, die von einem externen System bereitgestellt werden.
* **Externe System-ID**. Die ID des externen Systems für die Person. Dieses Feld wird automatisch ausgefüllt, wenn es in Daten enthalten ist, die von einem externen System bereitgestellt werden.
* **Geburtsdatum**. Das Geburtsdatum der Person im Format JJJJ-MM-TT.
* **Folio-ID**. Eine vom System generierte Nummer für den Personendatensatz.
* **Bestandsanfragenpräferenz**. Das **Abholregal** ist standardmäßig für alle Personen ausgewählt. Wenn auch **Lieferung** angekreuzt ist, wählen Sie **Bereitstellungspräferenz**.
* Wenn **Lieferung** als **Bereitstellungspräferenz** ausgewählt ist, wählen Sie die **Voreingestellte Lieferadresse**. Dieses Feld wird nur angezeigt und ist nur erforderlich, wenn **Lieferung** als Bestandsanfragenpräferenz ist. Adressen werden dem Personendatensatz im Abschnitt **Kontaktinformationen** hinzugefügt. Weitere Informationen sind unten im Abschnitt Kontaktinformationen zu finden.
* Wenn **Abholregal** als **Bestandsanfragenpräferenz** ausgewählt ist, muss eine **Voreingestellte Abhol-Servicestelle** ausgewählt werden. Allen Personendatensätzen ist mindestens ein Servicestelle zugewiesen, um den Ort für die Ausleihe oder Abholung von angeforderten Exemplaren anzugeben. Die Servicestellen werden in der App "Einstellungen" konfiguriert. Weitere Informationen dazu unter [Einstellungen > Mandant > Servicestellen](https://info.gbv.de/display/FOLIOGBVEXTERN/Einstellungen+%28Mandant%29%3A+Servicestellen).
* **Name der Abteilung (ACHTUNG: ÜBERSETZUNG DES FELDES FREI GEWÄHLT, CHECKEN)**. Name der Abteilung der Person, falls zutreffend. Um der Person einer Abteilung zuzuordnen, auf **Abteilung hinzufügen** klicken und die Abteilung aus der Dropdown-Liste auswählen. Diese Aktion ist wiederholbar, und Abteilungen können durch Klicken auf das **Mülleimer-Symbol** gelöscht werden. Die Schaltfläche **Abteilung hinzufügen** wird nur angezeigt, wenn Abteilungen in der App "Einstellungen" konfiguriert sind. Weitere Informationen unter [Einstellungen > Benutzer > Abteilungen](https://info.gbv.de/display/FOLIOGBVEXTERN/Einstellungen+%28Personen%29%3A+Abteilungen).
* **Benutzername**. Der Name, mit dem sich Bibliothekspersonal bei FOLIO anmelden. Hinweis: Andere Personen haben keinen Benutzernamen, da sie sich nicht bei FOLIO anmelden müssen.
* **Passwort**. Personen können einen Link zum Zurücksetzen des Passworts per E-Mail erhalten. Dieser Link verfällt nach 24 Stunden. Das Passwort muss die folgenden Standardvalidierungsregeln erfüllen:
    * Es muss mindestens 8 Zeichen enthalten.
    * Es muss sowohl Groß- als auch Kleinbuchstaben enthalten.
    * Es muss mindestens 1 numerisches Zeichen enthalten.
    * Mindestens 1 Sonderzeichen enthalten.
    * Enthält nicht den Benutzernamen.
    * Enthält keine Tastatursequenz.
    * Enthält nicht das gleiche Zeichen.
    * Enthält keine Leerzeichen.
    * **Hinweis**: Die Institution kann beschließen, für ihre Personen andere Regeln zur Validierung von Passwörtern anzuwenden.

## Kontaktinformationen

* **E-Mail (erforderlich)**. Die E-Mail Adresse der Person.
* **Telefon**. Die Telefonnummer der Person.
* **Mobiltelefon**. Die Mobiltelefonnummer der Person.
* **Bevorzugte Kontaktmöglichkeit (erforderlich)**. Die bevorzugte Kontaktmethode der Person festlegen: E-Mail, Post (Primäre Adresse) oder SMS.
* **Adressen**. Die Adresse der Person. Es können mehrere Adressen hinzugefügt werden. Auf **Adresse hinzufügen** klicken, um eine Adresse hinzuzufügen.
* Wählen Sie **Als primäre Adresse verwenden**, wenn die Adresse als Hauptadresse der Person gelten soll.
* **Adresstyp**. Den entsprechenden Adresstyp für die Adresse der Person auswählen. Adresstypen werden in der App "Einstellungen" konfiguriert. Weitere Informationen unter [Einstellungen > Personen > Adresstypen](https://info.gbv.de/display/FOLIOGBVEXTERN/Einstellungen+%28Personen%29%3A+Adresstypen).
* Die Felder mit den Adressinformationen ausfüllen und auf **Adresse hinzufügen** klicken, um die Adresse im Personendatensatz zu speichern.

## Benutzerdefinierte Felder

Der Abschnitt "Benutzerdefinierte Felder" wird nur angezeigt, wenn er in der App Einstellungen>Personen konfiguriert wurde. Weitere Informationen zum Konfigurieren des Abschnitts Benutzerdefinierte Felder unter Einstellungen /> Benutzer /> Benutzerdefinierte Felder.
