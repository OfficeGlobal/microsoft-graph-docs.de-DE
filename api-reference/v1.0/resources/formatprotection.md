---
title: FormatProtection-Ressourcentyp
description: Stellt den Formatschutz eines Bereichsobjekts dar.
localization_priority: Normal
ms.openlocfilehash: e4c32c8be8f6ef3aeaaf763ee88998bcbe235503
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876776"
---
# <a name="formatprotection-resource-type"></a><span data-ttu-id="ae1a9-103">FormatProtection-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="ae1a9-103">FormatProtection resource type</span></span>

<span data-ttu-id="ae1a9-104">Stellt den Formatschutz eines Bereichsobjekts dar.</span><span class="sxs-lookup"><span data-stu-id="ae1a9-104">Represents the format protection of a range object.</span></span>


## <a name="methods"></a><span data-ttu-id="ae1a9-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="ae1a9-105">Methods</span></span>

| <span data-ttu-id="ae1a9-106">Methode</span><span class="sxs-lookup"><span data-stu-id="ae1a9-106">Method</span></span>           | <span data-ttu-id="ae1a9-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="ae1a9-107">Return Type</span></span>    |<span data-ttu-id="ae1a9-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ae1a9-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ae1a9-109">FormatProtection abrufen</span><span class="sxs-lookup"><span data-stu-id="ae1a9-109">Get FormatProtection</span></span>](../api/formatprotection-get.md) | [<span data-ttu-id="ae1a9-110">FormatProtection</span><span class="sxs-lookup"><span data-stu-id="ae1a9-110">FormatProtection</span></span>](formatprotection.md) |<span data-ttu-id="ae1a9-111">Dient zum Lesen der Eigenschaften und der Beziehungen des formatProtection-Objekts.</span><span class="sxs-lookup"><span data-stu-id="ae1a9-111">Read properties and relationships of formatProtection object.</span></span>|
|[<span data-ttu-id="ae1a9-112">Update</span><span class="sxs-lookup"><span data-stu-id="ae1a9-112">Update</span></span>](../api/formatprotection-update.md) | [<span data-ttu-id="ae1a9-113">FormatProtection</span><span class="sxs-lookup"><span data-stu-id="ae1a9-113">FormatProtection</span></span>](formatprotection.md)  |<span data-ttu-id="ae1a9-114">Dient zum Aktualisieren des FormatProtection-Objekts.</span><span class="sxs-lookup"><span data-stu-id="ae1a9-114">Update FormatProtection object.</span></span> |

## <a name="properties"></a><span data-ttu-id="ae1a9-115">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ae1a9-115">Properties</span></span>
| <span data-ttu-id="ae1a9-116">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ae1a9-116">Property</span></span>     | <span data-ttu-id="ae1a9-117">Typ</span><span class="sxs-lookup"><span data-stu-id="ae1a9-117">Type</span></span>   |<span data-ttu-id="ae1a9-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ae1a9-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ae1a9-119">formulaHidden</span><span class="sxs-lookup"><span data-stu-id="ae1a9-119">formulaHidden</span></span>|<span data-ttu-id="ae1a9-120">boolean</span><span class="sxs-lookup"><span data-stu-id="ae1a9-120">boolean</span></span>|<span data-ttu-id="ae1a9-p101">Zeigt an, ob Excel die Formel für die Zellen im Bereich ausblendet. Ein Nullwert gibt an, dass der gesamte Bereich keine einheitliche Einstellung zur Formelausblendung hat.</span><span class="sxs-lookup"><span data-stu-id="ae1a9-p101">Indicates if Excel hides the formula for the cells in the range. A null value indicates that the entire range doesn't have uniform formula hidden setting.</span></span>|
|<span data-ttu-id="ae1a9-123">locked</span><span class="sxs-lookup"><span data-stu-id="ae1a9-123">locked</span></span>|<span data-ttu-id="ae1a9-124">boolean</span><span class="sxs-lookup"><span data-stu-id="ae1a9-124">boolean</span></span>|<span data-ttu-id="ae1a9-p102">Gibt an, ob Excel die Zellen im Objekt sperrt. Ein Nullwert gibt an, dass der gesamte Bereich keine einheitliche Einstellung zum Sperren hat.</span><span class="sxs-lookup"><span data-stu-id="ae1a9-p102">Indicates if Excel locks the cells in the object. A null value indicates that the entire range doesn't have uniform lock setting.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ae1a9-127">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="ae1a9-127">Relationships</span></span>
<span data-ttu-id="ae1a9-128">Keine</span><span class="sxs-lookup"><span data-stu-id="ae1a9-128">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="ae1a9-129">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ae1a9-129">JSON representation</span></span>

<span data-ttu-id="ae1a9-130">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="ae1a9-130">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookFormatProtection"
}-->

```json
{
  "formulaHidden": true,
  "locked": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "FormatProtection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
