---
title: Trend Ressourcentyp
description: Rich-Beziehung Herstellen einer Verbindung mit einem Benutzer Dokumente, die auf den Benutzer (für den Benutzer relevant sind) Trend sind. OneDrive-Dateien, und um die Benutzer können Dateien, die auf SharePoint-Teamwebsites trend.
ms.openlocfilehash: 7d240c4358047ca9ba3d6b8340fbfb7d893a6a1d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062161"
---
# <a name="trending-resource-type"></a><span data-ttu-id="94596-104">Trend Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="94596-104">trending resource type</span></span>

> <span data-ttu-id="94596-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="94596-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="94596-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="94596-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="94596-107">Rich-Beziehung Herstellen einer Verbindung mit einem Benutzer Dokumente, die auf den Benutzer (für den Benutzer relevant sind) Trend sind.</span><span class="sxs-lookup"><span data-stu-id="94596-107">Rich relationship connecting a user to documents that are trending around the user (are relevant to the user).</span></span> <span data-ttu-id="94596-108">OneDrive-Dateien, und um die Benutzer können Dateien, die auf SharePoint-Teamwebsites trend.</span><span class="sxs-lookup"><span data-stu-id="94596-108">OneDrive files, and files stored on SharePoint team sites can trend around the user.</span></span>

## <a name="methods"></a><span data-ttu-id="94596-109">Methoden</span><span class="sxs-lookup"><span data-stu-id="94596-109">Methods</span></span>

| <span data-ttu-id="94596-110">Methode</span><span class="sxs-lookup"><span data-stu-id="94596-110">Method</span></span>       | <span data-ttu-id="94596-111">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="94596-111">Return Type</span></span>  |<span data-ttu-id="94596-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="94596-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="94596-113">Liste Trend</span><span class="sxs-lookup"><span data-stu-id="94596-113">List trending</span></span>](../api/insights-list-trending.md) |<span data-ttu-id="94596-114">[Insights_trending](insights-trending.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="94596-114">[insights_trending](insights-trending.md) collection</span></span>| <span data-ttu-id="94596-115">Abrufen einer Liste von Trend-Dateien.</span><span class="sxs-lookup"><span data-stu-id="94596-115">Get a list of trending files.</span></span>|

## <a name="properties"></a><span data-ttu-id="94596-116">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="94596-116">Properties</span></span>

| <span data-ttu-id="94596-117">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="94596-117">Property</span></span>      | <span data-ttu-id="94596-118">Typ</span><span class="sxs-lookup"><span data-stu-id="94596-118">Type</span></span>                              | <span data-ttu-id="94596-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="94596-119">Description</span></span>  |
| ------------- |---------------                    | -------------|
| <span data-ttu-id="94596-120">id</span><span class="sxs-lookup"><span data-stu-id="94596-120">id</span></span>                    | <span data-ttu-id="94596-121">String</span><span class="sxs-lookup"><span data-stu-id="94596-121">String</span></span>                    | <span data-ttu-id="94596-122">Eindeutiger Bezeichner der Beziehung.</span><span class="sxs-lookup"><span data-stu-id="94596-122">Unique identifier of the relationship.</span></span> <span data-ttu-id="94596-123">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="94596-123">Read only.</span></span>        |
| <span data-ttu-id="94596-124">weight</span><span class="sxs-lookup"><span data-stu-id="94596-124">weight</span></span>                | <span data-ttu-id="94596-125">Gleitkommawert mit doppelter Genauigkeit</span><span class="sxs-lookup"><span data-stu-id="94596-125">Double</span></span>                    | <span data-ttu-id="94596-126">Der Wert, der angibt, wie viel das Dokument aktuell Trend ist.</span><span class="sxs-lookup"><span data-stu-id="94596-126">Value indicating how much the document is currently trending.</span></span> <span data-ttu-id="94596-127">Je höher die Zahl ist, desto das Dokument ist derzeit Trend um den Benutzer (aussagekräftiger ist es).</span><span class="sxs-lookup"><span data-stu-id="94596-127">The larger the number, the more the document is currently trending around the user (the more relevant it is).</span></span> <span data-ttu-id="94596-128">Zurückgegebene Dokumente werden durch diesen Wert sortiert.</span><span class="sxs-lookup"><span data-stu-id="94596-128">Returned documents are sorted by this value.</span></span>  |
| <span data-ttu-id="94596-129">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="94596-129">resourceVisualization</span></span> | [<span data-ttu-id="94596-130">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="94596-130">resourceVisualization</span></span>](insights-resourcevisualization.md)    | <span data-ttu-id="94596-131">Eigenschaften, die Sie verwenden können, um das Dokument in Ihre Erfahrung visualisieren.</span><span class="sxs-lookup"><span data-stu-id="94596-131">Properties that you can use to visualize the document in your experience.</span></span> |
| <span data-ttu-id="94596-132">resourceReference</span><span class="sxs-lookup"><span data-stu-id="94596-132">resourceReference</span></span>     | [<span data-ttu-id="94596-133">resourceReference</span><span class="sxs-lookup"><span data-stu-id="94596-133">resourceReference</span></span>](insights-resourcereference.md)        | <span data-ttu-id="94596-134">Referenz-Eigenschaften des Dokuments Trend, wie die Url und den Typ des Dokuments.</span><span class="sxs-lookup"><span data-stu-id="94596-134">Reference properties of the trending document, such as the url and type of the document.</span></span> |

## <a name="relationships"></a><span data-ttu-id="94596-135">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="94596-135">Relationships</span></span>

| <span data-ttu-id="94596-136">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="94596-136">Property</span></span>      | <span data-ttu-id="94596-137">Typ</span><span class="sxs-lookup"><span data-stu-id="94596-137">Type</span></span>          | <span data-ttu-id="94596-138">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="94596-138">Description</span></span>  |
| ------------- |---------------| -------------|
| <span data-ttu-id="94596-139">resource</span><span class="sxs-lookup"><span data-stu-id="94596-139">resource</span></span>      | <span data-ttu-id="94596-140">Entität</span><span class="sxs-lookup"><span data-stu-id="94596-140">Entity</span></span>        | <span data-ttu-id="94596-141">Zum Navigieren zu dem Trend Dokument verwendet.</span><span class="sxs-lookup"><span data-stu-id="94596-141">Used for navigating to the trending document.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="94596-142">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="94596-142">JSON representation</span></span>

<span data-ttu-id="94596-143">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="94596-143">Here is a JSON representation of the resource</span></span>

```json
{
  "id": "string",
  "weight": "double",
  "resourceVisualization": [{"@odata.type": "microsoft.graph.resourceVisualization"}],
  "resourceReference": [{"@odata.type": "microsoft.graph.resourceReference"}],
  
  "resource": [ { "@odata.type": "microsoft.graph.entity" } ]
}
```