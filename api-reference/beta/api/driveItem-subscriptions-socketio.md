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
# <a name="get-websocket-endpoint"></a><span data-ttu-id="0fa21-103">Abrufen von Websocket-Endpunkt</span><span class="sxs-lookup"><span data-stu-id="0fa21-103">Get websocket endpoint</span></span>

> <span data-ttu-id="0fa21-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="0fa21-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span>
<span data-ttu-id="0fa21-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0fa21-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0fa21-106">Ermöglicht Ihnen, zum Empfangen von Benachrichtigungen für ein [Laufwerk][] mit [socket.io][]nahezu in Echtzeit ändern.</span><span class="sxs-lookup"><span data-stu-id="0fa21-106">Allows you to receive near-real-time change notifications for a [drive][] using [socket.io][].</span></span>
<span data-ttu-id="0fa21-107">Socket.IO ist eine häufig verwendete Benachrichtigungen-Bibliothek für JavaScript, das WebSockets nutzt.</span><span class="sxs-lookup"><span data-stu-id="0fa21-107">Socket.io is a popular notifications library for JavaScript that utilizes WebSockets.</span></span> <span data-ttu-id="0fa21-108">Weitere Informationen finden Sie unter [socket.io](https://socket.io).</span><span class="sxs-lookup"><span data-stu-id="0fa21-108">To learn more, see [socket.io](https://socket.io).</span></span>

[drive]: ../resources/drive.md
[Socket.IO]: https://socket.io/
[socket.io]: https://socket.io/

## <a name="permissions"></a><span data-ttu-id="0fa21-111">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="0fa21-111">Permissions</span></span>

<span data-ttu-id="0fa21-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0fa21-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0fa21-114">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0fa21-114">Permission type</span></span>                        | <span data-ttu-id="0fa21-115">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0fa21-115">Permissions (from least to most privileged)</span></span>
|:---------------------------------------|:-------------------------------------------
| <span data-ttu-id="0fa21-116">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0fa21-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="0fa21-117">Files.Read, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0fa21-117">Files.Read, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>
| <span data-ttu-id="0fa21-118">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0fa21-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0fa21-119">Files.Read, Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0fa21-119">Files.Read, Files.ReadWrite, Files.ReadWrite.All</span></span>
| <span data-ttu-id="0fa21-120">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0fa21-120">Application</span></span>                            | <span data-ttu-id="0fa21-121">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0fa21-121">Not supported.</span></span>

## <a name="http-request"></a><span data-ttu-id="0fa21-122">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0fa21-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/drive/root/subscriptions/socketIo
GET /drives/{driveId}/root/subscriptions/socketIo
GET /groups/{groupId}/drive/root/subscriptions/socketIo
GET /sites/{siteId}/lists/{listId}/drive/root/subscriptions/socketIo
```

## <a name="example"></a><span data-ttu-id="0fa21-123">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0fa21-123">Example</span></span>

### <a name="request"></a><span data-ttu-id="0fa21-124">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0fa21-124">Request</span></span>

<!-- { "blockType": "request", "name": "drive_root_subscriptions_socketIo" } -->
```http
GET /me/drive/root/subscriptions/socketIo
```

### <a name="response"></a><span data-ttu-id="0fa21-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="0fa21-125">Response</span></span>

<span data-ttu-id="0fa21-126">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und ein [Abonnement](../resources/subscription.md) -Objekt aus der Antwort.</span><span class="sxs-lookup"><span data-stu-id="0fa21-126">If successful, this method returns a `200 OK` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>

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

<span data-ttu-id="0fa21-127">Die `notificationUrl` socket.io-Endpunkt-URL zurückgegeben wird.</span><span class="sxs-lookup"><span data-stu-id="0fa21-127">The `notificationUrl` returned is a socket.io endpoint URL.</span></span>
<span data-ttu-id="0fa21-128">Die Zeichenfolge für die Verwendung mit einem Client socket.io auf Aufteilen der `/callback?` token.</span><span class="sxs-lookup"><span data-stu-id="0fa21-128">To use it with a socket.io client, split the string on the `/callback?` token.</span></span>
<span data-ttu-id="0fa21-129">Der Teil der Zeichenfolge vor dem `/callback?` ist die socket.io Endpunkt-URL und der Teil der Zeichenfolge nach ist eine undurchsichtige Abfragezeichenfolge, die in die Bibliothek zugewiesen werden soll.</span><span class="sxs-lookup"><span data-stu-id="0fa21-129">The part of the string before `/callback?` is the socket.io endpoint URL and the part of the string after is an opaque query string that must be given to the libary.</span></span>

<span data-ttu-id="0fa21-130">Das folgende Beispiel zeigt, wie Sie mit der `notificationUrl` mit socket.io in JavaScript.</span><span class="sxs-lookup"><span data-stu-id="0fa21-130">The following example shows how to use the `notificationUrl` with socket.io in JavaScript.</span></span>

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
