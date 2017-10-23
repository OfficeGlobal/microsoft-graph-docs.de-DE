---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: CurrencyColumn
ms.openlocfilehash: 4f3ae97e5abfb84ad523caf74fa70b1f1ec0322a
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/28/2017
---
# <a name="currencycolumn-resource-type"></a><span data-ttu-id="85311-102">CurrencyColumn-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="85311-102">CurrencyColumn resource type</span></span>

<span data-ttu-id="85311-103">Die **numberColumn** einer [columnDefinition](columnDefinition.md)-Ressource gibt an, dass es sich bei den Spaltenwerten um Währungen handelt.</span><span class="sxs-lookup"><span data-stu-id="85311-103">The **currencyColumn** on a [columnDefinition](columnDefinition.md) resource indicates that the column's values represent currency.</span></span>

## <a name="json-representation"></a><span data-ttu-id="85311-104">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="85311-104">JSON representation</span></span>

<span data-ttu-id="85311-105">Es folgt eine JSON-Darstellung einer **currencyColumn**-Ressource.</span><span class="sxs-lookup"><span data-stu-id="85311-105">Here is a JSON representation of a **baseItem** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.currencyColumn" } -->

```json
{
  "locale": "en-us"
}
```

## <a name="properties"></a><span data-ttu-id="85311-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="85311-106">Properties</span></span>

| <span data-ttu-id="85311-107">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="85311-107">Property name</span></span> | <span data-ttu-id="85311-108">Typ</span><span class="sxs-lookup"><span data-stu-id="85311-108">Type</span></span>   | <span data-ttu-id="85311-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="85311-109">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="85311-110">**locale**</span><span class="sxs-lookup"><span data-stu-id="85311-110">**locale**</span></span>    | <span data-ttu-id="85311-111">string</span><span class="sxs-lookup"><span data-stu-id="85311-111">string</span></span> | <span data-ttu-id="85311-112">Gibt das Gebiet an, aus dem das Währungssymbol abzuleiten ist.</span><span class="sxs-lookup"><span data-stu-id="85311-112">Specifies the locale from which to infer the currency symbol.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/CurrencyColumn"
} -->
