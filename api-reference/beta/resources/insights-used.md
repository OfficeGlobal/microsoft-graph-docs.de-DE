---
title: Ressourcentyp verwendet
description: Einen Einblick, Dokumente, die von einem bestimmten Benutzer darstellt. Einblicke in die gibt, die zutreffenden Dokumente, die ein Benutzer anzeigen oder darauf zugreifen.
author: simonhult
ms.openlocfilehash: 89eac33ad954905c77a26df669bb15a2cf471edd
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27323485"
---
# <a name="used-resource-type"></a><span data-ttu-id="f74d2-104">Ressourcentyp verwendet</span><span class="sxs-lookup"><span data-stu-id="f74d2-104">used resource type</span></span>

> <span data-ttu-id="f74d2-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f74d2-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f74d2-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f74d2-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f74d2-107">Einen Einblick, Dokumente, die von einem bestimmten Benutzer darstellt.</span><span class="sxs-lookup"><span data-stu-id="f74d2-107">An insight representing documents used by a specific user.</span></span> <span data-ttu-id="f74d2-108">Einblicke in die gibt, die zutreffenden Dokumente, die ein Benutzer anzeigen oder darauf zugreifen.</span><span class="sxs-lookup"><span data-stu-id="f74d2-108">The insights returns the most relevant documents that a user viewed or accessed.</span></span> <span data-ttu-id="f74d2-109">Dazu gehören Dokumente in:</span><span class="sxs-lookup"><span data-stu-id="f74d2-109">This includes documents in:</span></span>

- <span data-ttu-id="f74d2-110">OneDrive for Business</span><span class="sxs-lookup"><span data-stu-id="f74d2-110">OneDrive for Business</span></span>
- <span data-ttu-id="f74d2-111">SharePoint</span><span class="sxs-lookup"><span data-stu-id="f74d2-111">SharePoint</span></span>

## <a name="methods"></a><span data-ttu-id="f74d2-112">Methoden</span><span class="sxs-lookup"><span data-stu-id="f74d2-112">Methods</span></span>

