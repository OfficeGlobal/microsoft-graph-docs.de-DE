---
title: sizeRange-Ressourcentyp
description: Gibt die maximale und minimale Größe (in Kilobyte) an, die eine eingehende Nachrichten aufweisen muss, damit eine Bedingung oder Ausnahme zutrifft.
localization_priority: Normal
ms.openlocfilehash: ae754d0666185023272860864ef17f038aecff7c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27873542"
---
# <a name="sizerange-resource-type"></a><span data-ttu-id="c258a-103">sizeRange-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="c258a-103">sizeRange resource type</span></span>


<span data-ttu-id="c258a-104">Gibt die maximale und minimale Größe (in Kilobyte) an, die eine eingehende Nachrichten aufweisen muss, damit eine Bedingung oder Ausnahme zutrifft.</span><span class="sxs-lookup"><span data-stu-id="c258a-104">Specifies the maximum and minimum sizes (in kilobytes) that an incoming message must have in order for a condition or exception to apply.</span></span>

## <a name="properties"></a><span data-ttu-id="c258a-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="c258a-105">Properties</span></span>
| <span data-ttu-id="c258a-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c258a-106">Property</span></span>     | <span data-ttu-id="c258a-107">Typ</span><span class="sxs-lookup"><span data-stu-id="c258a-107">Type</span></span>   |<span data-ttu-id="c258a-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c258a-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c258a-109">maximumSize</span><span class="sxs-lookup"><span data-stu-id="c258a-109">maximumSize</span></span> | <span data-ttu-id="c258a-110">Int32</span><span class="sxs-lookup"><span data-stu-id="c258a-110">Int32</span></span> | <span data-ttu-id="c258a-111">Die maximale Größe (in Kilobyte), die eine eingehende Nachrichten aufweisen muss, damit eine Bedingung oder Ausnahme zutrifft.</span><span class="sxs-lookup"><span data-stu-id="c258a-111">The maximum size (in kilobytes) that an incoming message must have in order for a condition or exception to apply.</span></span> |
| <span data-ttu-id="c258a-112">minimumSize</span><span class="sxs-lookup"><span data-stu-id="c258a-112">minimumSize</span></span> | <span data-ttu-id="c258a-113">Int32</span><span class="sxs-lookup"><span data-stu-id="c258a-113">Int32</span></span> | <span data-ttu-id="c258a-114">Die minimale Größe (in Kilobyte), die eine eingehende Nachrichten aufweisen muss, damit eine Bedingung oder Ausnahme zutrifft.</span><span class="sxs-lookup"><span data-stu-id="c258a-114">The minimum size (in kilobytes) that an incoming message must have in order for a condition or exception to apply.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="c258a-115">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="c258a-115">JSON representation</span></span>
<span data-ttu-id="c258a-116">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="c258a-116">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
   ],
  "@odata.type": "microsoft.graph.sizeRange"
}-->

```json
{
  "maximumSize": "Int32",
  "minimumSize": "Int32"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "sizeRange resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
