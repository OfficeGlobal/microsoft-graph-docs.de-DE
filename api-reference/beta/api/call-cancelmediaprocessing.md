---
title: 'Rufen Sie: CancelMediaProcessing'
description: Bricht Media Verarbeitung für alle laufenden Vorgänge PlayPrompt oder DNS-Eintrags.
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: 9885e05bdca0d04daf597190eb118c81b8774c0a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27859451"
---
# <a name="call-cancelmediaprocessing"></a><span data-ttu-id="033f5-103">Rufen Sie: CancelMediaProcessing</span><span class="sxs-lookup"><span data-stu-id="033f5-103">call: cancelMediaProcessing</span></span>

> <span data-ttu-id="033f5-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="033f5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="033f5-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="033f5-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="033f5-106">Bricht Media Verarbeitung für alle laufenden Vorgänge PlayPrompt oder DNS-Eintrags.</span><span class="sxs-lookup"><span data-stu-id="033f5-106">Cancels media processing for all in-progress any PlayPrompt or Record operations.</span></span>

## <a name="permissions"></a><span data-ttu-id="033f5-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="033f5-107">Permissions</span></span>
<span data-ttu-id="033f5-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="033f5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="033f5-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="033f5-110">Permission type</span></span>                        | <span data-ttu-id="033f5-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="033f5-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="033f5-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="033f5-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="033f5-113">Nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="033f5-113">Not Supported.</span></span>                              |
| <span data-ttu-id="033f5-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="033f5-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="033f5-115">Nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="033f5-115">Not Supported.</span></span>                              |
| <span data-ttu-id="033f5-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="033f5-116">Application</span></span>                            | <span data-ttu-id="033f5-117">Keine.</span><span class="sxs-lookup"><span data-stu-id="033f5-117">None.</span></span>                                       |

## <a name="http-request"></a><span data-ttu-id="033f5-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="033f5-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/cancelMediaProcessing
POST /applications/{id}/calls/{id}/cancelMediaProcessing
```

## <a name="request-headers"></a><span data-ttu-id="033f5-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="033f5-119">Request headers</span></span>
| <span data-ttu-id="033f5-120">Name</span><span class="sxs-lookup"><span data-stu-id="033f5-120">Name</span></span>          | <span data-ttu-id="033f5-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="033f5-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="033f5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="033f5-122">Authorization</span></span> | <span data-ttu-id="033f5-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="033f5-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="033f5-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="033f5-125">Request body</span></span>
<span data-ttu-id="033f5-126">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="033f5-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="033f5-127">Parameter</span><span class="sxs-lookup"><span data-stu-id="033f5-127">Parameter</span></span>      | <span data-ttu-id="033f5-128">Typ</span><span class="sxs-lookup"><span data-stu-id="033f5-128">Type</span></span>    | <span data-ttu-id="033f5-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="033f5-129">Description</span></span>                                                    |
|:---------------|:--------|:---------------------------------------------------------------|
| <span data-ttu-id="033f5-130">all</span><span class="sxs-lookup"><span data-stu-id="033f5-130">all</span></span>            | <span data-ttu-id="033f5-131">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="033f5-131">Boolean</span></span> | <span data-ttu-id="033f5-132">Das Flag, der angibt, ob alle Vorgänge oder aktuellen beenden.</span><span class="sxs-lookup"><span data-stu-id="033f5-132">The flag indicating whether to stop all operations or current.</span></span> |
| <span data-ttu-id="033f5-133">clientContext</span><span class="sxs-lookup"><span data-stu-id="033f5-133">clientContext</span></span>  | <span data-ttu-id="033f5-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="033f5-134">String</span></span>  | <span data-ttu-id="033f5-135">Der Clientkontext.</span><span class="sxs-lookup"><span data-stu-id="033f5-135">The client context.</span></span>                                            |

## <a name="response"></a><span data-ttu-id="033f5-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="033f5-136">Response</span></span>
<span data-ttu-id="033f5-137">Gibt `202 Accepted` Antwortcode und ein Location-Header mit einem Uri, um die [CommsOperation](../resources/commsoperation.md) für diese Anforderung erstellt.</span><span class="sxs-lookup"><span data-stu-id="033f5-137">Returns `202 Accepted` response code and a Location header with a uri to the [commsOperation](../resources/commsoperation.md) created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="033f5-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="033f5-138">Example</span></span>
<span data-ttu-id="033f5-139">Das folgende Beispiel illustriert, wie Sie diese API aufrufen können.</span><span class="sxs-lookup"><span data-stu-id="033f5-139">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="033f5-140">Anforderung</span><span class="sxs-lookup"><span data-stu-id="033f5-140">Request</span></span>
<span data-ttu-id="033f5-141">Das folgende Beispiel zeigt die Antwort.</span><span class="sxs-lookup"><span data-stu-id="033f5-141">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "call-cancelMediaProcessing"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/cancelMediaProcessing
Content-Type: application/json
Content-Length: 62

{
  "all": true,
  "clientContext": "clientContext-value"
}
```

##### <a name="response"></a><span data-ttu-id="033f5-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="033f5-142">Response</span></span>

> <span data-ttu-id="033f5-p104">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="033f5-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.commsOperation"
} -->
```http
HTTP/1.1 202 Accepted
Location: https://graph.microsoft.com/beta/app/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5
```

##### <a name="notification---operation-completed"></a><span data-ttu-id="033f5-145">Benachrichtigung - Vorgang abgeschlossen</span><span class="sxs-lookup"><span data-stu-id="033f5-145">Notification - operation completed</span></span>

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
  "description": "call: cancelMediaProcessing",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
