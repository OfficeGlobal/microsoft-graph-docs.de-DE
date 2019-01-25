---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: DateTimeColumn
localization_priority: Normal
ms.openlocfilehash: e49b749adeaf7b04f9324fe00f9c73bf61f8b2dc
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518681"
---
# <a name="datetimecolumn-resource-type"></a><span data-ttu-id="95de3-102">DateTimeColumn-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="95de3-102">DateTimeColumn resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="95de3-103">Die **dateTimeColumn** einer [columnDefinition](columndefinition.md)-Ressource gibt an, dass es sich bei den Spaltenwerten um Daten oder Uhrzeiten handelt.</span><span class="sxs-lookup"><span data-stu-id="95de3-103">The **dateTimeColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are dates or times.</span></span>

## <a name="json-representation"></a><span data-ttu-id="95de3-104">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="95de3-104">JSON representation</span></span>

<span data-ttu-id="95de3-105">Es folgt eine JSON-Darstellung einer **dateTimeColumn**-Ressource.</span><span class="sxs-lookup"><span data-stu-id="95de3-105">Here is a JSON representation of a **dateTimeColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.dateTimeColumn" } -->

```json
{
  "displayAs": "default | friendly | standard",
  "format": "dateOnly | dateTime"
}
```

## <a name="properties"></a><span data-ttu-id="95de3-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="95de3-106">Properties</span></span>

| <span data-ttu-id="95de3-107">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="95de3-107">Property name</span></span>      | <span data-ttu-id="95de3-108">Typ</span><span class="sxs-lookup"><span data-stu-id="95de3-108">Type</span></span>               | <span data-ttu-id="95de3-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="95de3-109">Description</span></span>
|:-------------------|:-------------------|:----------------------------------------------
| <span data-ttu-id="95de3-110">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="95de3-110">**displayAs**</span></span>      | <span data-ttu-id="95de3-111">string</span><span class="sxs-lookup"><span data-stu-id="95de3-111">string</span></span>             | <span data-ttu-id="95de3-112">Wie sollte der Wert in der UX dargestellt werden?</span><span class="sxs-lookup"><span data-stu-id="95de3-112">How the value should be presented in the UX.</span></span> <span data-ttu-id="95de3-113">Muss `default`, `friendly` oder `standard` sein.</span><span class="sxs-lookup"><span data-stu-id="95de3-113">Must be one of `default`, `friendly`, or `standard`.</span></span> <span data-ttu-id="95de3-114">Weitere Einzelheiten finden Sie weiter unten.</span><span class="sxs-lookup"><span data-stu-id="95de3-114">See below for more details.</span></span> <span data-ttu-id="95de3-115">Wenn nicht angegeben, werden sie als `default` behandelt.</span><span class="sxs-lookup"><span data-stu-id="95de3-115">If unspecified, treated as `default`.</span></span>
| <span data-ttu-id="95de3-116">**format**</span><span class="sxs-lookup"><span data-stu-id="95de3-116">**format**</span></span>         | <span data-ttu-id="95de3-117">string</span><span class="sxs-lookup"><span data-stu-id="95de3-117">string</span></span>             | <span data-ttu-id="95de3-118">Gibt an, ob der Wert nur als Datum oder als Datum und Uhrzeit angezeigt werden soll.</span><span class="sxs-lookup"><span data-stu-id="95de3-118">Indicates whether the value should be presented as a date only or a date and time.</span></span> <span data-ttu-id="95de3-119">Muss `dateOnly` oder `dateTime` sein.</span><span class="sxs-lookup"><span data-stu-id="95de3-119">Must be one of `dateOnly` or `dateTime`</span></span>

## <a name="displayas-values"></a><span data-ttu-id="95de3-120">DisplayAs-Werte</span><span class="sxs-lookup"><span data-stu-id="95de3-120">DisplayAs values</span></span>

| <span data-ttu-id="95de3-121">Wert</span><span class="sxs-lookup"><span data-stu-id="95de3-121">Value</span></span>        | <span data-ttu-id="95de3-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="95de3-122">Description</span></span>
|:-------------|:--------------------------------------------------------------
| <span data-ttu-id="95de3-123">**default**</span><span class="sxs-lookup"><span data-stu-id="95de3-123">**default**</span></span>  | <span data-ttu-id="95de3-124">Verwendet das standardmäßige Rendering in der UX.</span><span class="sxs-lookup"><span data-stu-id="95de3-124">Uses the default rendering in the UX.</span></span>
| <span data-ttu-id="95de3-125">**friendly**</span><span class="sxs-lookup"><span data-stu-id="95de3-125">**friendly**</span></span> | <span data-ttu-id="95de3-126">Verwendet eine benutzerfreundliche relative Darstellung (z. B.</span><span class="sxs-lookup"><span data-stu-id="95de3-126">Uses a friendly relative representation (eg.</span></span> <span data-ttu-id="95de3-127">"heute um 15:00 Uhr")</span><span class="sxs-lookup"><span data-stu-id="95de3-127">"today at 3:00 PM")</span></span>
| <span data-ttu-id="95de3-128">**standard**</span><span class="sxs-lookup"><span data-stu-id="95de3-128">**standard**</span></span> | <span data-ttu-id="95de3-129">Verwendet die standardmäßige absolute Darstellung (z. B.</span><span class="sxs-lookup"><span data-stu-id="95de3-129">Uses the standard absolute representation (eg.</span></span> <span data-ttu-id="95de3-130">"10.05.2017 15:20 Uhr")</span><span class="sxs-lookup"><span data-stu-id="95de3-130">"5/10/2017 3:20 PM")</span></span>


<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/DateTimeColumn",
  "suppressions": [
    "Error: /api-reference/beta/resources/datetimecolumn.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
