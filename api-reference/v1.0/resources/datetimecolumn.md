---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: DateTimeColumn
ms.openlocfilehash: 3e61cae016a8ebccae1af59d18c559d6adf63b0f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27019072"
---
# <a name="datetimecolumn-resource-type"></a><span data-ttu-id="4850a-102">DateTimeColumn-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="4850a-102">DateTimeColumn resource type</span></span>

<span data-ttu-id="4850a-103">Die **dateTimeColumn** einer [columnDefinition](columndefinition.md)-Ressource gibt an, dass es sich bei den Spaltenwerten um Daten oder Uhrzeiten handelt.</span><span class="sxs-lookup"><span data-stu-id="4850a-103">The **dateTimeColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are dates or times.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4850a-104">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="4850a-104">JSON representation</span></span>

<span data-ttu-id="4850a-105">Es folgt eine JSON-Darstellung einer **dateTimeColumn**-Ressource.</span><span class="sxs-lookup"><span data-stu-id="4850a-105">Here is a JSON representation of a **dateTimeColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.dateTimeColumn" } -->

```json
{
  "displayAs": "default | friendly | standard",
  "format": "dateOnly | dateTime"
}
```

## <a name="properties"></a><span data-ttu-id="4850a-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="4850a-106">Properties</span></span>

| <span data-ttu-id="4850a-107">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="4850a-107">Property name</span></span>      | <span data-ttu-id="4850a-108">Typ</span><span class="sxs-lookup"><span data-stu-id="4850a-108">Type</span></span>               | <span data-ttu-id="4850a-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4850a-109">Description</span></span>
|:-------------------|:-------------------|:----------------------------------------------
| <span data-ttu-id="4850a-110">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="4850a-110">**displayAs**</span></span>      | <span data-ttu-id="4850a-111">string</span><span class="sxs-lookup"><span data-stu-id="4850a-111">string</span></span>             | <span data-ttu-id="4850a-112">Wie sollte der Wert in der UX dargestellt werden?</span><span class="sxs-lookup"><span data-stu-id="4850a-112">How the value should be presented in the UX.</span></span> <span data-ttu-id="4850a-113">Muss `default`, `friendly` oder `standard` sein.</span><span class="sxs-lookup"><span data-stu-id="4850a-113">Must be one of `default`, `friendly`, or `standard`.</span></span> <span data-ttu-id="4850a-114">Weitere Einzelheiten finden Sie weiter unten.</span><span class="sxs-lookup"><span data-stu-id="4850a-114">See below for more details.</span></span> <span data-ttu-id="4850a-115">Wenn nicht angegeben, werden sie als `default` behandelt.</span><span class="sxs-lookup"><span data-stu-id="4850a-115">If unspecified, treated as `default`.</span></span>
| <span data-ttu-id="4850a-116">**format**</span><span class="sxs-lookup"><span data-stu-id="4850a-116">**format**</span></span>         | <span data-ttu-id="4850a-117">string</span><span class="sxs-lookup"><span data-stu-id="4850a-117">string</span></span>             | <span data-ttu-id="4850a-118">Gibt an, ob der Wert nur als Datum oder als Datum und Uhrzeit angezeigt werden soll.</span><span class="sxs-lookup"><span data-stu-id="4850a-118">Indicates whether the value should be presented as a date only or a date and time.</span></span> <span data-ttu-id="4850a-119">Muss `dateOnly` oder `dateTime` sein.</span><span class="sxs-lookup"><span data-stu-id="4850a-119">Must be one of `dateOnly` or `dateTime`</span></span>

## <a name="displayas-options"></a><span data-ttu-id="4850a-120">DisplayAs-Optionen</span><span class="sxs-lookup"><span data-stu-id="4850a-120">DisplayAs options</span></span>

| <span data-ttu-id="4850a-121">Wert</span><span class="sxs-lookup"><span data-stu-id="4850a-121">Value</span></span>        | <span data-ttu-id="4850a-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4850a-122">Description</span></span>
|:-------------|:--------------------------------------------------------------
| <span data-ttu-id="4850a-123">**default**</span><span class="sxs-lookup"><span data-stu-id="4850a-123">**default**</span></span>  | <span data-ttu-id="4850a-124">Verwendet das standardmäßige Rendering in der UX.</span><span class="sxs-lookup"><span data-stu-id="4850a-124">Uses the default rendering in the UX.</span></span>
| <span data-ttu-id="4850a-125">**friendly**</span><span class="sxs-lookup"><span data-stu-id="4850a-125">**friendly**</span></span> | <span data-ttu-id="4850a-126">Verwendet eine benutzerfreundliche relative Darstellung (z. B.</span><span class="sxs-lookup"><span data-stu-id="4850a-126">Uses a friendly relative representation (eg.</span></span> <span data-ttu-id="4850a-127">"heute um 15:00 Uhr")</span><span class="sxs-lookup"><span data-stu-id="4850a-127">"today at 3:00 PM")</span></span>
| <span data-ttu-id="4850a-128">**standard**</span><span class="sxs-lookup"><span data-stu-id="4850a-128">**standard**</span></span> | <span data-ttu-id="4850a-129">Verwendet die standardmäßige absolute Darstellung (z. B.</span><span class="sxs-lookup"><span data-stu-id="4850a-129">Uses the standard absolute representation (eg.</span></span> <span data-ttu-id="4850a-130">"10.05.2017 15:20 Uhr")</span><span class="sxs-lookup"><span data-stu-id="4850a-130">"5/10/2017 3:20 PM")</span></span>


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
