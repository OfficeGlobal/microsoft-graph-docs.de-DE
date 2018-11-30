---
title: ChartGridlines-Ressourcentyp
description: Stellt Haupt-Gitternetzlinien oder Hilfs-Gitternetzlinien auf einer Diagrammachse dar.
ms.openlocfilehash: c09580b2c669710d8aabf60e31c3c36965bfaa6a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058186"
---
# <a name="chartgridlines-resource-type"></a><span data-ttu-id="de357-103">ChartGridlines-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="de357-103">ChartGridlines resource type</span></span>

> <span data-ttu-id="de357-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="de357-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="de357-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="de357-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="de357-106">Stellt Hauptgitternetzlinien oder Hilfsgitternetzlinien auf einer Diagrammachse dar.</span><span class="sxs-lookup"><span data-stu-id="de357-106">Represents major or minor gridlines on a chart axis.</span></span>


## <a name="methods"></a><span data-ttu-id="de357-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="de357-107">Methods</span></span>

| <span data-ttu-id="de357-108">Methode</span><span class="sxs-lookup"><span data-stu-id="de357-108">Method</span></span>           | <span data-ttu-id="de357-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="de357-109">Return Type</span></span>    |<span data-ttu-id="de357-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="de357-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="de357-111">ChartGridlines abrufen</span><span class="sxs-lookup"><span data-stu-id="de357-111">Get ChartGridlines</span></span>](../api/chartgridlines-get.md) | [<span data-ttu-id="de357-112">ChartGridlines</span><span class="sxs-lookup"><span data-stu-id="de357-112">ChartGridlines</span></span>](chartgridlines.md) |<span data-ttu-id="de357-113">Dient zum Lesender Eigenschaften und der Beziehungen des chartGridlines-Objekts.</span><span class="sxs-lookup"><span data-stu-id="de357-113">Read properties and relationships of chartGridlines object.</span></span>|
|[<span data-ttu-id="de357-114">Update</span><span class="sxs-lookup"><span data-stu-id="de357-114">Update</span></span>](../api/chartgridlines-update.md) | [<span data-ttu-id="de357-115">ChartGridlines</span><span class="sxs-lookup"><span data-stu-id="de357-115">ChartGridlines</span></span>](chartgridlines.md)    |<span data-ttu-id="de357-116">Dient zum Aktualisieren des ChartGridlines-Objekts.</span><span class="sxs-lookup"><span data-stu-id="de357-116">Update ChartGridlines object.</span></span> |

## <a name="properties"></a><span data-ttu-id="de357-117">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="de357-117">Properties</span></span>
| <span data-ttu-id="de357-118">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="de357-118">Property</span></span>     | <span data-ttu-id="de357-119">Typ</span><span class="sxs-lookup"><span data-stu-id="de357-119">Type</span></span>   |<span data-ttu-id="de357-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="de357-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="de357-121">visible</span><span class="sxs-lookup"><span data-stu-id="de357-121">visible</span></span>|<span data-ttu-id="de357-122">boolean</span><span class="sxs-lookup"><span data-stu-id="de357-122">boolean</span></span>|<span data-ttu-id="de357-123">Boolescher Wert, der angibt, ob die Achsengitternetzlinien angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="de357-123">Boolean value representing if the axis gridlines are visible or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="de357-124">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="de357-124">Relationships</span></span>
| <span data-ttu-id="de357-125">Beziehung</span><span class="sxs-lookup"><span data-stu-id="de357-125">Relationship</span></span> | <span data-ttu-id="de357-126">Typ</span><span class="sxs-lookup"><span data-stu-id="de357-126">Type</span></span>   |<span data-ttu-id="de357-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="de357-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="de357-128">Format</span><span class="sxs-lookup"><span data-stu-id="de357-128">format</span></span>|[<span data-ttu-id="de357-129">ChartGridlinesFormat</span><span class="sxs-lookup"><span data-stu-id="de357-129">ChartGridlinesFormat</span></span>](chartgridlinesformat.md)|<span data-ttu-id="de357-p102">Stellt die Formatierung der Diagrammgitternetzlinien dar. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="de357-p102">Represents the formatting of chart gridlines. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="de357-132">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="de357-132">JSON representation</span></span>

<span data-ttu-id="de357-133">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="de357-133">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chartGridLines"
}-->

```json
{
  "visible": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartGridlines resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->