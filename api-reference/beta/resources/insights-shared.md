---
title: freigegebene Ressource-Typ
description: 'Einen Einblick, freigegebene mit oder von einem bestimmten Benutzer Dateien darstellt. Die folgenden freigegebenen Dateien werden unterstützt:'
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 2c3d91023e2d68704b54308dff9566673f71dfb0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27973706"
---
# <a name="shared-resource-type"></a><span data-ttu-id="70cd1-104">freigegebene Ressource-Typ</span><span class="sxs-lookup"><span data-stu-id="70cd1-104">shared resource type</span></span>

> <span data-ttu-id="70cd1-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="70cd1-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="70cd1-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="70cd1-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="70cd1-107">Einen Einblick, freigegebene mit oder von einem bestimmten Benutzer Dateien darstellt.</span><span class="sxs-lookup"><span data-stu-id="70cd1-107">An insight representing files shared with or by a specific user.</span></span> <span data-ttu-id="70cd1-108">Die folgenden freigegebenen Dateien werden unterstützt:</span><span class="sxs-lookup"><span data-stu-id="70cd1-108">The following shared files are supported:</span></span>

- <span data-ttu-id="70cd1-109">Anlagen direkt in eine e-Mail oder eine Besprechung einladen.</span><span class="sxs-lookup"><span data-stu-id="70cd1-109">Files attached directly in an email or a meeting invite.</span></span>
- <span data-ttu-id="70cd1-110">OneDrive für Bussiness und SharePoint modernen Anlagen - Dateien in OneDrive für Unternehmen und SharePoint, die Benutzer in einer e-Mail als ein Links freigeben.</span><span class="sxs-lookup"><span data-stu-id="70cd1-110">OneDrive for Bussiness and SharePoint modern attachments - files stored in OneDrive for Business and SharePoint that users share as a links in an email.</span></span>

<span data-ttu-id="70cd1-111">**Hinweis**: Wir arbeiten derzeit auf die Ergebnisse der Shared-API mit Daten auffüllen.</span><span class="sxs-lookup"><span data-stu-id="70cd1-111">**Note**: We are currently working on populating the results of the Shared API with data.</span></span> <span data-ttu-id="70cd1-112">Möglicherweise gibt es einige Daten in den ersten Wochen nach der Veröffentlichung fehlt.</span><span class="sxs-lookup"><span data-stu-id="70cd1-112">There may be some data missing in the first weeks after release.</span></span>

## <a name="methods"></a><span data-ttu-id="70cd1-113">Methoden</span><span class="sxs-lookup"><span data-stu-id="70cd1-113">Methods</span></span>

