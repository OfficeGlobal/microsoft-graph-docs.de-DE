---
title: Ressourcentyp verwendet
description: 'Einen Einblick, Dokumente, die von einem bestimmten Benutzer darstellt. Einblicke in die gibt, die zutreffenden Dokumente, die ein Benutzer anzeigen oder darauf zugreifen. Dazu gehören Dokumente in:'
ms.openlocfilehash: 3c82d268a67ef52d0ddfdad9193558080048ad6b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063993"
---
# <a name="used-resource-type"></a><span data-ttu-id="45d2e-105">Ressourcentyp verwendet</span><span class="sxs-lookup"><span data-stu-id="45d2e-105">used resource type</span></span>

> <span data-ttu-id="45d2e-106">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="45d2e-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="45d2e-107">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="45d2e-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="45d2e-108">Einen Einblick, Dokumente, die von einem bestimmten Benutzer darstellt.</span><span class="sxs-lookup"><span data-stu-id="45d2e-108">An insight representing documents used by a specific user.</span></span> <span data-ttu-id="45d2e-109">Einblicke in die gibt, die zutreffenden Dokumente, die ein Benutzer anzeigen oder darauf zugreifen.</span><span class="sxs-lookup"><span data-stu-id="45d2e-109">The insights returns the most relevant documents that a user viewed or accessed.</span></span> <span data-ttu-id="45d2e-110">Dazu gehören Dokumente in:</span><span class="sxs-lookup"><span data-stu-id="45d2e-110">This includes documents in:</span></span>

- <span data-ttu-id="45d2e-111">OneDrive for Business</span><span class="sxs-lookup"><span data-stu-id="45d2e-111">OneDrive for Business</span></span>
- <span data-ttu-id="45d2e-112">SharePoint</span><span class="sxs-lookup"><span data-stu-id="45d2e-112">SharePoint</span></span>

## <a name="methods"></a><span data-ttu-id="45d2e-113">Methoden</span><span class="sxs-lookup"><span data-stu-id="45d2e-113">Methods</span></span>

