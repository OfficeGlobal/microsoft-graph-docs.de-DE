---
title: Ressourcentyp stringKeyObjectValuePair
description: Schlüssel-Wert-Paar, in denen der Schlüssel ist eine Zeichenfolge und der Wert ist ein beliebiges JSON-Objekt, darstellt. Dies ist ein open OData-Typ, die eine Eigenschaft mit dem Namen haben erwartet `value` also ein gültiges JSON-Objekt.
ms.openlocfilehash: ae536b2aab87b9920c2afcbe324e30b5f5380dbb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061684"
---
# <a name="stringkeyobjectvaluepair-resource-type"></a><span data-ttu-id="7c26c-104">Ressourcentyp stringKeyObjectValuePair</span><span class="sxs-lookup"><span data-stu-id="7c26c-104">stringKeyObjectValuePair resource type</span></span>

> <span data-ttu-id="7c26c-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="7c26c-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7c26c-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7c26c-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7c26c-107">Schlüssel-Wert-Paar, in denen der Schlüssel ist eine Zeichenfolge und der Wert ist ein beliebiges JSON-Objekt, darstellt.</span><span class="sxs-lookup"><span data-stu-id="7c26c-107">Represents a key-value pair where the key is a string and the value is an arbitrary JSON object.</span></span> <span data-ttu-id="7c26c-108">Dies ist ein open OData-Typ, die eine Eigenschaft mit dem Namen haben erwartet `value` also ein gültiges JSON-Objekt.</span><span class="sxs-lookup"><span data-stu-id="7c26c-108">This is an OData open type that expects to have a property named `value` that is a valid JSON object.</span></span>

## <a name="properties"></a><span data-ttu-id="7c26c-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="7c26c-109">Properties</span></span>
| <span data-ttu-id="7c26c-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7c26c-110">Property</span></span>     | <span data-ttu-id="7c26c-111">Typ</span><span class="sxs-lookup"><span data-stu-id="7c26c-111">Type</span></span>   |<span data-ttu-id="7c26c-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7c26c-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7c26c-113">Key</span><span class="sxs-lookup"><span data-stu-id="7c26c-113">key</span></span>|<span data-ttu-id="7c26c-114">String</span><span class="sxs-lookup"><span data-stu-id="7c26c-114">String</span></span>|<span data-ttu-id="7c26c-115">Schlüssel.</span><span class="sxs-lookup"><span data-stu-id="7c26c-115">Key.</span></span>|
|<span data-ttu-id="7c26c-116">Wert</span><span class="sxs-lookup"><span data-stu-id="7c26c-116">value</span></span>|<span data-ttu-id="7c26c-117">Jede</span><span class="sxs-lookup"><span data-stu-id="7c26c-117">Any</span></span>|<span data-ttu-id="7c26c-118">Beliebige JSON-Objekt.</span><span class="sxs-lookup"><span data-stu-id="7c26c-118">Arbitrary JSON object.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7c26c-119">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="7c26c-119">JSON representation</span></span>

<span data-ttu-id="7c26c-120">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="7c26c-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.stringKeyObjectValuePair"
}-->

```json
{
  "key": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "stringKeyObjectValuePair resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->