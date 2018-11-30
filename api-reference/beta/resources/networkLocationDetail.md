---
title: Ressourcentyp networkLocationDetail
description: Gibt den Speicherort im Netzwerk zugeordneten Details an. .
ms.openlocfilehash: 5dd1410318d380a1b943de6a7dbb0d739172cc76
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062627"
---
# <a name="networklocationdetail-resource-type"></a><span data-ttu-id="3d4cf-104">Ressourcentyp networkLocationDetail</span><span class="sxs-lookup"><span data-stu-id="3d4cf-104">networkLocationDetail resource type</span></span>
<span data-ttu-id="3d4cf-105">Gibt den Speicherort im Netzwerk zugeordneten Details an.</span><span class="sxs-lookup"><span data-stu-id="3d4cf-105">Indicates details associated with the network location.</span></span> <span data-ttu-id="3d4cf-106">.</span><span class="sxs-lookup"><span data-stu-id="3d4cf-106"></span></span>



## <a name="properties"></a><span data-ttu-id="3d4cf-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="3d4cf-107">Properties</span></span>
| <span data-ttu-id="3d4cf-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3d4cf-108">Property</span></span>     | <span data-ttu-id="3d4cf-109">Typ</span><span class="sxs-lookup"><span data-stu-id="3d4cf-109">Type</span></span>   |<span data-ttu-id="3d4cf-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3d4cf-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3d4cf-111">networkType</span><span class="sxs-lookup"><span data-stu-id="3d4cf-111">networkType</span></span>|<span data-ttu-id="3d4cf-112">String</span><span class="sxs-lookup"><span data-stu-id="3d4cf-112">String</span></span>|<span data-ttu-id="3d4cf-113">Stellt den Typ des Netzwerks.</span><span class="sxs-lookup"><span data-stu-id="3d4cf-113">Provides the type of the network.</span></span> <span data-ttu-id="3d4cf-114">Mögliche Werte sind `intranet`, `extranet`, `namedNetwork`, und `trusted`.</span><span class="sxs-lookup"><span data-stu-id="3d4cf-114">Possible values are `intranet`, `extranet`, `namedNetwork`, and `trusted`.</span></span>|
|<span data-ttu-id="3d4cf-115">Netzwerkname</span><span class="sxs-lookup"><span data-stu-id="3d4cf-115">networkName</span></span>|<span data-ttu-id="3d4cf-116">String</span><span class="sxs-lookup"><span data-stu-id="3d4cf-116">String</span></span>|<span data-ttu-id="3d4cf-117">Name des Netzwerks.</span><span class="sxs-lookup"><span data-stu-id="3d4cf-117">Name of the network.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="3d4cf-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="3d4cf-118">JSON representation</span></span>

<span data-ttu-id="3d4cf-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="3d4cf-119">Here is a JSON representation of the resource.</span></span>

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