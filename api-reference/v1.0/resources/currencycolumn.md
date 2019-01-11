---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: CurrencyColumn
localization_priority: Normal
ms.openlocfilehash: e4ee085882cadafc0102ee31e17841978cef7822
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27836456"
---
# <a name="currencycolumn-resource-type"></a><span data-ttu-id="a6b0a-102">CurrencyColumn-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="a6b0a-102">CurrencyColumn resource type</span></span>

<span data-ttu-id="a6b0a-103">Die **numberColumn** einer [columnDefinition](columndefinition.md)-Ressource gibt an, dass es sich bei den Spaltenwerten um Währungen handelt.</span><span class="sxs-lookup"><span data-stu-id="a6b0a-103">The **currencyColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values represent currency.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a6b0a-104">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="a6b0a-104">JSON representation</span></span>

<span data-ttu-id="a6b0a-105">Es folgt eine JSON-Darstellung einer **currencyColumn**-Ressource.</span><span class="sxs-lookup"><span data-stu-id="a6b0a-105">Here is a JSON representation of a **currencyColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.currencyColumn" } -->

```json
{
  "locale": "en-us"
}
```

## <a name="properties"></a><span data-ttu-id="a6b0a-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="a6b0a-106">Properties</span></span>

| <span data-ttu-id="a6b0a-107">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="a6b0a-107">Property name</span></span> | <span data-ttu-id="a6b0a-108">Typ</span><span class="sxs-lookup"><span data-stu-id="a6b0a-108">Type</span></span>   | <span data-ttu-id="a6b0a-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a6b0a-109">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="a6b0a-110">**locale**</span><span class="sxs-lookup"><span data-stu-id="a6b0a-110">**locale**</span></span>    | <span data-ttu-id="a6b0a-111">string</span><span class="sxs-lookup"><span data-stu-id="a6b0a-111">string</span></span> | <span data-ttu-id="a6b0a-112">Gibt das Gebiet an, aus dem das Währungssymbol abzuleiten ist.</span><span class="sxs-lookup"><span data-stu-id="a6b0a-112">Specifies the locale from which to infer the currency symbol.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/CurrencyColumn"
} -->
