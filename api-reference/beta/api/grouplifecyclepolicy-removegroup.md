---
title: 'groupLifecyclePolicy: removeGroup'
description: Entfernt eine Gruppe aus einer Lebenszyklusrichtlinie.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: b3fd7f46c9c35777468a8436433d034ff000ea5b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524884"
---
# <a name="grouplifecyclepolicy-removegroup"></a>groupLifecyclePolicy: removeGroup

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Entfernt eine Gruppe aus einer Lebenszyklusrichtlinie.

## <a name="permissions"></a>Berechtigungen

Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).


|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) | Directory.ReadWrite.All    |
|Delegiert (persönliches Microsoft-Konto) | Nicht unterstützt |
|Anwendung |  Directory.ReadWrite.All |

## <a name="http-request"></a>HTTP-Anforderung
<!-- { "blockType": "ignored" } -->
```http
POST /groupLifecyclePolicies/{id}/removeGroup
```

## <a name="request-headers"></a>Anforderungsheader

| Name | Beschreibung |
|:---------------|:----------|
| Authorization | Bearer {token}. Erforderlich. |
| Content-Type  | application/json |

## <a name="request-body"></a>Anforderungstext
Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.

| Parameter | Typ | Beschreibung |
|:---------------|:--------|:----------|
|groupId|Guid| Die ID der Gruppe, die aus der Richtlinie entfernt werden soll.|

## <a name="response"></a>Antwort

Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben. Wenn die Gruppe aus der Richtlinie entfernt wird, wird der Wert **true** im Antworttext zurückgegeben. Andernfalls wird der Wert **false** im Antworttext zurückgegeben.

## <a name="example"></a>Beispiel

##### <a name="request"></a>Anforderung

<!-- {
  "blockType": "ignored",
  "name": "grouplifecyclepolicy_removegroup"
} -->
```http
POST https://graph.microsoft.com/beta/groupLifecyclePolicies/{id}/removeGroup
Content-type: application/json
Content-length: 57

{
  "groupId": "ffffffff-ffff-ffff-ffff-ffffffffffff"
}
```

##### <a name="response"></a>Antwort
<!-- { "blockType": "ignored" } -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 21

{
  "value": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "groupLifecyclePolicy: removegroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/grouplifecyclepolicy-removegroup.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
