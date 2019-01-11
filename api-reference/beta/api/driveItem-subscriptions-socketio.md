---
title: Abrufen von Websocket-Endpunkt
description: Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.
localization_priority: Normal
ms.openlocfilehash: a981a4d02d2e40fec0cb2bca397c7b7794d36867
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27859794"
---
# <a name="get-websocket-endpoint"></a>Abrufen von Websocket-Endpunkt

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.
Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Ermöglicht Ihnen, zum Empfangen von Benachrichtigungen für ein [Laufwerk][] mit [socket.io][]nahezu in Echtzeit ändern.
Socket.IO ist eine häufig verwendete Benachrichtigungen-Bibliothek für JavaScript, das WebSockets nutzt. Weitere Informationen finden Sie unter [socket.io](https://socket.io).

[drive]: ../resources/drive.md
[Socket.IO]: https://socket.io/

## <a name="permissions"></a>Berechtigungen

Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

| Berechtigungstyp                        | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)
|:---------------------------------------|:-------------------------------------------
| Delegiert (Geschäfts-, Schul- oder Unikonto)     | Files.Read, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All
| Delegiert (persönliches Microsoft-Konto) | Files.Read, Files.ReadWrite, Files.ReadWrite.All
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

Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und ein [Abonnement](../resources/subscription.md) -Objekt aus der Antwort.

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

Die `notificationUrl` socket.io-Endpunkt-URL zurückgegeben wird.
Die Zeichenfolge für die Verwendung mit einem Client socket.io auf Aufteilen der `/callback?` token.
Der Teil der Zeichenfolge vor dem `/callback?` ist die socket.io Endpunkt-URL und der Teil der Zeichenfolge nach ist eine undurchsichtige Abfragezeichenfolge, die in die Bibliothek zugewiesen werden soll.

Das folgende Beispiel zeigt, wie Sie mit der `notificationUrl` mit socket.io in JavaScript.

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

<!-- {
  "type": "#page.annotation"
}-->
