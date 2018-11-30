---
title: itemBody-Ressourcentyp
description: Stellt Eigenschaften des Textkörpers eines Elements dar, z. B. eine Nachricht, ein Ereignis oder ein Gruppenbeitrag.
ms.openlocfilehash: 4ceada2ffe8106c270aa262d32ff85e349a8e657
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058216"
---
# <a name="itembody-resource-type"></a><span data-ttu-id="a45c9-103">itemBody-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="a45c9-103">itemBody resource type</span></span>

> <span data-ttu-id="a45c9-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="a45c9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a45c9-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a45c9-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a45c9-106">Stellt Eigenschaften des Textkörpers eines Elements dar, z. B. eine Nachricht, ein Ereignis oder ein Gruppenbeitrag.</span><span class="sxs-lookup"><span data-stu-id="a45c9-106">Represents properties of the body of an item, such as a message, event or group post.</span></span>

## <a name="properties"></a><span data-ttu-id="a45c9-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="a45c9-107">Properties</span></span>
| <span data-ttu-id="a45c9-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a45c9-108">Property</span></span>     | <span data-ttu-id="a45c9-109">Typ</span><span class="sxs-lookup"><span data-stu-id="a45c9-109">Type</span></span>   |<span data-ttu-id="a45c9-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a45c9-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a45c9-111">Inhalt</span><span class="sxs-lookup"><span data-stu-id="a45c9-111">content</span></span>|<span data-ttu-id="a45c9-112">String</span><span class="sxs-lookup"><span data-stu-id="a45c9-112">String</span></span>|<span data-ttu-id="a45c9-113">Der Inhalt des Elements.</span><span class="sxs-lookup"><span data-stu-id="a45c9-113">The content of the item.</span></span>|
|<span data-ttu-id="a45c9-114">contentType</span><span class="sxs-lookup"><span data-stu-id="a45c9-114">contentType</span></span>|<span data-ttu-id="a45c9-115">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a45c9-115">String</span></span>|<span data-ttu-id="a45c9-p102">Der Typ des Inhalts. Mögliche Werte sind `Text` und `HTML`.</span><span class="sxs-lookup"><span data-stu-id="a45c9-p102">The type of the content. Possible values are `Text` and `HTML`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a45c9-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="a45c9-118">JSON representation</span></span>

<span data-ttu-id="a45c9-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="a45c9-119">Here is a JSON representation of the resource</span></span>

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
