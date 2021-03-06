---
title: deviceCompliancePolicy-Ressourcentyp
description: 'Dies ist die Basisklasse für die Konformitätsrichtlinie. Konformitätsrichtlinien sind plattformspezifisch, und einzelne plattformspezifische Konformitätsrichtlinien erben von dieser Klasse. '
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e556fd8619ef16b4212711511592de2b26e4772a
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30255612"
---
# <a name="devicecompliancepolicy-resource-type"></a>deviceCompliancePolicy-Ressourcentyp

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Dies ist die Basisklasse für die Konformitätsrichtlinie. Konformitätsrichtlinien sind plattformspezifisch, und einzelne plattformspezifische Konformitätsrichtlinien erben von dieser Klasse. 

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[DeviceCompliancePolicies auflisten](../api/intune-deviceconfig-devicecompliancepolicy-list.md)|[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)-Objekte.|
|[DeviceCompliancePolicy abrufen](../api/intune-deviceconfig-devicecompliancepolicy-get.md)|[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)|Lesen von Eigenschaften und Beziehungen des [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)-Objekts.|
|[assign-Aktion](../api/intune-deviceconfig-devicecompliancepolicy-assign.md)|Sammlung von Objekten des Typs [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)|Noch nicht dokumentiert|
|[scheduleActionsForRules-Aktion](../api/intune-deviceconfig-devicecompliancepolicy-scheduleactionsforrules.md)|Keine|Noch nicht dokumentiert.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|string|Schlüssel der Entität.|
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
|assignments|Collection von Objekten des Typs [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)|Sammlung von Zuweisungen für die Konformitätsrichtlinie.|

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
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "version": 1024
}
```



