---
title: Chat Thread erstellen
description: Erstellen Sie einen neuen Chat Thread in den angegebenen DDE-Kanal, durch die Stamm-Nachrichten bereitstellen.
ms.openlocfilehash: 9a2a35a086c6689d1b76a56b70cd3637ec23c3a4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058352"
---
# <a name="create-chat-thread"></a>Chat Thread erstellen

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Erstellen Sie einen neuen Chat Thread in den angegebenen [DDE-Kanal](../resources/channel.md) , durch die Stamm-Nachrichten bereitstellen.

## <a name="permissions"></a>Berechtigungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) | Group.ReadWrite.All    |
|Delegiert (persönliches Microsoft-Konto) | Nicht unterstützt    |
|Anwendung | Nicht unterstützt |

> Nur die [Berechtigungen delegiert](/graph/permissions-reference) werden gegenwärtig unterstützt für diesen Vorgang.  Zukünftige Versionen werden Anwendungsberechtigungen unterstützen. 

## <a name="http-request"></a>HTTP-Anforderung
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/channels/{id}/chatThreads
```
## <a name="request-headers"></a>Anforderungsheader
| Name       | Typ | Beschreibung|
|:---------------|:--------|:----------|
| Authorization  | string  | Bearer {token}. Erforderlich. |

## <a name="request-body"></a>Anforderungstext
Geben Sie im Textkörper Anforderung eine JSON-Darstellung der ein [ChatThread](../resources/chatthread.md) -Objekt, das die RootMessage-Eigenschaft enthält.

## <a name="response"></a>Antwort

Wenn der Vorgang erfolgreich war, gibt diese Methode `201 Created` Antwortcode mit einem leeren Antwort Meldungstext.

## <a name="example"></a>Beispiel
##### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
<!-- {
  "blockType": "request",
  "name": "create_chatthread_from_channel"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/channels/{id}/chatThreads
Content-type: application/json

{
  "rootMessage": {
      "body": {
        "contentType": 1,
        "content": "<h1>Hello world</h1>"
      }
  }
}
```

> Derzeit ContentType muss eine ganze Zahl, sondern als eine Zeichenfolge angegeben werden: 0 für "Text" oder "html" 1.  Zukünftige Versionen der API werden dieses Problem zu beheben.

##### <a name="response"></a>Antwort

Nachfolgend sehen Sie ein Beispiel der Antwort.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatThread"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 160

{
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create thread",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->