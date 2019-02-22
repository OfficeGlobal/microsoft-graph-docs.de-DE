---
title: deviceManagementScriptGroupAssignment-Ressourcentyp
description: Enthält Eigenschaften zum Zuweisen eines Geräteverwaltungsskripts zu einer Gruppe.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 27028d14289e3e0efdfa705d35d02d67d1fb1835
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30154698"
---
# <a name="devicemanagementscriptgroupassignment-resource-type"></a>deviceManagementScriptGroupAssignment-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Enthält Eigenschaften zum Zuweisen eines Geräteverwaltungsskripts zu einer Gruppe.

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[DeviceManagementScriptGroupAssignments aufListen](../api/intune-devices-devicemanagementscriptgroupassignment-list.md)|[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) -Sammlung|AufListen von Eigenschaften und Beziehungen der [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) -Objekte.|
|[DeviceManagementScriptGroupAssignment abrufen](../api/intune-devices-devicemanagementscriptgroupassignment-get.md)|[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)|Lesen von Eigenschaften und Beziehungen des [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) -Objekts.|
|[DeviceManagementScriptGroupAssignment erstellen](../api/intune-devices-devicemanagementscriptgroupassignment-create.md)|[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)|Erstellen eines neuen [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) -Objekts.|
|[DeviceManagementScriptGroupAssignment löschen](../api/intune-devices-devicemanagementscriptgroupassignment-delete.md)|Keine|Löscht eine [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md).|
|[DeviceManagementScriptGroupAssignment aktualisieren](../api/intune-devices-devicemanagementscriptgroupassignment-update.md)|[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)|Aktualisieren der Eigenschaften eines [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Schlüssel der Zuordnungs Entität "Device Management Script Group".|
|targetGroupId|Zeichenfolge|Die ID der Azure Active Directory-Gruppe, auf die wir das Skript ausrichten.|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementScriptGroupAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementScriptGroupAssignment",
  "id": "String (identifier)",
  "targetGroupId": "String"
}
```




