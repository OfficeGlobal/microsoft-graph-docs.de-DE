---
title: Abrufen von Websocket-Endpunkt
description: Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 736684812d2cbc10affed82a3f946d75731f6768
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519794"
---
# <a name="get-websocket-endpoint"></a><span data-ttu-id="8db02-103">Abrufen von Websocket-Endpunkt</span><span class="sxs-lookup"><span data-stu-id="8db02-103">Get websocket endpoint</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="8db02-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8db02-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8db02-105">Ermöglicht Ihnen, zum Empfangen von Benachrichtigungen für ein [Laufwerk][] mit [socket.io][]nahezu in Echtzeit ändern.</span><span class="sxs-lookup"><span data-stu-id="8db02-105">Allows you to receive near-real-time change notifications for a [drive][] using [socket.io][].</span></span>
<span data-ttu-id="8db02-106">Socket.IO ist eine häufig verwendete Benachrichtigungen-Bibliothek für JavaScript, das WebSockets nutzt.</span><span class="sxs-lookup"><span data-stu-id="8db02-106">Socket.io is a popular notifications library for JavaScript that utilizes WebSockets.</span></span> <span data-ttu-id="8db02-107">Weitere Informationen finden Sie unter [socket.io](https://socket.io).</span><span class="sxs-lookup"><span data-stu-id="8db02-107">To learn more, see [socket.io](https://socket.io).</span></span>

[drive]: ../resources/drive.md
[Socket.IO]: https://socket.io/
[socket.io]: https://socket.io/

## <a name="permissions"></a><span data-ttu-id="8db02-110">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="8db02-110">Permissions</span></span>

<span data-ttu-id="8db02-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8db02-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8db02-113">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8db02-113">Permission type</span></span>                        | <span data-ttu-id="8db02-114">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8db02-114">Permissions (from least to most privileged)</span></span>
|:---------------------------------------|:-------------------------------------------
| <span data-ttu-id="8db02-115">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8db02-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="8db02-116">Files.Read, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8db02-116">Files.Read, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>
| <span data-ttu-id="8db02-117">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8db02-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8db02-118">Files.Read, Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8db02-118">Files.Read, Files.ReadWrite, Files.ReadWrite.All</span></span>
| <span data-ttu-id="8db02-119">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8db02-119">Application</span></span>                            | <span data-ttu-id="8db02-120">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8db02-120">Not supported.</span></span>

## <a name="http-request"></a><span data-ttu-id="8db02-121">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8db02-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/drive/root/subscriptions/socketIo
GET /drives/{driveId}/root/subscriptions/socketIo
GET /groups/{groupId}/drive/root/subscriptions/socketIo
GET /sites/{siteId}/lists/{listId}/drive/root/subscriptions/socketIo
```

## <a name="example"></a><span data-ttu-id="8db02-122">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8db02-122">Example</span></span>

### <a name="request"></a><span data-ttu-id="8db02-123">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8db02-123">Request</span></span>

<!-- { "blockType": "request", "name": "drive_root_subscriptions_socketIo" } -->
```http
GET /me/drive/root/subscriptions/socketIo
```

### <a name="response"></a><span data-ttu-id="8db02-124">Antwort</span><span class="sxs-lookup"><span data-stu-id="8db02-124">Response</span></span>

<span data-ttu-id="8db02-125">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und ein [Abonnement](../resources/subscription.md) -Objekt aus der Antwort.</span><span class="sxs-lookup"><span data-stu-id="8db02-125">If successful, this method returns a `200 OK` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>

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

<span data-ttu-id="8db02-126">Die `notificationUrl` socket.io-Endpunkt-URL zurückgegeben wird.</span><span class="sxs-lookup"><span data-stu-id="8db02-126">The `notificationUrl` returned is a socket.io endpoint URL.</span></span>
<span data-ttu-id="8db02-127">Die Zeichenfolge für die Verwendung mit einem Client socket.io auf Aufteilen der `/callback?` token.</span><span class="sxs-lookup"><span data-stu-id="8db02-127">To use it with a socket.io client, split the string on the `/callback?` token.</span></span>
<span data-ttu-id="8db02-128">Der Teil der Zeichenfolge vor dem `/callback?` ist die socket.io Endpunkt-URL und der Teil der Zeichenfolge nach ist eine undurchsichtige Abfragezeichenfolge, die in die Bibliothek zugewiesen werden soll.</span><span class="sxs-lookup"><span data-stu-id="8db02-128">The part of the string before `/callback?` is the socket.io endpoint URL and the part of the string after is an opaque query string that must be given to the libary.</span></span>

<span data-ttu-id="8db02-129">Das folgende Beispiel zeigt, wie Sie mit der `notificationUrl` mit socket.io in JavaScript.</span><span class="sxs-lookup"><span data-stu-id="8db02-129">The following example shows how to use the `notificationUrl` with socket.io in JavaScript.</span></span>

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
