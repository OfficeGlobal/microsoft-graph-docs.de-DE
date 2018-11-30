---
title: sizeRange-Ressourcentyp
description: Gibt die maximale und minimale Größe (in Kilobyte) an, die eine eingehende Nachrichten aufweisen muss, damit eine Bedingung oder Ausnahme zutrifft.
ms.openlocfilehash: c84843116055c8ef13b7961b6ee180c4c896c80f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063658"
---
# <a name="sizerange-resource-type"></a><span data-ttu-id="a9c06-103">sizeRange-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="a9c06-103">sizeRange resource type</span></span>

> <span data-ttu-id="a9c06-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="a9c06-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a9c06-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a9c06-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a9c06-106">Gibt die maximale und minimale Größe (in Kilobyte) an, die eine eingehende Nachrichten aufweisen muss, damit eine Bedingung oder Ausnahme zutrifft.</span><span class="sxs-lookup"><span data-stu-id="a9c06-106">Specifies the maximum and minimum sizes (in kilobytes) that an incoming message must have in order for a condition or exception to apply.</span></span>

## <a name="properties"></a><span data-ttu-id="a9c06-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="a9c06-107">Properties</span></span>
| <span data-ttu-id="a9c06-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a9c06-108">Property</span></span>     | <span data-ttu-id="a9c06-109">Typ</span><span class="sxs-lookup"><span data-stu-id="a9c06-109">Type</span></span>   |<span data-ttu-id="a9c06-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a9c06-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a9c06-111">maximumSize</span><span class="sxs-lookup"><span data-stu-id="a9c06-111">maximumSize</span></span> | <span data-ttu-id="a9c06-112">Int32</span><span class="sxs-lookup"><span data-stu-id="a9c06-112">Int32</span></span> | <span data-ttu-id="a9c06-113">Die maximale Größe (in Kilobyte), die eine eingehende Nachrichten aufweisen muss, damit eine Bedingung oder Ausnahme zutrifft.</span><span class="sxs-lookup"><span data-stu-id="a9c06-113">The maximum size (in kilobytes) that an incoming message must have in order for a condition or exception to apply.</span></span> |
| <span data-ttu-id="a9c06-114">minimumSize</span><span class="sxs-lookup"><span data-stu-id="a9c06-114">minimumSize</span></span> | <span data-ttu-id="a9c06-115">Int32</span><span class="sxs-lookup"><span data-stu-id="a9c06-115">Int32</span></span> | <span data-ttu-id="a9c06-116">Die minimale Größe (in Kilobyte), die eine eingehende Nachrichten aufweisen muss, damit eine Bedingung oder Ausnahme zutrifft.</span><span class="sxs-lookup"><span data-stu-id="a9c06-116">The minimum size (in kilobytes) that an incoming message must have in order for a condition or exception to apply.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="a9c06-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="a9c06-117">JSON representation</span></span>
<span data-ttu-id="a9c06-118">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="a9c06-118">Here is a JSON representation of the resource.</span></span>

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