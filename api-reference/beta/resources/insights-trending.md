---
title: Trend Ressourcentyp
description: Rich-Beziehung Herstellen einer Verbindung mit einem Benutzer Dokumente, die auf den Benutzer (für den Benutzer relevant sind) Trend sind. OneDrive-Dateien, und um die Benutzer können Dateien, die auf SharePoint-Teamwebsites trend.
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 587b52107f3a7f9892603afb8273ce55b6faa549
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29577410"
---
# <a name="trending-resource-type"></a><span data-ttu-id="8fb0a-104">Trend Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="8fb0a-104">trending resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8fb0a-105">Rich-Beziehung Herstellen einer Verbindung mit einem Benutzer Dokumente, die auf den Benutzer (für den Benutzer relevant sind) Trend sind.</span><span class="sxs-lookup"><span data-stu-id="8fb0a-105">Rich relationship connecting a user to documents that are trending around the user (are relevant to the user).</span></span> <span data-ttu-id="8fb0a-106">OneDrive-Dateien, und um die Benutzer können Dateien, die auf SharePoint-Teamwebsites trend.</span><span class="sxs-lookup"><span data-stu-id="8fb0a-106">OneDrive files, and files stored on SharePoint team sites can trend around the user.</span></span>

## <a name="methods"></a><span data-ttu-id="8fb0a-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="8fb0a-107">Methods</span></span>

| <span data-ttu-id="8fb0a-108">Methode</span><span class="sxs-lookup"><span data-stu-id="8fb0a-108">Method</span></span>       | <span data-ttu-id="8fb0a-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="8fb0a-109">Return Type</span></span>  |<span data-ttu-id="8fb0a-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8fb0a-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8fb0a-111">Liste Trend</span><span class="sxs-lookup"><span data-stu-id="8fb0a-111">List trending</span></span>](../api/insights-list-trending.md) |<span data-ttu-id="8fb0a-112">[Insights_trending](insights-trending.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="8fb0a-112">[insights_trending](insights-trending.md) collection</span></span>| <span data-ttu-id="8fb0a-113">Abrufen einer Liste von Trend-Dateien.</span><span class="sxs-lookup"><span data-stu-id="8fb0a-113">Get a list of trending files.</span></span>|

## <a name="properties"></a><span data-ttu-id="8fb0a-114">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="8fb0a-114">Properties</span></span>

| <span data-ttu-id="8fb0a-115">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8fb0a-115">Property</span></span>      | <span data-ttu-id="8fb0a-116">Typ</span><span class="sxs-lookup"><span data-stu-id="8fb0a-116">Type</span></span>                              | <span data-ttu-id="8fb0a-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8fb0a-117">Description</span></span>  |
| ------------- |---------------                    | -------------|
| <span data-ttu-id="8fb0a-118">id</span><span class="sxs-lookup"><span data-stu-id="8fb0a-118">id</span></span>                    | <span data-ttu-id="8fb0a-119">String</span><span class="sxs-lookup"><span data-stu-id="8fb0a-119">String</span></span>                    | <span data-ttu-id="8fb0a-120">Eindeutiger Bezeichner der Beziehung.</span><span class="sxs-lookup"><span data-stu-id="8fb0a-120">Unique identifier of the relationship.</span></span> <span data-ttu-id="8fb0a-121">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="8fb0a-121">Read only.</span></span>        |
| <span data-ttu-id="8fb0a-122">weight</span><span class="sxs-lookup"><span data-stu-id="8fb0a-122">weight</span></span>                | <span data-ttu-id="8fb0a-123">Gleitkommawert mit doppelter Genauigkeit</span><span class="sxs-lookup"><span data-stu-id="8fb0a-123">Double</span></span>                    | <span data-ttu-id="8fb0a-124">Der Wert, der angibt, wie viel das Dokument aktuell Trend ist.</span><span class="sxs-lookup"><span data-stu-id="8fb0a-124">Value indicating how much the document is currently trending.</span></span> <span data-ttu-id="8fb0a-125">Je höher die Zahl ist, desto das Dokument ist derzeit Trend um den Benutzer (aussagekräftiger ist es).</span><span class="sxs-lookup"><span data-stu-id="8fb0a-125">The larger the number, the more the document is currently trending around the user (the more relevant it is).</span></span> <span data-ttu-id="8fb0a-126">Zurückgegebene Dokumente werden durch diesen Wert sortiert.</span><span class="sxs-lookup"><span data-stu-id="8fb0a-126">Returned documents are sorted by this value.</span></span>  |
| <span data-ttu-id="8fb0a-127">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="8fb0a-127">resourceVisualization</span></span> | <span data-ttu-id="8fb0a-128">[ResourceVisualization](insights-resourcevisualization.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="8fb0a-128">[resourceVisualization](insights-resourcevisualization.md) collection</span></span> | <span data-ttu-id="8fb0a-129">Eigenschaften, die Sie verwenden können, um das Dokument in Ihre Erfahrung visualisieren.</span><span class="sxs-lookup"><span data-stu-id="8fb0a-129">Properties that you can use to visualize the document in your experience.</span></span> |
| <span data-ttu-id="8fb0a-130">resourceReference</span><span class="sxs-lookup"><span data-stu-id="8fb0a-130">resourceReference</span></span>     | <span data-ttu-id="8fb0a-131">[ResourceReference](insights-resourcereference.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="8fb0a-131">[resourceReference](insights-resourcereference.md) collection</span></span> | <span data-ttu-id="8fb0a-132">Referenz-Eigenschaften des Dokuments Trend, wie die Url und den Typ des Dokuments.</span><span class="sxs-lookup"><span data-stu-id="8fb0a-132">Reference properties of the trending document, such as the url and type of the document.</span></span> |

## <a name="relationships"></a><span data-ttu-id="8fb0a-133">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="8fb0a-133">Relationships</span></span>

| <span data-ttu-id="8fb0a-134">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8fb0a-134">Property</span></span>      | <span data-ttu-id="8fb0a-135">Typ</span><span class="sxs-lookup"><span data-stu-id="8fb0a-135">Type</span></span>          | <span data-ttu-id="8fb0a-136">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8fb0a-136">Description</span></span>  |
| ------------- |---------------| -------------|
| <span data-ttu-id="8fb0a-137">resource</span><span class="sxs-lookup"><span data-stu-id="8fb0a-137">resource</span></span>      | <span data-ttu-id="8fb0a-138">Entity-Auflistung</span><span class="sxs-lookup"><span data-stu-id="8fb0a-138">entity collection</span></span> | <span data-ttu-id="8fb0a-139">Zum Navigieren zu dem Trend Dokument verwendet.</span><span class="sxs-lookup"><span data-stu-id="8fb0a-139">Used for navigating to the trending document.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="8fb0a-140">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="8fb0a-140">JSON representation</span></span>

<span data-ttu-id="8fb0a-141">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="8fb0a-141">Here is a JSON representation of the resource</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.trending"
}-->
```json
{
  "id": "string",
  "weight": "double",
  "resourceVisualization": [{"@odata.type": "microsoft.graph.resourceVisualization"}],
  "resourceReference": [{"@odata.type": "microsoft.graph.resourceReference"}],
  
  "resource": [ { "@odata.type": "microsoft.graph.entity" } ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/insights-trending.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
