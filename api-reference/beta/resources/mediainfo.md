---
title: Ressourcentyp mediaInfo
description: Die Medieninformationen für die Aktionen für aufgefordert wird.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 217b9a5aaa88a1bbf343447fad344b322cfeb611
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27924531"
---
# <a name="mediainfo-resource-type"></a><span data-ttu-id="68db1-103">Ressourcentyp mediaInfo</span><span class="sxs-lookup"><span data-stu-id="68db1-103">mediaInfo resource type</span></span>

> <span data-ttu-id="68db1-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="68db1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="68db1-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="68db1-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="68db1-106">Die Medieninformationen für die Aktionen für aufgefordert wird.</span><span class="sxs-lookup"><span data-stu-id="68db1-106">The media information used in actions for prompts.</span></span>

## <a name="properties"></a><span data-ttu-id="68db1-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="68db1-107">Properties</span></span>
| <span data-ttu-id="68db1-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="68db1-108">Property</span></span>       | <span data-ttu-id="68db1-109">Typ</span><span class="sxs-lookup"><span data-stu-id="68db1-109">Type</span></span>    | <span data-ttu-id="68db1-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="68db1-110">Description</span></span>                      |
|:---------------|:--------|:---------------------------------|
| <span data-ttu-id="68db1-111">resourceId</span><span class="sxs-lookup"><span data-stu-id="68db1-111">resourceId</span></span>     | <span data-ttu-id="68db1-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="68db1-112">String</span></span>  | <span data-ttu-id="68db1-113">Eindeutige Identität der Ressource.</span><span class="sxs-lookup"><span data-stu-id="68db1-113">Unique identity of the resource.</span></span> |
| <span data-ttu-id="68db1-114">uri</span><span class="sxs-lookup"><span data-stu-id="68db1-114">uri</span></span>            | <span data-ttu-id="68db1-115">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="68db1-115">String</span></span>  | <span data-ttu-id="68db1-116">Pfad zu der Ressource.</span><span class="sxs-lookup"><span data-stu-id="68db1-116">Path to the resource.</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="68db1-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="68db1-117">JSON representation</span></span>

<span data-ttu-id="68db1-118">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="68db1-118">The following is a JSON representation of the resource.</span></span>

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
