---
title: GovernanceRoleSetting aktualisieren
description: Aktualisieren Sie die Eigenschaften des GovernanceRoleSetting.
ms.openlocfilehash: ca5752d51e5d59578594a12c80ae1cac316b48bc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058385"
---
# <a name="update-governancerolesetting"></a>GovernanceRoleSetting aktualisieren

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Aktualisieren Sie die Eigenschaften des [GovernanceRoleSetting](../resources/governancerolesetting.md).

## <a name="permissions"></a>Berechtigungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp      | Berechtigungen              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) | PrivilegedAccess.ReadWrite.AzureResources  |
|Delegiert (persönliches Microsoft-Konto) | Nicht unterstützt    |
|Anwendung | PrivilegedAccess.ReadWrite.AzureResources |

Diese API erfordert neben der Berechtigungsbereich den Requestor in mindestens einem `Active` Administrator rollenzuweisung (`owner` oder `user access administrator`) für die Ressource.
## <a name="http-request"></a>HTTP-Anforderung
<!-- { "blockType": "ignored" } -->
```http
PATCH /privilegedAccess/azureResources/roleSettings/{id}
```
## <a name="optional-request-headers"></a>Optionale Anforderungsheader
| Name       | Beschreibung|
|:-----------|:-----------|
| Authorization  | Bearer {code}|
| Content-type  | application/json|


## <a name="request-body"></a>Anforderungstext
Geben Sie im Textkörper Anforderung die Werte für [GovernanceRuleSettings](../resources/governancerulesetting.md) , die aktualisiert werden muss. 

| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|adminEligibleSettings|[governanceRuleSetting](../resources/governancerulesetting.md)|Die Einstellungen, die ausgewertet werden, wenn ein Administrator versucht, eine Aufgabe zu auswählbaren Rolle hinzufügen.|
|adminMemberSettings|[governanceRuleSetting](../resources/governancerulesetting.md)|Die Einstellungen, die ausgewertet werden, wenn ein Administrator versucht, eine direkte rollenzuweisung hinzufügen.|
|userEligibleSettings|[governanceRuleSetting](../resources/governancerulesetting.md)|Die Einstellungen, die ausgewertet werden, wenn ein Benutzer versucht, eine Aufgabe zu auswählbaren Rolle hinzufügen. Dies wird nicht unterstützt für `pimforazurerbac` Szenario vorläufig und kann in zukünftigen Szenarien zur Verfügung gestellt.|
|userMemberSettings|[governanceRuleSetting](../resources/governancerulesetting.md)|Die Einstellungen, die ausgewertet werden, wenn ein Benutzer versucht, seine rollenzuweisung aktivieren.|

## <a name="response"></a>Antwort
Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 NoContent` zurückgegeben. Im Antworttext wird nichts zurückgegeben. 

## <a name="error-codes"></a>Fehlercodes
Diese API folgt dem Standard-HTTP-Codes. Außerdem werden die benutzerdefinierten Fehlercodes unten angezeigt.
|Fehlercode     | Fehlermeldung         | Details             |
|:--------------| :---------------------|:--------------------|
| 400 BadRequest| RoleSettingNotFound   | Die [GovernanceRoleSetting](../resources/governancerolesetting.md) ist im System nicht vorhanden.
| 400 BadRequest| InvalidRoleSetting    | Die [GovernanceRuleSettings](../resources/governancerulesetting.md) Werte im Textkörper Anforderung ist ungültig.

## <a name="example"></a>Beispiel 
Dieses Beispiel aktualisiert die Rolle Einstellung für benutzerdefinierte Rolle 3 im Abonnement Wingtip Toys - "Bemerkungen".
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
<!-- {
  "type": "#page.annotation",
  "description": "Update governanceRoleSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->