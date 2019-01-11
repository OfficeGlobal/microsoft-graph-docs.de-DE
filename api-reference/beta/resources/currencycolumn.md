---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: CurrencyColumn
localization_priority: Normal
ms.openlocfilehash: 179c0bb1e5c82d7f2af17dcbcae08be8726f2ecd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27888935"
---
# <a name="currencycolumn-resource-type"></a><span data-ttu-id="93a86-102">CurrencyColumn-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="93a86-102">CurrencyColumn resource type</span></span>

> <span data-ttu-id="93a86-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="93a86-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="93a86-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="93a86-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="93a86-105">Die **numberColumn** einer [columnDefinition](columndefinition.md)-Ressource gibt an, dass es sich bei den Spaltenwerten um Währungen handelt.</span><span class="sxs-lookup"><span data-stu-id="93a86-105">The **currencyColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values represent currency.</span></span>

## <a name="json-representation"></a><span data-ttu-id="93a86-106">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="93a86-106">JSON representation</span></span>

<span data-ttu-id="93a86-107">Es folgt eine JSON-Darstellung einer **currencyColumn**-Ressource.</span><span class="sxs-lookup"><span data-stu-id="93a86-107">Here is a JSON representation of a **currencyColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.currencyColumn" } -->

```json
{
  "locale": "en-us"
}
```

## <a name="properties"></a><span data-ttu-id="93a86-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="93a86-108">Properties</span></span>

| <span data-ttu-id="93a86-109">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="93a86-109">Property name</span></span> | <span data-ttu-id="93a86-110">Typ</span><span class="sxs-lookup"><span data-stu-id="93a86-110">Type</span></span>   | <span data-ttu-id="93a86-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="93a86-111">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="93a86-112">**locale**</span><span class="sxs-lookup"><span data-stu-id="93a86-112">**locale**</span></span>    | <span data-ttu-id="93a86-113">string</span><span class="sxs-lookup"><span data-stu-id="93a86-113">string</span></span> | <span data-ttu-id="93a86-114">Gibt das Gebiet an, aus dem das Währungssymbol abzuleiten ist.</span><span class="sxs-lookup"><span data-stu-id="93a86-114">Specifies the locale from which to infer the currency symbol.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/CurrencyColumn"
} -->
