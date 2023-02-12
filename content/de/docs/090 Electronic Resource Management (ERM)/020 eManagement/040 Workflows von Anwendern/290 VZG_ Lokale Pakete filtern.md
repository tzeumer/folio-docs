---
title: "VZG: Lokale Pakete filtern"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [app-e_management, by-vzg, cat-workflows, for-anwender, by-community_einzelbeitrag, app-gokb]
weight: 290
Description: "
    Quellen: [GBV](https://info.gbv.de/display/FOLIOGBVEXTERN/VZG:+Lokale+Pakete+filtern)
    "
---

{{% pageinfo %}}
Stand 2023-01
{{% /pageinfo %}}

Für lokale Pakete aus der GOKb wurden in FOLIO zwei Eigenschaften hinzugefügt:

* Paketverfügbarkeitsbereich
* Paketverfügbarkeitsbeschränkungen

Der Paketverfügbarkeitsbereich wird verwendet, um die allgemeine Verfügbarkeit des Pakets zu erfassen - in der GOKb wird dies als die "Gültigkeit" des Pakets bezeichnet und kann einen der folgenden Werte annehmen:

* Global
* Konsortial
* Regional
* Andere
* Lokal

Paketverfügbarkeitsbeschränkungen werden verwendet, um spezifische Beschränkungen auf der Grundlage des Verfügbarkeitsbereichs aufzuzeichnen. Wenn z.B. der Verfügbarkeitsbereich = "regional" ist, dann ist die Verfügbarkeitsbeschränkung eine Liste der Regionen, in denen das Paket verfügbar ist.

Wenn GOKb-Daten abgerufen werden, funktioniert das folgendermaßen:

Wenn der Verfügbarkeitsbereich (GOKb-Gültigkeit) "Konsortium" oder "Regional" ist, werden die Verfügbarkeitsbeschränkungen aus dem GOKb-Feld "globalNote" gefüllt, das in der GOKb-Benutzeroberfläche als "Region/Konsortium" bezeichnet wird.

Wenn der Verfügbarkeitsbereich (GOKb-Gültigkeit) lokal ist, werden die Verfügbarkeitsbeschränkungen aus den Kuratierendengruppen in der GOKb übernommen (ein einzelnes GOKb-Paket kann mehrere Kuratierendengruppen haben, die wir alle in die Beschränkungen aufnehmen).

Dies ist detailliert in [https://issues.folio.org/browse/ERM-2307](https://issues.folio.org/browse/ERM-2307) beschrieben und ist Teil von mod-agreements 5.4.x (also ab Nolana)

Aus Sicht der Nutzer können Sie die Filter "Zuschnitt" und "Verfügbarkeit" verwenden, um die Pakete zu finden, die ihren Kriterien entsprechen (Auswahl der kuratorischen Gruppe im Filter "Verfügbarkeit"), gegebenenfalls in Kombination mit dem Filter "Zuschnitt" (lokal)

Beispiel: Lokale Pakete mit der kuratorischen Gruppe HeBIS auf Folio Snapshot ist [https://folio-snapshot.dev.folio.org/erm/packages?filters=availability.hebis%2Cscope.local&sort=name](https://folio-snapshot.dev.folio.org/erm/packages?filters=availability.hebis%2Cscope.local&sort=name).
