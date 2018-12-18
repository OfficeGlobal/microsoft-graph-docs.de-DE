---
title: Ressourcentyp windowsManagedDevice
description: Windows-Geräte, die verwaltet werden, oder über Intune Einschreibung
author: tfitzmac
ms.openlocfilehash: d432e4cdc4552117de56362df0fd632f6bc1719e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27328938"
---
# <a name="windowsmanageddevice-resource-type"></a>Ressourcentyp windowsManagedDevice

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Windows-Geräte, die verwaltet werden, oder über Intune Einschreibung

Erbt vom [managedDevice](../resources/intune-devices-manageddevice.md)

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Liste windowsManagedDevices](../api/intune-devices-windowsmanageddevice-list.md)|[WindowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) -Auflistung|Listeneigenschaften und Beziehungen der [WindowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) -Objekte.|
|[Abrufen von windowsManagedDevice](../api/intune-devices-windowsmanageddevice-get.md)|[windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md)|Lesen Sie Eigenschaften und Beziehungen des [WindowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) -Objekts.|
|[Erstellen von windowsManagedDevice](../api/intune-devices-windowsmanageddevice-create.md)|[windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md)|Erstellen eines neuen [WindowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) -Objekts.|
|[WindowsManagedDevice löschen](../api/intune-devices-windowsmanageddevice-delete.md)|Keines|Löscht eine [WindowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md).|
|[WindowsManagedDevice aktualisieren](../api/intune-devices-windowsmanageddevice-update.md)|[windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md)|Aktualisieren Sie die Eigenschaften eines [WindowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Eindeutiger Bezeichner für das Gerät Inherited aus [managedDevice](../resources/intune-devices-manageddevice.md)|
|userId|String|Eindeutiger Bezeichner für den Benutzer mit dem Gerät Inherited aus [managedDevice](../resources/intune-devices-manageddevice.md)|
|deviceName|String|Name des Geräts Inherited aus [managedDevice](../resources/intune-devices-manageddevice.md)|
|hardwareInformation|[hardwareInformation](../resources/intune-devices-hardwareinformation.md)|Die Hardward Details für das Gerät.  Enthält Informationen, wie Speicherplatz, Hersteller, Seriennummer. Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)|
|Besitzertyp|[Besitzertyp](../resources/intune-devices-ownertype.md)|Besitz des Geräts. "Unternehmen" oder "personal" Inherited aus [ManagedDevice](../resources/intune-devices-manageddevice.md)möglich. Mögliche Werte sind: `unknown`, `company` und `personal`.|
|managedDeviceOwnerType|[managedDeviceOwnerType](../resources/intune-devices-manageddeviceownertype.md)|Besitz des Geräts. "Unternehmen" oder "personal" Inherited aus [ManagedDevice](../resources/intune-devices-manageddevice.md)möglich. Mögliche Werte sind: `unknown`, `company` und `personal`.|
|deviceActionResults|Collection von Objekten des Typs [deviceActionResult](../resources/intune-devices-deviceactionresult.md)|Liste von Objekten des Typs „ComplexType deviceActionResult“.
 Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)|
|managementState|[managementState](../resources/intune-devices-managementstate.md)|Verwaltungsstatus des Geräts. Geerbt von [ManagedDevice](../resources/intune-devices-manageddevice.md). Mögliche Werte sind: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled` und `discovered`.|
|enrolledDateTime|DateTimeOffset|Datum und Uhrzeit der Geräteregistrierung.
 Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)|
|lastSyncDateTime|DateTimeOffset|Datum und Uhrzeit der letzten erfolgreichen Synchronisierung des Geräts mit Intune.
 Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)|
|chassisType|[chassisType](../resources/intune-devices-chassistype.md)|Chassistyp des Geräts. Geerbt von [ManagedDevice](../resources/intune-devices-manageddevice.md). Mögliche Werte: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.|
|operatingSystem|String|Betriebssystem des Geräts. Windows iOS usw.. Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)|
|deviceType|[deviceType](../resources/intune-shared-devicetype.md)|Plattform des Geräts. Geerbt von [ManagedDevice](../resources/intune-devices-manageddevice.md). Mögliche Werte sind: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise` , `blackberry`, `palm`, `unknown`.|
|complianceState|[complianceState](../resources/intune-devices-compliancestate.md)|Konformitätsstatus des Geräts. Geerbt von [ManagedDevice](../resources/intune-devices-manageddevice.md). Mögliche Werte sind: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod` und `configManager`.|
|jailBroken|String|Gibt an, ob es sich um ein Gerät mit Jailbreak oder Rootzugriff handelt. Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)|
|managementAgent|[managementAgentType](../resources/intune-devices-managementagenttype.md)|Verwaltungskanal des Geräts. Intune, EAS usw. Geerbt von [ManagedDevice](../resources/intune-devices-manageddevice.md). Mögliche Werte sind: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController` und `microsoft365ManagedMdm`.|
|osVersion|String|Auf dem Gerät installierte Betriebssystemversion.
 Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)|
