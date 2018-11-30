---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: CurrencyColumn
ms.openlocfilehash: 21c95026eb61eb68c98010d8ac288be115e95ec8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065856"
---
# <a name="currencycolumn-resource-type"></a><span data-ttu-id="35e71-102">CurrencyColumn-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="35e71-102">CurrencyColumn resource type</span></span>

> <span data-ttu-id="35e71-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="35e71-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="35e71-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="35e71-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="35e71-105">Die **numberColumn** einer [columnDefinition](columndefinition.md)-Ressource gibt an, dass es sich bei den Spaltenwerten um Währungen handelt.</span><span class="sxs-lookup"><span data-stu-id="35e71-105">The **currencyColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values represent currency.</span></span>

## <a name="json-representation"></a><span data-ttu-id="35e71-106">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="35e71-106">JSON representation</span></span>

<span data-ttu-id="35e71-107">Es folgt eine JSON-Darstellung einer **currencyColumn**-Ressource.</span><span class="sxs-lookup"><span data-stu-id="35e71-107">Here is a JSON representation of a **currencyColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.currencyColumn" } -->

```json
{
  "locale": "en-us"
}
```

## <a name="properties"></a><span data-ttu-id="35e71-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="35e71-108">Properties</span></span>

| <span data-ttu-id="35e71-109">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="35e71-109">Property name</span></span> | <span data-ttu-id="35e71-110">Typ</span><span class="sxs-lookup"><span data-stu-id="35e71-110">Type</span></span>   | <span data-ttu-id="35e71-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="35e71-111">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="35e71-112">**locale**</span><span class="sxs-lookup"><span data-stu-id="35e71-112">**locale**</span></span>    | <span data-ttu-id="35e71-113">string</span><span class="sxs-lookup"><span data-stu-id="35e71-113">string</span></span> | <span data-ttu-id="35e71-114">Gibt das Gebiet an, aus dem das Währungssymbol abzuleiten ist.</span><span class="sxs-lookup"><span data-stu-id="35e71-114">Specifies the locale from which to infer the currency symbol.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/CurrencyColumn"
} -->
