---
title: outlookItem-Ressourcentyp
description: Es folgt eine JSON-Darstellung der Ressource.
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: b88a450465798386ad57e82ff76896417301a606
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27817633"
---
# <a name="outlookitem-resource-type"></a><span data-ttu-id="cbee6-103">outlookItem-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="cbee6-103">outlookItem resource type</span></span>

> <span data-ttu-id="cbee6-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="cbee6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cbee6-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="cbee6-105">Use of these APIs in production applications is not supported.</span></span>

## <a name="json-representation"></a><span data-ttu-id="cbee6-106">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="cbee6-106">JSON representation</span></span>

<span data-ttu-id="cbee6-107">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="cbee6-107">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="cbee6-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="cbee6-108">Properties</span></span>
| <span data-ttu-id="cbee6-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="cbee6-109">Property</span></span>     | <span data-ttu-id="cbee6-110">Typ</span><span class="sxs-lookup"><span data-stu-id="cbee6-110">Type</span></span>   |<span data-ttu-id="cbee6-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cbee6-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cbee6-112">categories</span><span class="sxs-lookup"><span data-stu-id="cbee6-112">categories</span></span>|<span data-ttu-id="cbee6-113">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="cbee6-113">String collection</span></span>||
|<span data-ttu-id="cbee6-114">changeKey</span><span class="sxs-lookup"><span data-stu-id="cbee6-114">changeKey</span></span>|<span data-ttu-id="cbee6-115">String</span><span class="sxs-lookup"><span data-stu-id="cbee6-115">String</span></span>||
|<span data-ttu-id="cbee6-116">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cbee6-116">createdDateTime</span></span>|<span data-ttu-id="cbee6-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cbee6-117">DateTimeOffset</span></span>|<span data-ttu-id="cbee6-p102">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="cbee6-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="cbee6-120">id</span><span class="sxs-lookup"><span data-stu-id="cbee6-120">id</span></span>|<span data-ttu-id="cbee6-121">String</span><span class="sxs-lookup"><span data-stu-id="cbee6-121">String</span></span>| <span data-ttu-id="cbee6-122">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="cbee6-122">Read-only.</span></span>|
|<span data-ttu-id="cbee6-123">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cbee6-123">lastModifiedDateTime</span></span>|<span data-ttu-id="cbee6-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cbee6-124">DateTimeOffset</span></span>|<span data-ttu-id="cbee6-p103">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="cbee6-p103">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="relationships"></a><span data-ttu-id="cbee6-127">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="cbee6-127">Relationships</span></span>
<span data-ttu-id="cbee6-128">Keine</span><span class="sxs-lookup"><span data-stu-id="cbee6-128">None</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "outlookItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
