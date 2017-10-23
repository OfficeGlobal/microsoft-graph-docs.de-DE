---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: CalculatedColumn
ms.openlocfilehash: 44700ba7606243002798ec0ec84c3be30d38ef1f
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/28/2017
---
# <a name="calculatedcolumn-resource-type"></a><span data-ttu-id="d6f1f-102">CalculatedColumn-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="d6f1f-102">CalculatedColumn resource type</span></span>

<span data-ttu-id="d6f1f-103">Die **calculatedColumn** einer [columnDefinition](columnDefinition.md)-Ressource gibt an, dass die Daten der Spalten basierend auf anderen Spalten der Webseite berechnet werden.</span><span class="sxs-lookup"><span data-stu-id="d6f1f-103">The **calculatedColumn** on a [columnDefinition](columnDefinition.md) resource indicates that the column's data is calculated based on other columns in the site.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d6f1f-104">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d6f1f-104">JSON representation</span></span>

<span data-ttu-id="d6f1f-105">Es folgt eine JSON-Darstellung einer **calculatedColumn**-Ressource.</span><span class="sxs-lookup"><span data-stu-id="d6f1f-105">Here is a JSON representation of a **drive** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.calculatedColumn" } -->

```json
{
  "format": "dateOnly | dateTime",
  "formula": "=[Column1]+[Column2]+[Column3]",
  "outputType": "boolean | currency | dateTime | number | text",
}
```

## <a name="properties"></a><span data-ttu-id="d6f1f-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d6f1f-106">Properties</span></span>

| <span data-ttu-id="d6f1f-107">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="d6f1f-107">Property name</span></span>  | <span data-ttu-id="d6f1f-108">Typ</span><span class="sxs-lookup"><span data-stu-id="d6f1f-108">Type</span></span>    | <span data-ttu-id="d6f1f-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d6f1f-109">Description</span></span>
|:---------------|:--------|:--------------------------------------------------
| <span data-ttu-id="d6f1f-110">**format**</span><span class="sxs-lookup"><span data-stu-id="d6f1f-110">**format**</span></span>     | <span data-ttu-id="d6f1f-111">string</span><span class="sxs-lookup"><span data-stu-id="d6f1f-111">string</span></span>  | <span data-ttu-id="d6f1f-112">Für `dateTime`-Ausgabetypen das Format des Werts.</span><span class="sxs-lookup"><span data-stu-id="d6f1f-112">For `dateTime` output types, the format of the value.</span></span> <span data-ttu-id="d6f1f-113">Muss `dateOnly` oder `dateTime` sein.</span><span class="sxs-lookup"><span data-stu-id="d6f1f-113">Must be one of `dateOnly` or `dateTime`.</span></span>
| <span data-ttu-id="d6f1f-114">**formula**</span><span class="sxs-lookup"><span data-stu-id="d6f1f-114">**formula**</span></span>    | <span data-ttu-id="d6f1f-115">string</span><span class="sxs-lookup"><span data-stu-id="d6f1f-115">string</span></span>  | <span data-ttu-id="d6f1f-116">Die Formel, die verwendet wird, um den Wert für diese Spalte zu berechnen.</span><span class="sxs-lookup"><span data-stu-id="d6f1f-116">The formula used to compute the value for this column.</span></span>
| <span data-ttu-id="d6f1f-117">**outputType**</span><span class="sxs-lookup"><span data-stu-id="d6f1f-117">**outputType**</span></span> | <span data-ttu-id="d6f1f-118">string</span><span class="sxs-lookup"><span data-stu-id="d6f1f-118">string</span></span>  | <span data-ttu-id="d6f1f-119">Der Ausgabetyp, der verwendet wird, um Werte in dieser Spalte zu formatieren.</span><span class="sxs-lookup"><span data-stu-id="d6f1f-119">The output type used to format values in this column.</span></span> <span data-ttu-id="d6f1f-120">Muss `boolean`, `currency`, `dateTime`, `number` oder `text` sein.</span><span class="sxs-lookup"><span data-stu-id="d6f1f-120">Must be one of `boolean`, `currency`, `dateTime`, `number`, or `text`.</span></span>

<span data-ttu-id="d6f1f-121">In SharePoint-Formeln wird eine ähnliche Syntax wie in Excel-Formeln verwendet.</span><span class="sxs-lookup"><span data-stu-id="d6f1f-121">SharePoint formulas use a syntax similar to Excel formulas.</span></span>
<span data-ttu-id="d6f1f-122">Unter [Beispiele für häufig verwendete Formeln in SharePoint-Listen][SPFormulas] finden Sie weitere Informationen.</span><span class="sxs-lookup"><span data-stu-id="d6f1f-122">See [Examples of common formulas in SharePoint Lists][SPFormulas] for more information.</span></span>

[SPFormulas]: https://support.office.com/en-us/article/Examples-of-common-formulas-in-SharePoint-Lists-d81f5f21-2b4e-45ce-b170-bf7ebf6988b3

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/CalculatedColumn"
} -->
