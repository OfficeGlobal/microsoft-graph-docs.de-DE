---
title: GovernanceRoleAssignmentRequests aktualisieren
description: So aktualisieren Sie ihre Entscheidungen Administratoren können (`AdminApproved` oder `AdminDenied`) auf GovernanceRoleAssignmentRequests, die in den Status der sind `PendingAdminDecision`.
localization_priority: Normal
ms.openlocfilehash: 870cd685aade9bb722660b550ae210c6e10d1fe8
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514614"
---
# <a name="update-governanceroleassignmentrequests"></a>GovernanceRoleAssignmentRequests aktualisieren

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

So aktualisieren Sie ihre Entscheidungen Administratoren können (`AdminApproved` oder `AdminDenied`) auf [GovernanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) , die in den Status der sind `PendingAdminDecision`.

## <a name="permissions"></a>Berechtigungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

>**Hinweis:** Diese API erfordert auch, dass die anfordernde Person mindestens eine `Active` Administrator rollenzuweisung (`owner` oder `user access administrator`) für die Ressource, die die [GovernanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) gehört. 

|Berechtigungstyp      | Berechtigungen              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) | PrivilegedAccess.ReadWrite.AzureResources  |
|Delegiert (persönliches Microsoft-Konto) | Nicht unterstützt    |
|Anwendung | PrivilegedAccess.ReadWrite.AzureResources |

## <a name="http-request"></a>HTTP-Anforderung
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/roleAssignmentRequests/{id}/updateRequest   
```

## <a name="request-headers"></a>Anforderungsheader
| Name           | Beschreibung|
|:---------------|:----------|
| Authorization  | Bearer {code}|
| Content-type  | application/json|

## <a name="request-body"></a>Anforderungstext

|Parameter      |Typ                   |Erforderlich |Beschreibung|
|:-------------|:----------------------|:--------|:----------|
|Grund        |String                 |✓        |Der Grund für seine Entscheidung vom Administrator bereitgestellten.|
|Entscheidung        |String                 |✓        |Die Entscheidung Administrator der Rolle Zuordnung Anforderung. Der Wert aktualisiert werden sollen, als `AdminApproved` oder `AdminDenied`.|
|Zeitplan      |[governanceSchedule](../resources/governanceschedule.md)|        | Den Zeitplan der Rolle Zuordnung Anforderung. Status der `AdminApproved`, es ist erforderlich.|
|assignmentState      |String|         | Der Status der Aufgabe und die Werte sind möglich `Eligible` oder `Active`. Für die Entscheidung der `AdminApproved`, es ist erforderlich. |
### <a name="response"></a>Antwort
Diese Methode kann nur angewendet werden, auf Anfragen, die in den Status der sind `PendingAdminDecision`.

Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.

## <a name="example"></a>Beispiel
##### <a name="request"></a>Anforderung
<!-- {
  "blockType": "request",
  "name": "updaterequest_governanceroleassignmentrequest"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests/7c53453e-d5a4-41e0-8eb1-32d5ec8bfdee/updateRequest
```
##### <a name="request-body"></a>Anforderungstext
```json
{
  "reason":"approve the request to extend role assignment",
  "schedule":{
    "type":"Once",
    "startDateTime":"2018-02-20T07:31:13.451Z",
    "stopDateTime":"2018-05-21T07:31:13.451Z",
    },
  "decision":"AdminApproved",
  "assignmentState": "Eligible"
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
  "description": "UpdateRequest governanceRoleAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/governanceroleassignmentrequest-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
