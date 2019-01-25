---
title: 'Rufen Sie: CancelMediaProcessing'
description: Bricht Media Verarbeitung für alle laufenden Vorgänge PlayPrompt oder DNS-Eintrags.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 77c35cb0cfeaea6ebb2e623b32b1fa3c70f65777
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29527850"
---
# <a name="call-cancelmediaprocessing"></a><span data-ttu-id="4f4cf-103">Rufen Sie: CancelMediaProcessing</span><span class="sxs-lookup"><span data-stu-id="4f4cf-103">call: cancelMediaProcessing</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4f4cf-104">Bricht Media Verarbeitung für alle laufenden Vorgänge PlayPrompt oder DNS-Eintrags.</span><span class="sxs-lookup"><span data-stu-id="4f4cf-104">Cancels media processing for all in-progress any PlayPrompt or Record operations.</span></span>

## <a name="permissions"></a><span data-ttu-id="4f4cf-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="4f4cf-105">Permissions</span></span>
<span data-ttu-id="4f4cf-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4f4cf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4f4cf-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4f4cf-108">Permission type</span></span>                        | <span data-ttu-id="4f4cf-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4f4cf-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="4f4cf-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4f4cf-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="4f4cf-111">Nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4f4cf-111">Not Supported.</span></span>                              |
| <span data-ttu-id="4f4cf-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4f4cf-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4f4cf-113">Nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4f4cf-113">Not Supported.</span></span>                              |
| <span data-ttu-id="4f4cf-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4f4cf-114">Application</span></span>                            | <span data-ttu-id="4f4cf-115">Keine.</span><span class="sxs-lookup"><span data-stu-id="4f4cf-115">None.</span></span>                                       |

## <a name="http-request"></a><span data-ttu-id="4f4cf-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4f4cf-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/cancelMediaProcessing
POST /applications/{id}/calls/{id}/cancelMediaProcessing
```

## <a name="request-headers"></a><span data-ttu-id="4f4cf-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4f4cf-117">Request headers</span></span>
| <span data-ttu-id="4f4cf-118">Name</span><span class="sxs-lookup"><span data-stu-id="4f4cf-118">Name</span></span>          | <span data-ttu-id="4f4cf-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4f4cf-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="4f4cf-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="4f4cf-120">Authorization</span></span> | <span data-ttu-id="4f4cf-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="4f4cf-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4f4cf-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4f4cf-123">Request body</span></span>
<span data-ttu-id="4f4cf-124">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="4f4cf-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="4f4cf-125">Parameter</span><span class="sxs-lookup"><span data-stu-id="4f4cf-125">Parameter</span></span>      | <span data-ttu-id="4f4cf-126">Typ</span><span class="sxs-lookup"><span data-stu-id="4f4cf-126">Type</span></span>    | <span data-ttu-id="4f4cf-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4f4cf-127">Description</span></span>                                                    |
|:---------------|:--------|:---------------------------------------------------------------|
| <span data-ttu-id="4f4cf-128">all</span><span class="sxs-lookup"><span data-stu-id="4f4cf-128">all</span></span>            | <span data-ttu-id="4f4cf-129">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="4f4cf-129">Boolean</span></span> | <span data-ttu-id="4f4cf-130">Das Flag, der angibt, ob alle Vorgänge oder aktuellen beenden.</span><span class="sxs-lookup"><span data-stu-id="4f4cf-130">The flag indicating whether to stop all operations or current.</span></span> |
| <span data-ttu-id="4f4cf-131">ClientContext</span><span class="sxs-lookup"><span data-stu-id="4f4cf-131">clientContext</span></span>  | <span data-ttu-id="4f4cf-132">String</span><span class="sxs-lookup"><span data-stu-id="4f4cf-132">String</span></span>  | <span data-ttu-id="4f4cf-133">Der Clientkontext.</span><span class="sxs-lookup"><span data-stu-id="4f4cf-133">The client context.</span></span>                                            |

## <a name="response"></a><span data-ttu-id="4f4cf-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="4f4cf-134">Response</span></span>
<span data-ttu-id="4f4cf-135">Gibt `202 Accepted` Antwortcode und ein Location-Header mit einem Uri, um die [CommsOperation](../resources/commsoperation.md) für diese Anforderung erstellt.</span><span class="sxs-lookup"><span data-stu-id="4f4cf-135">Returns `202 Accepted` response code and a Location header with a uri to the [commsOperation](../resources/commsoperation.md) created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="4f4cf-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4f4cf-136">Example</span></span>
<span data-ttu-id="4f4cf-137">Das folgende Beispiel illustriert, wie Sie diese API aufrufen können.</span><span class="sxs-lookup"><span data-stu-id="4f4cf-137">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="4f4cf-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4f4cf-138">Request</span></span>
<span data-ttu-id="4f4cf-139">Das folgende Beispiel zeigt die Antwort.</span><span class="sxs-lookup"><span data-stu-id="4f4cf-139">The following example shows the request.</span></span>

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

##### <a name="response"></a><span data-ttu-id="4f4cf-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="4f4cf-140">Response</span></span>

> <span data-ttu-id="4f4cf-p103">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="4f4cf-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.commsOperation"
} -->
```http
HTTP/1.1 202 Accepted
Location: https://graph.microsoft.com/beta/app/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5
```

##### <a name="notification---operation-completed"></a><span data-ttu-id="4f4cf-143">Benachrichtigung - Vorgang abgeschlossen</span><span class="sxs-lookup"><span data-stu-id="4f4cf-143">Notification - operation completed</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "call: cancelMediaProcessing",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/call-cancelmediaprocessing.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
