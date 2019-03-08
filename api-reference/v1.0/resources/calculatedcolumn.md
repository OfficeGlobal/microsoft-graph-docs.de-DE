---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: CalculatedColumn
localization_priority: Normal
ms.openlocfilehash: 66fbc59fa9fe4880c023086c9bd334e04650bc73
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2019
ms.locfileid: "30481713"
---
# <a name="calculatedcolumn-resource-type"></a><span data-ttu-id="9525c-102">CalculatedColumn-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="9525c-102">CalculatedColumn resource type</span></span>

<span data-ttu-id="9525c-103">Die **calculatedColumn** einer [columnDefinition](columndefinition.md)-Ressource gibt an, dass die Daten der Spalten basierend auf anderen Spalten der Webseite berechnet werden.</span><span class="sxs-lookup"><span data-stu-id="9525c-103">The **calculatedColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's data is calculated based on other columns in the site.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9525c-104">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="9525c-104">JSON representation</span></span>

<span data-ttu-id="9525c-105">Es folgt eine JSON-Darstellung einer **calculatedColumn**-Ressource.</span><span class="sxs-lookup"><span data-stu-id="9525c-105">Here is a JSON representation of a **calculatedColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.calculatedColumn" } -->

```json
{
  "format": "dateOnly | dateTime",
  "formula": "=[Column1]+[Column2]+[Column3]",
  "outputType": "boolean | currency | dateTime | number | text",
}
```

## <a name="properties"></a><span data-ttu-id="9525c-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="9525c-106">Properties</span></span>

| <span data-ttu-id="9525c-107">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="9525c-107">Property name</span></span>  | <span data-ttu-id="9525c-108">Typ</span><span class="sxs-lookup"><span data-stu-id="9525c-108">Type</span></span>    | <span data-ttu-id="9525c-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9525c-109">Description</span></span>
|:---------------|:--------|:--------------------------------------------------
| <span data-ttu-id="9525c-110">**format**</span><span class="sxs-lookup"><span data-stu-id="9525c-110">**format**</span></span>     | <span data-ttu-id="9525c-111">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9525c-111">string</span></span>  | <span data-ttu-id="9525c-112">Für `dateTime`-Ausgabetypen das Format des Werts.</span><span class="sxs-lookup"><span data-stu-id="9525c-112">For `dateTime` output types, the format of the value.</span></span> <span data-ttu-id="9525c-113">Muss `dateOnly` oder `dateTime` sein.</span><span class="sxs-lookup"><span data-stu-id="9525c-113">Must be one of `dateOnly` or `dateTime`.</span></span>
| <span data-ttu-id="9525c-114">**formula**</span><span class="sxs-lookup"><span data-stu-id="9525c-114">**formula**</span></span>    | <span data-ttu-id="9525c-115">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9525c-115">string</span></span>  | <span data-ttu-id="9525c-116">Die Formel, die verwendet wird, um den Wert für diese Spalte zu berechnen.</span><span class="sxs-lookup"><span data-stu-id="9525c-116">The formula used to compute the value for this column.</span></span>
| <span data-ttu-id="9525c-117">**outputType**</span><span class="sxs-lookup"><span data-stu-id="9525c-117">**outputType**</span></span> | <span data-ttu-id="9525c-118">string</span><span class="sxs-lookup"><span data-stu-id="9525c-118">string</span></span>  | <span data-ttu-id="9525c-119">Der Ausgabetyp, der verwendet wird, um Werte in dieser Spalte zu formatieren.</span><span class="sxs-lookup"><span data-stu-id="9525c-119">The output type used to format values in this column.</span></span> <span data-ttu-id="9525c-120">Muss `boolean`, `currency`, `dateTime`, `number` oder `text` sein.</span><span class="sxs-lookup"><span data-stu-id="9525c-120">Must be one of `boolean`, `currency`, `dateTime`, `number`, or `text`.</span></span>

<span data-ttu-id="9525c-121">In SharePoint-Formeln wird eine ähnliche Syntax wie in Excel-Formeln verwendet.</span><span class="sxs-lookup"><span data-stu-id="9525c-121">SharePoint formulas use a syntax similar to Excel formulas.</span></span>
<span data-ttu-id="9525c-122">Unter [Beispiele für häufig verwendete Formeln in SharePoint-Listen][SPFormulas] finden Sie weitere Informationen.</span><span class="sxs-lookup"><span data-stu-id="9525c-122">See [Examples of common formulas in SharePoint Lists][SPFormulas] for more information.</span></span>

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
