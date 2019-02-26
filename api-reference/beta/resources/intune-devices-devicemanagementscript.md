---
title: Devicemanagementscript hinzugefügt-Ressourcentyp
description: InTune bietet Kunden die Möglichkeit, ihre PowerShell-Skripts auf den angemeldeten Windows 10 Azure Active Directory-Geräten auszuführen. Das Skript kann einmal oder periodisch ausgeführt werden.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e3fffd6bec8866066824725f1477e6de0e71ebf9
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30164064"
---
# <a name="devicemanagementscript-resource-type"></a>Devicemanagementscript hinzugefügt-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

InTune bietet Kunden die Möglichkeit, ihre PowerShell-Skripts auf den angemeldeten Windows 10 Azure Active Directory-Geräten auszuführen. Das Skript kann einmal oder periodisch ausgeführt werden.

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[DeviceManagementScripts aufListen](../api/intune-devices-devicemanagementscript-list.md)|[devicemanagementscript hinzugefügt](../resources/intune-devices-devicemanagementscript.md) -Sammlung|AufListen von Eigenschaften und Beziehungen der [devicemanagementscript hinzugefügt](../resources/intune-devices-devicemanagementscript.md) -Objekte.|
|[Devicemanagementscript hinzugefügt abrufen](../api/intune-devices-devicemanagementscript-get.md)|[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)|Lesen von Eigenschaften und Beziehungen des [devicemanagementscript hinzugefügt](../resources/intune-devices-devicemanagementscript.md) -Objekts.|
|[Devicemanagementscript hinzugefügt erstellen](../api/intune-devices-devicemanagementscript-create.md)|[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)|Erstellen eines neuen [devicemanagementscript hinzugefügt](../resources/intune-devices-devicemanagementscript.md) -Objekts.|
|[Devicemanagementscript hinzugefügt löschen](../api/intune-devices-devicemanagementscript-delete.md)|Keine|Löscht eine [devicemanagementscript hinzugefügt](../resources/intune-devices-devicemanagementscript.md).|
|[Devicemanagementscript hinzugefügt aktualisieren](../api/intune-devices-devicemanagementscript-update.md)|[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)|Aktualisieren der Eigenschaften eines [devicemanagementscript hinzugefügt](../resources/intune-devices-devicemanagementscript.md) -Objekts.|
|[assign-Aktion](../api/intune-devices-devicemanagementscript-assign.md)|Keine|Noch nicht dokumentiert|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|string|Eindeutiger Bezeichner für das Geräte Verwaltungsskript.|
|displayName|Zeichenfolge|Name des Geräteverwaltungs-Skripts.|
|description|String|Optionale Beschreibung des Device Management-Skripts.|
|runSchedule|[runSchedule](../resources/intune-devices-runschedule.md)|Das Intervall für die Ausführung des Skripts. Wenn nicht definiert, wird das Skript einmal ausgeführt|
|scriptContent|Binär|Der Skriptinhalt.|
|createdDateTime|DateTimeOffset|Das Datum und die Uhrzeit, zu der das Geräte Verwaltungsskript erstellt wurde.|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung des Geräteverwaltungsskripts.|
|runAsAccount|[runAsAccountType](../resources/intune-shared-runasaccounttype.md)|Gibt den Typ des Ausführungskontexts an, in dem das Geräte Verwaltungsskript ausgeführt wird. Mögliche Werte sind: `system` und `user`.|
|enforceSignatureCheck|Boolean|Geben Sie an, ob die skriptsignatur überprüft werden muss.|
|fileName|Zeichenfolge|Skriptdateiname.|
|Rolescopetagids zur|String collection|Liste der Bereichstag-IDs für diese PowerShellScript-Instanz.|
|runAs32Bit|Boolean|Ein Wert, der angibt, ob das PowerShell-Skript als 32-Bit ausgeführt werden soll|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|groupAssignments|[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) -Sammlung|Die Liste der Gruppenzuweisungen für das Geräte Verwaltungsskript.|
|assignments|[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) -Sammlung|Die Liste der Gruppenzuweisungen für das Geräte Verwaltungsskript.|
|runSummary|[deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md)|Führen Sie eine Zusammenfassung für Device Management-Skripts aus.|
|deviceRunStates|[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) -Sammlung|Liste der Ausführungsstatus für dieses Skript auf allen Geräten.|
|Userrunstates wurden|[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) -Sammlung|Liste der Ausführungsstatus für dieses Skript für alle Benutzer.|

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




