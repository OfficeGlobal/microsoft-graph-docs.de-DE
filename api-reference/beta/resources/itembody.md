---
title: itemBody-Ressourcentyp
description: Stellt Eigenschaften des Textkörpers eines Elements dar, z. B. eine Nachricht, ein Ereignis oder ein Gruppenbeitrag.
localization_priority: Normal
ms.openlocfilehash: 791906c8442250d05d1b94b9eb9b19320f45e9c9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27872142"
---
# <a name="itembody-resource-type"></a><span data-ttu-id="1dc78-103">itemBody-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="1dc78-103">itemBody resource type</span></span>

> <span data-ttu-id="1dc78-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="1dc78-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1dc78-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1dc78-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1dc78-106">Stellt Eigenschaften des Textkörpers eines Elements dar, z. B. eine Nachricht, ein Ereignis oder ein Gruppenbeitrag.</span><span class="sxs-lookup"><span data-stu-id="1dc78-106">Represents properties of the body of an item, such as a message, event or group post.</span></span>

## <a name="properties"></a><span data-ttu-id="1dc78-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="1dc78-107">Properties</span></span>
| <span data-ttu-id="1dc78-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1dc78-108">Property</span></span>     | <span data-ttu-id="1dc78-109">Typ</span><span class="sxs-lookup"><span data-stu-id="1dc78-109">Type</span></span>   |<span data-ttu-id="1dc78-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1dc78-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1dc78-111">Inhalt</span><span class="sxs-lookup"><span data-stu-id="1dc78-111">content</span></span>|<span data-ttu-id="1dc78-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1dc78-112">String</span></span>|<span data-ttu-id="1dc78-113">Der Inhalt des Elements.</span><span class="sxs-lookup"><span data-stu-id="1dc78-113">The content of the item.</span></span>|
|<span data-ttu-id="1dc78-114">contentType</span><span class="sxs-lookup"><span data-stu-id="1dc78-114">contentType</span></span>|<span data-ttu-id="1dc78-115">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1dc78-115">String</span></span>|<span data-ttu-id="1dc78-p102">Der Typ des Inhalts. Mögliche Werte sind `Text` und `HTML`.</span><span class="sxs-lookup"><span data-stu-id="1dc78-p102">The type of the content. Possible values are `Text` and `HTML`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1dc78-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="1dc78-118">JSON representation</span></span>

<span data-ttu-id="1dc78-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="1dc78-119">Here is a JSON representation of the resource</span></span>

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
