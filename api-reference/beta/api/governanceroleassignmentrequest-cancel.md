---
title: GovernanceRoleAssignmentRequest Abbrechen
description: Abbrechen einer GovernanceRoleAssignmentRequest.
localization_priority: Normal
ms.openlocfilehash: 0437051a3d2550da8a8fe3e9984214ff7c885e3a
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521733"
---
# <a name="cancel-governanceroleassignmentrequest"></a>GovernanceRoleAssignmentRequest Abbrechen

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Abbrechen einer [GovernanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).

## <a name="permissions"></a>Berechtigungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp      | Berechtigungen              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) | PrivilegedAccess.ReadWrite.AzureResources  |
|Delegiert (persönliches Microsoft-Konto) | Nicht unterstützt    |
|Anwendung | PrivilegedAccess.ReadWrite.AzureResources |

## <a name="optional-query-parameters"></a>Optionale Abfrageparameter
Diese Methode bietet **keine** Unterstützung für [OData Abfrageparameter](/graph/query-parameters).

### <a name="http-request"></a>HTTP-Anforderung
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/roleAssignmentRequests/{id}/cancel
```

## <a name="request-headers"></a>Anforderungsheader
| Name       | Beschreibung|
|:---------------|:----------|
| Authorization  | Bearer {code}|
| Content-type  | application/json|

## <a name="request-body"></a>Anforderungstext
Geben Sie für diese Methode keinen Anforderungstext an.

## <a name="response"></a>Antwort
Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 NoContent` zurückgegeben. Im Antworttext wird nichts zurückgegeben. 

## <a name="error-codes"></a>Fehlercodes
Diese API folgt dem Standard-HTTP-Codes. Außerdem werden die benutzerdefinierten Fehlercodes unten angezeigt.
|Fehlercode     | Fehlermeldung              | Details |
|:--------------------| :---------------------|:--------------------|
| 400 BadRequest | RoleAssignmentRequestNotFound | Die GovernanceRoleAssignmentRequest ist im System nicht vorhanden.
| 400 BadRequest | RequestCannotBeCancelled    | Fordert nur in den Status der `Granted`, `PendingApproval`, `PendingApprovalProvisioning` und `PendingAdminDecision` abgebrochen werden kann.

## <a name="example"></a>Beispiel
##### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
<!-- {
  "blockType": "request",
  "name": "cancel_governanceroleassignmentrequest"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests/7c53453e-d5a4-41e0-8eb1-32d5ec8bfdee/cancel
```

##### <a name="response"></a>Antwort
<!-- {
  "blockType": "response",
  "truncated": false,
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
  "description": "Cancel governanceRoleAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/governanceroleassignmentrequest-cancel.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
