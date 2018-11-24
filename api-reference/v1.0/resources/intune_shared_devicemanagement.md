# <a name="devicemanagement-resource-type"></a>deviceManagement-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Die Ressource DeviceManagement stellt einen Container, deren Inhalt variieren nach Workflow je, einschließlich:  

- Überwachung der Ereignisse  
- Geschäftsbedingungen im Unternehmen   
- Die Konfiguration für Geräte  
- Geräteverwaltung  
- EndPoint Protection.  
- Registrierung Profile  
- Benachrichtigungen  
- Onboarding-Richtlinien, Einstellungen und details  
- Rollenbasierte Zugriffssteuerung (RBAC) Zugriffsrichtlinien  
- Remoteunterstützung Partner  
- Telekommunikation weite Management-Partner  
- Problembehandlung bei Ereignissen  
- Windows Information Protection Zusammenfassungen  

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[deviceManagement abrufen](../api/intune_shared_devicemanagement_get.md)|[deviceManagement](../resources/intune_shared_devicemanagement.md)|Lesen von Eigenschaften und Beziehungen des [deviceManagement](../resources/intune_shared_devicemanagement.md)-Objekts.|
|[deviceManagement aktualisieren](../api/intune_shared_devicemanagement_update.md)|[deviceManagement](../resources/intune_shared_devicemanagement.md)|Aktualisieren der Eigenschaften eines [deviceManagement](../resources/intune_shared_devicemanagement.md)-Objekts.|
|**Onboarding**|
|[verifyWindowsEnrollmentAutoDiscovery-Funktion](../api/intune_shared_devicemanagement_verifywindowsenrollmentautodiscovery.md)|Boolescher Wert|Noch nicht dokumentiert|
|**RBAC**|
|[GetEffectivePermissions-Funktion](../api/intune_shared_devicemanagement_geteffectivepermissions.md)|["RolePermission"](../resources/intune_rbac_rolepermission.md) Auflistung oder zeichenfolgenauflistung|Ruft die effektiven Berechtigungen des derzeit authentifizierten Benutzers ab.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Eindeutiger Bezeichner für das Gerät.
|
|**deviceConfiguration**|
|settings|[deviceManagementSettings](../resources/intune_deviceconfig_devicemanagementsettings.md)|Einstellungen auf Kontoebene|
|**deviceManagement**|
|subscriptionState|String|Status des Abonnements bei der Lösung für Mobilgeräteverwaltung des Mandanten. Die möglichen Werte sind: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.|
|**Onboarding**|
|intuneBrand|[intuneBrand](../resources/intune_onboarding_intunebrand.md)|„intuneBrand“ enthält Daten, mit denen das Aussehen der Unternehmensportal-Anwendungen und des Endbenutzer-Webportals angepasst wird.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|**Überwachung**|
|auditEvents|[auditEvent](../resources/intune_auditing_auditevent.md)-Sammlung|Audit-Ereignisse|
|**Geschäftsbedingungen im Unternehmen**|
|termsAndConditions|[termsAndConditions](../resources/intune_companyterms_termsandconditions.md)-Sammlung|Die allgemeinen Geschäftsbedingungen für die Geräteverwaltung des Unternehmens.|
|**deviceConfiguration**|
|deviceCompliancePolicies|[deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)-Sammlung|Die Gerätekompatibilitätsrichtlinie|
|deviceCompliancePolicyDeviceStateSummary|[deviceCompliancePolicyDeviceStateSummary](../resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary.md)|Die Gerätekompatibilitäts-Statuszusammenfassung für dieses Konto|
|deviceCompliancePolicySettingStateSummaries|[deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md)-Sammlung|Die Zusammenfassungsstatus von Kompatibilitätsrichtlinieneinstellungen für dieses Konto|
|deviceConfigurationDeviceStateSummaries|[deviceConfigurationDeviceStateSummary](../resources/intune_deviceconfig_deviceconfigurationdevicestatesummary.md)|Die Gerätekonfigurations-Gerätestatuszusammenfassung für dieses Konto.|
|deviceConfigurations|[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)-Sammlung|Die Gerätekonfigurationen|
|iosUpdateStatuses|[iosUpdateDeviceStatus](../resources/intune_deviceconfig_iosupdatedevicestatus.md)-Sammlung|Die IOS-Softwareupdate-Installationsstatus für dieses Konto|
|softwareUpdateStatusSummary|[softwareUpdateStatusSummary](../resources/intune_deviceconfig_softwareupdatestatussummary.md)|Die Softwareaktualisierungs-Statuszusammenfassung|
|**deviceManagement**|
|applePushNotificationCertificate|[applePushNotificationCertificate](../resources/intune_devices_applepushnotificationcertificate.md)|Apple Push Notification-Zertifikat.|
|detectedApps|[detectedApp](../resources/intune_devices_detectedapp.md)-Sammlung|Die Liste der erkannten Apps, die einem Gerät zugeordnet sind.|
|managedDeviceOverview|[managedDeviceOverview](../resources/intune_devices_manageddeviceoverview.md)|Geräteübersicht|
|managedDevices|[managedDevice](../resources/intune_devices_manageddevice.md)-Sammlung|Die Liste der verwalteten Geräte|
|**Registrierung**|
|importedWindowsAutopilotDeviceIdentities|[importedWindowsAutopilotDeviceIdentity](../resources/intune_enrollment_importedwindowsautopilotdeviceidentity.md)-Sammlung|Sammlung von importierten Windows Autopilot-Geräten|
|importedWindowsAutopilotDeviceIdentityUploads|[ImportedWindowsAutopilotDeviceIdentityUpload](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityupload.md) -Auflistung|Auflistung von Windows Autopilot, die Geräte hochladen.|
|**Benachrichtigungen**|
|notificationMessageTemplates|[notificationMessageTemplate](../resources/intune_notification_notificationmessagetemplate.md)-Sammlung|Benachrichtigungsvorlage|
|**Onboarding**|
|conditionalAccessSettings|[onPremisesConditionalAccessSettings](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md)|Die Exchange-Einstellungen für den lokalen, bedingten Zugriff. Für den lokalen, bedingten Zugriff müssen Geräte registriert und für den E-Mail-Zugriff kompatibel sein.|
|deviceCategories|[deviceCategory](../resources/intune_shared_devicecategory.md)-Sammlung|Die Liste der Gerätekategorien mit dem Mandanten.|
|deviceEnrollmentConfigurations|[deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)-Sammlung|Die Liste der Konfigurationen der Geräteregistrierung.|
|deviceManagementPartners|[deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md)-Sammlung|Die Liste der vom Mandanten konfigurierten Geräteverwaltungspartner.|
|exchangeConnectors|[deviceManagementExchangeConnector](../resources/intune_onboarding_devicemanagementexchangeconnector.md)-Sammlung|Die Liste der vom Mandanten konfigurierten Exchange-Connectors.|
|mobileThreatDefenseConnectors|[mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md)-Sammlung|Die Liste der vom Mandanten konfigurierten MTD-Connectors (Mobile Threat Defense).|
|**RBAC**|
|resourceOperations|[resourceOperation](../resources/intune_rbac_resourceoperation.md)-Sammlung|Ressourcenvorgänge|
|roleAssignments|[DeviceAndAppManagementRoleAssignment](../resources/intune_rbac_deviceandappmanagementroleassignment.md)-Sammlung|Rollenzuweisungen|
|roleDefinitions|[roleDefinition](../resources/intune_rbac_roledefinition.md)-Sammlung|Rollendefinitionen|
|**Remoteunterstützung**|
|remoteAssistancePartners|[remoteAssistancePartner](../resources/intune_remoteassistance_remoteassistancepartner.md)-Sammlung|Die Partner für die Remoteunterstützung.|
|**Telekommunikation Ausgaben management**|
|telecomExpenseManagementPartners|[telecomExpenseManagementPartner](../resources/intune_tem_telecomexpensemanagementpartner.md)-Sammlung|Telecom Expense Management-Partner|
|**Problembehandlung**|
|troubleshootingEvents|[deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)-Sammlung|Die Liste der Problembehandlungsereignisse für den Mandanten.|
|**Windows-Datenschutz**|
|windowsInformationProtectionAppLearningSummaries|[windowsInformationProtectionAppLearningSummary](../resources/intune_wip_windowsinformationprotectionapplearningsummary.md)-Sammlung|Windows Information Protection  – App-Schulungszusammenfassung|
|windowsInformationProtectionNetworkLearningSummaries|[windowsInformationProtectionNetworkLearningSummary](../resources/intune_wip_windowsinformationprotectionnetworklearningsummary.md)-Sammlung|Windows Information Protection – Netzwerk-Schulungszusammenfassung|


## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.deviceManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagement",
  "id": "String (identifier)",
  "intuneBrand": {"@odata.type": "microsoft.graph.intuneBrand"},
  "subscriptionState": "String",
  "settings": {"@odata.type": "microsoft.graph.deviceManagementSettings"}
}
```



