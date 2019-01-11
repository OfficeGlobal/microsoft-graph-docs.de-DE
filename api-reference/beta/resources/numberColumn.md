---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: NumberColumn
localization_priority: Normal
ms.openlocfilehash: a0f5d13381c82a42159d0802d850d9996aaf8b54
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27855181"
---
# <a name="numbercolumn-resource-type"></a><span data-ttu-id="16bcd-102">NumberColumn-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="16bcd-102">NumberColumn resource type</span></span>

> <span data-ttu-id="16bcd-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="16bcd-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="16bcd-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="16bcd-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="16bcd-105">Die **numberColumn** einer [columnDefinition](columndefinition.md)-Ressource gibt an, dass es sich bei den Spaltenwerten um Zahlen handelt.</span><span class="sxs-lookup"><span data-stu-id="16bcd-105">The **numberColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are numbers.</span></span>

## <a name="json-representation"></a><span data-ttu-id="16bcd-106">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="16bcd-106">JSON representation</span></span>

<span data-ttu-id="16bcd-107">Es folgt eine JSON-Darstellung einer **numberColumn**-Ressource.</span><span class="sxs-lookup"><span data-stu-id="16bcd-107">Here is a JSON representation of a **numberColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.numberColumn" } -->

```json
{
  "decimalPlaces": "automatic | none | one | two | three | four | five",
  "displayAs": "number | percentage",
  "maximum": 10.551,
  "minimum": 99.993
}
```

## <a name="properties"></a><span data-ttu-id="16bcd-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="16bcd-108">Properties</span></span>

| <span data-ttu-id="16bcd-109">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="16bcd-109">Property name</span></span>      | <span data-ttu-id="16bcd-110">Typ</span><span class="sxs-lookup"><span data-stu-id="16bcd-110">Type</span></span>   | <span data-ttu-id="16bcd-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="16bcd-111">Description</span></span>
|:-------------------|:-------|:-----------------------------------------------
| <span data-ttu-id="16bcd-112">**decimalPlaces**</span><span class="sxs-lookup"><span data-stu-id="16bcd-112">**decimalPlaces**</span></span>  | <span data-ttu-id="16bcd-113">string</span><span class="sxs-lookup"><span data-stu-id="16bcd-113">string</span></span> | <span data-ttu-id="16bcd-114">Wie viele Dezimalstellen angezeigt werden sollen.</span><span class="sxs-lookup"><span data-stu-id="16bcd-114">How many decimal places to display.</span></span> <span data-ttu-id="16bcd-115">Informationen zu den möglichen Werten finden Sie weiter unten.</span><span class="sxs-lookup"><span data-stu-id="16bcd-115">See below for information about the possible values.</span></span>
| <span data-ttu-id="16bcd-116">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="16bcd-116">**displayAs**</span></span>      | <span data-ttu-id="16bcd-117">string</span><span class="sxs-lookup"><span data-stu-id="16bcd-117">string</span></span> | <span data-ttu-id="16bcd-118">Wie sollte der Wert in der UX dargestellt werden.</span><span class="sxs-lookup"><span data-stu-id="16bcd-118">How the value should be presented in the UX.</span></span> <span data-ttu-id="16bcd-119">Müssen `number` oder `percentage` sein.</span><span class="sxs-lookup"><span data-stu-id="16bcd-119">Must be one of `number` or `percentage`.</span></span> <span data-ttu-id="16bcd-120">Wenn nicht angegeben, werden sie als `number` behandelt.</span><span class="sxs-lookup"><span data-stu-id="16bcd-120">If unspecified, treated as `number`.</span></span>
| <span data-ttu-id="16bcd-121">**maximum**</span><span class="sxs-lookup"><span data-stu-id="16bcd-121">**maximum**</span></span>        | <span data-ttu-id="16bcd-122">double</span><span class="sxs-lookup"><span data-stu-id="16bcd-122">double</span></span> | <span data-ttu-id="16bcd-123">Der maximal zulässige Wert.</span><span class="sxs-lookup"><span data-stu-id="16bcd-123">The maximum permitted value.</span></span>
| <span data-ttu-id="16bcd-124">**minimum**</span><span class="sxs-lookup"><span data-stu-id="16bcd-124">**minimum**</span></span>        | <span data-ttu-id="16bcd-125">double</span><span class="sxs-lookup"><span data-stu-id="16bcd-125">double</span></span> | <span data-ttu-id="16bcd-126">Der minimal zulässige Wert.</span><span class="sxs-lookup"><span data-stu-id="16bcd-126">The minimum permitted value.</span></span>

