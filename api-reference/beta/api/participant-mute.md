---
title: 'Teilnehmer: stumm schalten'
description: Stummschalten eines bestimmten Teilnehmers in den Anruf.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: d41d97556aff7093660c0cdfb75a43f8b862c0d7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27964473"
---
# <a name="participant-mute"></a><span data-ttu-id="e5c09-103">Teilnehmer: stumm schalten</span><span class="sxs-lookup"><span data-stu-id="e5c09-103">participant: mute</span></span>

> <span data-ttu-id="e5c09-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="e5c09-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e5c09-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e5c09-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e5c09-106">Stummschalten eines bestimmten Teilnehmers in den Anruf.</span><span class="sxs-lookup"><span data-stu-id="e5c09-106">Mute a specific participant in the call.</span></span>

## <a name="permissions"></a><span data-ttu-id="e5c09-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="e5c09-107">Permissions</span></span>
<span data-ttu-id="e5c09-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e5c09-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e5c09-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e5c09-110">Permission type</span></span> | <span data-ttu-id="e5c09-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e5c09-111">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="e5c09-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e5c09-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="e5c09-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e5c09-113">Not Supported</span></span>        |
| <span data-ttu-id="e5c09-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e5c09-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e5c09-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e5c09-115">Not Supported</span></span>        |
| <span data-ttu-id="e5c09-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e5c09-116">Application</span></span>     | <span data-ttu-id="e5c09-117">Keine</span><span class="sxs-lookup"><span data-stu-id="e5c09-117">None</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="e5c09-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e5c09-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/participants/{id}/mute
POST /applications/{id}/calls/{id}/participants/{id}/mute
```

## <a name="request-headers"></a><span data-ttu-id="e5c09-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e5c09-119">Request headers</span></span>
| <span data-ttu-id="e5c09-120">Name</span><span class="sxs-lookup"><span data-stu-id="e5c09-120">Name</span></span>          | <span data-ttu-id="e5c09-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e5c09-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="e5c09-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e5c09-122">Authorization</span></span> | <span data-ttu-id="e5c09-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e5c09-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e5c09-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e5c09-125">Request body</span></span>
<span data-ttu-id="e5c09-126">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="e5c09-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e5c09-127">Parameter</span><span class="sxs-lookup"><span data-stu-id="e5c09-127">Parameter</span></span>      | <span data-ttu-id="e5c09-128">Typ</span><span class="sxs-lookup"><span data-stu-id="e5c09-128">Type</span></span>    |<span data-ttu-id="e5c09-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e5c09-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e5c09-130">clientContext</span><span class="sxs-lookup"><span data-stu-id="e5c09-130">clientContext</span></span>|<span data-ttu-id="e5c09-131">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e5c09-131">String</span></span>|<span data-ttu-id="e5c09-132">Der Clientkontext.</span><span class="sxs-lookup"><span data-stu-id="e5c09-132">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="e5c09-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="e5c09-133">Response</span></span>
<span data-ttu-id="e5c09-134">Wenn der Vorgang erfolgreich war, gibt diese Methode `200 OK` Antwortobjekt Code und [CommsOperation](../resources/commsoperation.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="e5c09-134">If successful, this method returns `200 OK` response code and [commsOperation](../resources/commsoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e5c09-135">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e5c09-135">Example</span></span>
<span data-ttu-id="e5c09-136">Das folgende Beispiel illustriert, wie Sie diese API aufrufen können.</span><span class="sxs-lookup"><span data-stu-id="e5c09-136">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="e5c09-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e5c09-137">Request</span></span>
<span data-ttu-id="e5c09-138">Das folgende Beispiel zeigt die Antwort.</span><span class="sxs-lookup"><span data-stu-id="e5c09-138">The following example shows the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "participant-mute"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/participants/{id}/mute
Content-Type: application/json
Content-Length: 46

{
  "clientContext": "clientContext-value"
}
```

##### <a name="response"></a><span data-ttu-id="e5c09-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="e5c09-139">Response</span></span>

> <span data-ttu-id="e5c09-p104">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="e5c09-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.commsOperation",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 259

{
  "id": "17e3b46c-f61d-4f4d-9635-c626ef18e6ad",
  "status": "completed",
  "createdDateTime": "2018-09-06T15:58:41Z",
  "lastActionDateTime": "2018-09-06T15:58:41Z",
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c"
}
```

## <a name="example---mute-specific-participant"></a><span data-ttu-id="e5c09-142">Beispiel - bestimmten Teilnehmer stumm schalten</span><span class="sxs-lookup"><span data-stu-id="e5c09-142">Example - Mute specific participant</span></span>

##### <a name="request"></a><span data-ttu-id="e5c09-143">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e5c09-143">Request</span></span>

```http
POST /app/calls/57DAB8B1894C409AB240BD8BEAE78896/participants/0698446E77E24E4D85F80597083CB830/mute
Authorization: Bearer <TOKEN>
Content-Type: application/json

{
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c"
}
```

##### <a name="response"></a><span data-ttu-id="e5c09-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="e5c09-144">Response</span></span>

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 259
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsOperation",
  "truncated": true
}-->
```json
{
  "id": "17e3b46c-f61d-4f4d-9635-c626ef18e6ad",
  "status": "completed",
  "createdDateTime": "2018-09-06T15:58:41Z",
  "lastActionDateTime": "2018-09-06T15:58:41Z",
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c"
}
```

##### <a name="notification---roster-updated-with-participant-muted"></a><span data-ttu-id="e5c09-145">Benachrichtigung - Teilnehmerliste aktualisiert mit Teilnehmer stumm geschaltet.</span><span class="sxs-lookup"><span data-stu-id="e5c09-145">Notification - roster updated with participant muted</span></span>

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
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896/participants",
      "resourceData": [
        {
          "@odata.type": "#microsoft.graph.participant",
          "id": "0698446E77E24E4D85F80597083CB830",
          "info": {
            "identity": {
              "user": {
                "displayName": "Test User",
                "id": "8A34A46B-3D17-4ADC-8DCE-DC4E7D572698"
              }
            },
            "region": "westus",
            "languageId": "en-US"
          },
          "mediaStreams": [
            {
              "mediaType": "audio",
              "label": "main-audio",
              "sourceId": "1",
              "direction": "sendReceive",
              "serverMuted": false
            }
          ],
          "isMuted": true,
          "isInLobby": false
        },
        {
          "@odata.type": "#microsoft.graph.participant",
          "id": "123456W77E24E4D85F80597083CB830",
          "info": {
            "identity": {
              "application": {
                "displayName": "Test Bot",
                "id": "1234A46B-3D17-4ADC-8DCE-DC4E7D556789"
              }
            },
            "region": "westus",
            "languageId": "en-US"
          },
          "mediaStreams": [
            {
              "mediaType": "audio",
              "label": "main-audio",
              "sourceId": "2",
              "direction": "sendReceive",
              "serverMuted": false
            }
          ],
          "isInLobby": false
        }
      ]
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "participant: mute",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
