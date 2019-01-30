---
title: itemBody-Ressourcentyp
description: Stellt Eigenschaften des Textkörpers eines Elements dar, z. B. eine Nachricht, ein Ereignis oder ein Gruppenbeitrag.
localization_priority: Normal
ms.openlocfilehash: df2e7e8cea9e1b2e6a6d1011029a1898e2794f45
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/30/2019
ms.locfileid: "29642562"
---
# <a name="itembody-resource-type"></a><span data-ttu-id="6b68b-103">itemBody-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="6b68b-103">itemBody resource type</span></span>

<span data-ttu-id="6b68b-104">Stellt Eigenschaften des Textkörpers eines Elements dar, z. B. eine Nachricht, ein Ereignis oder ein Gruppenbeitrag.</span><span class="sxs-lookup"><span data-stu-id="6b68b-104">Represents properties of the body of an item, such as a message, event or group post.</span></span>

## <a name="properties"></a><span data-ttu-id="6b68b-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="6b68b-105">Properties</span></span>
| <span data-ttu-id="6b68b-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6b68b-106">Property</span></span>     | <span data-ttu-id="6b68b-107">Typ</span><span class="sxs-lookup"><span data-stu-id="6b68b-107">Type</span></span>   |<span data-ttu-id="6b68b-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6b68b-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6b68b-109">Inhalt</span><span class="sxs-lookup"><span data-stu-id="6b68b-109">content</span></span>|<span data-ttu-id="6b68b-110">String</span><span class="sxs-lookup"><span data-stu-id="6b68b-110">String</span></span>|<span data-ttu-id="6b68b-111">Der Inhalt des Elements.</span><span class="sxs-lookup"><span data-stu-id="6b68b-111">The content of the item.</span></span>|
|<span data-ttu-id="6b68b-112">contentType</span><span class="sxs-lookup"><span data-stu-id="6b68b-112">contentType</span></span>|<span data-ttu-id="6b68b-113">bodyType</span><span class="sxs-lookup"><span data-stu-id="6b68b-113">bodyType</span></span>|<span data-ttu-id="6b68b-p101">Der Typ des Inhalts. Mögliche Werte sind `text` und `HTML`.</span><span class="sxs-lookup"><span data-stu-id="6b68b-p101">The type of the content. Possible values are `text` and `HTML`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6b68b-116">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="6b68b-116">JSON representation</span></span>

<span data-ttu-id="6b68b-117">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="6b68b-117">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.itemBody"
}-->

```json
{
  "content": "string",
  "contentType": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "itemBody resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
