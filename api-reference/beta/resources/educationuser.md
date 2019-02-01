---
title: educationUser-Ressourcentyp
description: Ein Benutzer im System. Dies ist eine bildungsspezifische Variante des Benutzers mit derselben `id`, den Microsoft Graph vom nicht bildungsspezifischen `/users`-Endpunkt zurückgibt.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: d0467ed9ac03a1607d575b6eac5f6b3330b68c3c
ms.sourcegitcommit: d6209114cbbe8072e3ecf7eba23819ae5ace7db5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/01/2019
ms.locfileid: "29690931"
---
# <a name="educationuser-resource-type"></a>educationUser-Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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
|assignedPlans|[assignedPlan](assignedplan.md) collection|Die Pläne, die dem Benutzer zugewiesen sind. Schreibgeschützt. Lässt keine NULL-Werte zu. |
|businessPhones|String-Sammlung|Die Telefonnummern für den Benutzer. **Hinweis:** Obwohl dies eine String-Sammlung ist, kann nur eine Nummer für diese Eigenschaft festgelegt werden.|
|createdBy|[identitySet](identityset.md)| Entität, die den Benutzer erstellt hat. |
|department|String|Der Name der Abteilung, in der der Benutzer arbeitet. Unterstützt $filter.|
|displayName|String|Der Name des Benutzers, der im Adressbuch angezeigt wird. Dies ist normalerweise eine Kombination aus dem Vornamen, der Initiale des weiteren Vornamens und des Nachnamens. Diese Eigenschaft ist beim Erstellen eines Benutzers erforderlich und kann nicht bei Updates deaktiviert werden. Unterstützt $filter und $orderby.|
|externalSource|`educationExternalSource`| Quelle, aus der dieser Benutzer erstellt wurde. Mögliche Werte sind: `sis`, `manual` und `unkownFutureValue`.|
|givenName|String|Der Vorname des Benutzers. Unterstützt $filter.|
|id|string|Der eindeutige Bezeichner des Benutzers. Geerbt von [directoryObject](directoryobject.md). Key. Lässt keine Nullwerte zu. Schreibgeschützt.|
|mail|String|Die SMTP-Adresse des Benutzers, z. B. „jeff@contoso.onmicrosoft.com“. Schreibgeschützt. Unterstützt $filter.|
|mailingAddress|[physicalAddress](physicaladdress.md)| E-Mail-Adresse des Benutzers|
|mailNickname|String|Der E-Mail-Alias für den Benutzer. Diese Eigenschaft muss beim Erstellen eines Benutzers angegeben werden. Unterstützt $filter.|
|middleName| String | Der zweite Vorname des Benutzers|
|mobilePhone|String|Die Nummer des primären Mobiltelefons für den Benutzer.|
|passwordPolicies|String|Gibt die Kennwortrichtlinien für den Benutzer an. Dieser Wert ist eine Enumeration, deren einziger möglicher Wert „DisableStrongPassword“ lautet. Damit können schwächere Kennwörter als in der Standardrichtlinie angegeben festgelegt werden. Auch „DisablePasswordExpiration“ kann angegeben werden. Die beiden können zusammen angegeben werden. Beispiel: "DisablePasswordExpiration, DisableStrongPassword".|
|passwordProfile|[passwordProfile](passwordprofile.md)|Gibt das Kennwortprofil für den Benutzer an. Das Profil enthält das Kennwort des Benutzers. Diese Eigenschaft ist erforderlich, wenn ein Benutzer erstellt wird. Das Kennwort im Profil muss den Mindestanforderungen entsprechen, wie von der **passwordPolicies**-Eigenschaft angegeben. Standardmäßig ist ein sicheres Kennwort erforderlich.|
|preferredLanguage|Zeichenfolge|Die bevorzugte Sprache für den Benutzer. Muss im ISO 639-1-Code angegeben werden. Beispiel: „en-US“.|
|primaryRole|string| Standardrolle für einen Benutzer. Die Rolle des Benutzers kann in einer einzelnen Klasse unterschiedlich sein. Mögliche Werte sind: `student`, `teacher` und `enum_sentinel`. Unterstützt $filter.|
|provisionedPlans|[ProvisionedPlan](provisionedplan.md)-Sammlung|Die Pläne, die für den Benutzer bereitgestellt wurden. Schreibgeschützt. Lässt keine NULL-Werte zu. |
|residenceAddress|[physicalAddress](physicaladdress.md)| Die Wohnadresse des Benutzers|
|relatedContacts|[RelatedContact](relatedcontact.md) -Auflistung|Gruppe von Kontakten, die im Zusammenhang mit der Benutzer.  Diese optionale Eigenschaft muss in einer $select-Klausel angegeben werden und kann nur für einen einzelnen Benutzer abgerufen werden.|
|student|[educationStudent](educationstudent.md)| Ist die primäre Rolle Kursteilnehmer, enthält dieser Block spezifische Daten für Kursteilnehmer.|
|surname|String|Der Nachname des Benutzers. Unterstützt $filter.|
|teacher|[educationTeacher](educationteacher.md)| Ist die primäre Rolle Lehrer, enthält dieser Block lehrerspezifische Daten.|
|usageLocation|String|Ein aus zwei Buchstaben bestehender Ländercode (ISO-Standard 3166). Erforderlich für Benutzer, denen Lizenzen zugewiesen werden, aufgrund der gesetzlichen Vorschrift, dass die Verfügbarkeit von Diensten in einzelnen Ländern oder Regionen geprüft werden muss. Beispiele: "DE", "GB" und "US". Lässt keine Nullwerte zu. Unterstützt $filter.|
|userPrincipalName|Zeichenfolge|Der User Principal Name (UPN) des Benutzers. Der UPN ist ein Anmeldename des Benutzers im Internetformat, der auf dem Internetstandard RFC 822 basiert. Gemäß der Konvention sollte er dem E-Mail-Namen des Benutzers zugeordnet sein. Das allgemeine Format lautet „alias@domäne“, wobei „domäne“ in der Sammlung der verifizierten Domänen des Mandanten vorhanden sein muss. Diese Eigenschaft ist erforderlich, wenn ein Benutzer erstellt wird. Auf die verifizierten Domänen für den Mandanten kann über die **verifiedDomains** -Eigenschaft von [organization](organization.md) zugegriffen werden. Unterstützt $Filter und $orderby.
|userType|String|Ein Zeichenfolgenwert kann zum Klassifizieren der Benutzertypen in Ihrem Verzeichnis verwendet werden, z. B. „Member“ und „Guest“. Unterstützt $filter.          |

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|classes|[educationClass](educationclass.md)-Sammlung| Klassen, zu denen der Benutzer gehört. Nullwerte zulassend.|
|schools|[educationSchool](educationschool.md)-Sammlung| Schulen, zu denen der Benutzer gehört. Lässt Nullwerte zu.|
|assignments| [educationAssignment](educationassignment.md)| Liste von Zuweisungen für den Benutzer. Lässt Nullwerte zu.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationUser"
}-->

```json
{
  "id": "string",
  "displayName": "string",
  "givenName": "string",
  "middleName": "string",
  "surname": "string",
  "mail": "string",
  "mobilePhone": "string",
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "externalSource": "string",
  "mailingAddress": {"@odata.type": "microsoft.graph.physicalAddress"},
  "primaryRole": "string",
  "residenceAddress": {"@odata.type": "microsoft.graph.physicalAddress"},
  "student": {"@odata.type": "microsoft.graph.educationStudent"},
  "teacher": {"@odata.type": "microsoft.graph.educationTeacher"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationuser.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
