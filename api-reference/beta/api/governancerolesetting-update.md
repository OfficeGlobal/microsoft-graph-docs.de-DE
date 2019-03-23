---
title: GovernanceRoleSetting aktualisieren
description: Aktualisieren Sie die Eigenschaften von governanceRoleSetting.
localization_priority: Normal
ms.openlocfilehash: f9c851f95df340693626ff82c960243eb2f85b54
ms.sourcegitcommit: 3615f9475d57bfbb3a8c4402af863897f592dfbd
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/23/2019
ms.locfileid: "30789620"
---
# <a name="update-governancerolesetting"></a>GovernanceRoleSetting aktualisieren

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Aktualisieren Sie die Eigenschaften von [governanceRoleSetting](../resources/governancerolesetting.md).

## <a name="permissions"></a>Berechtigungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

>**Hinweis:** Diese API erfordert außerdem, dass die anfordernden Person über `Active` mindestens eine Administratorrollen`owner` Zuweisung `user access administrator`(oder) für die Ressource verfügt.

|Berechtigungstyp      | Berechtigungen              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) | PrivilegedAccess. ReadWrite. AzureResources  |
|Delegiert (persönliches Microsoft-Konto) | Nicht unterstützt    |
|Anwendung | PrivilegedAccess. ReadWrite. AzureResources |

## <a name="http-request"></a>HTTP-Anforderung
<!-- { "blockType": "ignored" } -->
```http
PATCH /privilegedAccess/azureResources/roleSettings/{id}
```
## <a name="request-headers"></a>Anforderungsheader
| Name       | Beschreibung|
|:-----------|:-----------|
| Authorization  | Bearer {code}|
| Content-type  | application/json|


## <a name="request-body"></a>Anforderungstext
Geben Sie im Anforderungstext die Werte für [governanceRuleSettings](../resources/governancerulesetting.md) an, die aktualisiert werden müssen. 

| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|adminEligibleSettings|[governanceRuleSetting](../resources/governancerulesetting.md) -Sammlung|Die Regeleinstellungen, die ausgewertet werden, wenn ein Administrator versucht, eine berechtigte Rollenzuweisung hinzuzufügen.|
|adminMemberSettings|[governanceRuleSetting](../resources/governancerulesetting.md) -Sammlung|Die Regeleinstellungen, die ausgewertet werden, wenn ein Administrator versucht, eine direkte Mitglieds Rollenzuweisung hinzuzufügen.|
|userEligibleSettings|[governanceRuleSetting](../resources/governancerulesetting.md) -Sammlung|Die Regeleinstellungen, die ausgewertet werden, wenn ein Benutzer versucht, eine berechtigte Rollenzuweisung hinzuzufügen. Dies wird für `pimforazurerbac` das Szenario für jetzt nicht unterstützt und ist möglicherweise in den zukünftigen Szenarien verfügbar.|
|userMemberSettings|[governanceRuleSetting](../resources/governancerulesetting.md) -Sammlung|Die Regeleinstellungen, die ausgewertet werden, wenn ein Benutzer versucht, seine Rollenzuweisung zu aktivieren.|

## <a name="response"></a>Antwort
Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 NoContent` zurückgegeben. Im Antworttext wird nichts zurückgegeben. 

### <a name="error-codes"></a>Fehlercodes
Diese API gibt die standardmäßigen HTTP-Fehlercodes zurück. Darüber hinaus werden die folgenden benutzerdefinierten Fehlercodes zurückgegeben.

|Fehlercode     | Fehlermeldung         | Details             |
|:--------------| :---------------------|:--------------------|
| 400 BadRequest| RoleSettingNotFound   | Die [governanceRoleSetting](../resources/governancerolesetting.md) ist nicht im System vorhanden.
| 400 BadRequest| InvalidRoleSetting    | Die im Anforderungstext angegebenen [governanceRuleSettings](../resources/governancerulesetting.md) -Werte sind ungültig.

## <a name="example"></a>Beispiel 
In diesem Beispiel wird die Rollen Einstellung für die benutzerdefinierte Rolle 3 im Abonnement "Flügelspitze Toys-Prod" aktualisiert.
##### <a name="request"></a>Anforderung
<!-- {
  "blockType": "request",
  "name": "update_governancerolesetting"
}-->
```http
PATCH https://graph.microsoft.com/beta/privilegedAccess/pimforazurerbac/roleSettings/5fb5aef8-1081-4b8e-bb16-9d5d0385bab5
Content-type: application/json
Content-length: 350

{
  "adminEligibleSettings":[{"ruleIdentifier":"ExpirationRule","setting":"{\"permanentAssignment\":false,\"maximumGrantPeriodInMinutes\":129600}"}]
}
```
##### <a name="response"></a>Antwort
<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update governanceRoleSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/governancerolesetting-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
