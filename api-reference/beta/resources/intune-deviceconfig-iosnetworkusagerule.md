---
title: iosNetworkUsageRule-Ressourcentyp
description: In Netzwerknutzungsregeln können Unternehmen angeben, wie verwaltete Apps Netzwerke, beispielsweise Mobilfunknetze, verwenden.
localization_priority: Normal
ms.openlocfilehash: 6cf2f0cd88c25a625b12b3adcaac6ccc366ea0e2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860998"
---
# <a name="iosnetworkusagerule-resource-type"></a>iosNetworkUsageRule-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

In Netzwerknutzungsregeln können Unternehmen angeben, wie verwaltete Apps Netzwerke, beispielsweise Mobilfunknetze, verwenden.
## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|managedApps|[appListItem](../resources/intune-deviceconfig-applistitem.md)-Sammlung|Informationen zu den verwalteten Apps, auf die diese Regel angewendet werden wird. Diese Sammlung kann bis zu 500 Elemente enthalten.|
|cellularDataBlockWhenRoaming|Boolean|Wenn dies auf „true“ festgelegt wird, können die entsprechenden verwalteten Apps beim Roaming keine mobilen Daten verwenden.|
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





