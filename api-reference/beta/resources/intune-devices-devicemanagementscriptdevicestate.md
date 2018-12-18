---
title: Ressourcentyp deviceManagementScriptDeviceState
description: Enthält Eigenschaften für Gerät Zustand des Skripts Management Gerät ausführen.
author: tfitzmac
ms.openlocfilehash: 5667de5351ea3130ab0c3e00a55013ada66ed01a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27337324"
---
# <a name="devicemanagementscriptdevicestate-resource-type"></a>Ressourcentyp deviceManagementScriptDeviceState

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Enthält Eigenschaften für Gerät Zustand des Skripts Management Gerät ausführen.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Liste deviceManagementScriptDeviceStates](../api/intune-devices-devicemanagementscriptdevicestate-list.md)|[DeviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) -Auflistung|Listeneigenschaften und Beziehungen der [DeviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) -Objekte.|
|[Abrufen von deviceManagementScriptDeviceState](../api/intune-devices-devicemanagementscriptdevicestate-get.md)|[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)|Lesen Sie Eigenschaften und Beziehungen des [DeviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) -Objekts.|
|[Erstellen von deviceManagementScriptDeviceState](../api/intune-devices-devicemanagementscriptdevicestate-create.md)|[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)|Erstellen eines neuen [DeviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) -Objekts.|
|[DeviceManagementScriptDeviceState löschen](../api/intune-devices-devicemanagementscriptdevicestate-delete.md)|Keines|Löscht eine [DeviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md).|
|[DeviceManagementScriptDeviceState aktualisieren](../api/intune-devices-devicemanagementscriptdevicestate-update.md)|[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)|Aktualisieren Sie die Eigenschaften eines [DeviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Taste der Gerät Management Skript Gerät Zustand Entität.|
|runState|[runState](../resources/intune-shared-runstate.md)|Status der letzten Ausführung des Skripts Management Gerät. Mögliche Werte sind: `unknown`, `success` und `fail`.|
|resultMessage|String|Details der Ausgabe.|
|lastStateUpdateDateTime|DateTimeOffset|Zeitpunkt führt das Gerät Management-Skript aus.|
|errorCode|Int32|Fehlercode, fehlerhafte Ausführung des Skripts Management Gerät entspricht.|
|errorDescription|String|Fehlerhafte Ausführung des Skripts Management Gerät entsprechend der Beschreibung des Fehlers.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|managedDevice|[managedDevice](../resources/intune-devices-manageddevice.md)|Die verwaltete Geräte, die das Gerät Management Skript ausgeführt wird.|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementScriptDeviceState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementScriptDeviceState",
  "id": "String (identifier)",
  "runState": "String",
  "resultMessage": "String",
  "lastStateUpdateDateTime": "String (timestamp)",
  "errorCode": 1024,
  "errorDescription": "String"
}
```





