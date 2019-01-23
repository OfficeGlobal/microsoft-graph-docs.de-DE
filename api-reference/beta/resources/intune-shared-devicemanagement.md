---
title: deviceManagement-Ressourcentyp
description: 'Die Ressource DeviceManagement stellt einen Container, deren Inhalt variieren nach Workflow je, einschließlich:  '
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: 05620a5b34125920399434824d9f42ccea989c72
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396420"
---
# <a name="devicemanagement-resource-type"></a>deviceManagement-Ressourcentyp

> **Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.

Die Ressource DeviceManagement stellt einen Container, deren Inhalt variieren nach Workflow je, einschließlich:  

- Android for Work-Einstellungen
- Überwachung der Ereignisse
- Geschäftsbedingungen im Unternehmen 
- Im Unternehmen Registrierung Profile
- Die Konfiguration für Geräte
- Geräteverwaltung
- Elektronische SIM (ESIM)
- Zauns
- Benachrichtigungen
- Onboarding-Richtlinien, Einstellungen und details
- Remotezugriff
- Remoteunterstützung Partner
- Rollenbasierte Zugriffssteuerung (RBAC) Zugriffsrichtlinien
- Telekommunikation weite Management-Partner
- Problembehandlung bei Ereignissen
- Windows Information Protection Zusammenfassungen

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[deviceManagement abrufen](../api/intune-shared-devicemanagement-get.md)|Lesen von Eigenschaften und Beziehungen des [deviceManagement](../resources/intune-shared-devicemanagement.md)-Objekts.|
|[deviceManagement aktualisieren](../api/intune-shared-devicemanagement-update.md)|Aktualisieren der Eigenschaften eines [deviceManagement](../resources/intune-shared-devicemanagement.md)-Objekts.|
|**deviceConfiguration**|
|[EnableLegacyPcManagement Aktion](../api/intune-shared-devicemanagement-enablelegacypcmanagement.md)|Keine|Noch nicht dokumentiert|
|**deviceManagement**|
|[SendCustomNotificationToCompanyPortal Aktion](../api/intune-shared-devicemanagement-sendcustomnotificationtocompanyportal.md)|Keine|Noch nicht dokumentiert|
|**Onboarding**|
|[verifyWindowsEnrollmentAutoDiscovery-Funktion](../api/intune-shared-devicemanagement-verifywindowsenrollmentautodiscovery.md)|Boolescher Wert|Noch nicht dokumentiert|
|**Rollenbasierte Zugriffssteuerung (RBAC)**|
|[GetEffectivePermissions-Funktion](../api/intune-shared-devicemanagement-geteffectivepermissions.md)|[rolePermission](../resources/intune-rbac-rolepermission.md)-Sammlung|Ruft die effektiven Berechtigungen des derzeit authentifizierten Benutzers ab.|
|[GetRoleScopeTagsByIds-Funktion](../api/intune-shared-devicemanagement-getrolescopetagsbyids.md)|[RoleScopeTag](../resources/intune-rbac-rolescopetag.md) -Auflistung|Noch nicht dokumentiert|
|[GetRoleScopeTagsByResource-Funktion](../api/intune-shared-devicemanagement-getrolescopetagsbyresource.md)|[RoleScopeTag](../resources/intune-rbac-rolescopetag.md) -Auflistung|Noch nicht dokumentiert|


## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Eindeutiger Bezeichner für das Gerät.|
|**deviceConfiguration**|
|intuneAccountId|Guid|Intune Konto-ID für die angegebenen Mandanten|
|legacyPcManangementEnabled|Boolean|Die Eigenschaft zum Aktivieren von nicht-MDM verwaltet legacy PC-Verwaltung für dieses Konto. Diese Eigenschaft ist schreibgeschützt.|
|maximumDepTokens|Int32|Maximal zulässige Anzahl von DEP Token pro Mandant.|
|settings|[deviceManagementSettings](../resources/intune-deviceconfig-devicemanagementsettings.md)|Einstellungen auf Kontoebene|
|**deviceManagement**|
|accountMoveCompletionDateTime|DateTimeOffset|Das Datum & Uhrzeit wann Mandantendaten zwischen Scaleunits verschoben.|
|adminConsent|[adminConsent](../resources/intune-devices-adminconsent.md)|Informationen zum Unternehmensadministrator Zustimmung.|
|deviceProtectionOverview|[deviceProtectionOverview](../resources/intune-devices-deviceprotectionoverview.md)|Gerät Protection Overview.|
|managedDeviceCleanupSettings|[managedDeviceCleanupSettings](../resources/intune-devices-manageddevicecleanupsettings.md)|Cleanup-Regel|
|subscriptionState|[deviceManagementSubscriptionState](../resources/intune-devices-devicemanagementsubscriptionstate.md)|Status des Abonnements bei der Lösung für Mobilgeräteverwaltung des Mandanten. Mögliche Werte sind: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked` und `lockedOut`.|
|Abonnements|[deviceManagementSubscriptions](../resources/intune-devices-devicemanagementsubscriptions.md)|Mandanten-Abonnement. Mögliche Werte sind: `none`, `intune`, `office365`, `intunePremium`, `intune_EDU` und `intune_SMB`.|
|windowsMalwareOverview|[windowsMalwareOverview](../resources/intune-devices-windowsmalwareoverview.md)|Übersicht über die Malware für Windows-Geräte.|
|**Onboarding**|
|intuneBrand|[intuneBrand](../resources/intune-onboarding-intunebrand.md)|„intuneBrand“ enthält Daten, mit denen das Aussehen der Unternehmensportal-Anwendungen und des Endbenutzer-Webportals angepasst wird.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;|
|:---|:---|:---|
|**Android für die Arbeit**|
|androidDeviceOwnerEnrollmentProfiles|[AndroidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) -Auflistung|Android-Gerät Besitzer Registrierung Profil Entitäten.|
|androidForWorkAppConfigurationSchemas|[androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md)-Sammlung|Android for Work-App – Konfigurationsschemaentitäten|
|androidForWorkEnrollmentProfiles|[androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md)-Sammlung|Android for Work-Registrierungsprofilentitäten.|
|androidForWorkSettings|[androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md)|Die Singleton-Entität mit Android for Work-Einstellungen.|
|androidManagedStoreAccountEnterpriseSettings|[androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md)|Der Singleton Android verwaltet speichern Konto Enterprise Einstellungen Entität.|
|androidManagedStoreAppConfigurationSchemas|[AndroidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) -Auflistung|Android Enterprise app Configuration Schema-Entitäten.|
|**Überwachung**|
|auditEvents|[auditEvent](../resources/intune-auditing-auditevent.md)-Sammlung|Audit-Ereignisse|
|**Unternehmen Begriffe**|
|termsAndConditions|[termsAndConditions](../resources/intune-companyterms-termsandconditions.md)-Sammlung|Die allgemeinen Geschäftsbedingungen für die Geräteverwaltung des Unternehmens.|
|**Unternehmens-Registrierung**|
|enrollmentProfiles|[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) -Auflistung|Die Registrierung Profile.|
|importedAppleDeviceIdentities|[ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) -Auflistung|Die importierten Apple Gerät Identitäten.|
|importedDeviceIdentities|[ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) -Auflistung|Die importierten Gerät Identitäten.|
|**deviceConfiguration**|
|advancedThreatProtectionOnboardingStateSummary|[advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md)|Zusammenfassung des Status des ATP Onboarding Status für dieses Konto.|
|cartToClassAssociations|[CartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) -Auflistung|Der Einkaufswagen in Klasse Zuordnungen.|
|deviceCompliancePolicies|[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)-Sammlung|Die Gerätekompatibilitätsrichtlinie|
|deviceCompliancePolicyDeviceStateSummary|[deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md)|Die Gerätekompatibilitäts-Statuszusammenfassung für dieses Konto|
|deviceCompliancePolicySettingStateSummaries|[deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md)-Sammlung|Die Zusammenfassungsstatus von Kompatibilitätsrichtlinieneinstellungen für dieses Konto|
|deviceConfigurationConflictSummary|[DeviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) -Auflistung|Zusammenfassung der Richtlinien in Konflikt Zustand für dieses Konto.|
|deviceConfigurationDeviceStateSummaries|[deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md)|Die Gerätekonfigurations-Gerätestatuszusammenfassung für dieses Konto.|
|deviceConfigurationRestrictedAppsViolations|[RestrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) -Auflistung|Eingeschränkte apps Verstöße für dieses Konto.|
|deviceConfigurations|[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)-Sammlung|Die Gerätekonfigurationen|
|deviceConfigurationUserStateSummaries|[deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md)|Das Gerät Konfiguration Benutzerstatus Zusammenfassung für dieses Konto.|
|iosUpdateStatuses|[iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md)-Sammlung|Die IOS-Softwareupdate-Installationsstatus für dieses Konto|
|ndesConnectors|[NdesConnector](../resources/intune-deviceconfig-ndesconnector.md) -Auflistung|Die Auflistung der Ndes Connectors für dieses Konto.|
|softwareUpdateStatusSummary|[softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md)|Die Softwareaktualisierungs-Statuszusammenfassung|
|**deviceManagement**|
|applePushNotificationCertificate|[applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md)|Apple Push Notification-Zertifikat.|
|dataSharingConsents|[DataSharingConsent](../resources/intune-devices-datasharingconsent.md) -Auflistung|Datenfreigabe zustimmt.|
|detectedApps|[detectedApp](../resources/intune-devices-detectedapp.md)-Sammlung|Die Liste der erkannten Apps, die einem Gerät zugeordnet sind.|
|deviceManagementScripts|[DeviceManagementScript](../resources/intune-devices-devicemanagementscript.md) -Auflistung|Die Liste der Geräte-Verwaltungsskripts den Mandanten zugeordnet.|
|managedDeviceOverview|[managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md)|Geräteübersicht|
|managedDevices|[managedDevice](../resources/intune-devices-manageddevice.md)-Sammlung|Die Liste der verwalteten Geräte|
|remoteActionAudits|[RemoteActionAudit](../resources/intune-devices-remoteactionaudit.md) -Auflistung|Die Liste der Geräte remote Aktion überwacht mit den Mandanten.|
|windowsMalwareInformation|[WindowsMalwareInformation](../resources/intune-devices-windowsmalwareinformation.md) -Auflistung|Die Liste der betroffenen Malware im Mandanten.|
|**Registrierung**|
|depOnboardingSettings|[DepOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) -Auflistung|Diese Auflistungen von mehreren DEP Token pro-Mandanten.|
|importedDeviceIdentities|[ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) -Auflistung|Die importierten Gerät Identitäten.|
|importedWindowsAutopilotDeviceIdentities|[importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md)-Sammlung|Sammlung von importierten Windows Autopilot-Geräten|
|importedWindowsAutopilotDeviceIdentityUploads|[ImportedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) -Auflistung|Auflistung von Windows Autopilot, die Geräte hochladen.|
|windowsAutopilotDeploymentProfiles|[WindowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md) -Auflistung|Windows automatische pilotbereitstellung Profile|
|windowsAutopilotDeviceIdentities|[WindowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) -Auflistung|Die Windows Autopilot Gerät Identitäten, die Auflistung enthalten sind.|
|windowsAutopilotSettings|[windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)|Die Einstellungen der Windows Autopilot-Kontos.|
|**Eingebettete SIM**|
|embeddedSIMActivationCodePools|[EmbeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) -Auflistung|Die eingebettete SIM Aktivierung Code Pools von diesem Konto erstellt wurden.|
|**Zauns**|
|managementConditions|[ManagementCondition](../resources/intune-fencing-managementcondition.md) -Auflistung|Die Verwaltung von Bedingungen Gerätemanagement des Unternehmens zugeordnet.|
|managementConditionStatements|[ManagementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) -Auflistung|Die Bedingung Management Anweisungen Gerätemanagement des Unternehmens zugeordnet.|
|**Benachrichtigungen**|
|notificationMessageTemplates|[notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md)-Sammlung|Benachrichtigungsvorlage|
|**Onboarding**|
|conditionalAccessSettings|[onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md)|Die Exchange-Einstellungen für den lokalen, bedingten Zugriff. Für den lokalen, bedingten Zugriff müssen Geräte registriert und für den E-Mail-Zugriff kompatibel sein.|
|deviceCategories|[deviceCategory](../resources/intune-shared-devicecategory.md)-Sammlung|Die Liste der Gerätekategorien mit dem Mandanten.|
|deviceEnrollmentConfigurations|[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)-Sammlung|Die Liste der Konfigurationen der Geräteregistrierung.|
|deviceManagementPartners|[deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md)-Sammlung|Die Liste der vom Mandanten konfigurierten Geräteverwaltungspartner.|
|exchangeConnectors|[deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md)-Sammlung|Die Liste der vom Mandanten konfigurierten Exchange-Connectors.|
|exchangeOnPremisesPolicies|[DeviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) -Auflistung|Die Liste der durch die Mandanten-konfigurierten Exchange auf Premisis Richtlinien.|
|exchangeOnPremisesPolicy|[deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md)|Die Richtlinie für die mobilen Gerätezugriffs auf lokalen Exchange-Steuerelemente|
|mobileThreatDefenseConnectors|[mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md)-Sammlung|Die Liste der vom Mandanten konfigurierten MTD-Connectors (Mobile Threat Defense).|
|**Remotezugriff**|
|userPfxCertificates|[UserPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) -Auflistung|Die Auflistung der PFX-Zertifikate, die einem Benutzer zugeordnet.|
|**Remoteunterstützung**|
|remoteAssistancePartners|[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md)-Sammlung|Die Partner für die Remoteunterstützung.|
|**Rollenbasierte Zugriffssteuerung (RBAC)**|
|resourceOperations|[resourceOperation](../resources/intune-rbac-resourceoperation.md)-Sammlung|Ressourcenvorgänge|
|roleAssignments|[DeviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md)-Sammlung|Rollenzuweisungen|
|roleDefinitions|[roleDefinition](../resources/intune-rbac-roledefinition.md)-Sammlung|Rollendefinitionen|
|roleScopeTags|[RoleScopeTag](../resources/intune-rbac-rolescopetag.md) -Auflistung|Die Rolle Bereich Tags.|
|**Telekommunikation Ausgaben Management (TEM)**|
|telecomExpenseManagementPartners|[telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md)-Sammlung|Telecom Expense Management-Partner|
|**Problembehandlung**|
|troubleshootingEvents|[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)-Sammlung|Die Liste der Problembehandlungsereignisse für den Mandanten.|
|**Windows-Datenschutz**|
|intuneBrandingProfiles|[IntuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) -Auflistung|Branding Profile Ziel AAD Gruppen Intune|
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



