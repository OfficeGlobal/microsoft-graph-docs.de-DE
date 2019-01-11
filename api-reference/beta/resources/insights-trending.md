---
title: Trend Ressourcentyp
description: Rich-Beziehung Herstellen einer Verbindung mit einem Benutzer Dokumente, die auf den Benutzer (für den Benutzer relevant sind) Trend sind. OneDrive-Dateien, und um die Benutzer können Dateien, die auf SharePoint-Teamwebsites trend.
author: simonhult
localization_priority: Normal
ms.openlocfilehash: dc0154d3985e5f6e1e4770bb7d10bc727a0eb0ae
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27862384"
---
# <a name="trending-resource-type"></a><span data-ttu-id="d2769-104">Trend Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="d2769-104">trending resource type</span></span>

> <span data-ttu-id="d2769-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="d2769-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d2769-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d2769-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d2769-107">Rich-Beziehung Herstellen einer Verbindung mit einem Benutzer Dokumente, die auf den Benutzer (für den Benutzer relevant sind) Trend sind.</span><span class="sxs-lookup"><span data-stu-id="d2769-107">Rich relationship connecting a user to documents that are trending around the user (are relevant to the user).</span></span> <span data-ttu-id="d2769-108">OneDrive-Dateien, und um die Benutzer können Dateien, die auf SharePoint-Teamwebsites trend.</span><span class="sxs-lookup"><span data-stu-id="d2769-108">OneDrive files, and files stored on SharePoint team sites can trend around the user.</span></span>

## <a name="methods"></a><span data-ttu-id="d2769-109">Methoden</span><span class="sxs-lookup"><span data-stu-id="d2769-109">Methods</span></span>

| <span data-ttu-id="d2769-110">Methode</span><span class="sxs-lookup"><span data-stu-id="d2769-110">Method</span></span>       | <span data-ttu-id="d2769-111">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="d2769-111">Return Type</span></span>  |<span data-ttu-id="d2769-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d2769-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d2769-113">Liste Trend</span><span class="sxs-lookup"><span data-stu-id="d2769-113">List trending</span></span>](../api/insights-list-trending.md) |<span data-ttu-id="d2769-114">[Insights_trending](insights-trending.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="d2769-114">[insights_trending](insights-trending.md) collection</span></span>| <span data-ttu-id="d2769-115">Abrufen einer Liste von Trend-Dateien.</span><span class="sxs-lookup"><span data-stu-id="d2769-115">Get a list of trending files.</span></span>|

## <a name="properties"></a><span data-ttu-id="d2769-116">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d2769-116">Properties</span></span>

| <span data-ttu-id="d2769-117">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d2769-117">Property</span></span>      | <span data-ttu-id="d2769-118">Typ</span><span class="sxs-lookup"><span data-stu-id="d2769-118">Type</span></span>                              | <span data-ttu-id="d2769-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d2769-119">Description</span></span>  |
| ------------- |---------------                    | -------------|
| <span data-ttu-id="d2769-120">id</span><span class="sxs-lookup"><span data-stu-id="d2769-120">id</span></span>                    | <span data-ttu-id="d2769-121">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d2769-121">String</span></span>                    | <span data-ttu-id="d2769-122">Eindeutiger Bezeichner der Beziehung.</span><span class="sxs-lookup"><span data-stu-id="d2769-122">Unique identifier of the relationship.</span></span> <span data-ttu-id="d2769-123">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d2769-123">Read only.</span></span>        |
| <span data-ttu-id="d2769-124">weight</span><span class="sxs-lookup"><span data-stu-id="d2769-124">weight</span></span>                | <span data-ttu-id="d2769-125">Gleitkommawert mit doppelter Genauigkeit</span><span class="sxs-lookup"><span data-stu-id="d2769-125">Double</span></span>                    | <span data-ttu-id="d2769-126">Der Wert, der angibt, wie viel das Dokument aktuell Trend ist.</span><span class="sxs-lookup"><span data-stu-id="d2769-126">Value indicating how much the document is currently trending.</span></span> <span data-ttu-id="d2769-127">Je höher die Zahl ist, desto das Dokument ist derzeit Trend um den Benutzer (aussagekräftiger ist es).</span><span class="sxs-lookup"><span data-stu-id="d2769-127">The larger the number, the more the document is currently trending around the user (the more relevant it is).</span></span> <span data-ttu-id="d2769-128">Zurückgegebene Dokumente werden durch diesen Wert sortiert.</span><span class="sxs-lookup"><span data-stu-id="d2769-128">Returned documents are sorted by this value.</span></span>  |
| <span data-ttu-id="d2769-129">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="d2769-129">resourceVisualization</span></span> | [<span data-ttu-id="d2769-130">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="d2769-130">resourceVisualization</span></span>](insights-resourcevisualization.md)    | <span data-ttu-id="d2769-131">Eigenschaften, die Sie verwenden können, um das Dokument in Ihre Erfahrung visualisieren.</span><span class="sxs-lookup"><span data-stu-id="d2769-131">Properties that you can use to visualize the document in your experience.</span></span> |
| <span data-ttu-id="d2769-132">resourceReference</span><span class="sxs-lookup"><span data-stu-id="d2769-132">resourceReference</span></span>     | [<span data-ttu-id="d2769-133">resourceReference</span><span class="sxs-lookup"><span data-stu-id="d2769-133">resourceReference</span></span>](insights-resourcereference.md)        | <span data-ttu-id="d2769-134">Referenz-Eigenschaften des Dokuments Trend, wie die Url und den Typ des Dokuments.</span><span class="sxs-lookup"><span data-stu-id="d2769-134">Reference properties of the trending document, such as the url and type of the document.</span></span> |

## <a name="relationships"></a><span data-ttu-id="d2769-135">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="d2769-135">Relationships</span></span>

| <span data-ttu-id="d2769-136">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d2769-136">Property</span></span>      | <span data-ttu-id="d2769-137">Typ</span><span class="sxs-lookup"><span data-stu-id="d2769-137">Type</span></span>          | <span data-ttu-id="d2769-138">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d2769-138">Description</span></span>  |
| ------------- |---------------| -------------|
| <span data-ttu-id="d2769-139">resource</span><span class="sxs-lookup"><span data-stu-id="d2769-139">resource</span></span>      | <span data-ttu-id="d2769-140">Entität</span><span class="sxs-lookup"><span data-stu-id="d2769-140">Entity</span></span>        | <span data-ttu-id="d2769-141">Zum Navigieren zu dem Trend Dokument verwendet.</span><span class="sxs-lookup"><span data-stu-id="d2769-141">Used for navigating to the trending document.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d2769-142">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d2769-142">JSON representation</span></span>

<span data-ttu-id="d2769-143">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d2769-143">Here is a JSON representation of the resource</span></span>

```json
{
  "id": "string",
  "weight": "double",
  "resourceVisualization": [{"@odata.type": "microsoft.graph.resourceVisualization"}],
  "resourceReference": [{"@odata.type": "microsoft.graph.resourceReference"}],
  
  "resource": [ { "@odata.type": "microsoft.graph.entity" } ]
}
```
