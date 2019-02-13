---
title: Teilnehmer auflisten
description: Abrufen einer Liste der Teilnehmer-Objekte in den Anruf.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: bc38af4a6bee4a380a001310303d67efb2705dcf
ms.sourcegitcommit: bdbc68ed8eaf43386d2cdf7b79e64ebbe1e860c0
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/13/2019
ms.locfileid: "29967347"
---
# <a name="list-participants"></a><span data-ttu-id="8caa9-103">Teilnehmer auflisten</span><span class="sxs-lookup"><span data-stu-id="8caa9-103">List participants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8caa9-104">Abrufen einer Liste der Teilnehmer-Objekte in den Anruf.</span><span class="sxs-lookup"><span data-stu-id="8caa9-104">Retrieve a list of participant objects in the call.</span></span>

## <a name="permissions"></a><span data-ttu-id="8caa9-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="8caa9-105">Permissions</span></span>

<span data-ttu-id="8caa9-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8caa9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8caa9-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8caa9-108">Permission type</span></span> | <span data-ttu-id="8caa9-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8caa9-109">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="8caa9-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8caa9-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="8caa9-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8caa9-111">Not Supported</span></span>        |
| <span data-ttu-id="8caa9-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8caa9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8caa9-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8caa9-113">Not Supported</span></span>        |
| <span data-ttu-id="8caa9-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8caa9-114">Application</span></span>     | <span data-ttu-id="8caa9-115">Keine</span><span class="sxs-lookup"><span data-stu-id="8caa9-115">None</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="8caa9-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8caa9-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /app/calls/{id}/participants
GET /applications/{id}/calls/{id}/participants
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8caa9-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="8caa9-117">Optional query parameters</span></span>

<span data-ttu-id="8caa9-118">Diese Methode unterstützt die [OData-Abfrage-Parameter](/graph/query-parameters) , mit denen die Antwort anpassen.</span><span class="sxs-lookup"><span data-stu-id="8caa9-118">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8caa9-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8caa9-119">Request headers</span></span>

| <span data-ttu-id="8caa9-120">Name</span><span class="sxs-lookup"><span data-stu-id="8caa9-120">Name</span></span>          | <span data-ttu-id="8caa9-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8caa9-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="8caa9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8caa9-122">Authorization</span></span> | <span data-ttu-id="8caa9-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8caa9-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8caa9-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8caa9-125">Request body</span></span>

<span data-ttu-id="8caa9-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="8caa9-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8caa9-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="8caa9-127">Response</span></span>

<span data-ttu-id="8caa9-128">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und Auflistung von Objekten im Antworttext [Teilnehmer](../resources/participant.md) .</span><span class="sxs-lookup"><span data-stu-id="8caa9-128">If successful, this method returns a `200 OK` response code and collection of [participant](../resources/participant.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8caa9-129">Beispiele</span><span class="sxs-lookup"><span data-stu-id="8caa9-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8caa9-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8caa9-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get-participants"
}-->

```http
GET https://graph.microsoft.com/beta/app/calls/57DAB8B1894C409AB240BD8BEAE78896/participants
Authorization: Bearer <TOKEN>
```

<!-- markdownlint-disable MD024 -->

### <a name="response"></a><span data-ttu-id="8caa9-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="8caa9-131">Response</span></span>

> <span data-ttu-id="8caa9-p103">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="8caa9-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
