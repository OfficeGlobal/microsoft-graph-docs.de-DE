---
title: FilterDatetime-Ressourcentyp
description: Stellt dar, wie ein Datum beim Filtern nach Werten gefiltert wird.
ms.openlocfilehash: 8156b9f5779dd8d70ff3a839d8a6ef4f5753bacd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016155"
---
# <a name="filterdatetime-resource-type"></a><span data-ttu-id="08507-103">FilterDatetime-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="08507-103">FilterDatetime resource type</span></span>

<span data-ttu-id="08507-104">Stellt dar, wie ein Datum beim Filtern nach Werten gefiltert wird.</span><span class="sxs-lookup"><span data-stu-id="08507-104">Represents how to filter a date when filtering on values.</span></span>

## <a name="properties"></a><span data-ttu-id="08507-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="08507-105">Properties</span></span>
| <span data-ttu-id="08507-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="08507-106">Property</span></span>     | <span data-ttu-id="08507-107">Typ</span><span class="sxs-lookup"><span data-stu-id="08507-107">Type</span></span>   |<span data-ttu-id="08507-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="08507-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="08507-109">date</span><span class="sxs-lookup"><span data-stu-id="08507-109">date</span></span>|<span data-ttu-id="08507-110">string</span><span class="sxs-lookup"><span data-stu-id="08507-110">string</span></span>|<span data-ttu-id="08507-111">Das Datum im ISO8601-Format zum Filtern von Daten.</span><span class="sxs-lookup"><span data-stu-id="08507-111">The date in ISO8601 format used to filter data.</span></span>|
|<span data-ttu-id="08507-112">specificity</span><span class="sxs-lookup"><span data-stu-id="08507-112">specificity</span></span>|<span data-ttu-id="08507-113">string</span><span class="sxs-lookup"><span data-stu-id="08507-113">string</span></span>|<span data-ttu-id="08507-114">Wie bestimmte das Datum verwendet werden soll, Daten zu halten.</span><span class="sxs-lookup"><span data-stu-id="08507-114">How specific the date should be used to keep data.</span></span> <span data-ttu-id="08507-115">Angenommen, wenn das Datum 2005-04-02 ist und die Spezifität auf "Month" festgelegt wird, bleiben Filteroperation alle Zeilen mit einem Datum im Monat April 2009.</span><span class="sxs-lookup"><span data-stu-id="08507-115">For example, if the date is 2005-04-02 and the specifity is set to "month", the filter operation will keep all rows with a date in the month of april 2009.</span></span> <span data-ttu-id="08507-116">Die möglichen Werte sind: `Year`, `Monday`, `Day`, `Hour`, `Minute`, `Second`.</span><span class="sxs-lookup"><span data-stu-id="08507-116">The possible values are: `Year`, `Monday`, `Day`, `Hour`, `Minute`, `Second`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="08507-117">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="08507-117">Relationships</span></span>
<span data-ttu-id="08507-118">Keine</span><span class="sxs-lookup"><span data-stu-id="08507-118">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="08507-119">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="08507-119">JSON representation</span></span>

<span data-ttu-id="08507-120">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="08507-120">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookFilterDateTime"
}-->

```json
{
  "date": "string",
  "specificity": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "FilterDatetime resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->