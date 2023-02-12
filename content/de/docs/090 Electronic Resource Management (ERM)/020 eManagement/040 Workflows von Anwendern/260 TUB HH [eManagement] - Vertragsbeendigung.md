---
title: "TUB HH [eManagement] - Vertragsbeendigung"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [app-e_management, by-tubhh, cat-workflows, for-anwender, by-community_einzelbeitrag]
weight: 260
Description: "
    Quellen: [Originalquelle](https://intranet.b.tu-harburg.de/mediawiki/index.php?title=FOLIO/Module/ERM/Workflows/Vertragsende) & [GBV](https://info.gbv.de/display/FOLIOGBVEXTERN/TUB+HH+[eManagement]+-+Vertragsbeendigung)
    "
---

{{% pageinfo %}}
Stand 2023-01
{{% /pageinfo %}}

## Fall 1: Alle E-Medien sind dauerhaft zugänging

### Vereinbarung

-   Enddatum des aktuellen Vereinbarungszeitraums: Das Enddatum wird gesetzt
-   Status: Der Status bleibt auf "aktiv"
-   verknüpfter Lizenzvertrag: Insofern der Lizenzvertrag auch für den dauerhaften Zugriff gültig ist, bleibt er weiterhin als "wirkend" verknüpft
-   Dauerhafter Zugriff: "ja"

## Fall 2: Alle E-Medien sind nach Beendigung des Vertrags nicht mehr zugängig

### Vereinbarung

-   Enddatum des aktuellen Vereinbarungszeitraums: Das Enddatum wird gesetzt
-   Status: Der Status wird auf "abgeschlossen" geändert
-   Grund für die Schließung: Wird entsprechend ausgewählt
-   Vereinbarungskomponenten: Das Enddatum wird auch in den Vereinbarungskomponenten bei "aktiv bis" gesetzt

## Fall 3: Nur ein Teil der E-Medien ist nach Vertragsbeendigung noch zugängig

### Vereinbarung für die Vertragslaufzeit

-   Enddatum des aktuellen Vereinbarungszeitraums: Das Enddatum wird gesetzt
-   Status: Der Status wird auf "abgeschlossen" geändert
-   Grund für die Schließung: Wird entsprechend ausgewählt
-   Vereinbarungskomponenten: Das Enddatum wird auch in den Vereinbarungskomponenten bei "aktiv bis" gesetzt
-   Die Vereinbarung wird mit der 2. Vereinbarung für den dauerhaften Zugriff verknüft

### Vereinbarung für den dauerhaften Zugriff

-   siehe [TUB HH \[eManagement\] - Erfassung von Paketen im PCA-Modell (Post Cancellation Access)](https://info.gbv.de/pages/viewpage.action?pageId=855343330)
