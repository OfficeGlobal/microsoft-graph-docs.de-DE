---
title: iPv4Range-Ressourcentyp
description: IP-V4-Bereich
ms.openlocfilehash: 8b59101e1fcdb5ab88d9c24a0359f8abb1687818
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018850"
---
# <a name="ipv4range-resource-type"></a><span data-ttu-id="658c8-103">iPv4Range-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="658c8-103">iPv4Range resource type</span></span>

> <span data-ttu-id="658c8-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="658c8-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="658c8-105">IP-V4-Bereich</span><span class="sxs-lookup"><span data-stu-id="658c8-105">IP V4 range</span></span>

<span data-ttu-id="658c8-106">Erbt von [ipRange](../resources/intune-mam-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="658c8-106">Inherits from [ipRange](../resources/intune-mam-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="658c8-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="658c8-107">Properties</span></span>
|<span data-ttu-id="658c8-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="658c8-108">Property</span></span>|<span data-ttu-id="658c8-109">Typ</span><span class="sxs-lookup"><span data-stu-id="658c8-109">Type</span></span>|<span data-ttu-id="658c8-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="658c8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="658c8-111">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="658c8-111">lowerAddress</span></span>|<span data-ttu-id="658c8-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="658c8-112">String</span></span>|<span data-ttu-id="658c8-113">Untere IP-Adresse</span><span class="sxs-lookup"><span data-stu-id="658c8-113">Lower IP Address</span></span>|
|<span data-ttu-id="658c8-114">upperAddress</span><span class="sxs-lookup"><span data-stu-id="658c8-114">upperAddress</span></span>|<span data-ttu-id="658c8-115">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="658c8-115">String</span></span>|<span data-ttu-id="658c8-116">Obere IP-Adresse</span><span class="sxs-lookup"><span data-stu-id="658c8-116">Upper IP Address</span></span>|

## <a name="relationships"></a><span data-ttu-id="658c8-117">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="658c8-117">Relationships</span></span>
<span data-ttu-id="658c8-118">Keine</span><span class="sxs-lookup"><span data-stu-id="658c8-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="658c8-119">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="658c8-119">JSON Representation</span></span>
<span data-ttu-id="658c8-120">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="658c8-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iPv4Range"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iPv4Range",
  "lowerAddress": "String",
  "upperAddress": "String"
}
```



