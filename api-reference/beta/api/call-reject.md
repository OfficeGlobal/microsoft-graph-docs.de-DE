---
title: 'Rufen Sie: ablehnen'
description: Ablehnen eines eingehenden Anrufs an.
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: 06037d86be99e162a57b54f77d7b4363062f5858
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27849476"
---
# <a name="call-reject"></a><span data-ttu-id="24a29-103">Rufen Sie: ablehnen</span><span class="sxs-lookup"><span data-stu-id="24a29-103">call: reject</span></span>

> <span data-ttu-id="24a29-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="24a29-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="24a29-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="24a29-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="24a29-106">Ablehnen eines eingehenden Anrufs an.</span><span class="sxs-lookup"><span data-stu-id="24a29-106">Reject an incoming call.</span></span>

## <a name="permissions"></a><span data-ttu-id="24a29-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="24a29-107">Permissions</span></span>
<span data-ttu-id="24a29-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="24a29-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="24a29-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="24a29-110">Permission type</span></span> | <span data-ttu-id="24a29-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="24a29-111">Permissions (from least to most privileged)</span></span>                |
| :-------------- | :--------------------------------------------------------- |
| <span data-ttu-id="24a29-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="24a29-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="24a29-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="24a29-113">Not Supported</span></span>                       |
| <span data-ttu-id="24a29-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="24a29-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="24a29-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="24a29-115">Not Supported</span></span>                       |
| <span data-ttu-id="24a29-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="24a29-116">Application</span></span>     | <span data-ttu-id="24a29-117">Keine</span><span class="sxs-lookup"><span data-stu-id="24a29-117">None</span></span>                                                       |

## <a name="http-request"></a><span data-ttu-id="24a29-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="24a29-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/reject
POST /applications/{id}/calls/{id}/reject
```

## <a name="request-headers"></a><span data-ttu-id="24a29-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="24a29-119">Request headers</span></span>
| <span data-ttu-id="24a29-120">Name</span><span class="sxs-lookup"><span data-stu-id="24a29-120">Name</span></span>          | <span data-ttu-id="24a29-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="24a29-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="24a29-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="24a29-122">Authorization</span></span> | <span data-ttu-id="24a29-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="24a29-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="24a29-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="24a29-125">Request body</span></span>
<span data-ttu-id="24a29-126">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="24a29-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="24a29-127">Parameter</span><span class="sxs-lookup"><span data-stu-id="24a29-127">Parameter</span></span>      | <span data-ttu-id="24a29-128">Typ</span><span class="sxs-lookup"><span data-stu-id="24a29-128">Type</span></span>    |<span data-ttu-id="24a29-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="24a29-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="24a29-130">Grund</span><span class="sxs-lookup"><span data-stu-id="24a29-130">reason</span></span>|<span data-ttu-id="24a29-131">String</span><span class="sxs-lookup"><span data-stu-id="24a29-131">String</span></span>|<span data-ttu-id="24a29-132">Der Ablehnungsgrund für die.</span><span class="sxs-lookup"><span data-stu-id="24a29-132">The rejection reason.</span></span>|

## <a name="response"></a><span data-ttu-id="24a29-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="24a29-133">Response</span></span>
<span data-ttu-id="24a29-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="24a29-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

```http
Returns `202 Accepted` response code
```

## <a name="example"></a><span data-ttu-id="24a29-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="24a29-136">Example</span></span>
<span data-ttu-id="24a29-137">Das folgende Beispiel illustriert, wie Sie diese API aufrufen können.</span><span class="sxs-lookup"><span data-stu-id="24a29-137">The following example shows how to call this API.</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="24a29-138">Benachrichtigung - eingehende</span><span class="sxs-lookup"><span data-stu-id="24a29-138">Notification - incoming</span></span>

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

##### <a name="request"></a><span data-ttu-id="24a29-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="24a29-139">Request</span></span>
<span data-ttu-id="24a29-140">Das folgende Beispiel zeigt die Antwort.</span><span class="sxs-lookup"><span data-stu-id="24a29-140">The following example shows the request.</span></span>

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

##### <a name="response"></a><span data-ttu-id="24a29-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="24a29-141">Response</span></span>
<span data-ttu-id="24a29-142">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="24a29-142">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---deleted"></a><span data-ttu-id="24a29-143">Benachrichtigung - gelöscht</span><span class="sxs-lookup"><span data-stu-id="24a29-143">Notification - deleted</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "call: reject",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
