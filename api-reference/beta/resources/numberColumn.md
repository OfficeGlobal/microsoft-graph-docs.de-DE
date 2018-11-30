---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: NumberColumn
ms.openlocfilehash: 27d17d3e9b9d3d1debcd20f2beb916222801ebe9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065765"
---
# <a name="numbercolumn-resource-type"></a><span data-ttu-id="697c5-102">NumberColumn-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="697c5-102">NumberColumn resource type</span></span>

> <span data-ttu-id="697c5-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="697c5-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="697c5-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="697c5-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="697c5-105">Die **numberColumn** einer [columnDefinition](columndefinition.md)-Ressource gibt an, dass es sich bei den Spaltenwerten um Zahlen handelt.</span><span class="sxs-lookup"><span data-stu-id="697c5-105">The **numberColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are numbers.</span></span>

## <a name="json-representation"></a><span data-ttu-id="697c5-106">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="697c5-106">JSON representation</span></span>

<span data-ttu-id="697c5-107">Es folgt eine JSON-Darstellung einer **numberColumn**-Ressource.</span><span class="sxs-lookup"><span data-stu-id="697c5-107">Here is a JSON representation of a **numberColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.numberColumn" } -->

```json
{
  "decimalPlaces": "automatic | none | one | two | three | four | five",
  "displayAs": "number | percentage",
  "maximum": 10.551,
  "minimum": 99.993
}
```

## <a name="properties"></a><span data-ttu-id="697c5-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="697c5-108">Properties</span></span>

| <span data-ttu-id="697c5-109">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="697c5-109">Property name</span></span>      | <span data-ttu-id="697c5-110">Typ</span><span class="sxs-lookup"><span data-stu-id="697c5-110">Type</span></span>   | <span data-ttu-id="697c5-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="697c5-111">Description</span></span>
|:-------------------|:-------|:-----------------------------------------------
| <span data-ttu-id="697c5-112">**decimalPlaces**</span><span class="sxs-lookup"><span data-stu-id="697c5-112">**decimalPlaces**</span></span>  | <span data-ttu-id="697c5-113">string</span><span class="sxs-lookup"><span data-stu-id="697c5-113">string</span></span> | <span data-ttu-id="697c5-114">Wie viele Dezimalstellen angezeigt werden sollen.</span><span class="sxs-lookup"><span data-stu-id="697c5-114">How many decimal places to display.</span></span> <span data-ttu-id="697c5-115">Informationen zu den möglichen Werten finden Sie weiter unten.</span><span class="sxs-lookup"><span data-stu-id="697c5-115">See below for information about the possible values.</span></span>
| <span data-ttu-id="697c5-116">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="697c5-116">**displayAs**</span></span>      | <span data-ttu-id="697c5-117">string</span><span class="sxs-lookup"><span data-stu-id="697c5-117">string</span></span> | <span data-ttu-id="697c5-118">Wie sollte der Wert in der UX dargestellt werden.</span><span class="sxs-lookup"><span data-stu-id="697c5-118">How the value should be presented in the UX.</span></span> <span data-ttu-id="697c5-119">Müssen `number` oder `percentage` sein.</span><span class="sxs-lookup"><span data-stu-id="697c5-119">Must be one of `number` or `percentage`.</span></span> <span data-ttu-id="697c5-120">Wenn nicht angegeben, werden sie als `number` behandelt.</span><span class="sxs-lookup"><span data-stu-id="697c5-120">If unspecified, treated as `number`.</span></span>
| <span data-ttu-id="697c5-121">**maximum**</span><span class="sxs-lookup"><span data-stu-id="697c5-121">**maximum**</span></span>        | <span data-ttu-id="697c5-122">double</span><span class="sxs-lookup"><span data-stu-id="697c5-122">double</span></span> | <span data-ttu-id="697c5-123">Der maximal zulässige Wert.</span><span class="sxs-lookup"><span data-stu-id="697c5-123">The maximum permitted value.</span></span>
| <span data-ttu-id="697c5-124">**minimum**</span><span class="sxs-lookup"><span data-stu-id="697c5-124">**minimum**</span></span>        | <span data-ttu-id="697c5-125">double</span><span class="sxs-lookup"><span data-stu-id="697c5-125">double</span></span> | <span data-ttu-id="697c5-126">Der minimal zulässige Wert.</span><span class="sxs-lookup"><span data-stu-id="697c5-126">The minimum permitted value.</span></span>

