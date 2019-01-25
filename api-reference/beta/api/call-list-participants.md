---
title: Liste Teilnehmer
description: Abrufen einer Liste der Teilnehmer-Objekte in den Anruf.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 4f4eb95e4aed03dfd9809f8afb0e3f3557717430
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29507621"
---
# <a name="list-participants"></a><span data-ttu-id="f8be5-103">Liste Teilnehmer</span><span class="sxs-lookup"><span data-stu-id="f8be5-103">List participants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f8be5-104">Abrufen einer Liste der Teilnehmer-Objekte in den Anruf.</span><span class="sxs-lookup"><span data-stu-id="f8be5-104">Retrieve a list of participant objects in the call.</span></span>

## <a name="permissions"></a><span data-ttu-id="f8be5-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f8be5-105">Permissions</span></span>
<span data-ttu-id="f8be5-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f8be5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f8be5-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f8be5-108">Permission type</span></span> | <span data-ttu-id="f8be5-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f8be5-109">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="f8be5-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f8be5-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="f8be5-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f8be5-111">Not Supported</span></span>        |
| <span data-ttu-id="f8be5-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f8be5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f8be5-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f8be5-113">Not Supported</span></span>        |
| <span data-ttu-id="f8be5-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f8be5-114">Application</span></span>     | <span data-ttu-id="f8be5-115">Keine</span><span class="sxs-lookup"><span data-stu-id="f8be5-115">None</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="f8be5-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f8be5-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /app/calls/{id}/participants
GET /applications/{id}/calls/{id}/participants
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f8be5-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="f8be5-117">Optional query parameters</span></span>
<span data-ttu-id="f8be5-118">Diese Methode unterstützt die [OData-Abfrage-Parameter](/graph/query-parameters) , mit denen die Antwort anpassen.</span><span class="sxs-lookup"><span data-stu-id="f8be5-118">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f8be5-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f8be5-119">Request headers</span></span>
| <span data-ttu-id="f8be5-120">Name</span><span class="sxs-lookup"><span data-stu-id="f8be5-120">Name</span></span>          | <span data-ttu-id="f8be5-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f8be5-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="f8be5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f8be5-122">Authorization</span></span> | <span data-ttu-id="f8be5-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f8be5-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f8be5-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f8be5-125">Request body</span></span>
<span data-ttu-id="f8be5-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="f8be5-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f8be5-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="f8be5-127">Response</span></span>
<span data-ttu-id="f8be5-128">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und Auflistung von Objekten im Antworttext [Teilnehmer](../resources/participant.md) .</span><span class="sxs-lookup"><span data-stu-id="f8be5-128">If successful, this method returns a `200 OK` response code and collection of [participant](../resources/participant.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f8be5-129">Beispiele</span><span class="sxs-lookup"><span data-stu-id="f8be5-129">Examples</span></span>

### <a name="example-1"></a><span data-ttu-id="f8be5-130">Beispiel 1</span><span class="sxs-lookup"><span data-stu-id="f8be5-130">Example 1</span></span>

##### <a name="request"></a><span data-ttu-id="f8be5-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f8be5-131">Request</span></span>
<span data-ttu-id="f8be5-132">Das folgende Beispiel zeigt die Antwort.</span><span class="sxs-lookup"><span data-stu-id="f8be5-132">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get-participants"
}-->
```http
GET https://graph.microsoft.com/beta/app/calls/{id}/participants
```

##### <a name="response"></a><span data-ttu-id="f8be5-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="f8be5-133">Response</span></span>

> <span data-ttu-id="f8be5-p103">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="f8be5-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.participant",
  "isCollection": true,
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1152

{
  "value": [
    {
      "id": "id-value",
      "info": {
        "identity": {
          "user": {
            "id": "550fae72-d251-43ec-868c-373732c2704f",
            "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
            "displayName": "Heidi Steen"
          }
        },
        "languageId": "languageId-value",
        "region": "region-value"
      },
      "isInLobby": false,
      "isMuted": true,
      "mediaStreams": [
        {
          "sourceId": "1",
          "direction": "sendReceive",
          "label": "main-audio",
          "mediaType": "audio",
          "serverMuted": false
        }
      ],
      "metadata": "metadata-value"
    }
  ]
}
```

### <a name="example-2"></a><span data-ttu-id="f8be5-136">Beispiel 2</span><span class="sxs-lookup"><span data-stu-id="f8be5-136">Example 2</span></span>

##### <a name="request"></a><span data-ttu-id="f8be5-137">Anfordern</span><span class="sxs-lookup"><span data-stu-id="f8be5-137">Request</span></span>

```http
GET /app/calls/57DAB8B1894C409AB240BD8BEAE78896/participants
Authorization: Bearer <TOKEN>
```

##### <a name="response"></a><span data-ttu-id="f8be5-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="f8be5-138">Response</span></span>

```http
HTTP/1.1 200 OK
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.participant",
  "isCollection": true,
  "truncated": true
}-->
```json
{
  "value": [
    {
      "id": "ABB33D04-3A2C-4D78-996F-9EEEF55EF119",
      "info": {
        "identity" : {
          "user" : {
            "displayName": "Test User",
            "id": "8A34A46B-3D17-4ADC-8DCE-DC4E7D572698"
          }
        },
        "region": "westus",
        "languageId": "en-US"
      },
      "mediaStreams": [
        {
          "sourceId": "1",
          "mediaType": "audio",
          "label": "main-audio",
          "direction": "sendReceive",
          "serverMuted": false
        }
      ]
    },
    {
      "id": "ABB33D04-3A2C-4D78-996F-9EEEF55EF119",
      "info": {
        "identity" : {
          "phone": {
            "displayName": "+12345678890",
            "id": "+12345678890"
          }
        }
      },
      "mediaStreams": [
        {
          "sourceId": "2",
          "mediaType": "audio",
          "label": "main-audio",
          "direction": "sendReceive",
          "serverMuted": false
        }
      ],
      "isMuted": true
    },
    {
      "id": "ABB33D04-3A2C-4D78-996F-9EEEF55EF119",
      "info": {
        "identity" : {
          "application" : {
            "displayName": "Test BOT",
            "id": "8A34A46B-3D17-4ADC-8DCE-DC4E7D572698"
          }
        },
        "region": "westus",
        "languageId": "en-US"
      },
      "mediaStreams": [
        {
          "sourceId": "3",
          "mediaType": "audio",
          "label": "main-audio",
          "direction": "sendReceive",
          "serverMuted": false
        }
      ],
      "isMuted": true
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List participants",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/call-list-participants.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
