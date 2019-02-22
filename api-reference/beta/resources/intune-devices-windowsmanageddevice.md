---
title: windowsManagedDevice-Ressourcentyp
description: Windows-Geräte, die über InTune verwaltet oder vorab registriert werden
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f0e5811df6bfcdb360b5f8f3b03822a38bdbaab4
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30161229"
---
# <a name="windowsmanageddevice-resource-type"></a>windowsManagedDevice-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Windows-Geräte, die über InTune verwaltet oder vorab registriert werden


Erbt von [managedDevice](../resources/intune-devices-manageddevice.md)

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[WindowsManagedDevices aufListen](../api/intune-devices-windowsmanageddevice-list.md)|[windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) -Sammlung|AufListen von Eigenschaften und Beziehungen der [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) -Objekte.|
|[WindowsManagedDevice abrufen](../api/intune-devices-windowsmanageddevice-get.md)|[windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md)|Lesen von Eigenschaften und Beziehungen des [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) -Objekts.|
|[WindowsManagedDevice erstellen](../api/intune-devices-windowsmanageddevice-create.md)|[windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md)|Erstellen eines neuen [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) -Objekts.|
|[WindowsManagedDevice löschen](../api/intune-devices-windowsmanageddevice-delete.md)|Keine|Löscht eine [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md).|
|[WindowsManagedDevice aktualisieren](../api/intune-devices-windowsmanageddevice-update.md)|[windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md)|Aktualisieren der Eigenschaften eines [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|string|Eindeutiger Bezeichner für das von [ManagedDevice](../resources/intune-devices-manageddevice.md) geerbte Gerät|
|userId|String|Eindeutiger Bezeichner für den Benutzer, der mit dem von [ManagedDevice](../resources/intune-devices-manageddevice.md) geerbten Gerät verknüpft ist|
|deviceName|Zeichenfolge|Name des von [ManagedDevice](../resources/intune-devices-manageddevice.md) geerbten Geräts|
|Dem|[Dem](../resources/intune-devices-hardwareinformation.md)|Die hardward-Details für das Gerät.  Enthält Informationen wie Speicherplatz, Hersteller, Seriennummer usw. Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)|
|ownerType|[ownerType](../resources/intune-devices-ownertype.md)|Der Besitzer des Geräts. Kann "Company" oder "Personal" von [ManagedDevice](../resources/intune-devices-manageddevice.md)geerbt werden. Mögliche Werte sind: `unknown`, `company` und `personal`.|
|managedDeviceOwnerType|[managedDeviceOwnerType](../resources/intune-devices-manageddeviceownertype.md)|Der Besitzer des Geräts. Kann "Company" oder "Personal" von [ManagedDevice](../resources/intune-devices-manageddevice.md)geerbt werden. Mögliche Werte sind: `unknown`, `company` und `personal`.|
|deviceActionResults|Collection von Objekten des Typs [deviceActionResult](../resources/intune-devices-deviceactionresult.md)|Liste von Objekten des Typs „ComplexType deviceActionResult“.
 Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)|
