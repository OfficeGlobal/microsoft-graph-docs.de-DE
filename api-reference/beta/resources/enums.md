---
title: Enumerationswerte
description: Microsoft Graph-Enumerationswerte
ms.openlocfilehash: 0e748b53d1b89a20e3973ec35aaf53e02d6a3428
ms.sourcegitcommit: 539ed08adf3b7ad3253c98636d4ab303ce00176e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/15/2019
ms.locfileid: "30057050"
---
### <a name="contactrelationship-values"></a>contactRelationship-Werte

|Element|Wert|Beschreibung|
|:---|:---|:---|
|Eltern|0|Das übergeordnete Element des Benutzers.|
|relativ|1| Der relative des Benutzers.|
|aide|2| Die aide des Benutzers.|
|Arzt|3| Der Arzt des Benutzers.|
|Guardian|4| Der Vormund des Benutzers.|
|untergeordneten|5| Das untergeordnete Element des Benutzers.|
|anderen|6| Eine nicht angegebene Beziehung zum Benutzer.|
|Enumerationsmember unknownfuturevalue "|7| Markerwert für zukünftige Kompatibilität.|

### <a name="timezonestandard-values"></a>timeZoneStandard-Werte

| Wert
|:-----------------
| Windows
| IANA


### <a name="availabilitystatus-values"></a>availabilityStatus-Werte

| Wert
|:-------------------------
| unknown
| frei
| mit Vorbehalt
| beschäftigt
| OOF  
| workingElsewhere


### <a name="freebusystatus-values"></a>freeBusyStatus-Werte

| Element            |Wert
|:------------------|:-------
| frei              | 0
| mit Vorbehalt         | 1
| beschäftigt              | 2
| OOF               | 3
| workingElsewhere  | 4
| unknown           | -1


### <a name="addresstype-values"></a>AddressType-Werte

| Wert
|:-------------------------
| unknown 
| Home
| Business 
| anderen


### <a name="physicaladdresstype-values"></a>: Physicaladdresstype-Werte

| Wert
|:-------------------------
| unknown 
| Home
| Business 
| anderen


### <a name="attendeetype-values"></a>attendeeType-Werte

| Wert
|:-------------------------
| erforderlich
| Optional
| resource


### <a name="externalaudiencescope-values"></a>externalAudienceScope-Werte

| Wert
|:-------------------------
| Keine
| contactsOnly
| all


### <a name="automaticrepliesstatus-values"></a>automaticRepliesStatus-Werte

| Wert
|:-------------------------
| deaktiviert
| alwaysEnabled
| Geplant


### <a name="calendarcolor-values"></a>calendarColor-Werte

| Element     | Wert
|:-----------|:----------
| Auto       | -1
| Hellblau  | 0
| Hellgrün | 1
| lightOrange| 2
| lightGray  | 3
| lightYellow| 4
| lightTeal  | 5
| lightPink  | 6
| Hellbraun | 7
| lightRed   | 8
| maxColor   | 9


### <a name="educationsynchronizationprofilestate-values"></a>educationSynchronizationProfileState-Werte

| Element     | Wert
|:-----------|:----------
| Löschen          | 2
| deletionFailed    | 3
| provisioningFailed | 5
| Bereitgestellt        | 6
| Provisioning       | 7
| Enumerationsmember unknownfuturevalue " | 8


### <a name="educationsynchronizationstatus-values"></a>educationSynchronizationStatus-Werte

| Element     | Wert
|:-----------|:----------
| angehalten          | 0
| inProgress    | 1
| Erfolgreich | 2
| error        | 3
| validationError | 4
| Quarantäne       | 5
| Enumerationsmember unknownfuturevalue " | 6

### <a name="educationexternalsource-values"></a>educationExternalSource-Werte

| Wert
|:-------------------------
| SIS
| Manuell
| Enumerationsmember unknownfuturevalue "


### <a name="educationgender-values"></a>educationGender-Werte

| Wert
|:-------------------------
| weiblich
| männlich
| anderen
| Enumerationsmember unknownfuturevalue "


### <a name="eventtype-values"></a>EventType-Werte

| Wert
|:-------------------------
| singleInstance
| vorkommen
| Ausnahme
| seriesMaster


### <a name="sensitivity-values"></a>Vertraulichkeits Werte

| Wert
|:-------------------------
| normal
| personal
| Private
| vertraulich


### <a name="importance-values"></a>Wichtigkeits Werte

