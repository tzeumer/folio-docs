---
title: "Vagrant"
linkTitle: "Vagrant"
date: 2023-02-01T00:00:00-00:00
tags: [by-folio, for-entwickler]
weight: 40
Description: "
    Quellen: [Folio](https://docs.folio.org/docs/getting-started/installation/vagrantboxes/) <!-- & [GBV](https://info.gebev.de/pages/viewpage.action?pageId=850624531) -->
    "
---

Wenn FOLIO nur ausprobiert werden soll, ohne es zu installieren, kann eine der vorgefertigten Vagrant-Boxen verwendet werden. FOLIO Vagrant-Box

![](/img/de/040%20Vagrant%20(Entwurf)/040%20Vagrant%20(Entwurf)_2023-02-20-19-44-00.png)

Vagrant-Boxen richten sich vorzüglich an Entwickler und Entwicklerinnen. Mit einer vorgefertigten Vagrant-Box kann eine FOLIO-Installation schnell zum Laufen gebracht werden. Auf diesen virtuellen Maschinen läuft eine Server oder PC: Neuinstallation (geplant) von FOLIO. Auf die Dienste Stripes und Okapi kann über Portweiterleitung zugegriffen werden. Es können neue Module auf dem Host-Betriebssystem erstellt und diese über ein reines Host-Netzwerk bereitgestellt werden, das bidirektionale Verbindungen zwischen dem Host- und dem Gastbetriebssystem ermöglicht, mit Okapi verbunden werden. Weitere Informationen zu Vagrant-Boxen sind unter https://github.com/folio-org/folio-ansible/blob/r3-2021-release/doc/index.md zu finden.