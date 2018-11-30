---
title: RangeSort-Ressourcentyp
description: Verwaltet Sortiervorgänge für Range-Objekte.
ms.openlocfilehash: 09f9a6763c634ee12251651a650d29528a534084
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017022"
---
# <a name="rangesort-resource-type"></a><span data-ttu-id="3b2a7-103">RangeSort-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="3b2a7-103">RangeSort resource type</span></span>

<span data-ttu-id="3b2a7-104">Verwaltet Sortiervorgänge für Range-Objekte.</span><span class="sxs-lookup"><span data-stu-id="3b2a7-104">Manages sorting operations on Range objects.</span></span>


## <a name="methods"></a><span data-ttu-id="3b2a7-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="3b2a7-105">Methods</span></span>

| <span data-ttu-id="3b2a7-106">Methode</span><span class="sxs-lookup"><span data-stu-id="3b2a7-106">Method</span></span>           | <span data-ttu-id="3b2a7-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="3b2a7-107">Return Type</span></span>    |<span data-ttu-id="3b2a7-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3b2a7-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3b2a7-109">Apply</span><span class="sxs-lookup"><span data-stu-id="3b2a7-109">Apply</span></span>](../api/rangesort-apply.md)|<span data-ttu-id="3b2a7-110">Keine</span><span class="sxs-lookup"><span data-stu-id="3b2a7-110">None</span></span>|<span data-ttu-id="3b2a7-111">Führt einen Sortiervorgang aus.</span><span class="sxs-lookup"><span data-stu-id="3b2a7-111">Perform a sort operation.</span></span>|

## <a name="properties"></a><span data-ttu-id="3b2a7-112">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="3b2a7-112">Properties</span></span>
<span data-ttu-id="3b2a7-113">Keine</span><span class="sxs-lookup"><span data-stu-id="3b2a7-113">None</span></span>

## <a name="relationships"></a><span data-ttu-id="3b2a7-114">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="3b2a7-114">Relationships</span></span>
<span data-ttu-id="3b2a7-115">Keine</span><span class="sxs-lookup"><span data-stu-id="3b2a7-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3b2a7-116">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="3b2a7-116">JSON representation</span></span>

<span data-ttu-id="3b2a7-117">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="3b2a7-117">Here is a JSON representation of the resource.</span></span>

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

##### <a name="request"></a><span data-ttu-id="3b2a7-118">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3b2a7-118">Request</span></span>
<span data-ttu-id="3b2a7-119">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3b2a7-119">Here is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "name": "range_sort"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/sort
```

##### <a name="response"></a><span data-ttu-id="3b2a7-120">Antwort</span><span class="sxs-lookup"><span data-stu-id="3b2a7-120">Response</span></span>
<span data-ttu-id="3b2a7-121">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="3b2a7-121">Here is an example of the response.</span></span> 
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