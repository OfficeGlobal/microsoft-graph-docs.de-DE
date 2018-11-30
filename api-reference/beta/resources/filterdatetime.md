---
title: FilterDatetime-Ressourcentyp
description: Stellt dar, wie ein Datum beim Filtern nach Werten gefiltert wird.
ms.openlocfilehash: d3cb0df48a1116a64a72413aa64cabdec46da6d9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062335"
---
# <a name="filterdatetime-resource-type"></a><span data-ttu-id="51cbb-103">FilterDatetime-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="51cbb-103">FilterDatetime resource type</span></span>

> <span data-ttu-id="51cbb-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="51cbb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="51cbb-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="51cbb-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="51cbb-106">Stellt dar, wie ein Datum beim Filtern nach Werten gefiltert wird.</span><span class="sxs-lookup"><span data-stu-id="51cbb-106">Represents how to filter a date when filtering on values.</span></span>

## <a name="properties"></a><span data-ttu-id="51cbb-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="51cbb-107">Properties</span></span>
| <span data-ttu-id="51cbb-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="51cbb-108">Property</span></span>     | <span data-ttu-id="51cbb-109">Typ</span><span class="sxs-lookup"><span data-stu-id="51cbb-109">Type</span></span>   |<span data-ttu-id="51cbb-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="51cbb-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="51cbb-111">date</span><span class="sxs-lookup"><span data-stu-id="51cbb-111">date</span></span>|<span data-ttu-id="51cbb-112">string</span><span class="sxs-lookup"><span data-stu-id="51cbb-112">string</span></span>|<span data-ttu-id="51cbb-113">Das Datum im ISO8601-Format zum Filtern von Daten.</span><span class="sxs-lookup"><span data-stu-id="51cbb-113">The date in ISO8601 format used to filter data.</span></span>|
|<span data-ttu-id="51cbb-114">specificity</span><span class="sxs-lookup"><span data-stu-id="51cbb-114">specificity</span></span>|<span data-ttu-id="51cbb-115">string</span><span class="sxs-lookup"><span data-stu-id="51cbb-115">string</span></span>|<span data-ttu-id="51cbb-p102">Genauigkeit des Datums zum Beibehalten von Daten. Wenn z. B. das Datum 2005-04-02 ist und die Spezifität auf „Monat“ festgelegt ist, werden beim Filtervorgang alle Zeilen mit einem Datum im Monat April 2009 beibehalten. Mögliche Werte:`Year`, `Monday`, `Day`, `Hour`, `Minute`, `Second`.</span><span class="sxs-lookup"><span data-stu-id="51cbb-p102">How specific the date should be used to keep data. For example, if the date is 2005-04-02 and the specifity is set to "month", the filter operation will keep all rows with a date in the month of april 2009. Possible values are: `Year`, `Monday`, `Day`, `Hour`, `Minute`, `Second`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="51cbb-119">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="51cbb-119">Relationships</span></span>
<span data-ttu-id="51cbb-120">Keine</span><span class="sxs-lookup"><span data-stu-id="51cbb-120">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="51cbb-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="51cbb-121">JSON representation</span></span>

<span data-ttu-id="51cbb-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="51cbb-122">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "FilterDatetime resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->