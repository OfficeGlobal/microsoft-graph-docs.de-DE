---
title: Benutzer aktualisieren
description: Mit dieser API können Sie die Eigenschaften eines Benutzerobjekts aktualisieren.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f8be2b9fa3c135e710b8a0bcf819187e6cb57959
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512822"
---
# <a name="update-user"></a>Benutzer aktualisieren

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Mit dieser API können Sie die Eigenschaften eines Benutzerobjekts aktualisieren.
## <a name="permissions"></a>Berechtigungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) | User.ReadWrite, User.ReadWrite.All, Directory.ReadWrite.All    |
|Delegiert (persönliches Microsoft-Konto) | User.ReadWrite    |
|Anwendung | User.ReadWrite.All, Directory.ReadWrite.All |

## <a name="http-request"></a>HTTP-Anforderung
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id | userPrincipalName}
```
## <a name="request-headers"></a>Anforderungsheader
| Kopfzeile       | Wert|
|:-----------|:------|
| Authorization  | Bearer {token}. Erforderlich.  |
| Content-Type  | application/json  |

## <a name="request-body"></a>Anforderungstext
Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.

| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|aboutMe|String|Ein Freihandform-Texteingabefeld, in dem der Benutzer sich selbst beschreiben kann.|
|accountEnabled|Boolean| **true**, wenn das Konto aktiviert ist; andernfalls **false**. Diese Eigenschaft ist erforderlich, wenn ein Benutzer erstellt wird. Unterstützt $filter.    |
|assignedLicenses|[assignedLicense](../resources/assignedlicense.md)-Sammlung|Die Lizenzen, die dem Benutzer zugewiesen sind. Lässt keine NULL-Werte zu.            |
|birthday|DateTimeOffset|Der Geburtstag des Benutzers. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`|
|city|String|Die Stadt, in der sich der Benutzer befindet. Unterstützt $filter.|
|Land|String|Land/Region, in dem/der sich der Benutzer befindet; z. B. „USA“ oder „UK“. Unterstützt $filter.|
|department|String|Der Name der Abteilung, in der der Benutzer arbeitet. Unterstützt $filter.|
|displayName|String|cDer Name, der im Adressbuch für den Benutzer angezeigt wird. Dies ist normalerweise eine Kombination aus dem Vornamen, der Initiale des weiteren Vornamens und des Nachnamens. Diese Eigenschaft ist beim Erstellen eines Benutzers erforderlich und kann nicht bei Updates deaktiviert werden. Unterstützt $Filter und $orderby.|
|EmployeeID|String|Die Mitarbeiter-ID von der Organisation, die dem Benutzer zugewiesen. Unterstützt $filter.|
|givenName|String|Der Vorname des Benutzers. Unterstützt $filter.|
|hireDate|DateTimeOffset|Das Einstellungsdatum des Benutzers. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`|
|interests|Zeichenfolgenauflistung|Eine Liste für den Benutzer, um dessen Interessen zu beschreiben.|
|jobTitle|String|Die Position des Benutzers. Unterstützt $filter.|
|mailNickname|Zeichenfolge|Der E-Mail-Alias für den Benutzer. Diese Eigenschaft muss beim Erstellen eines Benutzers angegeben werden. Unterstützt $filter.|
|mobilePhone|String|Die Nummer des primären Mobiltelefons für den Benutzer.|
|mySite|String|Die URL für die persönliche Website des Benutzers.|
|officeLocation|String|Der Bürostandort der Firma des Benutzers|
|onPremisesImmutableId|String|Diese Eigenschaft wird verwendet, um ein lokales Active Directory-Benutzerkonto dem Azure AD-Benutzerobjekt zuzuordnen. Diese Eigenschaft muss angegeben werden, wenn ein neues Benutzerkonto in Graph erstellt wird, wenn Sie eine Verbunddomäne für die **UserPrincipalName**-Eigenschaft (UPN) des Benutzers verwenden. **Wichtig:** Die Zeichen **$** und **_** können nicht verwendet werden, wenn Sie diese Eigenschaft angeben. Unterstützt $filter.                            |
|passwordPolicies|String|Gibt die Kennwortrichtlinien für den Benutzer an. Dieser Wert ist eine Enumeration, deren einziger möglicher Wert „DisableStrongPassword“ lautet. Damit können schwächere Kennwörter als in der Standardrichtlinie angegeben festgelegt werden. Auch „DisablePasswordExpiration“ kann angegeben werden. Beide können zusammen angegeben werden, z. B.: „DisablePasswordExpiration, DisableStrongPassword“.|
|passwordProfile|[PasswordProfile](../resources/passwordprofile.md)|Gibt das Kennwortprofil für den Benutzer an. Das Profil enthält das Kennwort des Benutzers. Diese Eigenschaft ist erforderlich, wenn ein Benutzer erstellt wird. Das Kennwort im Profil muss den Mindestanforderungen entsprechen, wie von der **passwordPolicies**-Eigenschaft angegeben. Standardmäßig ist ein sicheres Kennwort erforderlich.|
|pastProjects|Zeichenfolgenauflistung|Eine Liste zur Aufzählung der erledigten Projekte eines Benutzers.|
|postalCode|String|Die Postleitzahl für die Postanschrift des Benutzers. Die Postleitzahl ist für das Land/die Region des Benutzers spezifisch. In den USA enthält dieses Attribut den ZIP Code.|
|preferredLanguage|String|Die bevorzugte Sprache für den Benutzer. Muss im ISO 639-1-Code angegeben werden. Beispiel: „en-US“.|
|preferredName|String|Der bevorzugte Name für den Benutzer.|
|responsibilities|Zeichenfolgenauflistung|Eine Liste zur Aufzählung der Verantwortlichkeiten eines Benutzers.|
|schools|Zeichenfolgenauflistung|Eine Liste zur Aufzählung der vom Benutzer besuchten Schulen.|
|skills|Zeichenfolgenauflistung|Eine Liste zur Aufzählung der Qualifikationen eines Benutzers.|
|state|String|Bundesland oder Kanton in der Adresse des Benutzers. Unterstützt $filter.|
|streetAddress|String|Die Straße der Firma des Benutzers.|
|surname|String|Der Nachname des Benutzers. Unterstützt $filter.|
|usageLocation|String|Ein aus zwei Buchstaben bestehender Ländercode (ISO-Standard 3166). Erforderlich für Benutzer, denen Lizenzen zugewiesen werden, aufgrund der gesetzlichen Vorschrift, dass die Verfügbarkeit von Diensten in einzelnen Ländern geprüft werden muss.  Beispiele sind: „US“, „JP“ und „GB“. Lässt keine NULL-Werte zu. Unterstützt $filter.|
|userPrincipalName|String|Der User Principal Name (UPN) des Benutzers. Der UPN ist ein Anmeldename des Benutzers im Internetformat, der auf dem Internetstandard RFC 822 basiert. Gemäß der Konvention sollte er dem E-Mail-Namen des Benutzers zugeordnet sein. Das allgemeine Format lautet „alias@domäne“, wobei „domäne“ in der Sammlung der verifizierten Domänen des Mandanten vorhanden sein muss. Diese Eigenschaft ist erforderlich, wenn ein Benutzer erstellt wird. Auf die verifizierten Domänen für den Mandanten kann über die **verifiedDomains** -Eigenschaft von [organization](../resources/organization.md) zugegriffen werden. Unterstützt $Filter und $orderby.
|userType|Zeichenfolge|Ein Zeichenfolgenwert kann zum Klassifizieren der Benutzertypen in Ihrem Verzeichnis verwendet werden, z. B. „Member“ und „Guest“. Unterstützt $filter.          |

Da die Ressource **Benutzer** [Extensions](/graph/extensibility-overview)unterstützt, können Sie die `PATCH` Vorgang hinzufügen, aktualisieren oder Löschen von Ihren eigenen app-spezifischen Daten in benutzerdefinierten Eigenschaften einer Erweiterung in einer vorhandenen Instanz der **Benutzer** .

## <a name="response"></a>Antwort

Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.
## <a name="example"></a>Beispiel
##### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
<!-- {
  "blockType": "request",
  "name": "update_user"
}-->
```http
PATCH https://graph.microsoft.com/beta/me
Content-type: application/json
Content-length: 491

{
  "accountEnabled": true,
  "assignedLicenses": [
    {
      "disabledPlans": [ "bea13e0c-3828-4daa-a392-28af7ff61a0f" ],
      "skuId": "skuId-value"
    }
  ],
  "assignedPlans": [
    {
      "assignedDateTime": "2016-10-19T10:37:00Z",
      "capabilityStatus": "capabilityStatus-value",
      "service": "service-value",
      "servicePlanId": "bea13e0c-3828-4daa-a392-28af7ff61a0f"
    }
  ],
  "businessPhones": [
    "businessPhones-value"
  ],
  "city": "city-value"
}
```
##### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a>Siehe auch

- [Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen](/graph/extensibility-overview)
- [Hinzufügen von benutzerdefinierten Daten zu Benutzern mithilfe offener Erweiterungen (Preview)](/graph/extensibility-open-users)
- [Hinzufügen von benutzerdefinierten Daten zu Gruppen mithilfe von Schemaerweiterungen (Preview)](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update user",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
