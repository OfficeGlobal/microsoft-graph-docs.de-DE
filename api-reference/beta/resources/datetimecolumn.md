---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: DateTimeColumn
localization_priority: Normal
ms.openlocfilehash: 03ebb78adda52a9f98aec6635bbda48dd61e37e2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27889215"
---
# <a name="datetimecolumn-resource-type"></a><span data-ttu-id="9eed9-102">DateTimeColumn-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="9eed9-102">DateTimeColumn resource type</span></span>

> <span data-ttu-id="9eed9-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="9eed9-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9eed9-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9eed9-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9eed9-105">Die **dateTimeColumn** einer [columnDefinition](columndefinition.md)-Ressource gibt an, dass es sich bei den Spaltenwerten um Daten oder Uhrzeiten handelt.</span><span class="sxs-lookup"><span data-stu-id="9eed9-105">The **dateTimeColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are dates or times.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9eed9-106">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="9eed9-106">JSON representation</span></span>

<span data-ttu-id="9eed9-107">Es folgt eine JSON-Darstellung einer **dateTimeColumn**-Ressource.</span><span class="sxs-lookup"><span data-stu-id="9eed9-107">Here is a JSON representation of a **dateTimeColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.dateTimeColumn" } -->

```json
{
  "displayAs": "default | friendly | standard",
  "format": "dateOnly | dateTime"
}
```

## <a name="properties"></a><span data-ttu-id="9eed9-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="9eed9-108">Properties</span></span>

| <span data-ttu-id="9eed9-109">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="9eed9-109">Property name</span></span>      | <span data-ttu-id="9eed9-110">Typ</span><span class="sxs-lookup"><span data-stu-id="9eed9-110">Type</span></span>               | <span data-ttu-id="9eed9-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9eed9-111">Description</span></span>
|:-------------------|:-------------------|:----------------------------------------------
| <span data-ttu-id="9eed9-112">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="9eed9-112">**displayAs**</span></span>      | <span data-ttu-id="9eed9-113">string</span><span class="sxs-lookup"><span data-stu-id="9eed9-113">string</span></span>             | <span data-ttu-id="9eed9-114">Wie sollte der Wert in der UX dargestellt werden?</span><span class="sxs-lookup"><span data-stu-id="9eed9-114">How the value should be presented in the UX.</span></span> <span data-ttu-id="9eed9-115">Muss `default`, `friendly` oder `standard` sein.</span><span class="sxs-lookup"><span data-stu-id="9eed9-115">Must be one of `default`, `friendly`, or `standard`.</span></span> <span data-ttu-id="9eed9-116">Weitere Einzelheiten finden Sie weiter unten.</span><span class="sxs-lookup"><span data-stu-id="9eed9-116">See below for more details.</span></span> <span data-ttu-id="9eed9-117">Wenn nicht angegeben, werden sie als `default` behandelt.</span><span class="sxs-lookup"><span data-stu-id="9eed9-117">If unspecified, treated as `default`.</span></span>
| <span data-ttu-id="9eed9-118">**format**</span><span class="sxs-lookup"><span data-stu-id="9eed9-118">**format**</span></span>         | <span data-ttu-id="9eed9-119">string</span><span class="sxs-lookup"><span data-stu-id="9eed9-119">string</span></span>             | <span data-ttu-id="9eed9-120">Gibt an, ob der Wert nur als Datum oder als Datum und Uhrzeit angezeigt werden soll.</span><span class="sxs-lookup"><span data-stu-id="9eed9-120">Indicates whether the value should be presented as a date only or a date and time.</span></span> <span data-ttu-id="9eed9-121">Muss `dateOnly` oder `dateTime` sein.</span><span class="sxs-lookup"><span data-stu-id="9eed9-121">Must be one of `dateOnly` or `dateTime`</span></span>

## <a name="displayas-values"></a><span data-ttu-id="9eed9-122">DisplayAs-Werte</span><span class="sxs-lookup"><span data-stu-id="9eed9-122">DisplayAs values</span></span>

| <span data-ttu-id="9eed9-123">Wert</span><span class="sxs-lookup"><span data-stu-id="9eed9-123">Value</span></span>        | <span data-ttu-id="9eed9-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9eed9-124">Description</span></span>
|:-------------|:--------------------------------------------------------------
| <span data-ttu-id="9eed9-125">**default**</span><span class="sxs-lookup"><span data-stu-id="9eed9-125">**default**</span></span>  | <span data-ttu-id="9eed9-126">Verwendet das standardmäßige Rendering in der UX.</span><span class="sxs-lookup"><span data-stu-id="9eed9-126">Uses the default rendering in the UX.</span></span>
| <span data-ttu-id="9eed9-127">**friendly**</span><span class="sxs-lookup"><span data-stu-id="9eed9-127">**friendly**</span></span> | <span data-ttu-id="9eed9-128">Verwendet eine benutzerfreundliche relative Darstellung (z. B.</span><span class="sxs-lookup"><span data-stu-id="9eed9-128">Uses a friendly relative representation (eg.</span></span> <span data-ttu-id="9eed9-129">"heute um 15:00 Uhr")</span><span class="sxs-lookup"><span data-stu-id="9eed9-129">"today at 3:00 PM")</span></span>
| <span data-ttu-id="9eed9-130">**standard**</span><span class="sxs-lookup"><span data-stu-id="9eed9-130">**standard**</span></span> | <span data-ttu-id="9eed9-131">Verwendet die standardmäßige absolute Darstellung (z. B.</span><span class="sxs-lookup"><span data-stu-id="9eed9-131">Uses the standard absolute representation (eg.</span></span> <span data-ttu-id="9eed9-132">"10.05.2017 15:20 Uhr")</span><span class="sxs-lookup"><span data-stu-id="9eed9-132">"5/10/2017 3:20 PM")</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/DateTimeColumn"
} -->
