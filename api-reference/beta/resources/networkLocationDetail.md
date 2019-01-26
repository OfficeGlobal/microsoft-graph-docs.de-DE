---
title: Ressourcentyp networkLocationDetail
description: Gibt den Speicherort im Netzwerk zugeordneten Details an. .
localization_priority: Normal
ms.openlocfilehash: 62bdb23c63beb89b85386e6bea67face097cf1ae
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29570939"
---
# <a name="networklocationdetail-resource-type"></a><span data-ttu-id="65eb2-104">Ressourcentyp networkLocationDetail</span><span class="sxs-lookup"><span data-stu-id="65eb2-104">networkLocationDetail resource type</span></span>
<span data-ttu-id="65eb2-105">Gibt den Speicherort im Netzwerk zugeordneten Details an.</span><span class="sxs-lookup"><span data-stu-id="65eb2-105">Indicates details associated with the network location.</span></span> <span data-ttu-id="65eb2-106">.</span><span class="sxs-lookup"><span data-stu-id="65eb2-106"></span></span>



## <a name="properties"></a><span data-ttu-id="65eb2-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="65eb2-107">Properties</span></span>
| <span data-ttu-id="65eb2-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="65eb2-108">Property</span></span>     | <span data-ttu-id="65eb2-109">Typ</span><span class="sxs-lookup"><span data-stu-id="65eb2-109">Type</span></span>   |<span data-ttu-id="65eb2-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="65eb2-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="65eb2-111">networkType</span><span class="sxs-lookup"><span data-stu-id="65eb2-111">networkType</span></span>| <span data-ttu-id="65eb2-112">Enum-Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="65eb2-112">enum-string</span></span> |<span data-ttu-id="65eb2-113">Stellt den Typ des Netzwerks.</span><span class="sxs-lookup"><span data-stu-id="65eb2-113">Provides the type of the network.</span></span> <span data-ttu-id="65eb2-114">Mögliche Werte sind `intranet`, `extranet`, `namedNetwork`, und `trusted`.</span><span class="sxs-lookup"><span data-stu-id="65eb2-114">Possible values are `intranet`, `extranet`, `namedNetwork`, and `trusted`.</span></span>|
|<span data-ttu-id="65eb2-115">Netzwerkname</span><span class="sxs-lookup"><span data-stu-id="65eb2-115">networkName</span></span>|<span data-ttu-id="65eb2-116">String</span><span class="sxs-lookup"><span data-stu-id="65eb2-116">String</span></span>|<span data-ttu-id="65eb2-117">Name des Netzwerks.</span><span class="sxs-lookup"><span data-stu-id="65eb2-117">Name of the network.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="65eb2-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="65eb2-118">JSON representation</span></span>

<span data-ttu-id="65eb2-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="65eb2-119">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.deviceDetail"
}-->

```json
{
  "networkTypes": " intranet | extranet | namedNetwork | trusted ",
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
