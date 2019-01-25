---
title: 'Rufen Sie: Antwort'
description: Beantworten eines eingehenden Anrufs an.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: c5a93121e5f01939ad28808f7055fcad98a734ff
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29530048"
---
# <a name="call-answer"></a><span data-ttu-id="d7d14-103">Rufen Sie: Antwort</span><span class="sxs-lookup"><span data-stu-id="d7d14-103">call: answer</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d7d14-104">Beantworten eines eingehenden Anrufs an.</span><span class="sxs-lookup"><span data-stu-id="d7d14-104">Answer an incoming call.</span></span>

## <a name="permissions"></a><span data-ttu-id="d7d14-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="d7d14-105">Permissions</span></span>
<span data-ttu-id="d7d14-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d7d14-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d7d14-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d7d14-108">Permission type</span></span> | <span data-ttu-id="d7d14-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d7d14-109">Permissions (from least to most privileged)</span></span>                 |
| :-------------- | :-----------------------------------------------------------|
| <span data-ttu-id="d7d14-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d7d14-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="d7d14-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d7d14-111">Not Supported</span></span>                        |
| <span data-ttu-id="d7d14-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d7d14-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d7d14-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d7d14-113">Not Supported</span></span>                        |
| <span data-ttu-id="d7d14-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d7d14-114">Application</span></span>     | <span data-ttu-id="d7d14-115">Keine</span><span class="sxs-lookup"><span data-stu-id="d7d14-115">None</span></span>                                                        |

## <a name="http-request"></a><span data-ttu-id="d7d14-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d7d14-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/answer
POST /applications/{id}/calls/{id}/answer
```

## <a name="request-headers"></a><span data-ttu-id="d7d14-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d7d14-117">Request headers</span></span>
| <span data-ttu-id="d7d14-118">Name</span><span class="sxs-lookup"><span data-stu-id="d7d14-118">Name</span></span>          | <span data-ttu-id="d7d14-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d7d14-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="d7d14-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="d7d14-120">Authorization</span></span> | <span data-ttu-id="d7d14-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d7d14-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d7d14-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d7d14-123">Request body</span></span>
<span data-ttu-id="d7d14-124">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="d7d14-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d7d14-125">Parameter</span><span class="sxs-lookup"><span data-stu-id="d7d14-125">Parameter</span></span>        | <span data-ttu-id="d7d14-126">Typ</span><span class="sxs-lookup"><span data-stu-id="d7d14-126">Type</span></span>                                     |<span data-ttu-id="d7d14-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d7d14-127">Description</span></span>                                                                                                                                    |
|:-----------------|:-----------------------------------------|:----------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="d7d14-128">callbackUri</span><span class="sxs-lookup"><span data-stu-id="d7d14-128">callbackUri</span></span>       |<span data-ttu-id="d7d14-129">String</span><span class="sxs-lookup"><span data-stu-id="d7d14-129">String</span></span>                                    |<span data-ttu-id="d7d14-130">Der Rückruf oder Abonnement-ID auf dem Rückrufe zugestellt werden.</span><span class="sxs-lookup"><span data-stu-id="d7d14-130">The callback or subscription ID on which callbacks will be delivered.</span></span> <span data-ttu-id="d7d14-131">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d7d14-131">(Required)</span></span>                                                               |
|<span data-ttu-id="d7d14-132">acceptedModalities</span><span class="sxs-lookup"><span data-stu-id="d7d14-132">acceptedModalities</span></span>|<span data-ttu-id="d7d14-133">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="d7d14-133">String collection</span></span>                         |<span data-ttu-id="d7d14-134">Die Liste der akzeptieren Modalitäten.</span><span class="sxs-lookup"><span data-stu-id="d7d14-134">The list of accept modalities.</span></span> <span data-ttu-id="d7d14-135">Mögliche Werte sind: `unknown`, `audio`, `video`, `screenSharing`, `videoBasedScreenSharing`, `data`.</span><span class="sxs-lookup"><span data-stu-id="d7d14-135">Possible value are: `unknown`, `audio`, `video`, `screenSharing`, `videoBasedScreenSharing`, `data`.</span></span> <span data-ttu-id="d7d14-136">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d7d14-136">(Required)</span></span> |
|<span data-ttu-id="d7d14-137">mediaConfig</span><span class="sxs-lookup"><span data-stu-id="d7d14-137">mediaConfig</span></span>       |[<span data-ttu-id="d7d14-138">mediaConfig</span><span class="sxs-lookup"><span data-stu-id="d7d14-138">mediaConfig</span></span>](../resources/mediaconfig.md)|<span data-ttu-id="d7d14-139">Die Medienkonfiguration.</span><span class="sxs-lookup"><span data-stu-id="d7d14-139">The media configuration.</span></span> <span data-ttu-id="d7d14-140">Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="d7d14-140">(Required)</span></span>                                                                                                            |

## <a name="response"></a><span data-ttu-id="d7d14-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="d7d14-141">Response</span></span>
<span data-ttu-id="d7d14-142">Diese Methode gibt `202 Accepted` Antwortcode.</span><span class="sxs-lookup"><span data-stu-id="d7d14-142">This method returns `202 Accepted` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="d7d14-143">Beispiele</span><span class="sxs-lookup"><span data-stu-id="d7d14-143">Examples</span></span>
<span data-ttu-id="d7d14-144">Das folgende Beispiel illustriert, wie Sie diese API aufrufen können.</span><span class="sxs-lookup"><span data-stu-id="d7d14-144">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="d7d14-145">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d7d14-145">Request</span></span>
<span data-ttu-id="d7d14-146">Das folgende Beispiel zeigt die Antwort.</span><span class="sxs-lookup"><span data-stu-id="d7d14-146">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "call-answer"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/answer
Content-Type: application/json
Content-Length: 211

{
  "callbackUri": "callbackUri-value",
  "mediaConfig": {
    "@odata.type": "#microsoft.graph.appHostedMediaConfig",
    "blob": "<media config blob>"
  },
  "acceptedModalities": [
    "audio"
  ]
}
```

