---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: DateTimeColumn
localization_priority: Normal
ms.openlocfilehash: da8fe44e377a071ee3f20b82f7190b690dcfd6b2
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2019
ms.locfileid: "30482168"
---
# <a name="datetimecolumn-resource-type"></a><span data-ttu-id="965cf-102">DateTimeColumn-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="965cf-102">DateTimeColumn resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="965cf-103">Die **dateTimeColumn** einer [columnDefinition](columndefinition.md)-Ressource gibt an, dass es sich bei den Spaltenwerten um Daten oder Uhrzeiten handelt.</span><span class="sxs-lookup"><span data-stu-id="965cf-103">The **dateTimeColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are dates or times.</span></span>

## <a name="json-representation"></a><span data-ttu-id="965cf-104">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="965cf-104">JSON representation</span></span>

<span data-ttu-id="965cf-105">Es folgt eine JSON-Darstellung einer **dateTimeColumn**-Ressource.</span><span class="sxs-lookup"><span data-stu-id="965cf-105">Here is a JSON representation of a **dateTimeColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.dateTimeColumn" } -->

```json
{
  "displayAs": "default | friendly | standard",
  "format": "dateOnly | dateTime"
}
```

## <a name="properties"></a><span data-ttu-id="965cf-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="965cf-106">Properties</span></span>

| <span data-ttu-id="965cf-107">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="965cf-107">Property name</span></span>      | <span data-ttu-id="965cf-108">Typ</span><span class="sxs-lookup"><span data-stu-id="965cf-108">Type</span></span>               | <span data-ttu-id="965cf-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="965cf-109">Description</span></span>
|:-------------------|:-------------------|:----------------------------------------------
| <span data-ttu-id="965cf-110">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="965cf-110">**displayAs**</span></span>      | <span data-ttu-id="965cf-111">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="965cf-111">string</span></span>             | <span data-ttu-id="965cf-112">Wie sollte der Wert in der UX dargestellt werden?</span><span class="sxs-lookup"><span data-stu-id="965cf-112">How the value should be presented in the UX.</span></span> <span data-ttu-id="965cf-113">Muss `default`, `friendly` oder `standard` sein.</span><span class="sxs-lookup"><span data-stu-id="965cf-113">Must be one of `default`, `friendly`, or `standard`.</span></span> <span data-ttu-id="965cf-114">Weitere Einzelheiten finden Sie weiter unten.</span><span class="sxs-lookup"><span data-stu-id="965cf-114">See below for more details.</span></span> <span data-ttu-id="965cf-115">Wenn nicht angegeben, werden sie als `default` behandelt.</span><span class="sxs-lookup"><span data-stu-id="965cf-115">If unspecified, treated as `default`.</span></span>
| <span data-ttu-id="965cf-116">**format**</span><span class="sxs-lookup"><span data-stu-id="965cf-116">**format**</span></span>         | <span data-ttu-id="965cf-117">string</span><span class="sxs-lookup"><span data-stu-id="965cf-117">string</span></span>             | <span data-ttu-id="965cf-118">Gibt an, ob der Wert nur als Datum oder als Datum und Uhrzeit angezeigt werden soll.</span><span class="sxs-lookup"><span data-stu-id="965cf-118">Indicates whether the value should be presented as a date only or a date and time.</span></span> <span data-ttu-id="965cf-119">Muss `dateOnly` oder `dateTime` sein.</span><span class="sxs-lookup"><span data-stu-id="965cf-119">Must be one of `dateOnly` or `dateTime`</span></span>

## <a name="displayas-values"></a><span data-ttu-id="965cf-120">DisplayAs-Werte</span><span class="sxs-lookup"><span data-stu-id="965cf-120">DisplayAs values</span></span>

| <span data-ttu-id="965cf-121">Wert</span><span class="sxs-lookup"><span data-stu-id="965cf-121">Value</span></span>        | <span data-ttu-id="965cf-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="965cf-122">Description</span></span>
|:-------------|:--------------------------------------------------------------
| <span data-ttu-id="965cf-123">**default**</span><span class="sxs-lookup"><span data-stu-id="965cf-123">**default**</span></span>  | <span data-ttu-id="965cf-124">Verwendet das standardmäßige Rendering in der UX.</span><span class="sxs-lookup"><span data-stu-id="965cf-124">Uses the default rendering in the UX.</span></span>
| <span data-ttu-id="965cf-125">**friendly**</span><span class="sxs-lookup"><span data-stu-id="965cf-125">**friendly**</span></span> | <span data-ttu-id="965cf-126">Verwendet eine benutzerfreundliche relative Darstellung (z. B.</span><span class="sxs-lookup"><span data-stu-id="965cf-126">Uses a friendly relative representation (eg.</span></span> <span data-ttu-id="965cf-127">"heute um 15:00 Uhr")</span><span class="sxs-lookup"><span data-stu-id="965cf-127">"today at 3:00 PM")</span></span>
| <span data-ttu-id="965cf-128">**standard**</span><span class="sxs-lookup"><span data-stu-id="965cf-128">**standard**</span></span> | <span data-ttu-id="965cf-129">Verwendet die standardmäßige absolute Darstellung (z. B.</span><span class="sxs-lookup"><span data-stu-id="965cf-129">Uses the standard absolute representation (eg.</span></span> <span data-ttu-id="965cf-130">"10.05.2017 15:20 Uhr")</span><span class="sxs-lookup"><span data-stu-id="965cf-130">"5/10/2017 3:20 PM")</span></span>


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
