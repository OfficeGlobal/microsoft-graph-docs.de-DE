---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: NumberColumn
ms.openlocfilehash: 3bc5ef0c2764fc941959a69ae58402ce3717e7b3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27019279"
---
# <a name="numbercolumn-resource-type"></a><span data-ttu-id="83134-102">NumberColumn-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="83134-102">NumberColumn resource type</span></span>

<span data-ttu-id="83134-103">Die **numberColumn** einer [columnDefinition](columndefinition.md)-Ressource gibt an, dass es sich bei den Spaltenwerten um Zahlen handelt.</span><span class="sxs-lookup"><span data-stu-id="83134-103">The **numberColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are numbers.</span></span>

## <a name="json-representation"></a><span data-ttu-id="83134-104">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="83134-104">JSON representation</span></span>

<span data-ttu-id="83134-105">Es folgt eine JSON-Darstellung einer **numberColumn**-Ressource.</span><span class="sxs-lookup"><span data-stu-id="83134-105">Here is a JSON representation of a **numberColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.numberColumn" } -->

```json
{
  "decimalPlaces": "automatic | none | one | two | three | four | five",
  "displayAs": "number | percentage",
  "maximum": 10.551,
  "minimum": 99.993
}
```

## <a name="properties"></a><span data-ttu-id="83134-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="83134-106">Properties</span></span>

| <span data-ttu-id="83134-107">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="83134-107">Property name</span></span>      | <span data-ttu-id="83134-108">Typ</span><span class="sxs-lookup"><span data-stu-id="83134-108">Type</span></span>   | <span data-ttu-id="83134-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="83134-109">Description</span></span>
|:-------------------|:-------|:-----------------------------------------------
| <span data-ttu-id="83134-110">**decimalPlaces**</span><span class="sxs-lookup"><span data-stu-id="83134-110">**decimalPlaces**</span></span>  | <span data-ttu-id="83134-111">string</span><span class="sxs-lookup"><span data-stu-id="83134-111">string</span></span> | <span data-ttu-id="83134-112">Wie viele Dezimalstellen angezeigt werden sollen.</span><span class="sxs-lookup"><span data-stu-id="83134-112">How many decimal places to display.</span></span> <span data-ttu-id="83134-113">Informationen zu den möglichen Werten finden Sie weiter unten.</span><span class="sxs-lookup"><span data-stu-id="83134-113">See below for information about the possible values.</span></span>
| <span data-ttu-id="83134-114">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="83134-114">**displayAs**</span></span>      | <span data-ttu-id="83134-115">string</span><span class="sxs-lookup"><span data-stu-id="83134-115">string</span></span> | <span data-ttu-id="83134-116">Wie sollte der Wert in der UX dargestellt werden.</span><span class="sxs-lookup"><span data-stu-id="83134-116">How the value should be presented in the UX.</span></span> <span data-ttu-id="83134-117">Müssen `number` oder `percentage` sein.</span><span class="sxs-lookup"><span data-stu-id="83134-117">Must be one of `number` or `percentage`.</span></span> <span data-ttu-id="83134-118">Wenn nicht angegeben, werden sie als `number` behandelt.</span><span class="sxs-lookup"><span data-stu-id="83134-118">If unspecified, treated as `number`.</span></span>
| <span data-ttu-id="83134-119">**maximum**</span><span class="sxs-lookup"><span data-stu-id="83134-119">**maximum**</span></span>        | <span data-ttu-id="83134-120">double</span><span class="sxs-lookup"><span data-stu-id="83134-120">double</span></span> | <span data-ttu-id="83134-121">Der maximal zulässige Wert.</span><span class="sxs-lookup"><span data-stu-id="83134-121">The maximum permitted value.</span></span>
| <span data-ttu-id="83134-122">**minimum**</span><span class="sxs-lookup"><span data-stu-id="83134-122">**minimum**</span></span>        | <span data-ttu-id="83134-123">double</span><span class="sxs-lookup"><span data-stu-id="83134-123">double</span></span> | <span data-ttu-id="83134-124">Der minimal zulässige Wert.</span><span class="sxs-lookup"><span data-stu-id="83134-124">The minimum permitted value.</span></span>