| Wert
|:-------------------------
| mit niedriger
| normal
| hohe


### <a name="educationuserrole-values"></a>educationUserRole-Werte
| Wert
|:---------------------
| student
| teacher
| Keine
| Enumerationsmember unknownfuturevalue "


### <a name="meetingmessagetype-values"></a>meetingMessageType-Werte

| Wert
|:-----------------
| Keine
| meetingRequest
| meetingCancelled
| meetingAccepted
| meetingTentativelyAccepted
| meetingDeclined


### <a name="followupflagstatus-values"></a>followupFlagStatus-Werte

| Wert
|:-------------------------
| notFlagged
| complete
| gekennzeichnet


### <a name="inferenceclassificationtype-values"></a>inferenceClassificationType-Werte

| Wert
|:-----------------
| konzentriert
| anderen


### <a name="iosnotificationalerttype-values"></a>iosNotificationAlertType-Werte

| Wert
|:-------------------------
| deviceDefault
| Banner
| modal
| Keine

### <a name="deviceenrollmentfailurereason-values"></a>deviceEnrollmentFailureReason-Werte

| Wert
|:-------------
| unknown
| Authentifizierung
| Autorisierung
| accountValidation
| userValidation
| deviceNotSupported
| inMaintenance
| badRequest
| featureNotSupported
| enrollmentRestrictionsEnforced
| clientDisconnected


### <a name="bodytype-values"></a>BodyType-Werte
| Wert
|:---------
| text
| html


### <a name="locationtype-values"></a>LocationType-Werte

| Wert
|:-------------------------
| default
| Konferenzraum
| homeAddress
| businessAddress
| geoCoordinates
| streetAddress
| Hotel
| Restaurant
| localBusiness
| postalAddress

### <a name="locationuniqueidtype-values"></a>locationUniqueIdType-Werte

| Wert
|:-------------------------
| unknown
| locationStore
| Directory
| Private
| Bing


### <a name="messageactionflag-values"></a>messageActionFlag-Werte

| Wert
|:-------------------------
| Beliebiger Wert
| Aufruf
| doNotForward
| followUp
| FYI
| Weiterleiten
| noResponseNecessary
| Lesen
| Antworten
| replyToAll
| Bewertung


### <a name="onenoteuserrole-values"></a>onenoteUserRole-Werte

| Element      | Wert
|:------------|:------------
| Besitzer       | 0
| Mitwirkender | 1
| Reader      | 2
| Keine        | -1


### <a name="operationstatus-values"></a>operationStatus-Werte

| Wert
|:-----------------
| NotStarted
| Wird ausgeführt
| Completed
| Failed


### <a name="onenotepatchactiontype-values"></a>onenotePatchActionType-Werte

| Wert
|:-------------------------
| Ersetzen
| Anfügeabfrage
| Löschen
| Einfügen
| Voranstellen

### <a name="onenotepatchinsertposition-values"></a>onenotePatchInsertPosition-Werte

| Wert
|:-------------------------
| After
| Bevor


### <a name="phonetype-values"></a>phoneType-Werte

| Wert
|:-------------------------
| Home
| Business
| Mobile
| anderen
| Assistent
| homeFax
| businessFax
| otherFax
| Pager
| Radio


### <a name="plannerpreviewtype-values"></a>plannerPreviewType-Werte

| Wert
|:-------------------------
| Automatisch
| noPreview
| checklist
| description
| Referenz


### <a name="status-values"></a>Statuswerte

| Wert
|:-----------------
| Active
| updated
| deleted
| ignoriert
| Enumerationsmember unknownfuturevalue "


### <a name="weekindex-values"></a>weekIndex-Werte

| Wert
|:-------------------------
| ersten
| zweiten
| Dritt
| vierten
| Last


### <a name="dayofweek-values"></a>dayOfWeek-Werte

| Wert
|:-------------------------
| Sonntag
| Montag
| Dienstag
| Mittwoch
| Donnerstag
| Freitag
| Samstag

### <a name="recurrencepatterntype-values"></a>recurrencePatternType-Werte

| Wert
|:-------------------------
| täglich
| Downloads
| absoluteMonthly
| relativeMonthly
| absoluteYearly
| relativeYearly


### <a name="recurrencerangetype-values"></a>recurrenceRangeType-Werte

| Wert
|:-------------------------
| endDate
| noEnd
| nummeriert


