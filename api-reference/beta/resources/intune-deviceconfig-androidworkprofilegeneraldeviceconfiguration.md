---
title: androidWorkProfileGeneralDeviceConfiguration-Ressourcentyp
description: Allgemeine Gerätekonfiguration für Android-Arbeitsprofil.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8ba742fa77baacec4651aad3e1434c3434441a49
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30165835"
---
# <a name="androidworkprofilegeneraldeviceconfiguration-resource-type"></a>androidWorkProfileGeneralDeviceConfiguration-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Allgemeine Gerätekonfiguration für Android-Arbeitsprofil.


Sie erbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[AndroidWorkProfileGeneralDeviceConfigurations aufListen](../api/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration-list.md)|[androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) -Sammlung|AufListen von Eigenschaften und Beziehungen der [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) -Objekte.|
|[AndroidWorkProfileGeneralDeviceConfiguration abrufen](../api/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration-get.md)|[androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md)|Lesen von Eigenschaften und Beziehungen des [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) -Objekts.|
|[AndroidWorkProfileGeneralDeviceConfiguration erstellen](../api/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration-create.md)|[androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md)|Erstellen eines neuen [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) -Objekts.|
|[AndroidWorkProfileGeneralDeviceConfiguration löschen](../api/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration-delete.md)|Keine|Löscht eine [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md).|
|[AndroidWorkProfileGeneralDeviceConfiguration aktualisieren](../api/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration-update.md)|[androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md)|Aktualisieren der Eigenschaften eines [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|string|Schlüssel der Entität Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung des Objekts. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|Rolescopetagids zur|String collection|Liste der Bereichs Tags für diese Entitätsinstanz. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|supportsScopeTags|Boolescher Wert|Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereichs Tags unterstützt. Das Zuweisen zur ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert auf false festgelegt ist und Entitäten für bereichsbezogene Benutzer nicht sichtbar sind. Dies geschieht für in Silverlight erstellte Legacy Richtlinien und kann durch Löschen und erneutes Erstellen der Richtlinie im Azure-Portal aufgelöst werden. Diese Eigenschaft ist schreibgeschützt. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung des Objekts. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|description|Zeichenfolge|Beschreibung der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|displayName|Zeichenfolge|Name der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|Version|Int32|Version der Gerätekonfiguration. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|passwordBlockFingerprintUnlock|Boolean|Gibt an, ob die Entsperrung durch Fingerabdruck blockiert werden soll.|
|passwordBlockTrustAgents|Boolescher Wert|Gibt an, ob Smart Lock oder andere Vertrauensstellungs-Agents blockiert werden sollen.|
|passwordExpirationDays|Int32|Zeit in Tagen bis zum Ablaufen des Kennworts. Gültige Werte: 1 bis 365.|
|passwordMinimumLength|Int32|Mindestlänge von Kennwörtern. Gültige Werte: 4 bis 16.|
|passwordMinutesOfInactivityBeforeScreenTimeout|Int32|Zeitraum von Inaktivität in Minuten, bevor es zu einem Bildschirmtimeout kommt|
|passwordPreviousPasswordBlockCount|Int32|Anzahl der zuletzt verwendeten Kennwörter, die nicht erneut verwendet werden dürfen. Gültige Werte: 0 bis 24.|
|passwordSignInFailureCountBeforeFactoryReset|Int32|Legt fest, nach wie vielen fehlgeschlagenen Anmeldeversuchen eine Zurücksetzung auf die Werkseinstellungen durchgeführt wird. Gültige Werte 1 bis 16|
|passwordRequiredType|[androidWorkProfileRequiredPasswordType](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|Geforderter Kennworttyp. Mögliche Werte sind: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric` und `alphanumericWithSymbols`.|
|workProfileDataSharingType|[androidWorkProfileCrossProfileDataSharingType](../resources/intune-deviceconfig-androidworkprofilecrossprofiledatasharingtype.md)|Typ der zulässigen Datenfreigabe. Mögliche Werte: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.|
|workProfileBlockNotificationsWhileDeviceLocked|Boolescher Wert|Gibt an, ob Benachrichtigungen blockiert werden sollen, während das Gerät gesperrt ist.|
|workProfileBlockAddingAccounts|Boolescher Wert|Verhindern, dass Benutzerkonten im Arbeitsprofil hinzufügen/entfernen.|
|workProfileBluetoothEnableContactSharing|Boolescher Wert|Bluetooth-Geräte können auf Enterprise-Kontakte zugreifen.|
|workProfileBlockScreenCapture|Boolescher Wert|Blockieren der Bildschirmaufzeichnung im Arbeitsprofil.|
|workProfileBlockCrossProfileCallerId|Boolescher Wert|Blockieren der Anzeige von Arbeitsprofil-Anrufer-ID im persönlichen Profil.|
|workProfileBlockCamera|Boolescher Wert|Arbeitsprofil Kamera blockieren.|
|workProfileBlockCrossProfileContactsSearch|Boolescher Wert|Blockieren der Verfügbarkeit von Arbeitsprofil Kontakten im persönlichen Profil|
|workProfileBlockCrossProfileCopyPaste|Boolescher Wert|Boolescher Wert, der angibt, ob die Einstellung Cross profile Copy/Paste nicht zulassen aktiviert ist.|
|workProfileDefaultAppPermissionPolicy|[androidWorkProfileDefaultAppPermissionPolicyType](../resources/intune-deviceconfig-androidworkprofiledefaultapppermissionpolicytype.md)|Geforderter Kennworttyp. Mögliche Werte: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.|
|Eigenschaften workprofilepasswordblockfingerprintunlock|Boolescher Wert|Gibt an, ob die Fingerabdruck Sperre für das Arbeitsprofil blockiert werden soll.|
|workProfilePasswordBlockTrustAgents|Boolescher Wert|Gibt an, ob die Smart Lock-und andere Trust-Agents für das Arbeitsprofil blockiert werden sollen.|
|workProfilePasswordExpirationDays|Int32|Anzahl der Tage vor Ablauf des Arbeitsprofil Kennworts. Gültige Werte: 1 bis 365.|
|workProfilePasswordMinimumLength|Int32|Minimale Länge des Arbeitsprofil Kennworts. Gültige Werte: 4 bis 16.|
|workProfilePasswordMinNumericCharacters|Int32|Minimale Anzahl von numerischen Zeichen, die im Arbeitsprofil Kennwort erforderlich sind. Gültige Werte 1 bis 10|
|workProfilePasswordMinNonLetterCharacters|Int32|Mindestanzahl von Buchstaben, die im Arbeitsprofil Kennwort erforderlich sind. Gültige Werte 1 bis 10|
|workProfilePasswordMinLetterCharacters|Int32|Mindestanzahl von Buchstaben, die im Arbeitsprofil Kennwort erforderlich sind. Gültige Werte 1 bis 10|
|workProfilePasswordMinLowerCaseCharacters|Int32|Minimale Anzahl von Kleinbuchstaben, die im Arbeitsprofil Kennwort erforderlich sind. Gültige Werte 1 bis 10|
|workProfilePasswordMinUpperCaseCharacters|Int32|Minimale Anzahl von Großbuchstaben, die im Arbeitsprofil Kennwort erforderlich sind. Gültige Werte 1 bis 10|
|workProfilePasswordMinSymbolCharacters|Int32|Minimale Anzahl von Symbolen, die im Arbeitsprofil Kennwort erforderlich sind. Gültige Werte 1 bis 10|
|workProfilePasswordMinutesOfInactivityBeforeScreenTimeout|Int32|Zeitraum von Inaktivität in Minuten, bevor es zu einem Bildschirmtimeout kommt|
|workProfilePasswordPreviousPasswordBlockCount|Int32|Anzahl der vorherigen Arbeitsprofil Kennwörter, die blockiert werden sollen. Gültige Werte: 0 bis 24.|
|workProfilePasswordSignInFailureCountBeforeFactoryReset|Int32|Anzahl der zulässigen Anmeldefehler vor dem Entfernen des Arbeitsprofils und aller gelöschten Unternehmensdaten. Gültige Werte 1 bis 16|
|workProfilePasswordRequiredType|[androidWorkProfileRequiredPasswordType](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|Typ des erforderlichen Arbeitsprofil Kennworts. Mögliche Werte sind: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric` und `alphanumericWithSymbols`.|
|Workprofilerequirepassword wurden|Boolescher Wert|Kennwort ist erforderlich oder nicht für das Arbeitsprofil|
|securityRequireVerifyApps|Boolescher Wert|Legt fest, dass die Android-Funktion „Verify Apps“ aktiviert sein muss.|
|vpnAlwaysOnPackageIdentifier|Zeichenfolge|Aktivieren Sie den Sperrmodus für Always-on-VPN.|
|vpnEnableAlwaysOnLockdownMode|Boolescher Wert|Aktivieren Sie den Sperrmodus für Always-on-VPN.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|groupAssignments|[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) -Sammlung|Die Liste derGruppenzuweisungen für das Gerätekonfigurationsprofil. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|assignments|[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)-Sammlung|Liste der Zuweisungen für das Gerätekonfigurationsprofil. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceStatuses|[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)-Sammlung|Installationsstatus der Gerätekonfiguration nach Gerät. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|userStatuses|[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)-Sammlung|Installationsstatus der Gerätekonfiguration nach Benutzer. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|Übersicht über den Status der Gerätekonfiguration nach Gerät. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|Übersicht über den Status der Gerätekonfiguration nach Benutzer. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceSettingStateSummaries| [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)-Sammlung|Übersicht über den Einstellungsstatus für die Gerätekonfiguration nach Gerät. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidWorkProfileGeneralDeviceConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidWorkProfileGeneralDeviceConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockTrustAgents": true,
  "passwordExpirationDays": 1024,
  "passwordMinimumLength": 1024,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 1024,
  "passwordPreviousPasswordBlockCount": 1024,
  "passwordSignInFailureCountBeforeFactoryReset": 1024,
  "passwordRequiredType": "String",
  "workProfileDataSharingType": "String",
  "workProfileBlockNotificationsWhileDeviceLocked": true,
  "workProfileBlockAddingAccounts": true,
  "workProfileBluetoothEnableContactSharing": true,
  "workProfileBlockScreenCapture": true,
  "workProfileBlockCrossProfileCallerId": true,
  "workProfileBlockCamera": true,
  "workProfileBlockCrossProfileContactsSearch": true,
  "workProfileBlockCrossProfileCopyPaste": true,
  "workProfileDefaultAppPermissionPolicy": "String",
  "workProfilePasswordBlockFingerprintUnlock": true,
  "workProfilePasswordBlockTrustAgents": true,
  "workProfilePasswordExpirationDays": 1024,
  "workProfilePasswordMinimumLength": 1024,
  "workProfilePasswordMinNumericCharacters": 1024,
  "workProfilePasswordMinNonLetterCharacters": 1024,
  "workProfilePasswordMinLetterCharacters": 1024,
  "workProfilePasswordMinLowerCaseCharacters": 1024,
  "workProfilePasswordMinUpperCaseCharacters": 1024,
  "workProfilePasswordMinSymbolCharacters": 1024,
  "workProfilePasswordMinutesOfInactivityBeforeScreenTimeout": 1024,
  "workProfilePasswordPreviousPasswordBlockCount": 1024,
  "workProfilePasswordSignInFailureCountBeforeFactoryReset": 1024,
  "workProfilePasswordRequiredType": "String",
  "workProfileRequirePassword": true,
  "securityRequireVerifyApps": true,
  "vpnAlwaysOnPackageIdentifier": "String",
  "vpnEnableAlwaysOnLockdownMode": true
}
```




