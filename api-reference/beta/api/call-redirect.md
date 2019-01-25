---
title: 'Rufen Sie: Umleiten'
description: Umleiten eines eingehenden Anrufs an.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: a6a926aa082cc35896d11ec4124091b0d2c838c0
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511989"
---
# <a name="call-redirect"></a><span data-ttu-id="0b22a-103">Rufen Sie: Umleiten</span><span class="sxs-lookup"><span data-stu-id="0b22a-103">call: redirect</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0b22a-104">Umleiten eines eingehenden Anrufs an.</span><span class="sxs-lookup"><span data-stu-id="0b22a-104">Redirect an incoming call.</span></span>

## <a name="permissions"></a><span data-ttu-id="0b22a-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="0b22a-105">Permissions</span></span>
<span data-ttu-id="0b22a-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0b22a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0b22a-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0b22a-108">Permission type</span></span> | <span data-ttu-id="0b22a-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0b22a-109">Permissions (from least to most privileged)</span></span>         |
| :-------------- | :-------------------------------------------------- |
| <span data-ttu-id="0b22a-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0b22a-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="0b22a-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0b22a-111">Not Supported</span></span>                |
| <span data-ttu-id="0b22a-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0b22a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0b22a-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0b22a-113">Not Supported</span></span>                |
| <span data-ttu-id="0b22a-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0b22a-114">Application</span></span>     | <span data-ttu-id="0b22a-115">Calls.Initiate.All</span><span class="sxs-lookup"><span data-stu-id="0b22a-115">Calls.Initiate.All</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="0b22a-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0b22a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/redirect
POST /applications/{id}/calls/{id}/redirect
```

## <a name="request-headers"></a><span data-ttu-id="0b22a-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0b22a-117">Request headers</span></span>
| <span data-ttu-id="0b22a-118">Name</span><span class="sxs-lookup"><span data-stu-id="0b22a-118">Name</span></span>          | <span data-ttu-id="0b22a-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0b22a-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="0b22a-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="0b22a-120">Authorization</span></span> | <span data-ttu-id="0b22a-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0b22a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0b22a-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0b22a-123">Request body</span></span>
<span data-ttu-id="0b22a-124">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="0b22a-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="0b22a-125">Parameter</span><span class="sxs-lookup"><span data-stu-id="0b22a-125">Parameter</span></span>      | <span data-ttu-id="0b22a-126">Typ</span><span class="sxs-lookup"><span data-stu-id="0b22a-126">Type</span></span>    |<span data-ttu-id="0b22a-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0b22a-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0b22a-128">Ziele</span><span class="sxs-lookup"><span data-stu-id="0b22a-128">targets</span></span>|<span data-ttu-id="0b22a-129">[InvitationParticipantInfo](../resources/invitationparticipantinfo.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="0b22a-129">[invitationParticipantInfo](../resources/invitationparticipantinfo.md) collection</span></span>|<span data-ttu-id="0b22a-130">Die Teilnehmer Ziel des Vorgangs umleiten.</span><span class="sxs-lookup"><span data-stu-id="0b22a-130">The target participants of the redirect operation.</span></span>|
|<span data-ttu-id="0b22a-131">targetDisposition</span><span class="sxs-lookup"><span data-stu-id="0b22a-131">targetDisposition</span></span>|<span data-ttu-id="0b22a-132">String</span><span class="sxs-lookup"><span data-stu-id="0b22a-132">String</span></span>|<span data-ttu-id="0b22a-133">Der Wert ist:`default`</span><span class="sxs-lookup"><span data-stu-id="0b22a-133">The possible value is: `default`</span></span>|
|<span data-ttu-id="0b22a-134">timeout</span><span class="sxs-lookup"><span data-stu-id="0b22a-134">timeout</span></span>|<span data-ttu-id="0b22a-135">Int32</span><span class="sxs-lookup"><span data-stu-id="0b22a-135">Int32</span></span>|<span data-ttu-id="0b22a-136">Das Zeitlimit in Sekunden für den Umleitungsvorgang.</span><span class="sxs-lookup"><span data-stu-id="0b22a-136">The timeout in seconds for the redirect operation.</span></span>|
|<span data-ttu-id="0b22a-137">maskCallee</span><span class="sxs-lookup"><span data-stu-id="0b22a-137">maskCallee</span></span>|<span data-ttu-id="0b22a-138">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="0b22a-138">Boolean</span></span>|<span data-ttu-id="0b22a-139">Gibt an, ob der aufgerufene maskieren.</span><span class="sxs-lookup"><span data-stu-id="0b22a-139">Indicates whether to mask the callee.</span></span>|
|<span data-ttu-id="0b22a-140">maskCaller</span><span class="sxs-lookup"><span data-stu-id="0b22a-140">maskCaller</span></span>|<span data-ttu-id="0b22a-141">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="0b22a-141">Boolean</span></span>|<span data-ttu-id="0b22a-142">Gibt an, ob den Anrufer maskieren.</span><span class="sxs-lookup"><span data-stu-id="0b22a-142">Indicates whether to mask the caller.</span></span>|

## <a name="response"></a><span data-ttu-id="0b22a-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="0b22a-143">Response</span></span>
<span data-ttu-id="0b22a-144">Gibt `202 Accepted` Antwortcode</span><span class="sxs-lookup"><span data-stu-id="0b22a-144">Returns `202 Accepted` response code</span></span>

## <a name="examples"></a><span data-ttu-id="0b22a-145">Beispiele</span><span class="sxs-lookup"><span data-stu-id="0b22a-145">Examples</span></span>

### <a name="redirect-a-call"></a><span data-ttu-id="0b22a-146">Umleiten eines Anrufs</span><span class="sxs-lookup"><span data-stu-id="0b22a-146">Redirect a call</span></span>

##### <a name="request"></a><span data-ttu-id="0b22a-147">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0b22a-147">Request</span></span>
<span data-ttu-id="0b22a-148">Das folgende Beispiel zeigt die Antwort.</span><span class="sxs-lookup"><span data-stu-id="0b22a-148">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "call-redirect"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/redirect
Content-Type: application/json
Content-Length: 515

{
  "targets": [
    {
      "endpointType": "default",
      "identity": {
        "user": {
          "id": "550fae72-d251-43ec-868c-373732c2704f",
          "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
          "displayName": "Heidi Steen"
        }
      },
      "languageId": "en-US",
      "region": "westus"
    }
  ],
  "targetDisposition": "default",
  "timeout": 99,
  "maskCallee": false,
  "maskCaller": false
}
```