| <span data-ttu-id="f74d2-113">Methode</span><span class="sxs-lookup"><span data-stu-id="f74d2-113">Method</span></span>       | <span data-ttu-id="f74d2-114">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="f74d2-114">Return Type</span></span>  |<span data-ttu-id="f74d2-115">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f74d2-115">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f74d2-116">Verwendet wird</span><span class="sxs-lookup"><span data-stu-id="f74d2-116">List used</span></span>](../api/insights-list-used.md) |<span data-ttu-id="f74d2-117">[Insights_used](insights-used.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="f74d2-117">[insights_used](insights-used.md) collection</span></span>| <span data-ttu-id="f74d2-118">Rufen Sie eine Liste der geöffneten Dateien.</span><span class="sxs-lookup"><span data-stu-id="f74d2-118">Get a list of used files.</span></span>|

## <a name="properties"></a><span data-ttu-id="f74d2-119">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f74d2-119">Properties</span></span>

| <span data-ttu-id="f74d2-120">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f74d2-120">Property</span></span>              | <span data-ttu-id="f74d2-121">Typ</span><span class="sxs-lookup"><span data-stu-id="f74d2-121">Type</span></span>                      | <span data-ttu-id="f74d2-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f74d2-122">Description</span></span>  |
| -------------         |---------------            | -------------|
| <span data-ttu-id="f74d2-123">id</span><span class="sxs-lookup"><span data-stu-id="f74d2-123">id</span></span>                    | <span data-ttu-id="f74d2-124">String</span><span class="sxs-lookup"><span data-stu-id="f74d2-124">String</span></span>                    | <span data-ttu-id="f74d2-125">Eindeutiger Bezeichner der Beziehung.</span><span class="sxs-lookup"><span data-stu-id="f74d2-125">Unique identifier of the relationship.</span></span> <span data-ttu-id="f74d2-126">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="f74d2-126">Read only.</span></span>        |
| <span data-ttu-id="f74d2-127">lastUsed</span><span class="sxs-lookup"><span data-stu-id="f74d2-127">lastUsed</span></span>              | [<span data-ttu-id="f74d2-128">usageDetails</span><span class="sxs-lookup"><span data-stu-id="f74d2-128">usageDetails</span></span>](insights-usagedetails.md)              | <span data-ttu-id="f74d2-129">Wenn das Element zuletzt Informationen angezeigt und vom Benutzer geändert.</span><span class="sxs-lookup"><span data-stu-id="f74d2-129">Information about when the item was last viewed and modified by the user.</span></span> <span data-ttu-id="f74d2-130">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="f74d2-130">Read only.</span></span>     |
| <span data-ttu-id="f74d2-131">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="f74d2-131">resourceVisualization</span></span> | [<span data-ttu-id="f74d2-132">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="f74d2-132">resourceVisualization</span></span>](insights-resourcevisualization.md)                | <span data-ttu-id="f74d2-133">Eigenschaften, die Sie verwenden können, um das Dokument in Ihre Erfahrung visualisieren.</span><span class="sxs-lookup"><span data-stu-id="f74d2-133">Properties that you can use to visualize the document in your experience.</span></span> <span data-ttu-id="f74d2-134">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="f74d2-134">Read-only</span></span>      |
| <span data-ttu-id="f74d2-135">resourceReference</span><span class="sxs-lookup"><span data-stu-id="f74d2-135">resourceReference</span></span>     | [<span data-ttu-id="f74d2-136">resourceReference</span><span class="sxs-lookup"><span data-stu-id="f74d2-136">resourceReference</span></span>](insights-resourcereference.md)                      | <span data-ttu-id="f74d2-137">Referenz-Eigenschaften des Dokuments verwendete, wie die Url und den Typ des Dokuments.</span><span class="sxs-lookup"><span data-stu-id="f74d2-137">Reference properties of the used document, such as the url and type of the document.</span></span> <span data-ttu-id="f74d2-138">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="f74d2-138">Read-only</span></span>     |

## <a name="relationships"></a><span data-ttu-id="f74d2-139">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="f74d2-139">Relationships</span></span>

| <span data-ttu-id="f74d2-140">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f74d2-140">Property</span></span>      | <span data-ttu-id="f74d2-141">Typ</span><span class="sxs-lookup"><span data-stu-id="f74d2-141">Type</span></span>          | <span data-ttu-id="f74d2-142">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f74d2-142">Description</span></span>  |
| ------------- |---------------| -------------|
| <span data-ttu-id="f74d2-143">resource</span><span class="sxs-lookup"><span data-stu-id="f74d2-143">resource</span></span>      | <span data-ttu-id="f74d2-144">Entität</span><span class="sxs-lookup"><span data-stu-id="f74d2-144">Entity</span></span>        | <span data-ttu-id="f74d2-145">Verwendet zum Navigieren zu dem Element, das verwendet wurde.</span><span class="sxs-lookup"><span data-stu-id="f74d2-145">Used for navigating to the item that was used.</span></span> <span data-ttu-id="f74d2-146">Dateianlagen ist der Typ *FileAttachment*.</span><span class="sxs-lookup"><span data-stu-id="f74d2-146">For file attachments, the type is *fileAttachment*.</span></span> <span data-ttu-id="f74d2-147">Für verknüpfte Anlagen ist der Typ *DriveItem*.</span><span class="sxs-lookup"><span data-stu-id="f74d2-147">For linked attachments, the type is *driveItem*.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f74d2-148">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="f74d2-148">JSON representation</span></span>
<span data-ttu-id="f74d2-149">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="f74d2-149">Here is a JSON representation of the resource</span></span>

```json
{
  "id": "string",
  "lastUsed": "usageDetails",
  "resourceVisualization": "resourceVisualization",
  "resourceReference": "resourceReference",
  
  "resource": [ { "@odata.type": "microsoft.graph.entity" } ]
}
```