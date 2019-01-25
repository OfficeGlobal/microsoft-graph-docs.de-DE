---
title: Auflisten von groupLifecyclePolicies
description: Ruft eine Liste der groupLifecyclePolicy-Objekte ab, zu der eine Gruppe gehört.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 56ba6f47e1ccd0784f76204d0101171406263397
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514271"
---
# <a name="list-grouplifecyclepolicies"></a>Auflisten von groupLifecyclePolicies

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ruft eine Liste der [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md)-Objekte ab, zu der eine Gruppe gehört.

## <a name="permissions"></a>Berechtigungen

Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) | Directory.Read.All    |
|Delegiert (persönliches Microsoft-Konto) | Nicht unterstützt    |
|Anwendung | Directory.Read.All |

## <a name="http-request"></a>HTTP-Anforderung
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/groupLifecyclePolicies
```
## <a name="optional-query-parameters"></a>Optionale Abfrageparameter
Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.

## <a name="request-headers"></a>Anforderungsheader
| Name | Beschreibung |
|:----------|:----------|
| Authorization | Bearer {token}. Erforderlich. |

## <a name="request-body"></a>Anforderungstext
Geben Sie für diese Methode keinen Anforderungstext an.
## <a name="response"></a>Antwort
Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Sammlung von [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md)-Objekten im Antworttext zurück.
## <a name="example"></a>Beispiel

##### <a name="request"></a>Anforderung

<!-- {
  "blockType": "request",
  "name": "get_grouplifecyclepolicies"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/groupLifecyclePolicies
```
##### <a name="response"></a>Antwort

Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupLifecyclePolicy",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 227

{
  "value": [
    {
      "id": "ffffffff-ffff-ffff-ffff-ffffffffffff",
      "groupLifetimeInDays": 90,
      "managedGroupTypes": "Selected",
      "alternateNotificationEmails": "admin@contoso.com"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List groupLifecyclePolicies",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/group-list-grouplifecyclepolicies.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
