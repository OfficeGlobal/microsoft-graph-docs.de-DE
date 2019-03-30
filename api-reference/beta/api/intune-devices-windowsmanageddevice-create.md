---
title: WindowsManagedDevice erstellen
description: Erstellen eines neuen windowsManagedDevice-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 51c8f4281a65ac73f5db00e59a3df12a69967ec5
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30987118"
---
# <a name="create-windowsmanageddevice"></a>WindowsManagedDevice erstellen

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Erstellen eines neuen [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) -Objekts.

## <a name="prerequisites"></a>Voraussetzungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp|Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)|
|:---|:---|
|Delegiert (Geschäfts-, Schul- oder Unikonto)|DeviceManagementManagedDevices.ReadWrite.All|
|Delegiert (persönliches Microsoft-Konto)|Nicht unterstützt|
|Anwendung|Nicht unterstützt|

## <a name="http-request"></a>HTTP-Anforderung
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices
POST /deviceManagement/managedDevices
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices
```

## <a name="request-headers"></a>Anforderungsheader
|Kopfzeile|Wert|
|:---|:---|
|Authorization|Bearer&lt;token&gt; erforderlich|
|Annehmen|application/json|

## <a name="request-body"></a>Anforderungstext
Geben Sie im Anforderungstext eine JSON-Darstellung für das windowsManagedDevice-Objekt an.

In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der windowsManagedDevice erforderlich sind.

|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Eindeutiger Bezeichner für das von [ManagedDevice](../resources/intune-devices-manageddevice.md) geerbte Gerät|
|userId|String|Eindeutiger Bezeichner für den Benutzer, der mit dem von [ManagedDevice](../resources/intune-devices-manageddevice.md) geerbten Gerät verknüpft ist|
|deviceName|String|Name des von [ManagedDevice](../resources/intune-devices-manageddevice.md) geerbten Geräts|
|Dem|[Dem](../resources/intune-devices-hardwareinformation.md)|Die hardward-Details für das Gerät.  Enthält Informationen wie Speicherplatz, Hersteller, Seriennummer usw. Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)|
|ownerType|[ownerType](../resources/intune-devices-ownertype.md)|Der Besitzer des Geräts. Kann "Company" oder "Personal" von [ManagedDevice](../resources/intune-devices-manageddevice.md)geerbt werden. Mögliche Werte sind: `unknown`, `company` und `personal`.|
|managedDeviceOwnerType|[managedDeviceOwnerType](../resources/intune-devices-manageddeviceownertype.md)|Der Besitzer des Geräts. Kann "Company" oder "Personal" von [ManagedDevice](../resources/intune-devices-manageddevice.md)geerbt werden. Mögliche Werte sind: `unknown`, `company` und `personal`.|
|deviceActionResults|[deviceActionResult](../resources/intune-devices-deviceactionresult.md)-Sammlung|Liste von ComplexType DeviceActionResult-Objekten. Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)|
|managementState|[managementState](../resources/intune-devices-managementstate.md)|Verwaltungsstatus des Geräts. Von [ManagedDevice](../resources/intune-devices-manageddevice.md)geerbt. Mögliche Werte sind: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled` und `discovered`.|
|enrolledDateTime|DateTimeOffset|Registrierungszeit des Geräts. Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)|
|lastSyncDateTime|DateTimeOffset|Datum und Uhrzeit, zu dem bzw. der das Gerät zuletzt eine erfolgreiche Synchronisierung mit Intune durchgeführt hat. Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)|
|chassitype|[chassitype](../resources/intune-devices-chassistype.md)|Gehäusetyp des Geräts. Von [ManagedDevice](../resources/intune-devices-manageddevice.md)geerbt. Mögliche Werte: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.|
|operatingSystem|String|Betriebssystem des Geräts Windows, iOS, etc. Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)|
|deviceType|[deviceType](../resources/intune-shared-devicetype.md)|Plattform des Geräts. Von [ManagedDevice](../resources/intune-devices-manageddevice.md)geerbt. Mögliche Werte sind: `desktop`, `windowsRT`, `winMO6` `nokia` `windowsPhone` `mac` `winCE` `iPhone` `iPad` `iPod` `android` `iSocConsumer` `unix` `macMDM`,,,,,,,, `holoLens`,, `androidEnterprise` ,,,,,, `surfaceHub` `androidForWork` `winEmbedded` , `blackberry`, `palm`, `unknown`.|
|complianceState|[complianceState](../resources/intune-devices-compliancestate.md)|Compliancestatus des Geräts. Von [ManagedDevice](../resources/intune-devices-manageddevice.md)geerbt. Mögliche Werte: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.|
|jailBroken|String|Gibt an, ob es sich um ein Gerät mit Jailbreak oder Rootzugriff handelt. Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)|
|managementAgent|[managementAgentType](../resources/intune-devices-managementagenttype.md)|Verwaltungskanal des Geräts. InTune, EAS usw. Von [ManagedDevice](../resources/intune-devices-manageddevice.md)geerbt. Mögliche Werte sind: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController` und `microsoft365ManagedMdm`.|
|osVersion|String|Betriebssystemversion auf dem Gerät. Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)|
|easActivated|Boolescher Wert|Gibt an, ob das Gerät über Exchange ActiveSync-aktiviert ist. Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)|
|easDeviceId|String|Exchange ActiveSync-ID des Geräts. Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)|
|easActivationDateTime|DateTimeOffset|Exchange ActivationSync-Aktivierungszeit des Geräts. Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)|
|aadRegistered|Boolean|Gibt an, ob das Gerät für Azure Active Directory registriert ist. Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)|
|azureADRegistered|Boolescher Wert|Gibt an, ob das Gerät für Azure Active Directory registriert ist. Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)|
|deviceEnrollmentType|[deviceEnrollmentType](../resources/intune-shared-deviceenrollmenttype.md)|Registrierungstyp des Geräts. Von [ManagedDevice](../resources/intune-devices-manageddevice.md)geerbt. Mögliche Werte: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.|
|lostModeState|[lostModeState](../resources/intune-devices-lostmodestate.md)|Gibt an, ob der Modus verloren aktiviert oder deaktiviert von [ManagedDevice](../resources/intune-devices-manageddevice.md)geerbt wurde. Mögliche Werte sind: `disabled` und `enabled`.|
|activationLockBypassCode|String|Code, der ermöglicht, dass die Aktivierungssperre auf einem Gerät umgangen wird. Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)|
|emailAddress|String|E-Mail (e) für den Benutzer, der mit dem von [ManagedDevice](../resources/intune-devices-manageddevice.md) geerbten Gerät verknüpft ist|
|Eigenschaften azureactivedirectorydeviceid|String|Die eindeutige ID für das Azure Active Directory-Gerät. Schreibgeschützt. Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)|
|azureADDeviceId|String|Die eindeutige ID für das Azure Active Directory-Gerät. Schreibgeschützt. Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)|
|deviceRegistrationState|[deviceRegistrationState](../resources/intune-devices-deviceregistrationstate.md)|Geräteregistrierungsstatus Von [ManagedDevice](../resources/intune-devices-manageddevice.md)geerbt. Mögliche Werte: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.|
|deviceCategoryDisplayName|String|Anzeigename der Gerätekategorie, geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)|
|isSupervised|Boolescher Wert|Von [ManagedDevice](../resources/intune-devices-manageddevice.md) geerbter Geräte überwachter Status|
|exchangeLastSuccessfulSyncDateTime|DateTimeOffset|Letzter Zeitpunkt, zu dem das Gerät Exchange kontaktiert hat. Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)|
|exchangeAccessState|[deviceManagementExchangeAccessState](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|Der Zugriffsstatus des Geräts in Exchange. Von [ManagedDevice](../resources/intune-devices-manageddevice.md)geerbt. Mögliche Werte: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.|
|exchangeAccessStateReason|[deviceManagementExchangeAccessStateReason](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|Grund für den Zugriffsstatus des Geräts in Exchange. Von [ManagedDevice](../resources/intune-devices-manageddevice.md)geerbt. Mögliche Werte sind: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.|
|remoteAssistanceSessionUrl|String|Die URL, die ermöglicht, dass mit dem Gerät eine Remoteunterstützungssitzung eingerichtet wird. Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)|
|remoteAssistanceSessionErrorDetails|String|Eine Fehlerzeichenfolge, die Probleme beim Erstellen von Objekten für die Remoteunterstützungssitzung identifiziert. Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)|
|isEncrypted|Boolean|Von [ManagedDevice](../resources/intune-devices-manageddevice.md) geerbter Geräte Verschlüsselungsstatus|
|userPrincipalName|String|Von [ManagedDevice](../resources/intune-devices-manageddevice.md) geerbter Geräte Benutzerprinzipalname|
|model|String|Modell des von [ManagedDevice](../resources/intune-devices-manageddevice.md) geerbten Geräts|
|Hersteller|String|Hersteller des von [ManagedDevice](../resources/intune-devices-manageddevice.md) geerbten Geräts|
|imei|String|IMEI geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)|
|complianceGracePeriodExpirationDateTime|DateTimeOffset|Das Datum, an dem die Zeitdauer für die Geräte Konformität von [ManagedDevice](../resources/intune-devices-manageddevice.md) geerbt wurde|
|serialNumber|String|Von [ManagedDevice](../resources/intune-devices-manageddevice.md) geerbte Seriennummer|
|PhoneNumber|String|Telefonnummer des von [ManagedDevice](../resources/intune-devices-manageddevice.md) geerbten Geräts|
|androidSecurityPatchLevel|String|Von [ManagedDevice](../resources/intune-devices-manageddevice.md) geerbte Sicherheitspatch-Stufe von Android|
|userDisplayName|String|Von [ManagedDevice](../resources/intune-devices-manageddevice.md) geerbter Benutzeranzeigename|
|configurationManagerClientEnabledFeatures|[configurationManagerClientEnabledFeatures](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|Von [ManagedDevice](../resources/intune-devices-manageddevice.md) geerbte aktivierte-Client aktivierte Features|
|wiFiMacAddress|String|Von [ManagedDevice](../resources/intune-devices-manageddevice.md) geerbter Wi-Fi-Mac|
|deviceHealthAttestationState|[deviceHealthAttestationState](../resources/intune-devices-devicehealthattestationstate.md)|Integritätsnachweis für Geräte – Status Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)|
|subscriberCarrier|String|Von [ManagedDevice](../resources/intune-devices-manageddevice.md) geerbter Abonnent|
|meid|String|Von [ManagedDevice](../resources/intune-devices-manageddevice.md) GEERBTe MEID|
|totalStorageSpaceInBytes|Int64|Gesamtspeicher in Byte, geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)|
|freeStorageSpaceInBytes|Int64|Freier Speicher in von [ManagedDevice](../resources/intune-devices-manageddevice.md) geerbten bytes|
|managedDeviceName|String|Automatisch generierter Name zum Identifizieren eines Geräts. Kann mit einem Anzeigenamen überschrieben werden. Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)|
|partnerReportedThreatState|[managedDevicePartnerReportedHealthState](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|Gibt den Bedrohungsstatus eines Geräts an, wenn ein vom Konto und Gerät ein Mobile Threat Defense-Partner verwendet wird. Schreibgeschützt. Von [ManagedDevice](../resources/intune-devices-manageddevice.md)geerbt. Mögliche Werte: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.|
|usersLoggedOn|[loggedOnUser](../resources/intune-devices-loggedonuser.md) -Sammlung|Gibt die zuletzt angemeldeten Benutzer eines von [ManagedDevice](../resources/intune-devices-manageddevice.md) geerbten Geräts an.|
|preferMdmOverGroupPolicyAppliedDateTime|DateTimeOffset|Meldet den DateTime-Wert für die Einstellung preferMdmOverGroupPolicy.  Ist diese Einstellung festgelegt, überschreiben die Intune-MDM-Einstellungen Gruppenrichtlinieneinstellungen bei einem Konflikt. Schreibgeschützt. Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)|
|autopilotEnrolled|Boolescher Wert|Meldet, ob das verwaltete Gerät über Auto-Pilot registriert wird. Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)|
|requireUserEnrollmentApproval|Boolescher Wert|Meldet, ob das verwaltete iOS-Gerät Benutzer Genehmigungs Registrierung ist. Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)|
|managementCertificateExpirationDate|DateTimeOffset|Meldet Ablaufdatum für das Geräte Verwaltungszertifikat, das von [ManagedDevice](../resources/intune-devices-manageddevice.md) geerbt wurde|
|ICCID|String|Integrated Circuit Card Identifier, es ist die eindeutige Identifikationsnummer einer SIM-Karte. Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)|
|UDID|String|Eindeutige Gerätekennung für iOS-und macOS-Geräte. Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)|
|Rolescopetagids zur|String collection|Liste der Bereichstag-IDs für diese Geräteinstanz. Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)|
|windowsActiveMalwareCount|Int32|Anzahl der aktiven Schadsoftware für dieses Windows-Gerät, geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)|
|windowsRemediatedMalwareCount|Int32|Anzahl der korrigierten Schadsoftware für dieses Windows-Gerät, geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)|
|notes|String|Hinweise auf dem vom IT-Administrator erstellten Gerät werden von [ManagedDevice](../resources/intune-devices-manageddevice.md) geerbt.|
|configurationManagerClientHealthState|[configurationManagerClientHealthState](../resources/intune-devices-configurationmanagerclienthealthstate.md)|Configuration Manager-Clientintegritätsstatus, nur gültig für Geräte, die von [ManagedDevice](../resources/intune-devices-manageddevice.md) geerbten MDM/ConfigMgr-Agent verwaltet werden|



## <a name="response"></a>Antwort
Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) -Objekt im Antworttext zurück.

## <a name="example"></a>Beispiel

### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
``` http
POST https://graph.microsoft.com/beta/users/{usersId}/managedDevices
Content-type: application/json
Content-length: 7231