### <a name="onenotesourceservice-values"></a>onenoteSourceService-Werte
| Wert
|:---------------------
| Unbekannt
| OneDrive
| OneDriveForBusiness
| OnPremOneDriveForBusiness


### <a name="responsetype-values"></a>ResponseType-Werte

| Wert
|:-------------------------
| Keine
| organizer
| tentativelyAccepted
| akzeptierte
| abgelehnt
| notResponded


### <a name="activitydomain-values"></a>activityDomain-Werte

| Wert
|:-------------------------
| unknown
| work
| personal
| unrestricted


### <a name="websitetype-values"></a>WebSiteType-Werte

| Wert
|:-------------------------
| anderen
| Home
| work
| Blog
| profile


### <a name="categorycolor-values"></a>categoryColor-Werte

| Element   |Wert    
|:---------|:--------
| Keine     | -1      
| preset0  | 0       
| preset1  | 1       
| preset2  | 2       
| preset3  | 3       
| preset4  | 4       
| preset5  | 5       
| preset6  | 6       
| preset7  | 7       
| preset8  | 8       
| PRESET9  | 9       
| preset10 | 10      
| preset11 | 11      
| preset12 | 12      
| preset13 | 13      
| preset14 | 14      
| preset15 | 15      
| preset16 | 16      
| preset17 | 17      
| preset18 | 18      
| preset19 | 19      
| preset20 | 20      
| preset21 | 21      
| preset22 | 22      
| preset23 | 23      
| preset24 | 24      

### <a name="alertfeedback-values"></a>alertFeedback-Werte

Mögliche Feedback Werte für die Warnung, die von einem Analysten bereitgestellt wird.

|Element|Wert|Beschreibung|
|:---|:---|:---|
|unknown|0|Unbekannt.|
|truePositive|1|Alert ist true-positive.|
|falsePositive|2| Alert ist falsch-positiv.|
|benignPositive|3| Alert ist positiv.|

### <a name="filehashtype-values"></a>fileHashtype-Werte

|Element|Wert|Beschreibung|
|:---|:---|:---|
|unknown|0|UnBekannter Typ.|
|SHA1|1|SHA1-Hashtyp.|
|SHA256|2| SHA256-Hashtyp.|
|MD5|3| MD5-Hashtyp.|
|authenticodeHash256|4| AuthenticodeHash256-Hashtyp.|
|lsHash|5| LsHash-Hashtyp.|
|CTPH|6| CTPH-Hashtyp.|
|peSha1|7| PESHA1-Hashtyp.|
|peSha256|8| PESHA256-Hashtyp.|

### <a name="connectiondirection-values"></a>connectionDirection-Werte

|Element|Wert|Beschreibung|
|:---|:---|:---|
|unknown|0|Unbekannte Verbindung.|
|Inbound|1|Eingehende Verbindung.|
|Outbound|2| Ausgehende Verbindung.|

### <a name="connectionstatus-values"></a>connectionStatus-Werte

|Element|Wert|Beschreibung|
|:---|:---|:---|
|unknown|0|UnBekannter Verbindungsstatus.|
|versucht|1|Verbindung wurde versucht.|
|succeeded|2| Verbindung erfolgreich.|
|gesperrt|3| Verbindung blockiert.|
|failed|4| Fehler bei Verbindung.|

### <a name="processintegritylevel-values"></a>processIntegrityLevel-Werte

|Element|Wert|Beschreibung|
|:---|:---|:---|
|unknown|0|Unbekannt.|
|nicht vertrauenswürdigen|10|Integritätsebene ist nicht vertrauenswürdig.|
|mit niedriger|20| Integritätsstufe ist niedrig.|
|medium|30| Integritätsstufe ist Mittel.|
|hohe|40| Integritätsebene ist hoch.|
|System|50| Integritätsstufe ist System.|

### <a name="registryhive-values"></a>registryHive-Werte

