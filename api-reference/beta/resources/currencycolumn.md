---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: CurrencyColumn
localization_priority: Normal
ms.openlocfilehash: c89d709c93eeee0003d193d620166f8abffd9d41
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524499"
---
# <a name="currencycolumn-resource-type"></a><span data-ttu-id="be485-102">CurrencyColumn-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="be485-102">CurrencyColumn resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="be485-103">Die **numberColumn** einer [columnDefinition](columndefinition.md)-Ressource gibt an, dass es sich bei den Spaltenwerten um Währungen handelt.</span><span class="sxs-lookup"><span data-stu-id="be485-103">The **currencyColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values represent currency.</span></span>

## <a name="json-representation"></a><span data-ttu-id="be485-104">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="be485-104">JSON representation</span></span>

<span data-ttu-id="be485-105">Es folgt eine JSON-Darstellung einer **currencyColumn**-Ressource.</span><span class="sxs-lookup"><span data-stu-id="be485-105">Here is a JSON representation of a **currencyColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.currencyColumn" } -->

```json
{
  "locale": "en-us"
}
```

## <a name="properties"></a><span data-ttu-id="be485-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="be485-106">Properties</span></span>

| <span data-ttu-id="be485-107">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="be485-107">Property name</span></span> | <span data-ttu-id="be485-108">Typ</span><span class="sxs-lookup"><span data-stu-id="be485-108">Type</span></span>   | <span data-ttu-id="be485-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="be485-109">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="be485-110">**locale**</span><span class="sxs-lookup"><span data-stu-id="be485-110">**locale**</span></span>    | <span data-ttu-id="be485-111">string</span><span class="sxs-lookup"><span data-stu-id="be485-111">string</span></span> | <span data-ttu-id="be485-112">Gibt das Gebiet an, aus dem das Währungssymbol abzuleiten ist.</span><span class="sxs-lookup"><span data-stu-id="be485-112">Specifies the locale from which to infer the currency symbol.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/CurrencyColumn",
  "suppressions": [
    "Error: /api-reference/beta/resources/currencycolumn.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
