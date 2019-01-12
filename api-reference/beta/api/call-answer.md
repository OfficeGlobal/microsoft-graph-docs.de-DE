---
title: 'Rufen Sie: Antwort'
description: Beantworten eines eingehenden Anrufs an.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: d3927c41df6558b1c0d266afbdb25f1c12ac1e49
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27971613"
---
# <a name="call-answer"></a><span data-ttu-id="1c297-103">Rufen Sie: Antwort</span><span class="sxs-lookup"><span data-stu-id="1c297-103">call: answer</span></span>

> <span data-ttu-id="1c297-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="1c297-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1c297-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1c297-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1c297-106">Beantworten eines eingehenden Anrufs an.</span><span class="sxs-lookup"><span data-stu-id="1c297-106">Answer an incoming call.</span></span>

## <a name="permissions"></a><span data-ttu-id="1c297-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="1c297-107">Permissions</span></span>
<span data-ttu-id="1c297-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1c297-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1c297-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1c297-110">Permission type</span></span> | <span data-ttu-id="1c297-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1c297-111">Permissions (from least to most privileged)</span></span>                 |
| :-------------- | :-----------------------------------------------------------|
| <span data-ttu-id="1c297-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1c297-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="1c297-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1c297-113">Not Supported</span></span>                        |
| <span data-ttu-id="1c297-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1c297-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1c297-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1c297-115">Not Supported</span></span>                        |
| <span data-ttu-id="1c297-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1c297-116">Application</span></span>     | <span data-ttu-id="1c297-117">Keine</span><span class="sxs-lookup"><span data-stu-id="1c297-117">None</span></span>                                                        |

## <a name="http-request"></a><span data-ttu-id="1c297-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1c297-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/answer
POST /applications/{id}/calls/{id}/answer
```

## <a name="request-headers"></a><span data-ttu-id="1c297-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1c297-119">Request headers</span></span>
| <span data-ttu-id="1c297-120">Name</span><span class="sxs-lookup"><span data-stu-id="1c297-120">Name</span></span>          | <span data-ttu-id="1c297-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1c297-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="1c297-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1c297-122">Authorization</span></span> | <span data-ttu-id="1c297-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="1c297-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1c297-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1c297-125">Request body</span></span>
<span data-ttu-id="1c297-126">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="1c297-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="1c297-127">Parameter</span><span class="sxs-lookup"><span data-stu-id="1c297-127">Parameter</span></span>        | <span data-ttu-id="1c297-128">Typ</span><span class="sxs-lookup"><span data-stu-id="1c297-128">Type</span></span>                                     |<span data-ttu-id="1c297-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1c297-129">Description</span></span>                                                                                                                                    |
|:-----------------|:-----------------------------------------|:----------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="1c297-130">callbackUri</span><span class="sxs-lookup"><span data-stu-id="1c297-130">callbackUri</span></span>       |<span data-ttu-id="1c297-131">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1c297-131">String</span></span>                                    |<span data-ttu-id="1c297-132">Der Rückruf oder Abonnement-ID auf dem Rückrufe zugestellt werden.</span><span class="sxs-lookup"><span data-stu-id="1c297-132">The callback or subscription ID on which callbacks will be delivered.</span></span> <span data-ttu-id="1c297-133">(Erforderlich)</span><span class="sxs-lookup"><span data-stu-id="1c297-133">(Required)</span></span>                                                               |
|<span data-ttu-id="1c297-134">acceptedModalities</span><span class="sxs-lookup"><span data-stu-id="1c297-134">acceptedModalities</span></span>|<span data-ttu-id="1c297-135">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="1c297-135">String collection</span></span>                         |<span data-ttu-id="1c297-136">Die Liste der akzeptieren Modalitäten.</span><span class="sxs-lookup"><span data-stu-id="1c297-136">The list of accept modalities.</span></span> <span data-ttu-id="1c297-137">Mögliche Werte sind: `unknown`, `audio`, `video`, `screenSharing`, `videoBasedScreenSharing`, `data`.</span><span class="sxs-lookup"><span data-stu-id="1c297-137">Possible value are: `unknown`, `audio`, `video`, `screenSharing`, `videoBasedScreenSharing`, `data`.</span></span> <span data-ttu-id="1c297-138">(Erforderlich)</span><span class="sxs-lookup"><span data-stu-id="1c297-138">(Required)</span></span> |
|<span data-ttu-id="1c297-139">mediaConfig</span><span class="sxs-lookup"><span data-stu-id="1c297-139">mediaConfig</span></span>       |[<span data-ttu-id="1c297-140">mediaConfig</span><span class="sxs-lookup"><span data-stu-id="1c297-140">mediaConfig</span></span>](../resources/mediaconfig.md)|<span data-ttu-id="1c297-141">Die Medienkonfiguration.</span><span class="sxs-lookup"><span data-stu-id="1c297-141">The media configuration.</span></span> <span data-ttu-id="1c297-142">(Erforderlich)</span><span class="sxs-lookup"><span data-stu-id="1c297-142">(Required)</span></span>                                                                                                            |

## <a name="response"></a><span data-ttu-id="1c297-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="1c297-143">Response</span></span>
<span data-ttu-id="1c297-144">Diese Methode gibt `202 Accepted` Antwortcode.</span><span class="sxs-lookup"><span data-stu-id="1c297-144">This method returns `202 Accepted` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="1c297-145">Beispiele</span><span class="sxs-lookup"><span data-stu-id="1c297-145">Examples</span></span>
<span data-ttu-id="1c297-146">Das folgende Beispiel illustriert, wie Sie diese API aufrufen können.</span><span class="sxs-lookup"><span data-stu-id="1c297-146">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="1c297-147">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1c297-147">Request</span></span>
<span data-ttu-id="1c297-148">Das folgende Beispiel zeigt die Antwort.</span><span class="sxs-lookup"><span data-stu-id="1c297-148">The following example shows the request.</span></span>

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

##### <a name="response"></a><span data-ttu-id="1c297-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="1c297-149">Response</span></span>
<span data-ttu-id="1c297-150">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="1c297-150">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```

