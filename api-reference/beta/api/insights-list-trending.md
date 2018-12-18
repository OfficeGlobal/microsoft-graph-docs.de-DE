---
title: Liste Trend
description: Berechnete Insight, der die Liste der Elemente, um den Benutzer Trend zurückgibt.
author: simonhult
ms.openlocfilehash: de169f9960a1694e452b8dcfd16aafde89d3ac29
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27343414"
---
# <a name="list-trending"></a><span data-ttu-id="51af4-103">Liste Trend</span><span class="sxs-lookup"><span data-stu-id="51af4-103">List trending</span></span>

> <span data-ttu-id="51af4-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="51af4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="51af4-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="51af4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="51af4-106">Berechnete Insight, der die Liste der Elemente, um den Benutzer Trend zurückgibt.</span><span class="sxs-lookup"><span data-stu-id="51af4-106">Calculated insight that returns the list of items trending around the user.</span></span>

## <a name="permissions"></a><span data-ttu-id="51af4-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="51af4-107">Permissions</span></span>
<span data-ttu-id="51af4-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="51af4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="51af4-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="51af4-110">Permission type</span></span>      | <span data-ttu-id="51af4-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="51af4-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="51af4-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="51af4-112">Delegated (work or school account)</span></span> | <span data-ttu-id="51af4-113">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51af4-113">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="51af4-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="51af4-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="51af4-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="51af4-115">Not supported.</span></span>    |
|<span data-ttu-id="51af4-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="51af4-116">Application</span></span> | <span data-ttu-id="51af4-117">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51af4-117">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="51af4-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="51af4-118">HTTP request</span></span>
```http
GET /me/insights/trending
GET /users/{id | userPrincipalName}/insights/trending
```

## <a name="optional-query-parameters"></a><span data-ttu-id="51af4-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="51af4-119">Optional query parameters</span></span>
<span data-ttu-id="51af4-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="51af4-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="51af4-121">Sie können die `$filter` Parameter zum Filtern von Trend Elemente Abfragen.</span><span class="sxs-lookup"><span data-stu-id="51af4-121">You can use the `$filter` query parameter to filter trending items.</span></span> <span data-ttu-id="51af4-122">Beispielsweise basierend auf:</span><span class="sxs-lookup"><span data-stu-id="51af4-122">For example, based on Type:</span></span>

`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/Type eq 'PowerPoint'`

<span data-ttu-id="51af4-123">Basierend auf Containertyp oder:</span><span class="sxs-lookup"><span data-stu-id="51af4-123">Or based on Container Type:</span></span>

`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`

<span data-ttu-id="51af4-124">Finden Sie die verfügbaren Containertypen und Typen, die Sie nach [ResourceVisualization](../resources/insights-resourcevisualization.md)filtern können.</span><span class="sxs-lookup"><span data-stu-id="51af4-124">See the available Container Types and Types you can filter by in [resourceVisualization](../resources/insights-resourcevisualization.md).</span></span>


## <a name="request-headers"></a><span data-ttu-id="51af4-125">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="51af4-125">Request headers</span></span>
| <span data-ttu-id="51af4-126">Header</span><span class="sxs-lookup"><span data-stu-id="51af4-126">Header</span></span>       |  <span data-ttu-id="51af4-127">Wert</span><span class="sxs-lookup"><span data-stu-id="51af4-127">Value</span></span>|
|:-------------|:------|
| <span data-ttu-id="51af4-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="51af4-128">Authorization</span></span>  | <span data-ttu-id="51af4-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="51af4-p104">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="51af4-131">Accept</span><span class="sxs-lookup"><span data-stu-id="51af4-131">Accept</span></span>  | <span data-ttu-id="51af4-132">application/json</span><span class="sxs-lookup"><span data-stu-id="51af4-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="51af4-133">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="51af4-133">Request body</span></span>
<span data-ttu-id="51af4-134">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="51af4-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="51af4-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="51af4-135">Response</span></span>

<span data-ttu-id="51af4-136">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Liste der Elemente im Antworttext [Trend](../resources/insights-trending.md) .</span><span class="sxs-lookup"><span data-stu-id="51af4-136">If successful, this method returns a `200 OK` response code and a list of [trending](../resources/insights-trending.md) items in the response body.</span></span> <span data-ttu-id="51af4-137">Jedes Element enthält Visualisierungseigenschaften für das Element in Ihre Erfahrung anzuzeigen.</span><span class="sxs-lookup"><span data-stu-id="51af4-137">Each item contains visualization properties for displaying the item in your experience.</span></span>

## <a name="example"></a><span data-ttu-id="51af4-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="51af4-138">Example</span></span>
#### <a name="request"></a><span data-ttu-id="51af4-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="51af4-139">Request</span></span>
<span data-ttu-id="51af4-140">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="51af4-140">Here is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/beta/me/insights/trending
```
#### <a name="response"></a><span data-ttu-id="51af4-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="51af4-141">Response</span></span>
<span data-ttu-id="51af4-142">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="51af4-142">Here is an example of the response.</span></span> <span data-ttu-id="51af4-143">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="51af4-143">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="51af4-144">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="51af4-144">All of the properties will be returned from an actual call.</span></span> <span data-ttu-id="51af4-145">Finden Sie eine Beispiel ohne abgeschnittene Antwort am unteren Rand der Seite.</span><span class="sxs-lookup"><span data-stu-id="51af4-145">See an example un-truncated response at the bottom of the page.</span></span>
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

### <a name="expanding-resource"></a><span data-ttu-id="51af4-146">Erweitern der Ressource</span><span class="sxs-lookup"><span data-stu-id="51af4-146">Expanding resource</span></span>
<span data-ttu-id="51af4-147">Die Ressource, die durch einen Trend Einblick kann erweitert werden.</span><span class="sxs-lookup"><span data-stu-id="51af4-147">The resource referenced by a trending insight can be expanded.</span></span>
```http
GET https://graph.microsoft.com/beta/me/insights/trending/{id}/resource
```
