---
title: 'Teilnehmer: stumm schalten'
description: Stummschalten eines bestimmten Teilnehmers in den Anruf.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 0fa4190ca6a3871c42af3c753cb3d9d48d320bd5
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521740"
---
# <a name="participant-mute"></a><span data-ttu-id="c2f84-103">Teilnehmer: stumm schalten</span><span class="sxs-lookup"><span data-stu-id="c2f84-103">participant: mute</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c2f84-104">Stummschalten eines bestimmten Teilnehmers in den Anruf.</span><span class="sxs-lookup"><span data-stu-id="c2f84-104">Mute a specific participant in the call.</span></span>

## <a name="permissions"></a><span data-ttu-id="c2f84-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="c2f84-105">Permissions</span></span>
<span data-ttu-id="c2f84-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c2f84-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c2f84-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c2f84-108">Permission type</span></span> | <span data-ttu-id="c2f84-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c2f84-109">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="c2f84-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c2f84-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="c2f84-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c2f84-111">Not Supported</span></span>        |
| <span data-ttu-id="c2f84-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c2f84-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c2f84-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c2f84-113">Not Supported</span></span>        |
| <span data-ttu-id="c2f84-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c2f84-114">Application</span></span>     | <span data-ttu-id="c2f84-115">Keine</span><span class="sxs-lookup"><span data-stu-id="c2f84-115">None</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="c2f84-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c2f84-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/participants/{id}/mute
POST /applications/{id}/calls/{id}/participants/{id}/mute
```

## <a name="request-headers"></a><span data-ttu-id="c2f84-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c2f84-117">Request headers</span></span>
| <span data-ttu-id="c2f84-118">Name</span><span class="sxs-lookup"><span data-stu-id="c2f84-118">Name</span></span>          | <span data-ttu-id="c2f84-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c2f84-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="c2f84-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="c2f84-120">Authorization</span></span> | <span data-ttu-id="c2f84-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c2f84-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c2f84-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c2f84-123">Request body</span></span>
<span data-ttu-id="c2f84-124">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="c2f84-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c2f84-125">Parameter</span><span class="sxs-lookup"><span data-stu-id="c2f84-125">Parameter</span></span>      | <span data-ttu-id="c2f84-126">Typ</span><span class="sxs-lookup"><span data-stu-id="c2f84-126">Type</span></span>    |<span data-ttu-id="c2f84-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c2f84-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c2f84-128">ClientContext</span><span class="sxs-lookup"><span data-stu-id="c2f84-128">clientContext</span></span>|<span data-ttu-id="c2f84-129">String</span><span class="sxs-lookup"><span data-stu-id="c2f84-129">String</span></span>|<span data-ttu-id="c2f84-130">Der Clientkontext.</span><span class="sxs-lookup"><span data-stu-id="c2f84-130">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="c2f84-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="c2f84-131">Response</span></span>
<span data-ttu-id="c2f84-132">Wenn der Vorgang erfolgreich war, gibt diese Methode `200 OK` Antwortobjekt Code und [CommsOperation](../resources/commsoperation.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="c2f84-132">If successful, this method returns `200 OK` response code and [commsOperation](../resources/commsoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c2f84-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c2f84-133">Example</span></span>
<span data-ttu-id="c2f84-134">Das folgende Beispiel illustriert, wie Sie diese API aufrufen können.</span><span class="sxs-lookup"><span data-stu-id="c2f84-134">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="c2f84-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c2f84-135">Request</span></span>
<span data-ttu-id="c2f84-136">Das folgende Beispiel zeigt die Antwort.</span><span class="sxs-lookup"><span data-stu-id="c2f84-136">The following example shows the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="c2f84-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="c2f84-137">Response</span></span>

> <span data-ttu-id="c2f84-p103">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="c2f84-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

## <a name="example---mute-specific-participant"></a><span data-ttu-id="c2f84-140">Beispiel - bestimmten Teilnehmer stumm schalten</span><span class="sxs-lookup"><span data-stu-id="c2f84-140">Example - Mute specific participant</span></span>

##### <a name="request"></a><span data-ttu-id="c2f84-141">Anfordern</span><span class="sxs-lookup"><span data-stu-id="c2f84-141">Request</span></span>

```http
POST /app/calls/57DAB8B1894C409AB240BD8BEAE78896/participants/0698446E77E24E4D85F80597083CB830/mute
Authorization: Bearer <TOKEN>
Content-Type: application/json

{
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c"
}
```

##### <a name="response"></a><span data-ttu-id="c2f84-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="c2f84-142">Response</span></span>

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

##### <a name="notification---roster-updated-with-participant-muted"></a><span data-ttu-id="c2f84-143">Benachrichtigung - Teilnehmerliste aktualisiert mit Teilnehmer stumm geschaltet.</span><span class="sxs-lookup"><span data-stu-id="c2f84-143">Notification - roster updated with participant muted</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "participant: mute",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/participant-mute.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
