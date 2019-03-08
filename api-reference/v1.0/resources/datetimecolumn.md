---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: DateTimeColumn
localization_priority: Normal
ms.openlocfilehash: ba650ccbe307ba286cf2182bda35a21f3c675114
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2019
ms.locfileid: "30480173"
---
# <a name="datetimecolumn-resource-type"></a><span data-ttu-id="175c8-102">DateTimeColumn-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="175c8-102">DateTimeColumn resource type</span></span>

<span data-ttu-id="175c8-103">Die **dateTimeColumn** einer [columnDefinition](columndefinition.md)-Ressource gibt an, dass es sich bei den Spaltenwerten um Daten oder Uhrzeiten handelt.</span><span class="sxs-lookup"><span data-stu-id="175c8-103">The **dateTimeColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are dates or times.</span></span>

## <a name="json-representation"></a><span data-ttu-id="175c8-104">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="175c8-104">JSON representation</span></span>

<span data-ttu-id="175c8-105">Es folgt eine JSON-Darstellung einer **dateTimeColumn**-Ressource.</span><span class="sxs-lookup"><span data-stu-id="175c8-105">Here is a JSON representation of a **dateTimeColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.dateTimeColumn" } -->

```json
{
  "displayAs": "default | friendly | standard",
  "format": "dateOnly | dateTime"
}
```

## <a name="properties"></a><span data-ttu-id="175c8-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="175c8-106">Properties</span></span>

| <span data-ttu-id="175c8-107">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="175c8-107">Property name</span></span>      | <span data-ttu-id="175c8-108">Typ</span><span class="sxs-lookup"><span data-stu-id="175c8-108">Type</span></span>               | <span data-ttu-id="175c8-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="175c8-109">Description</span></span>
|:-------------------|:-------------------|:----------------------------------------------
| <span data-ttu-id="175c8-110">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="175c8-110">**displayAs**</span></span>      | <span data-ttu-id="175c8-111">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="175c8-111">string</span></span>             | <span data-ttu-id="175c8-112">Wie sollte der Wert in der UX dargestellt werden?</span><span class="sxs-lookup"><span data-stu-id="175c8-112">How the value should be presented in the UX.</span></span> <span data-ttu-id="175c8-113">Muss `default`, `friendly` oder `standard` sein.</span><span class="sxs-lookup"><span data-stu-id="175c8-113">Must be one of `default`, `friendly`, or `standard`.</span></span> <span data-ttu-id="175c8-114">Weitere Einzelheiten finden Sie weiter unten.</span><span class="sxs-lookup"><span data-stu-id="175c8-114">See below for more details.</span></span> <span data-ttu-id="175c8-115">Wenn nicht angegeben, werden sie als `default` behandelt.</span><span class="sxs-lookup"><span data-stu-id="175c8-115">If unspecified, treated as `default`.</span></span>
| <span data-ttu-id="175c8-116">**format**</span><span class="sxs-lookup"><span data-stu-id="175c8-116">**format**</span></span>         | <span data-ttu-id="175c8-117">string</span><span class="sxs-lookup"><span data-stu-id="175c8-117">string</span></span>             | <span data-ttu-id="175c8-118">Gibt an, ob der Wert nur als Datum oder als Datum und Uhrzeit angezeigt werden soll.</span><span class="sxs-lookup"><span data-stu-id="175c8-118">Indicates whether the value should be presented as a date only or a date and time.</span></span> <span data-ttu-id="175c8-119">Muss `dateOnly` oder `dateTime` sein.</span><span class="sxs-lookup"><span data-stu-id="175c8-119">Must be one of `dateOnly` or `dateTime`</span></span>

## <a name="displayas-options"></a><span data-ttu-id="175c8-120">Displays-Optionen</span><span class="sxs-lookup"><span data-stu-id="175c8-120">DisplayAs options</span></span>

| <span data-ttu-id="175c8-121">Wert</span><span class="sxs-lookup"><span data-stu-id="175c8-121">Value</span></span>        | <span data-ttu-id="175c8-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="175c8-122">Description</span></span>
|:-------------|:--------------------------------------------------------------
| <span data-ttu-id="175c8-123">**default**</span><span class="sxs-lookup"><span data-stu-id="175c8-123">**default**</span></span>  | <span data-ttu-id="175c8-124">Verwendet das standardmäßige Rendering in der UX.</span><span class="sxs-lookup"><span data-stu-id="175c8-124">Uses the default rendering in the UX.</span></span>
| <span data-ttu-id="175c8-125">**friendly**</span><span class="sxs-lookup"><span data-stu-id="175c8-125">**friendly**</span></span> | <span data-ttu-id="175c8-126">Verwendet eine benutzerfreundliche relative Darstellung (z. B.</span><span class="sxs-lookup"><span data-stu-id="175c8-126">Uses a friendly relative representation (eg.</span></span> <span data-ttu-id="175c8-127">"heute um 15:00 Uhr")</span><span class="sxs-lookup"><span data-stu-id="175c8-127">"today at 3:00 PM")</span></span>
| <span data-ttu-id="175c8-128">**standard**</span><span class="sxs-lookup"><span data-stu-id="175c8-128">**standard**</span></span> | <span data-ttu-id="175c8-129">Verwendet die standardmäßige absolute Darstellung (z. B.</span><span class="sxs-lookup"><span data-stu-id="175c8-129">Uses the standard absolute representation (eg.</span></span> <span data-ttu-id="175c8-130">"10.05.2017 15:20 Uhr")</span><span class="sxs-lookup"><span data-stu-id="175c8-130">"5/10/2017 3:20 PM")</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/choicecolumn.md:
      Found potential enums in resource example that weren't defined in a table:(checkBoxes,dropDownMenu,radioButtons) are in resource, but () are in table",
    "Warning: /api-reference/v1.0/resources/datetimecolumn.md:
      Found potential enums in resource example that weren't defined in a table:(default,friendly,standard) are in resource, but () are in table",
    "Warning: /api-reference/v1.0/resources/datetimecolumn.md:
      Found potential enums in resource example that weren't defined in a table:(dateOnly,dateTime) are in resource, but () are in table"
  ],
  "tocPath": "Resources/DateTimeColumn"
} -->
