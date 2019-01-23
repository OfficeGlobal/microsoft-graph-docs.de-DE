---
title: Ressourcentyp deviceManagementScript
description: Intune bietet Kunden die Möglichkeit, ihre Powershell-Skripts auf der registrierten Windows 10 Azure Active Directory verbunden Geräten ausführen. Das Skript kann einmal oder in regelmäßigen Abständen ausgeführt werden.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 4fda826ec8033cd51ad4dd13dbc5b523a21e9e3a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29412527"
---
# <a name="devicemanagementscript-resource-type"></a>Ressourcentyp deviceManagementScript

> **Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.

Intune bietet Kunden die Möglichkeit, ihre Powershell-Skripts auf der registrierten Windows 10 Azure Active Directory verbunden Geräten ausführen. Das Skript kann einmal oder in regelmäßigen Abständen ausgeführt werden.

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Liste deviceManagementScripts](../api/intune-devices-devicemanagementscript-list.md)|[DeviceManagementScript](../resources/intune-devices-devicemanagementscript.md) -Auflistung|Listeneigenschaften und Beziehungen der [DeviceManagementScript](../resources/intune-devices-devicemanagementscript.md) -Objekte.|
|[Abrufen von deviceManagementScript](../api/intune-devices-devicemanagementscript-get.md)|[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)|Lesen Sie Eigenschaften und Beziehungen des [DeviceManagementScript](../resources/intune-devices-devicemanagementscript.md) -Objekts.|
|[Erstellen von deviceManagementScript](../api/intune-devices-devicemanagementscript-create.md)|[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)|Erstellen eines neuen [DeviceManagementScript](../resources/intune-devices-devicemanagementscript.md) -Objekts.|
|[DeviceManagementScript löschen](../api/intune-devices-devicemanagementscript-delete.md)|Keine|Löscht eine [DeviceManagementScript](../resources/intune-devices-devicemanagementscript.md).|
|[DeviceManagementScript aktualisieren](../api/intune-devices-devicemanagementscript-update.md)|[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)|Aktualisieren Sie die Eigenschaften eines [DeviceManagementScript](../resources/intune-devices-devicemanagementscript.md) -Objekts.|
|[assign-Aktion](../api/intune-devices-devicemanagementscript-assign.md)|Keine|Noch nicht dokumentiert|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Eindeutiger Bezeichner für das Gerät Management-Skript.|
|displayName|Zeichenfolge|Name des Skripts Management Gerät.|
|description|Zeichenfolge|Optionale Beschreibung für das Gerät Management-Skript.|
|runSchedule|[runSchedule](../resources/intune-devices-runschedule.md)|Das Intervall für das Skript ausgeführt wird. Wenn nicht definiert das Skript einmal ausgeführt wird|
|scriptContent|Binär|Der Skriptinhalt.|
|createdDateTime|DateTimeOffset|Datum und Zeit für das Gerät Management-Skript erstellt wurde.|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung des Geräts Management-Skripts.|
|runAsAccount|[runAsAccountType](../resources/intune-shared-runasaccounttype.md)|Gibt den Typ des Ausführungskontexts, den das Gerät Management-Skript in ausgeführt wird. Mögliche Werte sind: `system` und `user`.|
|enforceSignatureCheck|Boolean|Geben Sie an, ob die Signatur Skript muss aktiviert sein.|
|fileName|Zeichenfolge|Dateiname des Skripts.|
|roleScopeTagIds|Zeichenfolgenauflistung|Liste der Bereichs-Tag-IDs für diese Instanz des PowerShellScript.|
|runAs32Bit|Boolean|Ein Wert, der angibt, ob das PowerShell-Skript als 32-Bit ausgeführt werden soll|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|groupAssignments|[DeviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) -Auflistung|Die Liste der Gruppe Zuordnungen für das Gerät Management-Skript.|
|assignments|[DeviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) -Auflistung|Die Liste der Gruppe Zuordnungen für das Gerät Management-Skript.|
|runSummary|[deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md)|Zusammenfassung für Device-Management-Skript ausführen.|
|deviceRunStates|[DeviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) -Auflistung|Liste der für dieses Skript auf allen Geräten ausführen Zustände.|
|userRunStates|[DeviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) -Auflistung|Liste der Laufzeit Zustände für dieses Skript für alle Benutzer.|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementScript"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementScript",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "runSchedule": {
    "@odata.type": "microsoft.graph.runSchedule"
  },
  "scriptContent": "binary",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "runAsAccount": "String",
  "enforceSignatureCheck": true,
  "fileName": "String",
  "roleScopeTagIds": [
    "String"
  ],
  "runAs32Bit": true
}
```




