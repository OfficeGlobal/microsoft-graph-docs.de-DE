---
title: managedDevice-Ressourcentyp
description: Über Intune verwaltete oder vorab registrierte Geräte
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 3643ec5020ea088b2da423ed44d0a1596e53e6a9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27955730"
---
# <a name="manageddevice-resource-type"></a>managedDevice-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Über Intune verwaltete oder vorab registrierte Geräte
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[managedDevices auflisten](../api/intune-devices-manageddevice-list.md)|[managedDevice](../resources/intune-devices-manageddevice.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [managedDevice](../resources/intune-devices-manageddevice.md)-Objekte.|
|[managedDevice abrufen](../api/intune-devices-manageddevice-get.md)|[managedDevice](../resources/intune-devices-manageddevice.md)|Lesen von Eigenschaften und Beziehungen des [managedDevice](../resources/intune-devices-manageddevice.md)-Objekts.|
|[managedDevice erstellen](../api/intune-devices-manageddevice-create.md)|[managedDevice](../resources/intune-devices-manageddevice.md)|Erstellen eines neuen [managedDevice](../resources/intune-devices-manageddevice.md)-Objekts.|
|[managedDevice löschen](../api/intune-devices-manageddevice-delete.md)|Keine|Löscht ein [managedDevice löschen](../resources/intune-devices-manageddevice.md).|
|[managedDevice aktualisieren](../api/intune-devices-manageddevice-update.md)|[managedDevice](../resources/intune-devices-manageddevice.md)|Aktualisieren der Eigenschaften eines [managedDeviceOverview](../resources/intune-devices-manageddevice.md)-Objekts.|
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

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Eindeutiger Bezeichner für das Gerät.
|
|userId|Zeichenfolge|Eindeutiger Bezeichner des Benutzers, der dem Gerät zugeordnet ist.
|
|deviceName|Zeichenfolge|Name des Geräts.
|
|managedDeviceOwnerType|[managedDeviceOwnerType](../resources/intune-devices-manageddeviceownertype.md)|Besitz des Geräts. 'Company' oder 'Privat' kann sein. Mögliche Werte sind: `unknown`, `company` und `personal`.|
|deviceActionResults|Collection von Objekten des Typs [deviceActionResult](../resources/intune-devices-deviceactionresult.md)|Liste von Objekten des Typs „ComplexType deviceActionResult“.
|
|enrolledDateTime|DateTimeOffset|Datum und Uhrzeit der Geräteregistrierung.
|
|lastSyncDateTime|DateTimeOffset|Datum und Uhrzeit der letzten erfolgreichen Synchronisierung des Geräts mit Intune.
|
|operatingSystem|Zeichenfolge|Betriebssystem des Geräts. Windows, iOS usw.|
|complianceState|[complianceState](../resources/intune-devices-compliancestate.md)|Konformitätsstatus des Geräts. Mögliche Werte sind: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod` und `configManager`.|
|jailBroken|Zeichenfolge|Gibt an, ob es sich um ein Gerät mit Jailbreak oder Rootzugriff handelt.|
|managementAgent|[managementAgentType](../resources/intune-devices-managementagenttype.md)|Verwaltungskanal des Geräts. Intune, EAS usw. Mögliche Werte sind: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf` und `googleCloudDevicePolicyController`.|
|osVersion|Zeichenfolge|Auf dem Gerät installierte Betriebssystemversion.
|
|easActivated|Boolescher Wert|Gibt an, ob für das Gerät Exchange ActiveSync aktiviert ist.|
|easDeviceId|Zeichenfolge|Exchange ActiveSync-ID des Geräts.
|
|easActivationDateTime|DateTimeOffset|Datum und Uhrzeit der Exchange ActiveSync-Aktivierung für das Gerät.
|
|azureADRegistered|Boolescher Wert|Gibt an, ob das Gerät in Azure Active Directory registriert ist.|
|deviceEnrollmentType|[deviceEnrollmentType](../resources/intune-devices-deviceenrollmenttype.md)|Registrierungstyp des Geräts. Mögliche Werte: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.|
|activationLockBypassCode|Zeichenfolge|Code, der die Umgehung der Aktivierungssperre des Geräts ermöglicht|
|emailAddress|Zeichenfolge|E-Mail-Adressen des Benutzers, der dem Gerät zugeordnet ist.
|
|azureADDeviceId|Zeichenfolge|Eindeutiger Bezeichner des Azure Active Directory-Geräts. Schreibgeschützt.|
|deviceRegistrationState|[deviceRegistrationState](../resources/intune-devices-deviceregistrationstate.md)|Registrierungsstatus des Geräts. Mögliche Werte sind: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset` und `notRegisteredPendingEnrollment`, `unknown`.|
|deviceCategoryDisplayName|Zeichenfolge|Anzeigename der Gerätekategorie.
|
|isSupervised|Boolescher Wert|Überwachungsstatus des Geräts.
|
|exchangeLastSuccessfulSyncDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Verbindung des Geräts mit Exchange|
|exchangeAccessState|[deviceManagementExchangeAccessState](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|Zugriffsstatus des Geräts in Exchange. Mögliche Werte sind: `none`, `unknown`, `allowed`, `blocked` und `quarantined`.|
|exchangeAccessStateReason|[deviceManagementExchangeAccessStateReason](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|Grund für den Zugriffsstatus des Geräts in Exchange. Mögliche Werte sind: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword` und `deviceNotKnownWithManagedApp`.|
|remoteAssistanceSessionUrl|Zeichenfolge|URL zur Einrichtung einer Remoteunterstützungssitzung mit dem Gerät.
|
|remoteAssistanceSessionErrorDetails|Zeichenfolge|Fehlerzeichenfolge zur Beschreibung von Fehlern beim Erstellen von Objekten für Remoteunterstützungssitzungen.
|
|isEncrypted|Boolescher Wert|Verschlüsselungsstatus des Geräts.
|
|userPrincipalName|Zeichenfolge|Benutzerprinzipalname für das Gerät.
|
|model|Zeichenfolge|Modell des Geräts.
|
|manufacturer|Zeichenfolge|Hersteller des Geräts.
|
|imei|Zeichenfolge|IMEI|
|complianceGracePeriodExpirationDateTime|DateTimeOffset|Datum und Uhrzeit des Ablaufs der Toleranzperiode für die Gerätekonformität.
|
|serialNumber|Zeichenfolge|Seriennummer.
|
|PhoneNumber|Zeichenfolge|Telefonnummer des Geräts.
|
|androidSecurityPatchLevel|Zeichenfolge|Android-Sicherheitspatchlevel.
|
|userDisplayName|Zeichenfolge|Anzeigename des Benutzers.
|
|configurationManagerClientEnabledFeatures|[configurationManagerClientEnabledFeatures](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|Aktivierte Funktionen des Konfigurations-Manager-Clients.
|
|wiFiMacAddress|Zeichenfolge|WLAN-MAC|
|deviceHealthAttestationState|[deviceHealthAttestationState](../resources/intune-devices-devicehealthattestationstate.md)|Status des Integritätsnachweises für Geräte.
|
|subscriberCarrier|Zeichenfolge|Netzbetreiber des Abonnenten.
|
|meid|Zeichenfolge|MEID|
|totalStorageSpaceInBytes|Int64|Gesamtspeicher in Byte.
|
|freeStorageSpaceInBytes|Int64|Freier Speicher in Byte.
|
|managedDeviceName|Zeichenfolge|Automatisch generierter Name zur Identifizierung des Geräts. Kann mit einem benutzerfreundlichen Namen überschrieben werden.|
|partnerReportedThreatState|[managedDevicePartnerReportedHealthState](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|Gibt den Bedrohungsstatus eines Geräts an, wenn das Konto und das Gerät einen Mobile Threat Defense-Partner nutzen. Schreibgeschützt. Mögliche Werte: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|deviceCategory|[deviceCategory](../resources/intune-shared-devicecategory.md)|Gerätekategorie|

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
  "enrolledDateTime": "String (timestamp)",
  "lastSyncDateTime": "String (timestamp)",
  "operatingSystem": "String",
  "complianceState": "String",
  "jailBroken": "String",
  "managementAgent": "String",
  "osVersion": "String",
  "easActivated": true,
  "easDeviceId": "String",
  "easActivationDateTime": "String (timestamp)",
  "azureADRegistered": true,
  "deviceEnrollmentType": "String",
  "activationLockBypassCode": "String",
  "emailAddress": "String",
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
  "partnerReportedThreatState": "String"
}
```



