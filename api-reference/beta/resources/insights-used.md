---
title: Ressourcentyp usedInsight
description: Einen Einblick, Dokumente, die von einem bestimmten Benutzer darstellt. Einblicke in die gibt, die zutreffenden Dokumente, die ein Benutzer anzeigen oder darauf zugreifen.
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 056654a5e467e202b2bde5ac8ee98dccab93d7c9
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574229"
---
# <a name="used-resource-type"></a><span data-ttu-id="83855-104">Ressourcentyp verwendet</span><span class="sxs-lookup"><span data-stu-id="83855-104">used resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="83855-105">Einen Einblick, Dokumente, die von einem bestimmten Benutzer darstellt.</span><span class="sxs-lookup"><span data-stu-id="83855-105">An insight representing documents used by a specific user.</span></span> <span data-ttu-id="83855-106">Einblicke in die gibt, die zutreffenden Dokumente, die ein Benutzer anzeigen oder darauf zugreifen.</span><span class="sxs-lookup"><span data-stu-id="83855-106">The insights returns the most relevant documents that a user viewed or accessed.</span></span> <span data-ttu-id="83855-107">Dazu gehören Dokumente in:</span><span class="sxs-lookup"><span data-stu-id="83855-107">This includes documents in:</span></span>

- <span data-ttu-id="83855-108">OneDrive for Business</span><span class="sxs-lookup"><span data-stu-id="83855-108">OneDrive for Business</span></span>
- <span data-ttu-id="83855-109">SharePoint</span><span class="sxs-lookup"><span data-stu-id="83855-109">SharePoint</span></span>

## <a name="methods"></a><span data-ttu-id="83855-110">Methoden</span><span class="sxs-lookup"><span data-stu-id="83855-110">Methods</span></span>

| <span data-ttu-id="83855-111">Methode</span><span class="sxs-lookup"><span data-stu-id="83855-111">Method</span></span>       | <span data-ttu-id="83855-112">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="83855-112">Return Type</span></span>  |<span data-ttu-id="83855-113">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="83855-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="83855-114">Verwendet wird</span><span class="sxs-lookup"><span data-stu-id="83855-114">List used</span></span>](../api/insights-list-used.md) |<span data-ttu-id="83855-115">[Insights_used](insights-used.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="83855-115">[insights_used](insights-used.md) collection</span></span>| <span data-ttu-id="83855-116">Rufen Sie eine Liste der geöffneten Dateien.</span><span class="sxs-lookup"><span data-stu-id="83855-116">Get a list of used files.</span></span>|

## <a name="properties"></a><span data-ttu-id="83855-117">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="83855-117">Properties</span></span>

| <span data-ttu-id="83855-118">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="83855-118">Property</span></span>              | <span data-ttu-id="83855-119">Typ</span><span class="sxs-lookup"><span data-stu-id="83855-119">Type</span></span>                      | <span data-ttu-id="83855-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="83855-120">Description</span></span>  |
| -------------         |---------------            | -------------|
| <span data-ttu-id="83855-121">id</span><span class="sxs-lookup"><span data-stu-id="83855-121">id</span></span>                    | <span data-ttu-id="83855-122">String</span><span class="sxs-lookup"><span data-stu-id="83855-122">String</span></span>                    | <span data-ttu-id="83855-123">Eindeutiger Bezeichner der Beziehung.</span><span class="sxs-lookup"><span data-stu-id="83855-123">Unique identifier of the relationship.</span></span> <span data-ttu-id="83855-124">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="83855-124">Read only.</span></span>        |
| <span data-ttu-id="83855-125">lastUsed</span><span class="sxs-lookup"><span data-stu-id="83855-125">lastUsed</span></span>              | [<span data-ttu-id="83855-126">usageDetails</span><span class="sxs-lookup"><span data-stu-id="83855-126">usageDetails</span></span>](insights-usagedetails.md)              | <span data-ttu-id="83855-127">Wenn das Element zuletzt Informationen angezeigt und vom Benutzer geändert.</span><span class="sxs-lookup"><span data-stu-id="83855-127">Information about when the item was last viewed and modified by the user.</span></span> <span data-ttu-id="83855-128">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="83855-128">Read only.</span></span>     |
| <span data-ttu-id="83855-129">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="83855-129">resourceVisualization</span></span> | [<span data-ttu-id="83855-130">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="83855-130">resourceVisualization</span></span>](insights-resourcevisualization.md)                | <span data-ttu-id="83855-131">Eigenschaften, die Sie verwenden können, um das Dokument in Ihre Erfahrung visualisieren.</span><span class="sxs-lookup"><span data-stu-id="83855-131">Properties that you can use to visualize the document in your experience.</span></span> <span data-ttu-id="83855-132">Schreibgeschützt</span><span class="sxs-lookup"><span data-stu-id="83855-132">Read-only</span></span>      |
| <span data-ttu-id="83855-133">resourceReference</span><span class="sxs-lookup"><span data-stu-id="83855-133">resourceReference</span></span>     | [<span data-ttu-id="83855-134">resourceReference</span><span class="sxs-lookup"><span data-stu-id="83855-134">resourceReference</span></span>](insights-resourcereference.md)                      | <span data-ttu-id="83855-135">Referenz-Eigenschaften des Dokuments verwendete, wie die Url und den Typ des Dokuments.</span><span class="sxs-lookup"><span data-stu-id="83855-135">Reference properties of the used document, such as the url and type of the document.</span></span> <span data-ttu-id="83855-136">Schreibgeschützt</span><span class="sxs-lookup"><span data-stu-id="83855-136">Read-only</span></span>     |

## <a name="relationships"></a><span data-ttu-id="83855-137">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="83855-137">Relationships</span></span>

| <span data-ttu-id="83855-138">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="83855-138">Property</span></span>      | <span data-ttu-id="83855-139">Typ</span><span class="sxs-lookup"><span data-stu-id="83855-139">Type</span></span>          | <span data-ttu-id="83855-140">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="83855-140">Description</span></span>  |
| ------------- |---------------| -------------|
| <span data-ttu-id="83855-141">resource</span><span class="sxs-lookup"><span data-stu-id="83855-141">resource</span></span>      | <span data-ttu-id="83855-142">Entity-Auflistung</span><span class="sxs-lookup"><span data-stu-id="83855-142">entity collection</span></span> | <span data-ttu-id="83855-143">Verwendet zum Navigieren zu dem Element, das verwendet wurde.</span><span class="sxs-lookup"><span data-stu-id="83855-143">Used for navigating to the item that was used.</span></span> <span data-ttu-id="83855-144">Dateianlagen ist der Typ *FileAttachment*.</span><span class="sxs-lookup"><span data-stu-id="83855-144">For file attachments, the type is *fileAttachment*.</span></span> <span data-ttu-id="83855-145">Für verknüpfte Anlagen ist der Typ *DriveItem*.</span><span class="sxs-lookup"><span data-stu-id="83855-145">For linked attachments, the type is *driveItem*.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="83855-146">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="83855-146">JSON representation</span></span>
<span data-ttu-id="83855-147">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="83855-147">Here is a JSON representation of the resource</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.usedInsight"
}-->
```json
{
  "id": "string",
  "lastUsed": "usageDetails",
  "resourceVisualization": "resourceVisualization",
  "resourceReference": "resourceReference",
  
  "resource": [ { "@odata.type": "microsoft.graph.entity" } ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/insights-used.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
