---
title: deviceConfigurationConflictSummary-Ressourcentyp
description: Konflikt Zusammenfassung für eine Reihe von Geräte Konfigurationsrichtlinien.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 50ff4b013f19badbfd510a9b84f8beae4adb621c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30175227"
---
# <a name="deviceconfigurationconflictsummary-resource-type"></a>deviceConfigurationConflictSummary-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Konflikt Zusammenfassung für eine Reihe von Geräte Konfigurationsrichtlinien.

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[DeviceConfigurationConflictSummaries aufListen](../api/intune-deviceconfig-deviceconfigurationconflictsummary-list.md)|[deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) -Sammlung|AufListen von Eigenschaften und Beziehungen der [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) -Objekte.|
|[DeviceConfigurationConflictSummary abrufen](../api/intune-deviceconfig-deviceconfigurationconflictsummary-get.md)|[deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)|Lesen von Eigenschaften und Beziehungen des [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) -Objekts.|
|[DeviceConfigurationConflictSummary erstellen](../api/intune-deviceconfig-deviceconfigurationconflictsummary-create.md)|[deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)|Erstellen eines neuen [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) -Objekts.|
|[DeviceConfigurationConflictSummary löschen](../api/intune-deviceconfig-deviceconfigurationconflictsummary-delete.md)|Keine|Löscht eine [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md).|
|[DeviceConfigurationConflictSummary aktualisieren](../api/intune-deviceconfig-deviceconfigurationconflictsummary-update.md)|[deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)|Aktualisieren der Eigenschaften eines [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|conflictingDeviceConfigurations|[settingSource](../resources/intune-deviceconfig-settingsource.md)-Sammlung|Die Gruppe von Richtlinien, die mit der angegebenen Einstellung in Konflikt stehen|
|id|Zeichenfolge|Die ID für diesen Satz von Konflikt verursachenden Richtlinien. Diese ID ist die IDs aller Richtlinien in ConflictingDeviceConfigurations in lexikografische Reihenfolge durch Unterstriche getrennt.|
|contributingSettings|String collection|Die Gruppe von Einstellungen, die mit den angegebenen Richtlinien in Konflikt stehen|
|deviceCheckinsImpacted|Int32|Die Anzahl der checkins, die von den widersprüchlichen Richtlinien und Einstellungen beeinflusst wurden|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfigurationConflictSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationConflictSummary",
  "conflictingDeviceConfigurations": [
    {
      "@odata.type": "microsoft.graph.settingSource",
      "id": "String",
      "displayName": "String"
    }
  ],
  "id": "String (identifier)",
  "contributingSettings": [
    "String"
  ],
  "deviceCheckinsImpacted": 1024
}
```




