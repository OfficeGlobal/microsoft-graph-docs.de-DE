---
title: freigegebene Ressource-Typ
description: 'Einen Einblick, freigegebene mit oder von einem bestimmten Benutzer Dateien darstellt. Die folgenden freigegebenen Dateien werden unterstützt:'
author: simonhult
localization_priority: Normal
ms.openlocfilehash: 289523f836d7b8080f7317e4d11301c71314ba93
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27880612"
---
# <a name="shared-resource-type"></a><span data-ttu-id="d67ac-104">freigegebene Ressource-Typ</span><span class="sxs-lookup"><span data-stu-id="d67ac-104">shared resource type</span></span>

> <span data-ttu-id="d67ac-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="d67ac-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d67ac-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d67ac-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d67ac-107">Einen Einblick, freigegebene mit oder von einem bestimmten Benutzer Dateien darstellt.</span><span class="sxs-lookup"><span data-stu-id="d67ac-107">An insight representing files shared with or by a specific user.</span></span> <span data-ttu-id="d67ac-108">Die folgenden freigegebenen Dateien werden unterstützt:</span><span class="sxs-lookup"><span data-stu-id="d67ac-108">The following shared files are supported:</span></span>

- <span data-ttu-id="d67ac-109">Anlagen direkt in eine e-Mail oder eine Besprechung einladen.</span><span class="sxs-lookup"><span data-stu-id="d67ac-109">Files attached directly in an email or a meeting invite.</span></span>
- <span data-ttu-id="d67ac-110">OneDrive für Bussiness und SharePoint modernen Anlagen - Dateien in OneDrive für Unternehmen und SharePoint, die Benutzer in einer e-Mail als ein Links freigeben.</span><span class="sxs-lookup"><span data-stu-id="d67ac-110">OneDrive for Bussiness and SharePoint modern attachments - files stored in OneDrive for Business and SharePoint that users share as a links in an email.</span></span>

<span data-ttu-id="d67ac-111">**Hinweis**: Wir arbeiten derzeit auf die Ergebnisse der Shared-API mit Daten auffüllen.</span><span class="sxs-lookup"><span data-stu-id="d67ac-111">**Note**: We are currently working on populating the results of the Shared API with data.</span></span> <span data-ttu-id="d67ac-112">Möglicherweise gibt es einige Daten in den ersten Wochen nach der Veröffentlichung fehlt.</span><span class="sxs-lookup"><span data-stu-id="d67ac-112">There may be some data missing in the first weeks after release.</span></span>

## <a name="methods"></a><span data-ttu-id="d67ac-113">Methoden</span><span class="sxs-lookup"><span data-stu-id="d67ac-113">Methods</span></span>

