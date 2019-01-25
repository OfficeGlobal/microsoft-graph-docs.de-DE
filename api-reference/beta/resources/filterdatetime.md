---
title: FilterDatetime-Ressourcentyp
description: Stellt dar, wie ein Datum beim Filtern nach Werten gefiltert wird.
localization_priority: Normal
ms.openlocfilehash: ad4341e13eadc911377ec7b9859d6a31305fadf8
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29507551"
---
# <a name="filterdatetime-resource-type"></a><span data-ttu-id="0b1f5-103">FilterDatetime-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="0b1f5-103">FilterDatetime resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0b1f5-104">Stellt dar, wie ein Datum beim Filtern nach Werten gefiltert wird.</span><span class="sxs-lookup"><span data-stu-id="0b1f5-104">Represents how to filter a date when filtering on values.</span></span>

## <a name="properties"></a><span data-ttu-id="0b1f5-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="0b1f5-105">Properties</span></span>
| <span data-ttu-id="0b1f5-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0b1f5-106">Property</span></span>     | <span data-ttu-id="0b1f5-107">Typ</span><span class="sxs-lookup"><span data-stu-id="0b1f5-107">Type</span></span>   |<span data-ttu-id="0b1f5-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0b1f5-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0b1f5-109">date</span><span class="sxs-lookup"><span data-stu-id="0b1f5-109">date</span></span>|<span data-ttu-id="0b1f5-110">string</span><span class="sxs-lookup"><span data-stu-id="0b1f5-110">string</span></span>|<span data-ttu-id="0b1f5-111">Das Datum im ISO8601-Format zum Filtern von Daten.</span><span class="sxs-lookup"><span data-stu-id="0b1f5-111">The date in ISO8601 format used to filter data.</span></span>|
|<span data-ttu-id="0b1f5-112">specificity</span><span class="sxs-lookup"><span data-stu-id="0b1f5-112">specificity</span></span>|<span data-ttu-id="0b1f5-113">string</span><span class="sxs-lookup"><span data-stu-id="0b1f5-113">string</span></span>|<span data-ttu-id="0b1f5-p101">Genauigkeit des Datums zum Beibehalten von Daten. Wenn z. B. das Datum 2005-04-02 ist und die Spezifität auf „Monat“ festgelegt ist, werden beim Filtervorgang alle Zeilen mit einem Datum im Monat April 2009 beibehalten. Mögliche Werte:`Year`, `Monday`, `Day`, `Hour`, `Minute`, `Second`.</span><span class="sxs-lookup"><span data-stu-id="0b1f5-p101">How specific the date should be used to keep data. For example, if the date is 2005-04-02 and the specifity is set to "month", the filter operation will keep all rows with a date in the month of april 2009. Possible values are: `Year`, `Monday`, `Day`, `Hour`, `Minute`, `Second`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0b1f5-117">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="0b1f5-117">Relationships</span></span>
<span data-ttu-id="0b1f5-118">Keine</span><span class="sxs-lookup"><span data-stu-id="0b1f5-118">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="0b1f5-119">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="0b1f5-119">JSON representation</span></span>

<span data-ttu-id="0b1f5-120">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="0b1f5-120">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.filterDateTime"
}-->

```json
{
  "date": "string",
  "specificity": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "FilterDatetime resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/filterdatetime.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
