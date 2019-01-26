---
title: freigegebene Ressource-Typ
description: 'Einen Einblick, freigegebene mit oder von einem bestimmten Benutzer Dateien darstellt. Die folgenden freigegebenen Dateien werden unterstützt:'
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 49e18318c1e93d2393b957b404ff4617b334f237
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573179"
---
# <a name="shared-resource-type"></a><span data-ttu-id="0d929-104">freigegebene Ressource-Typ</span><span class="sxs-lookup"><span data-stu-id="0d929-104">shared resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0d929-105">Einen Einblick, freigegebene mit oder von einem bestimmten Benutzer Dateien darstellt.</span><span class="sxs-lookup"><span data-stu-id="0d929-105">An insight representing files shared with or by a specific user.</span></span> <span data-ttu-id="0d929-106">Die folgenden freigegebenen Dateien werden unterstützt:</span><span class="sxs-lookup"><span data-stu-id="0d929-106">The following shared files are supported:</span></span>

- <span data-ttu-id="0d929-107">Anlagen direkt in eine e-Mail oder eine Besprechung einladen.</span><span class="sxs-lookup"><span data-stu-id="0d929-107">Files attached directly in an email or a meeting invite.</span></span>
- <span data-ttu-id="0d929-108">OneDrive für Bussiness und SharePoint modernen Anlagen - Dateien in OneDrive für Unternehmen und SharePoint, die Benutzer in einer e-Mail als ein Links freigeben.</span><span class="sxs-lookup"><span data-stu-id="0d929-108">OneDrive for Bussiness and SharePoint modern attachments - files stored in OneDrive for Business and SharePoint that users share as a links in an email.</span></span>

<span data-ttu-id="0d929-109">**Hinweis**: Wir arbeiten derzeit auf die Ergebnisse der Shared-API mit Daten auffüllen.</span><span class="sxs-lookup"><span data-stu-id="0d929-109">**Note**: We are currently working on populating the results of the Shared API with data.</span></span> <span data-ttu-id="0d929-110">Möglicherweise gibt es einige Daten in den ersten Wochen nach der Veröffentlichung fehlt.</span><span class="sxs-lookup"><span data-stu-id="0d929-110">There may be some data missing in the first weeks after release.</span></span>

## <a name="methods"></a><span data-ttu-id="0d929-111">Methoden</span><span class="sxs-lookup"><span data-stu-id="0d929-111">Methods</span></span>

| <span data-ttu-id="0d929-112">Methode</span><span class="sxs-lookup"><span data-stu-id="0d929-112">Method</span></span>       | <span data-ttu-id="0d929-113">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="0d929-113">Return Type</span></span>  |<span data-ttu-id="0d929-114">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0d929-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0d929-115">Gemeinsame Liste</span><span class="sxs-lookup"><span data-stu-id="0d929-115">List shared</span></span>](../api/insights-list-shared.md) |<span data-ttu-id="0d929-116">[Insights_shared](insights-shared.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="0d929-116">[insights_shared](insights-shared.md) collection</span></span>| <span data-ttu-id="0d929-117">Rufen Sie eine Liste der freigegebenen Dateien.</span><span class="sxs-lookup"><span data-stu-id="0d929-117">Get a list of shared files.</span></span>|

## <a name="properties"></a><span data-ttu-id="0d929-118">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="0d929-118">Properties</span></span>