## <a name="decimalplaces-values"></a><span data-ttu-id="697c5-127">DecimalPlaces-Werte</span><span class="sxs-lookup"><span data-stu-id="697c5-127">DecimalPlaces values</span></span>

| <span data-ttu-id="697c5-128">Wert</span><span class="sxs-lookup"><span data-stu-id="697c5-128">Value</span></span>          | <span data-ttu-id="697c5-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="697c5-129">Description</span></span>
|:---------------|:--------------------------------------------------------------
| <span data-ttu-id="697c5-130">**automatic**</span><span class="sxs-lookup"><span data-stu-id="697c5-130">**automatic**</span></span>  | <span data-ttu-id="697c5-131">Standard.</span><span class="sxs-lookup"><span data-stu-id="697c5-131">Default.</span></span> <span data-ttu-id="697c5-132">Dezimalstellen werden je nach Bedarf automatisch angezeigt.</span><span class="sxs-lookup"><span data-stu-id="697c5-132">Automatically display decimal places as needed.</span></span>
| <span data-ttu-id="697c5-133">**none**</span><span class="sxs-lookup"><span data-stu-id="697c5-133">**none**</span></span>       | <span data-ttu-id="697c5-134">Keine Dezimalstellen anzuzeigen.</span><span class="sxs-lookup"><span data-stu-id="697c5-134">Do not display any decimal places.</span></span>
| <span data-ttu-id="697c5-135">**one**</span><span class="sxs-lookup"><span data-stu-id="697c5-135">**one**</span></span>        | <span data-ttu-id="697c5-136">Immer eine Dezimalstelle anzeigen.</span><span class="sxs-lookup"><span data-stu-id="697c5-136">Always display one decimal place.</span></span>
| <span data-ttu-id="697c5-137">**two**</span><span class="sxs-lookup"><span data-stu-id="697c5-137">**two**</span></span>        | <span data-ttu-id="697c5-138">Immer zwei Dezimalstellen anzeigen.</span><span class="sxs-lookup"><span data-stu-id="697c5-138">Always display two decimal places.</span></span>
| <span data-ttu-id="697c5-139">**three**</span><span class="sxs-lookup"><span data-stu-id="697c5-139">**three**</span></span>      | <span data-ttu-id="697c5-140">Immer drei Dezimalstellen anzeigen.</span><span class="sxs-lookup"><span data-stu-id="697c5-140">Always display three decimal places.</span></span>
| <span data-ttu-id="697c5-141">**four**</span><span class="sxs-lookup"><span data-stu-id="697c5-141">**four**</span></span>       | <span data-ttu-id="697c5-142">Immer vier Dezimalstellen anzeigen.</span><span class="sxs-lookup"><span data-stu-id="697c5-142">Always display four decimal places.</span></span>
| <span data-ttu-id="697c5-143">**five**</span><span class="sxs-lookup"><span data-stu-id="697c5-143">**five**</span></span>       | <span data-ttu-id="697c5-144">Immer füng Dezimalstellen anzeigen.</span><span class="sxs-lookup"><span data-stu-id="697c5-144">Always display five decimal places.</span></span>

<span data-ttu-id="697c5-145">Hinweis: **decimalPlaces** und **displayAs** trifft darauf zu, wie Zahlen gerendert, nicht gespeichert werden.</span><span class="sxs-lookup"><span data-stu-id="697c5-145">Note: **decimalPlaces** and **displayAs** apply to how numbers are rendered, not stored.</span></span>
<span data-ttu-id="697c5-146">Diese Eigenschaften können aktualisiert werden.</span><span class="sxs-lookup"><span data-stu-id="697c5-146">These properties may be updated.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/NumberColumn"
} -->
