---
title: outlookItem-Ressourcentyp
description: Es folgt eine JSON-Darstellung der Ressource.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 7095be63657dacab2927abc3adb77854374c3674
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27941940"
---
# <a name="outlookitem-resource-type"></a><span data-ttu-id="7df9d-103">outlookItem-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="7df9d-103">outlookItem resource type</span></span>

> <span data-ttu-id="7df9d-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="7df9d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7df9d-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7df9d-105">Use of these APIs in production applications is not supported.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7df9d-106">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="7df9d-106">JSON representation</span></span>

<span data-ttu-id="7df9d-107">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="7df9d-107">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="7df9d-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="7df9d-108">Properties</span></span>
| <span data-ttu-id="7df9d-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7df9d-109">Property</span></span>     | <span data-ttu-id="7df9d-110">Typ</span><span class="sxs-lookup"><span data-stu-id="7df9d-110">Type</span></span>   |<span data-ttu-id="7df9d-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7df9d-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7df9d-112">categories</span><span class="sxs-lookup"><span data-stu-id="7df9d-112">categories</span></span>|<span data-ttu-id="7df9d-113">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="7df9d-113">String collection</span></span>||
|<span data-ttu-id="7df9d-114">changeKey</span><span class="sxs-lookup"><span data-stu-id="7df9d-114">changeKey</span></span>|<span data-ttu-id="7df9d-115">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7df9d-115">String</span></span>||
|<span data-ttu-id="7df9d-116">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7df9d-116">createdDateTime</span></span>|<span data-ttu-id="7df9d-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7df9d-117">DateTimeOffset</span></span>|<span data-ttu-id="7df9d-p102">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="7df9d-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="7df9d-120">id</span><span class="sxs-lookup"><span data-stu-id="7df9d-120">id</span></span>|<span data-ttu-id="7df9d-121">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7df9d-121">String</span></span>| <span data-ttu-id="7df9d-122">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="7df9d-122">Read-only.</span></span>|
|<span data-ttu-id="7df9d-123">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7df9d-123">lastModifiedDateTime</span></span>|<span data-ttu-id="7df9d-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7df9d-124">DateTimeOffset</span></span>|<span data-ttu-id="7df9d-p103">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="7df9d-p103">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="relationships"></a><span data-ttu-id="7df9d-127">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="7df9d-127">Relationships</span></span>
<span data-ttu-id="7df9d-128">Keine</span><span class="sxs-lookup"><span data-stu-id="7df9d-128">None</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "outlookItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
