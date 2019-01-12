---
title: Ressourcentyp deviceManagementScriptUserState
description: Enthält Eigenschaften für Benutzer Zustand des Skripts Management Gerät ausführen.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: d74e8276603355af58ccff50401f742c56147d7f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27942248"
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
|[DeviceManagementScriptUserState löschen](../api/intune-devices-devicemanagementscriptuserstate-delete.md)|Keine|Löscht eine [DeviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md).|
|[DeviceManagementScriptUserState aktualisieren](../api/intune-devices-devicemanagementscriptuserstate-update.md)|[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)|Aktualisieren Sie die Eigenschaften eines [DeviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Das Gerät Management Skript Zustand Benutzerentität-Taste.|
|successDeviceCount|Int32|Anzahl der Erfolg Geräte für bestimmte Benutzer.|
|errorDeviceCount|Int32|Anzahl der Fehler Geräte für bestimmte Benutzer.|
|userPrincipalName|Zeichenfolge|Prinzip-Benutzernamen eines bestimmten Benutzers.|

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





