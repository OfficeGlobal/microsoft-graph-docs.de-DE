---
title: iosNetworkUsageRule-Ressourcentyp
description: In Netzwerknutzungsregeln können Unternehmen angeben, wie verwaltete Apps Netzwerke, beispielsweise Mobilfunknetze, verwenden.
ms.openlocfilehash: 93cfd1f5eefe6f32fd0b112b24e3cdfba6969434
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062315"
---
# <a name="iosnetworkusagerule-resource-type"></a><span data-ttu-id="7e5e1-103">iosNetworkUsageRule-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="7e5e1-103">iosNetworkUsageRule resource type</span></span>

> <span data-ttu-id="7e5e1-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="7e5e1-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7e5e1-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7e5e1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7e5e1-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="7e5e1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7e5e1-107">In Netzwerknutzungsregeln können Unternehmen angeben, wie verwaltete Apps Netzwerke, beispielsweise Mobilfunknetze, verwenden.</span><span class="sxs-lookup"><span data-stu-id="7e5e1-107">Network Usage Rules allow enterprises to specify how managed apps use networks, such as cellular data networks.</span></span>
## <a name="properties"></a><span data-ttu-id="7e5e1-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="7e5e1-108">Properties</span></span>
|<span data-ttu-id="7e5e1-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7e5e1-109">Property</span></span>|<span data-ttu-id="7e5e1-110">Typ</span><span class="sxs-lookup"><span data-stu-id="7e5e1-110">Type</span></span>|<span data-ttu-id="7e5e1-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7e5e1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7e5e1-112">managedApps</span><span class="sxs-lookup"><span data-stu-id="7e5e1-112">managedApps</span></span>|<span data-ttu-id="7e5e1-113">[appListItem](../resources/intune-deviceconfig-applistitem.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="7e5e1-113">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="7e5e1-114">Informationen zu den verwalteten Apps, auf die diese Regel angewendet werden wird.</span><span class="sxs-lookup"><span data-stu-id="7e5e1-114">Information about the managed apps that this rule is going to apply to.</span></span> <span data-ttu-id="7e5e1-115">Diese Sammlung kann bis zu 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="7e5e1-115">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="7e5e1-116">cellularDataBlockWhenRoaming</span><span class="sxs-lookup"><span data-stu-id="7e5e1-116">cellularDataBlockWhenRoaming</span></span>|<span data-ttu-id="7e5e1-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="7e5e1-117">Boolean</span></span>|<span data-ttu-id="7e5e1-118">Wenn dies auf „true“ festgelegt wird, können die entsprechenden verwalteten Apps beim Roaming keine mobilen Daten verwenden.</span><span class="sxs-lookup"><span data-stu-id="7e5e1-118">If set to true, corresponding managed apps will not be allowed to use cellular data when roaming.</span></span>|
|<span data-ttu-id="7e5e1-119">cellularDataBlocked</span><span class="sxs-lookup"><span data-stu-id="7e5e1-119">cellularDataBlocked</span></span>|<span data-ttu-id="7e5e1-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="7e5e1-120">Boolean</span></span>|<span data-ttu-id="7e5e1-121">Wenn dies auf „true“ festgelegt wird, können die entsprechenden verwalteten Apps zu keiner Zeit mobile Daten verwenden.</span><span class="sxs-lookup"><span data-stu-id="7e5e1-121">If set to true, corresponding managed apps will not be allowed to use cellular data at any time.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7e5e1-122">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="7e5e1-122">Relationships</span></span>
<span data-ttu-id="7e5e1-123">Keine</span><span class="sxs-lookup"><span data-stu-id="7e5e1-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="7e5e1-124">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="7e5e1-124">JSON Representation</span></span>
<span data-ttu-id="7e5e1-125">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="7e5e1-125">Here is a JSON representation of the resource.</span></span>
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





