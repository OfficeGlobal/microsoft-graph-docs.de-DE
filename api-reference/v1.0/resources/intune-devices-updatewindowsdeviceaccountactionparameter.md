---
title: updateWindowsDeviceAccountActionParameter-Ressourcentyp
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d67599dfc9db2afa337324e3f1ba9334134458f4
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30256672"
---
# <a name="updatewindowsdeviceaccountactionparameter-resource-type"></a>updateWindowsDeviceAccountActionParameter-Ressourcentyp

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Noch nicht dokumentiert

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|deviceAccount|[windowsDeviceAccount](../resources/intune-devices-windowsdeviceaccount.md)|Noch nicht dokumentiert|
|passwordRotationEnabled|Boolean|Noch nicht dokumentiert|
|calendarSyncEnabled|Boolescher Wert|Noch nicht dokumentiert|
|deviceAccountEmail|Zeichenfolge|Noch nicht dokumentiert|
|exchangeServer|Zeichenfolge|Noch nicht dokumentiert.|
|sessionInitiationProtocalAddress|Zeichenfolge|Noch nicht dokumentiert|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.updateWindowsDeviceAccountActionParameter"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.updateWindowsDeviceAccountActionParameter",
  "deviceAccount": {
    "@odata.type": "microsoft.graph.windowsDeviceAccount",
    "password": "String"
  },
  "passwordRotationEnabled": true,
  "calendarSyncEnabled": true,
  "deviceAccountEmail": "String",
  "exchangeServer": "String",
  "sessionInitiationProtocalAddress": "String"
}
```



