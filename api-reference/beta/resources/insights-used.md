---
title: Ressourcentyp verwendet
description: Einen Einblick, Dokumente, die von einem bestimmten Benutzer darstellt. Einblicke in die gibt, die zutreffenden Dokumente, die ein Benutzer anzeigen oder darauf zugreifen.
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 35698741cd457f4e8d202b13dd9099bb2669b6e1
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/30/2019
ms.locfileid: "29642541"
---
# <a name="used-resource-type"></a><span data-ttu-id="399ea-104">Ressourcentyp verwendet</span><span class="sxs-lookup"><span data-stu-id="399ea-104">used resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="399ea-105">Einen Einblick, Dokumente, die von einem bestimmten Benutzer darstellt.</span><span class="sxs-lookup"><span data-stu-id="399ea-105">An insight representing documents used by a specific user.</span></span> <span data-ttu-id="399ea-106">Einblicke in die gibt, die zutreffenden Dokumente, die ein Benutzer anzeigen oder darauf zugreifen.</span><span class="sxs-lookup"><span data-stu-id="399ea-106">The insights returns the most relevant documents that a user viewed or accessed.</span></span> <span data-ttu-id="399ea-107">Dazu gehören Dokumente in:</span><span class="sxs-lookup"><span data-stu-id="399ea-107">This includes documents in:</span></span>

- <span data-ttu-id="399ea-108">OneDrive for Business</span><span class="sxs-lookup"><span data-stu-id="399ea-108">OneDrive for Business</span></span>
- <span data-ttu-id="399ea-109">SharePoint</span><span class="sxs-lookup"><span data-stu-id="399ea-109">SharePoint</span></span>

## <a name="methods"></a><span data-ttu-id="399ea-110">Methoden</span><span class="sxs-lookup"><span data-stu-id="399ea-110">Methods</span></span>

| <span data-ttu-id="399ea-111">Methode</span><span class="sxs-lookup"><span data-stu-id="399ea-111">Method</span></span>       | <span data-ttu-id="399ea-112">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="399ea-112">Return Type</span></span>  |<span data-ttu-id="399ea-113">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="399ea-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="399ea-114">Verwendet wird</span><span class="sxs-lookup"><span data-stu-id="399ea-114">List used</span></span>](../api/insights-list-used.md) |<span data-ttu-id="399ea-115">[Insights_used](insights-used.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="399ea-115">[insights_used](insights-used.md) collection</span></span>| <span data-ttu-id="399ea-116">Rufen Sie eine Liste der geöffneten Dateien.</span><span class="sxs-lookup"><span data-stu-id="399ea-116">Get a list of used files.</span></span>|

## <a name="properties"></a><span data-ttu-id="399ea-117">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="399ea-117">Properties</span></span>

| <span data-ttu-id="399ea-118">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="399ea-118">Property</span></span>              | <span data-ttu-id="399ea-119">Typ</span><span class="sxs-lookup"><span data-stu-id="399ea-119">Type</span></span>                      | <span data-ttu-id="399ea-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="399ea-120">Description</span></span>  |
| -------------         |---------------            | -------------|
| <span data-ttu-id="399ea-121">id</span><span class="sxs-lookup"><span data-stu-id="399ea-121">id</span></span>                    | <span data-ttu-id="399ea-122">String</span><span class="sxs-lookup"><span data-stu-id="399ea-122">String</span></span>                    | <span data-ttu-id="399ea-123">Eindeutiger Bezeichner der Beziehung.</span><span class="sxs-lookup"><span data-stu-id="399ea-123">Unique identifier of the relationship.</span></span> <span data-ttu-id="399ea-124">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="399ea-124">Read only.</span></span>        |
| <span data-ttu-id="399ea-125">lastUsed</span><span class="sxs-lookup"><span data-stu-id="399ea-125">lastUsed</span></span>              | [<span data-ttu-id="399ea-126">usageDetails</span><span class="sxs-lookup"><span data-stu-id="399ea-126">usageDetails</span></span>](insights-usagedetails.md)              | <span data-ttu-id="399ea-127">Wenn das Element zuletzt Informationen angezeigt und vom Benutzer geändert.</span><span class="sxs-lookup"><span data-stu-id="399ea-127">Information about when the item was last viewed and modified by the user.</span></span> <span data-ttu-id="399ea-128">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="399ea-128">Read only.</span></span>     |
| <span data-ttu-id="399ea-129">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="399ea-129">resourceVisualization</span></span> | [<span data-ttu-id="399ea-130">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="399ea-130">resourceVisualization</span></span>](insights-resourcevisualization.md)                | <span data-ttu-id="399ea-131">Eigenschaften, die Sie verwenden können, um das Dokument in Ihre Erfahrung visualisieren.</span><span class="sxs-lookup"><span data-stu-id="399ea-131">Properties that you can use to visualize the document in your experience.</span></span> <span data-ttu-id="399ea-132">Schreibgeschützt</span><span class="sxs-lookup"><span data-stu-id="399ea-132">Read-only</span></span>      |
| <span data-ttu-id="399ea-133">resourceReference</span><span class="sxs-lookup"><span data-stu-id="399ea-133">resourceReference</span></span>     | [<span data-ttu-id="399ea-134">resourceReference</span><span class="sxs-lookup"><span data-stu-id="399ea-134">resourceReference</span></span>](insights-resourcereference.md)                      | <span data-ttu-id="399ea-135">Referenz-Eigenschaften des Dokuments verwendete, wie die Url und den Typ des Dokuments.</span><span class="sxs-lookup"><span data-stu-id="399ea-135">Reference properties of the used document, such as the url and type of the document.</span></span> <span data-ttu-id="399ea-136">Schreibgeschützt</span><span class="sxs-lookup"><span data-stu-id="399ea-136">Read-only</span></span>     |

## <a name="relationships"></a><span data-ttu-id="399ea-137">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="399ea-137">Relationships</span></span>

| <span data-ttu-id="399ea-138">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="399ea-138">Property</span></span>      | <span data-ttu-id="399ea-139">Typ</span><span class="sxs-lookup"><span data-stu-id="399ea-139">Type</span></span>          | <span data-ttu-id="399ea-140">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="399ea-140">Description</span></span>  |
| ------------- |---------------| -------------|
| <span data-ttu-id="399ea-141">resource</span><span class="sxs-lookup"><span data-stu-id="399ea-141">resource</span></span>      | <span data-ttu-id="399ea-142">Entität</span><span class="sxs-lookup"><span data-stu-id="399ea-142">Entity</span></span>        | <span data-ttu-id="399ea-143">Verwendet zum Navigieren zu dem Element, das verwendet wurde.</span><span class="sxs-lookup"><span data-stu-id="399ea-143">Used for navigating to the item that was used.</span></span> <span data-ttu-id="399ea-144">Dateianlagen ist der Typ *FileAttachment*.</span><span class="sxs-lookup"><span data-stu-id="399ea-144">For file attachments, the type is *fileAttachment*.</span></span> <span data-ttu-id="399ea-145">Für verknüpfte Anlagen ist der Typ *DriveItem*.</span><span class="sxs-lookup"><span data-stu-id="399ea-145">For linked attachments, the type is *driveItem*.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="399ea-146">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="399ea-146">JSON representation</span></span>
<span data-ttu-id="399ea-147">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="399ea-147">Here is a JSON representation of the resource</span></span>

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
