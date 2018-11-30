---
title: iPv6Range-Ressourcentyp
description: IPV6-Bereich
ms.openlocfilehash: c2f17529b589fc2d7837f6a8f539ff64d5d82dd9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27020035"
---
# <a name="ipv6range-resource-type"></a><span data-ttu-id="0bb3c-103">iPv6Range-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="0bb3c-103">iPv6Range resource type</span></span>

> <span data-ttu-id="0bb3c-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="0bb3c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0bb3c-105">IPV6-Bereich</span><span class="sxs-lookup"><span data-stu-id="0bb3c-105">IP V6 range</span></span>

<span data-ttu-id="0bb3c-106">Erbt von [ipRange](../resources/intune-mam-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="0bb3c-106">Inherits from [ipRange](../resources/intune-mam-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0bb3c-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="0bb3c-107">Properties</span></span>
|<span data-ttu-id="0bb3c-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0bb3c-108">Property</span></span>|<span data-ttu-id="0bb3c-109">Typ</span><span class="sxs-lookup"><span data-stu-id="0bb3c-109">Type</span></span>|<span data-ttu-id="0bb3c-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0bb3c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0bb3c-111">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="0bb3c-111">lowerAddress</span></span>|<span data-ttu-id="0bb3c-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0bb3c-112">String</span></span>|<span data-ttu-id="0bb3c-113">Untere IP-Adresse</span><span class="sxs-lookup"><span data-stu-id="0bb3c-113">Lower IP Address</span></span>|
|<span data-ttu-id="0bb3c-114">upperAddress</span><span class="sxs-lookup"><span data-stu-id="0bb3c-114">upperAddress</span></span>|<span data-ttu-id="0bb3c-115">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0bb3c-115">String</span></span>|<span data-ttu-id="0bb3c-116">Obere IP-Adresse</span><span class="sxs-lookup"><span data-stu-id="0bb3c-116">Upper IP Address</span></span>|

## <a name="relationships"></a><span data-ttu-id="0bb3c-117">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="0bb3c-117">Relationships</span></span>
<span data-ttu-id="0bb3c-118">Keine</span><span class="sxs-lookup"><span data-stu-id="0bb3c-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0bb3c-119">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="0bb3c-119">JSON Representation</span></span>
<span data-ttu-id="0bb3c-120">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="0bb3c-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iPv6Range"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iPv6Range",
  "lowerAddress": "String",
  "upperAddress": "String"
}
```



