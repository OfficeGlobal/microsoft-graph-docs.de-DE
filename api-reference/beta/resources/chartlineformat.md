---
title: ChartLineFormat-Ressourcentyp
description: Kapselt die Formatierungsoptionen für Linienelemente.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: b4409eb18dab41d43adc038b702a65fa8d63e4de
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517932"
---
# <a name="chartlineformat-resource-type"></a><span data-ttu-id="08f33-103">ChartLineFormat-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="08f33-103">ChartLineFormat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="08f33-104">Kapselt die Formatierungsoptionen für Linienelemente.</span><span class="sxs-lookup"><span data-stu-id="08f33-104">Enapsulates the formatting options for line elements.</span></span>


## <a name="methods"></a><span data-ttu-id="08f33-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="08f33-105">Methods</span></span>

| <span data-ttu-id="08f33-106">Methode</span><span class="sxs-lookup"><span data-stu-id="08f33-106">Method</span></span>           | <span data-ttu-id="08f33-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="08f33-107">Return Type</span></span>    |<span data-ttu-id="08f33-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="08f33-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="08f33-109">ChartLineFormat abrufen</span><span class="sxs-lookup"><span data-stu-id="08f33-109">[Get ChartLineFormat](../api/chartlineformat-get.md)</span></span> | <span data-ttu-id="08f33-110">ChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="08f33-110">[ChartLineFormat](chartlineformat.md)</span></span> |<span data-ttu-id="08f33-111">Dient zum Lesen der Eigenschaften und Beziehungen eines chartLineFormat-Objekts.</span><span class="sxs-lookup"><span data-stu-id="08f33-111">Read properties and relationships of chartLineFormat object.</span></span>|
|[<span data-ttu-id="08f33-112">Update</span><span class="sxs-lookup"><span data-stu-id="08f33-112">Update</span></span>](../api/chartlineformat-update.md) | <span data-ttu-id="08f33-113">ChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="08f33-113">[ChartLineFormat](chartlineformat.md)</span></span> |<span data-ttu-id="08f33-114">Dient zum Aktualisieren des ChartLineFormat-Objekts.</span><span class="sxs-lookup"><span data-stu-id="08f33-114">Update ChartLineFormat object.</span></span> |
|[<span data-ttu-id="08f33-115">Clear</span><span class="sxs-lookup"><span data-stu-id="08f33-115">Clear</span></span>](../api/chartlineformat-clear.md)|<span data-ttu-id="08f33-116">Keine</span><span class="sxs-lookup"><span data-stu-id="08f33-116">None</span></span>|<span data-ttu-id="08f33-117">Löschen der Linienformatierung eines Diagrammelements.</span><span class="sxs-lookup"><span data-stu-id="08f33-117">Clear the line format of a chart element.</span></span>|

## <a name="properties"></a><span data-ttu-id="08f33-118">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="08f33-118">Properties</span></span>
| <span data-ttu-id="08f33-119">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="08f33-119">Property</span></span>     | <span data-ttu-id="08f33-120">Typ</span><span class="sxs-lookup"><span data-stu-id="08f33-120">Type</span></span>   |<span data-ttu-id="08f33-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="08f33-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="08f33-122">color</span><span class="sxs-lookup"><span data-stu-id="08f33-122">color</span></span>|<span data-ttu-id="08f33-123">string</span><span class="sxs-lookup"><span data-stu-id="08f33-123">string</span></span>|<span data-ttu-id="08f33-124">HTML-Farbcode, der die Farbe der Linien im Diagramm darstellt.</span><span class="sxs-lookup"><span data-stu-id="08f33-124">HTML color code representing the color of lines in the chart.</span></span>|

## <a name="relationships"></a><span data-ttu-id="08f33-125">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="08f33-125">Relationships</span></span>
<span data-ttu-id="08f33-126">Keine</span><span class="sxs-lookup"><span data-stu-id="08f33-126">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="08f33-127">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="08f33-127">JSON representation</span></span>

<span data-ttu-id="08f33-128">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="08f33-128">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chartLineFormat"
}-->

```json
{
  "color": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "ChartLineFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chartlineformat.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
