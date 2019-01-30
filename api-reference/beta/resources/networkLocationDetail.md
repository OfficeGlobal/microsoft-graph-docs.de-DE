---
title: Ressourcentyp networkLocationDetail
description: Gibt den Speicherort im Netzwerk zugeordneten Details an. .
localization_priority: Normal
ms.openlocfilehash: bfa84591f543253ed794016bbc2d25d325cd0bcc
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/30/2019
ms.locfileid: "29643762"
---
# <a name="networklocationdetail-resource-type"></a><span data-ttu-id="d43a5-104">Ressourcentyp networkLocationDetail</span><span class="sxs-lookup"><span data-stu-id="d43a5-104">networkLocationDetail resource type</span></span>
<span data-ttu-id="d43a5-105">Gibt den Speicherort im Netzwerk zugeordneten Details an.</span><span class="sxs-lookup"><span data-stu-id="d43a5-105">Indicates details associated with the network location.</span></span> <span data-ttu-id="d43a5-106">.</span><span class="sxs-lookup"><span data-stu-id="d43a5-106"></span></span>



## <a name="properties"></a><span data-ttu-id="d43a5-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d43a5-107">Properties</span></span>
| <span data-ttu-id="d43a5-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d43a5-108">Property</span></span>     | <span data-ttu-id="d43a5-109">Typ</span><span class="sxs-lookup"><span data-stu-id="d43a5-109">Type</span></span>   |<span data-ttu-id="d43a5-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d43a5-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d43a5-111">networkType</span><span class="sxs-lookup"><span data-stu-id="d43a5-111">networkType</span></span>|<span data-ttu-id="d43a5-112">String</span><span class="sxs-lookup"><span data-stu-id="d43a5-112">String</span></span>|<span data-ttu-id="d43a5-113">Stellt den Typ des Netzwerks.</span><span class="sxs-lookup"><span data-stu-id="d43a5-113">Provides the type of the network.</span></span> <span data-ttu-id="d43a5-114">Mögliche Werte sind `intranet`, `extranet`, `namedNetwork`, und `trusted`.</span><span class="sxs-lookup"><span data-stu-id="d43a5-114">Possible values are `intranet`, `extranet`, `namedNetwork`, and `trusted`.</span></span>|
|<span data-ttu-id="d43a5-115">Netzwerkname</span><span class="sxs-lookup"><span data-stu-id="d43a5-115">networkName</span></span>|<span data-ttu-id="d43a5-116">String</span><span class="sxs-lookup"><span data-stu-id="d43a5-116">String</span></span>|<span data-ttu-id="d43a5-117">Name des Netzwerks.</span><span class="sxs-lookup"><span data-stu-id="d43a5-117">Name of the network.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="d43a5-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d43a5-118">JSON representation</span></span>

<span data-ttu-id="d43a5-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d43a5-119">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.deviceDetail"
}-->

```json
{
  "networkTypes": "namedNetork",
  "networkName": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "deviceDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
