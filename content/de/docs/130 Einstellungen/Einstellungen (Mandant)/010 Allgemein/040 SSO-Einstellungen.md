---
title: "SSO-Einstellungen"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [app-einstellungen, by-folio, cat-einstellungen, for-admin, topic-sso]
weight: 40
Description: "
    Quellen: [Folio](https://docs.folio.org/docs/settings/settings_tenant/settings_tenant/#settings--tenant--sso-settings) & [GBV](https://info.gbv.de/display/FOLIOGBVEXTERN/Einstellungen+(Mandant):+SSO-Einstellungen)
    "
---

Diese Einstellung verwenden, wenn die Bibliothek ein Single Sign-On (SSO) für Mitarbeitende zur Anmeldung bei FOLIO einrichten möchte. SSO ermöglicht es dem Bibliothekspersonal, dieselbe Kennung und dasselbe Passwort zu verwenden, das sie auch für andere Dienste in der Bibliothek oder Universität benutzen, wodurch die Notwendigkeit entfällt, einen separaten Benutzernamen und ein separates Passwort nur für FOLIO zu verwenden.

Hinweis: Die Aktivierung von Single Sign-On erfordert in der Regel eine Abstimmung mit dem IT-Personal und/oder dem Identity Provider.

* **URL des Identity Providers**. Eine URL, unter der Metadaten über den Identitätsanbieter von FOLIO abgerufen werden können.
* **Metadaten herunterladen**. Nachdem alle SSO-Einstellungen ausgewählt wurden, auf Metadaten herunterladen klicken, um eine XML-Datei herunterzuladen, die an den Identity Provider gesendet werden sollte. Diese Datei muss erneut heruntergeladen werden, wenn irgendwelche Änderungen an diesen Einstellungen vorgenommen werden.
* **SAML-Binding**. Je nach Konfiguration Redirect-Binding wählen, um eine HTTP-Umleitung zur Anmeldeseite des Identity Providers zu verwenden, oder POST-Bindung, um ein HTTP-POST von der FOLIO-Anmeldeseite zu senden.
* **SAML-Attribut**. Das Attribut beim Identity Provider, das die Person eindeutig identifiziert.
* **Benutzereigenschaft**. Das Attribut in FOLIO, in dem das SAML-Attribut gefunden werden kann.