{
  "@odata.type": "#microsoft.graph.windowsManagedDevice",
  "userId": "User Id value",
  "deviceName": "Device Name value",
  "hardwareInformation": {
    "@odata.type": "microsoft.graph.hardwareInformation",
    "serialNumber": "Serial Number value",
    "totalStorageSpace": 1,
    "freeStorageSpace": 0,
    "imei": "Imei value",
    "meid": "Meid value",
    "manufacturer": "Manufacturer value",
    "model": "Model value",
    "phoneNumber": "Phone Number value",
    "subscriberCarrier": "Subscriber Carrier value",
    "cellularTechnology": "Cellular Technology value",
    "wifiMac": "Wifi Mac value",
    "operatingSystemLanguage": "Operating System Language value",
    "isSupervised": true,
    "isEncrypted": true,
    "isSharedDevice": true,
    "sharedDeviceCachedUsers": [
      {
        "@odata.type": "microsoft.graph.sharedAppleDeviceUser",
        "userPrincipalName": "User Principal Name value",
        "dataToSync": true,
        "dataQuota": 9,
        "dataUsed": 8
      }
    ],
    "tpmSpecificationVersion": "Tpm Specification Version value",
    "operatingSystemEdition": "Operating System Edition value",
    "deviceFullQualifiedDomainName": "Device Full Qualified Domain Name value",
    "deviceGuardVirtualizationBasedSecurityHardwareRequirementState": "secureBootRequired",
    "deviceGuardVirtualizationBasedSecurityState": "rebootRequired",
    "deviceGuardLocalSystemAuthorityCredentialGuardState": "rebootRequired"
  },
  "ownerType": "company",
  "managedDeviceOwnerType": "company",
  "deviceActionResults": [
    {
      "@odata.type": "microsoft.graph.deviceActionResult",
      "actionName": "Action Name value",
      "actionState": "pending",
      "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
      "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
    }
  ],
  "managementState": "retirePending",
  "enrolledDateTime": "2016-12-31T23:59:43.797191-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "chassisType": "desktop",
  "operatingSystem": "Operating System value",
  "deviceType": "windowsRT",
  "complianceState": "compliant",
  "jailBroken": "Jail Broken value",
  "managementAgent": "mdm",
  "osVersion": "Os Version value",
  "easActivated": true,
  "easDeviceId": "Eas Device Id value",
  "easActivationDateTime": "2016-12-31T23:59:43.4878784-08:00",
  "aadRegistered": true,
  "azureADRegistered": true,
  "deviceEnrollmentType": "userEnrollment",
  "lostModeState": "enabled",
  "activationLockBypassCode": "Activation Lock Bypass Code value",
  "emailAddress": "Email Address value",
  "azureActiveDirectoryDeviceId": "Azure Active Directory Device Id value",
  "azureADDeviceId": "Azure ADDevice Id value",
  "deviceRegistrationState": "registered",
  "deviceCategoryDisplayName": "Device Category Display Name value",
  "isSupervised": true,
  "exchangeLastSuccessfulSyncDateTime": "2017-01-01T00:00:45.8803083-08:00",
  "exchangeAccessState": "unknown",
  "exchangeAccessStateReason": "unknown",
  "remoteAssistanceSessionUrl": "https://example.com/remoteAssistanceSessionUrl/",
  "remoteAssistanceSessionErrorDetails": "Remote Assistance Session Error Details value",
  "isEncrypted": true,
  "userPrincipalName": "User Principal Name value",
  "model": "Model value",
  "manufacturer": "Manufacturer value",
  "imei": "Imei value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "serialNumber": "Serial Number value",
  "phoneNumber": "Phone Number value",
  "androidSecurityPatchLevel": "Android Security Patch Level value",
  "userDisplayName": "User Display Name value",
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
  "wiFiMacAddress": "Wi Fi Mac Address value",
  "deviceHealthAttestationState": {
    "@odata.type": "microsoft.graph.deviceHealthAttestationState",
    "lastUpdateDateTime": "Last Update Date Time value",
    "contentNamespaceUrl": "https://example.com/contentNamespaceUrl/",
    "deviceHealthAttestationStatus": "Device Health Attestation Status value",
    "contentVersion": "Content Version value",
    "issuedDateTime": "2016-12-31T23:58:22.1231038-08:00",
    "attestationIdentityKey": "Attestation Identity Key value",
    "resetCount": 10,
    "restartCount": 12,
    "dataExcutionPolicy": "Data Excution Policy value",
    "bitLockerStatus": "Bit Locker Status value",
    "bootManagerVersion": "Boot Manager Version value",
    "codeIntegrityCheckVersion": "Code Integrity Check Version value",
    "secureBoot": "Secure Boot value",
    "bootDebugging": "Boot Debugging value",
    "operatingSystemKernelDebugging": "Operating System Kernel Debugging value",
    "codeIntegrity": "Code Integrity value",
    "testSigning": "Test Signing value",
    "safeMode": "Safe Mode value",
    "windowsPE": "Windows PE value",
    "earlyLaunchAntiMalwareDriverProtection": "Early Launch Anti Malware Driver Protection value",
    "virtualSecureMode": "Virtual Secure Mode value",
    "pcrHashAlgorithm": "Pcr Hash Algorithm value",
    "bootAppSecurityVersion": "Boot App Security Version value",
    "bootManagerSecurityVersion": "Boot Manager Security Version value",
    "tpmVersion": "Tpm Version value",
    "pcr0": "Pcr0 value",
    "secureBootConfigurationPolicyFingerPrint": "Secure Boot Configuration Policy Finger Print value",
    "codeIntegrityPolicy": "Code Integrity Policy value",
    "bootRevisionListInfo": "Boot Revision List Info value",
    "operatingSystemRevListInfo": "Operating System Rev List Info value",
    "healthStatusMismatchInfo": "Health Status Mismatch Info value",
    "healthAttestationSupportedStatus": "Health Attestation Supported Status value"
  },
  "subscriberCarrier": "Subscriber Carrier value",
  "meid": "Meid value",
  "totalStorageSpaceInBytes": 8,
  "freeStorageSpaceInBytes": 7,
  "managedDeviceName": "Managed Device Name value",
  "partnerReportedThreatState": "activated",
  "usersLoggedOn": [
    {
      "@odata.type": "microsoft.graph.loggedOnUser",
      "userId": "User Id value",
      "lastLogOnDateTime": "2016-12-31T23:58:37.4262708-08:00"
    }
  ],
  "preferMdmOverGroupPolicyAppliedDateTime": "2016-12-31T23:57:34.4649887-08:00",
  "autopilotEnrolled": true,
  "requireUserEnrollmentApproval": true,
  "managementCertificateExpirationDate": "2016-12-31T23:57:59.9789653-08:00",
  "iccid": "Iccid value",
  "udid": "Udid value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "windowsActiveMalwareCount": 9,
  "windowsRemediatedMalwareCount": 13,
  "notes": "Notes value",
  "configurationManagerClientHealthState": {
    "@odata.type": "microsoft.graph.configurationManagerClientHealthState",
    "state": "installed",
    "errorCode": 9,
    "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00"
  }
}
```

### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 7280

{
  "@odata.type": "#microsoft.graph.windowsManagedDevice",
  "id": "97842b67-2b67-9784-672b-8497672b8497",
  "userId": "User Id value",
  "deviceName": "Device Name value",
  "hardwareInformation": {
    "@odata.type": "microsoft.graph.hardwareInformation",
    "serialNumber": "Serial Number value",
    "totalStorageSpace": 1,
    "freeStorageSpace": 0,
    "imei": "Imei value",
    "meid": "Meid value",
    "manufacturer": "Manufacturer value",
    "model": "Model value",
    "phoneNumber": "Phone Number value",
    "subscriberCarrier": "Subscriber Carrier value",
    "cellularTechnology": "Cellular Technology value",
    "wifiMac": "Wifi Mac value",
    "operatingSystemLanguage": "Operating System Language value",
    "isSupervised": true,
    "isEncrypted": true,
    "isSharedDevice": true,
    "sharedDeviceCachedUsers": [
      {
        "@odata.type": "microsoft.graph.sharedAppleDeviceUser",
        "userPrincipalName": "User Principal Name value",
        "dataToSync": true,
        "dataQuota": 9,
        "dataUsed": 8
      }
    ],
    "tpmSpecificationVersion": "Tpm Specification Version value",
    "operatingSystemEdition": "Operating System Edition value",
    "deviceFullQualifiedDomainName": "Device Full Qualified Domain Name value",
    "deviceGuardVirtualizationBasedSecurityHardwareRequirementState": "secureBootRequired",
    "deviceGuardVirtualizationBasedSecurityState": "rebootRequired",
    "deviceGuardLocalSystemAuthorityCredentialGuardState": "rebootRequired"
  },
  "ownerType": "company",
  "managedDeviceOwnerType": "company",
  "deviceActionResults": [
    {
      "@odata.type": "microsoft.graph.deviceActionResult",
      "actionName": "Action Name value",
      "actionState": "pending",
      "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
      "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
    }
  ],
  "managementState": "retirePending",
  "enrolledDateTime": "2016-12-31T23:59:43.797191-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "chassisType": "desktop",
  "operatingSystem": "Operating System value",
  "deviceType": "windowsRT",
  "complianceState": "compliant",
  "jailBroken": "Jail Broken value",
  "managementAgent": "mdm",
  "osVersion": "Os Version value",
  "easActivated": true,
  "easDeviceId": "Eas Device Id value",
  "easActivationDateTime": "2016-12-31T23:59:43.4878784-08:00",
  "aadRegistered": true,
  "azureADRegistered": true,
  "deviceEnrollmentType": "userEnrollment",
  "lostModeState": "enabled",
  "activationLockBypassCode": "Activation Lock Bypass Code value",
  "emailAddress": "Email Address value",
  "azureActiveDirectoryDeviceId": "Azure Active Directory Device Id value",
  "azureADDeviceId": "Azure ADDevice Id value",
  "deviceRegistrationState": "registered",
  "deviceCategoryDisplayName": "Device Category Display Name value",
  "isSupervised": true,
  "exchangeLastSuccessfulSyncDateTime": "2017-01-01T00:00:45.8803083-08:00",
  "exchangeAccessState": "unknown",
  "exchangeAccessStateReason": "unknown",
  "remoteAssistanceSessionUrl": "https://example.com/remoteAssistanceSessionUrl/",
  "remoteAssistanceSessionErrorDetails": "Remote Assistance Session Error Details value",
  "isEncrypted": true,
  "userPrincipalName": "User Principal Name value",
  "model": "Model value",
  "manufacturer": "Manufacturer value",
  "imei": "Imei value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "serialNumber": "Serial Number value",
  "phoneNumber": "Phone Number value",
  "androidSecurityPatchLevel": "Android Security Patch Level value",
  "userDisplayName": "User Display Name value",
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
  "wiFiMacAddress": "Wi Fi Mac Address value",
  "deviceHealthAttestationState": {
    "@odata.type": "microsoft.graph.deviceHealthAttestationState",
    "lastUpdateDateTime": "Last Update Date Time value",
    "contentNamespaceUrl": "https://example.com/contentNamespaceUrl/",
    "deviceHealthAttestationStatus": "Device Health Attestation Status value",
    "contentVersion": "Content Version value",
    "issuedDateTime": "2016-12-31T23:58:22.1231038-08:00",
    "attestationIdentityKey": "Attestation Identity Key value",
    "resetCount": 10,
    "restartCount": 12,
    "dataExcutionPolicy": "Data Excution Policy value",
    "bitLockerStatus": "Bit Locker Status value",
    "bootManagerVersion": "Boot Manager Version value",
    "codeIntegrityCheckVersion": "Code Integrity Check Version value",
    "secureBoot": "Secure Boot value",
    "bootDebugging": "Boot Debugging value",
    "operatingSystemKernelDebugging": "Operating System Kernel Debugging value",
    "codeIntegrity": "Code Integrity value",
    "testSigning": "Test Signing value",
    "safeMode": "Safe Mode value",
    "windowsPE": "Windows PE value",
    "earlyLaunchAntiMalwareDriverProtection": "Early Launch Anti Malware Driver Protection value",
    "virtualSecureMode": "Virtual Secure Mode value",
    "pcrHashAlgorithm": "Pcr Hash Algorithm value",
    "bootAppSecurityVersion": "Boot App Security Version value",
    "bootManagerSecurityVersion": "Boot Manager Security Version value",
    "tpmVersion": "Tpm Version value",
    "pcr0": "Pcr0 value",
    "secureBootConfigurationPolicyFingerPrint": "Secure Boot Configuration Policy Finger Print value",
    "codeIntegrityPolicy": "Code Integrity Policy value",
    "bootRevisionListInfo": "Boot Revision List Info value",
    "operatingSystemRevListInfo": "Operating System Rev List Info value",
    "healthStatusMismatchInfo": "Health Status Mismatch Info value",
    "healthAttestationSupportedStatus": "Health Attestation Supported Status value"
  },
  "subscriberCarrier": "Subscriber Carrier value",
  "meid": "Meid value",
  "totalStorageSpaceInBytes": 8,
  "freeStorageSpaceInBytes": 7,
  "managedDeviceName": "Managed Device Name value",
  "partnerReportedThreatState": "activated",
  "usersLoggedOn": [
    {
      "@odata.type": "microsoft.graph.loggedOnUser",
      "userId": "User Id value",
      "lastLogOnDateTime": "2016-12-31T23:58:37.4262708-08:00"
    }
  ],
  "preferMdmOverGroupPolicyAppliedDateTime": "2016-12-31T23:57:34.4649887-08:00",
  "autopilotEnrolled": true,
  "requireUserEnrollmentApproval": true,
  "managementCertificateExpirationDate": "2016-12-31T23:57:59.9789653-08:00",
  "iccid": "Iccid value",
  "udid": "Udid value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "windowsActiveMalwareCount": 9,
  "windowsRemediatedMalwareCount": 13,
  "notes": "Notes value",
  "configurationManagerClientHealthState": {
    "@odata.type": "microsoft.graph.configurationManagerClientHealthState",
    "state": "installed",
    "errorCode": 9,
    "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00"
  }
}
```




