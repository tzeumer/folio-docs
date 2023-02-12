---
title: "TUB HH [eManagement] - Ersterfassung Vereinbarung"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [app-e_management, by-tubhh, cat-workflows, for-anwender, by-community_einzelbeitrag]
weight: 210
Description: "
    Quellen: [Originalquelle](https://intranet.b.tu-harburg.de/mediawiki/index.php/FOLIO/Module/ERM/Workflows/Ersterfassung_Vereinbarung) & [GBV](https://info.gbv.de/display/FOLIOGBVEXTERN/TUB+HH+[eManagement]+-+Ersterfassung+Vereinbarung)
    "
---

{{% pageinfo %}}
Stand 2023-01
{{% /pageinfo %}}

## Erstes Eingabefenster/Kopfbereich

### Pflichtfelder

Pflichtfelder im Kopfbereich sind Name und Status.

### Name

* Bei der Schreibweise des Namens müssen doppelte Leerzeichen vermieden werden, da sonst die alphabetische Sortierung verändert wird. Auch Groß- und Kleinschreibung wirkt sich auf die Sortierung aus
* Die Namen werden in folgender Form erfasst:

### Bei Paketen:

1.  Stelle: Verlag
2.  Stelle: die Medienart (Journals/e-Books)
3.  Stelle: Nach einem Doppelpunkt ggf. der Paketname (z.B. Wirtschaftswissenschaften)
4.  Stelle: (Bei E-Book-Paketen das Jahr)
5.  Stelle: besonderes Erwerbungsmodell z.B. EBS

### Bei Datenbanken:

1.  Stelle: Verlag
2.  Stelle: Name der Datenbank

### Beschreibung

* In der eManagement-App nutzen wir die Beschreibung um Zeiträume zu erfassen, die durch Nationallizenzen abgedeckt sind. Beispiel, siehe Screenshot
    ![](/img/de/../../../attachments/210TUB~1_2023-02-09-23-12-46.png)

### Verlängerungspriorität

Wird ausgefüllt, wenn sicher ist, wie mit dem Paket zu verfahren ist (ansonsten Entscheidung Fachreferat abwarten oder Verlängerungsumfrage abwarten eingeben). Wenn Paket bestellt wurde und die Rechnung dementsprechend bearbeitet wurde, kann die Verlängerungspriorität wieder gelöscht werden. Sonst besteht die Gefahr dies zu vergessen und für das nächsten Jahr ist nicht mehr klar, welche Entscheidung wirklich getroffen wurde. Zudem lässt sich am Ende auf dem Dashboard nach der Verlängerungspriorität filtern.

**Definition der Auswahllistenwerte**

* _**Beim Lieferanten storniert:**_ Wir haben das laufende Paket bereits storniert. In Folio wird die Vereinbarung aber frühestens bei Ablauf des Vereinbarungszeitraum auf "abgeschlossen" gesetzt.
* _**Wird verlängert:**_ Die Vereinbarung läuft im laufenden Jahr aus. Die Entscheidung, dass das Paket verlängert werden soll. Wurde bereits getroffen.
* _**Angebot einholen:**_ Es muss erst ein neues Angebot eingeholt werden, bevor über die Verlängerung entschieden wird
* _**Entscheidung Fachreferat abwarten:**_ Das Paket bzw. aktuelles Angebot wurde zur Entscheidung an das Fachreferat weitergegeben
* _**Verlängerungsumfrage abwarten:**_ Insbesondere bei Konsortiallizenzen, gibt es vor Ablauf der Vertragslaufzeit Verlängerungsumfragen mit aktuellem Angebot
* _**Wird nicht verlängert:**_ Die Entscheidung, dass der auslaufende Vertrag nicht wieder verlängert wird, wurde bereits gefällt

## Vereinbarungszeiträume

Der Vereinbarungszeiträum entspricht dem Zeitraum einer Verlängerungsperiode oder Vertragsperiode, in der wir Zugriff auf die lizenzierten Medien haben Der Vereinbarungszeitraum muss nicht dem Gültigkeitszeitraum des Lizenzvertrags entsprechen Bei rückwirkender Erfassung kann man sich gut an den Bestellungen im ACQ orientieren um die vergangenen Vereinbarungszeiträume zu erfassen

## Interne Kontakte

Die internen Kontakte werden genutzt um das zuständige Fachreferat zu erfassen Die Fachreferenten werden nicht namentlich erfasst. Unter "Interne Kontakte" ist aus Fachreferat 2-6 auszuwählen. (Diese sind in der Personen-App bereits erfasst) Die Fachreferate werden in beiden Apps erfasst (eManagement und Lizenzverträge) In der Vereinbarung werden alle Fachreferate aufgenommen, die mit ihrem Budget an den in der Vereinbarung enthaltenen Paketen beteiligt sind, also auch wenn alle Fachreferate beteiligt sind. Abgesehen von den Fachreferaten erfassen wir keine weiteren internen Kontakte

## Vereinbarungskomponenten

Die Vereinbarungskomponenten können erst erfasst werden, wenn die entsprechenden Pakete in der GOKb erfasst und in Folio übertragen wurden. Vorgehen bei der Verknüpfung der E-Ressourcen in Vereinbarungskomponenten siehe Workflow (B-Handbuch/E-Ressourcen verknüpfen/E-Ressourcen-in-Vereinbarungskomponenten-verknüpfen)

## Informationen des Lizenzvertrags

Da wir die Lizenzverträge in Folio verwalten, verwenden wir den Punkt "Externe Lizenzverträge" nicht. Dieses Akkordeon ist für Bibliotheken gedacht, die ihre Lizenzverträge außerhalb von Folio verwalten Es können mehrere Lizenzverträge mit einer Vereinbarung verknüpft werden, jedoch nur ein wirkender Vertrag. Der Status "wirkend", "abgelaufen", oder "zukünftig" muss pro Vertrag ausgewählt werden. Der Status "wirkend" kann nur einmal vergeben werden. Es können daher nicht mehrere Vereinbarungskomponenten in einer Vereinbarung verwaltet werden, die je einen eigenen wirkenden Lizenzvertrag haben.

## Organisationen

* Die Organisationen werden ergänzend zu den Organisationen im Lizenzvertrag erfasst, können sich ggf. auch mit diesen überschneiden.
* Zur Erfassung von Organisationen siehe Workflow Pflege der Organisationen

### Hauptrollen zu Organisationen

* in der eManagement-App erfassen wir:
    * Mit der Rolle _**Lieferant**_: entweder den Buchhändler, den Konsortialführer oder den Verlag, je nachdem von wem wir die E-Medien "geliefert" bekommen
    * Mit der Rolle _**Anbieter**_: entweder den Verlag oder den Betreiber der Plattform über die die E-Medien bereitgestellt werden (wenn diese nicht vom Verlag betrieben wird; Bspl. MIT-eBooks auf IEEE Plattform)
    * Mit der Rolle _**Agentur**_ kann bei Bedarf eine 3. Organisation erfasst werden. z. B. wenn eine andere Organisation als der Lieferant für die Rechnungsstellung zuständig ist

### Zusätzliche Rollen zu Organisationen

* Dem Lieferanten kann eine zusätzliche Rolle hinzugefügt werden, entweder "Konsortialführende Organisation (zusätzliche Rolle) oder Buchhändler (zusätzliche Rolle)
    * Diese Rollen werden in der eMangement nicht alleinstehend sonder nur als zusätzliche Rolle verwendet
    * Die Rollen sollen Abfragen ermöglichen, welche Vereinbarungen über einen Buchhändler oder Konsortialführer laufen

### Primärorganisation

* Das Häkchen bei "Primärorgansisation" wird grundsätzlich beim Lieferanten gesetzt
* Die Primärorganisation erscheint im Kopf der Vereinbarungen

![](/img/de/../../../attachments/210TUB~1_2023-02-09-23-13-02.png)

## Ergänzende Eigenschaften

* wir haben primäre "_Ergänzende Eigenschaften_" festgelegt, die auf alle Vereinbarungen zutreffen
* weitere "_Optionale Ergänzende Eigenschaften_" können ausgewählt werden, treffen aber ggf. nur auf bestimmte Ressourcen-Arten zu.
* die ergänzenden Eigenschaften können zum größten Teil von der entsprechenden Pakete-Seite im Media-Wiki übernommen werden
* Stellt sich heraus, dass bestimmte ergänzende Eigenschaften sinnvoller als primäre oder optionale Eigenschaften genutzt werden können, kann dies durch einen System-Administrator geändert werden
* **Rechnungsstellung**: Das erwartete Datum der Rechnungsstellung nehmen wir bei rückwirkend erfassten Vereinbarungen nicht auf. Es wird erfasst, wenn die Vereinbarung zur Zeit der Bestellung erstellt wird.

## Ergänzende Dokumente

* Wir erfassen in der Vereinbarung vorerst keine Dokumente (ggf. neue Entscheidung zu späterem Zeitpunkt). Grundsätzlich haben wir aber Kategorien für folgende ergänzende Dokumente festgelegt:
    * Lieferantenbedingungen
    * Angebot
    * Bestellung
    * Zusätzliche Informationen
* Noch nicht wirkend (ggf. neue Entscheidung): Die ergänzenden Dokumente werden sowohl in Folio als auch auf Laufwerk G bzw. J oder im E-Medien-Account gespeichert
* Die Felder "Physischer Standort" und "URL" nutzen wir. Hier wird der Pfad zum Dokument hinterlegt.

## Nutzungsdatenquelle

* Hier kann eine Nutzungsdatenquelle aus der eUsage-App verknüpft werden, wenn diese bereits angelegt ist. Das bedeutet in der eUsage-App wurde ein Datensatz angelegt, der regelmäßig über Sushi oder den Nationalen Statistikserver die Nutzungsdaten zu Paketen abruft
    
    ![](/img/de/../../../attachments/210TUB~1_2023-02-09-23-13-20.png)

* Wird in der E-Management-App eine Verknüpfung erstellt, wird im Lesemodus zusätzlich das Akkordeon Nutzungsstatistiken angezeigt. Es wird eine Verbindung zwischen den in der Vereinbarung vorhandenen E-Ressourcen und der Statistikdaten hergestellt. Diese kann man sich im Lesemodus der Vereinbarung individuell anzeigen lassen (scheint noch nicht zu funktionieren, Stand 25.4.2022)
    ![](/img/de/../../../attachments/210TUB~1_2023-02-09-23-13-33.png)

## Zugehörige Vereinbarungen

* An dieser Stelle werden ggf. Vereinbarungen verknüpft, die mit dieser im Zusammenhang stehen.
* Verknüpft wird z.B.
    * ein EBS-Paket mit den EBS-Festkäufen
    * ein beendetes Paket mit dem entsprechenden Post-Cancellation-Access
    * eine vorangegangene oder folgende Vereinbarung mit der vorliegenden
* erst die zu verknüpfende Vereinbarung auswählen (Button "Vereinbarung verknüpfen")
* anschließen die entsprechende Beziehung auswählen
* ggf. eine Bemerkung zur Verknüpfung hinzufügen
* Die Verknüpfung erfolgt automatisch auch in der anderen Vereinbarung

## Sonstige Arbeitsschritte

### Media-Wiki

Nachdem ein Paket vollständig in Folio aufgenommen ist:

* Überprüfen, ob alle wichtigen Informationen von der Pakete-Seite übernommen wurden
* Pakete-Seiten erhalten die Kategorie "Folio-ERM-erfasst"
* Zusätzlich wird oben auf der Pakete-Seite der Satz (fett) eingefügt "Seite ggf. nicht mehr aktuell, Informationen werden nur noch in Folio gepflegt" Ergänzung zur Besprechung:
    * Bei E-Book-Paketen, die keine eigene Pakete-Seite haben, wird zur Information der Satz "Paket ist in Folio erfasst", an erster Stelle in fett eingefügt.
