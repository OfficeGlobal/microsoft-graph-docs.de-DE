---
title: Ressourcentyp callRoute
description: Der Typ des CallRoute.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: cfa470c4d3a03655221cab1f29baa60d00a8cf6c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512801"
---
# <a name="callroute-resource-type"></a><span data-ttu-id="2cf85-103">Ressourcentyp callRoute</span><span class="sxs-lookup"><span data-stu-id="2cf85-103">callRoute resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2cf85-104">Der Typ des CallRoute.</span><span class="sxs-lookup"><span data-stu-id="2cf85-104">The callRoute type.</span></span>

## <a name="properties"></a><span data-ttu-id="2cf85-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="2cf85-105">Properties</span></span>

| <span data-ttu-id="2cf85-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2cf85-106">Property</span></span>            | <span data-ttu-id="2cf85-107">Typ</span><span class="sxs-lookup"><span data-stu-id="2cf85-107">Type</span></span>                          | <span data-ttu-id="2cf85-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2cf85-108">Description</span></span>                                                  |
| :------------------ | :---------------------------- | :----------------------------------------------------------- |
| <span data-ttu-id="2cf85-109">Final</span><span class="sxs-lookup"><span data-stu-id="2cf85-109">final</span></span>               | [<span data-ttu-id="2cf85-110">identitySet</span><span class="sxs-lookup"><span data-stu-id="2cf85-110">identitySet</span></span>](identityset.md) | <span data-ttu-id="2cf85-111">Die Identität, die in die Unterhaltung aufgelöst wurde.</span><span class="sxs-lookup"><span data-stu-id="2cf85-111">The identity that was resolved to in the call.</span></span>               |
| <span data-ttu-id="2cf85-112">Original</span><span class="sxs-lookup"><span data-stu-id="2cf85-112">original</span></span>            | [<span data-ttu-id="2cf85-113">identitySet</span><span class="sxs-lookup"><span data-stu-id="2cf85-113">identitySet</span></span>](identityset.md) | <span data-ttu-id="2cf85-114">Die Identität, die ursprünglich in den Anruf verwendet wurde.</span><span class="sxs-lookup"><span data-stu-id="2cf85-114">The identity that was originally used in the call.</span></span>           |
| <span data-ttu-id="2cf85-115">routingType</span><span class="sxs-lookup"><span data-stu-id="2cf85-115">routingType</span></span>         | <span data-ttu-id="2cf85-116">String</span><span class="sxs-lookup"><span data-stu-id="2cf85-116">String</span></span>                        | <span data-ttu-id="2cf85-117">Mögliche Werte sind: `forwarded`, `lookup` und `selfFork`.</span><span class="sxs-lookup"><span data-stu-id="2cf85-117">Possible values are: `forwarded`, `lookup`, `selfFork`.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="2cf85-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="2cf85-118">JSON representation</span></span>

<span data-ttu-id="2cf85-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="2cf85-119">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRoute"
}-->
```json
{
  "final": {"@odata.type": "#microsoft.graph.identitySet"},
  "original": {"@odata.type": "#microsoft.graph.identitySet"},
  "routingType": "forwarded | lookup | selfFork"
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "callRoute resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/callroute.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
