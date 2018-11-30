---
title: AddIn Ressourcentyp
description: Es folgt eine JSON-Darstellung der Ressource.
ms.openlocfilehash: c95f6bcc7fa26d77bc5a9595a6c80d0c4a94769c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063806"
---
# <a name="addin-resource-type"></a><span data-ttu-id="9da89-103">AddIn Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="9da89-103">addIn resource type</span></span>

> <span data-ttu-id="9da89-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="9da89-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9da89-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9da89-105">Use of these APIs in production applications is not supported.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9da89-106">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="9da89-106">JSON representation</span></span>

<span data-ttu-id="9da89-107">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="9da89-107">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="9da89-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="9da89-108">Properties</span></span>
| <span data-ttu-id="9da89-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9da89-109">Property</span></span>     | <span data-ttu-id="9da89-110">Typ</span><span class="sxs-lookup"><span data-stu-id="9da89-110">Type</span></span>   |<span data-ttu-id="9da89-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9da89-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9da89-112">id</span><span class="sxs-lookup"><span data-stu-id="9da89-112">id</span></span>|<span data-ttu-id="9da89-113">GUID</span><span class="sxs-lookup"><span data-stu-id="9da89-113">guid</span></span>||
|<span data-ttu-id="9da89-114">properties</span><span class="sxs-lookup"><span data-stu-id="9da89-114">properties</span></span>|<span data-ttu-id="9da89-115">[KeyValue](keyvalue.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="9da89-115">[keyValue](keyvalue.md) collection</span></span>||
|<span data-ttu-id="9da89-116">Typ</span><span class="sxs-lookup"><span data-stu-id="9da89-116">type</span></span>|<span data-ttu-id="9da89-117">string</span><span class="sxs-lookup"><span data-stu-id="9da89-117">string</span></span>||

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "addIn resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->