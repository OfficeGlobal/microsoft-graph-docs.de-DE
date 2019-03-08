---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: CurrencyColumn
localization_priority: Normal
ms.openlocfilehash: 065ac52a4d5216a4b3e62df892c8fe0a07a82ed0
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2019
ms.locfileid: "30481531"
---
# <a name="currencycolumn-resource-type"></a><span data-ttu-id="dd4ed-102">CurrencyColumn-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="dd4ed-102">CurrencyColumn resource type</span></span>

<span data-ttu-id="dd4ed-103">Die **numberColumn** einer [columnDefinition](columndefinition.md)-Ressource gibt an, dass es sich bei den Spaltenwerten um Währungen handelt.</span><span class="sxs-lookup"><span data-stu-id="dd4ed-103">The **currencyColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values represent currency.</span></span>

## <a name="json-representation"></a><span data-ttu-id="dd4ed-104">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="dd4ed-104">JSON representation</span></span>

<span data-ttu-id="dd4ed-105">Es folgt eine JSON-Darstellung einer **currencyColumn**-Ressource.</span><span class="sxs-lookup"><span data-stu-id="dd4ed-105">Here is a JSON representation of a **currencyColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.currencyColumn" } -->

```json
{
  "locale": "en-us"
}
```

## <a name="properties"></a><span data-ttu-id="dd4ed-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="dd4ed-106">Properties</span></span>

| <span data-ttu-id="dd4ed-107">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="dd4ed-107">Property name</span></span> | <span data-ttu-id="dd4ed-108">Typ</span><span class="sxs-lookup"><span data-stu-id="dd4ed-108">Type</span></span>   | <span data-ttu-id="dd4ed-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="dd4ed-109">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="dd4ed-110">**locale**</span><span class="sxs-lookup"><span data-stu-id="dd4ed-110">**locale**</span></span>    | <span data-ttu-id="dd4ed-111">string</span><span class="sxs-lookup"><span data-stu-id="dd4ed-111">string</span></span> | <span data-ttu-id="dd4ed-112">Gibt das Gebiet an, aus dem das Währungssymbol abzuleiten ist.</span><span class="sxs-lookup"><span data-stu-id="dd4ed-112">Specifies the locale from which to infer the currency symbol.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/CurrencyColumn"
} -->
