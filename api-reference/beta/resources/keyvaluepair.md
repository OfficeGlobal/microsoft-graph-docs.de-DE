---
title: keyValuePair-Ressourcentyp
description: Schlüssel-Wert-Paar für Action-Parameter.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 86a5415c20721f717947238838341345ec9a4250
ms.sourcegitcommit: 88ddd033de0f36eedade277d57c922ebd0db5bba
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/02/2019
ms.locfileid: "30366938"
---
# <a name="keyvaluepair-resource-type"></a><span data-ttu-id="bdfe6-103">keyValuePair-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="bdfe6-103">keyValuePair resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bdfe6-104">Schlüssel-Wert-Paar für Action-Parameter.</span><span class="sxs-lookup"><span data-stu-id="bdfe6-104">Key value pair for action parameters.</span></span>

## <a name="properties"></a><span data-ttu-id="bdfe6-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="bdfe6-105">Properties</span></span>

| <span data-ttu-id="bdfe6-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="bdfe6-106">Property</span></span>     | <span data-ttu-id="bdfe6-107">Typ</span><span class="sxs-lookup"><span data-stu-id="bdfe6-107">Type</span></span>        | <span data-ttu-id="bdfe6-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bdfe6-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="bdfe6-109">name</span><span class="sxs-lookup"><span data-stu-id="bdfe6-109">name</span></span>|<span data-ttu-id="bdfe6-110">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bdfe6-110">String</span></span>|<span data-ttu-id="bdfe6-111">Namen für dieses Schlüssel-Wert-Paar</span><span class="sxs-lookup"><span data-stu-id="bdfe6-111">Name for this key-value pair</span></span>|
|<span data-ttu-id="bdfe6-112">Wert</span><span class="sxs-lookup"><span data-stu-id="bdfe6-112">value</span></span>|<span data-ttu-id="bdfe6-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bdfe6-113">String</span></span>|<span data-ttu-id="bdfe6-114">Wert für dieses Schlüssel-Wert-Paar</span><span class="sxs-lookup"><span data-stu-id="bdfe6-114">Value for this key-value pair</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bdfe6-115">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="bdfe6-115">JSON representation</span></span>

<span data-ttu-id="bdfe6-116">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="bdfe6-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.keyValuePair",
  "baseType": null
}-->

```json
{
  "name": "String",
  "value": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "keyValuePair resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->