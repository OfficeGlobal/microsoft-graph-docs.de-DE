---
title: RangeSort-Ressourcentyp
description: Verwaltet Sortiervorgänge für Range-Objekte.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: c52b4c6cc50bce7d518d26798db9f3d3da49cd1c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27816429"
---
# <a name="rangesort-resource-type"></a><span data-ttu-id="30be9-103">RangeSort-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="30be9-103">RangeSort resource type</span></span>

<span data-ttu-id="30be9-104">Verwaltet Sortiervorgänge für Range-Objekte.</span><span class="sxs-lookup"><span data-stu-id="30be9-104">Manages sorting operations on Range objects.</span></span>


## <a name="methods"></a><span data-ttu-id="30be9-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="30be9-105">Methods</span></span>

| <span data-ttu-id="30be9-106">Methode</span><span class="sxs-lookup"><span data-stu-id="30be9-106">Method</span></span>           | <span data-ttu-id="30be9-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="30be9-107">Return Type</span></span>    |<span data-ttu-id="30be9-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="30be9-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="30be9-109">Apply</span><span class="sxs-lookup"><span data-stu-id="30be9-109">Apply</span></span>](../api/rangesort-apply.md)|<span data-ttu-id="30be9-110">Keine</span><span class="sxs-lookup"><span data-stu-id="30be9-110">None</span></span>|<span data-ttu-id="30be9-111">Führt einen Sortiervorgang aus.</span><span class="sxs-lookup"><span data-stu-id="30be9-111">Perform a sort operation.</span></span>|

## <a name="properties"></a><span data-ttu-id="30be9-112">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="30be9-112">Properties</span></span>
<span data-ttu-id="30be9-113">Keine</span><span class="sxs-lookup"><span data-stu-id="30be9-113">None</span></span>

## <a name="relationships"></a><span data-ttu-id="30be9-114">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="30be9-114">Relationships</span></span>
<span data-ttu-id="30be9-115">Keine</span><span class="sxs-lookup"><span data-stu-id="30be9-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="30be9-116">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="30be9-116">JSON representation</span></span>

<span data-ttu-id="30be9-117">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="30be9-117">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookRangeSort"
}-->

```json
{
}
```

##### <a name="request"></a><span data-ttu-id="30be9-118">Anforderung</span><span class="sxs-lookup"><span data-stu-id="30be9-118">Request</span></span>
<span data-ttu-id="30be9-119">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="30be9-119">Here is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "name": "range_sort"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/sort
```

##### <a name="response"></a><span data-ttu-id="30be9-120">Antwort</span><span class="sxs-lookup"><span data-stu-id="30be9-120">Response</span></span>
<span data-ttu-id="30be9-121">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="30be9-121">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeSort"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "RangeSort resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
