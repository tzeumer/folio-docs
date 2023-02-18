---
title: "Bestandsanfragen auf Titelebene"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [by-folio, for-anwender, app-bestandsanfragen, cat-workflows]
weight: 40
Description: "
    Quellen: [Folio](xxx) & [GBV](xxx)
    "
---

Bibliotheksmitarbeitende erstellen Bestandsanfragen in der Bestandsanfragen-App. Die Bestandsanfrage kann auch von einem Personendatensatz in Personen oder einem Exemplardatensatz in Katalog aus gestartet werden. Diese Apps leiten zur Erstellung der Anfrage in die Bestandsanfragen-App weiter.

Bitte beachten, dass die Berechtigung zum Erstellen von Bestandsanfragen in der Bestandsanfragen-App vorhanden sein muss, um die Option zum Erstellen einer Anfrage aus dem Katalog zu sehen. Ebenfalls beachten, dass eine Bestandsanfrage auf Titelebene nur dann auf eine Instanz gestellt werden kann, wenn diese Instanz über einen Bestandseintrag verfügt. Ein Exemplardatensatz ist nicht erforderlich, um eine Bestandsanfrage zu erstellen, aber er ist erforderlich, um die Anfrage zu erfüllen.

1.  In der Ansicht **Bestandsanfrage** die Option **Aktionen > Neu** wählen.
2.  Um eine Bestandsanfrage auf Titelebene zu erstellen, sicherstellen, dass die Option **Bestandsanfrage auf Titelebene erstellen** aktiviert ist.
3.  Möglicherweise sind die Titelinformationen bereits eingegeben (wenn die Anfrage aus der Bestandsanfragen-App heraus gestartet wurde). Wenn nicht, muss nach dem Titel gesucht werden:
    1.  Auf **Titelsuche** klicken.
    2.  In dem daraufhin angezeigten Pop-up nach dem Titel suchen, für den die Bestandsanfrage gestellt werden soll.
    3.  Auf den Titel klicken, um ihn auszuwählen. Das Pop-up wird geschlossen und die Informationen zum Titel werden in das Bestandsanfrageformular eingefügt.
4.  Den **Bestandsanfragetyp** wählen. Welche Optionen angezeigt werden, hängt vom Status des Exemplars ab, das angefragt wird.
5.  Optional: Ein **Ablaufdatum Bestandsanfrage** eingeben. Wenn die Bestandsanfrage zum gewählten Datum noch offen ist, wird sie geschlossen und ihr Status ändert sich in Geschlossen - unerfüllt.
6.  Optional: Einen **Kommentar Benutzer/-in** eingeben. Wenn die Person das Exemplar zum Beispiel sofort benötigt, kann dies hier vermerkt werden. Die Kommentare werden im CSV-Bericht und auf den Entnahmezetteln angezeigt.
7.  Im Feld **Informationen über Benutzer/in** entweder den Barcode der Person scannen oder den Barcode eingeben und auf **Eingabe** klicken.
8.  Wenn der Barcode der Person nicht verfügbar ist, auf **Personensuche** klicken, um nach der Person zu suchen:
    1.  Im Dialogfeld **Person auswählen** nach der Person suchen.
    2.  Wenn die Person gefunden wurde, diese aus der Ergebnisliste der Personensuche auswählen. Sie wird auf in der Bestandsanfrage angewendet und  ihre Informationen werden angezeigt.
9.  Die **Bereitstellungspräferenz** wählen.
10.  Die **Abholservicestelle** oder die **Lieferadresse** wählen, je nachdem, was im vorherigen Schritt ausgewählt wurde.
11.  Auf **Speichern & schließen** klicken. Die Bestandsanfrage wird gespeichert und die Ansicht mit den Details der Anfrage wird angezeigt. Die Person erhält eine E-Mail-Benachrichtigung, dass ihre Bestandsanfrage bei der Bibliothek eingegangen ist, [sofern diese Benachrichtigung konfiguriert wurde]({{< ref "040 Benachrichtigungen Benutzende" >}}).

## Wie FOLIO entscheidet, welches Exemplar eine Bestandsanfrage auf Titelebene erfüllt

FOLIO prüft zunächst, ob ein Exemplar in der Instanz verfügbar ist. Wenn ein Exemplar verfügbar ist, prüft FOLIO die Ausleihregeln, um zu entscheiden, was als nächstes zu tun ist.

Wenn ein Exemplar verfügbar ist und die FOLIO-Ausleihregeln das Bestellen erlauben, wird die Bestandsanfrage auf Titelebene zu einer Bestellung für dieses Exemplar.

Wenn mehrere Exemplare verfügbar sind, wählt FOLIO zunächst ein Exemplar mit dem tatsächlichen Standort an der gewählten Abholservicestelle aus. Ist kein Exemplar an einem effektiven Standort der Abholservicestelle verfügbar, versucht FOLIO, ein Exemplar von einem anderen Standort dieser Servicestelle auszuwählen.

Wenn an einem effektiven Standort mit einer primären Servicestelle, die der Abholservicestelle des Anfragenden entspricht, kein passendes Exemplar verfügbar ist, sucht FOLIO nach Exemplaren an dem nächstgelegenen Standort.

Wenn zum Zeitpunkt der Erstellung der Anfrage keine Exemplare in der Instanz verfügbar sind, wird die Anfrage entweder zu einer Vormerkung oder zu einem Rückruf, je nach der in der Bestandsanfragen-App getroffenen Auswahl.

