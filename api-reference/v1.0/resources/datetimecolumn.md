---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: DateTimeColumn
ms.openlocfilehash: ce5f06b6e0d88324813372c2431b62e6b9105bcb
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/28/2017
---
# <a name="datetimecolumn-resource-type"></a><span data-ttu-id="8069e-102">DateTimeColumn-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="8069e-102">DateTimeColumn resource type</span></span>

<span data-ttu-id="8069e-103">Die **dateTimeColumn** einer [columnDefinition](columnDefinition.md)-Ressource gibt an, dass es sich bei den Spaltenwerten um Daten oder Uhrzeiten handelt.</span><span class="sxs-lookup"><span data-stu-id="8069e-103">The **dateTimeColumn** on a [columnDefinition](columnDefinition.md) resource indicates that the column's values are dates or times.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8069e-104">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="8069e-104">JSON representation</span></span>

<span data-ttu-id="8069e-105">Es folgt eine JSON-Darstellung einer **dateTimeColumn**-Ressource.</span><span class="sxs-lookup"><span data-stu-id="8069e-105">Here is a JSON representation of a **drive** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.dateTimeColumn" } -->

```json
{
  "displayAs": "default | friendly | standard",
  "format": "dateOnly | dateTime"
}
```

## <a name="properties"></a><span data-ttu-id="8069e-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="8069e-106">Properties</span></span>

| <span data-ttu-id="8069e-107">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="8069e-107">Property name</span></span>      | <span data-ttu-id="8069e-108">Typ</span><span class="sxs-lookup"><span data-stu-id="8069e-108">Type</span></span>               | <span data-ttu-id="8069e-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8069e-109">Description</span></span>
|:-------------------|:-------------------|:----------------------------------------------
| <span data-ttu-id="8069e-110">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="8069e-110">**displayAs**</span></span>      | <span data-ttu-id="8069e-111">string</span><span class="sxs-lookup"><span data-stu-id="8069e-111">string</span></span>             | <span data-ttu-id="8069e-112">Wie sollte der Wert in der UX dargestellt werden?</span><span class="sxs-lookup"><span data-stu-id="8069e-112">How the value should be presented in the UX.</span></span> <span data-ttu-id="8069e-113">Muss `default`, `friendly` oder `standard` sein.</span><span class="sxs-lookup"><span data-stu-id="8069e-113">Must be one of `default`, `friendly`, or `standard`.</span></span> <span data-ttu-id="8069e-114">Weitere Einzelheiten finden Sie weiter unten.</span><span class="sxs-lookup"><span data-stu-id="8069e-114">Read below for more details.</span></span> <span data-ttu-id="8069e-115">Wenn nicht angegeben, werden sie als `default` behandelt.</span><span class="sxs-lookup"><span data-stu-id="8069e-115">If unspecified, treated as `default`.</span></span>
| <span data-ttu-id="8069e-116">**format**</span><span class="sxs-lookup"><span data-stu-id="8069e-116">**format**</span></span>         | <span data-ttu-id="8069e-117">string</span><span class="sxs-lookup"><span data-stu-id="8069e-117">string</span></span>             | <span data-ttu-id="8069e-118">Gibt an, ob der Wert nur als Datum oder als Datum und Uhrzeit angezeigt werden soll.</span><span class="sxs-lookup"><span data-stu-id="8069e-118">Indicates whether the value should be presented as a date only or a date and time.</span></span> <span data-ttu-id="8069e-119">Muss `dateOnly` oder `dateTime` sein.</span><span class="sxs-lookup"><span data-stu-id="8069e-119">Must be one of `dateOnly` or `dateTime`</span></span>

## <a name="displayas-values"></a><span data-ttu-id="8069e-120">DisplayAs-Werte</span><span class="sxs-lookup"><span data-stu-id="8069e-120">DisplayAs values</span></span>

| <span data-ttu-id="8069e-121">Wert</span><span class="sxs-lookup"><span data-stu-id="8069e-121">Value</span></span>        | <span data-ttu-id="8069e-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8069e-122">Description</span></span>
|:-------------|:--------------------------------------------------------------
| <span data-ttu-id="8069e-123">**default**</span><span class="sxs-lookup"><span data-stu-id="8069e-123">**default**</span></span>  | <span data-ttu-id="8069e-124">Verwendet das standardmäßige Rendering in der UX.</span><span class="sxs-lookup"><span data-stu-id="8069e-124">Uses the default rendering in the UX.</span></span>
| <span data-ttu-id="8069e-125">**friendly**</span><span class="sxs-lookup"><span data-stu-id="8069e-125">**friendly**</span></span> | <span data-ttu-id="8069e-126">Verwendet eine benutzerfreundliche relative Darstellung (z. B.</span><span class="sxs-lookup"><span data-stu-id="8069e-126">Uses a friendly relative representation (eg.</span></span> <span data-ttu-id="8069e-127">"heute um 15:00 Uhr")</span><span class="sxs-lookup"><span data-stu-id="8069e-127">"today at 3:00 PM")</span></span>
| <span data-ttu-id="8069e-128">**standard**</span><span class="sxs-lookup"><span data-stu-id="8069e-128">**Standard**</span></span> | <span data-ttu-id="8069e-129">Verwendet die standardmäßige absolute Darstellung (z. B.</span><span class="sxs-lookup"><span data-stu-id="8069e-129">Uses the standard absolute representation (eg.</span></span> <span data-ttu-id="8069e-130">"10.05.2017 15:20 Uhr")</span><span class="sxs-lookup"><span data-stu-id="8069e-130">"5/10/2017 3:20 PM")</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/DateTimeColumn"
} -->
