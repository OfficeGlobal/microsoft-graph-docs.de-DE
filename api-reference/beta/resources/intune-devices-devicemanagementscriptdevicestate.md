---
title: deviceManagementScriptDeviceState-Ressourcentyp
description: Enthält Eigenschaften für den Geräte Ausführungsstatus des Geräteverwaltungsskripts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 390c48a6c7d0cf040891cf77e4e89bae3aeca79e
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30169762"
---
# <a name="devicemanagementscriptdevicestate-resource-type"></a>deviceManagementScriptDeviceState-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Enthält Eigenschaften für den Geräte Ausführungsstatus des Geräteverwaltungsskripts.

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[DeviceManagementScriptDeviceStates aufListen](../api/intune-devices-devicemanagementscriptdevicestate-list.md)|[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) -Sammlung|AufListen von Eigenschaften und Beziehungen der [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) -Objekte.|
|[DeviceManagementScriptDeviceState abrufen](../api/intune-devices-devicemanagementscriptdevicestate-get.md)|[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)|Lesen von Eigenschaften und Beziehungen des [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) -Objekts.|
|[DeviceManagementScriptDeviceState erstellen](../api/intune-devices-devicemanagementscriptdevicestate-create.md)|[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)|Erstellen eines neuen [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) -Objekts.|
|[DeviceManagementScriptDeviceState löschen](../api/intune-devices-devicemanagementscriptdevicestate-delete.md)|Keine|Löscht eine [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md).|
|[DeviceManagementScriptDeviceState aktualisieren](../api/intune-devices-devicemanagementscriptdevicestate-update.md)|[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)|Aktualisieren der Eigenschaften eines [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Schlüssel der Gerätestatus Entität des Device Management-Skripts.|
|runState|[runState](../resources/intune-shared-runstate.md)|Status der letzten Ausführung des Geräteverwaltungs-Skripts. Mögliche Werte sind: `unknown`, `success` und `fail`.|
|resultMessage|Zeichenfolge|Details der Ausführungs Ausgabe.|
|lastStateUpdateDateTime|DateTimeOffset|Der letzte Zeitpunkt, zu dem das Geräte Verwaltungsskript ausgeführt wird.|
|errorCode|Int32|Fehlercode, der einer fehlerhaften Ausführung des Geräteverwaltungsskripts entspricht.|
|errorDescription|Zeichenfolge|Fehlerbeschreibung, die dem fehlerhaften Ausführen des Geräteverwaltungsskripts entspricht.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|managedDevice|[managedDevice](../resources/intune-devices-manageddevice.md)|Die verwalteten Geräte, die das Geräte Verwaltungsskript ausführen.|

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




