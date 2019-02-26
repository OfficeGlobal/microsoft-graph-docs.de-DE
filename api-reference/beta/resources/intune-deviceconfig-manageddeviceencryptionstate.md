---
title: managedDeviceEncryptionState-Ressourcentyp
description: Verschlüsselungs Bericht pro Gerät
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ee73ab13ea48707eed745bced197fdd7ae5676b8
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30177847"
---
# <a name="manageddeviceencryptionstate-resource-type"></a>managedDeviceEncryptionState-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Verschlüsselungs Bericht pro Gerät

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[ManagedDeviceEncryptionStates aufListen](../api/intune-deviceconfig-manageddeviceencryptionstate-list.md)|[managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) -Sammlung|AufListen von Eigenschaften und Beziehungen der [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) -Objekte.|
|[ManagedDeviceEncryptionState abrufen](../api/intune-deviceconfig-manageddeviceencryptionstate-get.md)|[managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)|Lesen von Eigenschaften und Beziehungen des [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) -Objekts.|
|[ManagedDeviceEncryptionState erstellen](../api/intune-deviceconfig-manageddeviceencryptionstate-create.md)|[managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)|Erstellen eines neuen [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) -Objekts.|
|[ManagedDeviceEncryptionState löschen](../api/intune-deviceconfig-manageddeviceencryptionstate-delete.md)|Keine|Löscht eine [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md).|
|[ManagedDeviceEncryptionState aktualisieren](../api/intune-deviceconfig-manageddeviceencryptionstate-update.md)|[managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)|Aktualisieren der Eigenschaften eines [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Schlüssel der Entität|
|userPrincipalName|Zeichenfolge|Benutzername|
|deviceType|[deviceTypes](../resources/intune-deviceconfig-devicetypes.md)|Plattform des Geräts. Mögliche Werte sind: `desktop`, `windowsRT`, `winMO6` `nokia` `windowsPhone` `mac` `winCE` `iPhone` `iPad` `iPod` `android` `iSocConsumer` `unix` `macMDM`,,,,,,,, `holoLens`,, `androidEnterprise` ,,,,,, `surfaceHub` `androidForWork` `winEmbedded` , `blackberry`, `palm`, `unknown`.|
|osVersion|String|Betriebssystemversion des Geräts|
|tpmSpecificationVersion|Zeichenfolge|Geräte-TPM-Version|
|deviceName|Zeichenfolge|Gerätename|
|encryptionReadinessState|[encryptionReadinessState](../resources/intune-deviceconfig-encryptionreadinessstate.md)|Verschlüsselungs Bereitschaftsstatus. Mögliche Werte sind: `notReady` und `ready`.|
|encryptionState|[encryptionState](../resources/intune-deviceconfig-encryptionstate.md)|Geräte Verschlüsselungsstatus. Mögliche Werte sind: `notEncrypted` und `encrypted`.|
|encryptionPolicySettingState|[Wurde](../resources/intune-shared-compliancestatus.md)|Status der Verschlüsselungsrichtlinien Einstellung. Mögliche Werte sind: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict` und `notAssigned`.|
|advancedBitLockerStates|[advancedBitLockerState](../resources/intune-deviceconfig-advancedbitlockerstate.md)|Erweiterter BitLocker-Status. Mögliche Werte sind: `success`, `noUserConsent`, `osVolumeEncryptionMethodMismatch` `osVolumeTpmRequired` `osVolumeTpmOnlyRequired` `osVolumeTpmPinRequired` `osVolumeTpmStartupKeyRequired` `recoveryKeyBackupFailed` `fixedDriveNotEncrypted` `fixedDriveEncryptionMethodMismatch` `loggedOnUserNonAdmin` `windowsRecoveryEnvironmentNotConfigured` `tpmNotAvailable`,,,, `tpmNotReady`,,,,,,,,,, `networkError` `osVolumeTpmPinStartupKeyRequired` `osVolumeUnprotected`|
|policyDetails|[encryptionReportPolicyDetails](../resources/intune-deviceconfig-encryptionreportpolicydetails.md) -Sammlung|Richtlinien Details|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDeviceEncryptionState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceEncryptionState",
  "id": "String (identifier)",
  "userPrincipalName": "String",
  "deviceType": "String",
  "osVersion": "String",
  "tpmSpecificationVersion": "String",
  "deviceName": "String",
  "encryptionReadinessState": "String",
  "encryptionState": "String",
  "encryptionPolicySettingState": "String",
  "advancedBitLockerStates": "String",
  "policyDetails": [
    {
      "@odata.type": "microsoft.graph.encryptionReportPolicyDetails",
      "policyId": "String",
      "policyName": "String"
    }
  ]
}
```




