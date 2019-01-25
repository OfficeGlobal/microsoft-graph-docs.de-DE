---
title: Endpunkte auflisten
description: Abrufen einer Liste der Endpoint-Objekte.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: d8bb01d00fbac03a2b52d95179ec22ca769f9df2
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529831"
---
# <a name="list-endpoints"></a><span data-ttu-id="d0574-103">Endpunkte auflisten</span><span class="sxs-lookup"><span data-stu-id="d0574-103">List endpoints</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d0574-104">Abrufen einer Liste der [Endpoint](../resources/endpoint.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="d0574-104">Retrieve a list of [endpoint](../resources/endpoint.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="d0574-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="d0574-105">Permissions</span></span>
<span data-ttu-id="d0574-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d0574-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d0574-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d0574-108">Permission type</span></span>      | <span data-ttu-id="d0574-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d0574-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d0574-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d0574-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d0574-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0574-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="d0574-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d0574-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d0574-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d0574-113">Not supported.</span></span>    |
|<span data-ttu-id="d0574-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d0574-114">Application</span></span> | <span data-ttu-id="d0574-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0574-115">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d0574-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d0574-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/endpoints
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d0574-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="d0574-117">Optional query parameters</span></span>
<span data-ttu-id="d0574-118">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="d0574-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d0574-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d0574-119">Request headers</span></span>
| <span data-ttu-id="d0574-120">Name</span><span class="sxs-lookup"><span data-stu-id="d0574-120">Name</span></span>      |<span data-ttu-id="d0574-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d0574-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d0574-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d0574-122">Authorization</span></span>  | <span data-ttu-id="d0574-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d0574-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="d0574-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d0574-125">Content-Type</span></span>   | <span data-ttu-id="d0574-126">Application/Json</span><span class="sxs-lookup"><span data-stu-id="d0574-126">Application/Json</span></span> |

## <a name="request-body"></a><span data-ttu-id="d0574-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d0574-127">Request body</span></span>
<span data-ttu-id="d0574-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="d0574-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d0574-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="d0574-129">Response</span></span>

<span data-ttu-id="d0574-130">Wenn der Vorgang erfolgreich war, gibt diese Methode eine `200 OK` Antwortcode und Auflistung von [Endpoint](../resources/endpoint.md) -Objekte im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="d0574-130">If successful, this method returns a `200 OK` response code and collection of [Endpoint](../resources/endpoint.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d0574-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d0574-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d0574-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d0574-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_endpoints"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/endpoints
```
##### <a name="response"></a><span data-ttu-id="d0574-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="d0574-133">Response</span></span>
<span data-ttu-id="d0574-p103">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d0574-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.Endpoint",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 261

{
  "value": [
    {
      "capability": "Conversations",
      "providerId": "{Yammer GUID}",
      "providerName": "Yammer",
      "uri": "uri-value",
      "providerResourceId": "Yammer.FeedURL",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List endpoints",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/group-list-endpoints.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
