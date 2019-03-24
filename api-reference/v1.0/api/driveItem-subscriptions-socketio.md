---
author: daspek
ms.author: dspektor
title: WebSocket-Endpunkt abrufen
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 4d4577ea69c65d6ce003af96b0d96b55fe178fb5
ms.sourcegitcommit: 3615f9475d57bfbb3a8c4402af863897f592dfbd
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/23/2019
ms.locfileid: "30791954"
---
# <a name="get-websocket-endpoint"></a>WebSocket-Endpunkt abrufen

Ermöglicht Ihnen das Empfangen von Änderungsbenachrichtigungen in der nahen Echtzeit für ein [Laufwerk][] mithilfe von [Socket.IO][].
Socket.io ist eine beliebte Benachrichtigungs Bibliothek für JavaScript, die webSockets verwendet. Weitere Informationen finden Sie unter [Socket.IO](https://socket.io).

[drive]: ../resources/drive.md
[Socket.IO]: https://socket.io/

## <a name="permissions"></a>Berechtigungen

Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

| Berechtigungstyp                        | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)
|:---------------------------------------|:-------------------------------------------
| Delegiert (Geschäfts-, Schul- oder Unikonto)     | Files. Read, files. ReadWrite, files. ReadWrite. all, Sites. ReadWrite. all
| Delegiert (persönliches Microsoft-Konto) | Files. Read, files. ReadWrite, files. ReadWrite. all
| Anwendung                            | Nicht unterstützt

## <a name="http-request"></a>HTTP-Anforderung

<!-- { "blockType": "ignored" } -->

```http
GET /me/drive/root/subscriptions/socketIo
GET /drives/{driveId}/root/subscriptions/socketIo
GET /groups/{groupId}/drive/root/subscriptions/socketIo
GET /sites/{siteId}/lists/{listId}/drive/root/subscriptions/socketIo
```

## <a name="example"></a>Beispiel

### <a name="request"></a>Anforderung

<!-- { "blockType": "request", "name": "drive_root_subscriptions_socketIo" } -->
```http
GET /me/drive/root/subscriptions/socketIo
```

### <a name="response"></a>Antwort

Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein [Subscription](../resources/subscription.md) -Objekt im Antworttext zurück.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.subscription"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "opaqueId-fj3hd7yf283jfk193726nvc2w3i2diemdu8",
  "notificationUrl": "https://f3hb0mpua.svc.ms/zbaehwg/callback?snthgk=1ff3-2345672zz831837523"
}
```

Die `notificationUrl` zurückgegebene ist eine Socket.IO-Endpunkt-URL.
Um es mit einem socket.io-Client zu verwenden, teilen Sie die `/callback?` Zeichenfolge auf dem Token.
Der Teil der Zeichenfolge ist `/callback?` vor der Socket.IO-Endpunkt-URL und der Teil der Zeichenfolge nach ist eine undurchsichtige Abfragezeichenfolge, die an die Bibliothek gegeben werden muss.

Das folgende Beispiel zeigt, wie Sie `notificationUrl` mit Socket.IO in JavaScript verwenden.

```javascript
// this is the notificationUrl returned from this API
var notificationUrl = "https://f3hb0mpua.svc.ms/zbaehwg/callback?snthgk=1ff3-2345672zz831837523";

// after the split, split[0] will be everything leading up to '/callback?' and split[1] will be everything after.
var split = notificationUrl.split("/callback?");

// 'io' comes from the socket.io client library
var socket = io(split[0], { query: split[1] });

// these examples log to the console.
// your app would provide its own callbacks
socket.on("connect", ()=>console.log("Connected!"));
socket.on("notification", (data)=>console.log("Notification!", data));
```

<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/driveItem-subscriptions-socketio.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
