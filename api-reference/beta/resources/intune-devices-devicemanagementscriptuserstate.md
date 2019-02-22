---
title: deviceManagementScriptUserState-Ressourcentyp
description: Enthält Eigenschaften für den Benutzer Ausführungsstatus des Geräteverwaltungsskripts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9f2a0d24c76d0eb01e7a7edc889dae47ae5bc0fa
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30144744"
---
# <a name="devicemanagementscriptuserstate-resource-type"></a>deviceManagementScriptUserState-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Enthält Eigenschaften für den Benutzer Ausführungsstatus des Geräteverwaltungsskripts.

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[DeviceManagementScriptUserStates aufListen](../api/intune-devices-devicemanagementscriptuserstate-list.md)|[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) -Sammlung|AufListen von Eigenschaften und Beziehungen der [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) -Objekte.|
|[DeviceManagementScriptUserState abrufen](../api/intune-devices-devicemanagementscriptuserstate-get.md)|[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)|Lesen von Eigenschaften und Beziehungen des [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) -Objekts.|
|[DeviceManagementScriptUserState erstellen](../api/intune-devices-devicemanagementscriptuserstate-create.md)|[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)|Erstellen eines neuen [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) -Objekts.|
|[DeviceManagementScriptUserState löschen](../api/intune-devices-devicemanagementscriptuserstate-delete.md)|Keine|Löscht eine [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md).|
|[DeviceManagementScriptUserState aktualisieren](../api/intune-devices-devicemanagementscriptuserstate-update.md)|[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)|Aktualisieren der Eigenschaften eines [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|string|Schlüssel der Benutzerstatus Entität des Device Management-Skripts.|
|successDeviceCount|Int32|Anzahl der erfolgreichen Geräte für einen bestimmten Benutzer.|
|errorDeviceCount|Int32|Fehlergeräte Anzahl für einen bestimmten Benutzer.|
|userPrincipalName|Zeichenfolge|Benutzerprinzipalname des jeweiligen Benutzers.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|deviceRunStates|[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) -Sammlung|Liste der Ausführungsstatus für dieses Skript auf allen Geräten eines bestimmten Benutzers.|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementScriptUserState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementScriptUserState",
  "id": "String (identifier)",
  "successDeviceCount": 1024,
  "errorDeviceCount": 1024,
  "userPrincipalName": "String"
}
```




