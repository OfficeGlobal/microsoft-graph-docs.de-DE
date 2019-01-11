---
title: FormatProtection-Ressourcentyp
description: Stellt den Formatschutz eines Bereichsobjekts dar.
localization_priority: Normal
ms.openlocfilehash: 0b4add2e30a1e475adcb162903f771ce760f9285
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27805621"
---
# <a name="formatprotection-resource-type"></a><span data-ttu-id="ae75e-103">FormatProtection-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="ae75e-103">FormatProtection resource type</span></span>

> <span data-ttu-id="ae75e-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="ae75e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ae75e-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ae75e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ae75e-106">Stellt den Formatschutz eines Bereichsobjekts dar.</span><span class="sxs-lookup"><span data-stu-id="ae75e-106">Represents the format protection of a range object.</span></span>


## <a name="methods"></a><span data-ttu-id="ae75e-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="ae75e-107">Methods</span></span>

| <span data-ttu-id="ae75e-108">Methode</span><span class="sxs-lookup"><span data-stu-id="ae75e-108">Method</span></span>           | <span data-ttu-id="ae75e-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="ae75e-109">Return Type</span></span>    |<span data-ttu-id="ae75e-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ae75e-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ae75e-111">FormatProtection abrufen</span><span class="sxs-lookup"><span data-stu-id="ae75e-111">Get FormatProtection</span></span>](../api/formatprotection-get.md) | [<span data-ttu-id="ae75e-112">FormatProtection</span><span class="sxs-lookup"><span data-stu-id="ae75e-112">FormatProtection</span></span>](formatprotection.md) |<span data-ttu-id="ae75e-113">Dient zum Lesen der Eigenschaften und der Beziehungen des formatProtection-Objekts.</span><span class="sxs-lookup"><span data-stu-id="ae75e-113">Read properties and relationships of formatProtection object.</span></span>|
|[<span data-ttu-id="ae75e-114">Update</span><span class="sxs-lookup"><span data-stu-id="ae75e-114">Update</span></span>](../api/formatprotection-update.md) | [<span data-ttu-id="ae75e-115">FormatProtection</span><span class="sxs-lookup"><span data-stu-id="ae75e-115">FormatProtection</span></span>](formatprotection.md)  |<span data-ttu-id="ae75e-116">Dient zum Aktualisieren des FormatProtection-Objekts.</span><span class="sxs-lookup"><span data-stu-id="ae75e-116">Update FormatProtection object.</span></span> |

## <a name="properties"></a><span data-ttu-id="ae75e-117">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ae75e-117">Properties</span></span>
| <span data-ttu-id="ae75e-118">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ae75e-118">Property</span></span>     | <span data-ttu-id="ae75e-119">Typ</span><span class="sxs-lookup"><span data-stu-id="ae75e-119">Type</span></span>   |<span data-ttu-id="ae75e-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ae75e-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ae75e-121">formulaHidden</span><span class="sxs-lookup"><span data-stu-id="ae75e-121">formulaHidden</span></span>|<span data-ttu-id="ae75e-122">boolean</span><span class="sxs-lookup"><span data-stu-id="ae75e-122">boolean</span></span>|<span data-ttu-id="ae75e-p102">Zeigt an, ob Excel die Formel für die Zellen im Bereich ausblendet. Ein Nullwert gibt an, dass der gesamte Bereich keine einheitliche Einstellung zur Formelausblendung hat.</span><span class="sxs-lookup"><span data-stu-id="ae75e-p102">Indicates if Excel hides the formula for the cells in the range. A null value indicates that the entire range doesn't have uniform formula hidden setting.</span></span>|
|<span data-ttu-id="ae75e-125">locked</span><span class="sxs-lookup"><span data-stu-id="ae75e-125">locked</span></span>|<span data-ttu-id="ae75e-126">boolean</span><span class="sxs-lookup"><span data-stu-id="ae75e-126">boolean</span></span>|<span data-ttu-id="ae75e-p103">Gibt an, ob Excel die Zellen im Objekt sperrt. Ein Nullwert gibt an, dass der gesamte Bereich keine einheitliche Einstellung zum Sperren hat.</span><span class="sxs-lookup"><span data-stu-id="ae75e-p103">Indicates if Excel locks the cells in the object. A null value indicates that the entire range doesn't have uniform lock setting.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ae75e-129">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="ae75e-129">Relationships</span></span>
<span data-ttu-id="ae75e-130">Keine</span><span class="sxs-lookup"><span data-stu-id="ae75e-130">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="ae75e-131">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ae75e-131">JSON representation</span></span>

<span data-ttu-id="ae75e-132">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="ae75e-132">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "FormatProtection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
