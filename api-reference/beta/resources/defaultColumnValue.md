---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: DefaultColumnValue
localization_priority: Normal
ms.openlocfilehash: 6ceca45d09654771f161db63707682a4558b0d29
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27815547"
---
# <a name="defaultcolumnvalue-resource-type"></a><span data-ttu-id="c1d78-102">DefaultColumnValue-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="c1d78-102">DefaultColumnValue resource type</span></span>

> <span data-ttu-id="c1d78-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="c1d78-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c1d78-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c1d78-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c1d78-105">Der **DefaultColumnValue** einer [ColumnDefinition](columndefinition.md)-Ressource gibt den Standardwert für diese Spalte an.</span><span class="sxs-lookup"><span data-stu-id="c1d78-105">The **defaultColumnValue** on a [columnDefinition](columndefinition.md) resource specifies the default value for this column.</span></span>
<span data-ttu-id="c1d78-106">Der Standardwert kann entweder direkt oder als Formel angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="c1d78-106">The default value can either be specified directly or as a formula.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c1d78-107">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="c1d78-107">JSON representation</span></span>

<span data-ttu-id="c1d78-108">Es folgt eine JSON-Darstellung einer **defaultColumnValue**-Ressource.</span><span class="sxs-lookup"><span data-stu-id="c1d78-108">Here is a JSON representation of a **defaultColumnValue** resource.</span></span>
<!-- { "blockType": "resource", "@type": "microsoft.graph.defaultColumnValue" } -->

```json
{
  "formula": "=[Column1]+[Column2]+[Column3]",
  "value": "defaultValueString"
}
```

## <a name="properties"></a><span data-ttu-id="c1d78-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="c1d78-109">Properties</span></span>

| <span data-ttu-id="c1d78-110">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="c1d78-110">Property name</span></span> | <span data-ttu-id="c1d78-111">Typ</span><span class="sxs-lookup"><span data-stu-id="c1d78-111">Type</span></span>   | <span data-ttu-id="c1d78-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c1d78-112">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="c1d78-113">**formula**</span><span class="sxs-lookup"><span data-stu-id="c1d78-113">**formula**</span></span>   | <span data-ttu-id="c1d78-114">string</span><span class="sxs-lookup"><span data-stu-id="c1d78-114">string</span></span> | <span data-ttu-id="c1d78-115">Die Formel, die verwendet wird, um den Standardwert für diese Spalte zu berechnen.</span><span class="sxs-lookup"><span data-stu-id="c1d78-115">The formula used to compute the default value for this column.</span></span>
| <span data-ttu-id="c1d78-116">**value**</span><span class="sxs-lookup"><span data-stu-id="c1d78-116">**value**</span></span>     | <span data-ttu-id="c1d78-117">string</span><span class="sxs-lookup"><span data-stu-id="c1d78-117">string</span></span> | <span data-ttu-id="c1d78-118">Der direkte Wert, der als Standardwert für diese Spalte verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="c1d78-118">The direct value to use as the default value for this column.</span></span>

<span data-ttu-id="c1d78-119">Es kann jeweils nur **formula** oder **value** angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="c1d78-119">Only one of **formula** or **value** may be specified at a time.</span></span>

<span data-ttu-id="c1d78-120">In SharePoint-Formeln wird eine ähnliche Syntax wie in Excel-Formeln verwendet.</span><span class="sxs-lookup"><span data-stu-id="c1d78-120">SharePoint formulas use a syntax similar to Excel formulas.</span></span>
<span data-ttu-id="c1d78-121">Unter [Beispiele für häufig verwendete Formeln in SharePoint-Listen][SPFormulas] finden Sie weitere Informationen.</span><span class="sxs-lookup"><span data-stu-id="c1d78-121">See [Examples of common formulas in SharePoint Lists][SPFormulas] for more information.</span></span>

[SPFormulas]: https://support.office.com/en-us/article/Examples-of-common-formulas-in-SharePoint-Lists-d81f5f21-2b4e-45ce-b170-bf7ebf6988b3


<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/DefaultColumnValue"
} -->
