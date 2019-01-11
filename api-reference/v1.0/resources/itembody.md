---
title: itemBody-Ressourcentyp
description: Stellt Eigenschaften des Textkörpers eines Elements dar, z. B. eine Nachricht, ein Ereignis oder ein Gruppenbeitrag.
localization_priority: Normal
ms.openlocfilehash: 2eaf3b5e13833665c452eeecd74169915f5ac2fd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27805229"
---
# <a name="itembody-resource-type"></a><span data-ttu-id="03152-103">itemBody-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="03152-103">itemBody resource type</span></span>

<span data-ttu-id="03152-104">Stellt Eigenschaften des Textkörpers eines Elements dar, z. B. eine Nachricht, ein Ereignis oder ein Gruppenbeitrag.</span><span class="sxs-lookup"><span data-stu-id="03152-104">Represents properties of the body of an item, such as a message, event or group post.</span></span>

## <a name="properties"></a><span data-ttu-id="03152-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="03152-105">Properties</span></span>
| <span data-ttu-id="03152-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="03152-106">Property</span></span>     | <span data-ttu-id="03152-107">Typ</span><span class="sxs-lookup"><span data-stu-id="03152-107">Type</span></span>   |<span data-ttu-id="03152-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="03152-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="03152-109">Inhalt</span><span class="sxs-lookup"><span data-stu-id="03152-109">content</span></span>|<span data-ttu-id="03152-110">String</span><span class="sxs-lookup"><span data-stu-id="03152-110">String</span></span>|<span data-ttu-id="03152-111">Der Inhalt des Elements.</span><span class="sxs-lookup"><span data-stu-id="03152-111">The content of the item.</span></span>|
|<span data-ttu-id="03152-112">contentType</span><span class="sxs-lookup"><span data-stu-id="03152-112">contentType</span></span>|<span data-ttu-id="03152-113">bodyType</span><span class="sxs-lookup"><span data-stu-id="03152-113">bodyType</span></span>|<span data-ttu-id="03152-p101">Der Typ des Inhalts. Mögliche Werte sind `Text` und `HTML`.</span><span class="sxs-lookup"><span data-stu-id="03152-p101">The type of the content. Possible values are `Text` and `HTML`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="03152-116">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="03152-116">JSON representation</span></span>

<span data-ttu-id="03152-117">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="03152-117">Here is a JSON representation of the resource</span></span>

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
