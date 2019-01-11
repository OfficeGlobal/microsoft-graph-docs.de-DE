---
title: 'ChartPointsCollection: ItemAt'
description: Dient zum Abrufen eines Punkts anhand seiner Position in der Datenreihe.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: c497f0f15b3d1ddcdb3e5adb05d9e9d0b1ade57e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27829015"
---
# <a name="chartpointscollection-itemat"></a><span data-ttu-id="c1cfa-103">ChartPointsCollection: ItemAt</span><span class="sxs-lookup"><span data-stu-id="c1cfa-103">ChartPointsCollection: ItemAt</span></span>

> <span data-ttu-id="c1cfa-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="c1cfa-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c1cfa-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c1cfa-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c1cfa-106">Dient zum Abrufen eines Punkts anhand seiner Position in der Datenreihe.</span><span class="sxs-lookup"><span data-stu-id="c1cfa-106">Retrieve a point based on its position within the series.</span></span>
## <a name="permissions"></a><span data-ttu-id="c1cfa-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="c1cfa-107">Permissions</span></span>
<span data-ttu-id="c1cfa-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c1cfa-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c1cfa-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c1cfa-110">Permission type</span></span>      | <span data-ttu-id="c1cfa-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c1cfa-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c1cfa-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c1cfa-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c1cfa-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c1cfa-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c1cfa-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c1cfa-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c1cfa-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c1cfa-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c1cfa-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c1cfa-116">Application</span></span> | <span data-ttu-id="c1cfa-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c1cfa-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c1cfa-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c1cfa-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts(<name>)/series(<undefined>)/points/ItemAt

```
## <a name="request-headers"></a><span data-ttu-id="c1cfa-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c1cfa-119">Request headers</span></span>
| <span data-ttu-id="c1cfa-120">Name</span><span class="sxs-lookup"><span data-stu-id="c1cfa-120">Name</span></span>       | <span data-ttu-id="c1cfa-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c1cfa-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c1cfa-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c1cfa-122">Authorization</span></span>  | <span data-ttu-id="c1cfa-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c1cfa-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c1cfa-125">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="c1cfa-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="c1cfa-p104">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="c1cfa-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c1cfa-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c1cfa-128">Request body</span></span>
<span data-ttu-id="c1cfa-129">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="c1cfa-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c1cfa-130">Parameter</span><span class="sxs-lookup"><span data-stu-id="c1cfa-130">Parameter</span></span>    | <span data-ttu-id="c1cfa-131">Typ</span><span class="sxs-lookup"><span data-stu-id="c1cfa-131">Type</span></span>   |<span data-ttu-id="c1cfa-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c1cfa-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c1cfa-133">Index</span><span class="sxs-lookup"><span data-stu-id="c1cfa-133">index</span></span>|<span data-ttu-id="c1cfa-134">number</span><span class="sxs-lookup"><span data-stu-id="c1cfa-134">number</span></span>|<span data-ttu-id="c1cfa-p105">Index-Wert des abzurufenden Objekts. Nullindiziert.</span><span class="sxs-lookup"><span data-stu-id="c1cfa-p105">Index value of the object to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="c1cfa-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="c1cfa-137">Response</span></span>

<span data-ttu-id="c1cfa-138">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [ChartPoint](../resources/chartpoint.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c1cfa-138">If successful, this method returns `200 OK` response code and [ChartPoint](../resources/chartpoint.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c1cfa-139">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c1cfa-139">Example</span></span>
<span data-ttu-id="c1cfa-140">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="c1cfa-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c1cfa-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c1cfa-141">Request</span></span>
<span data-ttu-id="c1cfa-142">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c1cfa-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chartpointscollection_itemat"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/series(<undefined>)/points/ItemAt
Content-type: application/json
Content-length: 20

{
  "index": {
  }
}
```

##### <a name="response"></a><span data-ttu-id="c1cfa-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="c1cfa-143">Response</span></span>
<span data-ttu-id="c1cfa-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c1cfa-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartPoint"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 20

{
  "value": {
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartPointsCollection: ItemAt",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
