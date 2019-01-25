---
title: Diagramm erstellen
description: Verwenden Sie diese API zum Erstellen eines neuen Diagramms.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 27bd441e6002d69cf94f79b8e3de40f9614ad6a6
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522770"
---
# <a name="create-chart"></a><span data-ttu-id="2f974-103">Diagramm erstellen</span><span class="sxs-lookup"><span data-stu-id="2f974-103">Create Chart</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2f974-104">Verwenden Sie diese API zum Erstellen eines neuen Diagramms.</span><span class="sxs-lookup"><span data-stu-id="2f974-104">Use this API to create a new Chart.</span></span>
## <a name="permissions"></a><span data-ttu-id="2f974-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="2f974-105">Permissions</span></span>
<span data-ttu-id="2f974-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2f974-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2f974-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2f974-108">Permission type</span></span>      | <span data-ttu-id="2f974-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2f974-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2f974-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2f974-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2f974-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2f974-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="2f974-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2f974-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2f974-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2f974-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="2f974-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2f974-114">Application</span></span> | <span data-ttu-id="2f974-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2f974-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2f974-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2f974-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/

```
## <a name="request-headers"></a><span data-ttu-id="2f974-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2f974-117">Request headers</span></span>
| <span data-ttu-id="2f974-118">Name</span><span class="sxs-lookup"><span data-stu-id="2f974-118">Name</span></span>       | <span data-ttu-id="2f974-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2f974-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="2f974-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="2f974-120">Authorization</span></span>  | <span data-ttu-id="2f974-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="2f974-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2f974-123">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="2f974-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="2f974-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="2f974-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2f974-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2f974-126">Request body</span></span>
<span data-ttu-id="2f974-127">Geben Sie im Anforderungstext eine JSON-Darstellung des [Chart](../resources/chart.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="2f974-127">In the request body, supply a JSON representation of [Chart](../resources/chart.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="2f974-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="2f974-128">Response</span></span>

<span data-ttu-id="2f974-129">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und das [Chart](../resources/chart.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2f974-129">If successful, this method returns `201 Created` response code and [Chart](../resources/chart.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f974-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2f974-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2f974-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2f974-131">Request</span></span>
<span data-ttu-id="2f974-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2f974-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_chart_from_worksheet"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts
Content-type: application/json
Content-length: 52

{
  "id": "id-value",
  "height": 99,
  "left": 99
}
```
<span data-ttu-id="2f974-133">Geben Sie im Anforderungstext eine JSON-Darstellung des [Chart](../resources/chart.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="2f974-133">In the request body, supply a JSON representation of [Chart](../resources/chart.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="2f974-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="2f974-134">Response</span></span>
<span data-ttu-id="2f974-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2f974-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chart"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 52

{
  "id": "id-value",
  "height": 99,
  "left": 99
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create Chart",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/worksheet-post-charts.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
