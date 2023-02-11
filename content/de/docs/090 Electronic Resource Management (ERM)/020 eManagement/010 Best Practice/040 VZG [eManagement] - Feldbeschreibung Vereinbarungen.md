---
title: "VZG [eManagement] - Feldbeschreibung Vereinbarungen"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [app-e_management, cat-bestpractices, for-admin, by-vzg, by-community_einzelbeitrag]
weight: 10
Description: "
    Quellen: [GBV](https://info.gbv.de/display/FOLIOGBVEXTERN/VZG+[eManagement]+-+Feldbeschreibung+Vereinbarungen)
    "
---

|1|Feldbezeichnung|Beschreibung|Pflichtfeld|Wiederholbar|Typ|Ergänzende Informationen|
|:----|:----|:----|:----|:----|:----|:----|
|2|Name Name|Ein von der Einrichtung vergebener Name für die Vereinbarung|Ja|Nein|String|Beliebige Zeichenkette mit bis zu 255 Zeichen|
|3|Beschreibung Description|Eine von der Einrichtung vergebene Beschreibung für die Vereinbarung|Nein|Nein|String|Bis zu 1Gb Text|
|4|Status Status|Aktueller Status der Vereinbarung|Ja|Nein|Auswahlliste|Auswahlliste teilweise pro Mandant konfigurierbar|
|5|Grund für die Schließung Reason for closure|Für eine abgeschlossene Vereinbarung: der Grund, warum die Vereinbarung geschlossen wurde|Nein|Nein|Auswahlliste|Auswahlliste vollständig pro Mandant konfigurierbar|
|6|Verlängerungspriorität Renewal priority|Um zu erfassen, ob eine Vereinbarung verlängert, überprüft oder gekündigt werden soll|Nein|Nein|Auswahlliste|Auswahlliste vollständig pro Mandant konfigurierbar|
|7|Dauerhafter Zugriff? Perpetual Access?|Um zu erfassen, ob die Vereinbarung eine unbefristete Vereinbarung ist oder nicht|Nein|Nein|Auswahlliste|Auswahlliste nicht konfigurierbar|
|8|Alternativer Name|Ein von der Einrichtung vergebener alternativer Name für die Vereinbarung|Nein|Ja|String|Beliebige Zeichenkette mit bis zu 255 Zeichen|
|9|Vereinbarungszeitraum|Um einen oder mehrere Zeiträume zu erfassen, in denen die Vereinbarung gültig war|Ja|Ja|Vereinbarungszeitraum s. Reihen 9-12|s. Reihen 9-12|
|10|Startdatum|Datum, an dem die Vertragslaufzeit beginnt|Ja|Nein|Datum|beliebiges Datum|
|11|Enddatum|Datum, an dem die Vertragslaufzeit endet|Nein|Nein|Datum|beliebiges Datum nach dem Startdatum|
|12|Stornierungsfrist|Datum, bis zu dem der Anbieter über eine Kündigungsentscheidung innerhalb der Vertragslaufzeit informiert werden muss|Nein|Nein|Datum|beliebiges Datum|
|13|Hinweis zum Zeitraum|Eine Freitext-Notiz, die sich auf den Vertragszeitraum bezieht|Nein|Nein|String|Bis zu 1Gb Text|
|14|Interne Kontakte|Zur Erfassung von Kontakten innerhalb der Bibliothek, die eine Verantwortung oder Rolle in Bezug auf die Vereinbarung haben|Nein|Ja|Interne Kontakte s. Reihen 14-15|Siehe Definition eines internen Kontakts|
|15|Person|Eine Personr mit einer Beziehung zur Vereinbarung|Ja|Nein|Person in der Folio-Personen-App|Jede Folio-Person|
|16|Rolle|Die Rolle/Beziehung, die die Person zur Vereinbarung hat|Ja|Nein|Auswahlliste|Auswahlliste vollständig pro Mandant konfigurierbar|
|17|Vereinbarungskomponente|Zum Erfassen der Ressourcen (entweder Pakete oder einzelne Ressourcen), die Teil der Vereinbarung sind|Nein|Ja|Verinbarungskomponente s. Reihen 17-21|s. Reihen 17-21|
|18|Ressource|Ein Paket oder Titel|Ja|Nein|Ein Paket oder eine Titelressource wie in den Vereinbarungen "Eresources" ODER in eHoldings beschrieben|Vereinbarung, elektronische Ressource oder eHoldings-Paket oder -Titel|
|19|Aktiv ab|Datum, ab dem die Ressource in der Vereinbarung aktiv/gültig war (d. h. Datum, an dem die Ressource der Vereinbarung hinzugefügt wurde)|Nein|Nein|Datum|beliebiges Datum|
|20|Aktiv bis|Datum, bis zu dem die Ressource in der Vereinbarung aktiv/gültig war (d. h. Datum, an dem die Ressource aus der Vereinbarung entfernt wurde)|Nein|Nein|Datum|beliebiges Datum nach dem "Aktiv ab"-Datum|
|21|Bestellposten|Bestellposten, der sich auf die Ressource in der Verinbarungskomponente bezieht|Nein|Nein|Bestellposten in der Folio-Bestellungen-App|Purchase Order Line in the Folio Orders app|
|22|Benutzerdefinierte Abdeckung|Jede benutzerdefinierte Abdeckung (Daten/Bände/Ausgaben der Ressource, die unter der Vereinbarung zugänglich sind), die für die Ressource gilt. Dies gilt nur für Vereinbarungszeilen für Ressourcen, die in der internen eRessourcenliste "Vereinbarungen" beschrieben sind - die benutzerdefinierte Abdeckung für eHoldings-Ressourcen wird direkt in eHoldings festgelegt.|Nein|Ja|Benutzerdefinierte Abdeckung|Die Option "Benutzerdefinierte Abdeckung" ist nur dann relevant, wenn die Vereinbarung eine andere Abdeckung als die von einem Anbieter angebotene Standardabdeckung vorschreibt.  Die Option "Benutzerdefinierte Abdeckung" wird nicht bei Vertragskomponenten für eHoldings-Ressourcen angezeigt.|
|23|Allgemeine Hinweise zum Lizenzvertrag der Vereinbarung|Zum Erfassen allgemeiner Informationen über den Lizenzvertrag für die Vereinbarung|Nein|Nein|String|Beliebige Zeichenkette mit bis zu 255 Zeichen|
|24|Lizenzvertrag|Um eine Verknüpfung zu einem Lizenzvertrag (wie in der Folio-Lizenzverträge-App beschrieben) herzustellen, der die Vereinbarung regelt (oder geregelt hat/regeln wird)|Nein|Ja|Lizenzvertrags-Link s. Reihen 24-27|Siehe Definition eines Lizenzvertrags-Links s. Reihen 24-27|
|25|Lizenzvertrag (Lizenzvertragslink)|Ein Lizenzvertrag, der die Vereinbarung geregelt hat//derzeit regelt/regeln wird|Ja|Nein|Lizenzvertrag in der Folio-Lizenzverträge-App| |
|26|Status (dieser Vereinbarung) (Lizenzvertragslink)|Ob der Lizenzvertrag die Vereinbarung aktuell regelt oder nicht|Ja|Nein|Auswahlliste|Nur ein verknüpfter Lizenzvertrag kann zu einem gegebenen Zeitpunkt den Status "Regelnd" haben. Bei der Anzeige der Lizenzbedingungen, die für die Vereinbarung gelten, werden die Bedingungen aus der regelnden Lizenz (und alle zugehörigen aktiven Lizenzänderungen) verwendet.  Auswahlliste nicht konfigurierbar|
|27|Notiz (Lizenzvertragslink)|Hinweis zur Vereinbarung/Lizenzverknüpfung|Nein|Nein|String|Bis zu 1Gb Text|
|28|Vertragsänderung (Lizenzvertragslink)|Beziehung zwischen etwaigen Lizenzänderungen und der Vereinbarung|Nein|Nein|Vertragsänderungs-Link|Nur Änderungen, die mit dem regelnden Lizenzvertrag verknüpft sind, können die Bedingungen für eine Vereinbarung beeinflussen|
|29|Externer Lizenzvertag|Um ein Dokument zu erfassen, das einen Lizenzvertrag beschreibt, der außerhalb von Folio gespeichert ist und die Vereinbarung regelt|Nein|Ja|Dokument s. Reihen 29-33|Siehe Definition eines Dokuments|
|30|Name (Dokument)|Name für das Dokument|Ja|Nein|String|Beliebige Zeichenkette mit bis zu 255 Zeichen|
|31|Notiz (Dokument)|Freitextnotiz in Bezug auf das Dokument|Nein|Nein|String|Bis zu 1Gb Text|
|32|Physischer Standort (Dokument)|Der physische Standort des Dokuments|Eine der Optionen "Physischer Standort, URL oder Datei" ist erforderlich|Nein|String|Beliebige Zeichenkette mit bis zu 255 Zeichen|
|33|URL (Dokument)|Die URL für das Dokument|Eine der Optionen "Physischer Standort, URL oder Datei" ist erforderlich|Nein|URL|Gültige URL inklusive Protokoll (z. B. http, https)|
|34|Datei (Dokument)|Eine Datei, die das Dokument enthält|Eine der Optionen "Physischer Standort, URL oder Datei" ist erforderlich|Nein|Eine in Folio hochgeladene Datei|Jede Datei mit einer Größe von <200Mb|
|35|Organisation|Um Organisationen zu erfassen, die eine Verantwortung oder Rolle in Bezug auf die Vereinbarung haben|Nein|Ja|Organisationslink s. Reihen 35-36|Siehe Definition eines Organisationslinks|
|36|Organisation (Orgnaisationslink)|Eine Organisation, die eine Beziehung zur Vereinbarung hat|Ja|Nein|Organisation in der Folio-Organisationen-App|Beliebige Folio-Organisation|
|37|Rolle (Organisationslink)|Die Rolle/Beziehung, die die Organisation zur Vereinbarung hat|Ja|Nein|Auswahlliste|Auswahlliste teilweise pro Mandant konfigurierbar|
|38|Ergänzende Informationen|Zum Erfassen von Dokumenten, die Informationen über die Vereinbarung enthalten|Nein|Ja|Dokument s. Reihen 29-33|Siehe Definition eines Dokuments|
|39|Nutzungsdatenquelle|Zur Verknüpfung mit einer Nutzungsdatenquelle (wie in der Folio eUsage App beschrieben), die die Nutzungsdaten für Ressourcen in der Vereinbarung erfasst|Nein|Ja|Nutzungsdatenquelle-Link|Siehe Definition einer Nutzungsdatenquelle|
|40|Nutzungsdatenquelle (Nutzungsdatenquelle-Link)|Ein Anbieter von Nutzungsdaten, der eine Beziehung zur Vereinbarung hat|Ja|Nein|Nutzungsdatenquelle in Folio eUsage-App|Beliebige Nutzungsdatenquelle|
|41|Notiz Nutzungsdatenquelle-Link)|Freitext-Hinweis in Bezug auf die Nutzungsdatenquelle|Nein|Nein|String|Bis zu 1Gb Text|
|42|Zugehörige Vereinbarungen|Zur Verknüpfung mit anderen Vereinbarungen (wie in der Folio eManagement App beschrieben), die mit der Vereinbarung in Zusammenhang stehen|Nein|Ja|Vereinbarungslink s. Reihen 42-44|Siehe Definition eines Vereinbarungslinks s. Reihen 42-44|
|43|Vereinbarung (Vereinbarungslink)|Eine andere Vereinbarung mit einer Beziehung zur Vereinbarung|Ja|Nein|Vereinbarung in Folio eManagement App|Beliebige Folio-Vereinbarung|
|44|Beziehung der verknüpften Vereinbarung zu der Vereinbarung, die bearbeitet wird (Vereinbarungslink)|Die Beziehung, die die verknüpfte Vereinbarung zu der Vereinbarung hat|Ja|Nein|Auswahlliste|Vereinbarungs-Verknüpfungen sind reziprok und die gültigen Werte werden mit ihren reziproken Werten gepaart. Wenn eine Vereinbarungs-Verknüpfung erstellt wird, ist sie von beiden an der Verknüpfung beteiligten Vereinbarungen aus sichtbar und bearbeitbar, wobei die reziproken Wertepaare die Richtung der Beziehung angeben. Die reziproken Wertepaare sind: * ersetzt <-> wird ersetzt von * bietet Post-Cancellation Access für <-> hat Post-Cancellation Access in * zeichnet Demand-Driven Acquisition auf für <-> hat Demand-Driven Acquisition in  Auswahlliste nicht konfigurierbar|
|45|Notiz (Vereinbarungslink)|Freitext-Hinweis in Bezug auf den Vereinbarungslink|Nein|Nein|String|Bis zu 1Gb Text|


# Links
[Feldbeschreibungen aller Apps (Link zum Google Dokument)](https://docs.google.com/spreadsheets/d/1ZpB3-SZwD07E71OVMR1TLie2CZ8wbEq_q1AF-gSGLXo/edit#gid=1148873991)
