---
title: "Bestandsanfragen Bestandsanfragen zur Lieferung bearbeiten"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [by-folio, for-anwender, app-bestandsanfragen, cat-workflows]
weight: 120
Description: "
    Quellen: [Folio](https://docs.folio.org/docs/access/requests/requests/#processing-delivery-requests) & [GBV](https://info.gbv.de/display/FOLIOGBVEXTERN/Folio:+Bestandsanfragen+Bestandsanfragen+zur+Lieferung+bearbeiten)
    "
---

Wenn eine Bibliothek Exemplare an bestimmte Personen ausliefert, sollten sie Bestandsanfragen zur Lieferung einrichten. Wenn eine Bibliothek beispielsweise von Dozenten angeforderte Exemplare an deren Büro sendet, hat die Bibliothek über die Bestandsanfrage zur Lieferung die Adresse der Person und die Möglichkeit, das Exemplar nach Ankunft an die Person auszuleihen.

Die Zustellung muss zunächst im Personendatensatz einer Person aktiviert werden, und in ihrem Konto muss eine Standardlieferadresse angegeben sein. Diese Einstellung können manuell oder über einen Batch-Import konfiguriert werden. Die folgenden Schritte beschreiben, wie die Zustellung manuell aktiviert und eine Bestandsanfrage bearbeiten wird.

## Lieferungen manuelle im Personendatensatz einschalten

1.  Die Person in der App Personen suchen.
2.  Auf **Bearbeiten** klicken.
3.  Im **Personendatensatz**\-Fenster unter **Bestandsanfragenpräferenz** die Option **Lieferung** wählen, um die Zustellung zu aktivieren.
4.  Eine **Bereitstellungspräferenz** für die Person wählen.
5.  Eine **Voreingestellte Lieferadresse** wählen, die verwendet wird, wenn die Person eine Bestandsanfrage zur Lieferung hat. Wenn die Person keine Adresse in ihrem Personendatensatz hat, muss diese hinzugefügt werden.
6.  Auf **Speichern & schließen** klicken.

## Bestandsanfrage zur Lieferung erstellen

1.  [Eine Bestandsanfrage erstellen](https://info.gbv.de/display/FOLIOGBVEXTERN/Folio%3A+Bestandsanfragen+auf+Exemplarebene).
2.  Wenn die Person nicht die **Bereitstellungspräferenz** Lieferung hat, dann **Lieferung** wählen.
3.  Eine **Lieferadresse** wählen.
4.  Auf **Speichern & schließen** klicken, um die Bestandsanfrage zu starten.

## Rückgabe einer Bestandsanfrage zur Lieferung

Bestandsanfragen zur Lieferung werden nicht anders behandelt als Exemplare, die in das Abholregal gestellt werden. Die Bestandsanfrage zur Lieferung wird ausgelöst, sobald das Exemplar an einem beliebigen Standort zurückgebucht wird.

Wenn eine Bestandsanfrage zur Lieferung eingecheckt wird, gibt es zwei Möglichkeiten: das Exemplar kann an die Person ausgeliehen werden oder es kann auf die Bearbeitung der Anfrage gewartet werden.

Um das Exemplar an die Person auszuleihen, wie folgt vorgehen :

1.  Das Exemplar in der App Rückgaben verbuchen.
2.  Optional: Wenn im Dialog **Bestandsanfrage zur Lieferung weiterleiten** nicht gewünscht ist, dass ein Versandzettel gedruckt wird, die Checkbox **Zettel drucken** deaktivieren.
3.  Um das Exemplar an die Person auszuleihen, auf **Schließen und Ausleihen** klicken. Das Fenster Ausleihe erscheint und das Exemplar wird automatisch an die Person ausgeliehen.
4.  Um die Ausleihe zu beenden, auf **Session beenden** klicken.

Wenn mit der Bearbeitung der Bestandsanfrage gewartet werden soll, folgendermaßen vorgehen :

1.  Das Exemplar in der App Rückgabe eingeben.
2.  Optional: Wenn im Dialog Bestandsanfrage nicht gewünscht ist, dass ein Vormerkzettel gedruckt wird, deaktivieren Sie die Checkbox **Zettel drucken.**
3.  Auf **Schließen** klicken. Das Dialogfeld Bestandsanfrage wird geschlossen, und der Status des Exemplars ändert sich in Warten auf Lieferung.

