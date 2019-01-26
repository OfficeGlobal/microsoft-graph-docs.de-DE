---
title: AddIn Ressourcentyp
description: Es folgt eine JSON-Darstellung der Ressource.
localization_priority: Normal
ms.openlocfilehash: 4e930ef3073cd3ea242522b537170aece8d49e0d
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29570617"
---
# <a name="addin-resource-type"></a><span data-ttu-id="3386f-103">AddIn Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="3386f-103">addIn resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="json-representation"></a><span data-ttu-id="3386f-104">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="3386f-104">JSON representation</span></span>

<span data-ttu-id="3386f-105">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="3386f-105">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.addIn"
}-->

```json
{
  "id": "guid",
  "properties": [{"@odata.type": "microsoft.graph.keyvalue"}],
  "type": "string"
}

```
## <a name="properties"></a><span data-ttu-id="3386f-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="3386f-106">Properties</span></span>
| <span data-ttu-id="3386f-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3386f-107">Property</span></span>     | <span data-ttu-id="3386f-108">Typ</span><span class="sxs-lookup"><span data-stu-id="3386f-108">Type</span></span>   |<span data-ttu-id="3386f-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3386f-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3386f-110">id</span><span class="sxs-lookup"><span data-stu-id="3386f-110">id</span></span>|<span data-ttu-id="3386f-111">GUID</span><span class="sxs-lookup"><span data-stu-id="3386f-111">guid</span></span>||
|<span data-ttu-id="3386f-112">properties</span><span class="sxs-lookup"><span data-stu-id="3386f-112">properties</span></span>|<span data-ttu-id="3386f-113">[KeyValue](keyvalue.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="3386f-113">[keyvalue](keyvalue.md) collection</span></span>||
|<span data-ttu-id="3386f-114">type</span><span class="sxs-lookup"><span data-stu-id="3386f-114">type</span></span>|<span data-ttu-id="3386f-115">string</span><span class="sxs-lookup"><span data-stu-id="3386f-115">string</span></span>||

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "addIn resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/addin.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
