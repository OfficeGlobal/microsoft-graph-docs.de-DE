---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: NumberColumn
ms.openlocfilehash: 4aaff6539fc9c7ce77029463562c0f8fca57cac6
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/21/2018
ms.locfileid: "23266506"
---
# <a name="numbercolumn-resource-type"></a><span data-ttu-id="07c31-102">NumberColumn-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="07c31-102">NumberColumn resource type</span></span>

<span data-ttu-id="07c31-103">Die **numberColumn** einer [columnDefinition](columnDefinition.md)-Ressource gibt an, dass es sich bei den Spaltenwerten um Zahlen handelt.</span><span class="sxs-lookup"><span data-stu-id="07c31-103">The **numberColumn** on a [columnDefinition](columnDefinition.md) resource indicates that the column's values are numbers.</span></span>

## <a name="json-representation"></a><span data-ttu-id="07c31-104">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="07c31-104">JSON representation</span></span>

<span data-ttu-id="07c31-105">Es folgt eine JSON-Darstellung einer **numberColumn**-Ressource.</span><span class="sxs-lookup"><span data-stu-id="07c31-105">Here is a JSON representation of a **numberColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.numberColumn" } -->

```json
{
  "decimalPlaces": "automatic | none | one | two | three | four | five",
  "displayAs": "number | percentage",
  "maximum": 10.551,
  "minimum": 99.993
}
```

## <a name="properties"></a><span data-ttu-id="07c31-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="07c31-106">Properties</span></span>

| <span data-ttu-id="07c31-107">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="07c31-107">Property name</span></span>      | <span data-ttu-id="07c31-108">Typ</span><span class="sxs-lookup"><span data-stu-id="07c31-108">Type</span></span>   | <span data-ttu-id="07c31-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="07c31-109">Description</span></span>
|:-------------------|:-------|:-----------------------------------------------
| <span data-ttu-id="07c31-110">**decimalPlaces**</span><span class="sxs-lookup"><span data-stu-id="07c31-110">**decimalPlaces**</span></span>  | <span data-ttu-id="07c31-111">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="07c31-111">string</span></span> | <span data-ttu-id="07c31-112">Wie viele Dezimalstellen angezeigt werden sollen.</span><span class="sxs-lookup"><span data-stu-id="07c31-112">How many decimal places to display.</span></span> <span data-ttu-id="07c31-113">Informationen zu den möglichen Werten finden Sie weiter unten.</span><span class="sxs-lookup"><span data-stu-id="07c31-113">See below for information about the possible values.</span></span>
| <span data-ttu-id="07c31-114">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="07c31-114">**displayAs**</span></span>      | <span data-ttu-id="07c31-115">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="07c31-115">string</span></span> | <span data-ttu-id="07c31-116">Wie sollte der Wert in der UX dargestellt werden.</span><span class="sxs-lookup"><span data-stu-id="07c31-116">How the value should be presented in the UX.</span></span> <span data-ttu-id="07c31-117">Müssen `number` oder `percentage` sein.</span><span class="sxs-lookup"><span data-stu-id="07c31-117">Must be one of `number` or `percentage`.</span></span> <span data-ttu-id="07c31-118">Wenn nicht angegeben, werden sie als `number` behandelt.</span><span class="sxs-lookup"><span data-stu-id="07c31-118">If unspecified, treated as `number`.</span></span>
| <span data-ttu-id="07c31-119">**maximum**</span><span class="sxs-lookup"><span data-stu-id="07c31-119">**maximum**</span></span>        | <span data-ttu-id="07c31-120">doppelt</span><span class="sxs-lookup"><span data-stu-id="07c31-120">double</span></span> | <span data-ttu-id="07c31-121">Der maximal zulässige Wert.</span><span class="sxs-lookup"><span data-stu-id="07c31-121">The maximum permitted value.</span></span>
| <span data-ttu-id="07c31-122">**minimum**</span><span class="sxs-lookup"><span data-stu-id="07c31-122">**minimum**</span></span>        | <span data-ttu-id="07c31-123">doppelt</span><span class="sxs-lookup"><span data-stu-id="07c31-123">double</span></span> | <span data-ttu-id="07c31-124">Der minimal zulässige Wert.</span><span class="sxs-lookup"><span data-stu-id="07c31-124">The minimum permitted value.</span></span>

