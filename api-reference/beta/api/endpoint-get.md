---
title: Get-Endpunkt
description: Rufen Sie die Eigenschaften und die Beziehungen eines bestimmten Endpunkt-Objekts ab.
localization_priority: Normal
ms.openlocfilehash: 77ad5716e8e30a16f95bf62593a6530d5e759861
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27820447"
---
# <a name="get-endpoint"></a><span data-ttu-id="2b084-103">Get-Endpunkt</span><span class="sxs-lookup"><span data-stu-id="2b084-103">Get endpoint</span></span>

> <span data-ttu-id="2b084-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="2b084-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2b084-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2b084-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2b084-106">Rufen Sie die Eigenschaften und die Beziehungen eines bestimmten [Endpunkt](../resources/endpoint.md) -Objekts ab.</span><span class="sxs-lookup"><span data-stu-id="2b084-106">Retrieve the properties and relationships of a specific [endpoint](../resources/endpoint.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="2b084-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="2b084-107">Permissions</span></span>
<span data-ttu-id="2b084-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2b084-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="2b084-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2b084-110">Permission type</span></span>      | <span data-ttu-id="2b084-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2b084-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2b084-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2b084-112">Delegated (work or school account)</span></span> | <span data-ttu-id="2b084-113">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b084-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="2b084-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2b084-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2b084-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2b084-115">Not supported.</span></span>    |
|<span data-ttu-id="2b084-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2b084-116">Application</span></span> | <span data-ttu-id="2b084-117">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b084-117">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2b084-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2b084-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/endpoints/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="2b084-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="2b084-119">Optional query parameters</span></span>
<span data-ttu-id="2b084-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="2b084-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2b084-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2b084-121">Request headers</span></span>
| <span data-ttu-id="2b084-122">Name</span><span class="sxs-lookup"><span data-stu-id="2b084-122">Name</span></span>      |<span data-ttu-id="2b084-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2b084-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="2b084-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="2b084-124">Authorization</span></span>  | <span data-ttu-id="2b084-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="2b084-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="2b084-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2b084-127">Content-Type</span></span>   | <span data-ttu-id="2b084-128">Application/Json</span><span class="sxs-lookup"><span data-stu-id="2b084-128">Application/Json</span></span> |

## <a name="request-body"></a><span data-ttu-id="2b084-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2b084-129">Request body</span></span>
<span data-ttu-id="2b084-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="2b084-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2b084-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="2b084-131">Response</span></span>

<span data-ttu-id="2b084-132">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und [Endpunkt](../resources/endpoint.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="2b084-132">If successful, this method returns a `200 OK` response code and [Endpoint](../resources/endpoint.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2b084-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2b084-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2b084-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2b084-134">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_endpoint"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/endpoints/{id}
```
##### <a name="response"></a><span data-ttu-id="2b084-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="2b084-135">Response</span></span>
<span data-ttu-id="2b084-p104">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2b084-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.Endpoint"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 208

{
  "capability": "Conversations",
  "providerId": "{Yammer GUID}",
  "providerName": "Yammer",
  "uri": "uri-value",
  "providerResourceId": "Yammer.FeedURL",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get Endpoint",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
