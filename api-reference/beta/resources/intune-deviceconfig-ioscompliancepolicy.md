---
title: iosCompliancePolicy-Ressourcentyp
description: Diese Klasse enthält Konformitätseinstellungen für iOS.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a43ecbac4ddb4ec7c59c3c24ba8b0b3995e6430a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425939"
---
# <a name="ioscompliancepolicy-resource-type"></a>iosCompliancePolicy-Ressourcentyp

> **Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.

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
|roleScopeTagIds|Zeichenfolgenauflistung|Liste der Bereich Tags für diese Instanz der Entität. Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).|
|id|Zeichenfolge|Schlüssel der Entität Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung des Objekts. Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).|
|description|Zeichenfolge|Beschreibung der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung des Objekts. Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).|
|displayName|Zeichenfolge|Name der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).|
|Version|Int32|Version der Gerätekonfiguration. Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).|
|passcodeBlockSimple|Boolean|Gibt an, ob einfache Kennungen erlaubt sind.|
|passcodeExpirationDays|Int32|Zeit in Tagen bis zum Ablaufen der Kennung. Gültige Werte: 1 bis 65535.|
|passcodeMinimumLength|Int32|Mindestlänge von Kennungen. Gültige Werte: 4 bis 14.|
|passcodeMinutesOfInactivityBeforeLock|Int32|Zeitraum von Inaktivität in Minuten, bevor die Eingabe einer Kennung erforderlich ist.|
|passcodeMinutesOfInactivityBeforeScreenTimeout|Int32|Zeitraum von Inaktivität in Minuten, bevor es zu einem Bildschirmtimeout kommt|
|passcodePreviousPasscodeBlockCount|Int32|Anzahl der zuletzt verwendeten Kennungen, die nicht erneut verwendet werden dürfen. Gültige Werte: 1 bis 24.|
|passcodeMinimumCharacterSetCount|Int32|Anzahl der Zeichensätze, die im Kennwort enthalten sein müssen|
|passcodeRequiredType|[requiredPasswordType](../resources/intune-deviceconfig-requiredpasswordtype.md)|Der erforderliche Kennungstyp. Mögliche Werte sind: `deviceDefault`, `alphanumeric` und `numeric`.|
|passcodeRequired|Boolean|Gibt an, ob eine Kennung erforderlich ist.|
|osMinimumVersion|Zeichenfolge|Mindestversion von IOS.|
|osMaximumVersion|Zeichenfolge|Höchstversion von IOS.|
|osMinimumBuildVersion|Zeichenfolge|Minimale IOS Buildversion.|
|osMaximumBuildVersion|Zeichenfolge|Maximale IOS Buildversion.|
|securityBlockJailbrokenDevices|Boolean|Legt fest, dass weder gerootete Geräte verwendet werden dürfen noch Geräte, für die ein Jailbreak durchgeführt wurde.|
|deviceThreatProtectionEnabled|Boolean|Legt fest, dass auf Geräten der Gerätebedrohungsschutz aktiviert sein muss.|
|deviceThreatProtectionRequiredSecurityLevel|[deviceThreatProtectionLevel](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|Legt die Mindestrisikostufe fest, ab der Mobile Threat Protection einen Konformitätsverstoß melden soll. Mögliche Werte sind: `unavailable`, `secured`, `low`, `medium`, `high` und `notSet`.|
|managedEmailProfileRequired|Boolean|Gibt an, ob ein verwaltetes E-Mail-Profil erforderlich ist.|
|restrictedApps|Collection von Objekten des Typs [appListItem](../resources/intune-deviceconfig-applistitem.md)|Benötigen Sie das Gerät nicht die angegebenen apps installiert haben. Diese Sammlung kann maximal 100 Elemente enthalten.|

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
  "roleScopeTagIds": [
    "String"
  ],
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
  "passcodeMinutesOfInactivityBeforeScreenTimeout": 1024,
  "passcodePreviousPasscodeBlockCount": 1024,
  "passcodeMinimumCharacterSetCount": 1024,
  "passcodeRequiredType": "String",
  "passcodeRequired": true,
  "osMinimumVersion": "String",
  "osMaximumVersion": "String",
  "osMinimumBuildVersion": "String",
  "osMaximumBuildVersion": "String",
  "securityBlockJailbrokenDevices": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "String",
  "managedEmailProfileRequired": true,
  "restrictedApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "String",
      "publisher": "String",
      "appStoreUrl": "String",
      "appId": "String"
    }
  ]
}
```




