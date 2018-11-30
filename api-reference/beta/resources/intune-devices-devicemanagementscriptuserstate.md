---
title: Ressourcentyp deviceManagementScriptUserState
description: Enthält Eigenschaften für Benutzer Zustand des Skripts Management Gerät ausführen.
ms.openlocfilehash: 4e444c1eee438acba558a85e2a4ada14e44849bc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065926"
---
# <a name="devicemanagementscriptuserstate-resource-type"></a>Ressourcentyp deviceManagementScriptUserState

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Enthält Eigenschaften für Benutzer Zustand des Skripts Management Gerät ausführen.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Liste deviceManagementScriptUserStates](../api/intune-devices-devicemanagementscriptuserstate-list.md)|[DeviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) -Auflistung|Listeneigenschaften und Beziehungen der [DeviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) -Objekte.|
|[Abrufen von deviceManagementScriptUserState](../api/intune-devices-devicemanagementscriptuserstate-get.md)|[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)|Lesen Sie Eigenschaften und Beziehungen des [DeviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) -Objekts.|
|[Erstellen von deviceManagementScriptUserState](../api/intune-devices-devicemanagementscriptuserstate-create.md)|[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)|Erstellen eines neuen [DeviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) -Objekts.|
|[DeviceManagementScriptUserState löschen](../api/intune-devices-devicemanagementscriptuserstate-delete.md)|Keines|Löscht eine [DeviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md).|
|[DeviceManagementScriptUserState aktualisieren](../api/intune-devices-devicemanagementscriptuserstate-update.md)|[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)|Aktualisieren Sie die Eigenschaften eines [DeviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Das Gerät Management Skript Zustand Benutzerentität-Taste.|
|successDeviceCount|Int32|Anzahl der Erfolg Geräte für bestimmte Benutzer.|
|errorDeviceCount|Int32|Anzahl der Fehler Geräte für bestimmte Benutzer.|
|userPrincipalName|String|Prinzip-Benutzernamen eines bestimmten Benutzers.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|deviceRunStates|[DeviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) -Auflistung|Liste der Laufzeit Zustände für dieses Skript auf allen Geräten eines bestimmten Benutzers.|

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