### <a name="answer-voip-call-with-service-hosted-media"></a><span data-ttu-id="1c297-151">VOIP-Anruf mit gehosteten Dienst Medien</span><span class="sxs-lookup"><span data-stu-id="1c297-151">Answer VOIP call with service hosted media</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="1c297-152">Benachrichtigung - eingehende</span><span class="sxs-lookup"><span data-stu-id="1c297-152">Notification - incoming</span></span>

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

##### <a name="request"></a><span data-ttu-id="1c297-153">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1c297-153">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="1c297-154">Antwort</span><span class="sxs-lookup"><span data-stu-id="1c297-154">Response</span></span>

```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---establishing"></a><span data-ttu-id="1c297-155">Benachrichtigung - Einrichtung</span><span class="sxs-lookup"><span data-stu-id="1c297-155">Notification - establishing</span></span>

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

##### <a name="notification---established"></a><span data-ttu-id="1c297-156">Benachrichtigung - eingerichtet</span><span class="sxs-lookup"><span data-stu-id="1c297-156">Notification - established</span></span>

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

### <a name="answer-voip-call-with-application-hosted-media"></a><span data-ttu-id="1c297-157">VOIP-Anruf mit gehostete Anwendungsmedien</span><span class="sxs-lookup"><span data-stu-id="1c297-157">Answer VOIP call with application hosted media</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="1c297-158">Benachrichtigung - eingehende</span><span class="sxs-lookup"><span data-stu-id="1c297-158">Notification - incoming</span></span>

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

##### <a name="request"></a><span data-ttu-id="1c297-159">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1c297-159">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="1c297-160">Antwort</span><span class="sxs-lookup"><span data-stu-id="1c297-160">Response</span></span>

```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---establishing"></a><span data-ttu-id="1c297-161">Benachrichtigung - Einrichtung</span><span class="sxs-lookup"><span data-stu-id="1c297-161">Notification - establishing</span></span>

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

##### <a name="notification---established"></a><span data-ttu-id="1c297-162">Benachrichtigung - eingerichtet</span><span class="sxs-lookup"><span data-stu-id="1c297-162">Notification - established</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "call: answer",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
