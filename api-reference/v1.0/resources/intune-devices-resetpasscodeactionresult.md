---
title: resetPasscodeActionResult-Ressourcentyp
description: Kennung zurücksetzen – Aktionsergebnis
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2e23c3e7d39566df98ab57258a54ab6f637439d1
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30257001"
---
# <a name="resetpasscodeactionresult-resource-type"></a>resetPasscodeActionResult-Ressourcentyp

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Kennung zurücksetzen – Aktionsergebnis


Erbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|actionName|String|Aktionsname, geerbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)|
|actionState|[actionState](../resources/intune-devices-actionstate.md)|Status der von [DeviceActionResult](../resources/intune-devices-deviceactionresult.md)geerbten Aktion. Mögliche Werte sind: `none`, `pending`, `canceled`, `active`, `done`, `failed` und `notSupported`.|
|startDateTime|DateTimeOffset|Zeit, zu der die Aktion initiiert wurde. Geerbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)|
|lastUpdatedDateTime|DateTimeOffset|Zeit, zu der der Aktionszustand zuletzt aktualisiert wurde. Geerbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)|
|Zugangscode|Zeichenfolge|Neu erstellter Zugangscode für das Gerät |

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.resetPasscodeActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.resetPasscodeActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "passcode": "String"
}
```