| <span data-ttu-id="45d2e-114">Methode</span><span class="sxs-lookup"><span data-stu-id="45d2e-114">Method</span></span>       | <span data-ttu-id="45d2e-115">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="45d2e-115">Return Type</span></span>  |<span data-ttu-id="45d2e-116">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="45d2e-116">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="45d2e-117">Verwendet wird</span><span class="sxs-lookup"><span data-stu-id="45d2e-117">List used</span></span>](../api/insights-list-used.md) |<span data-ttu-id="45d2e-118">[Insights_used](insights-used.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="45d2e-118">[insights_used](insights-used.md) collection</span></span>| <span data-ttu-id="45d2e-119">Rufen Sie eine Liste der geöffneten Dateien.</span><span class="sxs-lookup"><span data-stu-id="45d2e-119">Get a list of used files.</span></span>|

## <a name="properties"></a><span data-ttu-id="45d2e-120">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="45d2e-120">Properties</span></span>

| <span data-ttu-id="45d2e-121">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="45d2e-121">Property</span></span>              | <span data-ttu-id="45d2e-122">Typ</span><span class="sxs-lookup"><span data-stu-id="45d2e-122">Type</span></span>                      | <span data-ttu-id="45d2e-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="45d2e-123">Description</span></span>  |
| -------------         |---------------            | -------------|
| <span data-ttu-id="45d2e-124">id</span><span class="sxs-lookup"><span data-stu-id="45d2e-124">id</span></span>                    | <span data-ttu-id="45d2e-125">String</span><span class="sxs-lookup"><span data-stu-id="45d2e-125">String</span></span>                    | <span data-ttu-id="45d2e-126">Eindeutiger Bezeichner der Beziehung.</span><span class="sxs-lookup"><span data-stu-id="45d2e-126">Unique identifier of the relationship.</span></span> <span data-ttu-id="45d2e-127">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="45d2e-127">Read only.</span></span>        |
| <span data-ttu-id="45d2e-128">lastUsed</span><span class="sxs-lookup"><span data-stu-id="45d2e-128">lastUsed</span></span>              | [<span data-ttu-id="45d2e-129">usageDetails</span><span class="sxs-lookup"><span data-stu-id="45d2e-129">usageDetails</span></span>](insights-usagedetails.md)              | <span data-ttu-id="45d2e-130">Wenn das Element zuletzt Informationen angezeigt und vom Benutzer geändert.</span><span class="sxs-lookup"><span data-stu-id="45d2e-130">Information about when the item was last viewed and modified by the user.</span></span> <span data-ttu-id="45d2e-131">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="45d2e-131">Read only.</span></span>     |
| <span data-ttu-id="45d2e-132">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="45d2e-132">resourceVisualization</span></span> | [<span data-ttu-id="45d2e-133">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="45d2e-133">resourceVisualization</span></span>](insights-resourcevisualization.md)                | <span data-ttu-id="45d2e-134">Eigenschaften, die Sie verwenden können, um das Dokument in Ihre Erfahrung visualisieren.</span><span class="sxs-lookup"><span data-stu-id="45d2e-134">Properties that you can use to visualize the document in your experience.</span></span> <span data-ttu-id="45d2e-135">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="45d2e-135">Read-only</span></span>      |
| <span data-ttu-id="45d2e-136">resourceReference</span><span class="sxs-lookup"><span data-stu-id="45d2e-136">resourceReference</span></span>     | [<span data-ttu-id="45d2e-137">resourceReference</span><span class="sxs-lookup"><span data-stu-id="45d2e-137">resourceReference</span></span>](insights-resourcereference.md)                      | <span data-ttu-id="45d2e-138">Referenz-Eigenschaften des Dokuments verwendete, wie die Url und den Typ des Dokuments.</span><span class="sxs-lookup"><span data-stu-id="45d2e-138">Reference properties of the used document, such as the url and type of the document.</span></span> <span data-ttu-id="45d2e-139">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="45d2e-139">Read-only</span></span>     |

## <a name="relationships"></a><span data-ttu-id="45d2e-140">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="45d2e-140">Relationships</span></span>

| <span data-ttu-id="45d2e-141">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="45d2e-141">Property</span></span>      | <span data-ttu-id="45d2e-142">Typ</span><span class="sxs-lookup"><span data-stu-id="45d2e-142">Type</span></span>          | <span data-ttu-id="45d2e-143">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="45d2e-143">Description</span></span>  |
| ------------- |---------------| -------------|
| <span data-ttu-id="45d2e-144">resource</span><span class="sxs-lookup"><span data-stu-id="45d2e-144">resource</span></span>      | <span data-ttu-id="45d2e-145">Entität</span><span class="sxs-lookup"><span data-stu-id="45d2e-145">Entity</span></span>        | <span data-ttu-id="45d2e-146">Verwendet zum Navigieren zu dem Element, das verwendet wurde.</span><span class="sxs-lookup"><span data-stu-id="45d2e-146">Used for navigating to the item that was used.</span></span> <span data-ttu-id="45d2e-147">Dateianlagen ist der Typ *FileAttachment*.</span><span class="sxs-lookup"><span data-stu-id="45d2e-147">For file attachments, the type is *fileAttachment*.</span></span> <span data-ttu-id="45d2e-148">Für verknüpfte Anlagen ist der Typ *DriveItem*.</span><span class="sxs-lookup"><span data-stu-id="45d2e-148">For linked attachments, the type is *driveItem*.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="45d2e-149">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="45d2e-149">JSON representation</span></span>
<span data-ttu-id="45d2e-150">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="45d2e-150">Here is a JSON representation of the resource</span></span>

```json
{
  "id": "string",
  "lastUsed": "usageDetails",
  "resourceVisualization": "resourceVisualization",
  "resourceReference": "resourceReference",
  
  "resource": [ { "@odata.type": "microsoft.graph.entity" } ]
}
```