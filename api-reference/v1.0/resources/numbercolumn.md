---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: NumberColumn
localization_priority: Normal
ms.openlocfilehash: 42824275bd79f4b631d53365997d2dd96984f7b5
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2019
ms.locfileid: "30480852"
---
# <a name="numbercolumn-resource-type"></a><span data-ttu-id="04796-102">NumberColumn-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="04796-102">NumberColumn resource type</span></span>

<span data-ttu-id="04796-103">Die **numberColumn** einer [columnDefinition](columndefinition.md)-Ressource gibt an, dass es sich bei den Spaltenwerten um Zahlen handelt.</span><span class="sxs-lookup"><span data-stu-id="04796-103">The **numberColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are numbers.</span></span>

## <a name="json-representation"></a><span data-ttu-id="04796-104">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="04796-104">JSON representation</span></span>

<span data-ttu-id="04796-105">Es folgt eine JSON-Darstellung einer **numberColumn**-Ressource.</span><span class="sxs-lookup"><span data-stu-id="04796-105">Here is a JSON representation of a **numberColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.numberColumn" } -->

```json
{
  "decimalPlaces": "automatic | none | one | two | three | four | five",
  "displayAs": "number | percentage",
  "maximum": 10.551,
  "minimum": 99.993
}
```

## <a name="properties"></a><span data-ttu-id="04796-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="04796-106">Properties</span></span>

| <span data-ttu-id="04796-107">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="04796-107">Property name</span></span>      | <span data-ttu-id="04796-108">Typ</span><span class="sxs-lookup"><span data-stu-id="04796-108">Type</span></span>   | <span data-ttu-id="04796-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="04796-109">Description</span></span>
|:-------------------|:-------|:-----------------------------------------------
| <span data-ttu-id="04796-110">**decimalPlaces**</span><span class="sxs-lookup"><span data-stu-id="04796-110">**decimalPlaces**</span></span>  | <span data-ttu-id="04796-111">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="04796-111">string</span></span> | <span data-ttu-id="04796-112">Wie viele Dezimalstellen angezeigt werden sollen.</span><span class="sxs-lookup"><span data-stu-id="04796-112">How many decimal places to display.</span></span> <span data-ttu-id="04796-113">Informationen zu den möglichen Werten finden Sie weiter unten.</span><span class="sxs-lookup"><span data-stu-id="04796-113">See below for information about the possible values.</span></span>
| <span data-ttu-id="04796-114">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="04796-114">**displayAs**</span></span>      | <span data-ttu-id="04796-115">string</span><span class="sxs-lookup"><span data-stu-id="04796-115">string</span></span> | <span data-ttu-id="04796-116">Wie sollte der Wert in der UX dargestellt werden.</span><span class="sxs-lookup"><span data-stu-id="04796-116">How the value should be presented in the UX.</span></span> <span data-ttu-id="04796-117">Müssen `number` oder `percentage` sein.</span><span class="sxs-lookup"><span data-stu-id="04796-117">Must be one of `number` or `percentage`.</span></span> <span data-ttu-id="04796-118">Wenn nicht angegeben, werden sie als `number` behandelt.</span><span class="sxs-lookup"><span data-stu-id="04796-118">If unspecified, treated as `number`.</span></span>
| <span data-ttu-id="04796-119">**maximum**</span><span class="sxs-lookup"><span data-stu-id="04796-119">**maximum**</span></span>        | <span data-ttu-id="04796-120">double</span><span class="sxs-lookup"><span data-stu-id="04796-120">double</span></span> | <span data-ttu-id="04796-121">Der maximal zulässige Wert.</span><span class="sxs-lookup"><span data-stu-id="04796-121">The maximum permitted value.</span></span>
| <span data-ttu-id="04796-122">**minimum**</span><span class="sxs-lookup"><span data-stu-id="04796-122">**minimum**</span></span>        | <span data-ttu-id="04796-123">double</span><span class="sxs-lookup"><span data-stu-id="04796-123">double</span></span> | <span data-ttu-id="04796-124">Der minimal zulässige Wert.</span><span class="sxs-lookup"><span data-stu-id="04796-124">The minimum permitted value.</span></span>

## <a name="decimalplaces"></a><span data-ttu-id="04796-125">DecimalPlaces</span><span class="sxs-lookup"><span data-stu-id="04796-125">DecimalPlaces</span></span>

| <span data-ttu-id="04796-126">Wert</span><span class="sxs-lookup"><span data-stu-id="04796-126">Value</span></span>          | <span data-ttu-id="04796-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="04796-127">Description</span></span>
|:---------------|:--------------------------------------------------------------
| <span data-ttu-id="04796-128">**automatic**</span><span class="sxs-lookup"><span data-stu-id="04796-128">**automatic**</span></span>  | <span data-ttu-id="04796-129">Standard.</span><span class="sxs-lookup"><span data-stu-id="04796-129">Default.</span></span> <span data-ttu-id="04796-130">Dezimalstellen werden je nach Bedarf automatisch angezeigt.</span><span class="sxs-lookup"><span data-stu-id="04796-130">Automatically display decimal places as needed.</span></span>
| <span data-ttu-id="04796-131">**none**</span><span class="sxs-lookup"><span data-stu-id="04796-131">**none**</span></span>       | <span data-ttu-id="04796-132">Keine Dezimalstellen anzuzeigen.</span><span class="sxs-lookup"><span data-stu-id="04796-132">Do not display any decimal places.</span></span>
| <span data-ttu-id="04796-133">**one**</span><span class="sxs-lookup"><span data-stu-id="04796-133">**one**</span></span>        | <span data-ttu-id="04796-134">Immer eine Dezimalstelle anzeigen.</span><span class="sxs-lookup"><span data-stu-id="04796-134">Always display one decimal place.</span></span>
| <span data-ttu-id="04796-135">**two**</span><span class="sxs-lookup"><span data-stu-id="04796-135">**two**</span></span>        | <span data-ttu-id="04796-136">Immer zwei Dezimalstellen anzeigen.</span><span class="sxs-lookup"><span data-stu-id="04796-136">Always display two decimal places.</span></span>
| <span data-ttu-id="04796-137">**three**</span><span class="sxs-lookup"><span data-stu-id="04796-137">**three**</span></span>      | <span data-ttu-id="04796-138">Immer drei Dezimalstellen anzeigen.</span><span class="sxs-lookup"><span data-stu-id="04796-138">Always display three decimal places.</span></span>
| <span data-ttu-id="04796-139">**four**</span><span class="sxs-lookup"><span data-stu-id="04796-139">**four**</span></span>       | <span data-ttu-id="04796-140">Immer vier Dezimalstellen anzeigen.</span><span class="sxs-lookup"><span data-stu-id="04796-140">Always display four decimal places.</span></span>
| <span data-ttu-id="04796-141">**five**</span><span class="sxs-lookup"><span data-stu-id="04796-141">**five**</span></span>       | <span data-ttu-id="04796-142">Immer füng Dezimalstellen anzeigen.</span><span class="sxs-lookup"><span data-stu-id="04796-142">Always display five decimal places.</span></span>

<span data-ttu-id="04796-143">Hinweis: **decimalPlaces** und **displayAs** trifft darauf zu, wie Zahlen gerendert, nicht gespeichert werden.</span><span class="sxs-lookup"><span data-stu-id="04796-143">Note: **decimalPlaces** and **displayAs** apply to how numbers are rendered, not stored.</span></span>
<span data-ttu-id="04796-144">Diese Eigenschaften können aktualisiert werden.</span><span class="sxs-lookup"><span data-stu-id="04796-144">These properties may be updated.</span></span>

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
