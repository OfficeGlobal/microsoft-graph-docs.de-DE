---
title: outlookItem-Ressourcentyp
description: Es folgt eine JSON-Darstellung der Ressource.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 8a44f9a2e568991c6803ebf72baf5f712f39ba64
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/30/2019
ms.locfileid: "29643797"
---
# <a name="outlookitem-resource-type"></a><span data-ttu-id="db526-103">outlookItem-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="db526-103">outlookItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="json-representation"></a><span data-ttu-id="db526-104">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="db526-104">JSON representation</span></span>

<span data-ttu-id="db526-105">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="db526-105">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.outlookitem"
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
## <a name="properties"></a><span data-ttu-id="db526-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="db526-106">Properties</span></span>
| <span data-ttu-id="db526-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="db526-107">Property</span></span>     | <span data-ttu-id="db526-108">Typ</span><span class="sxs-lookup"><span data-stu-id="db526-108">Type</span></span>   |<span data-ttu-id="db526-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="db526-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="db526-110">categories</span><span class="sxs-lookup"><span data-stu-id="db526-110">categories</span></span>|<span data-ttu-id="db526-111">String collection</span><span class="sxs-lookup"><span data-stu-id="db526-111">String collection</span></span>||
|<span data-ttu-id="db526-112">changeKey</span><span class="sxs-lookup"><span data-stu-id="db526-112">changeKey</span></span>|<span data-ttu-id="db526-113">String</span><span class="sxs-lookup"><span data-stu-id="db526-113">String</span></span>||
|<span data-ttu-id="db526-114">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="db526-114">createdDateTime</span></span>|<span data-ttu-id="db526-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="db526-115">DateTimeOffset</span></span>|<span data-ttu-id="db526-p101">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="db526-p101">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="db526-118">id</span><span class="sxs-lookup"><span data-stu-id="db526-118">id</span></span>|<span data-ttu-id="db526-119">String</span><span class="sxs-lookup"><span data-stu-id="db526-119">String</span></span>| <span data-ttu-id="db526-120">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="db526-120">Read-only.</span></span>|
|<span data-ttu-id="db526-121">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="db526-121">lastModifiedDateTime</span></span>|<span data-ttu-id="db526-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="db526-122">DateTimeOffset</span></span>|<span data-ttu-id="db526-p102">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="db526-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="relationships"></a><span data-ttu-id="db526-125">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="db526-125">Relationships</span></span>
<span data-ttu-id="db526-126">Keine</span><span class="sxs-lookup"><span data-stu-id="db526-126">None</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "outlookItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/outlookitem.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
