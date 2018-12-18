---
title: 'Rufen Sie: SubscribeToTone'
description: " Telefon."
author: VinodRavichandran
ms.openlocfilehash: 41c72cdeeb1017313f9f64c4bd268a2184229984
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27328301"
---
# <a name="call-subscribetotone"></a><span data-ttu-id="9b6ed-103">Rufen Sie: SubscribeToTone</span><span class="sxs-lookup"><span data-stu-id="9b6ed-103">call: subscribeToTone</span></span>

> <span data-ttu-id="9b6ed-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="9b6ed-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9b6ed-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9b6ed-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9b6ed-106">Abonnieren Sie DTMF (Dual-Tone Multi-Frequency Signaldaten).</span><span class="sxs-lookup"><span data-stu-id="9b6ed-106">Subscribe to DTMF (dual-tone multi-frequency signaling).</span></span> <span data-ttu-id="9b6ed-107">Dadurch können Sie benachrichtigt werden, wenn der Benutzer auf einem Telefon mit "Tonwahl" drückt.</span><span class="sxs-lookup"><span data-stu-id="9b6ed-107">This allows you to be notified when the user presses keys on a "touchtone" phone.</span></span>

## <a name="permissions"></a><span data-ttu-id="9b6ed-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="9b6ed-108">Permissions</span></span>
<span data-ttu-id="9b6ed-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9b6ed-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9b6ed-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9b6ed-111">Permission type</span></span> | <span data-ttu-id="9b6ed-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9b6ed-112">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="9b6ed-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9b6ed-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="9b6ed-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9b6ed-114">Not Supported</span></span>        |
| <span data-ttu-id="9b6ed-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9b6ed-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9b6ed-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9b6ed-116">Not Supported</span></span>        |
| <span data-ttu-id="9b6ed-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9b6ed-117">Application</span></span>     | <span data-ttu-id="9b6ed-118">Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="9b6ed-118">Calls.AccessMedia.All</span></span>                       |

## <a name="http-request"></a><span data-ttu-id="9b6ed-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9b6ed-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/subscribeToTone
POST /applications/{id}/calls/{id}/subscribeToTone
```

## <a name="request-headers"></a><span data-ttu-id="9b6ed-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9b6ed-120">Request headers</span></span>
| <span data-ttu-id="9b6ed-121">Name</span><span class="sxs-lookup"><span data-stu-id="9b6ed-121">Name</span></span>          | <span data-ttu-id="9b6ed-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9b6ed-122">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="9b6ed-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9b6ed-123">Authorization</span></span> | <span data-ttu-id="9b6ed-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9b6ed-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9b6ed-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9b6ed-126">Request body</span></span>
<span data-ttu-id="9b6ed-127">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="9b6ed-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="9b6ed-128">Parameter</span><span class="sxs-lookup"><span data-stu-id="9b6ed-128">Parameter</span></span>      | <span data-ttu-id="9b6ed-129">Typ</span><span class="sxs-lookup"><span data-stu-id="9b6ed-129">Type</span></span>    | <span data-ttu-id="9b6ed-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9b6ed-130">Description</span></span> |
|:---------------|:--------|:------------|
| <span data-ttu-id="9b6ed-131">clientContext</span><span class="sxs-lookup"><span data-stu-id="9b6ed-131">clientContext</span></span>  | <span data-ttu-id="9b6ed-132">String</span><span class="sxs-lookup"><span data-stu-id="9b6ed-132">String</span></span>  | <span data-ttu-id="9b6ed-133">Der Clientkontext.</span><span class="sxs-lookup"><span data-stu-id="9b6ed-133">The client context.</span></span> |

## <a name="response"></a><span data-ttu-id="9b6ed-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="9b6ed-134">Response</span></span>
<span data-ttu-id="9b6ed-135">Gibt `202 Accepted` Antwortcode und ein Location-Header mit einem Uri, um die [CommsOperation](../resources/commsoperation.md) für diese Anforderung erstellt.</span><span class="sxs-lookup"><span data-stu-id="9b6ed-135">Returns `202 Accepted` response code and a Location header with a uri to the [commsOperation](../resources/commsoperation.md) created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="9b6ed-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9b6ed-136">Example</span></span>
<span data-ttu-id="9b6ed-137">Das folgende Beispiel illustriert, wie Sie diese API aufrufen können.</span><span class="sxs-lookup"><span data-stu-id="9b6ed-137">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="9b6ed-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9b6ed-138">Request</span></span>
<span data-ttu-id="9b6ed-139">Das folgende Beispiel zeigt die Antwort.</span><span class="sxs-lookup"><span data-stu-id="9b6ed-139">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "call_subscribeToTone"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/subscribeToTone
Content-Type: application/json
Content-Length: 46

{
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c"
}
```

##### <a name="response"></a><span data-ttu-id="9b6ed-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="9b6ed-140">Response</span></span>

> <span data-ttu-id="9b6ed-p105">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="9b6ed-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.commsOperation"
} -->
```http
HTTP/1.1 202 Accepted
Location: https://graph.microsoft.com/beta/app/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5
```

##### <a name="notification---operation-completed"></a><span data-ttu-id="9b6ed-143">Benachrichtigung - Vorgang abgeschlossen</span><span class="sxs-lookup"><span data-stu-id="9b6ed-143">Notification - operation completed</span></span>

```http
POST https://bot.contoso.com/api/calls
Authorization: Bearer <TOKEN>
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "value": [
    {
      "changeType": "deleted",
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896/operations/0FE0623FD62842EDB4BD8AC290072CC5",
      "resourceData": {
        "@odata.type": "#microsoft.graph.commsOperation",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896/operations/0FE0623FD62842EDB4BD8AC290072CC5",
        "@odata.etag": "W/\"54451\"",
        "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c",
        "status": "completed"
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "call: subscribeToTone",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
