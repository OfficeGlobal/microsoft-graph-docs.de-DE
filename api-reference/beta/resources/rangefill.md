---
title: RangeFill-Ressourcentyp
description: Stellt den Hintergrund eines Bereichsobjekts dar.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: d1ae60c0b362ba8593f374c5edd505121cd18587
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509672"
---
# <a name="rangefill-resource-type"></a><span data-ttu-id="8e6dc-103">RangeFill-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="8e6dc-103">RangeFill resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8e6dc-104">Stellt den Hintergrund eines Bereichsobjekts dar.</span><span class="sxs-lookup"><span data-stu-id="8e6dc-104">Represents the background of a range object.</span></span>


## <a name="methods"></a><span data-ttu-id="8e6dc-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="8e6dc-105">Methods</span></span>

| <span data-ttu-id="8e6dc-106">Methode</span><span class="sxs-lookup"><span data-stu-id="8e6dc-106">Method</span></span>           | <span data-ttu-id="8e6dc-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="8e6dc-107">Return Type</span></span>    |<span data-ttu-id="8e6dc-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8e6dc-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8e6dc-109">RangeFill abrufen</span><span class="sxs-lookup"><span data-stu-id="8e6dc-109">[Get RangeFill](../api/rangefill-get.md)</span></span> | <span data-ttu-id="8e6dc-110">RangeFill</span><span class="sxs-lookup"><span data-stu-id="8e6dc-110">[RangeFill](rangefill.md)</span></span> |<span data-ttu-id="8e6dc-111">Dient zum Lesen der Eigenschaften und der Beziehungen des rangeFill-Objekts.</span><span class="sxs-lookup"><span data-stu-id="8e6dc-111">Read properties and relationships of rangeFill object.</span></span>|
|[<span data-ttu-id="8e6dc-112">Update</span><span class="sxs-lookup"><span data-stu-id="8e6dc-112">Update</span></span>](../api/rangefill-update.md) | <span data-ttu-id="8e6dc-113">RangeFill</span><span class="sxs-lookup"><span data-stu-id="8e6dc-113">[RangeFill](rangefill.md)</span></span>   |<span data-ttu-id="8e6dc-114">Dient zum Aktualisieren des RangeFill-Objekts.</span><span class="sxs-lookup"><span data-stu-id="8e6dc-114">Update RangeFill object.</span></span> |
|[<span data-ttu-id="8e6dc-115">Clear</span><span class="sxs-lookup"><span data-stu-id="8e6dc-115">Clear</span></span>](../api/rangefill-clear.md)|<span data-ttu-id="8e6dc-116">Keine</span><span class="sxs-lookup"><span data-stu-id="8e6dc-116">None</span></span>|<span data-ttu-id="8e6dc-117">Setzt den Hintergrund des Bereichs zurück.</span><span class="sxs-lookup"><span data-stu-id="8e6dc-117">Resets the range background.</span></span>|

## <a name="properties"></a><span data-ttu-id="8e6dc-118">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="8e6dc-118">Properties</span></span>
| <span data-ttu-id="8e6dc-119">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8e6dc-119">Property</span></span>     | <span data-ttu-id="8e6dc-120">Typ</span><span class="sxs-lookup"><span data-stu-id="8e6dc-120">Type</span></span>   |<span data-ttu-id="8e6dc-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8e6dc-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8e6dc-122">color</span><span class="sxs-lookup"><span data-stu-id="8e6dc-122">color</span></span>|<span data-ttu-id="8e6dc-123">string</span><span class="sxs-lookup"><span data-stu-id="8e6dc-123">string</span></span>|<span data-ttu-id="8e6dc-124">HTML-Farbcode, der die Farbe der Rahmenlinie, des Formulars #RRGGBB (z. B.  "FFA500") oder als benannte HTML-Farbe (z. B. "orange") darstellt.</span><span class="sxs-lookup"><span data-stu-id="8e6dc-124">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange")</span></span>|

## <a name="relationships"></a><span data-ttu-id="8e6dc-125">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="8e6dc-125">Relationships</span></span>
<span data-ttu-id="8e6dc-126">Keine</span><span class="sxs-lookup"><span data-stu-id="8e6dc-126">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="8e6dc-127">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="8e6dc-127">JSON representation</span></span>

<span data-ttu-id="8e6dc-128">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="8e6dc-128">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.rangeFill"
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
  "description": "RangeFill resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/rangefill.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
