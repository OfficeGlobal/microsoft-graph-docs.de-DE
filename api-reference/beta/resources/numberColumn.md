---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: NumberColumn
localization_priority: Normal
ms.openlocfilehash: edd495b62f0ccbd163ec31a2efca70923d0bc8ad
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2019
ms.locfileid: "30480768"
---
# <a name="numbercolumn-resource-type"></a><span data-ttu-id="ab1c8-102">NumberColumn-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="ab1c8-102">NumberColumn resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ab1c8-103">Die **numberColumn** einer [columnDefinition](columndefinition.md)-Ressource gibt an, dass es sich bei den Spaltenwerten um Zahlen handelt.</span><span class="sxs-lookup"><span data-stu-id="ab1c8-103">The **numberColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are numbers.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ab1c8-104">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ab1c8-104">JSON representation</span></span>

<span data-ttu-id="ab1c8-105">Es folgt eine JSON-Darstellung einer **numberColumn**-Ressource.</span><span class="sxs-lookup"><span data-stu-id="ab1c8-105">Here is a JSON representation of a **numberColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.numberColumn" } -->

```json
{
  "decimalPlaces": "automatic | none | one | two | three | four | five",
  "displayAs": "number | percentage",
  "maximum": 10.551,
  "minimum": 99.993
}
```

## <a name="properties"></a><span data-ttu-id="ab1c8-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ab1c8-106">Properties</span></span>

| <span data-ttu-id="ab1c8-107">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="ab1c8-107">Property name</span></span>      | <span data-ttu-id="ab1c8-108">Typ</span><span class="sxs-lookup"><span data-stu-id="ab1c8-108">Type</span></span>   | <span data-ttu-id="ab1c8-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ab1c8-109">Description</span></span>
|:-------------------|:-------|:-----------------------------------------------
| <span data-ttu-id="ab1c8-110">**decimalPlaces**</span><span class="sxs-lookup"><span data-stu-id="ab1c8-110">**decimalPlaces**</span></span>  | <span data-ttu-id="ab1c8-111">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ab1c8-111">string</span></span> | <span data-ttu-id="ab1c8-112">Wie viele Dezimalstellen angezeigt werden sollen.</span><span class="sxs-lookup"><span data-stu-id="ab1c8-112">How many decimal places to display.</span></span> <span data-ttu-id="ab1c8-113">Informationen zu den möglichen Werten finden Sie weiter unten.</span><span class="sxs-lookup"><span data-stu-id="ab1c8-113">See below for information about the possible values.</span></span>
| <span data-ttu-id="ab1c8-114">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="ab1c8-114">**displayAs**</span></span>      | <span data-ttu-id="ab1c8-115">string</span><span class="sxs-lookup"><span data-stu-id="ab1c8-115">string</span></span> | <span data-ttu-id="ab1c8-116">Wie sollte der Wert in der UX dargestellt werden.</span><span class="sxs-lookup"><span data-stu-id="ab1c8-116">How the value should be presented in the UX.</span></span> <span data-ttu-id="ab1c8-117">Müssen `number` oder `percentage` sein.</span><span class="sxs-lookup"><span data-stu-id="ab1c8-117">Must be one of `number` or `percentage`.</span></span> <span data-ttu-id="ab1c8-118">Wenn nicht angegeben, werden sie als `number` behandelt.</span><span class="sxs-lookup"><span data-stu-id="ab1c8-118">If unspecified, treated as `number`.</span></span>
| <span data-ttu-id="ab1c8-119">**maximum**</span><span class="sxs-lookup"><span data-stu-id="ab1c8-119">**maximum**</span></span>        | <span data-ttu-id="ab1c8-120">double</span><span class="sxs-lookup"><span data-stu-id="ab1c8-120">double</span></span> | <span data-ttu-id="ab1c8-121">Der maximal zulässige Wert.</span><span class="sxs-lookup"><span data-stu-id="ab1c8-121">The maximum permitted value.</span></span>
| <span data-ttu-id="ab1c8-122">**minimum**</span><span class="sxs-lookup"><span data-stu-id="ab1c8-122">**minimum**</span></span>        | <span data-ttu-id="ab1c8-123">double</span><span class="sxs-lookup"><span data-stu-id="ab1c8-123">double</span></span> | <span data-ttu-id="ab1c8-124">Der minimal zulässige Wert.</span><span class="sxs-lookup"><span data-stu-id="ab1c8-124">The minimum permitted value.</span></span>

