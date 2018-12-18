---
title: deviceActionResult-Ressourcentyp
description: Ergebnis von Gerätevorgang
author: tfitzmac
ms.openlocfilehash: 48429e059616d9af0e3cbdac8544e68354b94fb5
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27320545"
---
# <a name="deviceactionresult-resource-type"></a>deviceActionResult-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Ergebnis von Gerätevorgang
## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|actionName|Zeichenfolge|Name der Aktion|
|actionState|[actionState](../resources/intune-devices-actionstate.md)|Status der Aktion. Mögliche Werte sind: `none`, `pending`, `canceled`, `active`, `done`, `failed` und `notSupported`.|
|startDateTime|DateTimeOffset|Zeitpunkt der Einleitung der Aktion|
|lastUpdatedDateTime|DateTimeOffset|Zeitpunkt der letzten Aktualisierung des Aktionszustands|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)"
}
```