|easActivated|Boolescher Wert|Gibt an, ob für das Gerät Exchange ActiveSync aktiviert ist. Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)|
|easDeviceId|String|Exchange ActiveSync-ID des Geräts.
 Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)|
|easActivationDateTime|DateTimeOffset|Datum und Uhrzeit der Exchange ActiveSync-Aktivierung für das Gerät.
 Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)|
|aadRegistered|Boolescher Wert|Gibt an, ob das Gerät in Azure Active Directory registriert ist. Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)|
|azureADRegistered|Boolescher Wert|Gibt an, ob das Gerät in Azure Active Directory registriert ist. Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)|
|deviceEnrollmentType|[deviceEnrollmentType](../resources/intune-shared-deviceenrollmenttype.md)|Registrierungstyp des Geräts. Geerbt von [ManagedDevice](../resources/intune-devices-manageddevice.md). Mögliche Werte: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.|
|lostModeState|[lostModeState](../resources/intune-devices-lostmodestate.md)|Gibt an, ob verloren Modus aktiviert ist oder Inherited aus [ManagedDevice deaktiviert](../resources/intune-devices-manageddevice.md). Mögliche Werte sind: `disabled` und `enabled`.|
|activationLockBypassCode|String|Code, der die Umgehung der Aktivierungssperre des Geräts ermöglicht Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)|
|emailAddress|String|Email(s) für den Benutzer mit dem Gerät Inherited aus [managedDevice](../resources/intune-devices-manageddevice.md)|
|azureActiveDirectoryDeviceId|String|Eindeutiger Bezeichner des Azure Active Directory-Geräts. Schreibgeschützt. Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)|
|azureADDeviceId|String|Eindeutiger Bezeichner des Azure Active Directory-Geräts. Schreibgeschützt. Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)|
|deviceRegistrationState|[deviceRegistrationState](../resources/intune-devices-deviceregistrationstate.md)|Registrierungsstatus des Geräts. Geerbt von [ManagedDevice](../resources/intune-devices-manageddevice.md). Mögliche Werte sind: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset` und `notRegisteredPendingEnrollment`, `unknown`.|
|deviceCategoryDisplayName|String|Gerät Kategorie Anzeigenamen Inherited aus [managedDevice](../resources/intune-devices-manageddevice.md)|
|isSupervised|Boolescher Wert|Überwacht Gerätestatus Inherited aus [managedDevice](../resources/intune-devices-manageddevice.md)|
|exchangeLastSuccessfulSyncDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Verbindung des Geräts mit Exchange Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)|
|exchangeAccessState|[deviceManagementExchangeAccessState](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|Zugriffsstatus des Geräts in Exchange. Geerbt von [ManagedDevice](../resources/intune-devices-manageddevice.md). Mögliche Werte sind: `none`, `unknown`, `allowed`, `blocked` und `quarantined`.|
|exchangeAccessStateReason|[deviceManagementExchangeAccessStateReason](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|Grund für den Zugriffsstatus des Geräts in Exchange. Geerbt von [ManagedDevice](../resources/intune-devices-manageddevice.md). Mögliche Werte sind: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword` und `deviceNotKnownWithManagedApp`.|
|remoteAssistanceSessionUrl|String|URL zur Einrichtung einer Remoteunterstützungssitzung mit dem Gerät.
 Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)|