## <a name="decimalplaces-values"></a><span data-ttu-id="ab1c8-125">DecimalPlaces-Werte</span><span class="sxs-lookup"><span data-stu-id="ab1c8-125">DecimalPlaces values</span></span>

| <span data-ttu-id="ab1c8-126">Wert</span><span class="sxs-lookup"><span data-stu-id="ab1c8-126">Value</span></span>          | <span data-ttu-id="ab1c8-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ab1c8-127">Description</span></span>
|:---------------|:--------------------------------------------------------------
| <span data-ttu-id="ab1c8-128">**automatic**</span><span class="sxs-lookup"><span data-stu-id="ab1c8-128">**automatic**</span></span>  | <span data-ttu-id="ab1c8-129">Standard.</span><span class="sxs-lookup"><span data-stu-id="ab1c8-129">Default.</span></span> <span data-ttu-id="ab1c8-130">Dezimalstellen werden je nach Bedarf automatisch angezeigt.</span><span class="sxs-lookup"><span data-stu-id="ab1c8-130">Automatically display decimal places as needed.</span></span>
| <span data-ttu-id="ab1c8-131">**none**</span><span class="sxs-lookup"><span data-stu-id="ab1c8-131">**none**</span></span>       | <span data-ttu-id="ab1c8-132">Keine Dezimalstellen anzuzeigen.</span><span class="sxs-lookup"><span data-stu-id="ab1c8-132">Do not display any decimal places.</span></span>
| <span data-ttu-id="ab1c8-133">**one**</span><span class="sxs-lookup"><span data-stu-id="ab1c8-133">**one**</span></span>        | <span data-ttu-id="ab1c8-134">Immer eine Dezimalstelle anzeigen.</span><span class="sxs-lookup"><span data-stu-id="ab1c8-134">Always display one decimal place.</span></span>
| <span data-ttu-id="ab1c8-135">**two**</span><span class="sxs-lookup"><span data-stu-id="ab1c8-135">**two**</span></span>        | <span data-ttu-id="ab1c8-136">Immer zwei Dezimalstellen anzeigen.</span><span class="sxs-lookup"><span data-stu-id="ab1c8-136">Always display two decimal places.</span></span>
| <span data-ttu-id="ab1c8-137">**three**</span><span class="sxs-lookup"><span data-stu-id="ab1c8-137">**three**</span></span>      | <span data-ttu-id="ab1c8-138">Immer drei Dezimalstellen anzeigen.</span><span class="sxs-lookup"><span data-stu-id="ab1c8-138">Always display three decimal places.</span></span>
| <span data-ttu-id="ab1c8-139">**four**</span><span class="sxs-lookup"><span data-stu-id="ab1c8-139">**four**</span></span>       | <span data-ttu-id="ab1c8-140">Immer vier Dezimalstellen anzeigen.</span><span class="sxs-lookup"><span data-stu-id="ab1c8-140">Always display four decimal places.</span></span>
| <span data-ttu-id="ab1c8-141">**five**</span><span class="sxs-lookup"><span data-stu-id="ab1c8-141">**five**</span></span>       | <span data-ttu-id="ab1c8-142">Immer füng Dezimalstellen anzeigen.</span><span class="sxs-lookup"><span data-stu-id="ab1c8-142">Always display five decimal places.</span></span>

<span data-ttu-id="ab1c8-143">Hinweis: **decimalPlaces** und **displayAs** trifft darauf zu, wie Zahlen gerendert, nicht gespeichert werden.</span><span class="sxs-lookup"><span data-stu-id="ab1c8-143">Note: **decimalPlaces** and **displayAs** apply to how numbers are rendered, not stored.</span></span>
<span data-ttu-id="ab1c8-144">Diese Eigenschaften können aktualisiert werden.</span><span class="sxs-lookup"><span data-stu-id="ab1c8-144">These properties may be updated.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/NumberColumn",
  "suppressions": [
    "Error: /api-reference/beta/resources/numberColumn.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
