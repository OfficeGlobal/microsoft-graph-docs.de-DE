---
title: 'conversationThread: reply'
description: 'Beantworten Sie ein Thread in einer gruppenunterhaltung, und fügen Sie eine neue Bereitstellung hinzu. Sie können die übergeordnete Unterhaltung angeben. '
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 54609d291180fba6bc771ac2932ff3ef25d5d82f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513515"
---
# <a name="conversationthread-reply"></a>conversationThread: reply

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Dient zum Antworten auf einen Thread in einer Gruppenunterhaltung und zum Hinzufügen eines neuen Beitrags. Sie können die übergeordnete Unterhaltung in der Anforderung angeben, oder Sie können nur den Thread ohne die übergeordnete Unterhaltung angeben.

## <a name="permissions"></a>Berechtigungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) | Group.ReadWrite.All    |
|Delegiert (persönliches Microsoft-Konto) | Nicht unterstützt    |
|Anwendung | Nicht unterstützt    |

## <a name="http-request"></a>HTTP-Anforderung
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads/{id}/reply
POST /groups/{id}/conversations/{id}/threads/{id}/reply
```
## <a name="request-headers"></a>Anforderungsheader
| Kopfzeile       | Wert |
|:---------------|:--------|
| Authorization  | Bearer {token}. Erforderlich.  |
| Content-Type  | application/json. Erforderlich.   |

## <a name="request-body"></a>Anforderungstext
Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.

| Parameter    | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|Beitrag|[post](../resources/post.md)|Der neue Beitrag, mit dem geantwortet wird.|

## <a name="response"></a>Antwort

Wenn die Methode erfolgreich verläuft, wird der Antwortcode `202 Accepted` zurückgegeben. Im Antworttext wird nichts zurückgegeben.

## <a name="example"></a>Beispiel
Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.
##### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
<!-- {
  "blockType": "request",
  "name": "conversationthread_reply"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/threads/{id}/reply
Content-type: application/json
Content-length: 1131

{
  "post": {
    "body": {
      "contentType": "",
      "content": "content-value"
    }
  }
}
```

##### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort.
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "conversationThread: reply",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/conversationthread-reply.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
