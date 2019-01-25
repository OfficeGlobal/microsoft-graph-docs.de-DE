---
title: 'Rufen Sie: SubscribeToTone'
description: Abonnieren Sie DTMF (Dual-Tone Multi-Frequency Signaldaten). Dadurch können Sie benachrichtigt werden, wenn der Benutzer auf einem Telefon mit 'Tonwahl' drückt.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: f3fe078965877204b767b689ace293c3d4f46a9d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519444"
---
# <a name="call-subscribetotone"></a><span data-ttu-id="fa0a5-104">Rufen Sie: SubscribeToTone</span><span class="sxs-lookup"><span data-stu-id="fa0a5-104">call: subscribeToTone</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fa0a5-105">Abonnieren Sie DTMF (Dual-Tone Multi-Frequency Signaldaten).</span><span class="sxs-lookup"><span data-stu-id="fa0a5-105">Subscribe to DTMF (dual-tone multi-frequency signaling).</span></span> <span data-ttu-id="fa0a5-106">Dadurch können Sie benachrichtigt werden, wenn der Benutzer auf einem Telefon mit "Tonwahl" drückt.</span><span class="sxs-lookup"><span data-stu-id="fa0a5-106">This allows you to be notified when the user presses keys on a "touchtone" phone.</span></span>

## <a name="permissions"></a><span data-ttu-id="fa0a5-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="fa0a5-107">Permissions</span></span>
<span data-ttu-id="fa0a5-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fa0a5-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fa0a5-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="fa0a5-110">Permission type</span></span> | <span data-ttu-id="fa0a5-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="fa0a5-111">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="fa0a5-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="fa0a5-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="fa0a5-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fa0a5-113">Not Supported</span></span>        |
| <span data-ttu-id="fa0a5-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="fa0a5-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fa0a5-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fa0a5-115">Not Supported</span></span>        |
| <span data-ttu-id="fa0a5-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="fa0a5-116">Application</span></span>     | <span data-ttu-id="fa0a5-117">Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="fa0a5-117">Calls.AccessMedia.All</span></span>                       |

## <a name="http-request"></a><span data-ttu-id="fa0a5-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="fa0a5-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/subscribeToTone
POST /applications/{id}/calls/{id}/subscribeToTone
```

## <a name="request-headers"></a><span data-ttu-id="fa0a5-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="fa0a5-119">Request headers</span></span>
| <span data-ttu-id="fa0a5-120">Name</span><span class="sxs-lookup"><span data-stu-id="fa0a5-120">Name</span></span>          | <span data-ttu-id="fa0a5-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fa0a5-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="fa0a5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="fa0a5-122">Authorization</span></span> | <span data-ttu-id="fa0a5-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="fa0a5-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fa0a5-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="fa0a5-125">Request body</span></span>
<span data-ttu-id="fa0a5-126">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="fa0a5-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="fa0a5-127">Parameter</span><span class="sxs-lookup"><span data-stu-id="fa0a5-127">Parameter</span></span>      | <span data-ttu-id="fa0a5-128">Typ</span><span class="sxs-lookup"><span data-stu-id="fa0a5-128">Type</span></span>    | <span data-ttu-id="fa0a5-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fa0a5-129">Description</span></span> |
|:---------------|:--------|:------------|
| <span data-ttu-id="fa0a5-130">ClientContext</span><span class="sxs-lookup"><span data-stu-id="fa0a5-130">clientContext</span></span>  | <span data-ttu-id="fa0a5-131">String</span><span class="sxs-lookup"><span data-stu-id="fa0a5-131">String</span></span>  | <span data-ttu-id="fa0a5-132">Der Clientkontext.</span><span class="sxs-lookup"><span data-stu-id="fa0a5-132">The client context.</span></span> |

## <a name="response"></a><span data-ttu-id="fa0a5-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="fa0a5-133">Response</span></span>
<span data-ttu-id="fa0a5-134">Gibt `202 Accepted` Antwortcode und ein Location-Header mit einem Uri, um die [CommsOperation](../resources/commsoperation.md) für diese Anforderung erstellt.</span><span class="sxs-lookup"><span data-stu-id="fa0a5-134">Returns `202 Accepted` response code and a Location header with a uri to the [commsOperation](../resources/commsoperation.md) created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="fa0a5-135">Beispiel</span><span class="sxs-lookup"><span data-stu-id="fa0a5-135">Example</span></span>
<span data-ttu-id="fa0a5-136">Das folgende Beispiel illustriert, wie Sie diese API aufrufen können.</span><span class="sxs-lookup"><span data-stu-id="fa0a5-136">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="fa0a5-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="fa0a5-137">Request</span></span>
<span data-ttu-id="fa0a5-138">Das folgende Beispiel zeigt die Antwort.</span><span class="sxs-lookup"><span data-stu-id="fa0a5-138">The following example shows the request.</span></span>

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

##### <a name="response"></a><span data-ttu-id="fa0a5-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="fa0a5-139">Response</span></span>

> <span data-ttu-id="fa0a5-p105">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="fa0a5-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.commsOperation"
} -->
```http
HTTP/1.1 202 Accepted
Location: https://graph.microsoft.com/beta/app/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5
```

##### <a name="notification---operation-completed"></a><span data-ttu-id="fa0a5-142">Benachrichtigung - Vorgang abgeschlossen</span><span class="sxs-lookup"><span data-stu-id="fa0a5-142">Notification - operation completed</span></span>

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
  "description": "call: subscribeToTone",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/call-subscribetotone.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