| <span data-ttu-id="70cd1-114">Methode</span><span class="sxs-lookup"><span data-stu-id="70cd1-114">Method</span></span>       | <span data-ttu-id="70cd1-115">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="70cd1-115">Return Type</span></span>  |<span data-ttu-id="70cd1-116">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="70cd1-116">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="70cd1-117">Gemeinsame Liste</span><span class="sxs-lookup"><span data-stu-id="70cd1-117">List shared</span></span>](../api/insights-list-shared.md) |<span data-ttu-id="70cd1-118">[Insights_shared](insights-shared.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="70cd1-118">[insights_shared](insights-shared.md) collection</span></span>| <span data-ttu-id="70cd1-119">Rufen Sie eine Liste der freigegebenen Dateien.</span><span class="sxs-lookup"><span data-stu-id="70cd1-119">Get a list of shared files.</span></span>|

## <a name="properties"></a><span data-ttu-id="70cd1-120">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="70cd1-120">Properties</span></span>

| <span data-ttu-id="70cd1-121">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="70cd1-121">Property</span></span>              | <span data-ttu-id="70cd1-122">Typ</span><span class="sxs-lookup"><span data-stu-id="70cd1-122">Type</span></span>                      | <span data-ttu-id="70cd1-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="70cd1-123">Description</span></span>  |
| -------------         |---------------            | -------------|
| <span data-ttu-id="70cd1-124">id</span><span class="sxs-lookup"><span data-stu-id="70cd1-124">id</span></span>                    | <span data-ttu-id="70cd1-125">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="70cd1-125">String</span></span>                    | <span data-ttu-id="70cd1-126">Eindeutiger Bezeichner der Beziehung.</span><span class="sxs-lookup"><span data-stu-id="70cd1-126">Unique identifier of the relationship.</span></span> <span data-ttu-id="70cd1-127">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="70cd1-127">Read only.</span></span>        |
| <span data-ttu-id="70cd1-128">lastShared</span><span class="sxs-lookup"><span data-stu-id="70cd1-128">lastShared</span></span>            | [<span data-ttu-id="70cd1-129">sharingDetail</span><span class="sxs-lookup"><span data-stu-id="70cd1-129">sharingDetail</span></span>](insights-sharingdetail.md)                | <span data-ttu-id="70cd1-130">Informationen zu freigegebenen Elements.</span><span class="sxs-lookup"><span data-stu-id="70cd1-130">Details about the shared item.</span></span> <span data-ttu-id="70cd1-131">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="70cd1-131">Read only.</span></span>        |
| <span data-ttu-id="70cd1-132">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="70cd1-132">resourceVisualization</span></span> | [<span data-ttu-id="70cd1-133">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="70cd1-133">resourceVisualization</span></span>](insights-resourcevisualization.md)                | <span data-ttu-id="70cd1-134">Eigenschaften, die Sie verwenden können, um das Dokument in Ihre Erfahrung visualisieren.</span><span class="sxs-lookup"><span data-stu-id="70cd1-134">Properties that you can use to visualize the document in your experience.</span></span> <span data-ttu-id="70cd1-135">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="70cd1-135">Read-only</span></span>      |
| <span data-ttu-id="70cd1-136">resourceReference</span><span class="sxs-lookup"><span data-stu-id="70cd1-136">resourceReference</span></span>     | [<span data-ttu-id="70cd1-137">resourceReference</span><span class="sxs-lookup"><span data-stu-id="70cd1-137">resourceReference</span></span>](insights-resourcereference.md)                      | <span data-ttu-id="70cd1-138">Referenz-Eigenschaften des freigegebenen Dokuments, wie die Url und den Typ des Dokuments.</span><span class="sxs-lookup"><span data-stu-id="70cd1-138">Reference properties of the shared document, such as the url and type of the document.</span></span> <span data-ttu-id="70cd1-139">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="70cd1-139">Read-only</span></span>       |

## <a name="relationships"></a><span data-ttu-id="70cd1-140">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="70cd1-140">Relationships</span></span>

| <span data-ttu-id="70cd1-141">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="70cd1-141">Property</span></span>      | <span data-ttu-id="70cd1-142">Typ</span><span class="sxs-lookup"><span data-stu-id="70cd1-142">Type</span></span>          | <span data-ttu-id="70cd1-143">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="70cd1-143">Description</span></span>  |
| ------------- |---------------| -------------|
| <span data-ttu-id="70cd1-144">resource</span><span class="sxs-lookup"><span data-stu-id="70cd1-144">resource</span></span>      | <span data-ttu-id="70cd1-145">Entität</span><span class="sxs-lookup"><span data-stu-id="70cd1-145">Entity</span></span>        | <span data-ttu-id="70cd1-146">Verwendet zum Navigieren zu dem Element, das freigegeben wurde.</span><span class="sxs-lookup"><span data-stu-id="70cd1-146">Used for navigating to the item that was shared.</span></span> <span data-ttu-id="70cd1-147">Dateianlagen ist der Typ *FileAttachment*.</span><span class="sxs-lookup"><span data-stu-id="70cd1-147">For file attachments, the type is *fileAttachment*.</span></span> <span data-ttu-id="70cd1-148">Für verknüpfte Anlagen ist der Typ *DriveItem*.</span><span class="sxs-lookup"><span data-stu-id="70cd1-148">For linked attachments, the type is *driveItem*.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="70cd1-149">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="70cd1-149">JSON representation</span></span>
<span data-ttu-id="70cd1-150">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="70cd1-150">Here is a JSON representation of the resource</span></span>

```json
{
  "id": "string",
  "lastShared": "sharingDetail",
  "resourceVisualization": "resourceVisualization",
  "resourceReference": "resourceReference",
  
  "resource": [ { "@odata.type": "microsoft.graph.entity" } ]
}
```
