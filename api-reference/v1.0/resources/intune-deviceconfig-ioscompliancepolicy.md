---
title: iosCompliancePolicy-Ressourcentyp
description: Diese Klasse enthält Konformitätseinstellungen für iOS.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 1e5a2ef72769694d2dd4c5d7ae6e296d429c49b5
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27935955"
---
# <a name="ioscompliancepolicy-resource-type"></a>iosCompliancePolicy-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Diese Klasse enthält Konformitätseinstellungen für iOS.

Sie erbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[iosCompliancePolicies auflisten](../api/intune-deviceconfig-ioscompliancepolicy-list.md)|[iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md)-Objekte.|
|[iosCompliancePolicy abrufen](../api/intune-deviceconfig-ioscompliancepolicy-get.md)|[iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md)|Lesen von Eigenschaften und Beziehungen des [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md)-Objekts.|
|[iosCompliancePolicy erstellen](../api/intune-deviceconfig-ioscompliancepolicy-create.md)|[iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md)|Erstellen eines neuen [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md)-Objekts.|
|[iosCompliancePolicy löschen](../api/intune-deviceconfig-ioscompliancepolicy-delete.md)|Keine|Löscht ein [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md)-Objekt.|
|[iosCompliancePolicy aktualisieren](../api/intune-deviceconfig-ioscompliancepolicy-update.md)|[iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md)|Aktualisieren der Eigenschaften eines [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Schlüssel der Entität Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung des Objekts. Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).|
|description|Zeichenfolge|Beschreibung der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung des Objekts. Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).|
|displayName|Zeichenfolge|Name der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).|
|Version|Int32|Version der Gerätekonfiguration. Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).|
|passcodeBlockSimple|Boolescher Wert|Gibt an, ob einfache Kennungen erlaubt sind.|
|passcodeExpirationDays|Int32|Zeit in Tagen bis zum Ablaufen der Kennung. Gültige Werte: 1 bis 65535.|
|passcodeMinimumLength|Int32|Mindestlänge von Kennungen. Gültige Werte: 4 bis 14.|
|passcodeMinutesOfInactivityBeforeLock|Int32|Zeitraum von Inaktivität in Minuten, bevor die Eingabe einer Kennung erforderlich ist.|
|passcodePreviousPasscodeBlockCount|Int32|Anzahl der zuletzt verwendeten Kennungen, die nicht erneut verwendet werden dürfen. Gültige Werte: 1 bis 24.|
|passcodeMinimumCharacterSetCount|Int32|Anzahl der Zeichensätze, die im Kennwort enthalten sein müssen|
|passcodeRequiredType|[requiredPasswordType](../resources/intune-deviceconfig-requiredpasswordtype.md)|Der erforderliche Kennungstyp. Mögliche Werte sind: `deviceDefault`, `alphanumeric` und `numeric`.|
|passcodeRequired|Boolescher Wert|Gibt an, ob eine Kennung erforderlich ist.|
|osMinimumVersion|Zeichenfolge|Mindestversion von IOS.|
|osMaximumVersion|Zeichenfolge|Höchstversion von IOS.|
|securityBlockJailbrokenDevices|Boolescher Wert|Legt fest, dass weder gerootete Geräte verwendet werden dürfen noch Geräte, für die ein Jailbreak durchgeführt wurde.|
|deviceThreatProtectionEnabled|Boolescher Wert|Legt fest, dass auf Geräten der Gerätebedrohungsschutz aktiviert sein muss.|
|deviceThreatProtectionRequiredSecurityLevel|[deviceThreatProtectionLevel](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|Legt die Mindestrisikostufe fest, ab der Mobile Threat Protection einen Konformitätsverstoß melden soll. Mögliche Werte sind: `unavailable`, `secured`, `low`, `medium`, `high` und `notSet`.|
|managedEmailProfileRequired|Boolescher Wert|Gibt an, ob ein verwaltetes E-Mail-Profil erforderlich ist.|

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
  "@odata.type": "microsoft.graph.iosCompliancePolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosCompliancePolicy",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "version": 1024,
  "passcodeBlockSimple": true,
  "passcodeExpirationDays": 1024,
  "passcodeMinimumLength": 1024,
  "passcodeMinutesOfInactivityBeforeLock": 1024,
  "passcodePreviousPasscodeBlockCount": 1024,
  "passcodeMinimumCharacterSetCount": 1024,
  "passcodeRequiredType": "String",
  "passcodeRequired": true,
  "osMinimumVersion": "String",
  "osMaximumVersion": "String",
  "securityBlockJailbrokenDevices": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "String",
  "managedEmailProfileRequired": true
}
```



