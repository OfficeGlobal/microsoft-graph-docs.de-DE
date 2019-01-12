---
title: iosNetworkUsageRule-Ressourcentyp
description: In Netzwerknutzungsregeln können Unternehmen angeben, wie verwaltete Apps Netzwerke, beispielsweise Mobilfunknetze, verwenden.
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: 057ddb8027835702cdb487387efafb73cb986c2e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27964844"
---
# <a name="iosnetworkusagerule-resource-type"></a><span data-ttu-id="9ac38-103">iosNetworkUsageRule-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="9ac38-103">iosNetworkUsageRule resource type</span></span>

> <span data-ttu-id="9ac38-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="9ac38-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9ac38-105">In Netzwerknutzungsregeln können Unternehmen angeben, wie verwaltete Apps Netzwerke, beispielsweise Mobilfunknetze, verwenden.</span><span class="sxs-lookup"><span data-stu-id="9ac38-105">Network Usage Rules allow enterprises to specify how managed apps use networks, such as cellular data networks.</span></span>
## <a name="properties"></a><span data-ttu-id="9ac38-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="9ac38-106">Properties</span></span>
|<span data-ttu-id="9ac38-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9ac38-107">Property</span></span>|<span data-ttu-id="9ac38-108">Typ</span><span class="sxs-lookup"><span data-stu-id="9ac38-108">Type</span></span>|<span data-ttu-id="9ac38-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9ac38-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ac38-110">managedApps</span><span class="sxs-lookup"><span data-stu-id="9ac38-110">managedApps</span></span>|<span data-ttu-id="9ac38-111">[appListItem](../resources/intune-deviceconfig-applistitem.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="9ac38-111">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="9ac38-112">Informationen zu den verwalteten Apps, auf die diese Regel angewendet werden wird.</span><span class="sxs-lookup"><span data-stu-id="9ac38-112">Information about the managed apps that this rule is going to apply to.</span></span> <span data-ttu-id="9ac38-113">Diese Sammlung kann bis zu 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="9ac38-113">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="9ac38-114">cellularDataBlockWhenRoaming</span><span class="sxs-lookup"><span data-stu-id="9ac38-114">cellularDataBlockWhenRoaming</span></span>|<span data-ttu-id="9ac38-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ac38-115">Boolean</span></span>|<span data-ttu-id="9ac38-116">Wenn dies auf „true“ festgelegt wird, können die entsprechenden verwalteten Apps beim Roaming keine mobilen Daten verwenden.</span><span class="sxs-lookup"><span data-stu-id="9ac38-116">If set to true, corresponding managed apps will not be allowed to use cellular data when roaming.</span></span>|
|<span data-ttu-id="9ac38-117">cellularDataBlocked</span><span class="sxs-lookup"><span data-stu-id="9ac38-117">cellularDataBlocked</span></span>|<span data-ttu-id="9ac38-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ac38-118">Boolean</span></span>|<span data-ttu-id="9ac38-119">Wenn dies auf „true“ festgelegt wird, können die entsprechenden verwalteten Apps zu keiner Zeit mobile Daten verwenden.</span><span class="sxs-lookup"><span data-stu-id="9ac38-119">If set to true, corresponding managed apps will not be allowed to use cellular data at any time.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9ac38-120">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="9ac38-120">Relationships</span></span>
<span data-ttu-id="9ac38-121">Keine</span><span class="sxs-lookup"><span data-stu-id="9ac38-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="9ac38-122">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="9ac38-122">JSON Representation</span></span>
<span data-ttu-id="9ac38-123">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="9ac38-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosNetworkUsageRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosNetworkUsageRule",
  "managedApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "String",
      "publisher": "String",
      "appStoreUrl": "String",
      "appId": "String"
    }
  ],
  "cellularDataBlockWhenRoaming": true,
  "cellularDataBlocked": true
}
```



