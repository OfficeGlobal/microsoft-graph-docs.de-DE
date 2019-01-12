---
title: remoteLockActionResult-Ressourcentyp
description: Ergebnis einer Sperraktion mit einem Pin zum Entsperren
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 341d1425de71c7175346e1ba6b30fe2a81b696a4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27922718"
---
# <a name="remotelockactionresult-resource-type"></a>remoteLockActionResult-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Ergebnis einer Sperraktion mit einem Pin zum Entsperren

Erbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|actionName|Zeichenfolge|Aktionsname, geerbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)|
|actionState|[actionState](../resources/intune-devices-actionstate.md)|Status der Aktion Inherited aus [DeviceActionResult](../resources/intune-devices-deviceactionresult.md). Mögliche Werte sind: `none`, `pending`, `canceled`, `active`, `done`, `failed` und `notSupported`.|
|startDateTime|DateTimeOffset|Zeit, zu der die Aktion initiiert wurde. Geerbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)|
|lastUpdatedDateTime|DateTimeOffset|Zeit, zu der der Aktionszustand zuletzt aktualisiert wurde. Geerbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)|
|unlockPin|String|Pin zum Entsperren des Clients|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.remoteLockActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.remoteLockActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "unlockPin": "String"
}
```



