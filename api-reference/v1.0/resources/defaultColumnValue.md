---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: DefaultColumnValue
localization_priority: Normal
ms.openlocfilehash: 400fc25bf38f12db2be8cef21ddc351316d1265b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27810591"
---
# <a name="defaultcolumnvalue-resource-type"></a><span data-ttu-id="23daf-102">DefaultColumnValue-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="23daf-102">DefaultColumnValue resource type</span></span>

<span data-ttu-id="23daf-103">Der **DefaultColumnValue** einer [ColumnDefinition](columndefinition.md)-Ressource gibt den Standardwert für diese Spalte an.</span><span class="sxs-lookup"><span data-stu-id="23daf-103">The **defaultColumnValue** on a [columnDefinition](columndefinition.md) resource specifies the default value for this column.</span></span>
<span data-ttu-id="23daf-104">Der Standardwert kann entweder direkt oder als Formel angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="23daf-104">The default value can either be specified directly or as a formula.</span></span>

## <a name="json-representation"></a><span data-ttu-id="23daf-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="23daf-105">JSON representation</span></span>

<span data-ttu-id="23daf-106">Es folgt eine JSON-Darstellung einer **defaultColumnValue**-Ressource.</span><span class="sxs-lookup"><span data-stu-id="23daf-106">Here is a JSON representation of a **defaultColumnValue** resource.</span></span>
<!-- { "blockType": "resource", "@type": "microsoft.graph.defaultColumnValue" } -->

```json
{
  "formula": "=[Column1]+[Column2]+[Column3]",
  "value": "defaultValueString"
}
```

## <a name="properties"></a><span data-ttu-id="23daf-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="23daf-107">Properties</span></span>

| <span data-ttu-id="23daf-108">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="23daf-108">Property name</span></span> | <span data-ttu-id="23daf-109">Typ</span><span class="sxs-lookup"><span data-stu-id="23daf-109">Type</span></span>   | <span data-ttu-id="23daf-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="23daf-110">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="23daf-111">**formula**</span><span class="sxs-lookup"><span data-stu-id="23daf-111">**formula**</span></span>   | <span data-ttu-id="23daf-112">string</span><span class="sxs-lookup"><span data-stu-id="23daf-112">string</span></span> | <span data-ttu-id="23daf-113">Die Formel, die verwendet wird, um den Standardwert für diese Spalte zu berechnen.</span><span class="sxs-lookup"><span data-stu-id="23daf-113">The formula used to compute the default value for this column.</span></span>
| <span data-ttu-id="23daf-114">**value**</span><span class="sxs-lookup"><span data-stu-id="23daf-114">**value**</span></span>     | <span data-ttu-id="23daf-115">string</span><span class="sxs-lookup"><span data-stu-id="23daf-115">string</span></span> | <span data-ttu-id="23daf-116">Der direkte Wert, der als Standardwert für diese Spalte verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="23daf-116">The direct value to use as the default value for this column.</span></span>

<span data-ttu-id="23daf-117">Es kann jeweils nur **formula** oder **value** angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="23daf-117">Only one of **formula** or **value** may be specified at a time.</span></span>

<span data-ttu-id="23daf-118">In SharePoint-Formeln wird eine ähnliche Syntax wie in Excel-Formeln verwendet.</span><span class="sxs-lookup"><span data-stu-id="23daf-118">SharePoint formulas use a syntax similar to Excel formulas.</span></span>
<span data-ttu-id="23daf-119">Unter [Beispiele für häufig verwendete Formeln in SharePoint-Listen][SPFormulas] finden Sie weitere Informationen.</span><span class="sxs-lookup"><span data-stu-id="23daf-119">See [Examples of common formulas in SharePoint Lists][SPFormulas] for more information.</span></span>

[SPFormulas]: https://support.office.com/en-us/article/Examples-of-common-formulas-in-SharePoint-Lists-d81f5f21-2b4e-45ce-b170-bf7ebf6988b3


<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/DefaultColumnValue"
} -->
