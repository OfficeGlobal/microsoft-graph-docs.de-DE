---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: CalculatedColumn
localization_priority: Normal
ms.openlocfilehash: 74f0e6430d47e0015fa849bb0d4ddf81690a9355
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2019
ms.locfileid: "30481909"
---
# <a name="calculatedcolumn-resource-type"></a><span data-ttu-id="79e55-102">CalculatedColumn-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="79e55-102">CalculatedColumn resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="79e55-103">Die **calculatedColumn** einer [columnDefinition](columndefinition.md)-Ressource gibt an, dass die Daten der Spalten basierend auf anderen Spalten der Webseite berechnet werden.</span><span class="sxs-lookup"><span data-stu-id="79e55-103">The **calculatedColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's data is calculated based on other columns in the site.</span></span>

## <a name="json-representation"></a><span data-ttu-id="79e55-104">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="79e55-104">JSON representation</span></span>

<span data-ttu-id="79e55-105">Es folgt eine JSON-Darstellung einer **calculatedColumn**-Ressource.</span><span class="sxs-lookup"><span data-stu-id="79e55-105">Here is a JSON representation of a **calculatedColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.calculatedColumn" } -->

```json
{
  "format": "dateOnly | dateTime",
  "formula": "=[Column1]+[Column2]+[Column3]",
  "outputType": "boolean | currency | dateTime | number | text",
}
```

## <a name="properties"></a><span data-ttu-id="79e55-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="79e55-106">Properties</span></span>

| <span data-ttu-id="79e55-107">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="79e55-107">Property name</span></span>  | <span data-ttu-id="79e55-108">Typ</span><span class="sxs-lookup"><span data-stu-id="79e55-108">Type</span></span>    | <span data-ttu-id="79e55-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="79e55-109">Description</span></span>
|:---------------|:--------|:--------------------------------------------------
| <span data-ttu-id="79e55-110">**format**</span><span class="sxs-lookup"><span data-stu-id="79e55-110">**format**</span></span>     | <span data-ttu-id="79e55-111">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="79e55-111">string</span></span>  | <span data-ttu-id="79e55-112">Für `dateTime`-Ausgabetypen das Format des Werts.</span><span class="sxs-lookup"><span data-stu-id="79e55-112">For `dateTime` output types, the format of the value.</span></span> <span data-ttu-id="79e55-113">Muss `dateOnly` oder `dateTime` sein.</span><span class="sxs-lookup"><span data-stu-id="79e55-113">Must be one of `dateOnly` or `dateTime`.</span></span>
| <span data-ttu-id="79e55-114">**formula**</span><span class="sxs-lookup"><span data-stu-id="79e55-114">**formula**</span></span>    | <span data-ttu-id="79e55-115">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="79e55-115">string</span></span>  | <span data-ttu-id="79e55-116">Die Formel, die verwendet wird, um den Wert für diese Spalte zu berechnen.</span><span class="sxs-lookup"><span data-stu-id="79e55-116">The formula used to compute the value for this column.</span></span>
| <span data-ttu-id="79e55-117">**outputType**</span><span class="sxs-lookup"><span data-stu-id="79e55-117">**outputType**</span></span> | <span data-ttu-id="79e55-118">string</span><span class="sxs-lookup"><span data-stu-id="79e55-118">string</span></span>  | <span data-ttu-id="79e55-119">Der Ausgabetyp, der verwendet wird, um Werte in dieser Spalte zu formatieren.</span><span class="sxs-lookup"><span data-stu-id="79e55-119">The output type used to format values in this column.</span></span> <span data-ttu-id="79e55-120">Muss `boolean`, `currency`, `dateTime`, `number` oder `text` sein.</span><span class="sxs-lookup"><span data-stu-id="79e55-120">Must be one of `boolean`, `currency`, `dateTime`, `number`, or `text`.</span></span>

<span data-ttu-id="79e55-121">In SharePoint-Formeln wird eine ähnliche Syntax wie in Excel-Formeln verwendet.</span><span class="sxs-lookup"><span data-stu-id="79e55-121">SharePoint formulas use a syntax similar to Excel formulas.</span></span>
<span data-ttu-id="79e55-122">Unter [Beispiele für häufig verwendete Formeln in SharePoint-Listen][SPFormulas] finden Sie weitere Informationen.</span><span class="sxs-lookup"><span data-stu-id="79e55-122">See [Examples of common formulas in SharePoint Lists][SPFormulas] for more information.</span></span>

[SPFormulas]: https://support.office.com/en-us/article/Examples-of-common-formulas-in-SharePoint-Lists-d81f5f21-2b4e-45ce-b170-bf7ebf6988b3

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/CalculatedColumn",
  "suppressions": [
    "Error: /api-reference/beta/resources/calculatedColumn.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