Ist die Bestandsanfrage eine Vormerkung, verbleibt sie in der Warteliste für den Titel, wird aber erst dann mit einem Exemplar verknüpft, wenn die Anfrage an erster Position in der Warteliste steht und ein Exemplar zurückgegeben wird.

Handelt es sich bei der Bestandsanfrage um einen Rückruf, so gilt dieser für die Ausleihe, deren Fälligkeitsdatum dem aktuellen Fälligkeitsdatum am nächsten liegt. Wenn das Exemplar zurückgegeben wird, wird es der ersten offenen Bestandsanfrage zugeordnet, unabhängig davon, ob es sich bei dieser Anfrage um den Rückruf handelt, der die Rückgabe des Exemplars ausgelöst hat.

## Bestandsanfragen auf Titelebene anzeigen

wird eine Bestandsanfrage auf Titel-Ebene aufgerufen, werden zusätzliche Informationen angezeigt. Die Titelinformationen werden im oberen Akkordeon angezeigt, einschließlich der Anzahl der offenen Bestandsanfragen auf dieser Instanz.

Sobald eine Bestandsanfrage zu einer Bestellung oder einem Rückruf wird, wird auch das Akkordeon mit den Exemplarinformationen angezeigt, einschließlich der Anzahl der offenen Anfragen zu diesem Exemplar.

Bei Rückrufen zeigt die Exemplarinformation das Exemplar an, das zurückgerufen wurde, aber wenn dieses Exemplar zurückgegeben wird, wandert es auf die erste Anfrageposition in der Warteliste, auch wenn es nicht mit dieser speziellen Anfrage verbunden war.

## Bestandsanfrage auf Titelebene bearbeiten

Es können nur offene Bestandsanfragen bearbeitet werden. Sobald eine Bestandsanfrage geschlossen ist, kann sie nicht mehr bearbeitet werden.

1.  [Die Bestandsanfrage suchen]({{< ref "060 Bestandsanfragen suchen" >}}), die bearbeitet werden soll.
2.  In der Ansicht **Bestandsanfrage** die **Aktionen > Bearbeiten** wählen.
3.  Die Bestandsanfrage bearbeiten.
4.  Auf **Speichern & schließen** klicken. Die Bestandsanfrage wird aktualisiert.

## Bestandsanfrage auf Titelebene duplizieren

Alle offenen Bestandsanfragen können dupliziert werden. Wenn die Bestandsanfrage dupliziert wird, muss die anfordernde Person geändert werden, da eine Person nicht mehr als eine offene Bestandsanfrage auf derselben Instanz haben kann.

1.  [Die Bestandsanfrage suchen]({{< ref "060 Bestandsanfragen suchen" >}}), die duplizieren werden soll.
2.  In der Ansicht **Bestandsanfrage** die **Aktionen > Duplizieren** wählen. Es erscheint ein Fenster **Neue Anfrage** mit denselben Exemplarinformationen, Bestellinformationen und Informationen zur anfordernden Person der Anfrage, die duplizieren werden soll.
3.  Die Bestandsanfrage bearbeiten, bevor die Anfrage abgeschickt wird.
4.  Eine **Abholservicestelle** auswählen.
5.  Auf **Speichern & schließen** klicken. Die duplizierte Anfrage wird in der Ansicht Bestandsanfrage angezeigt.

## Bestandsanfrage auf Titelebene auf ein anderes Exemplar der selben Instanz umhängen

Um eine Bestandsanfrage-Warteliste aus dem Instanzdatensatz im Katalog anzuzeigen, die **Aktion > Anfragen anzeigen & neu ordnen** wählen.

Um eine Bestandsanfrage-Warteliste aus dem Datensatz einer Bestandsanfrage anzuzeigen, die Anfrage in der Bestandsanfragen-App suchen und dann **Aktion> Warteliste neu ordnen** wählen .

**Bereitstellung läuft** zeigt Anfragen an, die in Bearbeitung sind und denen ein Exemplar zugeordnet ist. Zu diesen Bestandsanfragen gehören:

* Bestandsanfragen, unabhängig vom Status der Anfrage. Das bedeutet, dass in diesem Abschnitt Bestandsanfragen mit dem Status **Offen - Noch nicht erfüllt** zu sehen sind.
* Bestandsanfragen, die **Offen - Im Abholregal** sind
    Bestandsanfragen, die **Offen - Warten auf Lieferung** sind
    Bestandsanfragen, die **Offen - In Transport** sind

**Offen - Noch nicht erfüllt** zeigt Bestandsanfragen und Rückrufe an, die noch nicht bearbeitet werden. Diese Bestandsanfragen können per Drag-and-Drop neu sortiert werden. Diese Bestandsanfragen haben alle den Status **Offen - Noch nicht erfüllt**.

In diesem Bereich kann die Spalte **Exemplarbarcode** Informationen enthalten oder auch leer sein.

* Bestandsanfrage auf Exemplarebene - der Barcode des angeforderten Exemplars ist zu sehen.
* Rückruf auf Titelebene - der Barcode des Exemplars, das zurückgerufen wurde, ist zu sehen. Bitte beachten, dass, wenn das Exemplar zurückgegeben wird und es eine Anfrage erfüllen könnte, die weiter oben in der Warteliste steht, diese Anfrage erfüllt wird, nicht die Anfrage, die den Rückruf ausgelöst hat.
* Bestandsanfrage auf Titelebene - die Spalte **Exemplarbarcode** ist leer.