## <a name="decimalplaces"></a><span data-ttu-id="07c31-125">DecimalPlaces</span><span class="sxs-lookup"><span data-stu-id="07c31-125">decimalPlaces</span></span>

| <span data-ttu-id="07c31-126">Wert</span><span class="sxs-lookup"><span data-stu-id="07c31-126">Value</span></span>          | <span data-ttu-id="07c31-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="07c31-127">Description</span></span>
|:---------------|:--------------------------------------------------------------
| <span data-ttu-id="07c31-128">**Automatisch**</span><span class="sxs-lookup"><span data-stu-id="07c31-128">**automatic**</span></span>  | <span data-ttu-id="07c31-129">Standard.</span><span class="sxs-lookup"><span data-stu-id="07c31-129">Default.</span></span> <span data-ttu-id="07c31-130">Dezimalstellen werden je nach Bedarf automatisch angezeigt.</span><span class="sxs-lookup"><span data-stu-id="07c31-130">Automatically display decimal places as needed.</span></span>
| <span data-ttu-id="07c31-131">**keine**</span><span class="sxs-lookup"><span data-stu-id="07c31-131">**none**</span></span>       | <span data-ttu-id="07c31-132">Keine Dezimalstellen anzuzeigen.</span><span class="sxs-lookup"><span data-stu-id="07c31-132">Do not display any decimal places.</span></span>
| <span data-ttu-id="07c31-133">**eine**</span><span class="sxs-lookup"><span data-stu-id="07c31-133">**one**</span></span>        | <span data-ttu-id="07c31-134">Immer eine Dezimalstelle anzeigen.</span><span class="sxs-lookup"><span data-stu-id="07c31-134">Always display one decimal place.</span></span>
| <span data-ttu-id="07c31-135">**zwei**</span><span class="sxs-lookup"><span data-stu-id="07c31-135">**two**</span></span>        | <span data-ttu-id="07c31-136">Immer zwei Dezimalstellen anzeigen.</span><span class="sxs-lookup"><span data-stu-id="07c31-136">Always display two decimal places.</span></span>
| <span data-ttu-id="07c31-137">**drei**</span><span class="sxs-lookup"><span data-stu-id="07c31-137">**three**</span></span>      | <span data-ttu-id="07c31-138">Immer drei Dezimalstellen anzeigen.</span><span class="sxs-lookup"><span data-stu-id="07c31-138">Always display three decimal places.</span></span>
| <span data-ttu-id="07c31-139">**vier**</span><span class="sxs-lookup"><span data-stu-id="07c31-139">**four**</span></span>       | <span data-ttu-id="07c31-140">Immer vier Dezimalstellen anzeigen.</span><span class="sxs-lookup"><span data-stu-id="07c31-140">Always display four decimal places.</span></span>
| <span data-ttu-id="07c31-141">**fünf**</span><span class="sxs-lookup"><span data-stu-id="07c31-141">**five**</span></span>       | <span data-ttu-id="07c31-142">Immer füng Dezimalstellen anzeigen.</span><span class="sxs-lookup"><span data-stu-id="07c31-142">Always display five decimal places.</span></span>

<span data-ttu-id="07c31-143">Hinweis: **decimalPlaces** und **displayAs** trifft darauf zu, wie Zahlen gerendert, nicht gespeichert werden.</span><span class="sxs-lookup"><span data-stu-id="07c31-143">Note: **decimalPlaces** and **displayAs** apply to how numbers are rendered, not stored.</span></span>
<span data-ttu-id="07c31-144">Diese Eigenschaften können aktualisiert werden.</span><span class="sxs-lookup"><span data-stu-id="07c31-144">These properties may be updated.</span></span>

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
