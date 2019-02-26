---
title: deviceManagementScriptAssignment-Ressourcentyp
description: Enthält Eigenschaften zum Zuweisen eines Geräteverwaltungsskripts zu einer Gruppe.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f7b3e777da3d50b7b044d0ebc406e95c65bdc892
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30165380"
---
# <a name="devicemanagementscriptassignment-resource-type"></a>deviceManagementScriptAssignment-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Enthält Eigenschaften zum Zuweisen eines Geräteverwaltungsskripts zu einer Gruppe.

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[DeviceManagementScriptAssignments aufListen](../api/intune-devices-devicemanagementscriptassignment-list.md)|[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) -Sammlung|AufListen von Eigenschaften und Beziehungen der [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) -Objekte.|
|[DeviceManagementScriptAssignment abrufen](../api/intune-devices-devicemanagementscriptassignment-get.md)|[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)|Lesen von Eigenschaften und Beziehungen des [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) -Objekts.|
|[DeviceManagementScriptAssignment erstellen](../api/intune-devices-devicemanagementscriptassignment-create.md)|[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)|Erstellen eines neuen [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) -Objekts.|
|[DeviceManagementScriptAssignment löschen](../api/intune-devices-devicemanagementscriptassignment-delete.md)|Keine|Löscht eine [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md).|
|[DeviceManagementScriptAssignment aktualisieren](../api/intune-devices-devicemanagementscriptassignment-update.md)|[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)|Aktualisieren der Eigenschaften eines [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Schlüssel der Zuordnungs Entität "Device Management Script Group".|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|Die ID der Azure Active Directory-Gruppe, auf die wir das Skript ausrichten.|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementScriptAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementScriptAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```




