---
title: responseStatus-Ressourcentyp
description: Der Antwortstatus einer Besprechungsanfrage.
localization_priority: Normal
ms.openlocfilehash: 110b0eb158043b9573deb3e3ced792119bfa91a7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27830779"
---
# <a name="responsestatus-resource-type"></a><span data-ttu-id="cb82d-103">responseStatus-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="cb82d-103">responseStatus resource type</span></span>

<span data-ttu-id="cb82d-104">Der Antwortstatus einer Besprechungsanfrage.</span><span class="sxs-lookup"><span data-stu-id="cb82d-104">The response status of a meeting request.</span></span>

## <a name="properties"></a><span data-ttu-id="cb82d-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="cb82d-105">Properties</span></span>

| <span data-ttu-id="cb82d-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="cb82d-106">Property</span></span> | <span data-ttu-id="cb82d-107">Typ</span><span class="sxs-lookup"><span data-stu-id="cb82d-107">Type</span></span>           | <span data-ttu-id="cb82d-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cb82d-108">Description</span></span> |
|:---------|:---------------|:------------|
| <span data-ttu-id="cb82d-109">Antwort</span><span class="sxs-lookup"><span data-stu-id="cb82d-109">response</span></span> | <span data-ttu-id="cb82d-110">responseType</span><span class="sxs-lookup"><span data-stu-id="cb82d-110">responseType</span></span>   | <span data-ttu-id="cb82d-111">Der Antworttyp.</span><span class="sxs-lookup"><span data-stu-id="cb82d-111">The response type.</span></span> <span data-ttu-id="cb82d-112">Die möglichen Werte sind: `None`, `Organizer`, `TentativelyAccepted`, `Accepted`, `Declined`, `NotResponded`.</span><span class="sxs-lookup"><span data-stu-id="cb82d-112">The possible values are: `None`, `Organizer`, `TentativelyAccepted`, `Accepted`, `Declined`, `NotResponded`.</span></span>
| <span data-ttu-id="cb82d-113">Uhrzeit</span><span class="sxs-lookup"><span data-stu-id="cb82d-113">time</span></span>     | <span data-ttu-id="cb82d-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cb82d-114">DateTimeOffset</span></span> | <span data-ttu-id="cb82d-p102">Datum und Uhrzeit, an dem bzw. der die Antwort zurückgegeben wurde. Hierfür wird das ISO 8601-Format, und die Angabe erfolgt immer in UTC-Zeit. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="cb82d-p102">The date and time that the response was returned. It uses ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>

## <a name="json-representation"></a><span data-ttu-id="cb82d-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="cb82d-118">JSON representation</span></span>

<span data-ttu-id="cb82d-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="cb82d-119">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.responseStatus"
}-->

```json
{
  "response": "String",
  "time": "String (timestamp)"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "responseStatus resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
