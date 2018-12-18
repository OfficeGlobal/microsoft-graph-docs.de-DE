---
title: educationUser-Ressourcentyp
description: Ein Benutzer im System. Dies ist eine bildungsspezifische Variante des Benutzers mit derselben `id`, den Microsoft Graph vom nicht bildungsspezifischen `/users`-Endpunkt zurückgibt.
author: mmast-msft
ms.openlocfilehash: 2c89b2a099ea8a21e9b2a5b8cbd4c394ddb7b0b3
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27342581"
---
# <a name="educationuser-resource-type"></a>educationUser-Ressourcentyp

Ein Benutzer im System. Dies ist eine bildungsspezifische Variante des Benutzers mit derselben `id`, den Microsoft Graph vom nicht bildungsspezifischen `/users`-Endpunkt zurückgibt.
Dieses Objekt enthält eine gezielte Teilmenge von Eigenschaften des [user](user.md)-Kernobjekts, erweitert um eine Reihe bildungsspezifischer Eigenschaften wie `primaryRole`, Kursteilnehmer- und Lehrerdaten.


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[educationUser abrufen](../api/educationuser-get.md) | [educationUser](educationuser.md) |Lesen von Eigenschaften und Beziehungen eines **educationUser**-Objekts.|
|[Klassen auflisten](../api/educationuser-list-classes.md) |[educationClass](educationclass.md)-Sammlung| Abrufen der **educationClass**-Objektsammlung, in der der Benutzer Mitglied ist.|
|[Schulen auflisten](../api/educationuser-list-schools.md) |[educationSchool](educationschool.md)-Sammlung| Abrufen der **educationSchool**-Objektsammlung, in der der Benutzer Mitglied ist.|
|[Benutzer abrufen](../api/educationuser-get-user.md) |[user](user.md)| Abrufen des einfachen Verzeichnis-**Benutzers**, der diesem **educationUser** entspricht.|
|[Aktualisieren](../api/educationuser-update.md) | [educationUser](educationuser.md)   |Aktualisieren eines **educationUser**-Objekts. |
|[Löschen](../api/educationuser-delete.md) | Keine |Löschen eines **educationUser**-Objekts. |

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|accountEnabled|Boolean| **True**, wenn das Konto aktiviert ist; andernfalls **false**. Diese Eigenschaft ist erforderlich, wenn ein Benutzer erstellt wird. Unterstützt $filter.    |
|assignedLicenses|[assignedLicense](assignedlicense.md) collection|Die Lizenzen, die dem Benutzer zugewiesen sind. Lässt keine NULL-Werte zu.            |
|assignedPlans|[assignedPlan](assignedplan.md)-Sammlung|Die Pläne, die dem Benutzer zugewiesen sind. Schreibgeschützt. Lässt keine NULL-Werte zu. |
|businessPhones|String-Sammlung|Die Telefonnummern für den Benutzer. **Hinweis:** Obwohl dies eine String-Sammlung ist, kann nur eine Nummer für diese Eigenschaft festgelegt werden.|
|createdBy|[identitySet](identityset.md)| Entität, die den Benutzer erstellt hat. |
|department|String|Der Name der Abteilung, in der der Benutzer arbeitet. Unterstützt $filter.|
|displayName|Zeichenfolge|Der Name des Benutzers, der im Adressbuch angezeigt wird. Dies ist normalerweise eine Kombination aus dem Vornamen, der Initiale des weiteren Vornamens und des Nachnamens. Diese Eigenschaft ist beim Erstellen eines Benutzers erforderlich und kann nicht bei Updates deaktiviert werden. Unterstützt $filter und $orderby.|
|externalSource|`educationExternalSource`| Quelle, aus der dieser Benutzer erstellt wurde. Die möglichen Werte sind: `sis`, `manual`, `unkownFutureValue`.|
|givenName|String|Der Vorname des Benutzers. Unterstützt $filter.|
|id|String|Der eindeutige Bezeichner des Benutzers. Geerbt von [directoryObject](directoryobject.md). Key. Lässt keine Nullwerte zu. Schreibgeschützt.|
|mail|String|Die SMTP-Adresse des Benutzers, z. B. „jeff@contoso.onmicrosoft.com“. Schreibgeschützt. Unterstützt $filter.|
|mailingAddress|[physicalAddress](physicaladdress.md)| E-Mail-Adresse des Benutzers|
|mailNickname|String|Der E-Mail-Alias für den Benutzer. Diese Eigenschaft muss beim Erstellen eines Benutzers angegeben werden. Unterstützt $filter.|
|middleName| String | Der zweite Vorname des Benutzers|
|mobilePhone|String|Die Nummer des primären Mobiltelefons für den Benutzer.|
|passwordPolicies|Zeichenfolge|Gibt die Kennwortrichtlinien für den Benutzer an. Dieser Wert ist eine Enumeration, deren einziger möglicher Wert „DisableStrongPassword“ lautet. Damit können schwächere Kennwörter als in der Standardrichtlinie angegeben festgelegt werden. Auch „DisablePasswordExpiration“ kann angegeben werden. Die beiden können zusammen angegeben werden. Beispiel: "DisablePasswordExpiration, DisableStrongPassword".|
|passwordProfile|[PasswordProfile](passwordprofile.md)|Gibt das Kennwortprofil für den Benutzer an. Das Profil enthält das Kennwort des Benutzers. Diese Eigenschaft ist erforderlich, wenn ein Benutzer erstellt wird. Das Kennwort im Profil muss den Mindestanforderungen entsprechen, wie von der **passwordPolicies**-Eigenschaft angegeben. Standardmäßig ist ein sicheres Kennwort erforderlich.|
|preferredLanguage|Zeichenfolge|Die bevorzugte Sprache für den Benutzer. Muss im ISO 639-1-Code angegeben werden. Beispiel: „en-US“.|
|primaryRole|educationUserRole| Standardrolle für einen Benutzer. Die Rolle des Benutzers kann in einer einzelnen Klasse unterschiedlich sein. Die möglichen Werte sind: `student`, `teacher`, `unknownFutureValue`. Unterstützt $filter.|
|provisionedPlans|[ProvisionedPlan](provisionedplan.md) collection|Die Pläne, die für den Benutzer bereitgestellt wurden. Schreibgeschützt. Lässt keine NULL-Werte zu. |
|residenceAddress|[physicalAddress](physicaladdress.md)| Die Wohnadresse des Benutzers|
|student|[educationStudent](educationstudent.md)| Ist die primäre Rolle Kursteilnehmer, enthält dieser Block spezifische Daten für Kursteilnehmer.|
|surname|String|Der Nachname des Benutzers. Unterstützt $filter.|
|teacher|[educationTeacher](educationteacher.md)| Ist die primäre Rolle Lehrer, enthält dieser Block lehrerspezifische Daten.|
|usageLocation|String|Ein aus zwei Buchstaben bestehender Ländercode (ISO-Standard 3166). Erforderlich für Benutzer, denen Lizenzen zugewiesen werden, aufgrund der gesetzlichen Vorschrift, dass die Verfügbarkeit von Diensten in einzelnen Ländern oder Regionen geprüft werden muss. Beispiele: "DE", "GB" und "US". Lässt keine Nullwerte zu. Unterstützt $filter.|
|userPrincipalName|String|Der User Principal Name (UPN) des Benutzers. Der UPN ist ein Anmeldename des Benutzers im Internetformat, der auf dem Internetstandard RFC 822 basiert. Gemäß der Konvention sollte er dem E-Mail-Namen des Benutzers zugeordnet sein. Das allgemeine Format lautet „alias@domäne“, wobei „domäne“ in der Sammlung der verifizierten Domänen des Mandanten vorhanden sein muss. Diese Eigenschaft ist erforderlich, wenn ein Benutzer erstellt wird. Auf die verifizierten Domänen für den Mandanten kann über die **verifiedDomains** -Eigenschaft von [organization](organization.md) zugegriffen werden. Unterstützt $Filter und $orderby.
|userType|String|Ein Zeichenfolgenwert kann zum Klassifizieren der Benutzertypen in Ihrem Verzeichnis verwendet werden, z. B. „Member“ und „Guest“. Unterstützt $filter.          |

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|classes|[educationClass](educationclass.md)-Sammlung| Klassen, zu denen der Benutzer gehört. Lässt Nullwerte zu.|
|schools|[educationSchool](educationschool.md)-Sammlung| Schulen, zu denen der Benutzer gehört. Lässt Nullwerte zu.|
|assignments| [educationAssignment](/graph/api/resources/educationassignment?view=graph-rest-beta)| Liste der Zuordnungen für den Benutzer. Lässt Nullwerte zu.|
|user|[Benutzer](user.md)| Der Directory-Benutzer, die diesen Benutzer entspricht.|

