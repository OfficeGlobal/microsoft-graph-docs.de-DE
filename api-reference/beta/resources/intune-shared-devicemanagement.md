---
title: deviceManagement-Ressourcentyp
description: 'Die deviceManagement-Ressource stellt einen Container dar, dessen Inhalt sich je nach Workflow unterscheidet, einschließlich:  '
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: 23ea35468bbff4010b5ed089b086fbb6cd7a9845
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30163028"
---
# <a name="devicemanagement-resource-type"></a>deviceManagement-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Die deviceManagement-Ressource stellt einen Container dar, dessen Inhalt sich je nach Workflow unterscheidet, einschließlich:  

- Android for Work-Einstellungen
- Überwachungsereignisse
- Geschäftsbedingungen 
- Unternehmens Registrierungs profile
- Geräte Konfigurationseinstellungen
- Geräteverwaltung
- Elektronische SIM (ESIM)
- Fechten
- Benachrichtigungen
- Onboarding-Richtlinien, Einstellungen und Details
- Remote Zugriff
- Remote Unterstützungspartner
- Rollenbasierte Zugriffssteuerungsrichtlinien
- Telecom-Ausdehnungs-VERWALTUNGSPARTNER
- Problembehandlung bei Ereignissen
- Zusammenfassungen von Windows Information Protection

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[deviceManagement abrufen](../api/intune-shared-devicemanagement-get.md)|Lesen von Eigenschaften und Beziehungen des [deviceManagement](../resources/intune-shared-devicemanagement.md)-Objekts.|
|[deviceManagement aktualisieren](../api/intune-shared-devicemanagement-update.md)|Aktualisieren der Eigenschaften eines [deviceManagement](../resources/intune-shared-devicemanagement.md)-Objekts.|
|**deviceConfiguration**|
|[enableLegacyPcManagement-Aktion](../api/intune-shared-devicemanagement-enablelegacypcmanagement.md)|Keine|Noch nicht dokumentiert|
|**deviceManagement**|
|[sendCustomNotificationToCompanyPortal-Aktion](../api/intune-shared-devicemanagement-sendcustomnotificationtocompanyportal.md)|Keine|Noch nicht dokumentiert|
|**Onboarding**|
|[verifyWindowsEnrollmentAutoDiscovery-Funktion](../api/intune-shared-devicemanagement-verifywindowsenrollmentautodiscovery.md)|Boolescher Wert|Noch nicht dokumentiert|
|**Rollenbasierte Zugriffssteuerung (RBAC)**|
|[GetEffectivePermissions-Funktion](../api/intune-shared-devicemanagement-geteffectivepermissions.md)|[rolePermission](../resources/intune-rbac-rolepermission.md)-Sammlung|Ruft die effektiven Berechtigungen des derzeit authentifizierten Benutzers ab.|
|[getRoleScopeTagsByIds-Funktion](../api/intune-shared-devicemanagement-getrolescopetagsbyids.md)|[roleScopeTag](../resources/intune-rbac-rolescopetag.md) -Sammlung|Noch nicht dokumentiert|
|[getRoleScopeTagsByResource-Funktion](../api/intune-shared-devicemanagement-getrolescopetagsbyresource.md)|[roleScopeTag](../resources/intune-rbac-rolescopetag.md) -Sammlung|Noch nicht dokumentiert|


## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Dem Gerät zugeordneter eindeutiger Bezeichner.|
|**deviceConfiguration**|
|intuneAccountId|Guid|InTune-Konto-ID für angegebenen Mandanten|
|legacyPcManangementEnabled|Boolean|Die Eigenschaft zum Aktivieren der nicht-MDM-verwalteten Legacy-PC-Verwaltung für dieses Konto. Diese Eigenschaft ist schreibgeschützt.|
|maximumDepTokens|Int32|Maximale Anzahl der pro-Mandanten zulässigen DEP-Token.|
|settings|[deviceManagementSettings](../resources/intune-deviceconfig-devicemanagementsettings.md)|Einstellungen auf Kontoebene|
|**deviceManagement**|
|accountMoveCompletionDateTime|DateTimeOffset|Das Datum & Zeitpunkt, zu dem die Mandantendaten zwischen scaleunits verschoben wurden.|
|adminConsent|[adminConsent](../resources/intune-devices-adminconsent.md)|Informationen zur Administrator Einwilligung.|
|deviceProtectionOverview|[deviceProtectionOverview](../resources/intune-devices-deviceprotectionoverview.md)|Übersicht über Geräteschutz.|
|managedDeviceCleanupSettings|[managedDeviceCleanupSettings](../resources/intune-devices-manageddevicecleanupsettings.md)|Regel zur Gerätebereinigung|
|subscriptionState|[deviceManagementSubscriptionState](../resources/intune-devices-devicemanagementsubscriptionstate.md)|Status des Abonnements bei der Lösung für Mobilgeräteverwaltung des Mandanten. Mögliche Werte sind: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked` und `lockedOut`.|
|Abonnements|[deviceManagementSubscriptions](../resources/intune-devices-devicemanagementsubscriptions.md)|Abonnement des Mandanten. Mögliche Werte sind: `none`, `intune`, `office365`, `intunePremium`, `intune_EDU` und `intune_SMB`.|
|windowsMalwareOverview|[windowsMalwareOverview](../resources/intune-devices-windowsmalwareoverview.md)|Übersicht über Malware für Windows-Geräte.|
|**Onboarding**|
|intuneBrand|[intuneBrand](../resources/intune-onboarding-intunebrand.md)|„intuneBrand“ enthält Daten, mit denen das Aussehen der Unternehmensportal-Anwendungen und des Endbenutzer-Webportals angepasst wird.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;|
|:---|:---|:---|
|**Android for Work**|
|androidDeviceOwnerEnrollmentProfiles|[androiddeviceownerenrollmentprofile hinzugefügt](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) -Sammlung|Android-Gerätebesitzer-Registrierungsprofil Entitäten.|
|androidForWorkAppConfigurationSchemas|[androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md)-Sammlung|Android for Work-App – Konfigurationsschemaentitäten|
|androidForWorkEnrollmentProfiles|[androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md)-Sammlung|Android for Work-Registrierungsprofilentitäten.|
|androidForWorkSettings|[androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md)|Die Singleton-Entität mit Android for Work-Einstellungen.|
|androidManagedStoreAccountEnterpriseSettings|[androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md)|Das Singleton-Android Managed Store-Konto Enterprise-Einstellungs Entität.|
|androidManagedStoreAppConfigurationSchemas|[androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) -Sammlung|Android-Organisations-App-Konfigurationsschema Entitäten.|
|**Überwachung**|
|auditEvents|[auditEvent](../resources/intune-auditing-auditevent.md)-Sammlung|Audit-Ereignisse|
|**Geschäftsbedingungen des Unternehmens**|
|termsAndConditions|[termsAndConditions](../resources/intune-companyterms-termsandconditions.md)-Sammlung|Die allgemeinen Geschäftsbedingungen für die Geräteverwaltung des Unternehmens.|
|**Unternehmensregistrierung**|
|enrollmentProfiles|[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) -Sammlung|Die Registrierungs Profile.|
|importedAppleDeviceIdentities|[importappledeviceidentitylist](../resources/intune-enrollment-importedappledeviceidentity.md) -Sammlung|Die importierten Apple-Geräte Identitäten.|
|importedDeviceIdentities|[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) -Sammlung|Die importierten Geräte Identitäten.|
|**deviceConfiguration**|
|advancedThreatProtectionOnboardingStateSummary|[advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md)|Der Status des ATP-onboardings für dieses Konto.|
|cartToClassAssociations|[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) -Sammlung|Der Wagen zu Klassenzuordnungen.|
|deviceCompliancePolicies|[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)-Sammlung|Die Gerätekompatibilitätsrichtlinie|
|deviceCompliancePolicyDeviceStateSummary|[deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md)|Die Gerätekompatibilitäts-Statuszusammenfassung für dieses Konto|
|deviceCompliancePolicySettingStateSummaries|[deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md)-Sammlung|Die Zusammenfassungsstatus von Kompatibilitätsrichtlinieneinstellungen für dieses Konto|
|deviceConfigurationConflictSummary|[deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) -Sammlung|Zusammenfassung der Richtlinien im Konfliktstatus für dieses Konto.|
|deviceConfigurationDeviceStateSummaries|[deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md)|Die Gerätekonfigurations-Gerätestatuszusammenfassung für dieses Konto.|
|deviceConfigurationRestrictedAppsViolations|[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) -Sammlung|Eingeschränkte apps-Verstöße für dieses Konto.|
|deviceConfigurations|[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)-Sammlung|Die Gerätekonfigurationen|
|deviceConfigurationUserStateSummaries|[deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md)|Die Benutzerstatus Zusammenfassung für Gerätekonfiguration für dieses Konto.|
|iosUpdateStatuses|[iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md)-Sammlung|Die IOS-Softwareupdate-Installationsstatus für dieses Konto|
|ndesConnectors|[ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) -Sammlung|Die Auflistung der NDES-Connectors für dieses Konto.|
|softwareUpdateStatusSummary|[softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md)|Die Softwareaktualisierungs-Statuszusammenfassung|
|**deviceManagement**|
|applePushNotificationCertificate|[applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md)|Apple Push Notification-Zertifikat.|
|dataSharingConsents|[dataSharingConsent](../resources/intune-devices-datasharingconsent.md) -Sammlung|Gemeinsame Nutzung von Daten.|
|detectedApps|[detectedApp](../resources/intune-devices-detectedapp.md)-Sammlung|Die Liste der erkannten Apps, die einem Gerät zugeordnet sind.|
|deviceManagementScripts|[devicemanagementscript hinzugefügt](../resources/intune-devices-devicemanagementscript.md) -Sammlung|Die Liste der Device Management-Skripts, die dem Mandanten zugeordnet sind.|
|managedDeviceOverview|[managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md)|Geräteübersicht|
|managedDevices|[managedDevice](../resources/intune-devices-manageddevice.md)-Sammlung|Die Liste der verwalteten Geräte|
|remoteActionAudits|[Remote Action Audit](../resources/intune-devices-remoteactionaudit.md) -Sammlung|Die Liste der Geräte Remote-Aktions Überwachungen mit dem Mandanten.|
|windowsMalwareInformation|[windowsMalwareInformation](../resources/intune-devices-windowsmalwareinformation.md) -Sammlung|Die Liste der betroffenen Schadsoftware im Mandanten.|
|**Registrierung**|
|depOnboardingSettings|[depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) -Sammlung|Diese Auflistungen mehrerer DEP-Token pro Mandant.|
|importedDeviceIdentities|[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) -Sammlung|Die importierten Geräte Identitäten.|
|importedWindowsAutopilotDeviceIdentities|[importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md)-Sammlung|Sammlung von importierten Windows Autopilot-Geräten|
|importedWindowsAutopilotDeviceIdentityUploads|[importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) -Sammlung|Sammlung von Windows Autopilot-Geräten hochladen.|
|windowsAutopilotDeploymentProfiles|[windowsautopilotdeploymentprofile hinzugefügt](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md) -Sammlung|Windows Auto Pilot-bereitstellungsprofile|
|windowsAutopilotDeviceIdentities|[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) -Sammlung|Die Windows Autopilot-Geräte Identitäten enthielten die Sammlung.|
|windowsAutopilotSettings|[windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)|Die Windows Autopilot-Kontoeinstellungen.|
|**Eingebettete SIM-Karte**|
|embeddedSIMActivationCodePools|[embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) -Sammlung|Die von diesem Konto erstellten eingebetteten SIM-Aktivierungscode Pools.|
|**Fechten**|
|managementConditions|[managementCondition](../resources/intune-fencing-managementcondition.md) -Sammlung|Die Verwaltungsbedingungen im Zusammenhang mit der Geräteverwaltung des Unternehmens.|
|managementConditionStatements|[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) -Sammlung|Die Verwaltungs Bedingungsanweisungen, die der Geräteverwaltung des Unternehmens zugeordnet sind.|
|**Benachrichtigungen**|
|notificationMessageTemplates|[notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md)-Sammlung|Benachrichtigungsvorlage|
|**Onboarding**|
|conditionalAccessSettings|[onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md)|Die Exchange-Einstellungen für den lokalen, bedingten Zugriff. Für den lokalen, bedingten Zugriff müssen Geräte registriert und für den E-Mail-Zugriff kompatibel sein.|
|deviceCategories|[deviceCategory](../resources/intune-shared-devicecategory.md)-Sammlung|Die Liste der Gerätekategorien mit dem Mandanten.|
|deviceEnrollmentConfigurations|[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)-Sammlung|Die Liste der Konfigurationen der Geräteregistrierung.|
|deviceManagementPartners|[deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md)-Sammlung|Die Liste der vom Mandanten konfigurierten Geräteverwaltungspartner.|
|exchangeConnectors|[deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md)-Sammlung|Die Liste der vom Mandanten konfigurierten Exchange-Connectors.|
|exchangeOnPremisesPolicies|[deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) -Sammlung|Die Liste der vom Mandanten konfigurierten Richtlinien für Exchange on premises.|
|exchangeOnPremisesPolicy|[deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md)|Die Richtlinie, die den Zugriff mobiler Geräte auf Exchange vor Ort steuert|
|mobileThreatDefenseConnectors|[mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md)-Sammlung|Die Liste der vom Mandanten konfigurierten MTD-Connectors (Mobile Threat Defense).|
|**Remote Zugriff**|
|Userpfxcertificateswurde|[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) -Sammlung|Sammlung von PFX-Zertifikaten, die einem Benutzer zugeordnet sind.|
|**Remote Unterstützung**|
|remoteAssistancePartners|[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md)-Sammlung|Die Partner für die Remoteunterstützung.|
|**Rollenbasierte Zugriffssteuerung (RBAC)**|
|resourceOperations|[resourceOperation](../resources/intune-rbac-resourceoperation.md)-Sammlung|Ressourcenvorgänge|
|roleAssignments|[DeviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md)-Sammlung|Rollenzuweisungen|
|roleDefinitions|[roleDefinition](../resources/intune-rbac-roledefinition.md)-Sammlung|Rollendefinitionen|
|roleScopeTags|[roleScopeTag](../resources/intune-rbac-rolescopetag.md) -Sammlung|Die Rollenbereichs Tags.|
|**Telekom-Spesenmanagement (TEM)**|
|telecomExpenseManagementPartners|[telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md)-Sammlung|Telecom Expense Management-Partner|
|**Problembehandlung**|
|troubleshootingEvents|[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)-Sammlung|Die Liste der Problembehandlungsereignisse für den Mandanten.|
|**Windows Information Protection**|
|intuneBrandingProfiles|[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) -Sammlung|InTune-Branding-Profile für AAD-Gruppen|
|windowsInformationProtectionAppLearningSummaries|[windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md)-Sammlung|Windows Information Protection  – App-Schulungszusammenfassung|
|windowsInformationProtectionNetworkLearningSummaries|[windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md)-Sammlung|Windows Information Protection – Netzwerk-Schulungszusammenfassung|


## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagement",
  "id": "String (identifier)",
  "subscriptionState": "String"
}
```



