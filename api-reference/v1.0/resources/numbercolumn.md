---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: NumberColumn
ms.openlocfilehash: 8aa366e3c4f59fc5d22f945c863bab4f91373b67
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/28/2017
---
# <a name="numbercolumn-resource-type"></a><span data-ttu-id="9be1f-102">NumberColumn-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="9be1f-102">NumberColumn resource type</span></span>

<span data-ttu-id="9be1f-103">Die **numberColumn** einer [columnDefinition](columnDefinition.md)-Ressource gibt an, dass es sich bei den Spaltenwerten um Zahlen handelt.</span><span class="sxs-lookup"><span data-stu-id="9be1f-103">The **numberColumn** on a [columnDefinition](columnDefinition.md) resource indicates that the column's values are numbers.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9be1f-104">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="9be1f-104">JSON representation</span></span>

<span data-ttu-id="9be1f-105">Es folgt eine JSON-Darstellung einer **numberColumn**-Ressource.</span><span class="sxs-lookup"><span data-stu-id="9be1f-105">Here is a JSON representation of a **drive** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.numberColumn" } -->

```json
{
  "decimalPlaces": "automatic | none | one | two | three | four | five",
  "displayAs": "number | percentage",
  "maximum": 10.551,
  "minimum": 99.993
}
```

## <a name="properties"></a><span data-ttu-id="9be1f-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="9be1f-106">Properties</span></span>

| <span data-ttu-id="9be1f-107">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="9be1f-107">Property name</span></span>      | <span data-ttu-id="9be1f-108">Typ</span><span class="sxs-lookup"><span data-stu-id="9be1f-108">Type</span></span>   | <span data-ttu-id="9be1f-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9be1f-109">Description</span></span>
|:-------------------|:-------|:-----------------------------------------------
| <span data-ttu-id="9be1f-110">**decimalPlaces**</span><span class="sxs-lookup"><span data-stu-id="9be1f-110">**DecimalPlaces**</span></span>  | <span data-ttu-id="9be1f-111">string</span><span class="sxs-lookup"><span data-stu-id="9be1f-111">string</span></span> | <span data-ttu-id="9be1f-112">Wie viele Dezimalstellen angezeigt werden sollen.</span><span class="sxs-lookup"><span data-stu-id="9be1f-112">How many decimal places to display.</span></span> <span data-ttu-id="9be1f-113">Informationen zu den möglichen Werten finden Sie weiter unten.</span><span class="sxs-lookup"><span data-stu-id="9be1f-113">See below for information about the possible values.</span></span>
| <span data-ttu-id="9be1f-114">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="9be1f-114">**displayAs**</span></span>      | <span data-ttu-id="9be1f-115">string</span><span class="sxs-lookup"><span data-stu-id="9be1f-115">string</span></span> | <span data-ttu-id="9be1f-116">Wie sollte der Wert in der UX dargestellt werden?</span><span class="sxs-lookup"><span data-stu-id="9be1f-116">How the value should be presented in the UX.</span></span> <span data-ttu-id="9be1f-117">Müssen `number` oder `percentage` sein.</span><span class="sxs-lookup"><span data-stu-id="9be1f-117">Must be one of `number` or `percentage`.</span></span> <span data-ttu-id="9be1f-118">Wenn nicht angegeben, werden sie als `number` behandelt.</span><span class="sxs-lookup"><span data-stu-id="9be1f-118">If unspecified, treated as `number`.</span></span>
| <span data-ttu-id="9be1f-119">**maximum**</span><span class="sxs-lookup"><span data-stu-id="9be1f-119">**maximum**</span></span>        | <span data-ttu-id="9be1f-120">double</span><span class="sxs-lookup"><span data-stu-id="9be1f-120">double</span></span> | <span data-ttu-id="9be1f-121">Der maximal zulässige Wert.</span><span class="sxs-lookup"><span data-stu-id="9be1f-121">The maximum permitted value.</span></span>
| <span data-ttu-id="9be1f-122">**minimum**</span><span class="sxs-lookup"><span data-stu-id="9be1f-122">**minimum**</span></span>        | <span data-ttu-id="9be1f-123">double</span><span class="sxs-lookup"><span data-stu-id="9be1f-123">double</span></span> | <span data-ttu-id="9be1f-124">Der minimal zulässige Wert.</span><span class="sxs-lookup"><span data-stu-id="9be1f-124">The minimum permitted value.</span></span>

