---
title: 'Rufen Sie: SubscribeToTone'
description: Abonnieren Sie DTMF (Dual-Tone Multi-Frequency Signaldaten). Dadurch können Sie benachrichtigt werden, wenn der Benutzer auf einem Telefon mit 'Tonwahl' drückt.
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: 226edd59e7d826dd7304ae45ec58c360e8ef3191
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27833432"
---
# <a name="call-subscribetotone"></a><span data-ttu-id="fad89-104">Rufen Sie: SubscribeToTone</span><span class="sxs-lookup"><span data-stu-id="fad89-104">call: subscribeToTone</span></span>

> <span data-ttu-id="fad89-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="fad89-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fad89-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="fad89-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fad89-107">Abonnieren Sie DTMF (Dual-Tone Multi-Frequency Signaldaten).</span><span class="sxs-lookup"><span data-stu-id="fad89-107">Subscribe to DTMF (dual-tone multi-frequency signaling).</span></span> <span data-ttu-id="fad89-108">Dadurch können Sie benachrichtigt werden, wenn der Benutzer auf einem Telefon mit "Tonwahl" drückt.</span><span class="sxs-lookup"><span data-stu-id="fad89-108">This allows you to be notified when the user presses keys on a "touchtone" phone.</span></span>

## <a name="permissions"></a><span data-ttu-id="fad89-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="fad89-109">Permissions</span></span>
<span data-ttu-id="fad89-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fad89-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fad89-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="fad89-112">Permission type</span></span> | <span data-ttu-id="fad89-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="fad89-113">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="fad89-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="fad89-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="fad89-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fad89-115">Not Supported</span></span>        |
| <span data-ttu-id="fad89-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="fad89-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fad89-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fad89-117">Not Supported</span></span>        |
| <span data-ttu-id="fad89-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="fad89-118">Application</span></span>     | <span data-ttu-id="fad89-119">Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="fad89-119">Calls.AccessMedia.All</span></span>                       |

## <a name="http-request"></a><span data-ttu-id="fad89-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="fad89-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/subscribeToTone
POST /applications/{id}/calls/{id}/subscribeToTone
```

## <a name="request-headers"></a><span data-ttu-id="fad89-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="fad89-121">Request headers</span></span>
| <span data-ttu-id="fad89-122">Name</span><span class="sxs-lookup"><span data-stu-id="fad89-122">Name</span></span>          | <span data-ttu-id="fad89-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fad89-123">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="fad89-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="fad89-124">Authorization</span></span> | <span data-ttu-id="fad89-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="fad89-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fad89-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="fad89-127">Request body</span></span>
<span data-ttu-id="fad89-128">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="fad89-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="fad89-129">Parameter</span><span class="sxs-lookup"><span data-stu-id="fad89-129">Parameter</span></span>      | <span data-ttu-id="fad89-130">Typ</span><span class="sxs-lookup"><span data-stu-id="fad89-130">Type</span></span>    | <span data-ttu-id="fad89-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fad89-131">Description</span></span> |
|:---------------|:--------|:------------|
| <span data-ttu-id="fad89-132">clientContext</span><span class="sxs-lookup"><span data-stu-id="fad89-132">clientContext</span></span>  | <span data-ttu-id="fad89-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fad89-133">String</span></span>  | <span data-ttu-id="fad89-134">Der Clientkontext.</span><span class="sxs-lookup"><span data-stu-id="fad89-134">The client context.</span></span> |

## <a name="response"></a><span data-ttu-id="fad89-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="fad89-135">Response</span></span>
<span data-ttu-id="fad89-136">Gibt `202 Accepted` Antwortcode und ein Location-Header mit einem Uri, um die [CommsOperation](../resources/commsoperation.md) für diese Anforderung erstellt.</span><span class="sxs-lookup"><span data-stu-id="fad89-136">Returns `202 Accepted` response code and a Location header with a uri to the [commsOperation](../resources/commsoperation.md) created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="fad89-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="fad89-137">Example</span></span>
<span data-ttu-id="fad89-138">Das folgende Beispiel illustriert, wie Sie diese API aufrufen können.</span><span class="sxs-lookup"><span data-stu-id="fad89-138">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="fad89-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="fad89-139">Request</span></span>
<span data-ttu-id="fad89-140">Das folgende Beispiel zeigt die Antwort.</span><span class="sxs-lookup"><span data-stu-id="fad89-140">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "call-subscribeToTone"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/subscribeToTone
Content-Type: application/json
Content-Length: 46

{
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c"
}
```

##### <a name="response"></a><span data-ttu-id="fad89-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="fad89-141">Response</span></span>

> <span data-ttu-id="fad89-p106">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="fad89-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.commsOperation"
} -->
```http
HTTP/1.1 202 Accepted
Location: https://graph.microsoft.com/beta/app/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5
```

##### <a name="notification---operation-completed"></a><span data-ttu-id="fad89-144">Benachrichtigung - Vorgang abgeschlossen</span><span class="sxs-lookup"><span data-stu-id="fad89-144">Notification - operation completed</span></span>

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
