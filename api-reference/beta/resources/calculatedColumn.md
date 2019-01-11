---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: CalculatedColumn
localization_priority: Normal
ms.openlocfilehash: 5433b5b5a76d313f8f34e460400906479e6d3d7c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876055"
---
# <a name="calculatedcolumn-resource-type"></a><span data-ttu-id="53644-102">CalculatedColumn-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="53644-102">CalculatedColumn resource type</span></span>

> <span data-ttu-id="53644-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="53644-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="53644-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="53644-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="53644-105">Die **calculatedColumn** einer [columnDefinition](columndefinition.md)-Ressource gibt an, dass die Daten der Spalten basierend auf anderen Spalten der Webseite berechnet werden.</span><span class="sxs-lookup"><span data-stu-id="53644-105">The **calculatedColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's data is calculated based on other columns in the site.</span></span>

## <a name="json-representation"></a><span data-ttu-id="53644-106">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="53644-106">JSON representation</span></span>

<span data-ttu-id="53644-107">Es folgt eine JSON-Darstellung einer **calculatedColumn**-Ressource.</span><span class="sxs-lookup"><span data-stu-id="53644-107">Here is a JSON representation of a **calculatedColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.calculatedColumn" } -->

```json
{
  "format": "dateOnly | dateTime",
  "formula": "=[Column1]+[Column2]+[Column3]",
  "outputType": "boolean | currency | dateTime | number | text",
}
```

## <a name="properties"></a><span data-ttu-id="53644-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="53644-108">Properties</span></span>

| <span data-ttu-id="53644-109">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="53644-109">Property name</span></span>  | <span data-ttu-id="53644-110">Typ</span><span class="sxs-lookup"><span data-stu-id="53644-110">Type</span></span>    | <span data-ttu-id="53644-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="53644-111">Description</span></span>
|:---------------|:--------|:--------------------------------------------------
| <span data-ttu-id="53644-112">**format**</span><span class="sxs-lookup"><span data-stu-id="53644-112">**format**</span></span>     | <span data-ttu-id="53644-113">string</span><span class="sxs-lookup"><span data-stu-id="53644-113">string</span></span>  | <span data-ttu-id="53644-114">Für `dateTime`-Ausgabetypen das Format des Werts.</span><span class="sxs-lookup"><span data-stu-id="53644-114">For `dateTime` output types, the format of the value.</span></span> <span data-ttu-id="53644-115">Muss `dateOnly` oder `dateTime` sein.</span><span class="sxs-lookup"><span data-stu-id="53644-115">Must be one of `dateOnly` or `dateTime`.</span></span>
| <span data-ttu-id="53644-116">**formula**</span><span class="sxs-lookup"><span data-stu-id="53644-116">**formula**</span></span>    | <span data-ttu-id="53644-117">string</span><span class="sxs-lookup"><span data-stu-id="53644-117">string</span></span>  | <span data-ttu-id="53644-118">Die Formel, die verwendet wird, um den Wert für diese Spalte zu berechnen.</span><span class="sxs-lookup"><span data-stu-id="53644-118">The formula used to compute the value for this column.</span></span>
| <span data-ttu-id="53644-119">**outputType**</span><span class="sxs-lookup"><span data-stu-id="53644-119">**outputType**</span></span> | <span data-ttu-id="53644-120">string</span><span class="sxs-lookup"><span data-stu-id="53644-120">string</span></span>  | <span data-ttu-id="53644-121">Der Ausgabetyp, der verwendet wird, um Werte in dieser Spalte zu formatieren.</span><span class="sxs-lookup"><span data-stu-id="53644-121">The output type used to format values in this column.</span></span> <span data-ttu-id="53644-122">Muss `boolean`, `currency`, `dateTime`, `number` oder `text` sein.</span><span class="sxs-lookup"><span data-stu-id="53644-122">Must be one of `boolean`, `currency`, `dateTime`, `number`, or `text`.</span></span>

<span data-ttu-id="53644-123">In SharePoint-Formeln wird eine ähnliche Syntax wie in Excel-Formeln verwendet.</span><span class="sxs-lookup"><span data-stu-id="53644-123">SharePoint formulas use a syntax similar to Excel formulas.</span></span>
<span data-ttu-id="53644-124">Unter [Beispiele für häufig verwendete Formeln in SharePoint-Listen][SPFormulas] finden Sie weitere Informationen.</span><span class="sxs-lookup"><span data-stu-id="53644-124">See [Examples of common formulas in SharePoint Lists][SPFormulas] for more information.</span></span>

[SPFormulas]: https://support.office.com/en-us/article/Examples-of-common-formulas-in-SharePoint-Lists-d81f5f21-2b4e-45ce-b170-bf7ebf6988b3

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/CalculatedColumn"
} -->
