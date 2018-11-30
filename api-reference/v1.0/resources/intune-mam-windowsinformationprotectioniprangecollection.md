---
title: windowsInformationProtectionIPRangeCollection-Ressourcentyp
description: Windows Information Protection – IP-Bereichssammlung
ms.openlocfilehash: 41558014ec3d48af06788e15fc40786fe7f9aea4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017104"
---
# <a name="windowsinformationprotectioniprangecollection-resource-type"></a><span data-ttu-id="d4677-103">windowsInformationProtectionIPRangeCollection-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="d4677-103">windowsInformationProtectionIPRangeCollection resource type</span></span>

> <span data-ttu-id="d4677-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="d4677-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d4677-105">Windows Information Protection – IP-Bereichssammlung</span><span class="sxs-lookup"><span data-stu-id="d4677-105">Windows Information Protection IP Range Collection</span></span>
## <a name="properties"></a><span data-ttu-id="d4677-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d4677-106">Properties</span></span>
|<span data-ttu-id="d4677-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d4677-107">Property</span></span>|<span data-ttu-id="d4677-108">Typ</span><span class="sxs-lookup"><span data-stu-id="d4677-108">Type</span></span>|<span data-ttu-id="d4677-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d4677-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d4677-110">displayName</span><span class="sxs-lookup"><span data-stu-id="d4677-110">displayName</span></span>|<span data-ttu-id="d4677-111">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d4677-111">String</span></span>|<span data-ttu-id="d4677-112">Anzeigename</span><span class="sxs-lookup"><span data-stu-id="d4677-112">Display name</span></span>|
|<span data-ttu-id="d4677-113">ranges</span><span class="sxs-lookup"><span data-stu-id="d4677-113">ranges</span></span>|<span data-ttu-id="d4677-114">[ipRange](../resources/intune-mam-iprange.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="d4677-114">[ipRange](../resources/intune-mam-iprange.md) collection</span></span>|<span data-ttu-id="d4677-115">Sammlung der IP-Bereiche</span><span class="sxs-lookup"><span data-stu-id="d4677-115">Collection of ip ranges</span></span>|

## <a name="relationships"></a><span data-ttu-id="d4677-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="d4677-116">Relationships</span></span>
<span data-ttu-id="d4677-117">Keine</span><span class="sxs-lookup"><span data-stu-id="d4677-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d4677-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d4677-118">JSON Representation</span></span>
<span data-ttu-id="d4677-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d4677-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionIPRangeCollection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionIPRangeCollection",
  "displayName": "String",
  "ranges": [
    {
      "@odata.type": "microsoft.graph.ipRange",
      "lowerAddress": "String",
      "upperAddress": "String"
    }
  ]
}
```