| <span data-ttu-id="d67ac-114">Methode</span><span class="sxs-lookup"><span data-stu-id="d67ac-114">Method</span></span>       | <span data-ttu-id="d67ac-115">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="d67ac-115">Return Type</span></span>  |<span data-ttu-id="d67ac-116">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d67ac-116">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d67ac-117">Gemeinsame Liste</span><span class="sxs-lookup"><span data-stu-id="d67ac-117">List shared</span></span>](../api/insights-list-shared.md) |<span data-ttu-id="d67ac-118">[Insights_shared](insights-shared.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="d67ac-118">[insights_shared](insights-shared.md) collection</span></span>| <span data-ttu-id="d67ac-119">Rufen Sie eine Liste der freigegebenen Dateien.</span><span class="sxs-lookup"><span data-stu-id="d67ac-119">Get a list of shared files.</span></span>|

## <a name="properties"></a><span data-ttu-id="d67ac-120">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d67ac-120">Properties</span></span>

| <span data-ttu-id="d67ac-121">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d67ac-121">Property</span></span>              | <span data-ttu-id="d67ac-122">Typ</span><span class="sxs-lookup"><span data-stu-id="d67ac-122">Type</span></span>                      | <span data-ttu-id="d67ac-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d67ac-123">Description</span></span>  |
| -------------         |---------------            | -------------|
| <span data-ttu-id="d67ac-124">id</span><span class="sxs-lookup"><span data-stu-id="d67ac-124">id</span></span>                    | <span data-ttu-id="d67ac-125">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d67ac-125">String</span></span>                    | <span data-ttu-id="d67ac-126">Eindeutiger Bezeichner der Beziehung.</span><span class="sxs-lookup"><span data-stu-id="d67ac-126">Unique identifier of the relationship.</span></span> <span data-ttu-id="d67ac-127">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d67ac-127">Read only.</span></span>        |
| <span data-ttu-id="d67ac-128">lastShared</span><span class="sxs-lookup"><span data-stu-id="d67ac-128">lastShared</span></span>            | [<span data-ttu-id="d67ac-129">sharingDetail</span><span class="sxs-lookup"><span data-stu-id="d67ac-129">sharingDetail</span></span>](insights-sharingdetail.md)                | <span data-ttu-id="d67ac-130">Informationen zu freigegebenen Elements.</span><span class="sxs-lookup"><span data-stu-id="d67ac-130">Details about the shared item.</span></span> <span data-ttu-id="d67ac-131">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d67ac-131">Read only.</span></span>        |
| <span data-ttu-id="d67ac-132">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="d67ac-132">resourceVisualization</span></span> | [<span data-ttu-id="d67ac-133">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="d67ac-133">resourceVisualization</span></span>](insights-resourcevisualization.md)                | <span data-ttu-id="d67ac-134">Eigenschaften, die Sie verwenden können, um das Dokument in Ihre Erfahrung visualisieren.</span><span class="sxs-lookup"><span data-stu-id="d67ac-134">Properties that you can use to visualize the document in your experience.</span></span> <span data-ttu-id="d67ac-135">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d67ac-135">Read-only</span></span>      |
| <span data-ttu-id="d67ac-136">resourceReference</span><span class="sxs-lookup"><span data-stu-id="d67ac-136">resourceReference</span></span>     | [<span data-ttu-id="d67ac-137">resourceReference</span><span class="sxs-lookup"><span data-stu-id="d67ac-137">resourceReference</span></span>](insights-resourcereference.md)                      | <span data-ttu-id="d67ac-138">Referenz-Eigenschaften des freigegebenen Dokuments, wie die Url und den Typ des Dokuments.</span><span class="sxs-lookup"><span data-stu-id="d67ac-138">Reference properties of the shared document, such as the url and type of the document.</span></span> <span data-ttu-id="d67ac-139">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d67ac-139">Read-only</span></span>       |

## <a name="relationships"></a><span data-ttu-id="d67ac-140">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="d67ac-140">Relationships</span></span>

| <span data-ttu-id="d67ac-141">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d67ac-141">Property</span></span>      | <span data-ttu-id="d67ac-142">Typ</span><span class="sxs-lookup"><span data-stu-id="d67ac-142">Type</span></span>          | <span data-ttu-id="d67ac-143">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d67ac-143">Description</span></span>  |
| ------------- |---------------| -------------|
| <span data-ttu-id="d67ac-144">resource</span><span class="sxs-lookup"><span data-stu-id="d67ac-144">resource</span></span>      | <span data-ttu-id="d67ac-145">Entität</span><span class="sxs-lookup"><span data-stu-id="d67ac-145">Entity</span></span>        | <span data-ttu-id="d67ac-146">Verwendet zum Navigieren zu dem Element, das freigegeben wurde.</span><span class="sxs-lookup"><span data-stu-id="d67ac-146">Used for navigating to the item that was shared.</span></span> <span data-ttu-id="d67ac-147">Dateianlagen ist der Typ *FileAttachment*.</span><span class="sxs-lookup"><span data-stu-id="d67ac-147">For file attachments, the type is *fileAttachment*.</span></span> <span data-ttu-id="d67ac-148">Für verknüpfte Anlagen ist der Typ *DriveItem*.</span><span class="sxs-lookup"><span data-stu-id="d67ac-148">For linked attachments, the type is *driveItem*.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d67ac-149">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d67ac-149">JSON representation</span></span>
<span data-ttu-id="d67ac-150">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d67ac-150">Here is a JSON representation of the resource</span></span>

```json
{
  "id": "string",
  "lastShared": "sharingDetail",
  "resourceVisualization": "resourceVisualization",
  "resourceReference": "resourceReference",
  
  "resource": [ { "@odata.type": "microsoft.graph.entity" } ]
}
```
