---
title: deviceConfigurationAssignment-Ressourcentyp
description: Die Zuweisungsentität für die Gerätekonfiguration weist eine AAD-Gruppe einer bestimmten Gerätekonfiguration zu.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 80645a7b6724a71620eeebf4dfb4ba8a1b440db2
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30172632"
---
# <a name="deviceconfigurationassignment-resource-type"></a>deviceConfigurationAssignment-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Die Zuweisungsentität für die Gerätekonfiguration weist eine AAD-Gruppe einer bestimmten Gerätekonfiguration zu.

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[deviceConfigurationAssignments auflisten](../api/intune-deviceconfig-deviceconfigurationassignment-list.md)|[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)-Objekte.|
|[deviceConfigurationAssignment abrufen](../api/intune-deviceconfig-deviceconfigurationassignment-get.md)|[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|Lesen von Eigenschaften und Beziehungen des [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)-Objekts.|
|[deviceConfigurationAssignment erstellen](../api/intune-deviceconfig-deviceconfigurationassignment-create.md)|[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|Erstellen eines neuen [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)-Objekts.|
|[deviceConfigurationAssignment löschen](../api/intune-deviceconfig-deviceconfigurationassignment-delete.md)|Keine|Löscht ein [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)-Objekt.|
|[deviceConfigurationAssignment aktualisieren](../api/intune-deviceconfig-deviceconfigurationassignment-update.md)|[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|Aktualisieren der Eigenschaften eines [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Schlüssel der Zuweisung|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|Das Zuweisungsziel für die Gerätekonfiguration.|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfigurationAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```




