---
title: OnenoteEntitySchemaObjectModel-Ressource
description: Dies ist ein Basistyp für OneNote-Entitäten.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 168359bbdaa659db461aa33af96e402a4a81783d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27978711"
---
# <a name="onenoteentityschemaobjectmodel-resource"></a><span data-ttu-id="0f90f-103">OnenoteEntitySchemaObjectModel-Ressource</span><span class="sxs-lookup"><span data-stu-id="0f90f-103">onenoteEntitySchemaObjectModel resource</span></span>

<span data-ttu-id="0f90f-104">Dies ist ein Basistyp für OneNote-Entitäten.</span><span class="sxs-lookup"><span data-stu-id="0f90f-104">This is a base type for OneNote entities.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0f90f-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="0f90f-105">JSON representation</span></span>

<span data-ttu-id="0f90f-106">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="0f90f-106">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "abstract": true,
  "baseType": "microsoft.graph.onenoteEntityBaseModel",
  "optionalProperties": [
    "self"
  ],
  "@odata.type": "microsoft.graph.onenoteEntitySchemaObjectModel"
}-->

```json
{
  "createdDateTime": "String (timestamp)"
}

```
## <a name="properties"></a><span data-ttu-id="0f90f-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="0f90f-107">Properties</span></span>
| <span data-ttu-id="0f90f-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0f90f-108">Property</span></span>     | <span data-ttu-id="0f90f-109">Typ</span><span class="sxs-lookup"><span data-stu-id="0f90f-109">Type</span></span>   |<span data-ttu-id="0f90f-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0f90f-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0f90f-111">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0f90f-111">createdDateTime</span></span>|<span data-ttu-id="0f90f-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0f90f-112">DateTimeOffset</span></span>|<span data-ttu-id="0f90f-p101">Das Datum und die Uhrzeit der Erstellung der Seite. Der Zeitstempel stellt die Datums- und Uhrzeitinformationen im ISO 8601-Format dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="0f90f-p101">The date and time when the page was created. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|

<!-- uuid: bfb567de-2a2a-4b81-bf47-a55626a0c166
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "page resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
