---
title: iosNetworkUsageRule-Ressourcentyp
description: In Netzwerknutzungsregeln können Unternehmen angeben, wie verwaltete Apps Netzwerke, beispielsweise Mobilfunknetze, verwenden.
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: 7476f49c6049eb18e56fa57310aa75707f566bd0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912022"
---
# <a name="iosnetworkusagerule-resource-type"></a><span data-ttu-id="7d56c-103">iosNetworkUsageRule-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="7d56c-103">iosNetworkUsageRule resource type</span></span>

> <span data-ttu-id="7d56c-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="7d56c-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7d56c-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7d56c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7d56c-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="7d56c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7d56c-107">In Netzwerknutzungsregeln können Unternehmen angeben, wie verwaltete Apps Netzwerke, beispielsweise Mobilfunknetze, verwenden.</span><span class="sxs-lookup"><span data-stu-id="7d56c-107">Network Usage Rules allow enterprises to specify how managed apps use networks, such as cellular data networks.</span></span>
## <a name="properties"></a><span data-ttu-id="7d56c-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="7d56c-108">Properties</span></span>
|<span data-ttu-id="7d56c-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7d56c-109">Property</span></span>|<span data-ttu-id="7d56c-110">Typ</span><span class="sxs-lookup"><span data-stu-id="7d56c-110">Type</span></span>|<span data-ttu-id="7d56c-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7d56c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7d56c-112">managedApps</span><span class="sxs-lookup"><span data-stu-id="7d56c-112">managedApps</span></span>|<span data-ttu-id="7d56c-113">[appListItem](../resources/intune-deviceconfig-applistitem.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="7d56c-113">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="7d56c-114">Informationen zu den verwalteten Apps, auf die diese Regel angewendet werden wird.</span><span class="sxs-lookup"><span data-stu-id="7d56c-114">Information about the managed apps that this rule is going to apply to.</span></span> <span data-ttu-id="7d56c-115">Diese Sammlung kann bis zu 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="7d56c-115">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="7d56c-116">cellularDataBlockWhenRoaming</span><span class="sxs-lookup"><span data-stu-id="7d56c-116">cellularDataBlockWhenRoaming</span></span>|<span data-ttu-id="7d56c-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="7d56c-117">Boolean</span></span>|<span data-ttu-id="7d56c-118">Wenn dies auf „true“ festgelegt wird, können die entsprechenden verwalteten Apps beim Roaming keine mobilen Daten verwenden.</span><span class="sxs-lookup"><span data-stu-id="7d56c-118">If set to true, corresponding managed apps will not be allowed to use cellular data when roaming.</span></span>|
|<span data-ttu-id="7d56c-119">cellularDataBlocked</span><span class="sxs-lookup"><span data-stu-id="7d56c-119">cellularDataBlocked</span></span>|<span data-ttu-id="7d56c-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="7d56c-120">Boolean</span></span>|<span data-ttu-id="7d56c-121">Wenn dies auf „true“ festgelegt wird, können die entsprechenden verwalteten Apps zu keiner Zeit mobile Daten verwenden.</span><span class="sxs-lookup"><span data-stu-id="7d56c-121">If set to true, corresponding managed apps will not be allowed to use cellular data at any time.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7d56c-122">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="7d56c-122">Relationships</span></span>
<span data-ttu-id="7d56c-123">Keine</span><span class="sxs-lookup"><span data-stu-id="7d56c-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="7d56c-124">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="7d56c-124">JSON Representation</span></span>
<span data-ttu-id="7d56c-125">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="7d56c-125">Here is a JSON representation of the resource.</span></span>
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