## <a name="decimalplaces-values"></a><span data-ttu-id="9be1f-125">DecimalPlaces-Werte</span><span class="sxs-lookup"><span data-stu-id="9be1f-125">DecimalPlaces values</span></span>

| <span data-ttu-id="9be1f-126">Wert</span><span class="sxs-lookup"><span data-stu-id="9be1f-126">Value</span></span>          | <span data-ttu-id="9be1f-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9be1f-127">Description</span></span>
|:---------------|:--------------------------------------------------------------
| <span data-ttu-id="9be1f-128">**automatic**</span><span class="sxs-lookup"><span data-stu-id="9be1f-128">**Automatic**</span></span>  | <span data-ttu-id="9be1f-129">Standard.</span><span class="sxs-lookup"><span data-stu-id="9be1f-129">Default.</span></span> <span data-ttu-id="9be1f-130">Dezimalstellen werden je nach Bedarf automatisch angezeigt.</span><span class="sxs-lookup"><span data-stu-id="9be1f-130">Automatically display decimal places as needed.</span></span>
| <span data-ttu-id="9be1f-131">**none**</span><span class="sxs-lookup"><span data-stu-id="9be1f-131">**None**</span></span>       | <span data-ttu-id="9be1f-132">Keine Dezimalstellen anzuzeigen.</span><span class="sxs-lookup"><span data-stu-id="9be1f-132">Do not display any decimal places.</span></span>
| <span data-ttu-id="9be1f-133">**one**</span><span class="sxs-lookup"><span data-stu-id="9be1f-133">**One**</span></span>        | <span data-ttu-id="9be1f-134">Immer eine Dezimalstelle anzeigen.</span><span class="sxs-lookup"><span data-stu-id="9be1f-134">Always display one decimal place.</span></span>
| <span data-ttu-id="9be1f-135">**two**</span><span class="sxs-lookup"><span data-stu-id="9be1f-135">**Two**</span></span>        | <span data-ttu-id="9be1f-136">Immer zwei Dezimalstellen anzeigen.</span><span class="sxs-lookup"><span data-stu-id="9be1f-136">Always display two decimal places.</span></span>
| <span data-ttu-id="9be1f-137">**three**</span><span class="sxs-lookup"><span data-stu-id="9be1f-137">**Three**</span></span>      | <span data-ttu-id="9be1f-138">Immer drei Dezimalstellen anzeigen.</span><span class="sxs-lookup"><span data-stu-id="9be1f-138">Always display three decimal places.</span></span>
| <span data-ttu-id="9be1f-139">**four**</span><span class="sxs-lookup"><span data-stu-id="9be1f-139">**Four**</span></span>       | <span data-ttu-id="9be1f-140">Immer vier Dezimalstellen anzeigen.</span><span class="sxs-lookup"><span data-stu-id="9be1f-140">Always display four decimal places.</span></span>
| <span data-ttu-id="9be1f-141">**five**</span><span class="sxs-lookup"><span data-stu-id="9be1f-141">**five**</span></span>       | <span data-ttu-id="9be1f-142">Immer fünf Dezimalstellen anzeigen.</span><span class="sxs-lookup"><span data-stu-id="9be1f-142">Always display five decimal places.</span></span>

<span data-ttu-id="9be1f-143">Hinweis: **decimalPlaces** und **displayAs** trifft darauf zu, wie Zahlen gerendert, nicht gespeichert werden.</span><span class="sxs-lookup"><span data-stu-id="9be1f-143">Note: **decimalPlaces** and **displayAs** apply to how numbers are rendered, not stored.</span></span>
<span data-ttu-id="9be1f-144">Diese Eigenschaften können aktualisiert werden.</span><span class="sxs-lookup"><span data-stu-id="9be1f-144">These properties may be updated.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/NumberColumn"
} -->
