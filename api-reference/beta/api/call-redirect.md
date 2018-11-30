---
title: 'Rufen Sie: Umleiten'
description: Umleiten eines eingehenden Anrufs an.
ms.openlocfilehash: eeaff645c89910ac5dee4bc143d517cdd26389d1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058660"
---
# <a name="call-redirect"></a><span data-ttu-id="97a5f-103">Rufen Sie: Umleiten</span><span class="sxs-lookup"><span data-stu-id="97a5f-103">call: redirect</span></span>

> <span data-ttu-id="97a5f-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="97a5f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="97a5f-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="97a5f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="97a5f-106">Umleiten eines eingehenden Anrufs an.</span><span class="sxs-lookup"><span data-stu-id="97a5f-106">Redirect an incoming call.</span></span>

## <a name="permissions"></a><span data-ttu-id="97a5f-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="97a5f-107">Permissions</span></span>
<span data-ttu-id="97a5f-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="97a5f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="97a5f-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="97a5f-110">Permission type</span></span> | <span data-ttu-id="97a5f-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="97a5f-111">Permissions (from least to most privileged)</span></span>         |
| :-------------- | :-------------------------------------------------- |
| <span data-ttu-id="97a5f-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="97a5f-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="97a5f-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="97a5f-113">Not Supported</span></span>                |
| <span data-ttu-id="97a5f-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="97a5f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="97a5f-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="97a5f-115">Not Supported</span></span>                |
| <span data-ttu-id="97a5f-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="97a5f-116">Application</span></span>     | <span data-ttu-id="97a5f-117">Calls.Initiate.All</span><span class="sxs-lookup"><span data-stu-id="97a5f-117">Calls.Initiate.All</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="97a5f-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="97a5f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/redirect
POST /applications/{id}/calls/{id}/redirect
```

## <a name="request-headers"></a><span data-ttu-id="97a5f-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="97a5f-119">Request headers</span></span>
| <span data-ttu-id="97a5f-120">Name</span><span class="sxs-lookup"><span data-stu-id="97a5f-120">Name</span></span>          | <span data-ttu-id="97a5f-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="97a5f-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="97a5f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="97a5f-122">Authorization</span></span> | <span data-ttu-id="97a5f-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="97a5f-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="97a5f-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="97a5f-125">Request body</span></span>
<span data-ttu-id="97a5f-126">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="97a5f-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="97a5f-127">Parameter</span><span class="sxs-lookup"><span data-stu-id="97a5f-127">Parameter</span></span>      | <span data-ttu-id="97a5f-128">Typ</span><span class="sxs-lookup"><span data-stu-id="97a5f-128">Type</span></span>    |<span data-ttu-id="97a5f-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="97a5f-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="97a5f-130">Ziele</span><span class="sxs-lookup"><span data-stu-id="97a5f-130">targets</span></span>|<span data-ttu-id="97a5f-131">[InvitationParticipantInfo](../resources/invitationparticipantinfo.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="97a5f-131">[invitationParticipantInfo](../resources/invitationparticipantinfo.md) collection</span></span>|<span data-ttu-id="97a5f-132">Die Teilnehmer Ziel des Vorgangs umleiten.</span><span class="sxs-lookup"><span data-stu-id="97a5f-132">The target participants of the redirect operation.</span></span>|
|<span data-ttu-id="97a5f-133">targetDisposition</span><span class="sxs-lookup"><span data-stu-id="97a5f-133">targetDisposition</span></span>|<span data-ttu-id="97a5f-134">String</span><span class="sxs-lookup"><span data-stu-id="97a5f-134">String</span></span>|<span data-ttu-id="97a5f-135">Der Wert ist:`default`</span><span class="sxs-lookup"><span data-stu-id="97a5f-135">The possible value is: `default`</span></span>|
|<span data-ttu-id="97a5f-136">timeout</span><span class="sxs-lookup"><span data-stu-id="97a5f-136">timeout</span></span>|<span data-ttu-id="97a5f-137">Int32</span><span class="sxs-lookup"><span data-stu-id="97a5f-137">Int32</span></span>|<span data-ttu-id="97a5f-138">Das Zeitlimit in Sekunden für den Umleitungsvorgang.</span><span class="sxs-lookup"><span data-stu-id="97a5f-138">The timeout in seconds for the redirect operation.</span></span>|
|<span data-ttu-id="97a5f-139">maskCallee</span><span class="sxs-lookup"><span data-stu-id="97a5f-139">maskCallee</span></span>|<span data-ttu-id="97a5f-140">Boolesch</span><span class="sxs-lookup"><span data-stu-id="97a5f-140">Boolean</span></span>|<span data-ttu-id="97a5f-141">Gibt an, ob der aufgerufene maskieren.</span><span class="sxs-lookup"><span data-stu-id="97a5f-141">Indicates whether to mask the callee.</span></span>|
|<span data-ttu-id="97a5f-142">maskCaller</span><span class="sxs-lookup"><span data-stu-id="97a5f-142">maskCaller</span></span>|<span data-ttu-id="97a5f-143">Boolesch</span><span class="sxs-lookup"><span data-stu-id="97a5f-143">Boolean</span></span>|<span data-ttu-id="97a5f-144">Gibt an, ob den Anrufer maskieren.</span><span class="sxs-lookup"><span data-stu-id="97a5f-144">Indicates whether to mask the caller.</span></span>|

## <a name="response"></a><span data-ttu-id="97a5f-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="97a5f-145">Response</span></span>
<span data-ttu-id="97a5f-146">Gibt `202 Accepted` Antwortcode</span><span class="sxs-lookup"><span data-stu-id="97a5f-146">Returns `202 Accepted` response code</span></span>

## <a name="examples"></a><span data-ttu-id="97a5f-147">Beispiele</span><span class="sxs-lookup"><span data-stu-id="97a5f-147">Examples</span></span>

### <a name="redirect-a-call"></a><span data-ttu-id="97a5f-148">Umleiten eines Anrufs</span><span class="sxs-lookup"><span data-stu-id="97a5f-148">Redirect a call</span></span>

##### <a name="request"></a><span data-ttu-id="97a5f-149">Anforderung</span><span class="sxs-lookup"><span data-stu-id="97a5f-149">Request</span></span>
<span data-ttu-id="97a5f-150">Das folgende Beispiel zeigt die Antwort.</span><span class="sxs-lookup"><span data-stu-id="97a5f-150">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "call_redirect"
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

##### <a name="response"></a><span data-ttu-id="97a5f-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="97a5f-151">Response</span></span>

> <span data-ttu-id="97a5f-p104">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="97a5f-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```

### <a name="forward-a-call"></a><span data-ttu-id="97a5f-154">Weiterleiten eines Anrufs</span><span class="sxs-lookup"><span data-stu-id="97a5f-154">Forward a call</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="97a5f-155">Benachrichtigung - eingehende</span><span class="sxs-lookup"><span data-stu-id="97a5f-155">Notification - incoming</span></span>

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

##### <a name="request"></a><span data-ttu-id="97a5f-156">Anforderung</span><span class="sxs-lookup"><span data-stu-id="97a5f-156">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="97a5f-157">Antwort</span><span class="sxs-lookup"><span data-stu-id="97a5f-157">Response</span></span>

```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---redirecting"></a><span data-ttu-id="97a5f-158">Benachrichtigung - Umleitung</span><span class="sxs-lookup"><span data-stu-id="97a5f-158">Notification - redirecting</span></span>

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

##### <a name="notification---terminated"></a><span data-ttu-id="97a5f-159">Benachrichtigung - beendet</span><span class="sxs-lookup"><span data-stu-id="97a5f-159">Notification - terminated</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "call: redirect",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
