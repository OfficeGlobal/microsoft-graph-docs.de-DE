---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: DefaultColumnValue
ms.openlocfilehash: 73761e224a59b3a9a4206d5e1cfb058294b7f53b
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/28/2017
---
# <a name="defaultcolumnvalue-resource-type"></a><span data-ttu-id="96cd4-102">DefaultColumnValue-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="96cd4-102">DefaultColumnValue resource type</span></span>

<span data-ttu-id="96cd4-103">Der **DefaultColumnValue** einer [ColumnDefinition](columnDefinition.md)-Ressource gibt den Standardwert für diese Spalte an.</span><span class="sxs-lookup"><span data-stu-id="96cd4-103">The **defaultColumnValue** on a [columnDefinition](columnDefinition.md) resource specifies the default value for this column.</span></span>
<span data-ttu-id="96cd4-104">Der Standardwert kann entweder direkt oder als Formel angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="96cd4-104">The default value can either be specified directly or as a formula.</span></span>

## <a name="json-representation"></a><span data-ttu-id="96cd4-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="96cd4-105">JSON representation</span></span>

<span data-ttu-id="96cd4-106">Es folgt eine JSON-Darstellung einer **defaultColumnValue**-Ressource.</span><span class="sxs-lookup"><span data-stu-id="96cd4-106">Here is a JSON representation of a **baseItem** resource.</span></span>
<!-- { "blockType": "resource", "@type": "microsoft.graph.defaultColumnValue" } -->

```json
{
  "formula": "=[Column1]+[Column2]+[Column3]",
  "value": "defaultValueString"
}
```

## <a name="properties"></a><span data-ttu-id="96cd4-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="96cd4-107">Properties</span></span>

| <span data-ttu-id="96cd4-108">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="96cd4-108">Property name</span></span> | <span data-ttu-id="96cd4-109">Typ</span><span class="sxs-lookup"><span data-stu-id="96cd4-109">Type</span></span>   | <span data-ttu-id="96cd4-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="96cd4-110">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="96cd4-111">**formula**</span><span class="sxs-lookup"><span data-stu-id="96cd4-111">**formula**</span></span>   | <span data-ttu-id="96cd4-112">string</span><span class="sxs-lookup"><span data-stu-id="96cd4-112">string</span></span> | <span data-ttu-id="96cd4-113">Die Formel, die verwendet wird, um den Standardwert für diese Spalte zu berechnen.</span><span class="sxs-lookup"><span data-stu-id="96cd4-113">The formula used to compute the default value for this column.</span></span>
| <span data-ttu-id="96cd4-114">**value**</span><span class="sxs-lookup"><span data-stu-id="96cd4-114">**value**</span></span>     | <span data-ttu-id="96cd4-115">string</span><span class="sxs-lookup"><span data-stu-id="96cd4-115">string</span></span> | <span data-ttu-id="96cd4-116">Der direkte Wert, der als Standardwert für diese Spalte verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="96cd4-116">The direct value to use as the default value for this column.</span></span>

<span data-ttu-id="96cd4-117">Es kann jeweils nur **formula** oder **value** angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="96cd4-117">Only one of **formula** or **value** may be specified at a time.</span></span>

<span data-ttu-id="96cd4-118">In SharePoint-Formeln wird eine ähnliche Syntax wie in Excel-Formeln verwendet.</span><span class="sxs-lookup"><span data-stu-id="96cd4-118">SharePoint formulas use a syntax similar to Excel formulas.</span></span>
<span data-ttu-id="96cd4-119">Unter [Beispiele für häufig verwendete Formeln in SharePoint-Listen][SPFormulas] finden Sie weitere Informationen.</span><span class="sxs-lookup"><span data-stu-id="96cd4-119">See [Examples of common formulas in SharePoint Lists][SPFormulas] for more information.</span></span>

[SPFormulas]: https://support.office.com/en-us/article/Examples-of-common-formulas-in-SharePoint-Lists-d81f5f21-2b4e-45ce-b170-bf7ebf6988b3


<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/DefaultColumnValue"
} -->
