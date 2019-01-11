---
title: user-Ressourcentyp
description: Stellt ein Azure AD-Benutzerkonto dar. Erbt von directoryObject.
author: dkershaw10
localization_priority: Priority
ms.openlocfilehash: d9f15cd6f0b3169370257578f841a1821593f351
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27862496"
---
# <a name="user-resource-type"></a>user-Ressourcentyp

Stellt ein Azure AD-Benutzerkonto dar. Erbt von [directoryObject](directoryobject.md).

Diese Ressource unterstützt Folgendes:

- Hinzufügen von Ihren eigenen Daten zu benutzerdefinierten Eigenschaften als [Extensions](/graph/extensibility-overview).
- Abonnieren von [Benachrichtigungen zu ändern](/graph/webhooks).
- Verwenden einer [Delta-Abfrage](/graph/delta-query-overview) zum Nachverfolgen von inkrementellen Hinzufügungen, Löschungen und Aktualisierungen durch Bereitstellen der [delta](../api/user-delta.md)-Funktion.

## <a name="methods"></a>Methoden

| Methode       | Rückgabetyp  |Beschreibung|
|:---------------|:--------|:----------|
|[Benutzer auflisten](../api/user-list.md) |[Benutzersammlung](user.md)| Dient zum Abrufen einer Liste von Benutzerobjekten.|
|[Benutzer erstellen](../api/user-post-users.md) |[Benutzer](user.md)| Dient zum Erstellen eines neuen Benutzerobjekts.|
|[Benutzer abrufen](../api/user-get.md) | [user](user.md) |Liest Eigenschaften und Beziehungen des Benutzerobjekts.|
|[Update user](../api/user-update.md) | [user](user.md) |Aktualisiert das Benutzerobjekt. |
|[Delete user](../api/user-delete.md) | None |Löscht das Benutzerobjekt. |
|[List messages](../api/user-list-messages.md) |[Message](message.md) collection| Ruft alle Nachrichten im Postfach des angemeldeten Benutzers ab.|
|[Create Message](../api/user-post-messages.md) |[Message](message.md)| Erstellt eine neue Nachricht durch Veröffentlichung in der Nachrichtensammlung.|
|[List mailFolders](../api/user-list-mailfolders.md) |[MailFolder](mailfolder.md) collection| Ruft die E-Mail-Ordner-Sammlung unter dem Stammordner des angemeldeten Benutzers ab. |
|[Create mailFolder](../api/user-post-mailfolders.md) |[MailFolder](mailfolder.md)| Erstellt einen neuen MailFolder durch Veröffentlichung in der mailFolders-Sammlung.|
|[sendMail](../api/user-sendmail.md)|None|Sendet die im Anforderungstext angegebene Nachricht.|
|[List events](../api/user-list-events.md) |[Event](event.md) collection| Ruft eine Liste der event-Objekte im Postfach des Benutzers ab. Die Liste enthält einzelne Instanzen von Besprechungen und Serienmaster.|
|[Ereignis erstellen](../api/user-post-events.md) |[Event](event.md)| Erstellt ein neues Ereignis durch Veröffentlichen in der Ereignissammlung.|
|[List calendars](../api/user-list-calendars.md) |[Calendar](calendar.md) collection| Ruft eine Kalenderobjektsammlung ab.|
|[Create calendar](../api/user-post-calendars.md) |[Calendar](calendar.md)| Erstellt einen neuen Kalender durch Veröffentlichung in der Kalendersammlung.|
|[List calendarGroups](../api/user-list-calendargroups.md) |[CalendarGroup](calendargroup.md) collection| Ruft eine CalendarGroup-Objektsammlung ab.|
|[Create calendarGroup](../api/user-post-calendargroups.md) |[CalendarGroup](calendargroup.md)| Erstellt eine neue CalendarGroup durch Veröffentlichung in der CalendarGroups-Sammlung.|
|[List calendarView](../api/user-list-calendarview.md) |[Event](event.md) collection| Ruft eine Ereignisobjektsammlung ab.|
|[List contacts](../api/user-list-contacts.md) |[Contact](contact.md) collection| Ruft eine Kontaktsammlung aus dem Standardkontaktordner des angemeldeten Benutzers ab.|
|[Create Contact](../api/user-post-contacts.md) |[Kontakt](contact.md)| Erstellt einen neuen Kontakt durch Veröffentlichung in der Kontaktsesammlung.|
|[List contactFolders](../api/user-list-contactfolders.md) |[ContactFolder](contactfolder.md) collection| Ruft die Kontaktordnersammlung im Standardkontaktordner des angemeldeten Benutzers ab.|
|[Create ContactFolder](../api/user-post-contactfolders.md) |[ContactFolder](contactfolder.md)| Erstellt einen neuen ContactFolder durch Veröffentlichung in der ContactFolders-Sammlung.|
|[List directReports](../api/user-list-directreports.md) |[directoryObject](directoryobject.md) collection| Ruft die Benutzer und Kontakte, die an den Benutzer berichten, aus der directReports-Navigationseigenschaft ab.|
|[List manager](../api/user-list-manager.md) |[directoryObject](directoryobject.md) | Ruft den Benutzer oder Kontakt, der Vorgesetzter dieses Benutzers ist, aus der manager-Navigationseigenschaft ab.|
|[List memberOf](../api/user-list-memberof.md) |[directoryObject](directoryobject.md) collection| Ruft die Gruppen und Verzeichnisrollen, bei denen dieser Benutzer direktes Mitglied ist, aus der memberOf-Navigationseigenschaft ab.|
|[List ownedDevices](../api/user-list-owneddevices.md) |[directoryObject](directoryobject.md) collection| Ruft die Geräte, die dem Benutzer gehören, aus der ownedDevices-Navigationseigenschaft ab.|
|[List ownedObjects](../api/user-list-ownedobjects.md) |[directoryObject](directoryobject.md) collection| Ruft die Verzeichnisobjekte, die dem Benutzer gehören, aus der ownedDevices-Navigationseigenschaft ab.|
|[List registeredDevices](../api/user-list-registereddevices.md) |[directoryObject](directoryobject.md) collection| Ruft die Geräte, die für den Benutzer registriert sind, aus der registeredDevices-Navigationseigenschaft ab.|
|[List createdObjects](../api/user-list-createdobjects.md) |[directoryObject](directoryobject.md) collection| Ruft die Verzeichnisobjekte, die von dem Benutzer erstellt wurden, aus der createdObjects-Navigationseigenschaft ab.|
|[assignLicense](../api/user-assignlicense.md)|[Benutzer](user.md)|Fügt Abonnements für den Benutzer hinzu bzw. entfernt sie. Sie können auch bestimmte Pläne aktivieren oder deaktivieren, die mit einem Abonnement verknüpft sind.|
|[licenseDetails auflisten](../api/user-list-licensedetails.md) |[licenseDetails](licensedetails.md)-Sammlung| Dient zum Abrufen einer licenseDetails-Objektsammlung.|
|[checkMemberGroups](../api/user-checkmembergroups.md)|String collection|Sucht nach einer Mitgliedschaft in einer Liste von Gruppen. Die Überprüfung ist transitiv.|
|[getMemberGroups](../api/user-getmembergroups.md)|String collection|Gibt alle Gruppen zurück, bei denen der Benutzer Mitglied ist. Die Überprüfung ist transitiv.|
|[getMemberObjects](../api/user-getmemberobjects.md)|Zeichenfolgenauflistung| Gibt alle Gruppen und Verzeichnisrollen zurück, bei denen der Benutzer ein Mitglied ist. Die Überprüfung ist transitiv. |
|[reminderView](../api/user-reminderview.md)|[Reminder](reminder.md) collection|Gibt eine Liste von Kalendererinnerungen innerhalb der angegebenen Start- und Endzeiten zurück.|
|[delta](../api/user-delta.md)|Benutzersammlung| Dient zum Abrufen inkrementeller Änderungen für Benutzer. |
|**Offene Erweiterungen**| | |
|[Offene Erweiterung erstellen](../api/opentypeextension-post-opentypeextension.md) |[openTypeExtension](opentypeextension.md)| Erstellt eine offene Erweiterung und fügt benutzerdefinierte Eigenschaften zu einer neuen oder vorhandenen Ressource hinzu.|
|[Offene Erweiterung abrufen](../api/opentypeextension-get.md) |[openTypeExtension](opentypeextension.md)-Sammlung| Dient zum Abrufen einer offenen Erweiterung, die durch den Erweiterungsnamen identifiziert wird.|
|**Schemaerweiterungen**| | |
|[Schemaerweiterungswerte hinzufügen](/graph/extensibility-schema-groups) || Dient zum Erstellen einer Schemaerweiterungsdefinition und anschließenden Verwenden der Definition zum Hinzufügen benutzerdefinierter typisierter Daten zu einer Ressource.|