Enum für Registrierungsstrukturen gemäß der Definition von [https://docs.microsoft.com/en-us/windows/desktop/sysinfo/registry-hives](https://docs.microsoft.com/en-us/windows/desktop/sysinfo/registry-hives).

|Element|Wert|Beschreibung|
|:---|:---|:---|
|unknown|0|Unbekannte Struktur.|
|currentConfig|1|HKEY_CURRENT_CONFIG-Hive.|
|currentUser|2| HKEY_CURRENT_USER-Struktur.|
|localMachineSam|3| HKEY_LOCAL_MACHINE\SAM-Hive.|
|localMachineSamSoftware|4| HKEY_LOCAL_MACHINE\Software-Hive.|
|localMachineSystem|5| HKEY_LOCAL_MACHINE\System-Hive.|
|usersDefault|6| HKEY_USERS\\. Standardstruktur.|

### <a name="registryoperation-values"></a>registryOperation-Werte

Vorgang, der den Namen und/oder Wert des Registrierungsschlüssels geändert hat.

|Element|Wert|Beschreibung|
|:---|:---|:---|
|unknown|0|UnBekannter Registrierungs Werttyp.|
|create|1|Erstellen Sie die Registrierung.|
|Ändern|2|Ändern Sie die Registrierung.|
|Löschen|3|Registrierung löschen.|

### <a name="registryvaluetype-values"></a>registryValueType-Werte

Enum für Registrierungswert Typen gemäß der Definition [https://docs.microsoft.com/en-us/windows/desktop/sysinfo/registry-value-types](https://docs.microsoft.com/en-us/windows/desktop/sysinfo/registry-value-types)von.

|Element|Wert|Beschreibung|
|:---|:---|:---|
|unknown|0|UnBekannter Registrierungs Werttyp.|
|Binär|1|REG_BINARY-Registrierungs Werttyp.|
|DWORD|2| REG_DWORD-Registrierungs Werttyp.|
|dwordLittleEndian|3| REG_DWORD_LITTLE_ENDIAN-Registrierungs Werttyp.|
|dwordBigEndian|4| REG_DWORD_BIG_ENDIAN-Registrierungs Werttyp.|
|expandSz|5| REG_EXPAND_SZ-Registrierungs Werttyp.|
|Link|6| REG_LINK-Registrierungs Werttyp.|
|multiSz|7| REG_MULTI_SZ-Registrierungs Werttyp.|
|Keine|8| REG_NONE-Registrierungs Werttyp.|
|QWord|9| REG_QWORD-Registrierungs Werttyp.|
|qwordlittleEndian|10| REG_QWORD_LITTLE_ENDIAN-Registrierungs Werttyp.|
|SZ|11| REG_SZ-Registrierungs Werttyp.|

### <a name="alertseverity-values"></a>alertSeverity-Werte

Enum für den Schweregrad der Warnungen.

|Element|Wert|Beschreibung|
|:---|:---|:---|
|unknown|0|Schweregrad ist unbekannt.|
|Informations|1|Der Schweregrad dient nur zur Information.|
|mit niedriger|2| Schweregrad ist niedrig.|
|medium|3| Schweregrad ist Mittel.|
|hohe|4| Schweregrad ist hoch.|

### <a name="alertstatus-values"></a>alertStatus-Werte

Mögliche Werte eines Warnungs Lebenszyklusstatus (Stufe).

|Element|Wert|Beschreibung|
|:---|:---|:---|
|unknown|0|UnBekannter Status.|
|neuWarnung|10| Alert ist neu.|
|inProgress|20|Warnung wird ausgeführt.|
|aufgelöst|30|Warnung ist aufgelöst.|

### <a name="emailrole-values"></a>emailRole-Werte

Mögliche Werte für e-Mail-Rollen.

|Element|Wert|Beschreibung|
|:---|:---|:---|
|unknown|0|Unbekannte Rolle.|
|sender|1|Absender der e-Mail.|
|Empfänger|2|Empfänger der e-Mail.|

### <a name="logontype-values"></a>LoginType-Werte

Mögliche Werte für die Methode der Benutzeranmeldung.

|Element|Wert|Beschreibung|
|:---|:---|:---|
|unknown|-1|Unbekannt.|
|interaktive|0|Die Anmeldung ist interaktiv.|
|remoteInteractive|1| Die Anmeldung ist Remote interaktiv.|
|Netzwerk|2| Die Anmeldung ist Network.|
|batch|3| Die Anmeldung ist Batch.|
|service|4| Anmeldung ist Dienst.|

### <a name="useraccountsecuritytype-values"></a>userAccountSecurityType-Werte

Mögliche Werte für Benutzerkonto Typen (Gruppenmitgliedschaft), pro Windows-Definition.

|Element|Wert|Beschreibung|
|:---|:---|:---|
|unknown|-1|Unbekannt.|
|Standard|0|Mitglied der Standard Benutzergruppe.|
|macht|1| Mitglied der Gruppe der Hauptbenutzer.|
|Administrator|2| Mitglied der Gruppe Administratoren.|
