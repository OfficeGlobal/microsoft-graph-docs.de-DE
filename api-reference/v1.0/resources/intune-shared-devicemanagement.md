---
title: deviceManagement-Ressourcentyp
description: 'Die deviceManagement-Ressource stellt einen Container dar, dessen Inhalt sich je nach Workflow unterscheidet, einschließlich:  '
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: 08f04242b379fee6ebcc4496e10d342fd3ec342e
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30256035"
---
# <a name="devicemanagement-resource-type"></a>deviceManagement-Ressourcentyp

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Die deviceManagement-Ressource stellt einen Container dar, dessen Inhalt sich je nach Workflow unterscheidet, einschließlich:  

- Überwachungsereignisse  
- Geschäftsbedingungen   
- Geräte Konfigurationseinstellungen  
- Geräteverwaltung  
- Endpunktschutz  
- Registrierungs profile  
- Benachrichtigungen  
- Onboarding-Richtlinien, Einstellungen und Details  
- Rollenbasierte Zugriffssteuerungsrichtlinien  
- Remote Unterstützungspartner  
- Telecom-Ausdehnungs-VERWALTUNGSPARTNER  
- Problembehandlung bei Ereignissen  
- Zusammenfassungen von Windows Information Protection  

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[deviceManagement abrufen](../api/intune-shared-devicemanagement-get.md)|[deviceManagement](../resources/intune-shared-devicemanagement.md)|Lesen von Eigenschaften und Beziehungen des [deviceManagement](../resources/intune-shared-devicemanagement.md)-Objekts.|
|[deviceManagement aktualisieren](../api/intune-shared-devicemanagement-update.md)|[deviceManagement](../resources/intune-shared-devicemanagement.md)|Aktualisieren der Eigenschaften eines [deviceManagement](../resources/intune-shared-devicemanagement.md)-Objekts.|
|**Onboarding**|
|[verifyWindowsEnrollmentAutoDiscovery-Funktion](../api/intune-shared-devicemanagement-verifywindowsenrollmentautodiscovery.md)|Boolescher Wert|Noch nicht dokumentiert|
|**RBAC**|
|[GetEffectivePermissions-Funktion](../api/intune-shared-devicemanagement-geteffectivepermissions.md)|[rolePermission](../resources/intune-rbac-rolepermission.md) -Auflistung oder-Zeichenfolgensammlung|Ruft die effektiven Berechtigungen des derzeit authentifizierten Benutzers ab.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Eindeutiger Bezeichner für das Gerät.
|
|**deviceConfiguration**|
|settings|[deviceManagementSettings](../resources/intune-deviceconfig-devicemanagementsettings.md)|Einstellungen auf Kontoebene|
|**deviceManagement**|
|subscriptionState|String|Status des Abonnements bei der Lösung für Mobilgeräteverwaltung des Mandanten. Mögliche Werte sind: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.|
|**Onboarding**|
|intuneBrand|[intuneBrand](../resources/intune-onboarding-intunebrand.md)|„intuneBrand“ enthält Daten, mit denen das Aussehen der Unternehmensportal-Anwendungen und des Endbenutzer-Webportals angepasst wird.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|**Überwachung**|
|auditEvents|[auditEvent](../resources/intune-auditing-auditevent.md)-Sammlung|Audit-Ereignisse|
|**Geschäftsbedingungen**|
|termsAndConditions|[termsAndConditions](../resources/intune-companyterms-termsandconditions.md)-Sammlung|Die allgemeinen Geschäftsbedingungen für die Geräteverwaltung des Unternehmens.|
|**deviceConfiguration**|
|deviceCompliancePolicies|[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)-Sammlung|Die Gerätekompatibilitätsrichtlinie|
|deviceCompliancePolicyDeviceStateSummary|[deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md)|Die Gerätekompatibilitäts-Statuszusammenfassung für dieses Konto|
|deviceCompliancePolicySettingStateSummaries|[deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md)-Sammlung|Die Zusammenfassungsstatus von Kompatibilitätsrichtlinieneinstellungen für dieses Konto|
|deviceConfigurationDeviceStateSummaries|[deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md)|Die Gerätekonfigurations-Gerätestatuszusammenfassung für dieses Konto.|
|deviceConfigurations|[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)-Sammlung|Die Gerätekonfigurationen|
|iosUpdateStatuses|[iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md)-Sammlung|Die IOS-Softwareupdate-Installationsstatus für dieses Konto|
|softwareUpdateStatusSummary|[softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md)|Die Softwareaktualisierungs-Statuszusammenfassung|
|**deviceManagement**|
|applePushNotificationCertificate|[applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md)|Apple Push Notification-Zertifikat.|
|detectedApps|[detectedApp](../resources/intune-devices-detectedapp.md)-Sammlung|Die Liste der erkannten Apps, die einem Gerät zugeordnet sind.|
|managedDeviceOverview|[managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md)|Geräteübersicht|
|managedDevices|[managedDevice](../resources/intune-devices-manageddevice.md)-Sammlung|Die Liste der verwalteten Geräte|
|**Registrierung**|
|importedWindowsAutopilotDeviceIdentities|[importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md)-Sammlung|Sammlung von importierten Windows Autopilot-Geräten|
|importedWindowsAutopilotDeviceIdentityUploads|[importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) -Sammlung|Sammlung von Windows Autopilot-Geräten hochladen.|
|**Benachrichtigungen**|
|notificationMessageTemplates|[notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md)-Sammlung|Benachrichtigungsvorlage|
|**Onboarding**|
|conditionalAccessSettings|[onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md)|Die Exchange-Einstellungen für den lokalen, bedingten Zugriff. Für den lokalen, bedingten Zugriff müssen Geräte registriert und für den E-Mail-Zugriff kompatibel sein.|
|deviceCategories|[deviceCategory](../resources/intune-shared-devicecategory.md)-Sammlung|Die Liste der Gerätekategorien mit dem Mandanten.|
|deviceEnrollmentConfigurations|[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)-Sammlung|Die Liste der Konfigurationen der Geräteregistrierung.|
|deviceManagementPartners|[deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md)-Sammlung|Die Liste der vom Mandanten konfigurierten Geräteverwaltungspartner.|
|exchangeConnectors|[deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md)-Sammlung|Die Liste der vom Mandanten konfigurierten Exchange-Connectors.|
|mobileThreatDefenseConnectors|[mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md)-Sammlung|Die Liste der vom Mandanten konfigurierten MTD-Connectors (Mobile Threat Defense).|
|**RBAC**|
|resourceOperations|[resourceOperation](../resources/intune-rbac-resourceoperation.md)-Sammlung|Ressourcenvorgänge|
|roleAssignments|[DeviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md)-Sammlung|Rollenzuweisungen|
|roleDefinitions|[roleDefinition](../resources/intune-rbac-roledefinition.md)-Sammlung|Rollendefinitionen|
|**Remote Unterstützung**|
|remoteAssistancePartners|[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md)-Sammlung|Die Partner für die Remoteunterstützung.|
|**Telekom-Spesenverwaltung**|
|telecomExpenseManagementPartners|[telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md)-Sammlung|Telecom Expense Management-Partner|
|**Problembehandlung**|
|troubleshootingEvents|[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)-Sammlung|Die Liste der Problembehandlungsereignisse für den Mandanten.|
|**Windows Information Protection**|
|windowsInformationProtectionAppLearningSummaries|[windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md)-Sammlung|Windows Information Protection  – App-Schulungszusammenfassung|
|windowsInformationProtectionNetworkLearningSummaries|[windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md)-Sammlung|Windows Information Protection – Netzwerk-Schulungszusammenfassung|


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



