---
title: 'ChartSeriesCollection: ItemAt'
description: Ruft eine Datenreihe anhand ihrer Position in der Sammlung ab.
author: lumine2008
ms.openlocfilehash: e1027919034688fd90380497a42b77707fa1de72
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27316436"
---
# <a name="chartseriescollection-itemat"></a><span data-ttu-id="ca214-103">ChartSeriesCollection: ItemAt</span><span class="sxs-lookup"><span data-stu-id="ca214-103">ChartSeriesCollection: ItemAt</span></span>

> <span data-ttu-id="ca214-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="ca214-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ca214-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ca214-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ca214-106">Ruft eine Datenreihe anhand ihrer Position in der Sammlung ab.</span><span class="sxs-lookup"><span data-stu-id="ca214-106">Retrieves a series based on its position in the collection</span></span>
## <a name="permissions"></a><span data-ttu-id="ca214-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="ca214-107">Permissions</span></span>
<span data-ttu-id="ca214-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ca214-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ca214-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ca214-110">Permission type</span></span>      | <span data-ttu-id="ca214-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ca214-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ca214-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ca214-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ca214-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ca214-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ca214-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ca214-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ca214-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ca214-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ca214-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ca214-116">Application</span></span> | <span data-ttu-id="ca214-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ca214-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ca214-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ca214-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts(<name>)/series/ItemAt

```
## <a name="request-headers"></a><span data-ttu-id="ca214-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ca214-119">Request headers</span></span>
| <span data-ttu-id="ca214-120">Name</span><span class="sxs-lookup"><span data-stu-id="ca214-120">Name</span></span>       | <span data-ttu-id="ca214-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ca214-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ca214-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ca214-122">Authorization</span></span>  | <span data-ttu-id="ca214-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ca214-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ca214-125">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="ca214-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="ca214-p104">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="ca214-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ca214-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ca214-128">Request body</span></span>
<span data-ttu-id="ca214-129">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="ca214-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="ca214-130">Parameter</span><span class="sxs-lookup"><span data-stu-id="ca214-130">Parameter</span></span>    | <span data-ttu-id="ca214-131">Typ</span><span class="sxs-lookup"><span data-stu-id="ca214-131">Type</span></span>   |<span data-ttu-id="ca214-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ca214-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ca214-133">Index</span><span class="sxs-lookup"><span data-stu-id="ca214-133">index</span></span>|<span data-ttu-id="ca214-134">number</span><span class="sxs-lookup"><span data-stu-id="ca214-134">number</span></span>|<span data-ttu-id="ca214-p105">Index-Wert des abzurufenden Objekts. Nullindiziert.</span><span class="sxs-lookup"><span data-stu-id="ca214-p105">Index value of the object to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="ca214-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="ca214-137">Response</span></span>

<span data-ttu-id="ca214-138">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [ChartSeries](../resources/chartseries.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ca214-138">If successful, this method returns `200 OK` response code and [ChartSeries](../resources/chartseries.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ca214-139">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ca214-139">Example</span></span>
<span data-ttu-id="ca214-140">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="ca214-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="ca214-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ca214-141">Request</span></span>
<span data-ttu-id="ca214-142">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ca214-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chartseriescollection_itemat"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/series/ItemAt
Content-type: application/json
Content-length: 20

{
  "index": {
  }
}
```

##### <a name="response"></a><span data-ttu-id="ca214-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="ca214-143">Response</span></span>
<span data-ttu-id="ca214-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ca214-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartSeries"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 26

{
  "name": "name-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartSeriesCollection: ItemAt",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->