|remoteAssistanceSessionErrorDetails|String|Fehlerzeichenfolge zur Beschreibung von Fehlern beim Erstellen von Objekten für Remoteunterstützungssitzungen.
 Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)|
|isEncrypted|Boolescher Wert|Verschlüsselung Gerätestatus Inherited aus [managedDevice](../resources/intune-devices-manageddevice.md)|
|userPrincipalName|String|Gerät Benutzerprinzipalnamen Inherited aus [managedDevice](../resources/intune-devices-manageddevice.md)|
|model|String|Modell des Geräts Inherited aus [managedDevice](../resources/intune-devices-manageddevice.md)|
|manufacturer|String|Hersteller des Geräts Inherited aus [managedDevice](../resources/intune-devices-manageddevice.md)|
|imei|String|IMEI von [ManagedDevice](../resources/intune-devices-manageddevice.md) geerbt|
|complianceGracePeriodExpirationDateTime|DateTimeOffset|Die DateTime beim Gerät Compliance Inherited aus [ManagedDevice](../resources/intune-devices-manageddevice.md) Aktivierungszeitraums|
|serialNumber|String|SerialNumber von [ManagedDevice](../resources/intune-devices-manageddevice.md) geerbt|
|PhoneNumber|String|Rufnummer des Geräts Inherited aus [managedDevice](../resources/intune-devices-manageddevice.md)|
|androidSecurityPatchLevel|String|Android Patch Sicherheitsstufe Inherited von [managedDevice](../resources/intune-devices-manageddevice.md)|
|userDisplayName|String|Anzeigename des Benutzers Inherited aus [managedDevice](../resources/intune-devices-manageddevice.md)|
|configurationManagerClientEnabledFeatures|[configurationManagerClientEnabledFeatures](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|ConfigrMgr-Client aktiviert Inherited-Funktionen, [managedDevice](../resources/intune-devices-manageddevice.md)|
|wiFiMacAddress|String|Wi-Fi MAC von [ManagedDevice](../resources/intune-devices-manageddevice.md) geerbt.|
|deviceHealthAttestationState|[deviceHealthAttestationState](../resources/intune-devices-devicehealthattestationstate.md)|Status des Integritätsnachweises für Geräte.
 Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)|