## <a name="decimalplaces-values"></a><span data-ttu-id="16bcd-127">DecimalPlaces-Werte</span><span class="sxs-lookup"><span data-stu-id="16bcd-127">DecimalPlaces values</span></span>

| <span data-ttu-id="16bcd-128">Wert</span><span class="sxs-lookup"><span data-stu-id="16bcd-128">Value</span></span>          | <span data-ttu-id="16bcd-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="16bcd-129">Description</span></span>
|:---------------|:--------------------------------------------------------------
| <span data-ttu-id="16bcd-130">**automatic**</span><span class="sxs-lookup"><span data-stu-id="16bcd-130">**automatic**</span></span>  | <span data-ttu-id="16bcd-131">Standard.</span><span class="sxs-lookup"><span data-stu-id="16bcd-131">Default.</span></span> <span data-ttu-id="16bcd-132">Dezimalstellen werden je nach Bedarf automatisch angezeigt.</span><span class="sxs-lookup"><span data-stu-id="16bcd-132">Automatically display decimal places as needed.</span></span>
| <span data-ttu-id="16bcd-133">**none**</span><span class="sxs-lookup"><span data-stu-id="16bcd-133">**none**</span></span>       | <span data-ttu-id="16bcd-134">Keine Dezimalstellen anzuzeigen.</span><span class="sxs-lookup"><span data-stu-id="16bcd-134">Do not display any decimal places.</span></span>
| <span data-ttu-id="16bcd-135">**one**</span><span class="sxs-lookup"><span data-stu-id="16bcd-135">**one**</span></span>        | <span data-ttu-id="16bcd-136">Immer eine Dezimalstelle anzeigen.</span><span class="sxs-lookup"><span data-stu-id="16bcd-136">Always display one decimal place.</span></span>
| <span data-ttu-id="16bcd-137">**two**</span><span class="sxs-lookup"><span data-stu-id="16bcd-137">**two**</span></span>        | <span data-ttu-id="16bcd-138">Immer zwei Dezimalstellen anzeigen.</span><span class="sxs-lookup"><span data-stu-id="16bcd-138">Always display two decimal places.</span></span>
| <span data-ttu-id="16bcd-139">**three**</span><span class="sxs-lookup"><span data-stu-id="16bcd-139">**three**</span></span>      | <span data-ttu-id="16bcd-140">Immer drei Dezimalstellen anzeigen.</span><span class="sxs-lookup"><span data-stu-id="16bcd-140">Always display three decimal places.</span></span>
| <span data-ttu-id="16bcd-141">**four**</span><span class="sxs-lookup"><span data-stu-id="16bcd-141">**four**</span></span>       | <span data-ttu-id="16bcd-142">Immer vier Dezimalstellen anzeigen.</span><span class="sxs-lookup"><span data-stu-id="16bcd-142">Always display four decimal places.</span></span>
| <span data-ttu-id="16bcd-143">**five**</span><span class="sxs-lookup"><span data-stu-id="16bcd-143">**five**</span></span>       | <span data-ttu-id="16bcd-144">Immer füng Dezimalstellen anzeigen.</span><span class="sxs-lookup"><span data-stu-id="16bcd-144">Always display five decimal places.</span></span>

<span data-ttu-id="16bcd-145">Hinweis: **decimalPlaces** und **displayAs** trifft darauf zu, wie Zahlen gerendert, nicht gespeichert werden.</span><span class="sxs-lookup"><span data-stu-id="16bcd-145">Note: **decimalPlaces** and **displayAs** apply to how numbers are rendered, not stored.</span></span>
<span data-ttu-id="16bcd-146">Diese Eigenschaften können aktualisiert werden.</span><span class="sxs-lookup"><span data-stu-id="16bcd-146">These properties may be updated.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/NumberColumn"
} -->
