---
title: 'Rufen Sie: ablehnen'
description: Ablehnen eines eingehenden Anrufs an.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 5b42ebee208431cd0a02be291d07f580d98c87a1
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516189"
---
# <a name="call-reject"></a><span data-ttu-id="30fbd-103">Rufen Sie: ablehnen</span><span class="sxs-lookup"><span data-stu-id="30fbd-103">call: reject</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="30fbd-104">Ablehnen eines eingehenden Anrufs an.</span><span class="sxs-lookup"><span data-stu-id="30fbd-104">Reject an incoming call.</span></span>

## <a name="permissions"></a><span data-ttu-id="30fbd-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="30fbd-105">Permissions</span></span>
<span data-ttu-id="30fbd-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="30fbd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="30fbd-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="30fbd-108">Permission type</span></span> | <span data-ttu-id="30fbd-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="30fbd-109">Permissions (from least to most privileged)</span></span>                |
| :-------------- | :--------------------------------------------------------- |
| <span data-ttu-id="30fbd-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="30fbd-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="30fbd-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="30fbd-111">Not Supported</span></span>                       |
| <span data-ttu-id="30fbd-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="30fbd-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="30fbd-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="30fbd-113">Not Supported</span></span>                       |
| <span data-ttu-id="30fbd-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="30fbd-114">Application</span></span>     | <span data-ttu-id="30fbd-115">Keine</span><span class="sxs-lookup"><span data-stu-id="30fbd-115">None</span></span>                                                       |

## <a name="http-request"></a><span data-ttu-id="30fbd-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="30fbd-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/reject
POST /applications/{id}/calls/{id}/reject
```

## <a name="request-headers"></a><span data-ttu-id="30fbd-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="30fbd-117">Request headers</span></span>
| <span data-ttu-id="30fbd-118">Name</span><span class="sxs-lookup"><span data-stu-id="30fbd-118">Name</span></span>          | <span data-ttu-id="30fbd-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="30fbd-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="30fbd-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="30fbd-120">Authorization</span></span> | <span data-ttu-id="30fbd-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="30fbd-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="30fbd-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="30fbd-123">Request body</span></span>
<span data-ttu-id="30fbd-124">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="30fbd-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="30fbd-125">Parameter</span><span class="sxs-lookup"><span data-stu-id="30fbd-125">Parameter</span></span>      | <span data-ttu-id="30fbd-126">Typ</span><span class="sxs-lookup"><span data-stu-id="30fbd-126">Type</span></span>    |<span data-ttu-id="30fbd-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="30fbd-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="30fbd-128">Grund</span><span class="sxs-lookup"><span data-stu-id="30fbd-128">reason</span></span>|<span data-ttu-id="30fbd-129">String</span><span class="sxs-lookup"><span data-stu-id="30fbd-129">String</span></span>|<span data-ttu-id="30fbd-130">Der Ablehnungsgrund für die.</span><span class="sxs-lookup"><span data-stu-id="30fbd-130">The rejection reason.</span></span>|

## <a name="response"></a><span data-ttu-id="30fbd-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="30fbd-131">Response</span></span>
<span data-ttu-id="30fbd-p103">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="30fbd-p103">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

```http
Returns `202 Accepted` response code
```

## <a name="example"></a><span data-ttu-id="30fbd-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="30fbd-134">Example</span></span>
<span data-ttu-id="30fbd-135">Das folgende Beispiel illustriert, wie Sie diese API aufrufen können.</span><span class="sxs-lookup"><span data-stu-id="30fbd-135">The following example shows how to call this API.</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="30fbd-136">Benachrichtigung - eingehende</span><span class="sxs-lookup"><span data-stu-id="30fbd-136">Notification - incoming</span></span>

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
      "changeType": "created",
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
        "@odata.etag": "W/\"5445\"",
        "state": "incoming",
        "direction": "incoming",
        "source": {
          "identity": {
            "user": {
              "displayName": "Test User",
              "id": "8A34A46B-3D17-4ADC-8DCE-DC4E7D572698"
            }
          },
          "region": "westus",
          "languageId": "en-US"
        },
        "targets": [
          {
            "identity": {
              "application": {
                "displayName": "Test BOT",
                "id": "8A34A46B-3D17-4ADC-8DCE-DC4E7D572698"
              }
            },
            "region": "westus",
            "languageId": "en-US"
          }
        ],
        "requestedModalities": [ "audio", "video" ]
      }
    }
  ]
}
```

##### <a name="request"></a><span data-ttu-id="30fbd-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="30fbd-137">Request</span></span>
<span data-ttu-id="30fbd-138">Das folgende Beispiel zeigt die Antwort.</span><span class="sxs-lookup"><span data-stu-id="30fbd-138">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "call-reject"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/reject
Content-Type: application/json
Content-Length: 24

{
  "reason": "none"
}
```

##### <a name="response"></a><span data-ttu-id="30fbd-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="30fbd-139">Response</span></span>
<span data-ttu-id="30fbd-140">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="30fbd-140">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---deleted"></a><span data-ttu-id="30fbd-141">Benachrichtigung - gelöscht</span><span class="sxs-lookup"><span data-stu-id="30fbd-141">Notification - deleted</span></span>

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
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
        "@odata.etag": "W/\"5445\""
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
  "description": "call: reject",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/call-reject.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
