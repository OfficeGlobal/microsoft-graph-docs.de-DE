---
title: Liste trendingAround
description: Berechnete Insight, der die Liste der Elemente, um einen Benutzer Trend zurückgibt.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 625ae9d66ce1b891ebdba3209d92bd0e88b06a94
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29507628"
---
# <a name="list-trendingaround"></a><span data-ttu-id="10b02-103">Liste trendingAround</span><span class="sxs-lookup"><span data-stu-id="10b02-103">List trendingAround</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="10b02-104">Berechnete Insight, der die Liste der Elemente, um einen Benutzer Trend zurückgibt.</span><span class="sxs-lookup"><span data-stu-id="10b02-104">Calculated insight that returns the list of items trending around a user.</span></span>

<span data-ttu-id="10b02-105">**Hinweis:** Diese API wird als veraltet markiert und durch die [Trend-API](../resources/insights-trending.md)ersetzt werden.</span><span class="sxs-lookup"><span data-stu-id="10b02-105">**Note:** This API will be deprecated and replaced by the [Trending API](../resources/insights-trending.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="10b02-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="10b02-106">Permissions</span></span>
<span data-ttu-id="10b02-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="10b02-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="10b02-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="10b02-109">Permission type</span></span>      | <span data-ttu-id="10b02-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="10b02-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="10b02-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="10b02-111">Delegated (work or school account)</span></span> | <span data-ttu-id="10b02-112">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="10b02-112">Sites.Read.All</span></span>    |
|<span data-ttu-id="10b02-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="10b02-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="10b02-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="10b02-114">Not supported.</span></span>    |
|<span data-ttu-id="10b02-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="10b02-115">Application</span></span> | <span data-ttu-id="10b02-116">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="10b02-116">Sites.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="10b02-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="10b02-117">HTTP request</span></span>
```http
GET /me/trendingAround
GET /users/{id | userPrincipalName}/trendingAround
GET /drive/root/createdByUser/trendingAround
GET /drive/root/lastModifiedByUser/trendingAround
```
## <a name="optional-query-parameters"></a><span data-ttu-id="10b02-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="10b02-118">Optional query parameters</span></span>
<span data-ttu-id="10b02-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="10b02-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="10b02-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="10b02-120">Request headers</span></span>
| <span data-ttu-id="10b02-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="10b02-121">Header</span></span>         | <span data-ttu-id="10b02-122">Wert</span><span class="sxs-lookup"><span data-stu-id="10b02-122">Value</span></span>                      |
|:---------------|:---------------------------|
| <span data-ttu-id="10b02-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="10b02-123">Authorization</span></span>  | <span data-ttu-id="10b02-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="10b02-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="10b02-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="10b02-126">Content-Type</span></span>   | <span data-ttu-id="10b02-127">application/json</span><span class="sxs-lookup"><span data-stu-id="10b02-127">application/json</span></span>           |

## <a name="request-body"></a><span data-ttu-id="10b02-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="10b02-128">Request body</span></span>
<span data-ttu-id="10b02-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="10b02-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="10b02-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="10b02-130">Response</span></span>

<span data-ttu-id="10b02-131">Wenn erfolgreich, gibt diese Methode einen 200 OK-Antwortcode und eine Auflistung von [DriveItem](../resources/driveitem.md) -Objekten im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="10b02-131">If successful, this method returns a 200 OK response code and collection of [driveItem](../resources/driveitem.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="10b02-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="10b02-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="10b02-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="10b02-133">Request</span></span>
```http
GET https://graph.microsoft.com/beta/me/trendingAround
```
##### <a name="response"></a><span data-ttu-id="10b02-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="10b02-134">Response</span></span>
<span data-ttu-id="10b02-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="10b02-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 226

{
  "id": "id-value",
  "name": "name-value",
  "DateTimeCreated": "DateTimeCreated-value",
  "DateTimeLastModified": "DateTimeLastModified-value",
  "webUrl": "webUrl-value",
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/user-list-trendingaround.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
