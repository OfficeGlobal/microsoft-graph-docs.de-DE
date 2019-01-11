---
title: deviceCompliancePolicy-Ressourcentyp
description: 'Dies ist die Basisklasse für die Konformitätsrichtlinie. Konformitätsrichtlinien sind plattformspezifisch, und einzelne plattformspezifische Konformitätsrichtlinien erben von dieser Klasse. '
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 8bf029c65d086e8389d5f4cd1a108cc795a785e4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27810122"
---
# <a name="devicecompliancepolicy-resource-type"></a>deviceCompliancePolicy-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Dies ist die Basisklasse für die Konformitätsrichtlinie. Konformitätsrichtlinien sind plattformspezifisch, und einzelne plattformspezifische Konformitätsrichtlinien erben von dieser Klasse. 
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[DeviceCompliancePolicies auflisten](../api/intune-deviceconfig-devicecompliancepolicy-list.md)|[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)-Objekte.|
|[DeviceCompliancePolicy abrufen](../api/intune-deviceconfig-devicecompliancepolicy-get.md)|[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)|Lesen von Eigenschaften und Beziehungen des [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)-Objekts.|
|[assign-Aktion](../api/intune-deviceconfig-devicecompliancepolicy-assign.md)|Sammlung von Objekten des Typs [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)|Noch nicht dokumentiert|
|[scheduleActionsForRules-Aktion](../api/intune-deviceconfig-devicecompliancepolicy-scheduleactionsforrules.md)|Keine|Noch nicht dokumentiert|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|roleScopeTagIds|Collection von Objekten des Typs „String“|Liste der Bereich Tags für diese Instanz der Entität.|
|id|Zeichenfolge|Schlüssel der Entität.|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung des Objekts|
|description|Zeichenfolge|Vom Administrator bereitgestellte Beschreibung der Gerätekonfiguration|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung des Objekts.|
|displayName|Zeichenfolge|Vom Administrator bereitgestellter Name der Gerätekonfiguration|
|version|Int32|Version der Gerätekonfiguration.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|scheduledActionsForRule|Sammlung von Objekten des Typs [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md)|Die Liste der geplanten Aktion für diese Regel|
|deviceStatuses|Sammlung von Objekten des Typs [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md)|Liste von Objekten des Typs „deviceComplianceDeviceStatus“.|
|userStatuses|Sammlung von Objekten des Typs [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md)|Liste von Objekten des Typs „deviceComplianceUserStatus“.|
|deviceStatusOverview|[deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md)|Übersicht über den Status der Gerätekonformität nach Gerät|
|userStatusOverview|[deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md)|Übersicht über den Status der Gerätekonformität nach Benutzer|
|deviceSettingStateSummaries| [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)-Sammlung|Übersicht über den Einstellungsstatus der Konformitätsrichtlinie nach Gerät|
|assignments|Sammlung von Objekten des Typs [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)|Sammlung von Zuweisungen für die Konformitätsrichtlinie.|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceCompliancePolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicy",
  "roleScopeTagIds": [
    "String"
  ],
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "version": 1024
}
```





