---
title: outlookItem-Ressourcentyp
description: Es folgt eine JSON-Darstellung der Ressource.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 3bbfe6119d279a1a708b44128a7d134664d7b040
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27967049"
---
# <a name="outlookitem-resource-type"></a><span data-ttu-id="8b13a-103">outlookItem-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="8b13a-103">outlookItem resource type</span></span>



## <a name="json-representation"></a><span data-ttu-id="8b13a-104">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="8b13a-104">JSON representation</span></span>

<span data-ttu-id="8b13a-105">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="8b13a-105">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="8b13a-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="8b13a-106">Properties</span></span>
| <span data-ttu-id="8b13a-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8b13a-107">Property</span></span>     | <span data-ttu-id="8b13a-108">Typ</span><span class="sxs-lookup"><span data-stu-id="8b13a-108">Type</span></span>   |<span data-ttu-id="8b13a-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8b13a-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8b13a-110">categories</span><span class="sxs-lookup"><span data-stu-id="8b13a-110">categories</span></span>|<span data-ttu-id="8b13a-111">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="8b13a-111">String collection</span></span>|<span data-ttu-id="8b13a-112">Die Kategorien, die dem Element zugeordneten</span><span class="sxs-lookup"><span data-stu-id="8b13a-112">The categories associated with the item</span></span>|
|<span data-ttu-id="8b13a-113">changeKey</span><span class="sxs-lookup"><span data-stu-id="8b13a-113">changeKey</span></span>|<span data-ttu-id="8b13a-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8b13a-114">String</span></span>|<span data-ttu-id="8b13a-115">Gibt die Version des Elements.</span><span class="sxs-lookup"><span data-stu-id="8b13a-115">Identifies the version of the item.</span></span> <span data-ttu-id="8b13a-116">Jedes Mal, wenn das Element geändert wird, ändert ChangeKey sowie.</span><span class="sxs-lookup"><span data-stu-id="8b13a-116">Every time the item is changed, changeKey changes as well.</span></span> <span data-ttu-id="8b13a-117">Dies ermöglicht Exchange zu Änderungen an die richtige Version des Objekts zu übernehmen.</span><span class="sxs-lookup"><span data-stu-id="8b13a-117">This allows Exchange to apply changes to the correct version of the object.</span></span> <span data-ttu-id="8b13a-118">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="8b13a-118">Read-only.</span></span>|
|<span data-ttu-id="8b13a-119">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8b13a-119">createdDateTime</span></span>|<span data-ttu-id="8b13a-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8b13a-120">DateTimeOffset</span></span>|<span data-ttu-id="8b13a-p102">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="8b13a-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="8b13a-123">id</span><span class="sxs-lookup"><span data-stu-id="8b13a-123">id</span></span>|<span data-ttu-id="8b13a-124">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8b13a-124">String</span></span>| <span data-ttu-id="8b13a-125">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="8b13a-125">Read-only.</span></span>|
|<span data-ttu-id="8b13a-126">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8b13a-126">lastModifiedDateTime</span></span>|<span data-ttu-id="8b13a-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8b13a-127">DateTimeOffset</span></span>|<span data-ttu-id="8b13a-p103">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="8b13a-p103">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="relationships"></a><span data-ttu-id="8b13a-130">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="8b13a-130">Relationships</span></span>
<span data-ttu-id="8b13a-131">Keine</span><span class="sxs-lookup"><span data-stu-id="8b13a-131">None</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "outlookItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