## <a name="decimalplaces"></a><span data-ttu-id="83134-125">DecimalPlaces</span><span class="sxs-lookup"><span data-stu-id="83134-125">DecimalPlaces</span></span>

| <span data-ttu-id="83134-126">Wert</span><span class="sxs-lookup"><span data-stu-id="83134-126">Value</span></span>          | <span data-ttu-id="83134-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="83134-127">Description</span></span>
|:---------------|:--------------------------------------------------------------
| <span data-ttu-id="83134-128">**automatic**</span><span class="sxs-lookup"><span data-stu-id="83134-128">**automatic**</span></span>  | <span data-ttu-id="83134-129">Standard.</span><span class="sxs-lookup"><span data-stu-id="83134-129">Default.</span></span> <span data-ttu-id="83134-130">Dezimalstellen werden je nach Bedarf automatisch angezeigt.</span><span class="sxs-lookup"><span data-stu-id="83134-130">Automatically display decimal places as needed.</span></span>
| <span data-ttu-id="83134-131">**none**</span><span class="sxs-lookup"><span data-stu-id="83134-131">**none**</span></span>       | <span data-ttu-id="83134-132">Keine Dezimalstellen anzuzeigen.</span><span class="sxs-lookup"><span data-stu-id="83134-132">Do not display any decimal places.</span></span>
| <span data-ttu-id="83134-133">**one**</span><span class="sxs-lookup"><span data-stu-id="83134-133">**one**</span></span>        | <span data-ttu-id="83134-134">Immer eine Dezimalstelle anzeigen.</span><span class="sxs-lookup"><span data-stu-id="83134-134">Always display one decimal place.</span></span>
| <span data-ttu-id="83134-135">**two**</span><span class="sxs-lookup"><span data-stu-id="83134-135">**two**</span></span>        | <span data-ttu-id="83134-136">Immer zwei Dezimalstellen anzeigen.</span><span class="sxs-lookup"><span data-stu-id="83134-136">Always display two decimal places.</span></span>
| <span data-ttu-id="83134-137">**three**</span><span class="sxs-lookup"><span data-stu-id="83134-137">**three**</span></span>      | <span data-ttu-id="83134-138">Immer drei Dezimalstellen anzeigen.</span><span class="sxs-lookup"><span data-stu-id="83134-138">Always display three decimal places.</span></span>
| <span data-ttu-id="83134-139">**four**</span><span class="sxs-lookup"><span data-stu-id="83134-139">**four**</span></span>       | <span data-ttu-id="83134-140">Immer vier Dezimalstellen anzeigen.</span><span class="sxs-lookup"><span data-stu-id="83134-140">Always display four decimal places.</span></span>
| <span data-ttu-id="83134-141">**five**</span><span class="sxs-lookup"><span data-stu-id="83134-141">**five**</span></span>       | <span data-ttu-id="83134-142">Immer füng Dezimalstellen anzeigen.</span><span class="sxs-lookup"><span data-stu-id="83134-142">Always display five decimal places.</span></span>

<span data-ttu-id="83134-143">Hinweis: **decimalPlaces** und **displayAs** trifft darauf zu, wie Zahlen gerendert, nicht gespeichert werden.</span><span class="sxs-lookup"><span data-stu-id="83134-143">Note: **decimalPlaces** and **displayAs** apply to how numbers are rendered, not stored.</span></span>
<span data-ttu-id="83134-144">Diese Eigenschaften können aktualisiert werden.</span><span class="sxs-lookup"><span data-stu-id="83134-144">These properties may be updated.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/numbercolumn.md:
      Found potential enums in resource example that weren't defined in a table:(automatic,none,one,two,three,four,five) are in resource, but () are in table",
    "Warning: /api-reference/v1.0/resources/numbercolumn.md:
      Found potential enums in resource example that weren't defined in a table:(number,percentage) are in resource, but () are in table"
  ],
  "tocPath": "Resources/NumberColumn"
} -->
