---
title: Ressourcentyp mediaInfo
description: Die Medieninformationen für die Aktionen für aufgefordert wird.
author: VinodRavichandran
ms.openlocfilehash: ea2eaa9e8e85da737df4c0c0170457fb3350820b
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380275"
---
# <a name="mediainfo-resource-type"></a><span data-ttu-id="07831-103">Ressourcentyp mediaInfo</span><span class="sxs-lookup"><span data-stu-id="07831-103">mediaInfo resource type</span></span>

> <span data-ttu-id="07831-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="07831-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="07831-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="07831-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="07831-106">Die Medieninformationen für die Aktionen für aufgefordert wird.</span><span class="sxs-lookup"><span data-stu-id="07831-106">The media information used in actions for prompts.</span></span>

## <a name="properties"></a><span data-ttu-id="07831-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="07831-107">Properties</span></span>
| <span data-ttu-id="07831-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="07831-108">Property</span></span>       | <span data-ttu-id="07831-109">Typ</span><span class="sxs-lookup"><span data-stu-id="07831-109">Type</span></span>    | <span data-ttu-id="07831-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="07831-110">Description</span></span>                      |
|:---------------|:--------|:---------------------------------|
| <span data-ttu-id="07831-111">resourceId</span><span class="sxs-lookup"><span data-stu-id="07831-111">resourceId</span></span>     | <span data-ttu-id="07831-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="07831-112">String</span></span>  | <span data-ttu-id="07831-113">Eindeutige Identität der Ressource.</span><span class="sxs-lookup"><span data-stu-id="07831-113">Unique identity of the resource.</span></span> |
| <span data-ttu-id="07831-114">uri</span><span class="sxs-lookup"><span data-stu-id="07831-114">uri</span></span>            | <span data-ttu-id="07831-115">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="07831-115">String</span></span>  | <span data-ttu-id="07831-116">Pfad zu der Ressource.</span><span class="sxs-lookup"><span data-stu-id="07831-116">Path to the resource.</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="07831-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="07831-117">JSON representation</span></span>

<span data-ttu-id="07831-118">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="07831-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.mediaInfo"
}-->
```json
{
  "resourceId": "String",
  "uri": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mediaInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->