## <a name="properties"></a>Eigenschaften

| Eigenschaft       | Typ    |Beschreibung|
|:---------------|:--------|:----------|
|aboutMe|String|Ein Freihandform-Texteingabefeld, in dem der Benutzer sich selbst beschreiben kann.|
|accountEnabled|Boolean| **true**, wenn das Konto aktiviert ist; andernfalls **false**. Diese Eigenschaft ist erforderlich, wenn ein Benutzer erstellt wird. Unterstützt $filter.    |
|ageGroup|String|Die ALTER Gruppe des Benutzers festgelegt. Zulässige Werte: `null`, `minor`, `notAdult` und `adult`. Die [rechtliche Alter mitgliedergruppendefinitionen-Eigenschaft](#legal-age-group-property-definitions) für Weitere Informationen finden Sie unter. |
|assignedLicenses|[assignedLicense](assignedlicense.md) collection|Die Lizenzen, die dem Benutzer zugewiesen sind. Lässt keine NULL-Werte zu.            |
|assignedPlans|[assignedPlan](assignedplan.md)-Sammlung|Die Pläne, die dem Benutzer zugewiesen sind. Schreibgeschützt. Lässt keine NULL-Werte zu. |
|birthday|DateTimeOffset|Der Geburtstag des Benutzers. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`|
|businessPhones|String-Sammlung|Die Telefonnummern für den Benutzer. HINWEIS: Obwohl dies eine String-Sammlung ist, kann nur eine Nummer für diese Eigenschaft festgelegt werden.|
|Ort|String|Die Stadt, in der sich der Benutzer befindet. Unterstützt $filter.|
|companyName | String | Der Unternehmensname, dem der Benutzer zugewiesen ist. Schreibgeschützt. |
|consentProvidedForMinor|String|Legt fest, ob Zustimmung für Minderjährige abgerufen wurde. Zulässige Werte: `null`, `granted`, `denied` und `notRequired`. Die [rechtliche Alter mitgliedergruppendefinitionen-Eigenschaft](#legal-age-group-property-definitions) für Weitere Informationen finden Sie unter.|
|Land|String|Land/Region, in dem/der sich der Benutzer befindet; z. B. „USA“ oder „UK“. Unterstützt $filter.|
|createdDateTime | DateTimeOffset |Das Erstellungsdatum des User-Objekts. |
|department|String|Der Name der Abteilung, in der der Benutzer arbeitet. Unterstützt $filter.|
|displayName|String|cDer Name, der im Adressbuch für den Benutzer angezeigt wird. Dies ist normalerweise eine Kombination aus dem Vornamen, der Initiale des weiteren Vornamens und des Nachnamens. Diese Eigenschaft ist beim Erstellen eines Benutzers erforderlich und kann nicht bei Updates deaktiviert werden. Unterstützt $Filter und $orderby.|
|givenName|String|Der Vorname des Benutzers. Unterstützt $filter.|
|hireDate|DateTimeOffset|Das Einstellungsdatum des Benutzers. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`|
|id|String|Der eindeutige Bezeichner des Benutzers. Geerbt von [directoryObject](directoryobject.md). Key. Lässt keine Nullwerte zu. Schreibgeschützt.|
|imAddresses|String-Sammlung|Die VOIP-SIP-Adressen (Voice oder IP; Session Initiation Protocol) der Chatnachricht für den Benutzer. Schreibgeschützt.|
|interests|Zeichenfolgenauflistung|Eine Liste für den Benutzer, um dessen Interessen zu beschreiben.|
|jobTitle|String|Die Position des Benutzers. Unterstützt $filter.|
|legalAgeGroupClassification|String| Wird von enterpriseanwendungen verwendet, um der Altersgruppe Legal des Benutzers zu bestimmen. Diese Eigenschaft ist schreibgeschützt und berechnete basierend auf `ageGroup` und `consentProvidedForMinor` Eigenschaften. Zulässige Werte: `null`, `minorWithOutParentalConsent`, `minorWithParentalConsent`, `minorNoParentalConsentRequired`, `notAdult` und `adult`. Verweisen Sie auf die [Legal Alter mitgliedergruppendefinitionen-Eigenschaft](#legal-age-group-property-definitions) für Weitere Informationen.)|
|mail|String|Die SMTP-Adresse des Benutzers, z. B. „jeff@contoso.onmicrosoft.com“. Schreibgeschützt. Unterstützt $filter.|
|mailboxSettings|[mailboxSettings](mailboxsettings.md)|Einstellungen für das primäre Postfach des angemeldeten Benutzers. Sie können Einstellungen für das Senden von automatischen Antworten auf eingehende Nachrichten, das Gebietsschema und die Zeitzone [abrufen](../api/user-get-mailboxsettings.md) oder [aktualisieren](../api/user-update-mailboxsettings.md).|
|mailNickname|String|Der E-Mail-Alias für den Benutzer. Diese Eigenschaft muss beim Erstellen eines Benutzers angegeben werden. Unterstützt $filter.|
|mobilePhone|String|Die Nummer des primären Mobiltelefons für den Benutzer.|
|mySite|String|Die URL für die persönliche Website des Benutzers.|
|officeLocation|String|Der Bürostandort der Firma des Benutzers|
|onPremisesDomainName|String| Enthält lokale `domainFQDN`, auch als bezeichnet DnsDomänenName aus dem lokalen Verzeichnis synchronisiert. Die Eigenschaft wird nur für Kunden aufgefüllt, die ihre lokalen Verzeichnis zu Azure Active Directory über Azure AD-Connect synchronisiert werden. Schreibgeschützt. |
|onPremisesExtensionAttributes|[OnPremisesExtensionAttributes](onpremisesextensionattributes.md)|"Extensionattributes" 1-15 für den Benutzer enthält. Beachten Sie, dass der einzelnen Erweiterungsattribute auswählbar weder gefiltert werden. Für eine `onPremisesSyncEnabled` Benutzer, diese Gruppe von Eigenschaften ist dem Format mastered lokale und ist schreibgeschützt. Für einen Benutzer nur-Cloud-(wobei `onPremisesSyncEnabled` ist false), können diese Eigenschaften festgelegt werden, während der Erstellung oder zu aktualisieren. |
|onPremisesImmutableId|String|Diese Eigenschaft wird verwendet, um eine lokale Active Directory-Benutzerkonto in ihrer Azure AD-Benutzerobjekt zuordnen. Diese Eigenschaft muss angegeben werden, wenn ein neues Benutzerkonto im Diagramm erstellen, wenn Sie eine verbunddomäne für die Benutzereigenschaft **UserPrincipalName** (UPN) verwenden. **Wichtig:** Die **$** und **\_** Zeichen können nicht verwendet werden, wenn Sie diese Eigenschaft festlegen. Unterstützt $filter.                            |
|onPremisesLastSyncDateTime|DateTimeOffset|Gibt den letzten Zeitpunkt an, zu dem das Objekt mit dem lokalen Verzeichnis synchronisiert wurde. Beispiel: „2013-02-16T03:04:54Z“. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`. Schreibgeschützt.|
|onPremisesProvisioningErrors|[OnPremisesProvisioningError](onpremisesprovisioningerror.md) -Auflistung| Fehler beim Microsoft Synchronisierung während der Bereitstellung verwenden. |
|onPremisesSamAccountName|String| Enthält lokale `samAccountName` aus dem lokalen Verzeichnis synchronisiert. Die Eigenschaft wird nur für Kunden aufgefüllt, die ihre lokalen Verzeichnis zu Azure Active Directory über Azure AD-Connect synchronisiert werden. Schreibgeschützt. |
|onPremisesSecurityIdentifier|String|Enthält die lokale Sicherheits-ID (SID) für den Benutzer, der von der lokalen Bereitstellung in der Cloud synchronisiert wurde. Schreibgeschützt.|
|onPremisesSyncEnabled|Boolean| **true**, wenn das Objekt aus einem lokalen Verzeichnis synchronisiert wird; **false**, wenn das Objekt ursprünglich aus einem lokalen Verzeichnis synchronisiert wurde, aber nicht mehr synchronisiert wird; **NULL**, wenn dieses Objekt nie aus einem lokalen Verzeichnis synchronisiert wurde (Standard). Schreibgeschützt |
|onPremisesUserPrincipalName|String| Enthält lokale `userPrincipalName` aus dem lokalen Verzeichnis synchronisiert. Die Eigenschaft wird nur für Kunden aufgefüllt, die ihre lokalen Verzeichnis zu Azure Active Directory über Azure AD-Connect synchronisiert werden. Schreibgeschützt. |
|passwordPolicies|String|Gibt die Kennwortrichtlinien für den Benutzer an. Dieser Wert ist eine Enumeration, deren einziger möglicher Wert „DisableStrongPassword“ lautet. Damit können schwächere Kennwörter als in der Standardrichtlinie angegeben festgelegt werden. Auch „DisablePasswordExpiration“ kann angegeben werden. Beide können zusammen angegeben werden, z. B.: „DisablePasswordExpiration, DisableStrongPassword“.|
|passwordProfile|[PasswordProfile](passwordprofile.md)|Gibt das Kennwortprofil für den Benutzer an. Das Profil enthält das Kennwort des Benutzers. Diese Eigenschaft ist erforderlich, wenn ein Benutzer erstellt wird. Das Kennwort im Profil muss den Mindestanforderungen entsprechen, wie von der **passwordPolicies**-Eigenschaft angegeben. Standardmäßig ist ein sicheres Kennwort erforderlich.|
|pastProjects|Zeichenfolgenauflistung|Eine Liste zur Aufzählung der erledigten Projekte eines Benutzers.|
|postalCode|String|Die Postleitzahl für die Postanschrift des Benutzers. Die Postleitzahl ist für das Land/die Region des Benutzers spezifisch. In den USA enthält dieses Attribut den ZIP Code.|
|preferredDataLocation|String|Die bevorzugte Datenspeicherort für den Benutzer. Weitere Informationen finden Sie unter [OneDrive Online Multi-Geo](https://docs.microsoft.com/sharepoint/dev/solution-guidance/multigeo-introduction).|
|preferredLanguage|String|Die bevorzugte Sprache für den Benutzer. Muss im ISO 639-1-Code angegeben werden. Beispiel: „en-US“.|
|preferredName|String|Der bevorzugte Name für den Benutzer.|
|provisionedPlans|[ProvisionedPlan](provisionedplan.md) collection|Die Pläne, die für den Benutzer bereitgestellt wurden. Schreibgeschützt. Lässt keine NULL-Werte zu. |
|proxyAddresses|Zeichenfolgenauflistung|Beispiel: `["SMTP: bob@contoso.com", "smtp: bob@sales.contoso.com"]` Der **any**-Operator ist für Filterausdrücke für mehrwertige Eigenschaften erforderlich. Schreibgeschützt, lässt keine NULL-Werte zu. Unterstützt $filter.          |
|responsibilities|Zeichenfolgenauflistung|Eine Liste zur Aufzählung der Verantwortlichkeiten eines Benutzers.|
|schools|Zeichenfolgenauflistung|Eine Liste zur Aufzählung der vom Benutzer besuchten Schulen.|
|skills|Zeichenfolgenauflistung|Eine Liste zur Aufzählung der Qualifikationen eines Benutzers.|
|state|String|Bundesland oder Kanton in der Adresse des Benutzers. Unterstützt $filter.|
|streetAddress|String|Die Straße der Firma des Benutzers.|
|surname|Zeichenfolge|Der Nachname des Benutzers. Unterstützt $filter.|
|usageLocation|String|Ein aus zwei Buchstaben bestehender Ländercode (ISO-Standard 3166). Erforderlich für Benutzer, denen Lizenzen zugewiesen werden, aufgrund der gesetzlichen Vorschrift, dass die Verfügbarkeit von Diensten in einzelnen Ländern geprüft werden muss.  Beispiele sind: „US“, „JP“ und „GB“. Lässt keine NULL-Werte zu. Unterstützt $filter.|
|userPrincipalName|String|Der User Principal Name (UPN) des Benutzers. Der UPN ist ein Anmeldename des Benutzers im Internetformat, der auf dem Internetstandard RFC 822 basiert. Gemäß der Konvention sollte er dem E-Mail-Namen des Benutzers zugeordnet sein. Das allgemeine Format lautet „alias@domäne“, wobei „domäne“ in der Sammlung der verifizierten Domänen des Mandanten vorhanden sein muss. Diese Eigenschaft ist erforderlich, wenn ein Benutzer erstellt wird. Auf die verifizierten Domänen für den Mandanten kann über die **verifiedDomains** -Eigenschaft von [organization](organization.md) zugegriffen werden. Unterstützt $Filter und $orderby.
|userType|String|Ein Zeichenfolgenwert kann zum Klassifizieren der Benutzertypen in Ihrem Verzeichnis verwendet werden, z. B. „Member“ und „Guest“. Unterstützt $filter.          |

### <a name="legal-age-group-property-definitions"></a>Legal Alter mitgliedergruppendefinitionen-Eigenschaft

In diesem Abschnitt wird erläutert, wie die drei Gruppeneigenschaften Alter (`legalAgeGroupClassification`, `ageGroup` und `consentProvidedForMinor`) werden von Azure AD-Administratoren und Anwendungsentwickler Enterprise verwendet, um die ALTER-bezogene Auflagen erfüllen.

Beispiel: Cameron ist Administrator eines Verzeichnisses für eine Grundschule in Holyport im Vereinigten Königreich. Am Anfang des Jahres School wird er die Aufnahmen Unterlagen Zustimmung von der Minor übergeordneten Elementen basierend auf den Alter-bezogene Vorschriften der im Vereinigten Königreich abgerufen. Die Zustimmung des übergeordneten Objekts kann die Nebenversionsnummer Konto von Holyport Schule und Microsoft apps verwendet werden. Cameron klicken Sie dann alle Konten erstellt und AgeGroup auf "minor" und "erteilt" ConsentProvidedForMinor festgelegt. Durch seinen Studenten verwendete Anwendungen können dann Features zu unterdrücken, die nicht für Minderjährige geeignet sind.

#### <a name="legal-age-group-classification"></a>Legal Alter Gruppe Klassifikation

Diese Eigenschaft schreibgeschützt wird von Enterprise-Anwendungsentwickler verwendet, um sicherzustellen, dass die richtige Handhabung eines Benutzers basierend auf ihrer Legal Altersgruppe. Es wird berechnet, basierend auf dem Benutzer `ageGroup` und `consentProvidedForMinor` Eigenschaften.

| Wert    | #  |Beschreibung|
|:---------------|:--------|:----------|
|null|0|Standardwert nicht `ageGroup` für den Benutzer festgelegt wurde.|
|minorWithoutParentalConsent |1|(Für die zukünftige Verwendung reserviert)|
|minorWithParentalConsent|2| Der Benutzer ist ein Minor basierend auf dem Alter-bezogene Vorschriften ihres Landes betrachtet oder Region und der Administrator des Kontos aus Erziehungsberechtigte entsprechende Zustimmung erhalten hat.|
|oben|3|Der Benutzer betrachtet basierend auf der ALTER-bezogene Vorschriften ihrer Land oder Region oben.|
|notAdult|4|Der Benutzer hat ihren Ursprung einem Land oder Region, die zusätzliche Alter-bezogene Vorschriften (beispielsweise USA, Vereinigtes Königreich, Europäische Union oder South Korea) verfügt, und das Alter des Benutzers ist zwischen einem Minor und ein Versender nicht jugendfreier Alter (als vorgesehenen basierend auf Land oder Region). Im Allgemeinen, dies bedeutet, dass Teenager als gelten `notAdult` in regulierten Ländern.|
|minorNoParentalConsentRequired|5|Der Benutzer ist ein Minor aber aus einem Land oder Region, die keine Vorschriften Alter-bezogene hat.|

#### <a name="age-group-and-minor-consent"></a>Alter Gruppe und minor Zustimmung

Die ALTER Gruppe und minor Zustimmung sind optionalen Eigenschaften von Azure AD-Administratoren verwendet, um sicherzustellen, dass die Verwendung eines Kontos ordnungsgemäß basierend auf der ALTER-bezogene behördlichen Vorschriften für Land oder Region des Benutzers behandelt wird.

#### <a name="agegroup-property"></a>AgeGroup-Eigenschaft

| Wert    | #  |Beschreibung|
|:---------------|:--------|:----------|
|null|0|Standardwert nicht `ageGroup` für den Benutzer festgelegt wurde.|
|minor|1|Der Benutzer ist ein Minor berücksichtigen.|
|notAdult|2|Der Benutzer ist aus einem Land, die gesetzliche Vorschriften, USA, Vereinigtes Königreich, Europäische Union oder South Korea hat) und Alter des Benutzers ist größer als die obere Grenze der Kind Alter (gemäß den Anweisungen in Land) und weniger als untere Grenze der Versender nicht jugendfreier Alter (als vorgesehenen basierend auf Land oder Region) . Teenager praktisch, gelten als `notAdult` in regulierten Ländern.|
|oben|3|Der Benutzer sollte wie oben behandelten sein.|

#### <a name="consentprovidedforminor-property"></a>ConsentProvidedForMinor-Eigenschaft

| Wert    | #  |Beschreibung|
|:---------------|:--------|:----------|
|null|0|Standardwert nicht `consentProvidedForMinor` für den Benutzer festgelegt wurde.|
|erteilt|1|Der Benutzer über ein Konto verfügen hat Einwilligung wurde.|
|denied|2|Zustimmung wurde nicht für den Benutzer ein Konto abgerufen wurden.|
|notRequired|3|Der Benutzer ist an einem Standort, der keine Zustimmung erforderlich ist.|
 
## <a name="relationships"></a>Beziehungen

| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|Aktivitäten|[UserActivity](projectrome-activity.md) -Auflistung|Die Aktivitäten des Benutzers für Geräte. Schreibgeschützt. Lässt Nullwerte zu.|
|calendar|[Calendar](calendar.md)|Primärer Kalender des Benutzers. Schreibgeschützt.|
|calendarGroups|[CalendarGroup](calendargroup.md) collection|Die Kalendergruppen des Benutzers. Schreibgeschützt. Lässt NULL-Werte zu.|
|calendarView|[Event](event.md) collection|Die Kalenderansicht für den Kalender. Schreibgeschützt. Lässt NULL-Werte zu.|
|calendars|[Kalendersammlung](calendar.md)|Die Kalender des Benutzers. Schreibgeschützt. Lässt NULL-Werte zu.|
|contactFolders|[ContactFolder](contactfolder.md) collection|Die Kontakteordner des Benutzers. Schreibgeschützt. Lässt NULL-Werte zu.|
|contacts|[Contact](contact.md) collection|Die Kontakte des Benutzers. Schreibgeschützt. Lässt NULL-Werte zu.|
|createdObjects|[directoryObject](directoryobject.md)-Sammlung|Verzeichnisobjekte, die vom Benutzer erstellt wurden. Schreibgeschützt. Lässt NULL-Werte zu.|
|directReports|[directoryObject](directoryobject.md) collection|Die Benutzer und Kontakte, die an den Benutzer berichten. (Die Benutzer und Kontakte, deren manager-Eigenschaft auf diesen Benutzer festgelegt ist.) Schreibgeschützt. Lässt NULL-Werte zu. |
|drive|[drive](drive.md)|OneDrive eines Benutzers. Schreibgeschützt.|
|drives|[Laufwerkssammlung](drive.md)| Eine Sammlung von Laufwerken, die für diesen Benutzer zur Verfügung stehen. Schreibgeschützt. |
|events|[Event](event.md) collection|Die Ereignisse des Benutzers. Standardmäßig werden Ereignisse unter dem Standard-Kalender angezeigt. Schreibgeschützt. Lässt NULL-Werte zu.|
|Erweiterungen|[extension](extension.md)-Sammlung|Die Sammlung der für den Benutzer definierten offenen Erweiterungen. Schreibgeschützt. Lässt NULL-Werte zu.|
|inferenceClassification | [inferenceClassification](inferenceclassification.md) | Relevanzklassifizierung von Nachrichten des Benutzers basierend auf expliziten Kennzeichnungen, die die abgeleitete Relevanz oder Wichtigkeit außer Kraft setzen. |
|licenseDetails|[LicenseDetails](licensedetails.md) -Auflistung|Eine Auflistung von Lizenzdetails des Benutzers. Lässt Nullwerte zu.|
|mailFolders|[MailFolder](mailfolder.md)-Sammlung| Die E-Mail-Ordner des Benutzers. Schreibgeschützt. Lässt NULL-Werte zu.|
|manager|[directoryObject](directoryobject.md)|Der Benutzer oder Kontakt, der Vorgesetzter dieses Benutzers ist. Schreibgeschützt. (HTTP-Methoden: GET, PUT, DELETE.)|
|memberOf|[directoryObject](directoryobject.md)-Sammlung|Die Gruppen und Verzeichnisrollen, bei denen der Benutzer Mitglied ist. Schreibgeschützt. Lässt NULL-Werte zu.|
|messages|[Nachrichten](message.md)-Sammlung|Die Nachrichten in einem Postfach oder Ordner. Schreibgeschützt. Lässt NULL-Werte zu.|
|onenote|[OneNote](onenote.md)| Schreibgeschützt.|
|Outlook|[OutlookUser](outlookuser.md)| Schreibgeschützt.|
|ownedDevices|[directoryObject](directoryobject.md)-Sammlung|Geräte, die der Benutzer besitzt. Schreibgeschützt. Lässt NULL-Werte zu.|
|ownedObjects|[directoryObject](directoryobject.md)-Sammlung|Verzeichnisobjekte, die der Benutzer besitzt. Schreibgeschützt. Lässt NULL-Werte zu.|
|Personen|[Person](person.md) -Auflistung| Personen, die für den Benutzer relevant sind. Schreibgeschützt. Lässt Nullwerte zu.
|Foto|[profilePhoto](profilephoto.md)| Das Profilfoto des Benutzers. Schreibgeschützt.|
|Planner|[plannerUser](planneruser.md)| Einstiegspunkt für die Planner-Ressource, die für einen Benutzer vorhanden sein kann. Schreibgeschützt.|
|registeredDevices|[directoryObject](directoryobject.md)-Sammlung|Geräte, die für den Benutzer registriert sind. Schreibgeschützt. Lässt Nullwerte zu.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.directoryObject",
  "openType": true,
  "optionalProperties": [
    "appRoleAssignments",
    "calendar",
    "calendarGroups",
    "calendarView",
    "calendars",
    "contactFolders",
    "contacts",
    "createdObjects",
    "directReports",
    "drive",
    "events",
    "extensions",
    "joinedGroups",
    "mailFolders",
    "manager",
    "memberOf",
    "messages",
    "oauth2PermissionGrants",
    "onenote",
    "ownedDevices",
    "ownedObjects",
    "photo",
    "registeredDevices"
  ],
  "@odata.type": "microsoft.graph.user",
  "@odata.annotations": [
    {
      "capabilities": {
        "changeTracking": true
      }
    },
    {
      "property": "calendar",
      "capabilities": {
        "changeTracking": false,
        "deletable": false,
        "expandable": false,
        "insertable": false,
        "searchable": false,
        "updatable": false
      }
    },
    {
      "property": "calendarGroups",
      "capabilities": {
        "changeTracking": false,
        "expandable": false,
        "searchable": false
      }
    },
    {
      "property": "calendars",
      "capabilities": {
        "changeTracking": false,
        "expandable": false,
        "searchable": false
      }
    },
    {
      "property": "calendarView",
      "capabilities": {
        "changeTracking": true,
        "deletable": false,
        "expandable": true,
        "insertable": false,
        "navigability": "single",
        "searchable": false,
        "updatable": false
      }
    },
    {
      "property": "contactFolders",
      "capabilities": {
        "changeTracking": true,
        "expandable": false,
        "searchable": false
      }
    },
    {
      "property": "contacts",
      "capabilities": {
        "changeTracking": true,
        "expandable": false
      }
    },
    {
      "property": "events",
      "capabilities": {
        "changeTracking": false,
        "expandable": false,
        "searchable": false
      }
    },
    {
      "property": "inferenceClassification",
      "capabilities": {
        "changeTracking": false,
        "deletable": false,
        "expandable": false,
        "insertable": false,
        "searchable": false
      }
    },
    {
      "property": "mailFolders",
      "capabilities": {
        "changeTracking": true,
        "expandable": false,
        "searchable": false
      }
    },
    {
      "property": "messages",
      "capabilities": {
        "changeTracking": false,
        "expandable": false
      }
    },
    {
      "property": "people",
      "capabilities": {
        "changeTracking": false,
        "deletable": false,
        "expandable": false,
        "insertable": false,
        "updatable": false
      }
    },
    {
      "property": "photo",
      "capabilities": {
        "changeTracking": false,
        "deletable": false,
        "expandable": false,
        "insertable": false,
        "searchable": false
      }
    },
    {
      "property": "photos",
      "capabilities": {
        "changeTracking": false,
        "deletable": false,
        "expandable": false,
        "insertable": false,
        "searchable": false,
        "updatable": false
      }
    }
  ]
}-->

```json
{
  "aboutMe": "string",
  "accountEnabled": true,
  "ageGroup": "string",
  "assignedLicenses": [{"@odata.type": "microsoft.graph.assignedLicense"}],
  "assignedPlans": [{"@odata.type": "microsoft.graph.assignedPlan"}],
  "birthday": "String (timestamp)",
  "businessPhones": ["string"],
  "city": "string",
  "companyName": "string",
  "consentProvidedForMinor": "string",
  "country": "string",
  "department": "string",
  "displayName": "string",
  "givenName": "string",
  "hireDate": "String (timestamp)",
  "id": "string (identifier)",
  "imAddresses": ["string"],
  "interests": ["string"],
  "jobTitle": "string",
  "legalAgeGroupClassification": "string",
  "mail": "string",
  "mailboxSettings": {"@odata.type": "microsoft.graph.mailboxSettings"},
  "mailNickname": "string",
  "mobilePhone": "string",
  "mySite": "string",
  "officeLocation": "string",
  "onPremisesDomainName": "string",
  "onPremisesExtensionAttributes": {"@odata.type": "microsoft.graph.onPremisesExtensionAttributes"},
  "onPremisesImmutableId": "string",
  "onPremisesLastSyncDateTime": "String (timestamp)",
  "onPremisesProvisioningErrors": [{"@odata.type": "microsoft.graph.onPremisesProvisioningError"}],
  "onPremisesSamAccountName": "string",
  "onPremisesSecurityIdentifier": "string",
  "onPremisesSyncEnabled": true,
  "onPremisesUserPrincipalName": "string",
  "passwordPolicies": "string",
  "passwordProfile": {"@odata.type": "microsoft.graph.passwordProfile"},
  "pastProjects": ["string"],
  "postalCode": "string",
  "preferredDataLocation": "string",
  "preferredLanguage": "string",
  "preferredName": "string",
  "provisionedPlans": [{"@odata.type": "microsoft.graph.provisionedPlan"}],
  "proxyAddresses": ["string"],
  "responsibilities": ["string"],
  "schools": ["string"],
  "skills": ["string"],
  "state": "string",
  "streetAddress": "string",
  "surname": "string",
  "usageLocation": "string",
  "userPrincipalName": "string",
  "userType": "string",

  "calendar": { "@odata.type": "microsoft.graph.calendar" },
  "calendarGroups": [{ "@odata.type": "microsoft.graph.calendarGroup" }],
  "calendarView": [{ "@odata.type": "microsoft.graph.event" }],
  "calendars": [ {"@odata.type": "microsoft.graph.calendar"} ],
  "contacts": [ { "@odata.type": "microsoft.graph.contact" } ],
  "contactFolders": [ { "@odata.type": "microsoft.graph.contactFolder" } ],
  "createdObjects": [ { "@odata.type": "microsoft.graph.directoryObject" } ],
  "directReports": [ { "@odata.type": "microsoft.graph.directoryObject" } ],
  "drive": { "@odata.type": "microsoft.graph.drive" },
  "drives": [ { "@odata.type": "microsoft.graph.drive" } ],
  "events": [ { "@odata.type": "microsoft.graph.event" } ],
  "inferenceClassification": { "@odata.type": "microsoft.graph.inferenceClassification" },
  "mailFolders": [ { "@odata.type": "microsoft.graph.mailFolder" } ],
  "manager": { "@odata.type": "microsoft.graph.directoryObject" },
  "memberOf": [ { "@odata.type": "microsoft.graph.directoryObject" } ],
  "messages": [ { "@odata.type": "microsoft.graph.message" } ],
  "outlook": { "@odata.type": "microsoft.graph.outlookUser" },
  "ownedDevices": [ { "@odata.type": "microsoft.graph.directoryObject" } ],
  "ownedObjects": [ { "@odata.type": "microsoft.graph.directoryObject" } ],
  "photo": { "@odata.type": "microsoft.graph.profilePhoto" },
  "registeredDevices": [ { "@odata.type": "microsoft.graph.directoryObject" } ]
}

```

## <a name="see-also"></a>Weitere Artikel

- [Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen](/graph/extensibility-overview)
- [Hinzufügen von benutzerdefinierten Daten zu Benutzern mithilfe offener Erweiterungen](/graph/extensibility-open-users)
- [Hinzufügen von benutzerdefinierten Daten zu Gruppen mithilfe von Schemaerweiterungen](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user resource",
  "keywords": "",
  "suppressions" : [
     "Warning: /api-reference/v1.0/resources/user.md/microsoft.graph.user:
      Property 'createdDateTime' found in markdown table but not in resource definition."
  ],
  "section": "documentation",
  "tocPath": ""
}-->