##### <a name="response"></a><span data-ttu-id="d7d14-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="d7d14-147">Response</span></span>
<span data-ttu-id="d7d14-148">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="d7d14-148">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```

### <a name="answer-voip-call-with-service-hosted-media"></a><span data-ttu-id="d7d14-149">VOIP-Anruf mit gehosteten Dienst Medien</span><span class="sxs-lookup"><span data-stu-id="d7d14-149">Answer VOIP call with service hosted media</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="d7d14-150">Benachrichtigung - eingehende</span><span class="sxs-lookup"><span data-stu-id="d7d14-150">Notification - incoming</span></span>

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
        "callRoutes": [
          {
            "routingType": "lookup",
            "original": {
              "phone": {
                "id": "+14258828080"
              }
            },
            "final": {
              "user": {
                "id": "29362BD4-CD58-4ED0-A206-0E4A33DBB0B6",
                "displayName": "Heidi Steen"
              }
            }
          }
        ],
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
            "languageId": "en-US"
          }
        ],
        "requestedModalities": [ "audio" ]
      }
    }
  ]
}
```

##### <a name="request"></a><span data-ttu-id="d7d14-151">Anfordern</span><span class="sxs-lookup"><span data-stu-id="d7d14-151">Request</span></span>

```http
POST /app/calls/57DAB8B1894C409AB240BD8BEAE78896/answer
Authorization: Bearer <TOKEN>
Content-Type: application/json
```

<!-- {
  "blockType": "ignored",
  "name": "call-answer"
}-->
```json
{
  "callbackUri": "https://bot.contoso.com/api/calls",
  "acceptedModalities": [ "audio" ],
  "mediaConfig": {
    "@odata.type": "#microsoft.graph.serviceHostedMediaConfig",
    "preFetchMedia": [
      {
        "uri": "https://cdn.contoso.com/beep.wav",
        "resourceId": "1D6DE2D4-CD51-4309-8DAA-70768651088E"
      },
      {
        "uri": "https://cdn.contoso.com/cool.wav",
        "resourceId": "1D6DE2D4-CD51-4309-8DAA-70768651088F"
      }
    ]
  }
}
```

##### <a name="response"></a><span data-ttu-id="d7d14-152">Antwort</span><span class="sxs-lookup"><span data-stu-id="d7d14-152">Response</span></span>

```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---establishing"></a><span data-ttu-id="d7d14-153">Benachrichtigung - Einrichtung</span><span class="sxs-lookup"><span data-stu-id="d7d14-153">Notification - establishing</span></span>

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
      "changeType": "updated",
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
        "@odata.etag": "W/\"5445\"",
        "state": "establishing"
      }
    }
  ]
}
```

##### <a name="notification---established"></a><span data-ttu-id="d7d14-154">Benachrichtigung - eingerichtet</span><span class="sxs-lookup"><span data-stu-id="d7d14-154">Notification - established</span></span>

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
      "changeType": "updated",
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
        "@odata.etag": "W/\"5445\"",
        "state": "established"
      }
    }
  ]
}
```

### <a name="answer-voip-call-with-application-hosted-media"></a><span data-ttu-id="d7d14-155">VOIP-Anruf mit gehostete Anwendungsmedien</span><span class="sxs-lookup"><span data-stu-id="d7d14-155">Answer VOIP call with application hosted media</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="d7d14-156">Benachrichtigung - eingehende</span><span class="sxs-lookup"><span data-stu-id="d7d14-156">Notification - incoming</span></span>

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
          "@odata.type": "#microsoft.graph.participantInfo",
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
            "@odata.type": "#microsoft.graph.participantInfo",
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
        "requestedModalities": [ "audio" ]
      }
    }
  ]
}
```

##### <a name="request"></a><span data-ttu-id="d7d14-157">Anfordern</span><span class="sxs-lookup"><span data-stu-id="d7d14-157">Request</span></span>

```http
POST /app/calls/57DAB8B1894C409AB240BD8BEAE78896/answer
Authorization: Bearer <TOKEN>
Content-Type: application/json
```

<!-- {
  "blockType": "ignored",
  "name": "call-answer"
}-->
```json
{
  "callbackUri": "https://bot.contoso.com/api/calls",
  "acceptedModalities": [ "audio" ],
  "mediaConfig": {
    "@odata.type": "#microsoft.graph.appHostedMediaConfig",
    "blob": "<media config blob>"
  }
}
```

##### <a name="response"></a><span data-ttu-id="d7d14-158">Antwort</span><span class="sxs-lookup"><span data-stu-id="d7d14-158">Response</span></span>

```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---establishing"></a><span data-ttu-id="d7d14-159">Benachrichtigung - Einrichtung</span><span class="sxs-lookup"><span data-stu-id="d7d14-159">Notification - establishing</span></span>

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
      "changeType": "updated",
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
        "@odata.etag": "W/\"5445\"",
        "state": "establishing"
      }
    }
  ]
}
```

##### <a name="notification---established"></a><span data-ttu-id="d7d14-160">Benachrichtigung - eingerichtet</span><span class="sxs-lookup"><span data-stu-id="d7d14-160">Notification - established</span></span>

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
      "changeType": "updated",
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
        "@odata.etag": "W/\"5445\"",
        "state": "established"
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
  "description": "call: answer",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/call-answer.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
