---
title: managedDevice-Ressourcentyp
description: Über Intune verwaltete oder vorab registrierte Geräte
ms.openlocfilehash: eaca9444df77c2f95f6a6f9845c9383cd53cd99f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063524"
---
# <a name="manageddevice-resource-type"></a>managedDevice-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Über Intune verwaltete oder vorab registrierte Geräte
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[managedDevice abrufen](../api/intune-devices-manageddevice-get.md)|[managedDevice](../resources/intune-devices-manageddevice.md)|Lesen von Eigenschaften und Beziehungen des [managedDevice](../resources/intune-devices-manageddevice.md)-Objekts.|
|[managedDevice aktualisieren](../api/intune-devices-manageddevice-update.md)|[managedDevice](../resources/intune-devices-manageddevice.md)|Aktualisieren der Eigenschaften eines [managedDeviceOverview](../resources/intune-devices-manageddevice.md)-Objekts.|
|[ExecuteAction-Aktion](../api/intune-devices-manageddevice-executeaction.md)|[bulkManagedDeviceActionResult](../resources/intune-devices-bulkmanageddeviceactionresult.md)|Noch nicht dokumentiert|
|[EnableLostMode Aktion](../api/intune-devices-manageddevice-enablelostmode.md)|Keines|Verloren-Modus aktivieren|
|[PlayLostModeSound Aktion](../api/intune-devices-manageddevice-playlostmodesound.md)|Keine|Remotesperre|
|[SetDeviceName Aktion](../api/intune-devices-manageddevice-setdevicename.md)|Keines|Festlegen Sie Name des Aufnahmegeräts des Geräts.|
|[retire-Aktion](../api/intune-devices-manageddevice-retire.md)|Keine|Zurückziehen eines Geräts|
|[wipe-Aktion](../api/intune-devices-manageddevice-wipe.md)|Keine|Zurücksetzen eines Geräts|
|[resetPasscode-Aktion](../api/intune-devices-manageddevice-resetpasscode.md)|Keine|Kennung zurücksetzen|
|[remoteLock-Aktion](../api/intune-devices-manageddevice-remotelock.md)|Keine|Remotesperre|
|[requestRemoteAssistance-Aktion](../api/intune-devices-manageddevice-requestremoteassistance.md)|Keine|Remoteunterstützung anfordern|
|[disableLostMode-Aktion](../api/intune-devices-manageddevice-disablelostmode.md)|Keine|Modus für verlorene Geräte deaktivieren|
|[locateDevice-Aktion](../api/intune-devices-manageddevice-locatedevice.md)|Keine|Suchen eines Geräts|
|[bypassActivationLock-Aktion](../api/intune-devices-manageddevice-bypassactivationlock.md)|Keine|Aktivierungssperre umgehen|
|[rebootNow-Aktion](../api/intune-devices-manageddevice-rebootnow.md)|Keine|Gerät neu starten|
|[shutDown-Aktion](../api/intune-devices-manageddevice-shutdown.md)|Keine|Gerät abschalten|
|[recoverPasscode-Aktion](../api/intune-devices-manageddevice-recoverpasscode.md)|Keine|Kennung wiederherstellen|
|[cleanWindowsDevice-Aktion](../api/intune-devices-manageddevice-cleanwindowsdevice.md)|Keine|Windows-Gerät bereinigen|
|[logoutSharedAppleDeviceActiveUser-Aktion](../api/intune-devices-manageddevice-logoutsharedappledeviceactiveuser.md)|Keine|Aktiven Benutzer von freigegebenem Apple-Gerät abmelden|
|[deleteUserFromSharedAppleDevice-Aktion](../api/intune-devices-manageddevice-deleteuserfromsharedappledevice.md)|Keine|Benutzer von freigegebenem Apple-Gerät löschen|
|[syncDevice-Aktion](../api/intune-devices-manageddevice-syncdevice.md)|Keine|Noch nicht dokumentiert.|
|[windowsDefenderScan-Aktion](../api/intune-devices-manageddevice-windowsdefenderscan.md)|Keine|Noch nicht dokumentiert.|
|[windowsDefenderUpdateSignatures-Aktion](../api/intune-devices-manageddevice-windowsdefenderupdatesignatures.md)|Keine|Noch nicht dokumentiert.|
|[updateWindowsDeviceAccount-Aktion](../api/intune-devices-manageddevice-updatewindowsdeviceaccount.md)|Keine|Noch nicht dokumentiert|
|[RevokeAppleVppLicenses Aktion](../api/intune-devices-manageddevice-revokeapplevpplicenses.md)|Keines|Alle Apple Vpp Lizenzen für ein Gerät widerrufen|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Eindeutiger Bezeichner für das Gerät.
|
|userId|String|Eindeutiger Bezeichner des Benutzers, der dem Gerät zugeordnet ist.
|
|deviceName|String|Name des Geräts.
|
|hardwareInformation|[hardwareInformation](../resources/intune-devices-hardwareinformation.md)|Die Hardward Details für das Gerät.  Enthält Informationen, wie Speicherplatz, Hersteller, Seriennummer.|
|Besitzertyp|[Besitzertyp](../resources/intune-devices-ownertype.md)|Besitz des Geräts. 'Company' oder 'Privat' kann sein. Mögliche Werte sind: `unknown`, `company` und `personal`.|
|managedDeviceOwnerType|[managedDeviceOwnerType](../resources/intune-devices-manageddeviceownertype.md)|Besitz des Geräts. 'Company' oder 'Privat' kann sein. Mögliche Werte sind: `unknown`, `company` und `personal`.|
|deviceActionResults|Collection von Objekten des Typs [deviceActionResult](../resources/intune-devices-deviceactionresult.md)|Liste von Objekten des Typs „ComplexType deviceActionResult“.
|
|managementState|[managementState](../resources/intune-devices-managementstate.md)|Verwaltungsstatus des Geräts. Mögliche Werte sind: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled` und `discovered`.|
|enrolledDateTime|DateTimeOffset|Datum und Uhrzeit der Geräteregistrierung.
|
|lastSyncDateTime|DateTimeOffset|Datum und Uhrzeit der letzten erfolgreichen Synchronisierung des Geräts mit Intune.
|
|chassisType|[chassisType](../resources/intune-devices-chassistype.md)|Chassistyp des Geräts. Mögliche Werte: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.|
|operatingSystem|String|Betriebssystem des Geräts. Windows, iOS usw.|
|deviceType|[deviceType](../resources/intune-shared-devicetype.md)|Plattform des Geräts. Mögliche Werte sind: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise` , `blackberry`, `palm`, `unknown`.|
|complianceState|[complianceState](../resources/intune-devices-compliancestate.md)|Konformitätsstatus des Geräts. Mögliche Werte sind: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod` und `configManager`.|
|jailBroken|String|Gibt an, ob es sich um ein Gerät mit Jailbreak oder Rootzugriff handelt.|
|managementAgent|[managementAgentType](../resources/intune-devices-managementagenttype.md)|Verwaltungskanal des Geräts. Intune, EAS usw. Mögliche Werte sind: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.|
|osVersion|String|Auf dem Gerät installierte Betriebssystemversion.
|
|easActivated|Boolescher Wert|Gibt an, ob für das Gerät Exchange ActiveSync aktiviert ist.|
|easDeviceId|String|Exchange ActiveSync-ID des Geräts.
|
|easActivationDateTime|DateTimeOffset|Datum und Uhrzeit der Exchange ActiveSync-Aktivierung für das Gerät.
|
|aadRegistered|Boolescher Wert|Gibt an, ob das Gerät in Azure Active Directory registriert ist.|
|azureADRegistered|Boolescher Wert|Gibt an, ob das Gerät in Azure Active Directory registriert ist.|
|deviceEnrollmentType|[deviceEnrollmentType](../resources/intune-shared-deviceenrollmenttype.md)|Registrierungstyp des Geräts. Mögliche Werte: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.|
|lostModeState|[lostModeState](../resources/intune-devices-lostmodestate.md)|Gibt an, ob verloren-Modus aktiviert oder deaktiviert ist. Mögliche Werte sind: `disabled` und `enabled`.|
|activationLockBypassCode|String|Code, der die Umgehung der Aktivierungssperre des Geräts ermöglicht|
|emailAddress|String|E-Mail-Adressen des Benutzers, der dem Gerät zugeordnet ist.
|
|azureActiveDirectoryDeviceId|String|Eindeutiger Bezeichner des Azure Active Directory-Geräts. Schreibgeschützt.|
|azureADDeviceId|String|Eindeutiger Bezeichner des Azure Active Directory-Geräts. Schreibgeschützt.|
|deviceRegistrationState|[deviceRegistrationState](../resources/intune-devices-deviceregistrationstate.md)|Registrierungsstatus des Geräts. Mögliche Werte sind: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset` und `notRegisteredPendingEnrollment`, `unknown`.|
|deviceCategoryDisplayName|String|Anzeigename der Gerätekategorie.
|
|isSupervised|Boolescher Wert|Überwachungsstatus des Geräts.
|
|exchangeLastSuccessfulSyncDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Verbindung des Geräts mit Exchange|
|exchangeAccessState|[deviceManagementExchangeAccessState](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|Zugriffsstatus des Geräts in Exchange. Mögliche Werte sind: `none`, `unknown`, `allowed`, `blocked` und `quarantined`.|
|exchangeAccessStateReason|[deviceManagementExchangeAccessStateReason](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|Grund für den Zugriffsstatus des Geräts in Exchange. Mögliche Werte sind: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword` und `deviceNotKnownWithManagedApp`.|
|remoteAssistanceSessionUrl|String|URL zur Einrichtung einer Remoteunterstützungssitzung mit dem Gerät.
|
|remoteAssistanceSessionErrorDetails|String|Fehlerzeichenfolge zur Beschreibung von Fehlern beim Erstellen von Objekten für Remoteunterstützungssitzungen.
|
|isEncrypted|Boolescher Wert|Verschlüsselungsstatus des Geräts.
|
|userPrincipalName|String|Benutzerprinzipalname für das Gerät.
|
|model|String|Modell des Geräts.
|
|manufacturer|String|Hersteller des Geräts.
|
|imei|String|IMEI|
|complianceGracePeriodExpirationDateTime|DateTimeOffset|Datum und Uhrzeit des Ablaufs der Toleranzperiode für die Gerätekonformität.
|
|serialNumber|String|Seriennummer.
|
|PhoneNumber|String|Telefonnummer des Geräts.
|
|androidSecurityPatchLevel|String|Android-Sicherheitspatchlevel.
|
|userDisplayName|String|Anzeigename des Benutzers.
|
|configurationManagerClientEnabledFeatures|[configurationManagerClientEnabledFeatures](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|Aktivierte Funktionen des Konfigurations-Manager-Clients.
|
|wiFiMacAddress|String|WLAN-MAC|
|deviceHealthAttestationState|[deviceHealthAttestationState](../resources/intune-devices-devicehealthattestationstate.md)|Status des Integritätsnachweises für Geräte.
|
|subscriberCarrier|String|Netzbetreiber des Abonnenten.
|
|meid|String|MEID|
|totalStorageSpaceInBytes|Int64|Gesamtspeicher in Byte.
|
|freeStorageSpaceInBytes|Int64|Freier Speicher in Byte.
|
|managedDeviceName|String|Automatisch generierter Name zur Identifizierung des Geräts. Kann mit einem benutzerfreundlichen Namen überschrieben werden.|
|partnerReportedThreatState|[managedDevicePartnerReportedHealthState](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|Gibt den Bedrohungsstatus eines Geräts an, wenn das Konto und das Gerät einen Mobile Threat Defense-Partner nutzen. Schreibgeschützt. Mögliche Werte: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.|
|usersLoggedOn|[LoggedOnUser](../resources/intune-devices-loggedonuser.md) -Auflistung|Gibt das letzte angemeldete Benutzer eines Geräts|
|preferMdmOverGroupPolicyAppliedDateTime|DateTimeOffset|Meldet den DateTime-Wert die Einstellung PreferMdmOverGroupPolicy festgelegt wurde.  Wenn festgelegt ist, werden die Intune MDM Einstellungen Group Policy Settings außer Kraft setzen, wenn ein Konflikt vorliegt. Schreibgeschützt.|
|autopilotEnrolled|Boolesch|Gibt an, ob das verwaltete Geräte über den Auto-Pilot registriert ist.|
|requireUserEnrollmentApproval|Boolesch|Gibt an, ob das Gerät verwalteten iOS Benutzer Genehmigung Registrierung wird.|
|managementCertificateExpirationDate|DateTimeOffset|Ablaufdatum des Zertifikats Berichte Gerät management|
|iccid|String|Chip Karte Bezeichner, ist es eine SIM-Karte eindeutige ID-Nummer.|
|UDID|String|Eindeutige Geräte-ID für iOS und Mac OS-Geräte.|
|roleScopeTagIds|Collection von Objekten des Typs „String“|Liste der Bereichs-Tag-IDs für diese Instanz des Geräts.|
|windowsActiveMalwareCount|Int32|Anzahl von aktiven Malware für dieses Windows-Gerät|
|windowsRemediatedMalwareCount|Int32|Anzahl der für gewartete Malware für dieses Windows-Gerät|
|notes|String|Notes auf dem Gerät durch den IT-Administrator erstellt|
|configurationManagerClientHealthState|[configurationManagerClientHealthState](../resources/intune-devices-configurationmanagerclienthealthstate.md)|Konfigurations-Manager-Client Integritätsstatus, gilt nur für Geräte verwaltet von MDM/Configuration Manager-Agent|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|detectedApps|[detectedApp](../resources/intune-devices-detectedapp.md)-Sammlung|Alle Programme, die derzeit auf dem Gerät installiert.|
|deviceCategory|[deviceCategory](../resources/intune-shared-devicecategory.md)|Gerätekategorie|
|windowsProtectionState|[windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md)|Das Gerät Sicherheitsstatus.|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDevice"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDevice",
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