|subscriberCarrier|String|Abonnenten des Netzbetreibers von [ManagedDevice](../resources/intune-devices-manageddevice.md) geerbt.|
|meid|String|MEID von [ManagedDevice](../resources/intune-devices-manageddevice.md) geerbt|
|totalStorageSpaceInBytes|Int64|Gesamtspeicher in Bytes von [ManagedDevice](../resources/intune-devices-manageddevice.md) geerbt|
|freeStorageSpaceInBytes|Int64|Freien Speicher in Bytes von [ManagedDevice](../resources/intune-devices-manageddevice.md) geerbt|
|managedDeviceName|String|Automatisch generierter Name zur Identifizierung des Geräts. Kann mit einem benutzerfreundlichen Namen überschrieben werden. Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)|
|partnerReportedThreatState|[managedDevicePartnerReportedHealthState](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|Gibt den Bedrohungsstatus eines Geräts an, wenn das Konto und das Gerät einen Mobile Threat Defense-Partner nutzen. Schreibgeschützt. Geerbt von [ManagedDevice](../resources/intune-devices-manageddevice.md). Mögliche Werte: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.|
|usersLoggedOn|[LoggedOnUser](../resources/intune-devices-loggedonuser.md) -Auflistung|Gibt das letzte angemeldete Benutzer eines Geräts Inherited aus [managedDevice](../resources/intune-devices-manageddevice.md)|
|preferMdmOverGroupPolicyAppliedDateTime|DateTimeOffset|Meldet den DateTime-Wert die Einstellung PreferMdmOverGroupPolicy festgelegt wurde.  Wenn festgelegt ist, werden die Intune MDM Einstellungen Group Policy Settings außer Kraft setzen, wenn ein Konflikt vorliegt. Schreibgeschützt. Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)|
|autopilotEnrolled|Boolesch|Gibt an, ob das verwaltete Geräte über den Auto-Pilot registriert ist. Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)|
|requireUserEnrollmentApproval|Boolesch|Gibt an, ob das Gerät verwalteten iOS Benutzer Genehmigung Registrierung wird. Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)|
|managementCertificateExpirationDate|DateTimeOffset|Gerät Management Ablaufdatum des Zertifikats Inherited aus [ManagedDevice](../resources/intune-devices-manageddevice.md) -Berichte|
|iccid|String|Chip Karte Bezeichner, ist es eine SIM-Karte eindeutige ID-Nummer. Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)|
|UDID|String|Eindeutige Geräte-ID für iOS und Mac OS-Geräte. Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)|
|roleScopeTagIds|Collection von Objekten des Typs „String“|Liste der Bereichs-Tag-IDs für diese Instanz des Geräts. Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)|
|windowsActiveMalwareCount|Int32|Anzahl von aktiven Malware für dieses Windows-Gerät Inherited aus [managedDevice](../resources/intune-devices-manageddevice.md)|
|windowsRemediatedMalwareCount|Int32|Anzahl der für das Windows-Gerät Inherited aus [ManagedDevice](../resources/intune-devices-manageddevice.md) für gewartete Schadsoftware|
|notes|String|Notes auf dem Gerät von IT Admin geerbt von [ManagedDevice](../resources/intune-devices-manageddevice.md) erstellt|
|configurationManagerClientHealthState|[configurationManagerClientHealthState](../resources/intune-devices-configurationmanagerclienthealthstate.md)|Konfigurations-Manager-Client Integritätsstatus, gilt nur für Geräte, die von MDM/Configuration Manager-Agent geerbt von [ManagedDevice](../resources/intune-devices-manageddevice.md) verwaltet|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|detectedApps|[detectedApp](../resources/intune-devices-detectedapp.md)-Sammlung|Alle Programme, die derzeit auf dem Gerät installiert Inherited aus [managedDevice](../resources/intune-devices-manageddevice.md)|
|deviceCategory|[deviceCategory](../resources/intune-shared-devicecategory.md)|Gerätekategorie Inherited aus [managedDevice](../resources/intune-devices-manageddevice.md)|
|windowsProtectionState|[windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md)|Das Gerät Sicherheitsstatus. Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsManagedDevice"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsManagedDevice",
  "id": "String (identifier)",
  "userId": "String",
  "deviceName": "String",
  "hardwareInformation": {
    "@odata.type": "microsoft.graph.hardwareInformation",
    "serialNumber": "String",
    "totalStorageSpace": 1024,
    "freeStorageSpace": 1024,
    "imei": "String",
    "meid": "String",
    "manufacturer": "String",
    "model": "String",
    "phoneNumber": "String",
    "subscriberCarrier": "String",
    "cellularTechnology": "String",
    "wifiMac": "String",
    "operatingSystemLanguage": "String",
    "isSupervised": true,
    "isEncrypted": true,
    "isSharedDevice": true,
    "sharedDeviceCachedUsers": [
      {
        "@odata.type": "microsoft.graph.sharedAppleDeviceUser",
        "userPrincipalName": "String",
        "dataToSync": true,
        "dataQuota": 1024,
        "dataUsed": 1024
      }
    ],
    "tpmSpecificationVersion": "String",
    "operatingSystemEdition": "String",
    "deviceFullQualifiedDomainName": "String",
    "deviceGuardVirtualizationBasedSecurityHardwareRequirementState": "String",
    "deviceGuardVirtualizationBasedSecurityState": "String",
    "deviceGuardLocalSystemAuthorityCredentialGuardState": "String"
  },
  "ownerType": "String",
  "managedDeviceOwnerType": "String",
  "deviceActionResults": [
    {
      "@odata.type": "microsoft.graph.deviceActionResult",
      "actionName": "String",
      "actionState": "String",
      "startDateTime": "String (timestamp)",
      "lastUpdatedDateTime": "String (timestamp)"
    }
  ],
  "managementState": "String",
  "enrolledDateTime": "String (timestamp)",
  "lastSyncDateTime": "String (timestamp)",
  "chassisType": "String",
  "operatingSystem": "String",
  "deviceType": "String",
  "complianceState": "String",
  "jailBroken": "String",
  "managementAgent": "String",
  "osVersion": "String",
  "easActivated": true,
  "easDeviceId": "String",
  "easActivationDateTime": "String (timestamp)",
  "aadRegistered": true,
  "azureADRegistered": true,
  "deviceEnrollmentType": "String",
  "lostModeState": "String",
  "activationLockBypassCode": "String",
  "emailAddress": "String",
  "azureActiveDirectoryDeviceId": "String",
  "azureADDeviceId": "String",
  "deviceRegistrationState": "String",
  "deviceCategoryDisplayName": "String",
  "isSupervised": true,
  "exchangeLastSuccessfulSyncDateTime": "String (timestamp)",
  "exchangeAccessState": "String",
  "exchangeAccessStateReason": "String",
  "remoteAssistanceSessionUrl": "String",
  "remoteAssistanceSessionErrorDetails": "String",
  "isEncrypted": true,
  "userPrincipalName": "String",
  "model": "String",
  "manufacturer": "String",
  "imei": "String",
  "complianceGracePeriodExpirationDateTime": "String (timestamp)",
  "serialNumber": "String",
  "phoneNumber": "String",
  "androidSecurityPatchLevel": "String",
  "userDisplayName": "String",
  "configurationManagerClientEnabledFeatures": {
    "@odata.type": "microsoft.graph.configurationManagerClientEnabledFeatures",
    "inventory": true,
    "modernApps": true,
    "resourceAccess": true,
    "deviceConfiguration": true,
    "compliancePolicy": true,
    "windowsUpdateForBusiness": true
  },
  "wiFiMacAddress": "String",
  "deviceHealthAttestationState": {
    "@odata.type": "microsoft.graph.deviceHealthAttestationState",
    "lastUpdateDateTime": "String",
    "contentNamespaceUrl": "String",
    "deviceHealthAttestationStatus": "String",
    "contentVersion": "String",
    "issuedDateTime": "String (timestamp)",
    "attestationIdentityKey": "String",
    "resetCount": 1024,
    "restartCount": 1024,
    "dataExcutionPolicy": "String",
    "bitLockerStatus": "String",
    "bootManagerVersion": "String",
    "codeIntegrityCheckVersion": "String",
    "secureBoot": "String",
    "bootDebugging": "String",
    "operatingSystemKernelDebugging": "String",
    "codeIntegrity": "String",
    "testSigning": "String",
    "safeMode": "String",
    "windowsPE": "String",
    "earlyLaunchAntiMalwareDriverProtection": "String",
    "virtualSecureMode": "String",
    "pcrHashAlgorithm": "String",
    "bootAppSecurityVersion": "String",
    "bootManagerSecurityVersion": "String",
    "tpmVersion": "String",
    "pcr0": "String",
    "secureBootConfigurationPolicyFingerPrint": "String",
    "codeIntegrityPolicy": "String",
    "bootRevisionListInfo": "String",
    "operatingSystemRevListInfo": "String",
    "healthStatusMismatchInfo": "String",
    "healthAttestationSupportedStatus": "String"
  },
  "subscriberCarrier": "String",
  "meid": "String",
  "totalStorageSpaceInBytes": 1024,
  "freeStorageSpaceInBytes": 1024,
  "managedDeviceName": "String",
  "partnerReportedThreatState": "String",
  "usersLoggedOn": [
    {
      "@odata.type": "microsoft.graph.loggedOnUser",
      "userId": "String",
      "lastLogOnDateTime": "String (timestamp)"
    }
  ],
  "preferMdmOverGroupPolicyAppliedDateTime": "String (timestamp)",
  "autopilotEnrolled": true,
  "requireUserEnrollmentApproval": true,
  "managementCertificateExpirationDate": "String (timestamp)",
  "iccid": "String",
  "udid": "String",
  "roleScopeTagIds": [
    "String"
  ],
  "windowsActiveMalwareCount": 1024,
  "windowsRemediatedMalwareCount": 1024,
  "notes": "String",
  "configurationManagerClientHealthState": {
    "@odata.type": "microsoft.graph.configurationManagerClientHealthState",
    "state": "String",
    "errorCode": 1024,
    "lastSyncDateTime": "String (timestamp)"
  }
}
```





