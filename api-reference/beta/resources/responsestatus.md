---
title: responseStatus-Ressourcentyp
description: Der Antwortstatus einer Besprechungsanfrage.
localization_priority: Normal
ms.openlocfilehash: 270c432235b929af2cb55ff63e10397fea5f92fb
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528074"
---
# <a name="responsestatus-resource-type"></a><span data-ttu-id="1577a-103">responseStatus-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="1577a-103">responseStatus resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1577a-104">Der Antwortstatus einer Besprechungsanfrage.</span><span class="sxs-lookup"><span data-stu-id="1577a-104">The response status of a meeting request.</span></span>

## <a name="properties"></a><span data-ttu-id="1577a-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="1577a-105">Properties</span></span>

| <span data-ttu-id="1577a-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1577a-106">Property</span></span> | <span data-ttu-id="1577a-107">Typ</span><span class="sxs-lookup"><span data-stu-id="1577a-107">Type</span></span>           | <span data-ttu-id="1577a-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1577a-108">Description</span></span> |
|:---------|:---------------|:------------|
| <span data-ttu-id="1577a-109">Antwort</span><span class="sxs-lookup"><span data-stu-id="1577a-109">response</span></span> | <span data-ttu-id="1577a-110">String</span><span class="sxs-lookup"><span data-stu-id="1577a-110">String</span></span>         | <span data-ttu-id="1577a-111">Der Antworttyp.</span><span class="sxs-lookup"><span data-stu-id="1577a-111">The response type.</span></span> <span data-ttu-id="1577a-112">Mögliche Werte: `None`, `Organizer`, `TentativelyAccepted`, `Accepted`, `Declined`, `NotResponded`.</span><span class="sxs-lookup"><span data-stu-id="1577a-112">Possible values are: `None`, `Organizer`, `TentativelyAccepted`, `Accepted`, `Declined`, `NotResponded`.</span></span>
| <span data-ttu-id="1577a-113">Uhrzeit</span><span class="sxs-lookup"><span data-stu-id="1577a-113">time</span></span>     | <span data-ttu-id="1577a-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1577a-114">DateTimeOffset</span></span> | <span data-ttu-id="1577a-p102">Datum und Uhrzeit, an dem bzw. der die Antwort zurückgegeben wurde. Hierfür wird das ISO 8601-Format, und die Angabe erfolgt immer in UTC-Zeit. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="1577a-p102">The date and time that the response was returned. It uses ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>

## <a name="json-representation"></a><span data-ttu-id="1577a-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="1577a-118">JSON representation</span></span>

<span data-ttu-id="1577a-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="1577a-119">Here is a JSON representation of the resource</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "responseStatus resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/responsestatus.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
