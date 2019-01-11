---
title: OnenoteEntityHierarchyModel-Ressource
description: Dies ist ein Basistyp für OneNote-Entitäten.
author: Jewan-microsoft
localization_priority: Normal
ms.openlocfilehash: 9dbab25bb3afa69c434545fceaa6cbc869fb7dcc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27858877"
---
# <a name="onenoteentityhierarchymodel-resource"></a><span data-ttu-id="27dda-103">OnenoteEntityHierarchyModel-Ressource</span><span class="sxs-lookup"><span data-stu-id="27dda-103">onenoteEntityHierarchyModel resource</span></span>

<span data-ttu-id="27dda-104">Dies ist ein Basistyp für OneNote-Entitäten.</span><span class="sxs-lookup"><span data-stu-id="27dda-104">This is a base type for OneNote entities.</span></span>

## <a name="json-representation"></a><span data-ttu-id="27dda-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="27dda-105">JSON representation</span></span>

<span data-ttu-id="27dda-106">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="27dda-106">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "abstract": true,
  "baseType": "microsoft.graph.onenoteEntitySchemaObjectModel",
  "optionalProperties": [
    "self"
  ],
  "@odata.type": "microsoft.graph.onenoteEntityHierarchyModel"
}-->

```json
{
  "displayName": "string",
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)"
}

```
## <a name="properties"></a><span data-ttu-id="27dda-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="27dda-107">Properties</span></span>
## <a name="properties"></a><span data-ttu-id="27dda-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="27dda-108">Properties</span></span>
| <span data-ttu-id="27dda-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="27dda-109">Property</span></span>     | <span data-ttu-id="27dda-110">Typ</span><span class="sxs-lookup"><span data-stu-id="27dda-110">Type</span></span>   |<span data-ttu-id="27dda-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="27dda-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="27dda-112">displayName</span><span class="sxs-lookup"><span data-stu-id="27dda-112">displayName</span></span>|<span data-ttu-id="27dda-113">String</span><span class="sxs-lookup"><span data-stu-id="27dda-113">String</span></span>|<span data-ttu-id="27dda-114">Der Name des Notizbuchs.</span><span class="sxs-lookup"><span data-stu-id="27dda-114">The name of the notebook.</span></span>|
|<span data-ttu-id="27dda-115">createdBy</span><span class="sxs-lookup"><span data-stu-id="27dda-115">createdBy</span></span>|[<span data-ttu-id="27dda-116">identitySet</span><span class="sxs-lookup"><span data-stu-id="27dda-116">identitySet</span></span>](identityset.md)|<span data-ttu-id="27dda-p101">Die Identität des Benutzers, des Geräts und der Anwendung, von denen das Element erstellt wurde. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="27dda-p101">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="27dda-119">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="27dda-119">lastModifiedBy</span></span>|[<span data-ttu-id="27dda-120">identitySet</span><span class="sxs-lookup"><span data-stu-id="27dda-120">identitySet</span></span>](identityset.md)|<span data-ttu-id="27dda-p102">Die Identität des Benutzers, des Geräts und der Anwendung, von denen das Element erstellt wurde. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="27dda-p102">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="27dda-123">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="27dda-123">lastModifiedDateTime</span></span>|<span data-ttu-id="27dda-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="27dda-124">DateTimeOffset</span></span>|<span data-ttu-id="27dda-p103">Das Datum und die Uhrzeit der letzten Änderung des Notizbuchs. Der Zeitstempel stellt die Datums- und Uhrzeitinformationen im ISO 8601-Format dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="27dda-p103">The date and time when the notebook was last modified. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|

<!-- uuid: 8b1af557-1a7c-4432-86eb-94989c2d4b54
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "page resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
