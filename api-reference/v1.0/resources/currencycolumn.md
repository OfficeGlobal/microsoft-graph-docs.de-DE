---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: CurrencyColumn
ms.openlocfilehash: 796bd9fc7bf379ea38dc2d2f602411740caf4b86
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27019791"
---
# <a name="currencycolumn-resource-type"></a><span data-ttu-id="f91e1-102">CurrencyColumn-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="f91e1-102">CurrencyColumn resource type</span></span>

<span data-ttu-id="f91e1-103">Die **numberColumn** einer [columnDefinition](columndefinition.md)-Ressource gibt an, dass es sich bei den Spaltenwerten um Währungen handelt.</span><span class="sxs-lookup"><span data-stu-id="f91e1-103">The **currencyColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values represent currency.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f91e1-104">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="f91e1-104">JSON representation</span></span>

<span data-ttu-id="f91e1-105">Es folgt eine JSON-Darstellung einer **currencyColumn**-Ressource.</span><span class="sxs-lookup"><span data-stu-id="f91e1-105">Here is a JSON representation of a **currencyColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.currencyColumn" } -->

```json
{
  "locale": "en-us"
}
```

## <a name="properties"></a><span data-ttu-id="f91e1-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f91e1-106">Properties</span></span>

| <span data-ttu-id="f91e1-107">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="f91e1-107">Property name</span></span> | <span data-ttu-id="f91e1-108">Typ</span><span class="sxs-lookup"><span data-stu-id="f91e1-108">Type</span></span>   | <span data-ttu-id="f91e1-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f91e1-109">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="f91e1-110">**locale**</span><span class="sxs-lookup"><span data-stu-id="f91e1-110">**locale**</span></span>    | <span data-ttu-id="f91e1-111">string</span><span class="sxs-lookup"><span data-stu-id="f91e1-111">string</span></span> | <span data-ttu-id="f91e1-112">Gibt das Gebiet an, aus dem das Währungssymbol abzuleiten ist.</span><span class="sxs-lookup"><span data-stu-id="f91e1-112">Specifies the locale from which to infer the currency symbol.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/CurrencyColumn"
} -->