| <span data-ttu-id="0d929-119">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0d929-119">Property</span></span>              | <span data-ttu-id="0d929-120">Typ</span><span class="sxs-lookup"><span data-stu-id="0d929-120">Type</span></span>                      | <span data-ttu-id="0d929-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0d929-121">Description</span></span>  |
| -------------         |---------------            | -------------|
| <span data-ttu-id="0d929-122">id</span><span class="sxs-lookup"><span data-stu-id="0d929-122">id</span></span>                    | <span data-ttu-id="0d929-123">String</span><span class="sxs-lookup"><span data-stu-id="0d929-123">String</span></span>                    | <span data-ttu-id="0d929-124">Eindeutiger Bezeichner der Beziehung.</span><span class="sxs-lookup"><span data-stu-id="0d929-124">Unique identifier of the relationship.</span></span> <span data-ttu-id="0d929-125">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="0d929-125">Read only.</span></span>        |
| <span data-ttu-id="0d929-126">lastShared</span><span class="sxs-lookup"><span data-stu-id="0d929-126">lastShared</span></span>            | [<span data-ttu-id="0d929-127">sharingDetail</span><span class="sxs-lookup"><span data-stu-id="0d929-127">sharingDetail</span></span>](insights-sharingdetail.md)                | <span data-ttu-id="0d929-128">Informationen zu freigegebenen Elements.</span><span class="sxs-lookup"><span data-stu-id="0d929-128">Details about the shared item.</span></span> <span data-ttu-id="0d929-129">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="0d929-129">Read only.</span></span>        |
| <span data-ttu-id="0d929-130">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="0d929-130">resourceVisualization</span></span> | [<span data-ttu-id="0d929-131">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="0d929-131">resourceVisualization</span></span>](insights-resourcevisualization.md)                | <span data-ttu-id="0d929-132">Eigenschaften, die Sie verwenden können, um das Dokument in Ihre Erfahrung visualisieren.</span><span class="sxs-lookup"><span data-stu-id="0d929-132">Properties that you can use to visualize the document in your experience.</span></span> <span data-ttu-id="0d929-133">Schreibgeschützt</span><span class="sxs-lookup"><span data-stu-id="0d929-133">Read-only</span></span>      |
| <span data-ttu-id="0d929-134">resourceReference</span><span class="sxs-lookup"><span data-stu-id="0d929-134">resourceReference</span></span>     | [<span data-ttu-id="0d929-135">resourceReference</span><span class="sxs-lookup"><span data-stu-id="0d929-135">resourceReference</span></span>](insights-resourcereference.md)                      | <span data-ttu-id="0d929-136">Referenz-Eigenschaften des freigegebenen Dokuments, wie die Url und den Typ des Dokuments.</span><span class="sxs-lookup"><span data-stu-id="0d929-136">Reference properties of the shared document, such as the url and type of the document.</span></span> <span data-ttu-id="0d929-137">Schreibgeschützt</span><span class="sxs-lookup"><span data-stu-id="0d929-137">Read-only</span></span>       |

## <a name="relationships"></a><span data-ttu-id="0d929-138">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="0d929-138">Relationships</span></span>

| <span data-ttu-id="0d929-139">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0d929-139">Property</span></span>      | <span data-ttu-id="0d929-140">Typ</span><span class="sxs-lookup"><span data-stu-id="0d929-140">Type</span></span>          | <span data-ttu-id="0d929-141">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0d929-141">Description</span></span>  |
| ------------- |---------------| -------------|
| <span data-ttu-id="0d929-142">resource</span><span class="sxs-lookup"><span data-stu-id="0d929-142">resource</span></span>      | <span data-ttu-id="0d929-143">Entity-Auflistung</span><span class="sxs-lookup"><span data-stu-id="0d929-143">entity collection</span></span> | <span data-ttu-id="0d929-144">Verwendet zum Navigieren zu dem Element, das freigegeben wurde.</span><span class="sxs-lookup"><span data-stu-id="0d929-144">Used for navigating to the item that was shared.</span></span> <span data-ttu-id="0d929-145">Dateianlagen ist der Typ *FileAttachment*.</span><span class="sxs-lookup"><span data-stu-id="0d929-145">For file attachments, the type is *fileAttachment*.</span></span> <span data-ttu-id="0d929-146">Für verknüpfte Anlagen ist der Typ *DriveItem*.</span><span class="sxs-lookup"><span data-stu-id="0d929-146">For linked attachments, the type is *driveItem*.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="0d929-147">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="0d929-147">JSON representation</span></span>
<span data-ttu-id="0d929-148">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="0d929-148">Here is a JSON representation of the resource</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.shared"
}-->
```json
{
  "id": "string",
  "lastShared": "sharingDetail",
  "resourceVisualization": "resourceVisualization",
  "resourceReference": "resourceReference",
  
  "resource": [ { "@odata.type": "microsoft.graph.entity" } ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/insights-shared.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
