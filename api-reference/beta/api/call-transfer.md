---
title: 'Rufen Sie: Übertragung'
description: Weiterleiten eines aktiven Anrufs.
author: VinodRavichandran
ms.openlocfilehash: 71d250453051c705dcc0646a8e4ad298253d0ee6
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380506"
---
# <a name="call-transfer"></a><span data-ttu-id="fc879-103">Rufen Sie: Übertragung</span><span class="sxs-lookup"><span data-stu-id="fc879-103">call: transfer</span></span>

> <span data-ttu-id="fc879-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="fc879-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fc879-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="fc879-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fc879-106">Weiterleiten eines aktiven Anrufs.</span><span class="sxs-lookup"><span data-stu-id="fc879-106">Transfer an active call.</span></span>

## <a name="permissions"></a><span data-ttu-id="fc879-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="fc879-107">Permissions</span></span>
<span data-ttu-id="fc879-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fc879-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fc879-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="fc879-110">Permission type</span></span> | <span data-ttu-id="fc879-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="fc879-111">Permissions (from least to most privileged)</span></span>         |
| :-------------- | :-------------------------------------------------- |
| <span data-ttu-id="fc879-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="fc879-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="fc879-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fc879-113">Not Supported</span></span>                |
| <span data-ttu-id="fc879-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="fc879-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fc879-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fc879-115">Not Supported</span></span>                |
| <span data-ttu-id="fc879-116">Application</span><span class="sxs-lookup"><span data-stu-id="fc879-116">Application</span></span>     | <span data-ttu-id="fc879-117">Calls.Initiate.All</span><span class="sxs-lookup"><span data-stu-id="fc879-117">Calls.Initiate.All</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="fc879-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="fc879-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/transfer
POST /applications/{id}/calls/{id}/transfer
```

## <a name="request-headers"></a><span data-ttu-id="fc879-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="fc879-119">Request headers</span></span>
| <span data-ttu-id="fc879-120">Name</span><span class="sxs-lookup"><span data-stu-id="fc879-120">Name</span></span>          | <span data-ttu-id="fc879-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fc879-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="fc879-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="fc879-122">Authorization</span></span> | <span data-ttu-id="fc879-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="fc879-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fc879-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="fc879-125">Request body</span></span>
<span data-ttu-id="fc879-126">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="fc879-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="fc879-127">Parameter</span><span class="sxs-lookup"><span data-stu-id="fc879-127">Parameter</span></span>      | <span data-ttu-id="fc879-128">Typ</span><span class="sxs-lookup"><span data-stu-id="fc879-128">Type</span></span>    |<span data-ttu-id="fc879-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fc879-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fc879-130">transferTarget</span><span class="sxs-lookup"><span data-stu-id="fc879-130">transferTarget</span></span>|[<span data-ttu-id="fc879-131">invitationParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="fc879-131">invitationParticipantInfo</span></span>](../resources/invitationparticipantinfo.md)|<span data-ttu-id="fc879-132">Der Teilnehmer, der das Ziel der Übertragung ist.</span><span class="sxs-lookup"><span data-stu-id="fc879-132">The participant which is the target of the transfer.</span></span>|
|<span data-ttu-id="fc879-133">clientContext</span><span class="sxs-lookup"><span data-stu-id="fc879-133">clientContext</span></span>|<span data-ttu-id="fc879-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fc879-134">String</span></span>|<span data-ttu-id="fc879-135">Der Clientkontext.</span><span class="sxs-lookup"><span data-stu-id="fc879-135">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="fc879-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="fc879-136">Response</span></span>
<span data-ttu-id="fc879-137">Gibt `202 Accepted` Antwortcode.</span><span class="sxs-lookup"><span data-stu-id="fc879-137">Returns `202 Accepted` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="fc879-138">Beispiele</span><span class="sxs-lookup"><span data-stu-id="fc879-138">Examples</span></span>

### <a name="transfer-call-directly-with-no-user-involvement"></a><span data-ttu-id="fc879-139">Anruf direkt mit ohne Benutzereingriff</span><span class="sxs-lookup"><span data-stu-id="fc879-139">Transfer call directly, with no user involvement</span></span>

<span data-ttu-id="fc879-140">Das folgende Beispiel illustriert, wie Sie diese API aufrufen können.</span><span class="sxs-lookup"><span data-stu-id="fc879-140">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="fc879-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="fc879-141">Request</span></span>
<span data-ttu-id="fc879-142">Das folgende Beispiel zeigt die Antwort.</span><span class="sxs-lookup"><span data-stu-id="fc879-142">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "call-transfer"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/transfer
Content-Type: application/json
Content-Length: 430

{
  "transferTarget": {
    "endpointType": "default",
    "identity": {
      "user": {
        "id": "550fae72-d251-43ec-868c-373732c2704f",
        "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
        "displayName": "Heidi Steen"
      }
    },
    "languageId": "languageId-value",
    "region": "region-value",
    "replacesCallId": "replacesCallId-value"
  },
  "clientContext": "clientContext-value"
}
```

