---
title: Liste Trend
description: Berechnete Insight, der die Liste der Elemente, um den Benutzer Trend zurückgibt.
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 512dcdfb8a94a2a90c47c4005298537d1d83f137
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525108"
---
# <a name="list-trending"></a><span data-ttu-id="91e85-103">Liste Trend</span><span class="sxs-lookup"><span data-stu-id="91e85-103">List trending</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="91e85-104">Berechnete Insight, der die Liste der Elemente, um den Benutzer Trend zurückgibt.</span><span class="sxs-lookup"><span data-stu-id="91e85-104">Calculated insight that returns the list of items trending around the user.</span></span>

## <a name="permissions"></a><span data-ttu-id="91e85-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="91e85-105">Permissions</span></span>
<span data-ttu-id="91e85-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="91e85-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="91e85-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="91e85-108">Permission type</span></span>      | <span data-ttu-id="91e85-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="91e85-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="91e85-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="91e85-110">Delegated (work or school account)</span></span> | <span data-ttu-id="91e85-111">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91e85-111">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="91e85-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="91e85-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="91e85-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="91e85-113">Not supported.</span></span>    |
|<span data-ttu-id="91e85-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="91e85-114">Application</span></span> | <span data-ttu-id="91e85-115">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91e85-115">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="91e85-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="91e85-116">HTTP request</span></span>
```http
GET /me/insights/trending
GET /users/{id | userPrincipalName}/insights/trending
```

## <a name="optional-query-parameters"></a><span data-ttu-id="91e85-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="91e85-117">Optional query parameters</span></span>
<span data-ttu-id="91e85-118">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="91e85-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="91e85-119">Sie können die `$filter` Parameter zum Filtern von Trend Elemente Abfragen.</span><span class="sxs-lookup"><span data-stu-id="91e85-119">You can use the `$filter` query parameter to filter trending items.</span></span> <span data-ttu-id="91e85-120">Beispielsweise basierend auf:</span><span class="sxs-lookup"><span data-stu-id="91e85-120">For example, based on Type:</span></span>

`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/Type eq 'PowerPoint'`

<span data-ttu-id="91e85-121">Basierend auf Containertyp oder:</span><span class="sxs-lookup"><span data-stu-id="91e85-121">Or based on Container Type:</span></span>

`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`

<span data-ttu-id="91e85-122">Finden Sie die verfügbaren Containertypen und Typen, die Sie nach [ResourceVisualization](../resources/insights-resourcevisualization.md)filtern können.</span><span class="sxs-lookup"><span data-stu-id="91e85-122">See the available Container Types and Types you can filter by in [resourceVisualization](../resources/insights-resourcevisualization.md).</span></span>


## <a name="request-headers"></a><span data-ttu-id="91e85-123">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="91e85-123">Request headers</span></span>
| <span data-ttu-id="91e85-124">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="91e85-124">Header</span></span>       |  <span data-ttu-id="91e85-125">Wert</span><span class="sxs-lookup"><span data-stu-id="91e85-125">Value</span></span>|
|:-------------|:------|
| <span data-ttu-id="91e85-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="91e85-126">Authorization</span></span>  | <span data-ttu-id="91e85-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="91e85-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="91e85-129">Annehmen</span><span class="sxs-lookup"><span data-stu-id="91e85-129">Accept</span></span>  | <span data-ttu-id="91e85-130">application/json</span><span class="sxs-lookup"><span data-stu-id="91e85-130">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="91e85-131">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="91e85-131">Request body</span></span>
<span data-ttu-id="91e85-132">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="91e85-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="91e85-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="91e85-133">Response</span></span>

<span data-ttu-id="91e85-134">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Liste der Elemente im Antworttext [Trend](../resources/insights-trending.md) .</span><span class="sxs-lookup"><span data-stu-id="91e85-134">If successful, this method returns a `200 OK` response code and a list of [trending](../resources/insights-trending.md) items in the response body.</span></span> <span data-ttu-id="91e85-135">Jedes Element enthält Visualisierungseigenschaften für das Element in Ihre Erfahrung anzuzeigen.</span><span class="sxs-lookup"><span data-stu-id="91e85-135">Each item contains visualization properties for displaying the item in your experience.</span></span>

## <a name="example"></a><span data-ttu-id="91e85-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="91e85-136">Example</span></span>
#### <a name="request"></a><span data-ttu-id="91e85-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="91e85-137">Request</span></span>
<span data-ttu-id="91e85-138">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="91e85-138">Here is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/beta/me/insights/trending
```
#### <a name="response"></a><span data-ttu-id="91e85-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="91e85-139">Response</span></span>
<span data-ttu-id="91e85-140">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="91e85-140">Here is an example of the response.</span></span> <span data-ttu-id="91e85-141">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="91e85-141">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="91e85-142">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="91e85-142">All of the properties will be returned from an actual call.</span></span> <span data-ttu-id="91e85-143">Finden Sie eine Beispiel ohne abgeschnittene Antwort am unteren Rand der Seite.</span><span class="sxs-lookup"><span data-stu-id="91e85-143">See an example un-truncated response at the bottom of the page.</span></span>
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 801

{
    "value": [
        {
            "id": "id-value",
            "weight": "weight-value",
            "resourceVisualization": {
                "title": "title-value",
                "type": "type-value",
                "mediaType": "mediaType-value",
                "previewImageUrl": "previewImageUrl-value",
                "previewText": "previewText-value",
                "containerWebUrl": "containerWebUrl-value",
                "containerDisplayName": "containerDisplayName-value",
                "containerType": "containerType-value"
            },
            "resourceReference": {
                "webUrl": "webUrl-value",
                "id": "id-value",
                "type": "type-value"
            }
        }
    ]
}
```

### <a name="expanding-resource"></a><span data-ttu-id="91e85-144">Erweitern der Ressource</span><span class="sxs-lookup"><span data-stu-id="91e85-144">Expanding resource</span></span>
<span data-ttu-id="91e85-145">Die Ressource, die durch einen Trend Einblick kann erweitert werden.</span><span class="sxs-lookup"><span data-stu-id="91e85-145">The resource referenced by a trending insight can be expanded.</span></span>
```http
GET https://graph.microsoft.com/beta/me/insights/trending/{id}/resource
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/insights-list-trending.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
