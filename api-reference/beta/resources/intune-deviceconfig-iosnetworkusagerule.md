---
title: iosNetworkUsageRule-Ressourcentyp
description: In Netzwerknutzungsregeln können Unternehmen angeben, wie verwaltete Apps Netzwerke, beispielsweise Mobilfunknetze, verwenden.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 0a287fcf8be771037a39efd821f5468acf518371
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398324"
---
# <a name="iosnetworkusagerule-resource-type"></a><span data-ttu-id="8f14d-103">iosNetworkUsageRule-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="8f14d-103">iosNetworkUsageRule resource type</span></span>

> <span data-ttu-id="8f14d-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="8f14d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="8f14d-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8f14d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8f14d-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8f14d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8f14d-107">In Netzwerknutzungsregeln können Unternehmen angeben, wie verwaltete Apps Netzwerke, beispielsweise Mobilfunknetze, verwenden.</span><span class="sxs-lookup"><span data-stu-id="8f14d-107">Network Usage Rules allow enterprises to specify how managed apps use networks, such as cellular data networks.</span></span>

## <a name="properties"></a><span data-ttu-id="8f14d-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="8f14d-108">Properties</span></span>
|<span data-ttu-id="8f14d-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8f14d-109">Property</span></span>|<span data-ttu-id="8f14d-110">Typ</span><span class="sxs-lookup"><span data-stu-id="8f14d-110">Type</span></span>|<span data-ttu-id="8f14d-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8f14d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8f14d-112">managedApps</span><span class="sxs-lookup"><span data-stu-id="8f14d-112">managedApps</span></span>|<span data-ttu-id="8f14d-113">[appListItem](../resources/intune-deviceconfig-applistitem.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="8f14d-113">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="8f14d-114">Informationen zu den verwalteten Apps, auf die diese Regel angewendet werden wird.</span><span class="sxs-lookup"><span data-stu-id="8f14d-114">Information about the managed apps that this rule is going to apply to.</span></span> <span data-ttu-id="8f14d-115">Diese Sammlung kann bis zu 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="8f14d-115">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="8f14d-116">cellularDataBlockWhenRoaming</span><span class="sxs-lookup"><span data-stu-id="8f14d-116">cellularDataBlockWhenRoaming</span></span>|<span data-ttu-id="8f14d-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f14d-117">Boolean</span></span>|<span data-ttu-id="8f14d-118">Wenn dies auf „true“ festgelegt wird, können die entsprechenden verwalteten Apps beim Roaming keine mobilen Daten verwenden.</span><span class="sxs-lookup"><span data-stu-id="8f14d-118">If set to true, corresponding managed apps will not be allowed to use cellular data when roaming.</span></span>|
|<span data-ttu-id="8f14d-119">cellularDataBlocked</span><span class="sxs-lookup"><span data-stu-id="8f14d-119">cellularDataBlocked</span></span>|<span data-ttu-id="8f14d-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f14d-120">Boolean</span></span>|<span data-ttu-id="8f14d-121">Wenn dies auf „true“ festgelegt wird, können die entsprechenden verwalteten Apps zu keiner Zeit mobile Daten verwenden.</span><span class="sxs-lookup"><span data-stu-id="8f14d-121">If set to true, corresponding managed apps will not be allowed to use cellular data at any time.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8f14d-122">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="8f14d-122">Relationships</span></span>
<span data-ttu-id="8f14d-123">Keine</span><span class="sxs-lookup"><span data-stu-id="8f14d-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8f14d-124">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="8f14d-124">JSON Representation</span></span>
<span data-ttu-id="8f14d-125">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="8f14d-125">Here is a JSON representation of the resource.</span></span>
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