##### <a name="response"></a><span data-ttu-id="fc879-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="fc879-143">Response</span></span>

> <span data-ttu-id="fc879-p104">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="fc879-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
}-->
```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---transferring"></a><span data-ttu-id="fc879-146">Benachrichtigung - Übertragung</span><span class="sxs-lookup"><span data-stu-id="fc879-146">Notification - transferring</span></span>

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
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896/operations/0FE0623FD62842EDB4BD8AC290072CC5",
      "resourceData": {
        "@odata.type": "#microsoft.graph.commsOperation",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896/operations/0FE0623FD62842EDB4BD8AC290072CC5",
        "@odata.etag": "W/\"54451\"",
        "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c",
        "resultInfo": {
          "code": "200",
          "subCode": "transferring"
        },
        "status": "running"
      }
    }
  ]
}
```

##### <a name="notification---transfer-accepted"></a><span data-ttu-id="fc879-147">Benachrichtigung - Übertragung akzeptiert</span><span class="sxs-lookup"><span data-stu-id="fc879-147">Notification - transfer accepted</span></span>

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
        "resultInfo": {
          "code": "200",
          "subCode": "transferAccepted"
        },
        "status": "completed"
      }
    }
  ]
}
```

##### <a name="notification---terminated"></a><span data-ttu-id="fc879-148">Benachrichtigung - beendet</span><span class="sxs-lookup"><span data-stu-id="fc879-148">Notification - terminated</span></span>

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
        "terminationReason": "AppTransferred"
      }
    }
  ]
}
```

### <a name="consultative-transfer"></a><span data-ttu-id="fc879-149">Konsultieren vor dem durchstellen</span><span class="sxs-lookup"><span data-stu-id="fc879-149">Consultative transfer</span></span>

##### <a name="request"></a><span data-ttu-id="fc879-150">Anforderung</span><span class="sxs-lookup"><span data-stu-id="fc879-150">Request</span></span>

```http
POST /app/calls/57DAB8B1894C409AB240BD8BEAE78896/transfer
Authorization: Bearer <TOKEN>
Content-Type: application/json
```
<!-- {
  "blockType": "ignored",
  "@odata.type": "call-transfer"
}-->
```json
{
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c",
  "transferTarget": {
    "endpointType": "default",
    "identity": {
      "user": {
        "id": "550fae72-d251-43ec-868c-373732c2704f",
        "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
        "displayName": "Heidi Steen"
      }
    },
    "languageId": "en-US",
    "region": "westus",
    "replacesCallId": "e5d39592-99bd-4db8-bca8-30fb894ec51d"
  }
}
```

##### <a name="response"></a><span data-ttu-id="fc879-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="fc879-151">Response</span></span>

> <span data-ttu-id="fc879-p105">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="fc879-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---transferring"></a><span data-ttu-id="fc879-154">Benachrichtigung - Übertragung</span><span class="sxs-lookup"><span data-stu-id="fc879-154">Notification - transferring</span></span>

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
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896/operations/0FE0623FD62842EDB4BD8AC290072CC5",
      "resourceData": {
        "@odata.type": "#microsoft.graph.commsOperation",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896/operations/0FE0623FD62842EDB4BD8AC290072CC5",
        "@odata.etag": "W/\"54451\"",
        "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c",
        "resultInfo": {
          "code": "200",
          "subCode": "transferring"
        },
        "status": "running"
      }
    }
  ]
}
```

##### <a name="notification---transfer-accepted"></a><span data-ttu-id="fc879-155">Benachrichtigung - Übertragung akzeptiert</span><span class="sxs-lookup"><span data-stu-id="fc879-155">Notification - transfer accepted</span></span>

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
        "resultInfo": {
          "code": "200",
          "subCode": "transferAccepted"
        },
        "status": "completed"
      }
    }
  ]
}
```

##### <a name="notification---terminated"></a><span data-ttu-id="fc879-156">Benachrichtigung - beendet</span><span class="sxs-lookup"><span data-stu-id="fc879-156">Notification - terminated</span></span>

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
        "terminationReason": "AppTransferred"
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "call: transfer",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