>**Hinweis:** Bei der **educationassignment**-Ressource handelt es sich um eine /beta-Version. Wenn Sie diese Ressource verwenden, überprüfen Sie unbedingt in regelmäßigen Abständen das [Änderungsprotokoll](/graph/changelog). Wenn Microsoft Graph-API-Ressourcen im /v1.0-Endpunkt veröffentlicht werden, wird die Version im Änderungsprotokoll aufgeführt. Wenn Ihre App die **educationassignment**-Ressource nutzt, müssen Sie die Basisanforderungs-URLs wie im folgenden Codeblock deklarieren:  
```JavaScript
var v1BaseUrl = “https://graph.microsoft.com/v1.0/education”;
var betaBaseUrl = “https://graph.microsoft.com/beta/education”;  // for administrativeUnit and educationOrganization
```


## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.educationUser"
}-->

```json
{
  "id": "string",
  "accountEnabled": true,
  "assignedLicenses": [{"@odata.type": "microsoft.graph.assignedLicense"}],
  "assignedPlans": [{"@odata.type": "microsoft.graph.assignedPlan"}],
  "businessPhones": ["555-555-6568"],
  "department": "string",
  "displayName": "string",
  "givenName": "string",
  "middleName": "string",
  "surname": "string",
  "mail": "string",
  "mailNickname": "string",
  "mobilePhone": "string",
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "externalSource": "string",
  "mailingAddress": {"@odata.type": "microsoft.graph.physicalAddress"},
  "passwordPolicies": "string",
  "passwordProfile": {"@odata.type": "microsoft.graph.passwordProfile"},
  "preferredLanguage": "string",
  "primaryRole": "string",
  "provisionedPlans": [{"@odata.type": "microsoft.graph.provisionedPlan"}],
  "residenceAddress": {"@odata.type": "microsoft.graph.physicalAddress"},
  "student": {"@odata.type": "microsoft.graph.educationStudent"},
  "teacher": {"@odata.type": "microsoft.graph.educationTeacher"},
  "usageLocation": "string",
  "userPrincipalName": "string",
  "userType": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationUser resource",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Error: microsoft.graph.educationUser/assignments:
      Referenced type microsoft.graph.educationAssignment is not defined in the doc set! Potential suggestion: UNKNOWN"
  ],
  "tocPath": ""
}-->
