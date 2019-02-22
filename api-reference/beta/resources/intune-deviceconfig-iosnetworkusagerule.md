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
# <a name="iosnetworkusagerule-resource-type"></a>iosNetworkUsageRule-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

In Netzwerknutzungsregeln können Unternehmen angeben, wie verwaltete Apps Netzwerke, beispielsweise Mobilfunknetze, verwenden.

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|managedApps|[appListItem](../resources/intune-deviceconfig-applistitem.md)-Sammlung|Informationen zu den verwalteten Apps, auf die diese Regel angewendet werden wird. Diese Sammlung kann bis zu 500 Elemente enthalten.|
|cellularDataBlockWhenRoaming|Boolescher Wert|Wenn dies auf „true“ festgelegt wird, können die entsprechenden verwalteten Apps beim Roaming keine mobilen Daten verwenden.|
|cellularDataBlocked|Boolean|Wenn dies auf „true“ festgelegt wird, können die entsprechenden verwalteten Apps zu keiner Zeit mobile Daten verwenden.|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
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




