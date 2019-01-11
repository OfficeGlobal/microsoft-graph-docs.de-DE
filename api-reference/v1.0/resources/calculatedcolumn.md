---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: CalculatedColumn
localization_priority: Normal
ms.openlocfilehash: 402ec948344931a0506026e4ad6abfaaa0ee5539
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876930"
---
# <a name="calculatedcolumn-resource-type"></a><span data-ttu-id="0b1d6-102">CalculatedColumn-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="0b1d6-102">CalculatedColumn resource type</span></span>

<span data-ttu-id="0b1d6-103">Die **calculatedColumn** einer [columnDefinition](columndefinition.md)-Ressource gibt an, dass die Daten der Spalten basierend auf anderen Spalten der Webseite berechnet werden.</span><span class="sxs-lookup"><span data-stu-id="0b1d6-103">The **calculatedColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's data is calculated based on other columns in the site.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0b1d6-104">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="0b1d6-104">JSON representation</span></span>

<span data-ttu-id="0b1d6-105">Es folgt eine JSON-Darstellung einer **calculatedColumn**-Ressource.</span><span class="sxs-lookup"><span data-stu-id="0b1d6-105">Here is a JSON representation of a **calculatedColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.calculatedColumn" } -->

```json
{
  "format": "dateOnly | dateTime",
  "formula": "=[Column1]+[Column2]+[Column3]",
  "outputType": "boolean | currency | dateTime | number | text",
}
```

## <a name="properties"></a><span data-ttu-id="0b1d6-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="0b1d6-106">Properties</span></span>

| <span data-ttu-id="0b1d6-107">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="0b1d6-107">Property name</span></span>  | <span data-ttu-id="0b1d6-108">Typ</span><span class="sxs-lookup"><span data-stu-id="0b1d6-108">Type</span></span>    | <span data-ttu-id="0b1d6-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0b1d6-109">Description</span></span>
|:---------------|:--------|:--------------------------------------------------
| <span data-ttu-id="0b1d6-110">**format**</span><span class="sxs-lookup"><span data-stu-id="0b1d6-110">**format**</span></span>     | <span data-ttu-id="0b1d6-111">string</span><span class="sxs-lookup"><span data-stu-id="0b1d6-111">string</span></span>  | <span data-ttu-id="0b1d6-112">Für `dateTime`-Ausgabetypen das Format des Werts.</span><span class="sxs-lookup"><span data-stu-id="0b1d6-112">For `dateTime` output types, the format of the value.</span></span> <span data-ttu-id="0b1d6-113">Muss `dateOnly` oder `dateTime` sein.</span><span class="sxs-lookup"><span data-stu-id="0b1d6-113">Must be one of `dateOnly` or `dateTime`.</span></span>
| <span data-ttu-id="0b1d6-114">**formula**</span><span class="sxs-lookup"><span data-stu-id="0b1d6-114">**formula**</span></span>    | <span data-ttu-id="0b1d6-115">string</span><span class="sxs-lookup"><span data-stu-id="0b1d6-115">string</span></span>  | <span data-ttu-id="0b1d6-116">Die Formel, die verwendet wird, um den Wert für diese Spalte zu berechnen.</span><span class="sxs-lookup"><span data-stu-id="0b1d6-116">The formula used to compute the value for this column.</span></span>
| <span data-ttu-id="0b1d6-117">**outputType**</span><span class="sxs-lookup"><span data-stu-id="0b1d6-117">**outputType**</span></span> | <span data-ttu-id="0b1d6-118">string</span><span class="sxs-lookup"><span data-stu-id="0b1d6-118">string</span></span>  | <span data-ttu-id="0b1d6-119">Der Ausgabetyp, der verwendet wird, um Werte in dieser Spalte zu formatieren.</span><span class="sxs-lookup"><span data-stu-id="0b1d6-119">The output type used to format values in this column.</span></span> <span data-ttu-id="0b1d6-120">Muss `boolean`, `currency`, `dateTime`, `number` oder `text` sein.</span><span class="sxs-lookup"><span data-stu-id="0b1d6-120">Must be one of `boolean`, `currency`, `dateTime`, `number`, or `text`.</span></span>

<span data-ttu-id="0b1d6-121">In SharePoint-Formeln wird eine ähnliche Syntax wie in Excel-Formeln verwendet.</span><span class="sxs-lookup"><span data-stu-id="0b1d6-121">SharePoint formulas use a syntax similar to Excel formulas.</span></span>
<span data-ttu-id="0b1d6-122">Unter [Beispiele für häufig verwendete Formeln in SharePoint-Listen][SPFormulas] finden Sie weitere Informationen.</span><span class="sxs-lookup"><span data-stu-id="0b1d6-122">See [Examples of common formulas in SharePoint Lists][SPFormulas] for more information.</span></span>

[SPFormulas]: https://support.office.com/en-us/article/Examples-of-common-formulas-in-SharePoint-Lists-d81f5f21-2b4e-45ce-b170-bf7ebf6988b3

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/calculatedcolumn.md:
      Found potential enums in resource example that weren't defined in a table:(dateOnly,dateTime) are in resource, but () are in table",
    "Warning: /api-reference/v1.0/resources/calculatedcolumn.md:
      Found potential enums in resource example that weren't defined in a table:(boolean,currency,dateTime,number,text) are in resource, but () are in table"
  ],
  "tocPath": "Resources/CalculatedColumn"
} -->
