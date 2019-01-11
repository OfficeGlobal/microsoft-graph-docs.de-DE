---
title: Liste trendingAround
description: Berechnete Insight, der die Liste der Elemente, um einen Benutzer Trend zurückgibt.
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: 1fca9fe47d1656b8b499fbf2e1f3fa1ee638f37e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27839459"
---
# <a name="list-trendingaround"></a><span data-ttu-id="17db5-103">Liste trendingAround</span><span class="sxs-lookup"><span data-stu-id="17db5-103">List trendingAround</span></span>

> <span data-ttu-id="17db5-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="17db5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="17db5-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="17db5-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="17db5-106">Berechnete Insight, der die Liste der Elemente, um einen Benutzer Trend zurückgibt.</span><span class="sxs-lookup"><span data-stu-id="17db5-106">Calculated insight that returns the list of items trending around a user.</span></span>

<span data-ttu-id="17db5-107">**Hinweis:** Diese API wird als veraltet markiert und durch die [Trend-API](../resources/insights-trending.md)ersetzt werden.</span><span class="sxs-lookup"><span data-stu-id="17db5-107">**Note:** This API will be deprecated and replaced by the [Trending API](../resources/insights-trending.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="17db5-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="17db5-108">Permissions</span></span>
<span data-ttu-id="17db5-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="17db5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="17db5-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="17db5-111">Permission type</span></span>      | <span data-ttu-id="17db5-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="17db5-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="17db5-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="17db5-113">Delegated (work or school account)</span></span> | <span data-ttu-id="17db5-114">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="17db5-114">Sites.Read.All</span></span>    |
|<span data-ttu-id="17db5-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="17db5-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="17db5-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="17db5-116">Not supported.</span></span>    |
|<span data-ttu-id="17db5-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="17db5-117">Application</span></span> | <span data-ttu-id="17db5-118">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="17db5-118">Sites.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="17db5-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="17db5-119">HTTP request</span></span>
```http
GET /me/trendingAround
GET /users/{id | userPrincipalName}/trendingAround
GET /drive/root/createdByUser/trendingAround
GET /drive/root/lastModifiedByUser/trendingAround
```
## <a name="optional-query-parameters"></a><span data-ttu-id="17db5-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="17db5-120">Optional query parameters</span></span>
<span data-ttu-id="17db5-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="17db5-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="17db5-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="17db5-122">Request headers</span></span>
| <span data-ttu-id="17db5-123">Header</span><span class="sxs-lookup"><span data-stu-id="17db5-123">Header</span></span>         | <span data-ttu-id="17db5-124">Wert</span><span class="sxs-lookup"><span data-stu-id="17db5-124">Value</span></span>                      |
|:---------------|:---------------------------|
| <span data-ttu-id="17db5-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="17db5-125">Authorization</span></span>  | <span data-ttu-id="17db5-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="17db5-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="17db5-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="17db5-128">Content-Type</span></span>   | <span data-ttu-id="17db5-129">application/json</span><span class="sxs-lookup"><span data-stu-id="17db5-129">application/json</span></span>           |

## <a name="request-body"></a><span data-ttu-id="17db5-130">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="17db5-130">Request body</span></span>
<span data-ttu-id="17db5-131">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="17db5-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="17db5-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="17db5-132">Response</span></span>

<span data-ttu-id="17db5-133">Wenn erfolgreich, gibt diese Methode einen 200 OK-Antwortcode und eine Auflistung von [DriveItem](../resources/driveitem.md) -Objekten im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="17db5-133">If successful, this method returns a 200 OK response code and collection of [driveItem](../resources/driveitem.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="17db5-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="17db5-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="17db5-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="17db5-135">Request</span></span>
```http
GET https://graph.microsoft.com/beta/me/trendingAround
```
##### <a name="response"></a><span data-ttu-id="17db5-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="17db5-136">Response</span></span>
<span data-ttu-id="17db5-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="17db5-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