|managementState|[managementState](../resources/intune-devices-managementstate.md)|Verwaltungsstatus des Geräts. Von [ManagedDevice](../resources/intune-devices-manageddevice.md)geerbt. Mögliche Werte sind: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled` und `discovered`.|
|enrolledDateTime|DateTimeOffset|Datum und Uhrzeit der Geräteregistrierung.
 Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)|
|lastSyncDateTime|DateTimeOffset|Datum und Uhrzeit der letzten erfolgreichen Synchronisierung des Geräts mit Intune.
 Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)|
|chassitype|[chassitype](../resources/intune-devices-chassistype.md)|Gehäusetyp des Geräts. Von [ManagedDevice](../resources/intune-devices-manageddevice.md)geerbt. Mögliche Werte: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.|
|operatingSystem|Zeichenfolge|Betriebssystem des Geräts. Windows, iOS, etc. Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)|
|deviceType|[deviceType](../resources/intune-shared-devicetype.md)|Plattform des Geräts. Von [ManagedDevice](../resources/intune-devices-manageddevice.md)geerbt. Mögliche Werte sind: `desktop`, `windowsRT`, `winMO6` `nokia` `windowsPhone` `mac` `winCE` `iPhone` `iPad` `iPod` `android` `iSocConsumer` `unix` `macMDM`,,,,,,,, `holoLens`,, `androidEnterprise` ,,,,,, `surfaceHub` `androidForWork` `winEmbedded` , `blackberry`, `palm`, `unknown`.|
|complianceState|[complianceState](../resources/intune-devices-compliancestate.md)|Konformitätsstatus des Geräts. Von [ManagedDevice](../resources/intune-devices-manageddevice.md)geerbt. Mögliche Werte sind: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod` und `configManager`.|
|jailBroken|String|Gibt an, ob es sich um ein Gerät mit Jailbreak oder Rootzugriff handelt. Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)|
|managementAgent|[managementAgentType](../resources/intune-devices-managementagenttype.md)|Verwaltungskanal des Geräts. InTune, EAS usw. Von [ManagedDevice](../resources/intune-devices-manageddevice.md)geerbt. Mögliche Werte sind: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController` und `microsoft365ManagedMdm`.|
|osVersion|Zeichenfolge|Auf dem Gerät installierte Betriebssystemversion.
 Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)|
|easActivated|Boolean|Gibt an, ob für das Gerät Exchange ActiveSync aktiviert ist. Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)|
|easDeviceId|Zeichenfolge|Exchange ActiveSync-ID des Geräts.
 Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)|
|easActivationDateTime|DateTimeOffset|Datum und Uhrzeit der Exchange ActiveSync-Aktivierung für das Gerät.
 Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)|
|aadRegistered|Boolescher Wert|Gibt an, ob das Gerät in Azure Active Directory registriert ist. Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)|
|azureADRegistered|Boolescher Wert|Gibt an, ob das Gerät in Azure Active Directory registriert ist. Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)|
|deviceEnrollmentType|[deviceEnrollmentType](../resources/intune-shared-deviceenrollmenttype.md)|Registrierungstyp des Geräts. Von [ManagedDevice](../resources/intune-devices-manageddevice.md)geerbt. Mögliche Werte: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.|
|lostModeState|[lostModeState](../resources/intune-devices-lostmodestate.md)|Gibt an, ob der Modus verloren aktiviert oder deaktiviert von [ManagedDevice](../resources/intune-devices-manageddevice.md)geerbt wurde. Mögliche Werte sind: `disabled` und `enabled`.|
|activationLockBypassCode|Zeichenfolge|Code, der die Umgehung der Aktivierungssperre des Geräts ermöglicht Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)|
|emailAddress|Zeichenfolge|E-Mail (e) für den Benutzer, der mit dem von [ManagedDevice](../resources/intune-devices-manageddevice.md) geerbten Gerät verknüpft ist|
|Eigenschaften azureactivedirectorydeviceid|Zeichenfolge|Eindeutiger Bezeichner des Azure Active Directory-Geräts. Schreibgeschützt. Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)|
|azureADDeviceId|Zeichenfolge|Eindeutiger Bezeichner des Azure Active Directory-Geräts. Schreibgeschützt. Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)|
|deviceRegistrationState|[deviceRegistrationState](../resources/intune-devices-deviceregistrationstate.md)|Registrierungsstatus des Geräts. Von [ManagedDevice](../resources/intune-devices-manageddevice.md)geerbt. Mögliche Werte sind: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset` und `notRegisteredPendingEnrollment`, `unknown`.|
|deviceCategoryDisplayName|Zeichenfolge|Anzeigename der Gerätekategorie, geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)|
|isSupervised|Boolean|Von [ManagedDevice](../resources/intune-devices-manageddevice.md) geerbter Geräte überwachter Status|
|exchangeLastSuccessfulSyncDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Verbindung des Geräts mit Exchange Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)|
|exchangeAccessState|[deviceManagementExchangeAccessState](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|Zugriffsstatus des Geräts in Exchange. Von [ManagedDevice](../resources/intune-devices-manageddevice.md)geerbt. Mögliche Werte: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.|
|exchangeAccessStateReason|[deviceManagementExchangeAccessStateReason](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|Grund für den Zugriffsstatus des Geräts in Exchange. Von [ManagedDevice](../resources/intune-devices-manageddevice.md)geerbt. Mögliche Werte sind: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword` und `deviceNotKnownWithManagedApp`.|
|remoteAssistanceSessionUrl|Zeichenfolge|URL zur Einrichtung einer Remoteunterstützungssitzung mit dem Gerät.
 Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)|
|remoteAssistanceSessionErrorDetails|Zeichenfolge|Fehlerzeichenfolge zur Beschreibung von Fehlern beim Erstellen von Objekten für Remoteunterstützungssitzungen.
 Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)|
|isEncrypted|Boolescher Wert|Von [ManagedDevice](../resources/intune-devices-manageddevice.md) geerbter Geräte Verschlüsselungsstatus|
|userPrincipalName|Zeichenfolge|Von [ManagedDevice](../resources/intune-devices-manageddevice.md) geerbter Geräte Benutzerprinzipalname|
|model|Zeichenfolge|Modell des von [ManagedDevice](../resources/intune-devices-manageddevice.md) geerbten Geräts|
|manufacturer|Zeichenfolge|Hersteller des von [ManagedDevice](../resources/intune-devices-manageddevice.md) geerbten Geräts|
|imei|String|IMEI geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)|
|complianceGracePeriodExpirationDateTime|DateTimeOffset|Das Datum, an dem die Zeitdauer für die Geräte Konformität von [ManagedDevice](../resources/intune-devices-manageddevice.md) geerbt wurde|
|serialNumber|String|Von [ManagedDevice](../resources/intune-devices-manageddevice.md) geerbte Seriennummer|
|PhoneNumber|Zeichenfolge|Telefonnummer des von [ManagedDevice](../resources/intune-devices-manageddevice.md) geerbten Geräts|
|androidSecurityPatchLevel|Zeichenfolge|Von [ManagedDevice](../resources/intune-devices-manageddevice.md) geerbte Sicherheitspatch-Stufe von Android|
|userDisplayName|Zeichenfolge|Von [ManagedDevice](../resources/intune-devices-manageddevice.md) geerbter Benutzeranzeigename|
|configurationManagerClientEnabledFeatures|[configurationManagerClientEnabledFeatures](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|Von [ManagedDevice](../resources/intune-devices-manageddevice.md) geerbte aktivierte-Client aktivierte Features|
|wiFiMacAddress|Zeichenfolge|Von [ManagedDevice](../resources/intune-devices-manageddevice.md) geerbter Wi-Fi-Mac|
|deviceHealthAttestationState|[deviceHealthAttestationState](../resources/intune-devices-devicehealthattestationstate.md)|Status des Integritätsnachweises für Geräte.
 Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)|
|subscriberCarrier|Zeichenfolge|Von [ManagedDevice](../resources/intune-devices-manageddevice.md) geerbter Abonnent|
|meid|Zeichenfolge|Von [ManagedDevice](../resources/intune-devices-manageddevice.md) GEERBTe MEID|
|totalStorageSpaceInBytes|Int64|Gesamtspeicher in Byte, geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)|
|freeStorageSpaceInBytes|Int64|Freier Speicher in von [ManagedDevice](../resources/intune-devices-manageddevice.md) geerbten bytes|
|managedDeviceName|String|Automatisch generierter Name zur Identifizierung des Geräts. Kann mit einem benutzerfreundlichen Namen überschrieben werden. Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)|
|partnerReportedThreatState|[managedDevicePartnerReportedHealthState](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|Gibt den Bedrohungsstatus eines Geräts an, wenn das Konto und das Gerät einen Mobile Threat Defense-Partner nutzen. Schreibgeschützt. Von [ManagedDevice](../resources/intune-devices-manageddevice.md)geerbt. Mögliche Werte: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.|
|usersLoggedOn|[loggedOnUser](../resources/intune-devices-loggedonuser.md) -Sammlung|Gibt die zuletzt angemeldeten Benutzer eines von [ManagedDevice](../resources/intune-devices-manageddevice.md) geerbten Geräts an.|
|preferMdmOverGroupPolicyAppliedDateTime|DateTimeOffset|Meldet den DateTime-Wert für die Einstellung preferMdmOverGroupPolicy.  Ist diese Einstellung festgelegt, überschreiben die Intune-MDM-Einstellungen Gruppenrichtlinieneinstellungen bei einem Konflikt. Schreibgeschützt. Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)|
|autopilotEnrolled|Boolescher Wert|Meldet, ob das verwaltete Gerät über Auto-Pilot registriert wird. Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)|
|requireUserEnrollmentApproval|Boolescher Wert|Meldet, ob das verwaltete iOS-Gerät Benutzer Genehmigungs Registrierung ist. Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)|
|managementCertificateExpirationDate|DateTimeOffset|Meldet Ablaufdatum für das Geräte Verwaltungszertifikat, das von [ManagedDevice](../resources/intune-devices-manageddevice.md) geerbt wurde|
|ICCID|Zeichenfolge|Integrated Circuit Card Identifier, es ist die eindeutige Identifikationsnummer einer SIM-Karte. Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)|
|UDID|Zeichenfolge|Eindeutige Gerätekennung für iOS-und macOS-Geräte. Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)|
|Rolescopetagids zur|String collection|Liste der Bereichstag-IDs für diese Geräteinstanz. Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)|
|windowsActiveMalwareCount|Int32|Anzahl der aktiven Schadsoftware für dieses Windows-Gerät, geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)|
|windowsRemediatedMalwareCount|Int32|Anzahl der korrigierten Schadsoftware für dieses Windows-Gerät, geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)|
|notes|Zeichenfolge|Hinweise auf dem vom IT-Administrator erstellten Gerät werden von [ManagedDevice](../resources/intune-devices-manageddevice.md) geerbt.|
|configurationManagerClientHealthState|[configurationManagerClientHealthState](../resources/intune-devices-configurationmanagerclienthealthstate.md)|Configuration Manager-Clientintegritätsstatus, nur gültig für Geräte, die von [ManagedDevice](../resources/intune-devices-manageddevice.md) geerbten MDM/ConfigMgr-Agent verwaltet werden|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|detectedApps|[detectedApp](../resources/intune-devices-detectedapp.md)-Sammlung|Alle derzeit auf dem Gerät installierten Anwendungen, die von [ManagedDevice](../resources/intune-devices-manageddevice.md) geerbt wurden|
|deviceCategory|[deviceCategory](../resources/intune-shared-devicecategory.md)|Von [ManagedDevice](../resources/intune-devices-manageddevice.md) geerbte Gerätekategorie|
|windowsProtectionState|[windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md)|Der Status des Geräteschutzes. Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)|

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
    "windowsUpdateForBusiness": true,
    "endpointProtection": true,
    "officeApps": true
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