##### <a name="response"></a><span data-ttu-id="0b22a-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="0b22a-149">Response</span></span>

> <span data-ttu-id="0b22a-p103">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="0b22a-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```

### <a name="forward-a-call"></a><span data-ttu-id="0b22a-152">Weiterleiten eines Anrufs</span><span class="sxs-lookup"><span data-stu-id="0b22a-152">Forward a call</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="0b22a-153">Benachrichtigung - eingehende</span><span class="sxs-lookup"><span data-stu-id="0b22a-153">Notification - incoming</span></span>

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

##### <a name="request"></a><span data-ttu-id="0b22a-154">Anfordern</span><span class="sxs-lookup"><span data-stu-id="0b22a-154">Request</span></span>

```http
POST https://graph.microsoft.com/beta/app/calls/57DAB8B1894C409AB240BD8BEAE78896/redirect
Authorization: Bearer <TOKEN>
Content-Type: application/json

{
  "targets": [
    {
      "endpointType": "default",
      "identity": {
        "user": {
          "id": "8A34A46B-3D17-4ADC-8DCE-DC4E7D572699"
        }
      },
      "languageId": "en-US",
      "region": "westus"
    }
  ],
  "targetDisposition": "default",
  "timeout": 60,
  "maskCallee": false,
  "maskCaller": false
}
```

##### <a name="response"></a><span data-ttu-id="0b22a-155">Antwort</span><span class="sxs-lookup"><span data-stu-id="0b22a-155">Response</span></span>

```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---redirecting"></a><span data-ttu-id="0b22a-156">Benachrichtigung - Umleitung</span><span class="sxs-lookup"><span data-stu-id="0b22a-156">Notification - redirecting</span></span>

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
        "state": "redirecting"
      }
    }
  ]
}
```

##### <a name="notification---terminated"></a><span data-ttu-id="0b22a-157">Benachrichtigung - beendet</span><span class="sxs-lookup"><span data-stu-id="0b22a-157">Notification - terminated</span></span>

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
        "@odata.etag": "W/\"5445\"",
        "state": "terminated",
        "answeredBy": {
          "identity": {
            "user": {
              "displayName": "Test User 2",
              "id": "8A34A46B-3D17-4ADC-8DCE-DC4E7D572699"
            }
          }
        },
        "terminationReason": "AppRedirected"
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
  "description": "call: redirect",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/call-redirect.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
