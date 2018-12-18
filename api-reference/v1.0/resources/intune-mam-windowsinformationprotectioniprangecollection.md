---
title: windowsInformationProtectionIPRangeCollection-Ressourcentyp
description: Windows Information Protection – IP-Bereichssammlung
author: tfitzmac
ms.openlocfilehash: 12030ab0b71448c644e4e664f9095dea3e48a26c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27319754"
---
# <a name="windowsinformationprotectioniprangecollection-resource-type"></a><span data-ttu-id="709de-103">windowsInformationProtectionIPRangeCollection-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="709de-103">windowsInformationProtectionIPRangeCollection resource type</span></span>

> <span data-ttu-id="709de-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="709de-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="709de-105">Windows Information Protection – IP-Bereichssammlung</span><span class="sxs-lookup"><span data-stu-id="709de-105">Windows Information Protection IP Range Collection</span></span>
## <a name="properties"></a><span data-ttu-id="709de-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="709de-106">Properties</span></span>
|<span data-ttu-id="709de-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="709de-107">Property</span></span>|<span data-ttu-id="709de-108">Typ</span><span class="sxs-lookup"><span data-stu-id="709de-108">Type</span></span>|<span data-ttu-id="709de-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="709de-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="709de-110">displayName</span><span class="sxs-lookup"><span data-stu-id="709de-110">displayName</span></span>|<span data-ttu-id="709de-111">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="709de-111">String</span></span>|<span data-ttu-id="709de-112">Anzeigename</span><span class="sxs-lookup"><span data-stu-id="709de-112">Display name</span></span>|
|<span data-ttu-id="709de-113">ranges</span><span class="sxs-lookup"><span data-stu-id="709de-113">ranges</span></span>|<span data-ttu-id="709de-114">[ipRange](../resources/intune-mam-iprange.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="709de-114">[ipRange](../resources/intune-mam-iprange.md) collection</span></span>|<span data-ttu-id="709de-115">Sammlung der IP-Bereiche</span><span class="sxs-lookup"><span data-stu-id="709de-115">Collection of ip ranges</span></span>|

## <a name="relationships"></a><span data-ttu-id="709de-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="709de-116">Relationships</span></span>
<span data-ttu-id="709de-117">Keine</span><span class="sxs-lookup"><span data-stu-id="709de-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="709de-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="709de-118">JSON Representation</span></span>
<span data-ttu-id="709de-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="709de-119">Here is a JSON representation of the resource.</span></span>
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



