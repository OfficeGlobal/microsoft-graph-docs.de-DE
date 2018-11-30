---
title: Liste Teilnehmer
description: Abrufen einer Liste der Teilnehmer-Objekte in den Anruf.
ms.openlocfilehash: a18dc609204712f1b7c7b31150975543277ffa67
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059962"
---
# <a name="list-participants"></a><span data-ttu-id="7b463-103">Liste Teilnehmer</span><span class="sxs-lookup"><span data-stu-id="7b463-103">List participants</span></span>

> <span data-ttu-id="7b463-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="7b463-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7b463-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7b463-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7b463-106">Abrufen einer Liste der Teilnehmer-Objekte in den Anruf.</span><span class="sxs-lookup"><span data-stu-id="7b463-106">Retrieve a list of participant objects in the call.</span></span>

## <a name="permissions"></a><span data-ttu-id="7b463-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="7b463-107">Permissions</span></span>
<span data-ttu-id="7b463-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7b463-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7b463-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7b463-110">Permission type</span></span> | <span data-ttu-id="7b463-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7b463-111">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="7b463-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7b463-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="7b463-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7b463-113">Not Supported</span></span>        |
| <span data-ttu-id="7b463-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7b463-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7b463-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7b463-115">Not Supported</span></span>        |
| <span data-ttu-id="7b463-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7b463-116">Application</span></span>     | <span data-ttu-id="7b463-117">Keines</span><span class="sxs-lookup"><span data-stu-id="7b463-117">None</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="7b463-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7b463-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /app/calls/{id}/participants
GET /applications/{id}/calls/{id}/participants
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7b463-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="7b463-119">Optional query parameters</span></span>
<span data-ttu-id="7b463-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="7b463-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7b463-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7b463-121">Request headers</span></span>
| <span data-ttu-id="7b463-122">Name</span><span class="sxs-lookup"><span data-stu-id="7b463-122">Name</span></span>          | <span data-ttu-id="7b463-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7b463-123">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="7b463-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="7b463-124">Authorization</span></span> | <span data-ttu-id="7b463-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="7b463-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7b463-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7b463-127">Request body</span></span>
<span data-ttu-id="7b463-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="7b463-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7b463-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="7b463-129">Response</span></span>
<span data-ttu-id="7b463-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und Auflistung von Objekten im Antworttext [Teilnehmer](../resources/participant.md) .</span><span class="sxs-lookup"><span data-stu-id="7b463-130">If successful, this method returns a `200 OK` response code and collection of [participant](../resources/participant.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7b463-131">Beispiele</span><span class="sxs-lookup"><span data-stu-id="7b463-131">Examples</span></span>

### <a name="example-1"></a><span data-ttu-id="7b463-132">Beispiel 1</span><span class="sxs-lookup"><span data-stu-id="7b463-132">Example 1</span></span>

##### <a name="request"></a><span data-ttu-id="7b463-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7b463-133">Request</span></span>
<span data-ttu-id="7b463-134">Das folgende Beispiel zeigt die Antwort.</span><span class="sxs-lookup"><span data-stu-id="7b463-134">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_participants"
}-->
```http
GET https://graph.microsoft.com/beta/app/calls/{id}/participants
```

##### <a name="response"></a><span data-ttu-id="7b463-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="7b463-135">Response</span></span>

> <span data-ttu-id="7b463-p104">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="7b463-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2"></a><span data-ttu-id="7b463-138">Beispiel 2</span><span class="sxs-lookup"><span data-stu-id="7b463-138">Example 2</span></span>

##### <a name="request"></a><span data-ttu-id="7b463-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7b463-139">Request</span></span>

```http
GET /app/calls/57DAB8B1894C409AB240BD8BEAE78896/participants
Authorization: Bearer <TOKEN>
```

##### <a name="response"></a><span data-ttu-id="7b463-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="7b463-140">Response</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "List participants",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
