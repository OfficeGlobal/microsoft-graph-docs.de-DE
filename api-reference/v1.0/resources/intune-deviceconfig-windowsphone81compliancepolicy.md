---
title: windowsPhone81CompliancePolicy-Ressourcentyp
description: Diese Klasse enthält Konformitätseinstellungen für Windows 8.1 Mobile.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 84299987b57133b2a48b739d9d88ed38398252b5
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30255087"
---
# <a name="windowsphone81compliancepolicy-resource-type"></a>windowsPhone81CompliancePolicy-Ressourcentyp

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Diese Klasse enthält Konformitätseinstellungen für Windows 8.1 Mobile.


Sie erbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[WindowsPhone81CompliancePolicies auflisten](../api/intune-deviceconfig-windowsphone81compliancepolicy-list.md)|[windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md)-Objekte.|
|[WindowsPhone81CompliancePolicy abrufen](../api/intune-deviceconfig-windowsphone81compliancepolicy-get.md)|[windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md)|Lesen von Eigenschaften und Beziehungen des [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md)-Objekts.|
|[WindowsPhone81CompliancePolicy erstellen](../api/intune-deviceconfig-windowsphone81compliancepolicy-create.md)|[windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md)|Erstellen eines neuen [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md)-Objekts.|
|[WindowsPhone81CompliancePolicy löschen](../api/intune-deviceconfig-windowsphone81compliancepolicy-delete.md)|Keine|Löscht ein [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md)-Objekt.|
|[WindowsPhone81CompliancePolicy aktualisieren](../api/intune-deviceconfig-windowsphone81compliancepolicy-update.md)|[windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md)|Aktualisieren der Eigenschaften eines [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|string|Schlüssel der Entität Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung des Objekts. Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).|
|description|String|Beschreibung der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung des Objekts. Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).|
|displayName|Zeichenfolge|Name der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).|
|Version|Int32|Version der Gerätekonfiguration. Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).|
|passwordBlockSimple|Boolean|Gibt an, ob die Kalendersynchronisierung blockiert werden soll.|
|passwordExpirationDays|Int32|Zeit in Tagen bis zum Ablaufen des Kennworts.|
|passwordMinimumLength|Int32|Mindestlänge von Kennwörtern|
|passwordMinutesOfInactivityBeforeLock|Int32|Zeitraum von Inaktivität in Minuten, nach dem die Eingabe eines Kennworts gefordert wird|
|passwordMinimumCharacterSetCount|Int32|Anzahl der Zeichensätze, die im Kennwort enthalten sein müssen|
|passwordRequiredType|[requiredPasswordType](../resources/intune-deviceconfig-requiredpasswordtype.md)|Geforderter Kennworttyp. Mögliche Werte sind: `deviceDefault`, `alphanumeric` und `numeric`.|
|passwordPreviousPasswordBlockCount|Int32|Anzahl der zuletzt verwendeten Kennwörter, die nicht erneut verwendet werden dürfen. Gültige Werte: 0 bis 24.|
|passwordRequired|Boolean|Legt fest, ob ein Kennwort gefordert wird.|
|osMinimumVersion|Zeichenfolge|Mindestversion von Windows Phone|
|osMaximumVersion|Zeichenfolge|Maximalversion von Windows Phone|
|storageRequireEncryption|Boolean|Verschlüsselung auf Windows Phone-Geräten erforderlich|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|scheduledActionsForRule|Sammlung von Objekten des Typs [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md)|Liste der geplanten Aktionen für die Regel. Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).|
|deviceStatuses|Sammlung von Objekten des Typs [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md)|Liste von Objekten des Typs „deviceComplianceDeviceStatus“. Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).|
|userStatuses|Sammlung von Objekten des Typs [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md)|Liste von Objekten des Typs „deviceComplianceUserStatus“. Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).|
|deviceStatusOverview|[deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md)|Übersicht über den Status der Gerätekonformität nach Gerät. Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).|
|userStatusOverview|[deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md)|Übersicht über den Status der Gerätekonformität nach Benutzer. Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).|
|deviceSettingStateSummaries| [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)-Sammlung|Übersicht über den Einstellungsstatus der Konformitätsrichtlinie nach Gerät. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-devicecompliancepolicy.md).|
|assignments|Sammlung von Objekten des Typs [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)|Sammlung von Zuweisungen für die Konformitätsrichtlinie. Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsPhone81CompliancePolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsPhone81CompliancePolicy",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "version": 1024,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 1024,
  "passwordMinimumLength": 1024,
  "passwordMinutesOfInactivityBeforeLock": 1024,
  "passwordMinimumCharacterSetCount": 1024,
  "passwordRequiredType": "String",
  "passwordPreviousPasswordBlockCount": 1024,
  "passwordRequired": true,
  "osMinimumVersion": "String",
  "osMaximumVersion": "String",
  "storageRequireEncryption": true
}
```



