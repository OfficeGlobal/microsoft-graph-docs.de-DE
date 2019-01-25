---
title: 'Rufen Sie: Übertragung'
description: Weiterleiten eines aktiven Anrufs.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: b1c503be31b17fb608abbec340aa9390ce315435
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516252"
---
# <a name="call-transfer"></a><span data-ttu-id="966ac-103">Rufen Sie: Übertragung</span><span class="sxs-lookup"><span data-stu-id="966ac-103">call: transfer</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="966ac-104">Weiterleiten eines aktiven Anrufs.</span><span class="sxs-lookup"><span data-stu-id="966ac-104">Transfer an active call.</span></span>

## <a name="permissions"></a><span data-ttu-id="966ac-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="966ac-105">Permissions</span></span>
<span data-ttu-id="966ac-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="966ac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="966ac-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="966ac-108">Permission type</span></span> | <span data-ttu-id="966ac-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="966ac-109">Permissions (from least to most privileged)</span></span>         |
| :-------------- | :-------------------------------------------------- |
| <span data-ttu-id="966ac-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="966ac-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="966ac-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="966ac-111">Not Supported</span></span>                |
| <span data-ttu-id="966ac-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="966ac-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="966ac-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="966ac-113">Not Supported</span></span>                |
| <span data-ttu-id="966ac-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="966ac-114">Application</span></span>     | <span data-ttu-id="966ac-115">Calls.Initiate.All</span><span class="sxs-lookup"><span data-stu-id="966ac-115">Calls.Initiate.All</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="966ac-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="966ac-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/transfer
POST /applications/{id}/calls/{id}/transfer
```

## <a name="request-headers"></a><span data-ttu-id="966ac-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="966ac-117">Request headers</span></span>
| <span data-ttu-id="966ac-118">Name</span><span class="sxs-lookup"><span data-stu-id="966ac-118">Name</span></span>          | <span data-ttu-id="966ac-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="966ac-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="966ac-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="966ac-120">Authorization</span></span> | <span data-ttu-id="966ac-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="966ac-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="966ac-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="966ac-123">Request body</span></span>
<span data-ttu-id="966ac-124">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="966ac-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="966ac-125">Parameter</span><span class="sxs-lookup"><span data-stu-id="966ac-125">Parameter</span></span>      | <span data-ttu-id="966ac-126">Typ</span><span class="sxs-lookup"><span data-stu-id="966ac-126">Type</span></span>    |<span data-ttu-id="966ac-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="966ac-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="966ac-128">transferTarget</span><span class="sxs-lookup"><span data-stu-id="966ac-128">transferTarget</span></span>|[<span data-ttu-id="966ac-129">invitationParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="966ac-129">invitationParticipantInfo</span></span>](../resources/invitationparticipantinfo.md)|<span data-ttu-id="966ac-130">Der Teilnehmer, der das Ziel der Übertragung ist.</span><span class="sxs-lookup"><span data-stu-id="966ac-130">The participant which is the target of the transfer.</span></span>|
|<span data-ttu-id="966ac-131">ClientContext</span><span class="sxs-lookup"><span data-stu-id="966ac-131">clientContext</span></span>|<span data-ttu-id="966ac-132">String</span><span class="sxs-lookup"><span data-stu-id="966ac-132">String</span></span>|<span data-ttu-id="966ac-133">Der Clientkontext.</span><span class="sxs-lookup"><span data-stu-id="966ac-133">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="966ac-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="966ac-134">Response</span></span>
<span data-ttu-id="966ac-135">Gibt `202 Accepted` Antwortcode.</span><span class="sxs-lookup"><span data-stu-id="966ac-135">Returns `202 Accepted` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="966ac-136">Beispiele</span><span class="sxs-lookup"><span data-stu-id="966ac-136">Examples</span></span>

### <a name="transfer-call-directly-with-no-user-involvement"></a><span data-ttu-id="966ac-137">Anruf direkt mit ohne Benutzereingriff</span><span class="sxs-lookup"><span data-stu-id="966ac-137">Transfer call directly, with no user involvement</span></span>

<span data-ttu-id="966ac-138">Das folgende Beispiel illustriert, wie Sie diese API aufrufen können.</span><span class="sxs-lookup"><span data-stu-id="966ac-138">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="966ac-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="966ac-139">Request</span></span>
<span data-ttu-id="966ac-140">Das folgende Beispiel zeigt die Antwort.</span><span class="sxs-lookup"><span data-stu-id="966ac-140">The following example shows the request.</span></span>

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

##### <a name="response"></a><span data-ttu-id="966ac-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="966ac-141">Response</span></span>

> <span data-ttu-id="966ac-p103">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="966ac-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
}-->
```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---transferring"></a><span data-ttu-id="966ac-144">Benachrichtigung - Übertragung</span><span class="sxs-lookup"><span data-stu-id="966ac-144">Notification - transferring</span></span>

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

##### <a name="notification---transfer-accepted"></a><span data-ttu-id="966ac-145">Benachrichtigung - Übertragung akzeptiert</span><span class="sxs-lookup"><span data-stu-id="966ac-145">Notification - transfer accepted</span></span>

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

##### <a name="notification---terminated"></a><span data-ttu-id="966ac-146">Benachrichtigung - beendet</span><span class="sxs-lookup"><span data-stu-id="966ac-146">Notification - terminated</span></span>

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

### <a name="consultative-transfer"></a><span data-ttu-id="966ac-147">Konsultieren vor dem durchstellen</span><span class="sxs-lookup"><span data-stu-id="966ac-147">Consultative transfer</span></span>

##### <a name="request"></a><span data-ttu-id="966ac-148">Anfordern</span><span class="sxs-lookup"><span data-stu-id="966ac-148">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="966ac-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="966ac-149">Response</span></span>

> <span data-ttu-id="966ac-p104">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="966ac-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---transferring"></a><span data-ttu-id="966ac-152">Benachrichtigung - Übertragung</span><span class="sxs-lookup"><span data-stu-id="966ac-152">Notification - transferring</span></span>

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

##### <a name="notification---transfer-accepted"></a><span data-ttu-id="966ac-153">Benachrichtigung - Übertragung akzeptiert</span><span class="sxs-lookup"><span data-stu-id="966ac-153">Notification - transfer accepted</span></span>

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

##### <a name="notification---terminated"></a><span data-ttu-id="966ac-154">Benachrichtigung - beendet</span><span class="sxs-lookup"><span data-stu-id="966ac-154">Notification - terminated</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "call: transfer",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/call-transfer.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
