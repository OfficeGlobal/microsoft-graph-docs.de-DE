---
title: Ressourcentyp deviceManagementScriptDeviceState
description: Enthält Eigenschaften für Gerät Zustand des Skripts Management Gerät ausführen.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8274a6dd5b38ee419738d250af0267533de6f00a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422474"
---
# <a name="devicemanagementscriptdevicestate-resource-type"></a>Ressourcentyp deviceManagementScriptDeviceState

> **Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.

Enthält Eigenschaften für Gerät Zustand des Skripts Management Gerät ausführen.

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Liste deviceManagementScriptDeviceStates](../api/intune-devices-devicemanagementscriptdevicestate-list.md)|[DeviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) -Auflistung|Listeneigenschaften und Beziehungen der [DeviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) -Objekte.|
|[Abrufen von deviceManagementScriptDeviceState](../api/intune-devices-devicemanagementscriptdevicestate-get.md)|[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)|Lesen Sie Eigenschaften und Beziehungen des [DeviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) -Objekts.|
|[Erstellen von deviceManagementScriptDeviceState](../api/intune-devices-devicemanagementscriptdevicestate-create.md)|[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)|Erstellen eines neuen [DeviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) -Objekts.|
|[DeviceManagementScriptDeviceState löschen](../api/intune-devices-devicemanagementscriptdevicestate-delete.md)|Keine|Löscht eine [DeviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md).|
|[DeviceManagementScriptDeviceState aktualisieren](../api/intune-devices-devicemanagementscriptdevicestate-update.md)|[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)|Aktualisieren Sie die Eigenschaften eines [DeviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Taste der Gerät Management Skript Gerät Zustand Entität.|
|runState|[runState](../resources/intune-shared-runstate.md)|Status der letzten Ausführung des Skripts Management Gerät. Mögliche Werte sind: `unknown`, `success` und `fail`.|
|resultMessage|Zeichenfolge|Details der Ausgabe.|
|lastStateUpdateDateTime|DateTimeOffset|Zeitpunkt führt das Gerät Management-Skript aus.|
|errorCode|Int32|Fehlercode, fehlerhafte Ausführung des Skripts Management Gerät entspricht.|
|errorDescription|Zeichenfolge|Fehlerhafte Ausführung des Skripts Management Gerät entsprechend der Beschreibung des Fehlers.|

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




