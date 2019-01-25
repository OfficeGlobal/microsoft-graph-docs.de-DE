---
title: FormatProtection-Ressourcentyp
description: Stellt den Formatschutz eines Bereichsobjekts dar.
localization_priority: Normal
ms.openlocfilehash: 7bc27060567136386ef1f08e6fe46e95980788a9
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509189"
---
# <a name="formatprotection-resource-type"></a><span data-ttu-id="a429f-103">FormatProtection-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="a429f-103">FormatProtection resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a429f-104">Stellt den Formatschutz eines Bereichsobjekts dar.</span><span class="sxs-lookup"><span data-stu-id="a429f-104">Represents the format protection of a range object.</span></span>


## <a name="methods"></a><span data-ttu-id="a429f-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="a429f-105">Methods</span></span>

| <span data-ttu-id="a429f-106">Methode</span><span class="sxs-lookup"><span data-stu-id="a429f-106">Method</span></span>           | <span data-ttu-id="a429f-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="a429f-107">Return Type</span></span>    |<span data-ttu-id="a429f-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a429f-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a429f-109">FormatProtection abrufen</span><span class="sxs-lookup"><span data-stu-id="a429f-109">[Get FormatProtection](../api/formatprotection-get.md)</span></span> | [<span data-ttu-id="a429f-110">formatProtection</span><span class="sxs-lookup"><span data-stu-id="a429f-110">FormatProtection</span></span>](formatprotection.md) |<span data-ttu-id="a429f-111">Dient zum Lesen der Eigenschaften und der Beziehungen des formatProtection-Objekts.</span><span class="sxs-lookup"><span data-stu-id="a429f-111">Read properties and relationships of formatProtection object.</span></span>|
|[<span data-ttu-id="a429f-112">Update</span><span class="sxs-lookup"><span data-stu-id="a429f-112">Update</span></span>](../api/formatprotection-update.md) | <span data-ttu-id="a429f-113">FormatProtection</span><span class="sxs-lookup"><span data-stu-id="a429f-113">[FormatProtection](formatprotection.md)</span></span>  |<span data-ttu-id="a429f-114">Dient zum Aktualisieren des FormatProtection-Objekts.</span><span class="sxs-lookup"><span data-stu-id="a429f-114">Update FormatProtection object.</span></span> |

## <a name="properties"></a><span data-ttu-id="a429f-115">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="a429f-115">Properties</span></span>
| <span data-ttu-id="a429f-116">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a429f-116">Property</span></span>     | <span data-ttu-id="a429f-117">Typ</span><span class="sxs-lookup"><span data-stu-id="a429f-117">Type</span></span>   |<span data-ttu-id="a429f-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a429f-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a429f-119">formulaHidden</span><span class="sxs-lookup"><span data-stu-id="a429f-119">formulaHidden</span></span>|<span data-ttu-id="a429f-120">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="a429f-120">boolean</span></span>|<span data-ttu-id="a429f-p101">Zeigt an, ob Excel die Formel für die Zellen im Bereich ausblendet. Ein Nullwert gibt an, dass der gesamte Bereich keine einheitliche Einstellung zur Formelausblendung hat.</span><span class="sxs-lookup"><span data-stu-id="a429f-p101">Indicates if Excel hides the formula for the cells in the range. A null value indicates that the entire range doesn't have uniform formula hidden setting.</span></span>|
|<span data-ttu-id="a429f-123">locked</span><span class="sxs-lookup"><span data-stu-id="a429f-123">locked</span></span>|<span data-ttu-id="a429f-124">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="a429f-124">boolean</span></span>|<span data-ttu-id="a429f-p102">Gibt an, ob Excel die Zellen im Objekt sperrt. Ein Nullwert gibt an, dass der gesamte Bereich keine einheitliche Einstellung zum Sperren hat.</span><span class="sxs-lookup"><span data-stu-id="a429f-p102">Indicates if Excel locks the cells in the object. A null value indicates that the entire range doesn't have uniform lock setting.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a429f-127">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="a429f-127">Relationships</span></span>
<span data-ttu-id="a429f-128">Keine</span><span class="sxs-lookup"><span data-stu-id="a429f-128">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="a429f-129">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="a429f-129">JSON representation</span></span>

<span data-ttu-id="a429f-130">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="a429f-130">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.formatProtection"
}-->

```json
{
  "formulaHidden": true,
  "locked": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "FormatProtection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/formatprotection.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
