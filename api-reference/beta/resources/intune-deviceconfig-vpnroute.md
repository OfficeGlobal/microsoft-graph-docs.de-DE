---
title: vpnRoute-Ressourcentyp
description: Definition der VPN-Route.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 54706d47267eef8fff6c465f24e4e9caa183ccc3
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30154299"
---
# <a name="vpnroute-resource-type"></a>vpnRoute-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Definition der VPN-Route.

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|destinationPrefix|Zeichenfolge|Ziel Präfix (IPv4/V6-Adresse).|
|prefixSize|Int32|Präfix Größe. (1-32). Gültige Werte 1 bis 32|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vpnRoute"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vpnRoute",
  "destinationPrefix": "String",
  "prefixSize": 1024
}
```




