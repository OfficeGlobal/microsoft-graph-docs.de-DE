---
title: 'Rufen Sie: PlayPrompt'
description: Wiedergabe einer Aufforderung in den Anruf.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 32ea1b838a71d40a6f6106a648962c6a77c29057
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29507789"
---
# <a name="call-playprompt"></a><span data-ttu-id="653be-103">Rufen Sie: PlayPrompt</span><span class="sxs-lookup"><span data-stu-id="653be-103">call: playPrompt</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="653be-104">Wiedergabe einer Aufforderung in den Anruf.</span><span class="sxs-lookup"><span data-stu-id="653be-104">Play a prompt in the call.</span></span>

## <a name="permissions"></a><span data-ttu-id="653be-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="653be-105">Permissions</span></span>
<span data-ttu-id="653be-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="653be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="653be-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="653be-108">Permission type</span></span>                        | <span data-ttu-id="653be-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="653be-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="653be-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="653be-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="653be-111">Nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="653be-111">Not Supported.</span></span>                               |
| <span data-ttu-id="653be-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="653be-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="653be-113">Nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="653be-113">Not Supported.</span></span>                               |
| <span data-ttu-id="653be-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="653be-114">Application</span></span>                            | <span data-ttu-id="653be-115">Keine.</span><span class="sxs-lookup"><span data-stu-id="653be-115">None.</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="653be-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="653be-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/playPrompt
POST /applications/{id}/calls/{id}/playPrompt
```

## <a name="request-headers"></a><span data-ttu-id="653be-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="653be-117">Request headers</span></span>
| <span data-ttu-id="653be-118">Name</span><span class="sxs-lookup"><span data-stu-id="653be-118">Name</span></span>          | <span data-ttu-id="653be-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="653be-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="653be-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="653be-120">Authorization</span></span> | <span data-ttu-id="653be-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="653be-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="653be-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="653be-123">Request body</span></span>
<span data-ttu-id="653be-124">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="653be-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="653be-125">Parameter</span><span class="sxs-lookup"><span data-stu-id="653be-125">Parameter</span></span>      | <span data-ttu-id="653be-126">Typ</span><span class="sxs-lookup"><span data-stu-id="653be-126">Type</span></span>    |<span data-ttu-id="653be-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="653be-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="653be-128">fordert</span><span class="sxs-lookup"><span data-stu-id="653be-128">prompts</span></span>|<span data-ttu-id="653be-129">[Prompt](../resources/prompt.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="653be-129">[prompt](../resources/prompt.md) collection</span></span>||
|<span data-ttu-id="653be-130">ClientContext</span><span class="sxs-lookup"><span data-stu-id="653be-130">clientContext</span></span>|<span data-ttu-id="653be-131">String</span><span class="sxs-lookup"><span data-stu-id="653be-131">String</span></span>|<span data-ttu-id="653be-132">Der Clientkontext.</span><span class="sxs-lookup"><span data-stu-id="653be-132">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="653be-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="653be-133">Response</span></span>
<span data-ttu-id="653be-134">Wenn der Vorgang erfolgreich war, gibt diese Methode `200 OK` Antwortobjekt Code und [PlayPromptOperation](../resources/playPromptOperation.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="653be-134">If successful, this method returns `200 OK` response code and [playPromptOperation](../resources/playPromptOperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="653be-135">Beispiel</span><span class="sxs-lookup"><span data-stu-id="653be-135">Example</span></span>
<span data-ttu-id="653be-136">Das folgende Beispiel illustriert, wie Sie diese API aufrufen können.</span><span class="sxs-lookup"><span data-stu-id="653be-136">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="653be-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="653be-137">Request</span></span>
<span data-ttu-id="653be-138">Das folgende Beispiel zeigt die Antwort.</span><span class="sxs-lookup"><span data-stu-id="653be-138">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "call-playPrompt"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/playPrompt
Content-Type: application/json
Content-Length: 166

{
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c",
  "prompts": [
    {
      "@odata.type": "#microsoft.graph.mediaPrompt",
      "mediaInfo": {
        "uri": "https://cdn.contoso.com/beep.wav",
        "resourceId": "1D6DE2D4-CD51-4309-8DAA-70768651088E"
      },
      "loop": 5
    }
  ]
}
```

##### <a name="response"></a><span data-ttu-id="653be-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="653be-139">Response</span></span>

> <span data-ttu-id="653be-p103">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="653be-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.playPromptOperation"
} -->
```http
HTTP/1.1 200 OK
Location: https://graph.microsoft.com/beta/app/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5
```

##### <a name="notification---operation-completed"></a><span data-ttu-id="653be-142">Benachrichtigung - Vorgang abgeschlossen</span><span class="sxs-lookup"><span data-stu-id="653be-142">Notification - operation completed</span></span>

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
        "@odata.type": "#microsoft.graph.playPromptOperation",
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
  "description": "call: playPrompt",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/call-playprompt.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
