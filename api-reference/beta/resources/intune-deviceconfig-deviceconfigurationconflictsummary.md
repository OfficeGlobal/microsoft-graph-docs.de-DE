---
title: Ressourcentyp deviceConfigurationConflictSummary
description: Zusammenfassung für einen Satz von Richtlinien für die Konfiguration von Geräte Konflikt.
ms.openlocfilehash: b292dd40bfb0502aa55109072ee9e9f59a8eb45a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061990"
---
# <a name="deviceconfigurationconflictsummary-resource-type"></a>Ressourcentyp deviceConfigurationConflictSummary

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Zusammenfassung für einen Satz von Richtlinien für die Konfiguration von Geräte Konflikt.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Liste deviceConfigurationConflictSummaries](../api/intune-deviceconfig-deviceconfigurationconflictsummary-list.md)|[DeviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) -Auflistung|Listeneigenschaften und Beziehungen der [DeviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) -Objekte.|
|[Abrufen von deviceConfigurationConflictSummary](../api/intune-deviceconfig-deviceconfigurationconflictsummary-get.md)|[deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)|Lesen Sie Eigenschaften und Beziehungen des [DeviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) -Objekts.|
|[Erstellen von deviceConfigurationConflictSummary](../api/intune-deviceconfig-deviceconfigurationconflictsummary-create.md)|[deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)|Erstellen eines neuen [DeviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) -Objekts.|
|[DeviceConfigurationConflictSummary löschen](../api/intune-deviceconfig-deviceconfigurationconflictsummary-delete.md)|Keines|Löscht eine [DeviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md).|
|[DeviceConfigurationConflictSummary aktualisieren](../api/intune-deviceconfig-deviceconfigurationconflictsummary-update.md)|[deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)|Aktualisieren Sie die Eigenschaften eines [DeviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|conflictingDeviceConfigurations|[settingSource](../resources/intune-deviceconfig-settingsource.md)-Sammlung|Der Satz von Richtlinien mit der angegebenen Einstellung in Konflikt|
|id|String|Die Id für diesen Satz von miteinander in Konflikt stehende Richtlinien. Diese Id ist die Ids aller Richtlinien in ConflictingDeviceConfigurations in lexikografischer Reihenfolge durch Unterstriche getrennt sind.|
|contributingSettings|Collection von Objekten des Typs „String“|Die Gruppe von Einstellungen in Konflikt mit der angegebenen Richtlinien|
|deviceCheckinsImpacted|Int32|Die Anzahl der durch die miteinander in Konflikt stehende Richtlinien und Einstellungen beeinträchtigt Eincheckvorgänge|

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





