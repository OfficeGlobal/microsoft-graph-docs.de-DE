---
title: iosNetworkUsageRule-Ressourcentyp
description: In Netzwerknutzungsregeln können Unternehmen angeben, wie verwaltete Apps Netzwerke, beispielsweise Mobilfunknetze, verwenden.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 03cc8c1586bb851d54d9ba87f947b6b6d7b254b5
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30168327"
---
# <a name="iosnetworkusagerule-resource-type"></a><span data-ttu-id="85cd9-103">iosNetworkUsageRule-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="85cd9-103">iosNetworkUsageRule resource type</span></span>

> <span data-ttu-id="85cd9-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="85cd9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="85cd9-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="85cd9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="85cd9-106">In Netzwerknutzungsregeln können Unternehmen angeben, wie verwaltete Apps Netzwerke, beispielsweise Mobilfunknetze, verwenden.</span><span class="sxs-lookup"><span data-stu-id="85cd9-106">Network Usage Rules allow enterprises to specify how managed apps use networks, such as cellular data networks.</span></span>

## <a name="properties"></a><span data-ttu-id="85cd9-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="85cd9-107">Properties</span></span>
|<span data-ttu-id="85cd9-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="85cd9-108">Property</span></span>|<span data-ttu-id="85cd9-109">Typ</span><span class="sxs-lookup"><span data-stu-id="85cd9-109">Type</span></span>|<span data-ttu-id="85cd9-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="85cd9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="85cd9-111">managedApps</span><span class="sxs-lookup"><span data-stu-id="85cd9-111">managedApps</span></span>|<span data-ttu-id="85cd9-112">[appListItem](../resources/intune-deviceconfig-applistitem.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="85cd9-112">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="85cd9-113">Informationen zu den verwalteten Apps, auf die diese Regel angewendet werden wird.</span><span class="sxs-lookup"><span data-stu-id="85cd9-113">Information about the managed apps that this rule is going to apply to.</span></span> <span data-ttu-id="85cd9-114">Diese Sammlung kann bis zu 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="85cd9-114">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="85cd9-115">cellularDataBlockWhenRoaming</span><span class="sxs-lookup"><span data-stu-id="85cd9-115">cellularDataBlockWhenRoaming</span></span>|<span data-ttu-id="85cd9-116">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="85cd9-116">Boolean</span></span>|<span data-ttu-id="85cd9-117">Wenn dies auf „true“ festgelegt wird, können die entsprechenden verwalteten Apps beim Roaming keine mobilen Daten verwenden.</span><span class="sxs-lookup"><span data-stu-id="85cd9-117">If set to true, corresponding managed apps will not be allowed to use cellular data when roaming.</span></span>|
|<span data-ttu-id="85cd9-118">cellularDataBlocked</span><span class="sxs-lookup"><span data-stu-id="85cd9-118">cellularDataBlocked</span></span>|<span data-ttu-id="85cd9-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="85cd9-119">Boolean</span></span>|<span data-ttu-id="85cd9-120">Wenn dies auf „true“ festgelegt wird, können die entsprechenden verwalteten Apps zu keiner Zeit mobile Daten verwenden.</span><span class="sxs-lookup"><span data-stu-id="85cd9-120">If set to true, corresponding managed apps will not be allowed to use cellular data at any time.</span></span>|

## <a name="relationships"></a><span data-ttu-id="85cd9-121">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="85cd9-121">Relationships</span></span>
<span data-ttu-id="85cd9-122">Keine</span><span class="sxs-lookup"><span data-stu-id="85cd9-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="85cd9-123">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="85cd9-123">JSON Representation</span></span>
<span data-ttu-id="85cd9-124">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="85cd9-124">Here is a JSON representation of the resource.</span></span>
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




