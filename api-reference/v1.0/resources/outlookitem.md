---
title: outlookItem-Ressourcentyp
description: Es folgt eine JSON-Darstellung der Ressource.
author: angelgolfer-ms
ms.openlocfilehash: 750239156e6f4e2874783ae160a7018fb58e259d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27332515"
---
# <a name="outlookitem-resource-type"></a><span data-ttu-id="1f7aa-103">outlookItem-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="1f7aa-103">outlookItem resource type</span></span>



## <a name="json-representation"></a><span data-ttu-id="1f7aa-104">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="1f7aa-104">JSON representation</span></span>

<span data-ttu-id="1f7aa-105">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="1f7aa-105">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "abstract": true,
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.outlookItem"
}-->

```json
{
  "categories": ["string"],
  "changeKey": "string",
  "createdDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}

```
## <a name="properties"></a><span data-ttu-id="1f7aa-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="1f7aa-106">Properties</span></span>
| <span data-ttu-id="1f7aa-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1f7aa-107">Property</span></span>     | <span data-ttu-id="1f7aa-108">Typ</span><span class="sxs-lookup"><span data-stu-id="1f7aa-108">Type</span></span>   |<span data-ttu-id="1f7aa-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1f7aa-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1f7aa-110">categories</span><span class="sxs-lookup"><span data-stu-id="1f7aa-110">categories</span></span>|<span data-ttu-id="1f7aa-111">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="1f7aa-111">String collection</span></span>|<span data-ttu-id="1f7aa-112">Die Kategorien, die dem Element zugeordneten</span><span class="sxs-lookup"><span data-stu-id="1f7aa-112">The categories associated with the item</span></span>|
|<span data-ttu-id="1f7aa-113">changeKey</span><span class="sxs-lookup"><span data-stu-id="1f7aa-113">changeKey</span></span>|<span data-ttu-id="1f7aa-114">String</span><span class="sxs-lookup"><span data-stu-id="1f7aa-114">String</span></span>|<span data-ttu-id="1f7aa-115">Gibt die Version des Elements.</span><span class="sxs-lookup"><span data-stu-id="1f7aa-115">Identifies the version of the item.</span></span> <span data-ttu-id="1f7aa-116">Jedes Mal, wenn das Element geändert wird, ändert ChangeKey sowie.</span><span class="sxs-lookup"><span data-stu-id="1f7aa-116">Every time the item is changed, changeKey changes as well.</span></span> <span data-ttu-id="1f7aa-117">Dies ermöglicht Exchange zu Änderungen an die richtige Version des Objekts zu übernehmen.</span><span class="sxs-lookup"><span data-stu-id="1f7aa-117">This allows Exchange to apply changes to the correct version of the object.</span></span> <span data-ttu-id="1f7aa-118">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="1f7aa-118">Read-only.</span></span>|
|<span data-ttu-id="1f7aa-119">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1f7aa-119">createdDateTime</span></span>|<span data-ttu-id="1f7aa-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1f7aa-120">DateTimeOffset</span></span>|<span data-ttu-id="1f7aa-p102">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="1f7aa-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="1f7aa-123">id</span><span class="sxs-lookup"><span data-stu-id="1f7aa-123">id</span></span>|<span data-ttu-id="1f7aa-124">String</span><span class="sxs-lookup"><span data-stu-id="1f7aa-124">String</span></span>| <span data-ttu-id="1f7aa-125">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="1f7aa-125">Read-only.</span></span>|
|<span data-ttu-id="1f7aa-126">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1f7aa-126">lastModifiedDateTime</span></span>|<span data-ttu-id="1f7aa-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1f7aa-127">DateTimeOffset</span></span>|<span data-ttu-id="1f7aa-p103">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="1f7aa-p103">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="relationships"></a><span data-ttu-id="1f7aa-130">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="1f7aa-130">Relationships</span></span>
<span data-ttu-id="1f7aa-131">Keine</span><span class="sxs-lookup"><span data-stu-id="1f7aa-131">None</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "outlookItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
