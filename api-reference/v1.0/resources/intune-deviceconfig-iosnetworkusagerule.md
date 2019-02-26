---
title: iosNetworkUsageRule-Ressourcentyp
description: In Netzwerknutzungsregeln können Unternehmen angeben, wie verwaltete Apps Netzwerke, beispielsweise Mobilfunknetze, verwenden.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 516e880e4b6230ca165426b849f57609dcc6e6ad
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30250103"
---
# <a name="iosnetworkusagerule-resource-type"></a><span data-ttu-id="3539a-103">iosNetworkUsageRule-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="3539a-103">iosNetworkUsageRule resource type</span></span>

> <span data-ttu-id="3539a-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="3539a-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3539a-105">In Netzwerknutzungsregeln können Unternehmen angeben, wie verwaltete Apps Netzwerke, beispielsweise Mobilfunknetze, verwenden.</span><span class="sxs-lookup"><span data-stu-id="3539a-105">Network Usage Rules allow enterprises to specify how managed apps use networks, such as cellular data networks.</span></span>

## <a name="properties"></a><span data-ttu-id="3539a-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="3539a-106">Properties</span></span>
|<span data-ttu-id="3539a-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3539a-107">Property</span></span>|<span data-ttu-id="3539a-108">Typ</span><span class="sxs-lookup"><span data-stu-id="3539a-108">Type</span></span>|<span data-ttu-id="3539a-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3539a-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3539a-110">managedApps</span><span class="sxs-lookup"><span data-stu-id="3539a-110">managedApps</span></span>|<span data-ttu-id="3539a-111">[appListItem](../resources/intune-deviceconfig-applistitem.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="3539a-111">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="3539a-112">Informationen zu den verwalteten Apps, auf die diese Regel angewendet werden wird.</span><span class="sxs-lookup"><span data-stu-id="3539a-112">Information about the managed apps that this rule is going to apply to.</span></span> <span data-ttu-id="3539a-113">Diese Sammlung kann bis zu 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="3539a-113">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="3539a-114">cellularDataBlockWhenRoaming</span><span class="sxs-lookup"><span data-stu-id="3539a-114">cellularDataBlockWhenRoaming</span></span>|<span data-ttu-id="3539a-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="3539a-115">Boolean</span></span>|<span data-ttu-id="3539a-116">Wenn dies auf „true“ festgelegt wird, können die entsprechenden verwalteten Apps beim Roaming keine mobilen Daten verwenden.</span><span class="sxs-lookup"><span data-stu-id="3539a-116">If set to true, corresponding managed apps will not be allowed to use cellular data when roaming.</span></span>|
|<span data-ttu-id="3539a-117">cellularDataBlocked</span><span class="sxs-lookup"><span data-stu-id="3539a-117">cellularDataBlocked</span></span>|<span data-ttu-id="3539a-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="3539a-118">Boolean</span></span>|<span data-ttu-id="3539a-119">Wenn dies auf „true“ festgelegt wird, können die entsprechenden verwalteten Apps zu keiner Zeit mobile Daten verwenden.</span><span class="sxs-lookup"><span data-stu-id="3539a-119">If set to true, corresponding managed apps will not be allowed to use cellular data at any time.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3539a-120">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="3539a-120">Relationships</span></span>
<span data-ttu-id="3539a-121">Keine</span><span class="sxs-lookup"><span data-stu-id="3539a-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3539a-122">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="3539a-122">JSON Representation</span></span>
<span data-ttu-id="3539a-123">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="3539a-123">Here is a JSON representation of the resource.</span></span>
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



