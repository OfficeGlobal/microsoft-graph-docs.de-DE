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
# <a name="get-websocket-endpoint"></a><span data-ttu-id="41656-102">WebSocket-Endpunkt abrufen</span><span class="sxs-lookup"><span data-stu-id="41656-102">Get websocket endpoint</span></span>

<span data-ttu-id="41656-103">Ermöglicht Ihnen das Empfangen von Änderungsbenachrichtigungen in der nahen Echtzeit für ein [Laufwerk][] mithilfe von [Socket.IO][].</span><span class="sxs-lookup"><span data-stu-id="41656-103">Allows you to receive near-real-time change notifications for a [drive][] using [socket.io][].</span></span>
<span data-ttu-id="41656-104">Socket.io ist eine beliebte Benachrichtigungs Bibliothek für JavaScript, die webSockets verwendet.</span><span class="sxs-lookup"><span data-stu-id="41656-104">Socket.io is a popular notifications library for JavaScript that utilizes WebSockets.</span></span> <span data-ttu-id="41656-105">Weitere Informationen finden Sie unter [Socket.IO](https://socket.io).</span><span class="sxs-lookup"><span data-stu-id="41656-105">To learn more, see [socket.io](https://socket.io).</span></span>

[drive]: ../resources/drive.md
[Socket.IO]: https://socket.io/
[socket.io]: https://socket.io/

## <a name="permissions"></a><span data-ttu-id="41656-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="41656-108">Permissions</span></span>

<span data-ttu-id="41656-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="41656-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="41656-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="41656-111">Permission type</span></span>                        | <span data-ttu-id="41656-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="41656-112">Permissions (from least to most privileged)</span></span>
|:---------------------------------------|:-------------------------------------------
| <span data-ttu-id="41656-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="41656-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="41656-114">Files. Read, files. ReadWrite, files. ReadWrite. all, Sites. ReadWrite. all</span><span class="sxs-lookup"><span data-stu-id="41656-114">Files.Read, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>
| <span data-ttu-id="41656-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="41656-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="41656-116">Files. Read, files. ReadWrite, files. ReadWrite. all</span><span class="sxs-lookup"><span data-stu-id="41656-116">Files.Read, Files.ReadWrite, Files.ReadWrite.All</span></span>
| <span data-ttu-id="41656-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="41656-117">Application</span></span>                            | <span data-ttu-id="41656-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="41656-118">Not supported.</span></span>

## <a name="http-request"></a><span data-ttu-id="41656-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="41656-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/drive/root/subscriptions/socketIo
GET /drives/{driveId}/root/subscriptions/socketIo
GET /groups/{groupId}/drive/root/subscriptions/socketIo
GET /sites/{siteId}/lists/{listId}/drive/root/subscriptions/socketIo
```

## <a name="example"></a><span data-ttu-id="41656-120">Beispiel</span><span class="sxs-lookup"><span data-stu-id="41656-120">Example</span></span>

### <a name="request"></a><span data-ttu-id="41656-121">Anforderung</span><span class="sxs-lookup"><span data-stu-id="41656-121">Request</span></span>

<!-- { "blockType": "request", "name": "drive_root_subscriptions_socketIo" } -->
```http
GET /me/drive/root/subscriptions/socketIo
```

### <a name="response"></a><span data-ttu-id="41656-122">Antwort</span><span class="sxs-lookup"><span data-stu-id="41656-122">Response</span></span>

<span data-ttu-id="41656-123">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein [Subscription](../resources/subscription.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="41656-123">If successful, this method returns a `200 OK` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>

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

<span data-ttu-id="41656-124">Die `notificationUrl` zurückgegebene ist eine Socket.IO-Endpunkt-URL.</span><span class="sxs-lookup"><span data-stu-id="41656-124">The `notificationUrl` returned is a socket.io endpoint URL.</span></span>
<span data-ttu-id="41656-125">Um es mit einem socket.io-Client zu verwenden, teilen Sie die `/callback?` Zeichenfolge auf dem Token.</span><span class="sxs-lookup"><span data-stu-id="41656-125">To use it with a socket.io client, split the string on the `/callback?` token.</span></span>
<span data-ttu-id="41656-126">Der Teil der Zeichenfolge ist `/callback?` vor der Socket.IO-Endpunkt-URL und der Teil der Zeichenfolge nach ist eine undurchsichtige Abfragezeichenfolge, die an die Bibliothek gegeben werden muss.</span><span class="sxs-lookup"><span data-stu-id="41656-126">The part of the string before `/callback?` is the socket.io endpoint URL and the part of the string after is an opaque query string that must be given to the libary.</span></span>

<span data-ttu-id="41656-127">Das folgende Beispiel zeigt, wie Sie `notificationUrl` mit Socket.IO in JavaScript verwenden.</span><span class="sxs-lookup"><span data-stu-id="41656-127">The following example shows how to use the `notificationUrl` with socket.io in JavaScript.</span></span>

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
