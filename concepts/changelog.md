---
title: Änderungsprotokoll für Microsoft Graph
description: Dieses Änderungsprotokoll deckt alle Änderungen in Microsoft Graph ab, einschließlich der Version 1.0 und des Beta-Endpunkts von Microsoft Graph-APIs.
author: jthake-msft
localization_priority: Priority
ms.openlocfilehash: f22796c779e93217cb28da29c333b4ab27e4d5c2
ms.sourcegitcommit: d1a9e7c8e1376a99c5a5416257889ec113613a77
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/07/2019
ms.locfileid: "30458708"
---
# <a name="changelog-for-microsoft-graph"></a>Änderungsprotokoll für Microsoft Graph

Dieses Änderungsprotokoll deckt alle Änderungen in Microsoft Graph ab, einschließlich der Version 1.0 und des Beta-Endpunkts von Microsoft Graph-APIs.

Ausführliche Informationen zu bekannten Problemen mit Microsoft Graph-APIs finden Sie unter [Bekannte Probleme](known-issues.md).

## <a name="march-2019"></a>März 2019

### <a name="directory-apis"></a>Verzeichnis-APIs

| **Änderungstyp** | **Version**   | **Beschreibung**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Ergänzungen | v1.0 | Hinzufügen der Eigenschaften **passwordNotificationWindowInDays** und **passwordValidityPeriodInDays** der Ressource [domain](/graph/api/resources/domain?view=graph-rest-1.0).|
| Ergänzungen | Beta und Version 1.0 | Die Eigenschaften **complianceExpirationDateTime**, **profileType** und **systemLabels** wurden der Ressource [device](/graph/api/resources/device?view=graph-rest-1.0) hinzugefügt.|
| Ergänzungen | Beta und Version 1.0 | Die Eigenschaft **isResourceAccount** wurde der Ressource [user](/graph/api/resources/user?view=graph-rest-1.0) hinzugefügt.|

## <a name="february-2019"></a>Februar 2019

### <a name="dynamics-365-business-central-api"></a>Dynamics 365 Business Central-API

| **Änderungstyp** | **Version**   | **Beschreibung**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Ergänzungen        | Beta          | Finanz-APIs für Dynamics 365 Business Central wurden hinzugefügt. Einzelheiten hierzu finden Sie in der [Finanz-API-Referenz](/graph/api/resources/dynamics-graph-reference?view=graph-rest-v1.0).|


## <a name="february-2019"></a>Februar 2019

### <a name="directory-apis"></a>Verzeichnis-APIs

| **Änderungstyp** | **Version**   | **Beschreibung**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Ergänzungen | v1.0 | Neuer Ressourcentyp [DirectoryObjectPartnerReference](/graph/api/resources/directoryobjectpartnerreference?view=graph-rest-1.0) hinzugefügt. |
| Ergänzungen | Beta und Version 1.0 | Die Eigenschaft **createdDateTime** wurde zu [organization](/graph/api/resources/organization?view=graph-rest-1.0) hinzugefügt. |
| Änderung | Beta und Version 1.0 | Die Eigenschaft **companyName** der Ressource [user](/graph/api/resources/user?view=graph-rest-1.0) wurde aktualisiert, um beschreibbar zu sein. |
| Änderung | Beta | Der Typ [targetResource](/graph/api/resources/targetresource?view=graph-rest-beta) enthält nun Eigenschaften, die zuvor für abgeleitete Typen verfügbar waren, die nicht mehr unterstützt werden. |
| Löschung | Beta | Die folgenden abgeleiteten Typen werden nicht mehr unterstützt und wurden entfernt: **targetResourceDevice**, **targetResourceDirectory**, **targetResourceGroup**, **targetResourcePolicy**, **targetResourceRole**, **targetResourceServicePrincipal**, **targetResourceUser** und **targetResourceOther**. |
| Ergänzungen |Beta | Hinzufügen der Eigenschaften **passwordNotificationWindowInDays** und **passwordValidityPeriodInDays** der Ressource [domain](/graph/api/resources/domain?view=graph-rest-beta).|

### <a name="education-apis"></a>Bildungs-APIs

| **Änderungstyp** | **Version**   | **Beschreibung**                          |
| :-------------- | :------------ | :--------------------------------------- |
|Ergänzungen |Beta|Neue relatedContacts Eigenschaft für [educationUser](/graph/api/resources/educationUser?view=graph-rest-beta) eingeführt.|
|Ergänzungen |v1.0|Neue relatedContacts Eigenschaft für [educationUser](/graph/api/resources/educationUser?view=graph-rest-v1.0) eingeführt.|

### <a name="microsoft-intune-apis"></a>Microsoft Intune-APIs

|Änderungstyp|Version|Beschreibung|
|:---|:---|:---|
|Ergänzungen|Beta|Hinzugefügte neue Entitäten:<br/>[androidOmaCpConfiguration](/graph/api/resources/intune-deviceconfig-androidomacpconfiguration?view=graph-rest-beta)<br/>[managedDeviceEncryptionState](/graph/api/resources/intune-deviceconfig-manageddeviceencryptionstate?view=graph-rest-beta)<br/>|
|Ergänzung|Beta|Die folgenden komplexen Typen wurden hinzugefügt:<br/>[deliveryOptimizationBandwidth](/graph/api/resources/intune-deviceconfig-deliveryoptimizationbandwidth?view=graph-rest-beta)<br/>[deliveryOptimizationBandwidthAbsolute](/graph/api/resources/intune-deviceconfig-deliveryoptimizationbandwidthabsolute?view=graph-rest-beta)<br/>[deliveryOptimizationBandwidthBusinessHoursLimit](/graph/api/resources/intune-deviceconfig-deliveryoptimizationbandwidthbusinesshourslimit?view=graph-rest-beta)<br/>[deliveryOptimizationBandwidthHoursWithPercentage](/graph/api/resources/intune-deviceconfig-deliveryoptimizationbandwidthhourswithpercentage?view=graph-rest-beta)<br/>[deliveryOptimizationBandwidthPercentage](/graph/api/resources/intune-deviceconfig-deliveryoptimizationbandwidthpercentage?view=graph-rest-beta)<br/>[deliveryOptimizationGroupIdCustom](/graph/api/resources/intune-deviceconfig-deliveryoptimizationgroupidcustom?view=graph-rest-beta)<br/>[deliveryOptimizationGroupIdSource](/graph/api/resources/intune-deviceconfig-deliveryoptimizationgroupidsource?view=graph-rest-beta)<br/>[deliveryOptimizationGroupIdSourceOptions](/graph/api/resources/intune-deviceconfig-deliveryoptimizationgroupidsourceoptions?view=graph-rest-beta)<br/>[deliveryOptimizationMaxCacheSize](/graph/api/resources/intune-deviceconfig-deliveryoptimizationmaxcachesize?view=graph-rest-beta)<br/>[deliveryOptimizationMaxCacheSizeAbsolute](/graph/api/resources/intune-deviceconfig-deliveryoptimizationmaxcachesizeabsolute?view=graph-rest-beta)<br/>[deliveryOptimizationMaxCacheSizePercentage](/graph/api/resources/intune-deviceconfig-deliveryoptimizationmaxcachesizepercentage?view=graph-rest-beta)<br/>[encryptionReportPolicyDetails](/graph/api/resources/intune-deviceconfig-encryptionreportpolicydetails?view=graph-rest-beta)<br/>|
|Ergänzung|Beta|Neue Enumerationstypen hinzugefügt:<br/>[advancedBitLockerState](/graph/api/resources/intune-deviceconfig-advancedbitlockerstate?view=graph-rest-beta)<br/>[deliveryOptimizationGroupIdOptionsType](/graph/api/resources/intune-deviceconfig-deliveryoptimizationgroupidoptionstype?view=graph-rest-beta)<br/>[deliveryOptimizationRestrictPeerSelectionByOptions](/graph/api/resources/intune-deviceconfig-deliveryoptimizationrestrictpeerselectionbyoptions?view=graph-rest-beta)<br/>[deviceTypes](/graph/api/resources/intune-deviceconfig-devicetypes?view=graph-rest-beta)<br/>[edgeKioskModeRestrictionType](/graph/api/resources/intune-deviceconfig-edgekioskmoderestrictiontype?view=graph-rest-beta)<br/>[encryptionReadinessState](/graph/api/resources/intune-deviceconfig-encryptionreadinessstate?view=graph-rest-beta)<br/>[encryptionState](/graph/api/resources/intune-deviceconfig-encryptionstate?view=graph-rest-beta)<br/>|
|Ergänzung|Beta|Eigenschaft **roleScopeTagIds** zur Entität [depOnboardingSetting](/graph/api/resources/intune-enrollment-deponboardingsetting?view=graph-rest-beta) hinzugefügt|
|Ergänzung|Beta|Eigenschaften **autoFillForceAuthentication**, **cellularBlockPlanModification**, **classroomForceAutomaticallyJoinClasses**, **classroomForceUnpromptedAppAndDeviceLock**, **esimBlockModification**, **proximityBlockSetupToNewDevice**, **softwareUpdatesEnforcedDelayInDays** und **softwareUpdatesForceDelayed** zur Entität [iosGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-iosgeneraldeviceconfiguration?view=graph-rest-beta) hinzugefügt|
|Ergänzung|Beta|Eigenschaften **softwareUpdatesEnforcedDelayInDays**, **softwareUpdatesForceDelayed** und **contentCachingBlocked** zur Entität [macOSGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-macosgeneraldeviceconfiguration?view=graph-rest-beta) hinzugefügt|
|Ergänzung|Beta|Eigenschaft **licensingType** zur Entität [microsoftStoreForBusinessApp](/graph/api/resources/intune-apps-microsoftstoreforbusinessapp?view=graph-rest-beta) hinzugefügt|
|Ergänzung|Beta|Eigenschaften **defenderSecurityCenterDisableClearTpmUI**, **defenderSecurityCenterDisableNotificationAreaUI**, **defenderSecurityCenterDisableVulnerableTpmFirmwareUpdateUI**, **defenderAdobeReaderLaunchChildProcess** und **defenderOfficeCommunicationAppsLaunchChildProcess** zur Entität [windows10EndpointProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windows10endpointprotectionconfiguration?view=graph-rest-beta) hinzugefügt|
|Ergänzung|Beta|Eigenschaften **edgeKioskModeRestriction**, **edgeKioskResetAfterIdleTimeInMinutes**, **defenderScheduleScanEnableLowCpuPriority**, **defenderDisableCatchupQuickScan**, **defenderDisableCatchupFullScan** und **edgeBlockSearchEngineCustomization** zur Entität [windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta) hinzugefügt|
|Ergänzung|Beta|Eigenschaft **enableWhiteGlove** zur Entität [windowsAutopilotDeploymentProfile](/graph/api/resources/intune-enrollment-windowsautopilotdeploymentprofile?view=graph-rest-beta) hinzugefügt|
|Ergänzung|Beta|Eigenschaften **restrictPeerSelectionBy**, **groupIdSource**, **bandwidthMode**, **backgroundDownloadFromHttpDelayInSeconds**, **foregroundDownloadFromHttpDelayInSeconds**, **minimumRamAllowedToPeerInGigabytes**, **minimumDiskSizeAllowedToPeerInGigabytes**, **minimumFileSizeToCacheInMegabytes**, **minimumBatteryPercentageAllowedToUpload**, **modifyCacheLocation**, **maximumCacheAgeInDays**, **maximumCacheSize** und **vpnPeerCaching** zur Entität [windowsDeliveryOptimizationConfiguration](/graph/api/resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration?view=graph-rest-beta) hinzugefügt|
|Ergänzung|Beta|Eigenschaft **lastCheckInDateTime** zur Entität [windowsInformationProtectionWipeAction](/graph/api/resources/intune-mam-windowsinformationprotectionwipeaction?view=graph-rest-beta) hinzugefügt|
|Ergänzung|Beta|Navigationseigenschaft **managedDeviceEncryptionStates** zur Entität [deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-beta) hinzugefügt|
|Ergänzung|Beta|Eigenschaften **endpointProtection** und **officeApps** zum komplexen Typ [configurationManagerClientEnabledFeatures](/graph/api/resources/intune-devices-configurationmanagerclientenabledfeatures?view=graph-rest-beta) hinzugefügt|
|Ergänzung|Beta|Eigenschaften **productName** und **publisher** zum komplexen Typ [win32LobAppMsiInformation](/graph/api/resources/intune-apps-win32lobappmsiinformation?view=graph-rest-beta) hinzugefügt|
|Ergänzung|Beta|Member **warn** zum Enumerationstyp [managedAppRemediationAction](/graph/api/resources/intune-mam-managedappremediationaction?view=graph-rest-beta) hinzugefügt|

### <a name="microsoft-teams-apis"></a>Microsoft Teams-APIs

| **Änderungstyp** | **Version**   | **Beschreibung**                          |
| :-------------- | :------------ | :--------------------------------------- |
|Ergänzungen |Beta und Version 1.0| Die **internalId**-Eigenschaft wurde zur [team](/graph/api/resources/team?view=graph-rest-v1.0)-Ressource hinzugefügt.|
|Ergänzungen |Beta und Version 1.0| Zusätzliche Unterstützung für die Konfiguration von [Registerkarten](teams-configuring-builtin-tabs.md) für Word, Excel, PowerPoint, PDF und Dokumentbibliotheken. |
|Ergänzungen |Beta| Die API [Senden einer Nachricht an einen Kanal](/graph/api/channel-post-chatmessage?view=graph-rest-beta) wurde eingeführt. |
|Ergänzungen |Beta| Die API [Antworten auf eine Nachricht in einem Kanal](/graph/api/channel-post-messagereply?view=graph-rest-beta) wurde eingeführt. |
|Löschung |Beta| POST /teams/{Id}/channels/{Id}/chatThreads API entfernt. Verwenden Sie stattdessen [Erstellen einer Nachricht in einem Kanal](/graph/api/channel-post-chatmessage?view=graph-rest-beta). |
|Ergänzungen |Beta | Unterstützung für Anwendungsberechtigungen wurde zur Ressource [installedApps](/graph/api/resources/teamsappinstallation?view=graph-rest-beta) hinzugefügt.|

### <a name="onenote"></a>OneNote

| **Änderungstyp** | **Version**   | **Beschreibung**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Ergänzungen        | Beta und Version 1.0 | Die [getNotebookFromWebUrl](/graph/api/notebook-getnotebookfromweburl?view=graph-rest-1.0)-Methode wurde hinzugefügt. |

### <a name="outlook-calendar"></a>Outlook-Kalender

| **Änderungstyp** | **Version**   | **Beschreibung**                          |
| :-------------- | :------------ | :--------------------------------------- |
|Änderung | Beta | Der Datentyp folgender Parameter von [findMeetingTimes](/graph/api/user-findmeetingtimes?view=graph-rest-beta) wurde geändert: <br>**attendees**: von **attendeeBase** auf [attendeeDataModel](/graph/api/resources/attendeedatamodel?view=graph-rest-beta) <br>**locationConstraint**: von **locationConstraint** auf [locationConstraints](/graph/api/resources/locationconstraints?view=graph-rest-beta) <br> **timeConstraint**: von **timeConstraint** auf [findMeetingTimesTimeConstraints](/graph/api/resources/findmeetingtimestimeconstraints?view=graph-rest-beta)|
|Änderung | Beta | Der Rückgabetyp von **findMeetingTimes** wurde von **meetingTimeSuggestionsResult** auf [findMeetingTimesResponse](/graph/api/resources/findmeetingtimesresponse?view=graph-rest-beta) geändert |
|Änderung | Beta | Die Antwortnutzlast von **findMeetingTimes** wurde geändert, um den **type** jedes Teilnehmers auszuschließen, der angibt, ob der Teilnehmer erforderlich, optional oder eine Ressource ist |
|Änderung | Beta | Basistyp von [locationConstraintItem](/graph/api/resources/locationconstraintitem?view=graph-rest-beta) wurde von [location](/graph/api/resources/location?view=graph-rest-beta) auf [locationDataModel](/graph/api/resources/locationdatamodel?view=graph-rest-beta) geändert |
|Änderung | Beta | Die Datentypen der folgenden Eigenschaften von [meetingTimeSuggestion](/graph/api/resources/meetingtimesuggestion?view=graph-rest-beta) wurden geändert: <br> **attendeeAvailability**: von Sammlung von **attendeeAvailability** auf Sammlung von [attendeeAvailabilityDataModel](/graph/api/resources/attendeeavailabilitydatamodel?view=graph-rest-beta) <br> **locations**: von Sammlung von [location](/graph/api/resources/location?view=graph-rest-beta) auf Sammlung von [locationDataModel](/graph/api/resources/locationdatamodel?view=graph-rest-beta) <br> **meetingTimeSlot**: von [timeSlot](/graph/api/resources/timeslot?view=graph-rest-beta) auf [meetingTimeSlotDataModel](/graph/api/resources/meetingtimeslotdatamodel?view=graph-rest-beta) <br> **organizerAvailability**: von **freeBusyStatus** auf **availabilityStatus** |
|Ergänzungen | Beta | Neue komplexe Typen: <br> [attendeeAvailabilityDataModel](/graph/api/resources/attendeeavailabilitydatamodel?view=graph-rest-beta) <br> [attendeeDataModel](/graph/api/resources/attendeedatamodel?view=graph-rest-beta) <br> [findMeetingTimesResponse](/graph/api/resources/findmeetingtimesresponse?view=graph-rest-beta) <br> [findMeetingTimesTimeConstraints](/graph/api/resources/findmeetingtimestimeconstraints?view=graph-rest-beta) <br> [locationConstraints](/graph/api/resources/locationconstraints?view=graph-rest-beta) <br> [locationDataModel](/graph/api/resources/locationdatamodel?view=graph-rest-beta) <br> [meetingTimeSlotDataModel](/graph/api/resources/meetingtimeslotdatamodel?view=graph-rest-beta) <br> [postalAddress](/graph/api/resources/postaladdress?view=graph-rest-beta) <br> [searchWindowTimeSlot](/graph/api/resources/searchwindowtimeslot?view=graph-rest-beta)|
|Ergänzungen | Beta | Neue Aufzählungen: <br> **addressType** <br> **availabilityStatus** |
|Ergänzungen | Beta | Die **order**-Eigenschaft wurde [meetingTimeSuggestion](/graph/api/resources/meetingtimesuggestion?view=graph-rest-beta) hinzugefügt |
|Löschung | Beta | Die folgenden komplexen Typen wurden entfernt: <br> **attendeeAvailability** <br> **locationConstraint** <br> **meetingTimeSuggestionsResult** <br>**timeConstraint** |

### <a name="security-apis"></a>Sicherheits-APIs

| **Änderungstyp** | **Version** | **Beschreibung**              |
| :-------------- | :---------- | :--------------------------------------- |
| Ergänzungen        | Beta       | Threat Intelligence-Indikator-APIs wurden zur [Sicherheits-API](/graph/api/resources/security-api-overview?view=graph-rest-beta) hinzugefügt, einschließlich der folgenden Ressourcen und Operationen:<br/>[tiIndicator](/graph/api/resources/tiindicator?view=graph-rest-beta) (und verknüpfte Entitäten)<br/> [Get tiIndicator](/graph/api/tiindicator-get?view=graph-rest-beta)<br/>[Create tiIndicator](/graph/api/tiindicators-post?view=graph-rest-beta)<br/>[List tiIndicators](/graph/api/tiindicators-list?view=graph-rest-beta)<br/>[Update tiIndicator](/graph/api/tiindicator-update?view=graph-rest-beta) <br/>[Delete tiIndicator](/graph/api/tiindicator-delete?view=graph-rest-beta) <br/>[deleteTiIndicators](/graph/api/tiindicator-deletetiindicators?view=graph-rest-beta) <br/>[deleteTiIndicatorsByExternalId](/graph/api/tiindicator-deletetiindicatorsbyexternalid?view=graph-rest-beta) <br/>[submitTiIndicators](/graph/api/tiindicator-submittiindicators?view=graph-rest-beta) <br/>[updateTiIndicators](/graph/api/tiindicator-updatetiindicators?view=graph-rest-beta)|
| Ergänzungen        | Beta       | Sicherheitsaktionen-APIs wurden zur [Sicherheits-API](/graph/api/resources/security-api-overview?view=graph-rest-beta) hinzugefügt, einschließlich der folgenden Ressourcen und Operationen:<br/>[SecurityAction](/graph/api/resources/securityaction?view=graph-rest-beta) (und verknüpften Entitäten)<br/> [Get securityAction](/graph/api/securityaction-get?view=graph-rest-beta)<br/>[Create securityAction](/graph/api/securityactions-post?view=graph-rest-beta)<br/>[List securityAction](/graph/api/securityactions-list?view=graph-rest-beta)<br/>[Cancel securityAction](/graph/api/securityaction-cancelsecurityaction?view=graph-rest-beta)
| Ergänzungen        | Beta        | Neue Sammlung [historyStates](/graph/api/resources/alerthistorystate?view=graph-rest-beta) vom komplexen Typ für Warnungen wurde eingeführt. </br>Funktion [UpdateAlerts](/graph/api/alert-updatealerts?view=graph-rest-beta) wurde hinzugefügt, um mehrere Warnungen in einer Anforderung zu aktualisieren. |

## <a name="january-2019"></a>Januar 2019

### <a name="azure-ad-apis"></a>Azure AD-APIs

| **Änderungstyp** | **Version**   | **Beschreibung**                          |
| :-------------- | :------------ | :--------------------------------------- |
|Ergänzungen |v1.0|Der neue Ressourcentyp für die [identityProvider](/graph/api/resources/identityprovider?view=graph-rest-v1.0)-Entität und die Vorgänge [create](/graph/api/identityprovider-post-identityproviders?view=graph-rest-v1.0), [list](/graph/api/identityprovider-list?view=graph-rest-v1.0), [get](/graph/api/identityprovider-get?view=graph-rest-v1.0), [update](/graph/api/identityprovider-update?view=graph-rest-v1.0) und [delete](/graph/api/identityprovider-delete?view=graph-rest-v1.0) wurden hinzugefügt.|

### <a name="directory-apis"></a>Verzeichnis-APIs

| **Änderungstyp** | **Version**   | **Beschreibung**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Ergänzungen | v1.0 | Neue Methode „transitiveMembers“ für [groups](/graph/api/group-list-transitivemembers?view=graph-rest-1.0) hinzugefügt. Diese Methode gibt eine flache Liste der Member einschließlich geschachtelter Member zurück.|
| Ergänzungen | v1.0 | Neue Methode „transitiveMemberOf“ für [users](/graph/api/user-list-transitivemembersof?view=graph-rest-1.0), [groups](/graph/api/group-list-transitivemembersof?view=graph-rest-beta) und [devices](/graph/api/device-list-transitivemembersof?view=graph-rest-1.0) hinzugefügt.|
| Ergänzungen | v1.0 | Neue Eigenschaften für [users](/graph/api/resources/user?view=graph-rest-1.0): **employeeId**, **faxNumber**, **onPremisesDistinguishedName**, **showInAddressList** und **otherMails** hinzugefügt.|
| Ergänzungen | v1.0 | Eigenschaft **forceChangePasswordNextSignInWithMfa** zum komplexen Typ [passwordProfile](/graph/api/resources/passwordprofile?view=graph-rest-v1.0) hinzugefügt.|
| Ergänzungen | v1.0 | Eigenschaft **licenseAssignmentStates** zur Entität [User](/graph/api/resources/user?view=graph-rest-1.0) für [Gruppenbasierte Lizenzierung](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-licensing-whatis-azure-portal) hinzugefügt.|
| Ergänzungen | v1.0 | Ressource **licenseAssignmentState** für [Gruppenbasierte Lizenzierung](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-licensing-whatis-azure-portal) hinzugefügt.| 
| Ergänzungen | v1.0 | Eigenschaften **assignedLicenses**, **licenseProcessingState**, **hasMembersWithLicenseErrors** und die Beziehung **membersWithLicenseErrors** wurden zur Entität [Group](/graph/api/resources/group?view=graph-rest-1.0) für [Gruppenbasierte Lizenzierung](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-licensing-whatis-azure-portal) hinzugefügt.|
| Ergänzungen | Beta | Eigenschaft **createdDateTime** wurde zur [user](/graph/api/resources/user?view=graph-rest-beta)-Ressource hinzugefügt.|

### <a name="microsoft-intune-apis"></a>Microsoft Intune-APIs

|Änderungstyp|Version|Beschreibung|
|:---|:---|:---|
|Ergänzungen|Beta|Hinzugefügte neue Entitäten:<br/>[appleVppTokenTroubleshootingEvent](/graph/api/resources/intune-troubleshooting-applevpptokentroubleshootingevent?view=graph-rest-beta)<br/>[appLogCollectionRequest](/graph/api/resources/intune-devices-applogcollectionrequest?view=graph-rest-beta)<br/>[windowsUpdateState](/graph/api/resources/intune-deviceconfig-windowsupdatestate?view=graph-rest-beta)<br/>|
|Ergänzungen|Beta|Die folgenden komplexen Typen wurden hinzugefügt:<br/>[appLogCollectionDownloadDetails](/graph/api/resources/intune-devices-applogcollectiondownloaddetails?view=graph-rest-beta)<br/>**deviceManagementTroubleshootingErrorDetails**<br/>[deviceManagementTroubleshootingErrorResource](/graph/api/resources/intune-troubleshooting-devicemanagementtroubleshootingerrorresource?view=graph-rest-beta)<br/>[win32LobAppAssignmentSettings](/graph/api/resources/intune-apps-win32lobappassignmentsettings?view=graph-rest-beta)<br/>|
|Ergänzungen|Beta|Neue Enumerationstypen hinzugefügt:<br/>[appLogDecryptionAlgorithm](/graph/api/resources/intune-devices-applogdecryptionalgorithm?view=graph-rest-beta)<br/>[appLogUploadState](/graph/api/resources/intune-devices-apploguploadstate?view=graph-rest-beta)<br/>[win32LobAppNotification](/graph/api/resources/intune-apps-win32lobappnotification?view=graph-rest-beta)<br/>[windowsUpdateStatus](/graph/api/resources/intune-deviceconfig-windowsupdatestatus?view=graph-rest-beta)<br/>|
|Ergänzungen|Beta|Aktion **createDownloadUrl** für [appLogCollectionRequest](/graph/api/resources/intune-devices-applogcollectionrequest?view=graph-rest-beta) hinzugefügt |
|Löschung|Beta|Die folgenden Entitäten wurden entfernt:<br/>**deviceManagementApplicabilityRuleOsEdition**<br/>**deviceManagementApplicabilityRuleOsVersion**<br/>|
|Ergänzungen|Beta|Eigenschaft **passwordSignInFailureCountBeforeFactoryReset** wurde zur Entität [androidCompliancePolicy](/graph/api/resources/intune-deviceconfig-androidcompliancepolicy?view=graph-rest-beta) hinzugefügt|
|Ergänzungen|Beta|Eigenschaft **passwordSignInFailureCountBeforeFactoryReset** wurde zur Entität [androidForWorkCompliancePolicy](/graph/api/resources/intune-deviceconfig-androidforworkcompliancepolicy?view=graph-rest-beta) hinzugefügt|
|Ergänzungen|Beta|Eigenschaft **passwordSignInFailureCountBeforeFactoryReset** wurde zur Entität [androidWorkProfileCompliancePolicy](/graph/api/resources/intune-deviceconfig-androidworkprofilecompliancepolicy?view=graph-rest-beta) hinzugefügt|
|Löschung|Beta|Eigenschaft **defaultProfileDisplayName** wurde aus der Entität [depOnboardingSetting](/graph/api/resources/intune-enrollment-deponboardingsetting?view=graph-rest-beta) entfernt|
|Ergänzungen|Beta|Eigenschaft **runAs32Bit** wurde zur Entität [deviceManagementScript](/graph/api/resources/intune-devices-devicemanagementscript?view=graph-rest-beta) hinzugefügt|
|Ergänzungen|Beta|Eigenschaften **troubleshootingErrorDetails**, **eventName** and **additionalInformation** wurden zur Entität [deviceManagementTroubleshootingEvent](/graph/api/resources/intune-troubleshooting-devicemanagementtroubleshootingevent?view=graph-rest-beta) hinzugefügt|
|Änderung|Beta|Die folgenden Eigenschaften für die Entität [macOSCertificateProfileBase](/graph/api/resources/intune-deviceconfig-macoscertificateprofilebase?view=graph-rest-beta) wurden geändert:<br/>**subjectAlternativeNameType** von erforderlich in optional<br/>|
|Ergänzungen|Beta|Eigenschaften **certificateStore** und **customSubjectAlternativeNames** wurden zur Entität [macOSScepCertificateProfile](/graph/api/resources/intune-deviceconfig-macosscepcertificateprofile?view=graph-rest-beta) hinzugefügt|
|Ergänzungen|Beta|Eigenschaft **officeConfigurationXml** wurde zur Entität [officeSuiteApp](/graph/api/resources/intune-apps-officesuiteapp?view=graph-rest-beta) hinzugefügt|
|Ergänzungen|Beta|Eigenschaft **createdDateTime** wurde zur Entität [organization](/graph/api/resources/intune-onboarding-organization?view=graph-rest-beta) hinzugefügt|
|Ergänzungen|Beta|Eigenschaft **bitLockerAllowStandardUserEncryption** wurde zur Entität [windows10EndpointProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windows10endpointprotectionconfiguration?view=graph-rest-beta) hinzugefügt|
|Löschung|Beta|Eigenschaften **localSecurityOptionsEnableAdministratorAccount**, **localSecurityOptionsEnableGuestAccount** und **lanManagerWorkstationEnableInsecureGuestLogons** wurden aus der Entität [windows10EndpointProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windows10endpointprotectionconfiguration?view=graph-rest-beta) entfernt|
|Ergänzungen|Beta|Eigenschaft **useSecurityKeyForSignin** wurde zur Entität [windowsIdentityProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windowsidentityprotectionconfiguration?view=graph-rest-beta) hinzugefügt|
|Ergänzungen|Beta|Navigationseigenschaft **mobileAppTroubleshootingEvents** wurde zur Entität [deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-beta) hinzugefügt|
|Ergänzungen|Beta|Navigationseigenschaft **appLogCollectionRequests** wurde zur Entität [mobileAppTroubleshootingEvent](/graph/api/resources/intune-devices-mobileapptroubleshootingevent?view=graph-rest-beta) hinzugefügt|

### <a name="microsoft-teams-apis"></a>Microsoft Teams-APIs

| **Änderungstyp** | **Version**   | **Beschreibung**                          |
| :-------------- | :------------ | :--------------------------------------- |
|Ergänzungen |Beta| educationStandard, educationClass, educationProfessionalLearningCommunity, educationStaff und unknownFutureValue wurde der [teamSpecialization](/graph/api/resources/teamspecialization?view=graph-rest-beta)-Enumeration hinzugefügt.|

### <a name="reports-apis"></a>Bericht-APIs

| **Änderungstyp** | **Version** | **Beschreibung**                  |
|:----------------|:------------|:-----------------------------------------|
| Ergänzungen        | Beta  | Eigenschaften **office365Active** und **office365Inactive** zu Entität [office365ServicesUserCounts](/graph/api/resources/office365ServicesUserCounts?view=graph-rest-beta) hinzugefügt.|

## <a name="december-2018"></a>Dezember 2018

### <a name="data-policy-api"></a>Datenrichtlinien-API

| **Änderungstyp** | **Version** | **Beschreibung**                          |
| :-------------- | :---------- | :--------------------------------------- |
|Ergänzungen |v1.0| Added new entity [dataPolicyOperation](/graph/api/resources/datapolicyoperation?view=graph-rest-1.0). This represents a submitted data policy operation for tracking purposes.
|Ergänzungen |v1.0| Added the [exportPersonalData](/graph/api/user-exportpersonaldata?view=graph-rest-1.0) action on [users](/graph/api/resources/users?view=graph-rest-1.0). This action submits a data policy operation request to export personal data stored by Microsoft for a user. |
|Ergänzungen |v1.0| Die Methode [dataPolicyOperations](/graph/api/datapolicyoperation-get?view=graph-rest-1.0) wurde hinzugefügt. Diese ruft Eigenschaften vom dataPolicyOperation-Objekt ab.|

### <a name="directory-apis"></a>Verzeichnis-APIs

| **Änderungstyp** | **Version**   | **Beschreibung**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Ergänzungen | Beta | Neue `expirationDateTime`-Eigenschaft wurde zu [Gruppen](https://docs.microsoft.com/en-us/graph/api/group-list-transitivemembers?view=graph-rest-beta) für den [Gruppenablauf](https://docs.microsoft.com/de-DE/azure/active-directory/users-groups-roles/groups-lifecycle) hinzugefügt.|
| Ergänzungen | Beta | Neuer Ressourcentyp [DirectoryObjectPartnerReference](/graph/api/resources/directoryobjectpartnerreference?view=graph-rest-beta) hinzugefügt.|
| Ergänzungen | Beta | Eigenschaft `createdDateTime` zur Ressource [organization](/graph/api/resources/organization?view=graph-rest-beta) hinzugefügt.|
| Ergänzung | v1.0 | Methode `memberOf` hinzugefügt, um die direkte [Mitgliedschaft](/graph/api/device-list-memberOf?view=graph-rest-1.0) eines [Geräts](/graph/api/resources/device?view=graph-rest-1.0) abzurufen. Diese Methode wurde zum Abrufen der Liste der Mitgliedschaften einschließlich geschachtelter Mitgliedschaften hinzugefügt.|
| Änderung    | Beta | Die Ressource [Organisationskontakte](/graph/api/resources/orgcontact?view=graph-rest-beta) wurde umstrukturiert. Die physischen Adresseigenschaften (`city`, `country`, `postalCode`, `streetAddress` und `state`) sowie `officeLocation` sind nun in einer `addresses`-Auflistung (des neuen Ressourcentyps [physicalOfficeAddress](/graph/api/resources/physicalofficeaddress?view=graph-rest-beta)) und `mobilePhone` enthalten, `businessPhones` und `faxNumber` sind nun in einer `phones`-Auflistung vorhanden. `companyName` und `imAddresses` wurden ebenfalls hinzugefügt.|

### <a name="microsoft-teams-apis"></a>Microsoft Teams-APIs

| **Änderungstyp** | **Version**   | **Beschreibung**                          |
| :-------------- | :------------ | :--------------------------------------- |
|Ergänzungen |Beta| Neuer Ressourcentyp [teamsTemplate](/graph/api/resources/teamstemplate?view=graph-rest-beta) eingeführt.|
|Ergänzung |Beta| Neuer Ressourcentyp [teamSpecialization](/graph/api/resources/teamspecialization?view=graph-rest-beta) eingeführt.|
|Ergänzung |Beta| Eigenschaften „isFavoriteByDefault“, „mail“ und „webUrl“ zu [channel](/graph/api/resources/channel?view=graph-rest-beta) hinzugefügt.|
|Ergänzung |Beta| Eigenschaft „displayName“ zu [team](/graph/api/resources/team?view=graph-rest-beta) hinzugefügt.|
|Ergänzung |Beta| Eigenschaft „description“ zu [team](/graph/api/resources/team?view=graph-rest-beta) hinzugefügt.|
|Ergänzung |Beta| Eigenschaft „classification“ zu [team](/graph/api/resources/team?view=graph-rest-beta) hinzugefügt.|
|Ergänzung |Beta| Eigenschaft [specialization](/graph/api/resources/teamspecialization?view=graph-rest-beta) zu [team](/graph/api/resources/team?view=graph-rest-beta) hinzugefügt.|
|Ergänzung |Beta| Eigenschaft [visibility](/graph/api/resources/teamvisibilitytype?view=graph-rest-beta) zu [team](/graph/api/resources/team?view=graph-rest-beta) hinzugefügt.|
|Ergänzung |Beta| Eigenschaft [template](/graph/api/resources/teamstemplate?view=graph-rest-beta) zu [team](/graph/api/resources/team?view=graph-rest-beta) hinzugefügt.|
|Ergänzung |Beta| Sammlung „owners“ zu [team](/graph/api/resources/team?view=graph-rest-beta) hinzugefügt.|
|Ergänzung |Beta| Neuer Enumerationsmember „unknownFutureValue“ in „teamVisibilityType“ eingeführt.|
|Ergänzung |Beta| Neuer Enumerationsmember „unknownFutureValue“ in „giphyRatingType“ eingeführt.|
|Ergänzung |Beta| Neuer Enumerationsmember „unknownFutureValue“ in „teamsAsyncOperationType“ eingeführt.|
|Ergänzung |Beta| Neuer Enumerationsmember „unknownFutureValue“ in „teamsAsyncOperationStatus“ eingeführt.|
|Ergänzung |Beta| Neuer Enumerationsmember „unknownFutureValue“ in „teamsAppDistributionMethod“ eingeführt.|
|Ergänzung |Beta| Neuer Ressourcentyp [/teamsTemplates](/graph/api/resources/teamstemplate?view=graph-rest-beta) eingeführt.|
|Ergänzungen | v1.0 | Unterstützung für Administratorberechtigungen für [team](/graph/api/resources/team?view=graph-rest-1.0), [channel](/graph/api/resources/channel?view=graph-rest-1.0) und [tab](/graph/api/resources/teamstab?view=graph-rest-1.0)-Vorgänge hinzugefügt. |

### <a name="privileged-identity-management-apis"></a>Privileged Identity Management-APIs

| **Änderungstyp** | **Version**   | **Beschreibung**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Ergänzungen | Beta | Eigenschaft `registeredRoot` zu Entität [governanceResource](/graph/api/resources/governanceresource?view=graph-rest-beta) hinzugefügt.|
| Änderung | Beta | Eigenschaft `onboardDateTime` der Entität [governanceResource](/graph/api/resources/governanceresource?view=graph-rest-beta) in `registeredDateTime` umbenannt.|
| Ergänzung | Beta | Neue Aktion [register resource](/graph/api/governanceresource-register?view=graph-rest-beta) hinzugefügt.|
| Entfernung | Beta | Eigenschaft `isPermanent` der Entität [governanceRoleAssignment](/graph/api/resources/governanceroleassignment?view=graph-rest-beta) entfernt.|
| Entfernung | Beta | Eigenschaft `roleAssignmentStartDateTime` der Entität [governanceRoleAssignmentRequest](/graph/api/resources/governanceroleassignmentrequest?view=graph-rest-beta) entfernt.|
| Entfernung | Beta | Eigenschaft `roleAssignmentEndDateTime` der Entität [governanceRoleAssignmentRequest](/graph/api/resources/governanceroleassignmentrequest?view=graph-rest-beta) entfernt.|

### <a name="security-apis"></a>Sicherheits-APIs

| **Änderungstyp** | **Version** | **Beschreibung**              |
| :-------------- | :---------- | :--------------------------------------- |
| Ergänzungen        | Beta        | Der neue komplexe Typ [complianceInformation](/graph/api/complianceInformation/team?view=graph-rest-beta) wurde eingeführt.|
| Ergänzungen        | Beta        | Der neue komplexe Typ [certificationControl](/graph/api/certificationControl/team?view=graph-rest-beta) wurde eingeführt.|

## <a name="november-2018"></a>November 2018

### <a name="data-policy-operations-api"></a>Datenrichtlinienoperationen-API

| **Änderungstyp** | **Version** | **Beschreibung**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Ergänzungen        | Beta        | Es wurde eine neue **Status**-Eigenschaft zu [dataPolicyOperation](/graph/api/resources/dataPolicyOperation?view=graph-rest-beta) hinzugefügt. Gibt den Fortschritt eines Vorgangs an.

### <a name="directory-apis"></a>Verzeichnis-APIs

| **Änderungstyp** | **Version**   | **Beschreibung**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Ergänzungen | v1.0 | Aktion [forceDelete](/graph/api/domain-forcedelete?view=graph-rest-1.0) zu [domains](/graph/api/resources/domain?view=graph-rest-1.0) hinzugefügt.|
| Ergänzungen | Beta | Neue Methode „transitiveMembers“ für [groups](/graph/api/group-list-transitivemembers?view=graph-rest-beta) hinzugefügt. Diese Methode gibt eine flache Liste der Member einschließlich geschachtelter Member zurück.|
| Ergänzungen | Beta | Neue Methode „transitiveMemberOf“ für [users](/graph/api/user-list-transitivemembersof?view=graph-rest-beta), [groups](/graph/api/group-list-transitivemembersof?view=graph-rest-beta), [devices](/graph/api/device-list-transitivemembersof?view=graph-rest-beta) und [service principals](/graph/api/serviceprincipal-list-transitivemembersof?view=graph-rest-beta) hinzugefügt.|
| Ergänzungen | Beta | Mehode „memberOf“ hinzugefügt, um die direkte [membership](/graph/api/device-list-members?view=graph-rest-beta) eines Geräts abzurufen. Diese Methode wurde zum Abrufen der Liste der Mitgliedschaften einschließlich geschachtelter Mitgliedschaften hinzugefügt.|
| Ergänzungen | Beta | Neue Eigenschaften zu [Benutzer](/graph/api/resources/user?view=graph-rest-beta) hinzugefügt: **faxNumber**, **onPremisesDistinguishedName** und **otherMails**.|
| Ergänzungen | Beta | Eigenschaft **forceChangePasswordNextSignInWithMfa** zum komplexen Typ [passwordProfile](/graph/api/resources/passwordprofile?view=graph-rest-beta) hinzugefügt.|
| Ergänzungen    | Beta | Eigenschaften „externalUserState“ und „externalUserStateChangeDateTime“ zum [user](/graph/api/resources/user?view=graph-rest-beta)-Objekt hinzugefügt.|

### <a name="microsoft-teams-apis"></a>Microsoft Teams-APIs

| **Änderungstyp** | **Version**   | **Beschreibung**                          |
| :-------------- | :------------ | :--------------------------------------- |
|Ergänzungen |v1.0| Neuen Ressourcentyp [team](/graph/api/resources/team?view=graph-rest-1.0) eingeführt.|
|Ergänzungen |v1.0| Neuen Ressourcentyp [channel](/graph/api/resources/channel?view=graph-rest-1.0) eingeführt.|
|Ergänzungen |v1.0| Neuen Ressourcentyp [teamsApp](/graph/api/resources/teamsapp?view=graph-rest-1.0) eingeführt.|
|Ergänzungen |v1.0| Neuen Ressourcentyp [teamsAppDefinition](/graph/api/resources/teamsappdefinition?view=graph-rest-1.0) eingeführt.|
|Ergänzungen |v1.0| Neuen Ressourcentyp [teamsAppInstallation](/graph/api/resources/teamsappinstallation?view=graph-rest-1.0) eingeführt.|
|Ergänzungen |v1.0| Neuen Ressourcentyp [teamsAsyncOperation](/graph/api/resources/teamsasyncoperation?view=graph-rest-1.0) eingeführt. |
|Ergänzungen |v1.0| Neuen komplexen Typ [teamGuestSettings](/graph/api/resources/teamguestsettings?view=graph-rest-1.0) eingeführt. |
|Ergänzungen |v1.0| Neuen komplexen Typ [teamMemberSettings](/graph/api/resources/teammembersettings?view=graph-rest-1.0) eingeführt. |
|Ergänzungen |v1.0| Neuen komplexen Typ [teamMessagingSettings](/graph/api/resources/teammessagingsettings?view=graph-rest-1.0) eingeführt. |
|Ergänzungen |v1.0| Neuen komplexen Typ [teamFunSettings](/graph/api/resources/teamfunsettings?view=graph-rest-1.0) eingeführt. |
|Ergänzungen |v1.0| Neue Aktion [Team klonen](/graph/api/team-clone?view=graph-rest-1.0) eingeführt. |
|Ergänzungen |v1.0| Neue Aktion [Team archivieren](/graph/api/team-archive?view=graph-rest-1.0) eingeführt.|
|Ergänzungen |v1.0| Neue Aktion [Archivierung von Team aufheben](/graph/api/team-unarchive?view=graph-rest-1.0) eingeführt. |
|Ergänzungen         | Beta          | Unterstützung von Anwendungsberechtigungen für [Team klonen](/graph/api/team-clone?view=graph-rest-beta) hinzugefügt. |
|Ergänzungen |Beta| Einführung von [/teams/{id}/installedApps](/graph/api/resources/teamsappinstallation?view=graph-rest-beta), das „/teams/{id}/apps“ mit einigen Unterschieden in der Payload ersetzt. |
|Ergänzungen |Beta| Einführung von [/appCatalogs/teamsApps/{id}/appDefinition](/graph/api/resources/teamsappdefinition?view=graph-rest-beta), was die Versionseigenschaft in [/appCatalogs/teamsApps/{id}](/graph/api/resources/teamsapp?view=graph-rest-beta) ersetzt. |
|Änderung   |Beta| Der Typ [/appCatalogs/teamsApps](/graph/api/resources/teamsapp?view=graph-rest-beta) wurde von „teamsCatalogApp“ in „teamsApp“ umbenannt. |
|Änderung   |Beta| Der Typ der Eigenschaft „distributionMethod“ in [/appCatalogs/teamsApps](/graph/api/resources/teamsapp?view=graph-rest-beta) wurde von „teamsCatalogAppDistributionMethod“ in „teamsAppDistributionMethod“ umbenannt.  |
|Entfernen |Beta| Die Methode „teamsCatalogAppDistributionMethod“ wurde in „teamsAppDistributionMethod“ umbenannt.  |
|Ergänzungen |Beta| Einführung von [/teams/{id}/installedApps](/graph/api/resources/teamsappinstallation?view=graph-rest-beta), das „/teams/{id}/apps“ mit einigen Unterschieden in der Payload ersetzt. |
|Ergänzungen |Beta| Die Eigenschaft „displayName“ wurde zu [teamsTab](/graph/api/resources/teamstab?view=graph-rest-beta) hinzugefügt. |
|Ergänzungen |Beta| Die Eigenschaft „messageId“ wurde zu [teamsTab](/graph/api/resources/teamstab?view=graph-rest-beta) hinzugefügt. |
|Ergänzungen |Beta| Die Eigenschaft „teamsApp“ wurde zu [teamsTab](/graph/api/resources/teamstab?view=graph-rest-beta) hinzugefügt. |
|Ergänzungen |Beta| Neuen Ressourcentyp [teamsAppInstallation](/graph/api/resources/teamsappinstallation?view=graph-rest-beta) eingeführt.|
|Ergänzungen |Beta| Neuen Ressourcentyp [teamsApp](/graph/api/resources/teamsapp?view=graph-rest-beta) eingeführt.|
|Ergänzungen |Beta| Neuen Ressourcentyp [teamsAppDefinition](/graph/api/resources/teamsappdefinition?view=graph-rest-beta) eingeführt.|
|Ergänzungen |Beta| Neuer Enumerationsmember „hiddenMembership“ in „teamVisibilityType“ eingeführt.|
|Ergänzungen |Beta| Neuer Enumerationsmember „createTeam“ in „teamsAsyncOperationType“ eingeführt.|
|Ergänzungen |Beta| Neuer Enumerationsmember „teamsAppDistributionMethod“ eingeführt.|
|Ergänzungen |Beta| Neue Aktualisierungs-App-Aktion unter [/teams/{id}/installedApps](/graph/api/resources/teamsappinstallation?view=graph-rest-beta) eingeführt. |

### <a name="reports-apis"></a>Bericht-APIs

| Änderungstyp | Version                                    | Beschreibung                              |
| :---------- | :----------------------------------------- | :--------------------------------------- |
| Ergänzungen    | Betaversion in Microsoft Graph China betrieben von 21Vianet | Die folgenden APIs wurden hinzugefügt:<br>[getEmailActivityUserDetail](/graph/api/reportroot-getemailactivityuserdetail?view=graph-rest-beta)<br>[getEmailActivityCounts](/graph/api/reportroot-getemailactivitycounts?view=graph-rest-beta)<br>[getEmailActivityUserCounts](/graph/api/reportroot-getemailactivityusercounts?view=graph-rest-beta)<br>[getEmailAppUsageUserDetail](/graph/api/reportroot-getemailappusageuserdetail?view=graph-rest-beta)<br>[getEmailAppUsageAppsUserCounts](/graph/api/reportroot-getemailappusageappsusercounts?view=graph-rest-beta)<br>[getEmailAppUsageUserCounts](/graph/api/reportroot-getemailappusageusercounts?view=graph-rest-beta)<br>[getEmailAppUsageVersionsUserCounts](/graph/api/reportroot-getemailappusageversionsusercounts?view=graph-rest-beta)<br>[getMailboxUsageDetail](/graph/api/reportroot-getmailboxusagedetail?view=graph-rest-beta)<br>[getMailboxUsageMailboxCounts](/graph/api/reportroot-getmailboxusagemailboxcounts?view=graph-rest-beta)<br>[getMailboxUsageQuotaStatusMailboxCounts](/graph/api/reportroot-getmailboxusagequotastatusmailboxcounts?view=graph-rest-beta)<br>[getMailboxUsageStorage](/graph/api/reportroot-getmailboxusagestorage?view=graph-rest-beta)<br>[getOffice365ActivationsUserDetail](/graph/api/reportroot-getoffice365activationsuserdetail?view=graph-rest-beta)<br>[getOffice365ActivationCounts](/graph/api/reportroot-getoffice365activationcounts?view=graph-rest-beta)<br>[getOffice365ActivationsUserCounts](/graph/api/reportroot-getoffice365activationsusercounts?view=graph-rest-beta)<br>[getOffice365ActiveUserDetail](/graph/api/reportroot-getoffice365activeuserdetail?view=graph-rest-beta)<br>[getOffice365ActiveUserCounts](/graph/api/reportroot-getoffice365activeusercounts?view=graph-rest-beta)<br>[getOffice365ServicesUserCounts](/graph/api/reportroot-getoffice365servicesusercounts?view=graph-rest-beta)<br>[getOffice365GroupsActivityDetail](/graph/api/reportroot-getoffice365groupsactivitydetail?view=graph-rest-beta)<br> [getOffice365GroupsActivityCounts](/graph/api/reportroot-getoffice365groupsactivitycounts?view=graph-rest-beta)<br>[getOffice365GroupsActivityGroupCounts](/graph/api/reportroot-getoffice365groupsactivitygroupcounts?view=graph-rest-beta)<br>[getOffice365GroupsActivityStorage](/graph/api/reportroot-getoffice365groupsactivitystorage?view=graph-rest-beta)<br>[getOffice365GroupsActivityFileCounts](/graph/api/reportroot-getoffice365groupsactivityfilecounts?view=graph-rest-beta)<br>[getOneDriveActivityUserDetail](/graph/api/reportroot-getonedriveactivityuserdetail?view=graph-rest-beta)<br>[getOneDriveActivityUserCounts](/graph/api/reportroot-getonedriveactivityusercounts?view=graph-rest-beta)<br>[getOneDriveActivityFileCounts](/graph/api/reportroot-getonedriveactivityfilecounts?view=graph-rest-beta)<br>[getOneDriveUsageAccountDetail](/graph/api/reportroot-getonedriveusageaccountdetail?view=graph-rest-beta)<br>[getOneDriveUsageAccountCounts](/graph/api/reportroot-getonedriveusageaccountcounts?view=graph-rest-beta)<br>[getOneDriveUsageFileCounts](/graph/api/reportroot-getonedriveusagefilecounts?view=graph-rest-beta)<br>[getOneDriveUsageStorage](/graph/api/reportroot-getonedriveusagestorage?view=graph-rest-beta)<br>[getSharePointActivityUserDetail](/graph/api/reportroot-getsharepointactivityuserdetail?view=graph-rest-beta)<br>[getSharePointActivityFileCounts](/graph/api/reportroot-getsharepointactivityfilecounts?view=graph-rest-beta)<br>[getSharePointActivityUserCounts](/graph/api/reportroot-getsharepointactivityusercounts?view=graph-rest-beta)<br>[getSharePointActivityPages](/graph/api/reportroot-getsharepointactivitypages?view=graph-rest-beta)<br>[getSharePointSiteUsageDetail](/graph/api/reportroot-getsharepointsiteusagedetail?view=graph-rest-beta)<br>[getSharePointSiteUsageFileCounts](/graph/api/reportroot-getsharepointsiteusagefilecounts?view=graph-rest-beta)<br>[getSharePointSiteUsageSiteCounts](/graph/api/reportroot-getsharepointsiteusagesitecounts?view=graph-rest-beta)<br>[getSharePointSiteUsageStorage](/graph/api/reportroot-getsharepointsiteusagestorage?view=graph-rest-beta)<br>[getSharePointSiteUsagePages](/graph/api/reportroot-getsharepointsiteusagepages?view=graph-rest-beta)<br>[getSkypeForBusinessActivityUserDetail](/graph/api/reportroot-getskypeforbusinessactivityuserdetail?view=graph-rest-beta)<br>[getSkypeForBusinessActivityCounts](/graph/api/reportroot-getskypeforbusinessactivitycounts?view=graph-rest-beta)<br>[getSkypeForBusinessActivityUserCounts](/graph/api/reportroot-getskypeforbusinessactivityusercounts?view=graph-rest-beta)<br>[getSkypeForBusinessDeviceUsageUserDetail](/graph/api/reportroot-getskypeforbusinessdeviceusageuserdetail?view=graph-rest-beta)<br>[getSkypeForBusinessDeviceUsageDistributionUserCounts](/graph/api/reportroot-getskypeforbusinessdeviceusagedistributionusercounts?view=graph-rest-beta)<br>[getSkypeForBusinessDeviceUsageUserCounts](/graph/api/reportroot-getskypeforbusinessdeviceusageusercounts?view=graph-rest-beta)<br>[getSkypeForBusinessOrganizerActivityCounts](/graph/api/reportroot-getskypeforbusinessorganizeractivitycounts?view=graph-rest-beta)<br>[getSkypeForBusinessOrganizerActivityUserCounts](/graph/api/reportroot-getskypeforbusinessorganizeractivityusercounts?view=graph-rest-beta)<br>[getSkypeForBusinessOrganizerActivityMinuteCounts](/graph/api/reportroot-getskypeforbusinessorganizeractivityminutecounts?view=graph-rest-beta)<br>[getSkypeForBusinessParticipantActivityCounts](/graph/api/reportroot-getskypeforbusinessparticipantactivitycounts?view=graph-rest-beta)<br>[getSkypeForBusinessParticipantActivityUserCounts](/graph/api/reportroot-getskypeforbusinessparticipantactivityusercounts?view=graph-rest-beta)<br>[getSkypeForBusinessParticipantActivityMinuteCounts](/graph/api/reportroot-getskypeforbusinessparticipantactivityminutecounts?view=graph-rest-beta)<br>[getSkypeForBusinessPeerToPeerActivityCounts](/graph/api/reportroot-getskypeforbusinesspeertopeeractivitycounts?view=graph-rest-beta)<br>[getSkypeForBusinessPeerToPeerActivityUserCounts](/graph/api/reportroot-getskypeforbusinesspeertopeeractivityusercounts?view=graph-rest-beta)<br>[getSkypeForBusinessPeerToPeerActivityMinuteCounts](/graph/api/reportroot-getskypeforbusinesspeertopeeractivityminutecounts?view=graph-rest-beta). |

## <a name="october-2018"></a>Oktober 2018

### <a name="directory-apis"></a>Verzeichnis-APIs

| **Änderungstyp** | **Version**   | **Beschreibung**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Ergänzungen | Beta | Neue Methode „transitiveMembers“ für [groups](/graph/api/group-list-transitivemembers?view=graph-rest-beta) hinzugefügt. Diese Methode gibt eine flache Liste der Member einschließlich geschachtelter Member zurück.|
| Ergänzungen | Beta | Neue Methode „transitiveMemberOf“ für [users](/graph/api/user-list-transitivemembersof?view=graph-rest-beta), [groups](/graph/api/group-list-transitivemembersof?view=graph-rest-beta), [devices](/graph/api/device-list-transitivemembersof?view=graph-rest-beta) und [service principals](/graph/api/serviceprincipal-list-transitivemembersof?view=graph-rest-beta) hinzugefügt.|
| Ergänzungen | Beta | Mehode „memberOf“ hinzugefügt, um die direkte [membership](/graph/api/device-list-members?view=graph-rest-beta) eines Geräts abzurufen. Diese Methode wurde zum Abrufen der Liste der Mitgliedschaften einschließlich geschachtelter Mitgliedschaften hinzugefügt.|
| Ergänzungen | Beta | Neue Eigenschaften zu [Benutzer](/graph/api/resources/user?view=graph-rest-beta) hinzugefügt: **faxNumber**, **onPremisesDistinguishedName** und **otherMails**.|

### <a name="riskyusers-apis"></a>RiskyUsers-APIs

| **Änderungstyp** | **Version**   | **Beschreibung**                          |
| :-------------- | :------------ | :--------------------------------------- |
|Ergänzungen |Beta| [riskyUsers-API](/graph/api/resources/riskyuser?view=graph-rest-beta) eingeführt,die Azure AD-Benutzer darstellt, die einem Risiko ausgesetzt sind, wie durch Azure AD Identity Protection erkannt. |


### <a name="signin-apis"></a>SignIn-APIs

| **Änderungstyp** | **Version**   | **Beschreibung**                          |
| :-------------- | :------------ | :--------------------------------------- |
|Änderung   |Beta| Eigenschaft `conditionalAccessPolicies` in `appliedConditionalAccessPolicy` umbenannt.|
|Ergänzungen |Beta| Weitere Risikoeigenschaften in die [signIn-API](/graph/api/resources/signin?view=graph-rest-beta) aufgenommen, darunter `riskDetail`, `riskLevelAggregated`, `riskLevelDuringSignIn`, `riskEventTypes`, und `riskState`|
|Ergänzungen |Beta| Weitere Anmeldeeigenschaften in die [signIn-API](/graph/api/resources/signin?view=graph-rest-beta) aufgenommen, darunter `authenticationProcessingDetails`, `originalRequestID`, `isInteractive`, `tokenIssuerName`, `tokenIssuerType`, `correlationId` und `processingTimeinMilliseconds`|
|Entfernen   |Beta| Eigenschaft `isRisky` entfernt.|

## <a name="october-2018"></a>Oktober 2018

### <a name="delta-query"></a>Delta-Abfrage

| **Änderungstyp** | **Version** | **Beschreibung**                  |
|:------------|:--------|:-----------------------------------------|
| Ergänzungen    | Beta   | [Deltaabfrage](delta-query-overview.md)-Funktion für [directoryObject](/graph/api/directoryobject-delta?view=graph-rest-beta) hinzugefügt |
| Änderung      | v1.0 und Beta  | Alternatives Verhalten zum Zurückgeben von geänderten Eigenschaften nur in JSON-Antworten für [users](/graph/api/user-delta?view=graph-rest-1.0) und [groups](/graph/api/group-delta?view=graph-rest-1.0) |
| Ergänzungen    | v1.0   | Funktion [delta](/graph/api/directoryrole-delta?view=graph-rest-1.0) für [directoryRole](/graph/api/resources/directoryrole?view=graph-rest-1.0) hinzugefügt, um [Änderungsverfolgung mit Delta-Abfragen zu unterstützen](delta-query-overview.md) |

### <a name="directory-apis"></a>Verzeichnis-APIs

| **Änderungstyp** | **Version**   | **Beschreibung**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Ergänzungen | Beta | Eigenschaft **licenseAssignmentStates** zur Entität [User](/graph/api/resources/user?view=graph-rest-beta) für [Gruppenbasierte Lizenzierung](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-licensing-whatis-azure-portal) hinzugefügt|
| Ergänzungen | Beta | Ressource **licenseAssignmentState** für [Gruppenbasierter Lizenzierung](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-licensing-whatis-azure-portal) hinzugefügt|
| Ergänzungen | Beta | Eigenschaften **assignedLicenses**, **licenseProcessingState**, **hasMembersWithLicenseErrors** und **membersWithLicenseErrors** zur Entität [Group](/graph/api/resources/group?view=graph-rest-beta) für [Gruppenbasierte Lizenzierung](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-licensing-whatis-azure-portal) hinzugefügt|

### <a name="microsoft-intune-apis"></a>Microsoft Intune-APIs

|Änderungstyp|Version|Beschreibung|
|:---|:---|:---|
|Ergänzungen|v1.0|Eigenschaft **tenantLockdownRequireNetworkDuringOutOfBoxExperience** zur Entität [windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-1.0) hinzugefügt|
|Ergänzungen|v1.0|Eigenschaft **v12_0** zum komplexen Typ [iosMinimumOperatingSystem](/graph/api/resources/intune-apps-iosminimumoperatingsystem?view=graph-rest-1.0) hinzugefüg|
|Ergänzungen|Beta|Eigenschaft **lastReportAggregationDateTime** zur Entität [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta) hinzugefügt|
|Ergänzungen|Beta|Hinzugefügte neue Entitäten:<br/>[intuneBrandingProfile](/graph/api/resources/intune-wip-intunebrandingprofile?view=graph-rest-beta)<br/>|
|Ergänzungen|Beta|Die folgenden komplexen Typen wurden hinzugefügt:<br/>[deviceAndAppManagementAssignedRoleIds](/graph/api/resources/intune-rbac-deviceandappmanagementassignedroleids?view=graph-rest-beta)<br/>|
|Ergänzungen|Beta|Neue Enumerationstypen hinzugefügt:<br/>[applicationGuardEnabledOptions](/graph/api/resources/intune-deviceconfig-applicationguardenabledoptions?view=graph-rest-beta)<br/>[autoRestartNotificationDismissalMethod](/graph/api/resources/intune-deviceconfig-autorestartnotificationdismissalmethod?view=graph-rest-beta)<br/>[meteredConnectionLimitType](/graph/api/resources/intune-deviceconfig-meteredconnectionlimittype?view=graph-rest-beta)<br/>|
|Ergänzungen|Beta|Aktion [enableLegacyPcManagement](/graph/api/intune-deviceconfig-devicemanagement-enablelegacypcmanagement?view=graph-rest-beta) für [deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-beta) hinzugefügt |
|Ergänzungen|Beta|Aktion [extendFeatureUpdatesPause](/graph/api/intune-deviceconfig-windowsupdateforbusinessconfiguration-extendfeatureupdatespause?view=graph-rest-beta) für [windowsUpdateForBusinessConfiguration](/graph/api/resources/intune-deviceconfig-windowsupdateforbusinessconfiguration?view=graph-rest-beta) hinzugefügt |
|Ergänzungen|Beta|Aktion [extendQualityUpdatesPause](/graph/api/intune-deviceconfig-windowsupdateforbusinessconfiguration-extendqualityupdatespause?view=graph-rest-beta) für [windowsUpdateForBusinessConfiguration](/graph/api/resources/intune-deviceconfig-windowsupdateforbusinessconfiguration?view=graph-rest-beta) hinzugefügt |
|Ergänzungen|Beta|Aktion [unassignUserFromDevice](/graph/api/intune-enrollment-windowsautopilotdeviceidentity-unassignuserfromdevice?view=graph-rest-beta) für [windowsAutopilotDeviceIdentity](/graph/api/resources/intune-enrollment-windowsautopilotdeviceidentity?view=graph-rest-beta) hinzugefügt |
|Ergänzungen|Beta|Funktion [getAssignedRoleIdsForLoggedInUser](/graph/api/intune-rbac-devicemanagement-getassignedroleidsforloggedinuser?view=graph-rest-beta) für [deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-beta) hinzugefügt |
|Ergänzungen|Beta|Funktion [getManagedDevicesWithAppFailures](/graph/api/intune-troubleshooting-user-getmanageddeviceswithappfailures?view=graph-rest-beta) für [user](/graph/api/resources/intune-devices-user?view=graph-rest-beta) hinzugefügt |
|Ergänzungen|Beta|Funktion [managedDeviceEnrollmentAbandonmentSummary](/graph/api/intune-troubleshooting-reportroot-manageddeviceenrollmentabandonmentsummary?view=graph-rest-beta) für [reportRoot](/graph/api/resources/intune-deviceconfig-reportroot?view=graph-rest-beta) hinzugefügt |
|Ergänzungen|Beta|Funktion [managedDeviceEnrollmentAbandonmentDetails](/graph/api/intune-troubleshooting-reportroot-manageddeviceenrollmentabandonmentdetails?view=graph-rest-beta) für [reportRoot](/graph/api/resources/intune-deviceconfig-reportroot?view=graph-rest-beta) hinzugefügt |
|Löschung|Beta|Eigenschaft **subjectAlternativeNameType** aus der Entität [androidForWorkCertificateProfileBase](/graph/api/resources/intune-deviceconfig-androidforworkcertificateprofilebase?view=graph-rest-beta) entfernt|
|Ergänzungen|Beta|Eigenschaft **subjectAlternativeNameType** aus der Entität [androidForWorkCertificateProfileBase](/graph/api/resources/intune-deviceconfig-androidforworkpkcscertificateprofile?view=graph-rest-beta) entfernt|
|Ergänzungen|Beta|Eigenschaften **certificateStore**, **customSubjectAlternativeNames** und **subjectAlternativeNameType** zur Entität [androidForWorkScepCertificateProfile](/graph/api/resources/intune-deviceconfig-androidforworkscepcertificateprofile?view=graph-rest-beta) hinzugefügt|
|Löschung|Beta|Eigenschaft **subjectAlternativeNameType** aus der Entität [androidWorkProfileCertificateProfileBase](/graph/api/resources/intune-deviceconfig-androidworkprofilecertificateprofilebase?view=graph-rest-beta) entfernt|
|Ergänzungen|Beta|Eigenschaft **subjectAlternativeNameType** zur Entität [androidWorkProfilePkcsCertificateProfile](/graph/api/resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile?view=graph-rest-beta) hinzugefügt|
|Ergänzungen|Beta|Eigenschaften **certificateStore**, **customSubjectAlternativeNames** und **subjectAlternativeNameType** zur Entität [androidWorkProfileScepCertificateProfile](/graph/api/resources/intune-deviceconfig-androidworkprofilescepcertificateprofile?view=graph-rest-beta) hinzugefügt|
|Ergänzungen|Beta|Eigenschaft **legacyPcManangementEnabled** zur Entität [deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-beta) hinzugefügt|
|Löschung|Beta|Eigenschaft **pinRequiredOnLaunchInsteadOfBiometric** aus der Entität [managedAppProtection](/graph/api/resources/intune-mam-managedappprotection?view=graph-rest-beta) entfernt|
|Ergänzungen|Beta|Eigenschaft **roleScopeTagIds** zur Entität [managedDeviceMobileAppConfiguration](/graph/api/resources/intune-apps-manageddevicemobileappconfiguration?view=graph-rest-beta) hinzugefügt|
|Ergänzungen|Beta|Eigenschaft **applicationGuardEnabledOptions** zur Entität [windows10EndpointProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windows10endpointprotectionconfiguration?view=graph-rest-beta) hinzugefügt|
|Ergänzungen|Beta|Eigenschaft **selectedMobileAppIds** zur Entität [windows10EnrollmentCompletionPageConfiguration](/graph/api/resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration?view=graph-rest-beta) hinzugefügt|
|Ergänzungen|Beta|Eigenschaften **engagedRestartDeadlineInDays**, **engagedRestartSnoozeScheduleInDays**, **engagedRestartTransitionScheduleInDays**, **autoRestartNotificationDismissal**, **scheduleRestartWarningInHours** und **scheduleImminentRestartWarningInMinutes** zur Entität [windowsUpdateForBusinessConfiguration](/graph/api/resources/intune-deviceconfig-windowsupdateforbusinessconfiguration?view=graph-rest-beta) hinzugefügt|
|Ergänzungen|Beta|Eigenschaften **preSharedKey** und **meteredConnectionLimit** zur Entität [windowsWifiConfiguration](/graph/api/resources/intune-deviceconfig-windowswificonfiguration?view=graph-rest-beta) hinzugefügt|
|Ergänzungen|Beta|Nagivationseigenschaft **intuneBrandingProfiles** zur Entität [deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-beta) hinzugefügt|
|Ergänzungen|Beta|Eigenschaften **v6_0**, **v7_0**, **v7_1**, **v8_0**, **v8_1** und **v9_0** zum komplexen Typ [androidMinimumOperatingSystem](/graph/api/resources/intune-apps-androidminimumoperatingsystem?view=graph-rest-beta) hinzugefügt|
|Ergänzungen|Beta|Eigenschaft **v12_0** zum komplexen Typ [iosMinimumOperatingSystem](/graph/api/resources/intune-apps-iosminimumoperatingsystem?view=graph-rest-beta) hinzugefügt|
|Löschung|Beta|Eigenschaft **runAsLoggedOnUser** aus dem komplexen Typ [win32LobAppPowerShellScriptDetection](/graph/api/resources/intune-apps-win32lobapppowershellscriptdetection?view=graph-rest-beta) entfernt|
|Ergänzungen|Beta|Eigenschaft **lastUpdateDateTime** zum komplexen Typ [osVersionCount](/graph/api/resources/intune-devices-osversioncount?view=graph-rest-beta) hinzugefügt|
|Ergänzungen|Beta|Eigenschaft **lastUpdateDateTime** zum komplexen Typ [windowsMalwareCategoryCount](/graph/api/resources/intune-devices-windowsmalwarecategorycount?view=graph-rest-beta) hinzugefügt|
|Ergänzungen|Beta|Eigenschaft **lastUpdateDateTime** zum komplexen Typ [windowsMalwareExecutionStateCount](/graph/api/resources/intune-devices-windowsmalwareexecutionstatecount?view=graph-rest-beta) hinzugefügt|
|Ergänzungen|Beta|Eigenschaft **lastUpdateDateTime** zum komplexen Typ [windowsMalwareNameCount](/graph/api/resources/intune-devices-windowsmalwarenamecount?view=graph-rest-beta) hinzugefügt|
|Ergänzungen|Beta|Eigenschaft **lastUpdateDateTime** zum komplexen Typ [windowsMalwareStateCount](/graph/api/resources/intune-devices-windowsmalwarestatecount?view=graph-rest-beta) hinzugefügt|

### <a name="microsoft-teams-apis"></a>Microsoft Teams-APIs

| **Änderungstyp** | **Version**   | **Beschreibung**                          |
| :-------------- | :------------ | :--------------------------------------- |
|Ergänzungen|Beta|Anwendungsberechtigungs-Unterstützung für die APIs [Team archivieren](/graph/api/team-archive?view=graph-rest-beta) und [Archivierung von Team aufheben](/graph/api/team-unarchive?view=graph-rest-beta) hinzugefügt.|

### <a name="outlook-contacts"></a>Outlook-Kontakte

| **Änderungstyp** | **Version** | **Beschreibung**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Entfernen         | v1.0        | Dies ist eine Korrektur der Dokumentation: Eigenschaft **flag** aus dem Thema zur Entität [contact](/graph/api/resources/contact?view=graph-rest-1.0) entfernt. Die Eigenschaft wurde in der Entität **contact** nie verfügbar gemacht.|

### <a name="privileged-identity-management-apis"></a>Privileged Identity Management-APIs

| **Änderungstyp** | **Version**   | **Beschreibung**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Änderung | Beta | Entität [privilegedapproval](/graph/api/resources/privilegedapproval?view=graph-rest-beta) geändert.|
| Ergänzungen | Beta | Entität [privilegedroleassignmentrequest](/graph/api/resources/privilegedroleassignmentrequest?view=graph-rest-beta) und die folgenden Methoden und Aktionen hinzugefügt:<br> [List](/graph/api/privilegedroleassignmentrequest-list?view=graph-rest-beta) <br> [Create](/graph/api/privilegedroleassignmentrequest-post?view=graph-rest-beta) <br> [Cancel](/graph/api/privilegedroleassignmentrequest-cancel?view=graph-rest-beta) <br> [My](/graph/api/privilegedroleassignmentrequest-my?view=graph-rest-beta) |
| Ergänzungen | Beta | [Update](/graph/api/privilegedrolesettings-update?view=graph-rest-beta) für [privilegedRoleSettings](/graph/api/resources/privilegedrolesettings?view=graph-rest-beta) hinzugefügt|
| Entfernen |Beta| [Self Activate Role Assignment](/graph/api/privilegedrole_selfactivate?view=graph-rest-beta) als veraltet markiert|

### <a name="reports-apis"></a>Bericht-APIs
| Änderungstyp | Version | Beschreibung                              |
|:------------|:--------|:-----------------------------------------|
| Ergänzungen    | v1.0    | Eigenschaft **Site ID** zu [getSharePointSiteUsageDetail](/graph/api/reportroot-getsharepointsiteusagedetail?view=graph-rest-1.0) hinzugefügt. |

## <a name="september-2018"></a>September 2018

### <a name="calls-and-online-meetings-api"></a>API für Anrufe und Onlinebesprechungen

| **Änderungstyp** | **Version** | **Beschreibung**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Änderung          | Beta        | Die Ressource [application](/graph/api/resources/application?view=graph-rest-beta) wurde aktualisiert und es wurde die Anrufsammlung hinzugefügt. |
| Änderung          | Beta        | Die Ressource [operation](/graph/api/resources/operation?view=graph-rest-beta) wurde aktualisiert, um lange ausgeführte APIs für Anrufe und Besprechungen zu unterstützen. |
| Ergänzungen        | Beta        | Ressource [call](/graph/api/resources/call?view=graph-rest-beta) wurde zur Unterstützung von Audio-/Videoanrufen (anfänglich in Microsoft Teams) hinzugefügt, einschließlich APIs zum [Erstellen von Anrufen](/graph/api/application-post-calls?view=graph-rest-beta), [Zurückholen eines Anrufs](/graph/api/call-get?view=graph-rest-beta), [Löschen eines Anrufs (Auflegen)](/graph/api/call-delete?view=graph-rest-beta), [Annehmen eines Anrufs](/graph/api/call-answer?view=graph-rest-beta), [Ablehnen eines Anrufs](/graph/api/call-reject?view=graph-rest-beta), [Umleiten eines Anrufs](/graph/api/call-redirect?view=graph-rest-beta) und [Weiterleiten eines Anrufs](/graph/api/call-transfer?view=graph-rest-beta). Darüber hinaus wurden APIs zur Unterstützung von [IVR-Szenarien](/graph/api/resources/calls-api-ivr-overview?view=graph-rest-beta): [Wiedergeben einer Telefonansage](/graph/api/call-playprompt?view=graph-rest-beta), [Aufzeichnen eines Anrufs](/graph/api/call-record?view=graph-rest-beta), [Abbrechen der Medienverarbeitung](/graph/api/call-cancelmediaprocessing?view=graph-rest-beta) und [Abonnieren von Tonwahlbenachrichtigungen](/graph/api/call-subscribetotone?view=graph-rest-beta) hinzugefügt. |
| Ergänzungen        | Beta        | Ressource [participant](/graph/api/resources/call?view=graph-rest-beta) und APIs zum Verwalten von Teilnehmern an Audio-/Videoanrufen und Besprechungen wurde hinzugefügt, einschließlich [Abrufen eines Teilnehmerobjekts](/graph/api/participant-get?view=graph-rest-beta), [Konfigurieren des Audiomixers eines Teilnehmers](/graph/api/participant-configuremixer?view=graph-rest-beta), Stummschalten [eines](/graph/api/participant-mute?view=graph-rest-beta) oder [aller](/graph/api/participant-muteall?view=graph-rest-beta) Teilnehmer, [Abrufen einer Teilnehmerliste](/graph/api/call-list-participants?view=graph-rest-beta) in einem Anruf/einer Besprechung und [Einladen von Teilnehmern](/graph/api/participant-invite?view=graph-rest-beta) zu einem Anruf/einer Besprechung. |
| Ergänzungen        | Beta        | APIs für Anwendungen zum Verwalten von Anrufen und Besprechung sowie zum Teilnehmen daran wurden hinzugefügt, einschließlich der Möglichkeit, [Inhalt zu teilen](/graph/api/call-changescreensharingrole?view=graph-rest-beta), [sich selbst stumm zu schalten und die Stummschaltung aufzuheben](/graph/api/call-unmute?view=graph-rest-beta) sowie [die mit dem Anruf verknüpften Metadaten zu aktualisieren](/graph/api/call-updatemetadata?view=graph-rest-beta). |
| Ergänzungen        | Beta        | Ressource [audio routing group](/graph/api/resources/audioroutinggroup?view=graph-rest-beta) und APIs zum Verwalten von privaten Audio-Routen zwischen Teilnehmern an einer Unterhaltung mit mehreren Beteiligten wurde hinzugefügt, einschließlich [Erstellen von Audio-Routinggruppen](/graph/api/call-post-audioroutinggroups?view=graph-rest-beta), [Abrufen einer Liste der Gruppen](/graph/api/audioroutinggroup-get?view=graph-rest-beta) sowie [Aktualisieren](/graph/api/audioroutinggroup-update?view=graph-rest-beta) und [Löschen](/graph/api/audioroutinggroup-delete?view=graph-rest-beta) der Gruppen. |
| Ergänzungen        | Beta        | Ressource [online meeting](/graph/api/resources/audioroutinggroup?view=graph-rest-beta) und APIs zum Verwalten von Microsoft Teams-Online-Besprechungen hinzugefügt. Anfänglicht ist nur eine API für Onlinebesprechungen zum [Abrufen eines Onlinebesprechungsobjekts](/graph/api/onlinemeeting-get?view=graph-rest-beta) verfügbar. Eine zugehörige Ressource für die [Audiokonferenz Informationen](/graph/api/resources/audioconferencing?view=graph-rest-beta), die mit einer Besprechung verknüpft ist (z. B. Einwahl URL, Passcodes und Telefonnummern) wurde ebenfalls hinzugefügt. |
| Ergänzungen        | Beta        | Viele der APIs für Anrufe und Besprechungen benötigen Zeit, bis sie abgeschlossen sind, sodass Ressourcen für diese langwierigen Operationen hinzugefügt wurden: [anrufspezifische Operationen](/graph/api/resources/commsoperation?view=graph-rest-beta), [Wiedergeben von Telefonansagen](/graph/api/resources/playpromptoperation?view=graph-rest-beta) und [Aufzeichnen](/graph/api/resources/recordoperation?view=graph-rest-beta).  |

### <a name="dynamics-365-business-central-api"></a>Dynamics 365 Business Central-API

| **Änderungstyp** | **Version**   | **Beschreibung**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Ergänzungen        | Beta          | Finanz-APIs für Dynamics 365 Business Central wurden hinzugefügt. Einzelheiten hierzu finden Sie in der [Finanz-API-Referenz](/graph/api/resources/dynamics-graph-reference?view=graph-rest-beta)

### <a name="microsoft-graph-data-connect"></a>Microsoft Graph Data Connect

| **Änderungstyp** | **Version**   | **Beschreibung**                          |
| :-------------- | :------------ | :--------------------------------------- |
|Ergänzungen         | Nicht zutreffend| Die Möglichkeit zum Zugreifen auf Office 365-Daten in einem Massenvorgang wurde eingeführt. Details finden Sie unter [Microsoft Graph Data Connect (Vorschau)](data-connect-overview.md).|

### <a name="microsoft-intune-apis"></a>Microsoft Intune-APIs
|Änderungstyp|Version|Beschreibung|
|:---|:---|:---|
|Ergänzungen|v1.0|[assign](/graph/api/intune-apps-manageddevicemobileappconfiguration-assign?view=graph-rest-1.0)-Aktion zu [managedDeviceMobileAppConfiguration](/graph/api/resources/intune-apps-manageddevicemobileappconfiguration?view=graph-rest-1.0) hinzugefügt. |
|Ergänzungen|Beta|Hinzugefügte neue Entitäten:<br/>[officeClientConfiguration](/graph/api/resources/intune-cirrus-officeclientconfiguration?view=graph-rest-beta)<br/>[officeClientConfigurationAssignment](/graph/api/resources/intune-cirrus-officeclientconfigurationassignment?view=graph-rest-beta)<br/>[officeConfiguration](/graph/api/resources/intune-cirrus-officeconfiguration?view=graph-rest-beta)<br/>[windowsOfficeClientConfiguration](/graph/api/resources/intune-cirrus-windowsofficeclientconfiguration?view=graph-rest-beta)<br/>[windowsOfficeClientSecurityConfiguration](/graph/api/resources/intune-cirrus-windowsofficeclientsecurityconfiguration?view=graph-rest-beta)<br/>|
|Ergänzungen|Beta|Die folgenden komplexen Typen wurden hinzugefügt:<br/>[officeClientCheckinStatus](/graph/api/resources/intune-cirrus-officeclientcheckinstatus?view=graph-rest-beta)<br/>[officeConfigurationAssignmentTarget](/graph/api/resources/intune-cirrus-officeconfigurationassignmenttarget?view=graph-rest-beta)<br/>[officeConfigurationGroupAssignmentTarget](/graph/api/resources/intune-cirrus-officeconfigurationgroupassignmenttarget?view=graph-rest-beta)<br/>[officeUserCheckinSummary](/graph/api/resources/intune-cirrus-officeusercheckinsummary?view=graph-rest-beta)<br/>|
|Ergänzungen|Beta|Aktion [assign](/graph/api/intune-cirrus-officeclientconfiguration-assign?view=graph-rest-beta) für [officeClientConfiguration](/graph/api/resources/intune-cirrus-officeclientconfiguration?view=graph-rest-beta) hinzugefügt |
|Ergänzungen|Beta|Aktion **updatePrioritie** für die Sammlung [officeClientConfiguration](/graph/api/resources/intune-cirrus-officeclientconfiguration?view=graph-rest-beta) hinzugefügt |
|Ergänzungen|Beta|Hinzugefügte neue Entitäten:<br/>[deviceConfigurationConflictSummary](/graph/api/resources/intune-deviceconfig-deviceconfigurationconflictsummary?view=graph-rest-beta)<br/>[importedWindowsAutopilotDeviceIdentityUpload](/graph/api/resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload?view=graph-rest-beta)<br/>[win32LobApp](/graph/api/resources/intune-apps-win32lobapp?view=graph-rest-beta)<br/>|
|Ergänzungen|Beta|Die folgenden kompleen Typen wurden hinzugefügt:<br/>[deviceConfigurationTargetedUserAndDevice](/graph/api/resources/intune-deviceconfig-deviceconfigurationtargeteduseranddevice?view=graph-rest-beta)<br/>[win32LobAppDetection](/graph/api/resources/intune-apps-win32lobappdetection?view=graph-rest-beta)<br/>[win32LobAppFileSystemDetection](/graph/api/resources/intune-apps-win32lobappfilesystemdetection?view=graph-rest-beta)<br/>[win32LobAppInstallExperience](/graph/api/resources/intune-apps-win32lobappinstallexperience?view=graph-rest-beta)<br/>[win32LobAppMsiInformation](/graph/api/resources/intune-apps-win32lobappmsiinformation?view=graph-rest-beta)<br/>[win32LobAppPowerShellScriptDetection](/graph/api/resources/intune-apps-win32lobapppowershellscriptdetection?view=graph-rest-beta)<br/>[win32LobAppProductCodeDetection](/graph/api/resources/intune-apps-win32lobappproductcodedetection?view=graph-rest-beta)<br/>[win32LobAppRegistryDetection](/graph/api/resources/intune-apps-win32lobappregistrydetection?view=graph-rest-beta)<br/>[win32LobAppReturnCode](/graph/api/resources/intune-apps-win32lobappreturncode?view=graph-rest-beta)<br/>[windows10AppsForceUpdateSchedule](/graph/api/resources/intune-deviceconfig-windows10appsforceupdateschedule?view=graph-rest-beta)<br/>|
|Ergänzungen|Beta|Neue Enumerationstypen hinzugefügt:<br/>[administratorConfiguredDeviceComplianceState](/graph/api/resources/intune-deviceconfig-administratorconfigureddevicecompliancestate?view=graph-rest-beta)<br/>[importedWindowsAutopilotDeviceIdentityUploadStatus](/graph/api/resources/intune-enrollment-importedwindowsautopilotdeviceidentityuploadstatus?view=graph-rest-beta)<br/>[microsoftStoreForBusinessPortalSelectionOptions](/graph/api/resources/intune-onboarding-microsoftstoreforbusinessportalselectionoptions?view=graph-rest-beta)<br/>[win32LobAppDetectionOperator](/graph/api/resources/intune-apps-win32lobappdetectionoperator?view=graph-rest-beta)<br/>[win32LobAppFileSystemDetectionType](/graph/api/resources/intune-apps-win32lobappfilesystemdetectiontype?view=graph-rest-beta)<br/>[win32LobAppMsiPackageType](/graph/api/resources/intune-apps-win32lobappmsipackagetype?view=graph-rest-beta)<br/>[win32LobAppRegistryDetectionType](/graph/api/resources/intune-apps-win32lobappregistrydetectiontype?view=graph-rest-beta)<br/>[win32LobAppReturnCodeType](/graph/api/resources/intune-apps-win32lobappreturncodetype?view=graph-rest-beta)<br/>[windows10AppsUpdateRecurrence](/graph/api/resources/intune-deviceconfig-windows10appsupdaterecurrence?view=graph-rest-beta)<br/>[windowsAppStartLayoutTileSize](/graph/api/resources/intune-deviceconfig-windowsappstartlayouttilesize?view=graph-rest-beta)<br/>[windowsAutopilotProfileAssignmentDetailedStatus](/graph/api/resources/intune-enrollment-windowsautopilotprofileassignmentdetailedstatus?view=graph-rest-beta)<br/>|
|Ergänzungen|Beta|Aktion **overrideComplianceState** für [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) hinzugefügt |
|Ergänzungen|Beta|Aktion **getTargetedUsersAndDevices** zur Sammlung [deviceConfiguration](/graph/api/resources/intune-deviceconfig-deviceconfiguration?view=graph-rest-beta) hinzugefügt |
|Ergänzungen|Beta|Funktion [autopilotDeviceStream](/graph/api/intune-enrollment-importedwindowsautopilotdeviceidentityupload-autopilotdevicestream?view=graph-rest-beta) zu [importedWindowsAutopilotDeviceIdentityUpload](/graph/api/resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload?view=graph-rest-beta) hinzugefügt |
|Ergänzungen|Beta|Eigenschaft **restrictedApps** für Entität [androidCompliancePolicy](/graph/api/resources/intune-deviceconfig-androidcompliancepolicy?view=graph-rest-beta) hinzugefügt|
|Ergänzungen|Beta|Eigenschaft **tokenCreationDateTime** zur Entität [androidDeviceOwnerEnrollmentProfile](/graph/api/resources/intune-androidforwork-androiddeviceownerenrollmentprofile?view=graph-rest-beta) hinzugefügt|
|Löschung|Beta|Eigenschaft **restrictedApps** aus der Entität [androidForWorkCompliancePolicy](/graph/api/resources/intune-deviceconfig-androidforworkcompliancepolicy?view=graph-rest-beta) entfernt|
|Löschung|Beta|Eigenschaft **restrictedApps** aus der Entität [androidWorkProfileCompliancePolicy](/graph/api/resources/intune-deviceconfig-androidworkprofilecompliancepolicy?view=graph-rest-beta) entfernt|
|Änderung|Beta|Die folgenden Eigenschaften der Entität [appleVpnConfiguration](/graph/api/resources/intune-deviceconfig-applevpnconfiguration?view=graph-rest-beta) wurden geändert:<br/>**enablePerApp** von „erforderlich“ zu „optional“<br/>|
|Ergänzung|Beta|Eigenschaften **disableProtectionOfManagedOutboundOpenInData** und **protectInboundDataFromUnknownSources** zur Entität [defaultManagedAppProtection](/graph/api/resources/intune-mam-defaultmanagedappprotection?view=graph-rest-beta) hinzugefügt|
|Ergänzungen|Beta|Eigenschaft **microsoftStoreForBusinessPortalSelection** zur Entität [deviceAppManagement](/graph/api/resources/intune-shared-deviceappmanagement?view=graph-rest-beta) hinzugefügt|
|Ergänzungen|Beta|Eigenschaft **passcodeMinutesOfInactivityBeforeScreenTimeout** zur Entität [iosCompliancePolicy](/graph/api/resources/intune-deviceconfig-ioscompliancepolicy?view=graph-rest-beta) hinzugefügt|
|Ergänzungen|Beta|Eigenschaft **useOAuth** zur Entität [iosEasEmailProfileConfiguration](/graph/api/resources/intune-deviceconfig-ioseasemailprofileconfiguration?view=graph-rest-beta) hinzugefügt|
|Ergänzungen|Beta|Eigenschaften **kioskModeBlockVolumeButtons**, **classroomForceRequestPermissionToLeaveClasses**, **keychainBlockCloudSync**, **pkiBlockOTAUpdates**, **privacyForceLimitAdTracking**, **enterpriseBookBlockBackup**, **enterpriseBookBlockMetadataSync**, **airPrintBlocked**, **airPrintBlockCredentialsStorage**, **airPrintForceTrustedTLS**, **airPrintBlockiBeaconDiscovery**, **blockSystemAppRemoval** and **vpnBlockCreation** zur Entität [iosGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-iosgeneraldeviceconfiguration?view=graph-rest-beta) hinzugefügt|
|Ergänzungen|Beta|Eigenschaften **disableProtectionOfManagedOutboundOpenInData** und **protectInboundDataFromUnknownSources** zur Entität [iosManagedAppProtection](/graph/api/resources/intune-mam-iosmanagedappprotection?view=graph-rest-beta) hinzugefügt|
|Ergänzungen|Beta|Eigenschaft **gatekeeperAllowedAppSource** zur Entität [macOSCompliancePolicy](/graph/api/resources/intune-deviceconfig-macoscompliancepolicy?view=graph-rest-beta) hinzugefügt|
|Ergänzungen|Beta|Eigenschaften **keychainBlockCloudSync**, **airPrintBlocked**, **airPrintForceTrustedTLS** und **airPrintBlockiBeaconDiscovery** zur Entität [macOSGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-macosgeneraldeviceconfiguration?view=graph-rest-beta) hinzugefügt|
|Ergänzungen|Beta|Eigenschaften **deviceModel** und **deviceManufacturer** zur Entität [managedAppRegistration](/graph/api/resources/intune-mam-managedappregistration?view=graph-rest-beta) hinzugefügt|
|Ergänzungen|Beta|Eigenschaft **enabledForScopeValidation** zur Entität [resourceOperation](/graph/api/resources/intune-rbac-resourceoperation?view=graph-rest-beta) hinzugefügt|
|Ergänzungen|Beta|Eigenschaft **claimTokenManagementFromExternalMdm** zur Entität [vppToken](/graph/api/resources/intune-onboarding-vpptoken?view=graph-rest-beta) hinzugefügt|
|Ergänzungen|Beta|Eigenschaft **windows10AppsForceUpdateSchedule** zur Entität [windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta) hinzugefügt|
|Ergänzungen|Beta|Eigenschaft **deploymentProfileAssignmentDetailedStatus** zur Entität [windowsAutopilotDeviceIdentity](/graph/api/resources/intune-enrollment-windowsautopilotdeviceidentity?view=graph-rest-beta) hinzugefügt|
|Ergänzungen|Beta|Navigationseigenschaften **deviceConfigurationConflictSummary** und **importedWindowsAutopilotDeviceIdentityUploads** zur Entität [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta) hinzugefügt|
|Ergänzungen|Beta|Navigationseigenschaft **intendedDeploymentProfile** zur Entität [windowsAutopilotDeviceIdentity](/graph/api/resources/intune-enrollment-windowsautopilotdeviceidentity?view=graph-rest-beta) hinzugefügt|
|Ergänzungen|Beta|Eigenschaften **startLayoutTileSize** und **name** zum komplexen Typ [windowsKioskAppBase](/graph/api/resources/intune-deviceconfig-windowskioskappbase?view=graph-rest-beta) hinzugefügt|
|Ergänzungen|Beta|Eigenschaften **desktopApplicationId** und **desktopApplicationLinkPath** zum komplexen Typ [windowsKioskDesktopApp](/graph/api/resources/intune-deviceconfig-windowskioskdesktopapp?view=graph-rest-beta) hinzugefügt|
|Löschung|Beta|Eigenschaft **name** aus dem komplexen Typ [windowsKioskDesktopApp](/graph/api/resources/intune-deviceconfig-windowskioskdesktopapp?view=graph-rest-beta) entfernt|
|Ergänzungen|Beta|Eigenschaft **disallowDesktopApps** zum komplexen Typ [windowsKioskMultipleApps](/graph/api/resources/intune-deviceconfig-windowskioskmultipleapps?view=graph-rest-beta) hinzugefügt|
|Änderung|Beta|Die folgenden Eigenschaften des komplexen Typs [windowsKioskMultipleApps](/graph/api/resources/intune-deviceconfig-windowskioskmultipleapps?view=graph-rest-beta) wurden geändert:<br/>**startMenuLayoutXml** von „erforderlich“ in „optional“<br/>|
|Ergänzungen|Beta|Die Eigenschaften **v10_1607**, **v10_1703**, **v10_1709** und **v10_1803**  um komplexen Typ [windowsMinimumOperatingSystem](/graph/api/resources/intune-apps-windowsminimumoperatingsystem?view=graph-rest-beta) hinzugefügt|
|Ergänzungen|Beta|Member **paloAltoGlobalProtect** zum Enumerationstyp [androidWorkProfileVpnConnectionType](/graph/api/resources/intune-deviceconfig-androidworkprofilevpnconnectiontype?view=graph-rest-beta) hinzugefügt|
|Ergänzungen|Beta|Member **remoteLock** zum Enumerationstyp [deviceComplianceActionType](/graph/api/resources/intune-deviceconfig-devicecomplianceactiontype?view=graph-rest-beta) hinzugefügt|


### <a name="microsoft-teams-apis"></a>Microsoft Teams-APIs

| **Änderungstyp** | **Version**   | **Beschreibung**                          |
| :-------------- | :------------ | :--------------------------------------- |
|Ergänzungen|Beta|API für [Registerkarten](/graph/api/resources/teamstab?view=graph-rest-beta) hinzugefügt.|
|Ergänzungen|Beta|API zum [Veröffentlichen von Apps für Ihre Organisation](/graph/api/resources/teamsapp?view=graph-rest-beta) hinzugefügt.|
|Ergänzungen|Beta|Unterstützung von Anwendungsberechtigungen für [GET /teams/{id}](/graph/api/team-get?view=graph-rest-beta) hinzugefügt. |
|Ergänzungen|Beta|Unterstützung von Anwendungsberechtigungen für [GET /teams/{id}/channels](/graph/api/group-list-channels?view=graph-rest-beta) hinzugefügt. |
|Ergänzungen|Beta|Unterstützung von Anwendungsberechtigungen für [GET /teams/{id}/channels/{id}](/graph/api/channel-get?view=graph-rest-beta) hinzugefügt. |
|Ergänzungen|Beta|Unterstützung von Anwendungsberechtigungen für [PUT /groups/{id}/team](/graph/api/team-put-teams?view=graph-rest-beta) hinzugefügt. |
|Ergänzungen|Beta|Unterstützung von Anwendungsberechtigungen für [PATCH /teams/{id}](/graph/api/team-update?view=graph-rest-beta) hinzugefügt. |
|Ergänzungen|Beta|Unterstützung von Anwendungsberechtigungen für [Channel erstellen](/graph/api/channel-post?view=graph-rest-beta), [Channel aktualisieren](/graph/api/channel-patch?view=graph-rest-beta) und [Channel löschen](/graph/api/channel-delete?view=graph-rest-beta) hinzugefügt. |
|Löschung|Beta| Eigenschaften „isBlocks“ und „installedState“ aus [teamsApp](/graph/api/resources/teamsapp?view=graph-rest-beta) entfernt.|
|Änderung| Beta | Kontexteigenschaft für [teamsApp](/graph/api/resources/teamsapp?view=graph-rest-beta) wurde in „distributionMethod“ umbenann.|

### <a name="onedrive-and-sharepoint-apis"></a>OneDrive- und SharePoint-APIs

| **Änderungstyp** | **Version** | **Beschreibung**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Ergänzungen        | Beta        | Das Argument **deferCommit** wurde zur Aktion [createUploadSession](/graph/api/driveitem-createuploadsession?view=graph-rest-beta) für [driveItem](/graph/api/resources/driveitem?view=graph-rest-beta) hinzugefügt|
| Ergänzungen        | Beta        | Komplexer Typ [storagePlanInformation](/graph/api/resources/storageplaninformation?view=graph-rest-beta) hinzugefügt |
| Ergänzungen        | Beta        | Eigenschaft **storagePlanInformation** zum komplexen Typ [quota](/graph/api/resources/quota?view=graph-rest-beta) hinzugefügt |
| Ergänzungen        | Beta        | Navigationseigenschaft **following** zur Entität [drive](/graph/api/resources/drive?view=graph-rest-beta) hinzugefügt. |
| Ergänzungen        | Beta        | Aktion [follow](/graph/api/driveitem-follow?view=graph-rest-beta) für [driveItem](/graph/api/resources/driveitem?view=graph-rest-beta) hinzugefügt |
| Ergänzungen        | Beta        | API [unfollow](/graph/api/driveitem-unfollow?view=graph-rest-beta) hinzugefügt |
| Ergänzungen        | Beta        | Eigenschaft **hasPassword** zur Entität [permission](/graph/api/resources/permission?view=graph-rest-beta) hinzugefügt |
| Ergänzungen        | Beta        | Eigenschaft **preventsDownload** zum komplexen Typ [sharingLink](/graph/api/resources/sharinglink?view=graph-rest-beta) hinzugefügt |
| Ergänzungen        | Beta        | Navigationseigenschaft **permission** zur Entität [sharedDriveItem](/graph/api/resources/shareddriveitem?view=graph-rest-beta) hinzugefügt. |
| Ergänzungen        | Beta        | Eigenschaft **geolocation** zur Entität [columnDefinition](/graph/api/resources/columndefinition?view=graph-rest-beta) hinzugefügt |
| Ergänzungen        | Beta        | Komplexer Typ [geolocationColumn](/graph/api/resources/geolocationcolumn?view=graph-rest-beta) hinzugefügt |
| Ergänzungen        | Beta        | Eigenschaft **analytics** zur Entität [driveItem](/graph/api/resources/driveitem?view=graph-rest-beta) hinzugefügt |
| Ergänzungen        | Beta        | Eigenschaft **analytics** zur Entität [site](/graph/api/resources/site?view=graph-rest-beta) hinzugefügt |
| Ergänzungen        | Beta        | Eigenschaft **analytics** zur Entität [listItem](/graph/api/resources/listitem?view=graph-rest-beta) hinzugefügt |
| Ergänzungen        | Beta        | Funktion **getActivitiesByInterval** zur Entität [driveItem](/graph/api/resources/driveitem?view=graph-rest-beta) hinzugefügt |
| Ergänzungen        | Beta        | Funktion **getActivitiesByInterval** zur Entität [site](/graph/api/resources/site?view=graph-rest-beta) hinzugefügt |
| Ergänzungen        | Beta        | Funktion **getActivitiesByInterval** zur Entität [listItem](/graph/api/resources/listitem?view=graph-rest-beta) hinzugefügt |
| Ergänzungen        | Beta        | Entität [itemAnalytics](/graph/api/resources/itemanalytics?view=graph-rest-beta) hinzugefügt |
| Ergänzungen        | Beta        | Entität [itemActivityStat](/graph/api/resources/itemactivity?view=graph-rest-beta) hinzugefügt |
| Ergänzungen        | Beta        | Komplexer Typ [itemActionStat](/graph/api/resources/itemactionstat?view=graph-rest-beta) hinzugefügt |
| Ergänzungen        | Beta        | Komplexer Typ [accessAction](/graph/api/resources/accessaction?view=graph-rest-beta) hinzugefügt |
| Ergänzungen        | Beta        | Komplexer Typ [incompleteData](/graph/api/resources/incompletedata?view=graph-rest-beta) hinzugefügt |
| Ergänzungen        | Beta        | Eigenschaft **access** zum komplexen Typ [itemActivity](/graph/api/resources/itemactivity?view=graph-rest-beta) hinzugefügt |
| Ergänzungen        | Beta        | Eigenschaft **location** zum komplexen Typ [itemActivity](/graph/api/resources/itemactivity?view=graph-rest-beta) hinzugefügt |
| Ergänzungen        | v1.0        | Aktion **preview** zur Entität [driveItem](/graph/api/resources/driveitem?view=graph-rest-1.0) hinzugefügt. |
| Ergänzungen        | v1.0        | Komplexer Typ [itemPreviewInfo](/graph/api/resources/itempreviewinfo?view=graph-rest-1.0) hinzugefügt |

### <a name="outlook-mail"></a>Outlook-Mail

| **Änderungstyp** | **Version**   | **Beschreibung**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Ergänzungen        | v1.0 und Beta | Die Eigenschaft **internetMessageHeaders** der Entität [message](/graph/api/resources/message?view=graph-rest-1.0) ist nun bei der Erstellung von Nachrichten nicht mehr schreibgeschützt. |


### <a name="project-rome-notifications-api"></a>Benachrichtigungs-API für Project Rome

| **Änderungstyp** | **Version** | **Beschreibung**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Ergänzungen          | Beta        | Ressourcentyp [notification](/graph/api/resources/projectrome-notification?view=graph-rest-beta) hinzugefügt. |
| Ergänzungen          | Beta        | [Create and publish notification] (/graph/api/projectrome_notification_post?view=graph-rest-beta)-API wurde hinzugefügt.|

### <a name="security-apis"></a>Sicherheits-APIs

| **Änderungstyp** | **Version** | **Beschreibung**              |
| :-------------- | :---------- | :--------------------------------------- |
| Ergänzungen        | Beta       | Secure Score-APIs wurden zur [Sicherheits-API](/graph/api/resources/securescore-api-overview?view=graph-rest-beta) hinzugefügt, einschließlich der folgenden Ressourcen und Operationen:<br/>[secureScores](/graph/api/resources/securescores?view=graph-rest-beta) (und verknüpfte Entitäten)<br/>[List secureScores](/graph/api/securescores-list?view=graph-rest-beta)<br/>[secureScoreControlProfiles](/graph/api/resources/securescorecontrolprofiles?view=graph-rest-beta)<br/>[List secureScoreControlProfiles](/graph/api/securescorecontrolprofiles-list?view=graph-rest-beta)<br/>[Update secureScoreControlProfiles](/graph/api/securescorecontrolprofiles-update?view=graph-rest-beta) |
| Ergänzungen        | Beta        | Der neue komplexe Typ [secureScoreControlStateUpdate](/graph/api/resources/securescorecontrolstateupdate?view=graph-rest-beta) wurde eingeführt. |


## <a name="august-2018"></a>August 2018

### <a name="delta-query"></a>Delta-Abfrage

| **Änderungstyp** | **Version** | **Beschreibung**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Ergänzungen        | Beta        | [Delta-Abfrage](delta-query-overview.md)-Funktion für die folgenden Entitäten in Azure AD wurde hinzugefügt:<br/>[application](/graph/api/application-delta?view=graph-rest-beta)<br/>[directoryRole](/graph/api/directoryrole-delta?view=graph-rest-beta)<br/>[servicePrincipal](/graph/api/serviceprincipal-delta?view=graph-rest-beta) |

### <a name="directory-apis"></a>Verzeichnis-APIs

| **Änderungstyp** | **Version**   | **Beschreibung**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Ergänzungen | v1.0 | isMultipleDataLocationsForServicesEnabled-Eigenschaft wurde der [Organization](/graph/api/resources/organization?view=graph-rest-beta)-Ressource hinzugefügt. Mit dieser Einstellung können Apps prüfen, ob dieser Mandant für Multi-Geo-Funktionen aktiviert ist. preferredDataLocation-Eigenschaft wurde den [user](/graph/api/resources/user?view=graph-rest-beta)- und [group](/graph/api/resources/group?view=graph-rest-beta)-Ressourcen hinzugefügt. Die Einstellung ermöglicht das Festlegen eines bevorzugten Datenspeicherorts für einen Benutzer oder Eine Gruppe.|
| Ergänzungen | v1.0 | Die Eigenschaft [onPremisesProvisioningErrors](/graph/api/resources/onpremisesprovisioningerror?view=graph-rest-1.0) wurde den Entitäten [User](/graph/api/resources/user?view=graph-rest-1.0) und [Group](/graph/api/resources/group?view=graph-rest-1.0) hinzugefügt, die Fehler bei der Verzeichnissynchronisierung von lokalen Verzeichnissen mit Azure Active Directory darstellen, wenn ein Synchronisierungsprodukt von Microsoft verwendet wird (einschließlich Azure AD Connect, DirSync und MIM + Connector).|
| Ergänzungen | v1.0 | Eigenschaft [onPremisesExtensionAttributes](/graph/api/resources/onpremisesextensionattributes?view=graph-rest-1.0) zur Entität [User](/graph/api/resources/user?view=graph-rest-1.0) hinzugefügt, die 15 benutzerdefinierte Erweiterungs-Attributeigenschaften enthält. Bei einem onPremisesSyncEnabled-Benutzer wird dieser Eigenschaftensatz als Master-Datensatz im lokalen Active Directory verwaltet und mit Azure AD synchronisiert. Er ist außerdem schreibgeschützt. Bei einem reinen Cloud-Benutzer (wenn „onPremisesSyncEnabled“ auf „false“ gesetzt ist) können diese Eigenschaften beim Erstellen oder Aktualisieren festgelegt werden.|
|Ergänzungen|v1.0|Eigenschaften **onPremisesDomainName**, **onPremisesSamAccountName** und **onPremisesUserPrincipalName** zur Entität [User](/graph/api/resources/user?view=graph-rest-1.0) hinzugefügt|

### <a name="microsoft-intune-apis"></a>Microsoft Intune-APIs

|Änderungstyp|Version|Beschreibung|
|:---|:---|:---|
|Ergänzungen|v1.0|Hinzugefügte neue Entitäten:<br/>[androidWorkProfileCompliancePolicy](/graph/api/resources/intune-deviceconfig-androidworkprofilecompliancepolicy?view=graph-rest-1.0)<br/>[androidWorkProfileCustomConfiguration](/graph/api/resources/intune-deviceconfig-androidworkprofilecustomconfiguration?view=graph-rest-1.0)<br/>[androidWorkProfileGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration?view=graph-rest-1.0)<br/>|
|Ergänzungen|v1.0|Neue Enumerationstypen hinzugefügt:<br/>[androidWorkProfileCrossProfileDataSharingType](/graph/api/resources/intune-deviceconfig-androidworkprofilecrossprofiledatasharingtype?view=graph-rest-1.0)<br/>[androidWorkProfileDefaultAppPermissionPolicyType](/graph/api/resources/intune-deviceconfig-androidworkprofiledefaultapppermissionpolicytype?view=graph-rest-1.0)<br/>[androidWorkProfileRequiredPasswordType](/graph/api/resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype?view=graph-rest-1.0)<br/>|
|Ergänzungen|v1.0|Die Funktion [managedDeviceEnrollmentFailureDetails](/graph/api/intune-shared-reportroot-manageddeviceenrollmentfailuredetails?view=graph-rest-1.0) wurde zu [reportRoot](/graph/api/resources/intune-shared-reportroot?view=graph-rest-1.0) hinzugefügt. |
|Ergänzungen|v1.0|Die Funktion [managedDeviceEnrollmentTopFailures](/graph/api/intune-shared-reportroot-manageddeviceenrollmenttopfailures?view=graph-rest-1.0) wurde zu [reportRoot](/graph/api/resources/intune-shared-reportroot?view=graph-rest-1.0) hinzugefügt. |
|Ergänzungen|v1.0|Eigenschaft **kioskModeBuiltInAppId** zur Entität [iosGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-iosgeneraldeviceconfiguration?view=graph-rest-1.0) hinzugefügt|
|Ergänzungen|v1.0|Member **notAssigned** zum Enumerationstyp [complianceStatus](/graph/api/resources/intune-shared-compliancestatus?view=graph-rest-1.0) hinzugefügt|
|Ergänzungen|v1.0|Member **pushNotification** zum Enumerationstyp [deviceComplianceActionType](/graph/api/resources/intune-deviceconfig-devicecomplianceactiontype?view=graph-rest-1.0) hinzugefügt|
|Ergänzungen|v1.0|Member **userAbandonment** zum Enumerationstyp [deviceEnrollmentFailureReason](/graph/api/resources/intune-troubleshooting-deviceenrollmentfailurereason?view=graph-rest-1.0) hinzugefügt|
|Ergänzungen|v1.0|Member **compromised** und **misconfigured** zum Enumerationstyp [managedDevicePartnerReportedHealthState](/graph/api/resources/intune-devices-manageddevicepartnerreportedhealthstate?view=graph-rest-1.0) hinzugefügt|
|Ergänzungen|v1.0|Member **assignedToExternalMDM** zum Enumerationstyp [vppTokenState](/graph/api/resources/intune-onboarding-vpptokenstate?view=graph-rest-1.0) hinzugefügt|
||
|Ergänzungen|Beta|Hinzugefügte neue Entitäten:<br/>[advancedThreatProtectionOnboardingDeviceSettingState](/graph/api/resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate?view=graph-rest-beta)<br/>[advancedThreatProtectionOnboardingStateSummary](/graph/api/resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary?view=graph-rest-beta)<br/>[depEnrollmentBaseProfile](/graph/api/resources/intune-enrollment-depenrollmentbaseprofile?view=graph-rest-beta)<br/>[depEnrollmentProfile](/graph/api/resources/intune-enrollment-depenrollmentprofile?view=graph-rest-beta)<br/>[depIOSEnrollmentProfile](/graph/api/resources/intune-enrollment-depiosenrollmentprofile?view=graph-rest-beta)<br/>[depMacOSEnrollmentProfile](/graph/api/resources/intune-enrollment-depmacosenrollmentprofile?view=graph-rest-beta)<br/>[enrollmentProfile](/graph/api/resources/intune-enrollment-enrollmentprofile?view=graph-rest-beta)<br/>[importedAppleDeviceIdentity](/graph/api/resources/intune-enrollment-importedappledeviceidentity?view=graph-rest-beta)<br/>[importedAppleDeviceIdentityResult](/graph/api/resources/intune-enrollment-importedappledeviceidentityresult?view=graph-rest-beta)<br/>[importedWindowsAutopilotDeviceIdentityUpload](/graph/api/resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload?view=graph-rest-beta)<br/>[roleScopeTag](/graph/api/resources/intune-rbac-rolescopetag?view=graph-rest-beta)<br/>[windowsIdentityProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windowsidentityprotectionconfiguration?view=graph-rest-beta)<br/>|
|Ergänzungen|Beta|Die folgenden komplexen Typen wurden hinzugefügt:<br/>[configurationManagerClientHealthState](/graph/api/resources/intune-devices-configurationmanagerclienthealthstate?view=graph-rest-beta)<br/>[customSubjectAlternativeName](/graph/api/resources/intune-deviceconfig-customsubjectalternativename?view=graph-rest-beta)<br/>[deviceManagementUserRightsLocalUserOrGroup](/graph/api/resources/intune-deviceconfig-devicemanagementuserrightslocaluserorgroup?view=graph-rest-beta)<br/>[deviceManagementUserRightsSetting](/graph/api/resources/intune-deviceconfig-devicemanagementuserrightssetting?view=graph-rest-beta)<br/>[managementCertificateWithThumbprint](/graph/api/resources/intune-enrollment-managementcertificatewiththumbprint?view=graph-rest-beta)<br/>[mobileAppSupportedDeviceType](/graph/api/resources/intune-troubleshooting-mobileappsupporteddevicetype?view=graph-rest-beta)<br/>[osVersionCount](/graph/api/resources/intune-devices-osversioncount?view=graph-rest-beta)<br/>[windowsMalwareCategoryCount](/graph/api/resources/intune-devices-windowsmalwarecategorycount?view=graph-rest-beta)<br/>[windowsMalwareExecutionStateCount](/graph/api/resources/intune-devices-windowsmalwareexecutionstatecount?view=graph-rest-beta)<br/>[windowsMalwareNameCount](/graph/api/resources/intune-devices-windowsmalwarenamecount?view=graph-rest-beta)<br/>[windowsMalwareOverview](/graph/api/resources/intune-devices-windowsmalwareoverview?view=graph-rest-beta)<br/>[windowsMalwareStateCount](/graph/api/resources/intune-devices-windowsmalwarestatecount?view=graph-rest-beta)<br/>|
|Ergänzungen|Beta|Neue Enumerationstypen hinzugefügt:<br/>[configurationManagerClientState](/graph/api/resources/intune-devices-configurationmanagerclientstate?view=graph-rest-beta)<br/>[depTokenType](/graph/api/resources/intune-enrollment-deptokentype?view=graph-rest-beta)<br/>[discoverySource](/graph/api/resources/intune-enrollment-discoverysource?view=graph-rest-beta)<br/>[importedWindowsAutopilotDeviceIdentityUploadStatus](/graph/api/resources/intune-enrollment-importedwindowsautopilotdeviceidentityuploadstatus?view=graph-rest-beta)<br/>[iTunesPairingMode](/graph/api/resources/intune-enrollment-itunespairingmode?view=graph-rest-beta)<br/>[lanManagerAuthenticationLevel](/graph/api/resources/intune-deviceconfig-lanmanagerauthenticationlevel?view=graph-rest-beta)<br/>[localSecurityOptionsMinimumSessionSecurity](/graph/api/resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity?view=graph-rest-beta)<br/>[resultantAppStateDetail](/graph/api/resources/intune-apps-resultantappstatedetail?view=graph-rest-beta)<br/>[vpnProviderType](/graph/api/resources/intune-deviceconfig-vpnprovidertype?view=graph-rest-beta)<br/>[windowsMalwareThreatState](/graph/api/resources/intune-devices-windowsmalwarethreatstate?view=graph-rest-beta)<br/>|
|Ergänzungen|Beta|Aktion [uploadDepToken](/graph/api/intune-enrollment-deponboardingsetting-uploaddeptoken?view=graph-rest-beta) zu [depOnboardingSetting](/graph/api/resources/intune-enrollment-deponboardingsetting?view=graph-rest-beta) hinzugefügt |
|Ergänzungen|Beta|Aktion [syncWithAppleDeviceEnrollmentProgram](/graph/api/intune-enrollment-deponboardingsetting-syncwithappledeviceenrollmentprogram?view=graph-rest-beta) zu [depOnboardingSetting](/graph/api/resources/intune-enrollment-deponboardingsetting?view=graph-rest-beta) hinzugefügt |
|Ergänzungen|Beta|Aktion [setDefaultProfile](/graph/api/intune-enrollment-enrollmentprofile-setdefaultprofile?view=graph-rest-beta) zu [enrollmentProfile](/graph/api/resources/intune-enrollment-enrollmentprofile?view=graph-rest-beta) hinzugefügt |
|Ergänzungen|Beta|Aktion **importAppleDeviceIdentityList** zur Sammlung [importedAppleDeviceIdentity](/graph/api/resources/intune-enrollment-importedappledeviceidentity?view=graph-rest-beta) hinzugefügt |
|Ergänzungen|Beta|Aktion [updateDeviceProfileAssignment](/graph/api/intune-enrollment-enrollmentprofile-updatedeviceprofileassignment?view=graph-rest-beta) zu [enrollmentProfile](/graph/api/resources/intune-enrollment-enrollmentprofile?view=graph-rest-beta) hinzugefügt |
|Ergänzungen|Beta|Aktion [shareForSchoolDataSyncService](/graph/api/intune-enrollment-deponboardingsetting-shareforschooldatasyncservice?view=graph-rest-beta) zu [depOnboardingSetting](/graph/api/resources/intune-enrollment-deponboardingsetting?view=graph-rest-beta) hinzugefügt |
|Ergänzungen|Beta|Aktion [unshareForSchoolDataSyncService](/graph/api/intune-enrollment-deponboardingsetting-unshareforschooldatasyncservice?view=graph-rest-beta) zu [depOnboardingSetting](/graph/api/resources/intune-enrollment-deponboardingsetting?view=graph-rest-beta) hinzugefügt |
|Ergänzungen|Beta|Aktion [assignUserToDevice](/graph/api/intune-enrollment-windowsautopilotdeviceidentity-assignusertodevice?view=graph-rest-beta) zu [windowsAutopilotDeviceIdentity](/graph/api/resources/intune-enrollment-windowsautopilotdeviceidentity?view=graph-rest-beta) hinzugefügt |
|Ergänzungen|Beta|Funktion [getRoleScopeTagsByResource](/graph/api/intune-rbac-devicemanagement-getrolescopetagsbyresource?view=graph-rest-beta) zu [deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-beta) hinzugefügt |
|Ergänzungen|Beta|Funktion [getRoleScopeTagsByIds](/graph/api/intune-rbac-devicemanagement-getrolescopetagsbyids?view=graph-rest-beta) zu [deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-beta) hinzugefügt |
|Ergänzungen|Beta|Funktion [getEncryptionPublicKey](/graph/api/intune-enrollment-deponboardingsetting-getencryptionpublickey?view=graph-rest-beta) zu [depOnboardingSetting](/graph/api/resources/intune-enrollment-deponboardingsetting?view=graph-rest-beta) hinzugefügt |
|Ergänzungen|Beta|Funktion [exportMobileConfig](/graph/api/intune-enrollment-enrollmentprofile-exportmobileconfig?view=graph-rest-beta) zu [enrollmentProfile](/graph/api/resources/intune-enrollment-enrollmentprofile?view=graph-rest-beta) hinzugefügt |
|Ergänzungen|Beta|Funktion [autopilotDeviceStream](/graph/api/intune-enrollment-importedwindowsautopilotdeviceidentityupload-autopilotdevicestream?view=graph-rest-beta) zu [importedWindowsAutopilotDeviceIdentityUpload](/graph/api/resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload?view=graph-rest-beta) hinzugefügt |
|Löschung|Beta|Sammlung **uploadDepToken** wurde entfernt |
|Löschung|Beta|Aktion **syncWithAppleDeviceEnrollmentProgram** aus der Sammlung [depOnboardingSetting](/graph/api/resources/intune-enrollment-deponboardingsetting?view=graph-rest-beta) entfernt |
|Löschung|Beta|Funktion **getEncryptionPublicKey** aus der Sammlung [depOnboardingSetting](/graph/api/resources/intune-enrollment-deponboardingsetting?view=graph-rest-beta) entfernt |
|Ergänzungen|Beta|Eigenschaft **restrictedApps** zur Entität [androidForWorkCompliancePolicy](/graph/api/resources/intune-deviceconfig-androidforworkcompliancepolicy?view=graph-rest-beta) hinzugefügt|
|Ergänzungen|Beta|Eigenschaften **vpnAlwaysOnPackageIdentifier** und **vpnEnableAlwaysOnLockdownMode** zur Entität [androidForWorkGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration?view=graph-rest-beta) hinzugefügt|
|Löschung|Beta|Eigenschaft **packageName** aus der Entität [androidForWorkMobileAppConfiguration](/graph/api/resources/intune-apps-androidforworkmobileappconfiguration?view=graph-rest-beta) entfernt|
|Ergänzungen|Beta|Eigenschaft **restrictedApps** zur Entität [androidWorkProfileCompliancePolicy](/graph/api/resources/intune-deviceconfig-androidworkprofilecompliancepolicy?view=graph-rest-beta) hinzugefügt|
|Ergänzungen|Beta|Eigenschaften **vpnAlwaysOnPackageIdentifier** und **vpnEnableAlwaysOnLockdownMode** zur Entität [androidWorkProfileGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration?view=graph-rest-beta) hinzugefügt|
|Ergänzungen|Beta|Die Eigenschaft **optInToDeviceIdSharing** wurde der Entität [appleVpnConfiguration](/graph/api/resources/intune-deviceconfig-applevpnconfiguration?view=graph-rest-beta) hinzugefügt.|
|Ergänzungen|Beta|Eigenschaften **tokenType**, **tokenName**, **syncedDeviceCount**, **defaultProfileDisplayName** und **dataSharingConsentGranted** zur Entität [depOnboardingSetting](/graph/api/resources/intune-enrollment-deponboardingsetting?view=graph-rest-beta) hinzugefügt|
|Ergänzungen|Beta|Eigenschaft **roleScopeTagIds** zur Entität [deviceCompliancePolicy](/graph/api/resources/intune-deviceconfig-devicecompliancepolicy?view=graph-rest-beta) hinzugefügt|
|Ergänzungen|Beta|Eigenschaften **roleScopeTagIds** und **supportsScopeTags** zur Entität [deviceConfiguration](/graph/api/resources/intune-deviceconfig-deviceconfiguration?view=graph-rest-beta) hinzugefügt|
|Ergänzungen|Beta|Die Eigenschaft **windowsMalwareOverview** wurde zur Entität [deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-beta) hinzugefügt.|
|Änderung|Beta|Die folgende Eigenschaften für die Entität [iosCertificateProfileBase](/graph/api/resources/intune-deviceconfig-ioscertificateprofilebase?view=graph-rest-beta) wurden geändert:<br/>**SubjectAlternativeNameType** von erforderlich in optional<br/>|
|Ergänzungen|Beta|Eigenschaft **restrictedApps** zur Entität [iosCompliancePolicy](/graph/api/resources/intune-deviceconfig-ioscompliancepolicy?view=graph-rest-beta) hinzugefügt|
|Ergänzungen|Beta|Eigenschaften **certificateStore** und **customSubjectAlternativeNames** zur Entität [iosScepCertificateProfile](/graph/api/resources/intune-deviceconfig-iosscepcertificateprofile?view=graph-rest-beta) hinzugefügt|
|Ergänzungen|Beta|Eigenschaft **enforcedSoftwareUpdateDelayInDays** zur Entität [iosUpdateConfiguration](/graph/api/resources/intune-deviceconfig-iosupdateconfiguration?view=graph-rest-beta) hinzugefügt|
|Ergänzungen|Beta|Eigenschaften **providerType**, **userDomain**, **strictEnforcement**, **cloudName** und **excludeList** zur Entität [iosVpnConfiguration](/graph/api/resources/intune-deviceconfig-iosvpnconfiguration?view=graph-rest-beta) hinzugefügt|
|Ergänzungen|Beta|Eigenschaften **safariBlockAutofill**, **cameraBlocked**, **iTunesBlockMusicService**, **spotlightBlockInternetResults**, **keyboardBlockDictation**, **definitionLookupBlocked**, **appleWatchBlockAutoUnlock**, **iTunesBlockFileSharing**, **iCloudBlockDocumentSync**, **iCloudBlockMail**, **iCloudBlockAddressBook**, **iCloudBlockCalendar**, **iCloudBlockReminders**, **iCloudBlockBookmarks**, **iCloudBlockNotes**, **airDropBlocked**, **passwordBlockModification** und **passwordBlockFingerprintUnlock** zur Entität [macOSGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-macosgeneraldeviceconfiguration?view=graph-rest-beta) hinzugefügt|
|Ergänzungen|Beta|Eigenschaften **roleScopeTagIds**, **windowsActiveMalwareCount**, **windowsRemediatedMalwareCount**, **notes** und **configurationManagerClientHealthState** zur Entität [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) hinzugefügt|
|Ergänzungen|Beta|Eigenschaft **installStateDetail** zur Entität [mobileAppInstallStatus](/graph/api/resources/intune-apps-mobileappinstallstatus?view=graph-rest-beta) hinzugefügt|
|Ergänzungen|Beta|Eigenschaft **roleScopeTagIds** zur Entität [notificationMessageTemplate](/graph/api/resources/intune-notification-notificationmessagetemplate?view=graph-rest-beta) hinzugefügt|
|Ergänzungen|Beta|Eigenschaften **targetVersion** und **updateVersion** zur Entität [officeSuiteApp](/graph/api/resources/intune-apps-officesuiteapp?view=graph-rest-beta) hinzugefügt|
|Ergänzungen|Beta|Eigenschaft **resource** zur Entität [resourceOperation](/graph/api/resources/intune-rbac-resourceoperation?view=graph-rest-beta) hinzugefügt|
|Ergänzungen|Beta|Eigenschaften **localStorage**, **setPowerPolicies** und **signInOnResume** zur Entität [sharedPCConfiguration](/graph/api/resources/intune-deviceconfig-sharedpcconfiguration?view=graph-rest-beta) hinzugefügt|
|Ergänzungen|Beta|Eigenschaft **configurationManagerComplianceRequired** zur Entität [windows10CompliancePolicy](/graph/api/resources/intune-deviceconfig-windows10compliancepolicy?view=graph-rest-beta) hinzugefügt|
|Ergänzungen|Beta|Eigenschaften **userRightsAccessCredentialManagerAsTrustedCaller**, **userRightsAllowAccessFromNetwork**, **userRightsBlockAccessFromNetwork**, **userRightsActAsPartOfTheOperatingSystem**, **userRightsLocalLogOn**, **userRightsBackupData**, **userRightsChangeSystemTime**, **userRightsCreateGlobalObjects**, **userRightsCreatePageFile**, **userRightsCreatePermanentSharedObjects**, **userRightsCreateSymbolicLinks**, **userRightsCreateToken**, **userRightsDebugPrograms**, **userRightsRemoteDesktopServicesLogOn**, **userRightsDelegation**, **userRightsGenerateSecurityAudits**, **userRightsImpersonateClient**, **userRightsIncreaseSchedulingPriority**, **userRightsLoadUnloadDrivers**, **userRightsLockMemory**, **userRightsManageAuditingAndSecurityLogs**, **userRightsManageVolumes**, **userRightsModifyFirmwareEnvironment**, **userRightsModifyObjectLabels**, **userRightsProfileSingleProcess**, **userRightsRemoteShutdown**, **userRightsRestoreData**, **userRightsTakeOwnership**, **userRightsRegisterProcessAsService**, **localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients**, **localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers**, **lanManagerAuthenticationLevel** und **lanManagerWorkstationEnableInsecureGuestLogons** zur Entität [windows10EndpointProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windows10endpointprotectionconfiguration?view=graph-rest-beta) hinzugefügt|
|Ergänzungen|Beta|Eigenschaften **passwordMinimumAgeInDays**, **tenantLockdownRequireNetworkDuringOutOfBoxExperience** und **dataProtectionBlockDirectMemoryAccess** zur Entität [windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta) hinzugefügt|
|Ergänzungen|Beta|Eigenschaft **extendedKeyUsages** zur Entität [windows10PkcsCertificateProfile](/graph/api/resources/intune-deviceconfig-windows10pkcscertificateprofile?view=graph-rest-beta) hinzugefügt|
|Ergänzungen|Beta|Eigenschaften **enableDnsRegistration** und **dnsSuffixes** zur Entität [windows10VpnConfiguration](/graph/api/resources/intune-deviceconfig-windows10vpnconfiguration?view=graph-rest-beta) hinzugefügt|
|Ergänzungen|Beta|Eigenschaft **customSubjectAlternativeNames** zur Entität [windows81CertificateProfileBase](/graph/api/resources/intune-deviceconfig-windows81certificateprofilebase?view=graph-rest-beta) hinzugefügt|
|Ergänzungen|Beta|Eigenschaften **extractHardwareHash** und **deviceNameTemplate** zur Entitiät [windowsAutopilotDeploymentProfile](/graph/api/resources/intune-enrollment-windowsautopilotdeploymentprofile?view=graph-rest-beta) hinzugefügt|
|Ergänzungen|Beta|Eigenschaften **addressableUserName** und **userPrincipalName** zur Entität [windowsAutopilotDeviceIdentity](/graph/api/resources/intune-enrollment-windowsautopilotdeviceidentity?view=graph-rest-beta) hinzugefügt|
|Ergänzungen|Beta|Eigenschaft **threatState** zur Entität [windowsDeviceMalwareState](/graph/api/resources/intune-devices-windowsdevicemalwarestate?view=graph-rest-beta) hinzugefügt|
|Ergänzungen|Beta|Eigenschaften **qualityUpdatesPauseStartDateTime**, **featureUpdatesPauseStartDateTime**, **featureUpdatesRollbackWindowInDays**, **qualityUpdatesWillBeRolledBack**, **featureUpdatesWillBeRolledBack**, **qualityUpdatesRollbackStartDateTime** und **featureUpdatesRollbackStartDateTime** zur Entität [windowsUpdateForBusinessConfiguration](/graph/api/resources/intune-deviceconfig-windowsupdateforbusinessconfiguration?view=graph-rest-beta) hinzugefügt|
|Ergänzungen|Beta|Eigenschaft **trustedServerCertificateNames** zur Entität [windowsWifiEnterpriseEAPConfiguration](/graph/api/resources/intune-deviceconfig-windowswifienterpriseeapconfiguration?view=graph-rest-beta) hinzugefügt|
|Ergänzungen|Beta|Navigationseigenschaften **defaultIosEnrollmentProfile**, **defaultMacOsEnrollmentProfile**, **enrollmentProfiles** und **importedAppleDeviceIdentities** navigation zur Entität [depOnboardingSetting](/graph/api/resources/intune-enrollment-deponboardingsetting?view=graph-rest-beta) hinzugefügt|
|Ergänzungen|Beta|Navigationseigenschaft **roleScopeTags** zur Entität [deviceAndAppManagementRoleAssignment](/graph/api/resources/intune-rbac-deviceandappmanagementroleassignment?view=graph-rest-beta) hinzugefügt|
|Ergänzungen|Beta|Navigationseigenschaften **advancedThreatProtectionOnboardingStateSummary**, **roleScopeTags** und **importedWindowsAutopilotDeviceIdentityUploads** zur Entität [deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-beta) hinzugefügt|
|Ergänzungen|Beta|Eigenschaft **supportedDeviceTypes** zum komplexen Typ [mobileAppIntentAndStateDetail](/graph/api/resources/intune-troubleshooting-mobileappintentandstatedetail?view=graph-rest-beta) hinzugefügt|
|Ergänzungen|Beta|Eigenschaft **hideEscapeLink** zum komplexen Typ [outOfBoxExperienceSettings](/graph/api/resources/intune-enrollment-outofboxexperiencesettings?view=graph-rest-beta) hinzugefügt|
|Ergänzungen|Beta|Member **zscalerPrivateAccess**, **f5Access2018**, **citrixSso** und **paloAltoGlobalProtectV2** zum Enumerationstyp [appleVpnConnectionType](/graph/api/resources/intune-deviceconfig-applevpnconnectiontype?view=graph-rest-beta) hinzugefügt|
|Ergänzungen|Beta|Member **userAbandonment** zum Enumerationstyp [deviceEnrollmentFailureReason](/graph/api/resources/intune-troubleshooting-deviceenrollmentfailurereason?view=graph-rest-beta) hinzugefügt|
|Ergänzungen|Beta|Member **blocked** zum Enumerationstyp [enrollmentState](/graph/api/resources/intune-enrollment-enrollmentstate?view=graph-rest-beta) hinzugefügt|
|Ergänzungen|Beta|Member **microsoft365ManagedMdm** zum Enumerationstyp [managementAgentType](/graph/api/resources/intune-devices-managementagenttype?view=graph-rest-beta) hinzugefügt|
|Ergänzungen|Beta|Member **domainNameService** zum Enumerationstyp [subjectAlternativeNameType](/graph/api/resources/intune-deviceconfig-subjectalternativenametype?view=graph-rest-beta) hinzugefügt|
|Ergänzungen|Beta|Member **wpa2Personal** und **wpa2Enterprise** zum Enumerationstyp [wiFiSecurityType](/graph/api/resources/intune-deviceconfig-wifisecuritytype?view=graph-rest-beta) hinzugefügt|
|Ergänzungen|Beta|Member **enterpriseUnwantedSoftware**, **ransom** und **hipsRule** zum Enumerationstyp [windowsMalwareCategory](/graph/api/resources/intune-devices-windowsmalwarecategory?view=graph-rest-beta) hinzugefügt|

### <a name="outlook-calendar"></a>Outlook-Kalender

| **Änderungstyp** | **Version**   | **Beschreibung**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Ergänzungen | Beta | Aktion [getSchedule](/graph/api/calendar-getschedule?view=graph-rest-beta) und die komplexen Typen [freeBusyError](/graph/api/resources/freebusyerror?view=graph-rest-beta), [scheduleInformation](/graph/api/resources/scheduleinformation?view=graph-rest-beta) und [scheduleItem](/graph/api/resources/scheduleitem?view=graph-rest-beta) hinzugefügt, um die [frei/belegt-, Verfügbarkeitsinformationen für Benutzer, Verteilerlisten und Ressourcen für einen bestimmten Zeitraum abzurufen](outlook-get-free-busy-schedule.md). |

### <a name="outlook-mail"></a>Outlook-Mail

| **Änderungstyp** | **Version**   | **Beschreibung**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Ergänzungen        | v1.0        | Unterstützung für die [getMailTips](/graph/api/user-getmailtips?view=graph-rest-1.0)-Aktion, um beliebige MailTips für bestimmte Empfänger zu erhalten, wurde hinzugefügt. Folgende Ressourcen wurden hinzugefügt: [automaticRepliesMailTips](/graph/api/resources/automaticrepliesmailtips?view=graph-rest-1.0), [mailTips](/graph/api/resources/mailtips?view=graph-rest-1.0), [mailTipsError](/graph/api/resources/mailtipserror?view=graph-rest-1.0). |

### <a name="reports-apis"></a>Bericht-APIs
| Änderungstyp | Version | Beschreibung                              |
|:------------|:--------|:-----------------------------------------|
| Ergänzungen    | v1.0    | Eigenschaft **Activated On Shared Computer** zu [getoffice365activationsuserdetail](/graph/api/reportroot-getoffice365activationsuserdetail?view=graph-rest-1.0) hinzugefügt. |
| Ergänzungen    | v1.0    | Eigenschaft **Shared Computer Activation** zu [getoffice365activationsusercounts](/graph/api/reportroot-getoffice365activationsusercounts?view=graph-rest-1.0) hinzugefügt. |

### <a name="security-apis"></a>Sicherheits-APIs

| **Änderungstyp** | **Version** | **Beschreibung**              |
| :-------------- | :---------- | :--------------------------------------- |
| Ergänzungen        | Beta       | Eigenschaften **activityGroupName**, **cloudAppStates**, **confidence** und **registryKeyStates** zu [alert](/graph/api/resources/alert?view=graph-rest-beta ) hinzugefügt. |
|Löschung|Beta| Eigenschaften **activityGroupStates**, **applicationStates**, **malwareWasRunning**, **riskScore** und **type** aus [alert](/graph/api/resources/alert?view=graph-rest-beta ) entfernt. |
|Änderung|Beta| Typ **comments** von `String` in `String collection` geändert und Typ **severity** von `String` in [alertSeverity](/graph/api/resources/alertseverityenumtype?view=graph-rest-beta)-Enumeration in [alert](/graph/api/resources/alert?view=graph-rest-beta) geändert. |
| Ergänzungen        | Beta       | Die folgenden Ressourcentypen wurden hinzugefügt: <br/> [cloudAppSecurityState](/graph/api/resources/cloudappsecuritystate?view=graph-rest-beta) <br/> [fileHash](/graph/api/resources/filehash?view=graph-rest-beta) <br/> [registryKeyState](/graph/api/resources/registrykeystate?view=graph-rest-beta) |
|Löschung|Beta| Die folgenden Ressourcentypen wurden entfernt: <br/> **activityGroupState**  <br/> **applicationSecurityState** |
| Ergänzungen        | Beta       | Die folgenden Enumerationen wurden hinzugefügt: <br/> [alertSeverity](/graph/api/resources/alertseverityenumtype?view=graph-rest-beta) <br/> [connectionDirection](/graph/api/resources/connectiondirectionenumtype?view=graph-rest-beta) <br/> [connectionStatus](/graph/api/resources/connectionstatusenumtype?view=graph-rest-beta) <br/> [emailRole](/graph/api/resources/emailroleenumtype?view=graph-rest-beta) <br/> [fileHashType](/graph/api/resources/filehashtypeenumtype?view=graph-rest-beta) <br/> [registryHive](/graph/api/resources/registryhiveenumtype?view=graph-rest-beta)  <br/> [registryOperation](/graph/api/resources/registryoperationenumtype?view=graph-rest-beta) <br/> [registryValueType](/graph/api/resources/registryvaluetypeenumtype?view=graph-rest-beta)|
|Löschung|Beta| Folgende Enumerationstypen wurden entfernt: <br/> **alertType** <br/> **applicationPermissionsRequired** |
| Ergänzungen        | Beta       | Eigenschaft **fileHash** zu [fileSecurityState](/graph/api/resources/filesecuritystate?view=graph-rest-beta ) hinzugefügt.|
|Löschung|Beta| Eigenschaften **authenticodeHash256** und **sha256** aus [fileSecurityState](/graph/api/resources/filesecuritystate?view=graph-rest-beta) entfernt. |
| Ergänzungen | Beta | Eigenschaft **os** zu [hostSecurityState](/graph/api/resources/hostsecuritystate?view=graph-rest-beta) hinzugefügt.|
| Ergänzungen | Beta | Eigenschaften **category**, **family** und **wasRunning** zu [malwareState](/graph/api/resources/malwarestate?view=graph-rest-beta) hinzugefügt.|
|Löschung|Beta| Eigenschaft **aliases** aus [malwareState](/graph/api/resources/malwarestate?view=graph-rest-beta) entfernt. |
|Änderung|Beta| Eigenschaft **malwareWasRunning** von [alert](/graph/api/resources/alert?view=graph-rest-beta ) in [malwareState](/graph/api/resources/malwarestate?view=graph-rest-beta) verschoben und in **wasRunning** umbenannt. |
| Ergänzungen        | Beta       | Eigenschaften **applicationName**, **destinationDomain**, **direction**, **domainRegisteredDateTime**, **localDnsName**, **natDestinationAddress**, **natDestinationPort**, **natSourceAddress**, **natSourcePort**, **riskScore**, **status** und **urlParameters** zu [networkConnection](/graph/api/resources/networkconnection?view=graph-rest-beta ) hinzugefügt.|
|Änderung|Beta| Eigenschaft **uri** zu **destinationUrl** geändert in [networkConnection](/graph/api/resources/networkconnection?view=graph-rest-beta ). |
| Ergänzungen        | Beta       | Eigenschaft **fileHash** zu [process](/graph/api/resources/process?view=graph-rest-beta ) hinzugefügt.|
|Löschung|Beta| Eigenschaften **authenticodeHash256** und **sha256** aus [process](/graph/api/resources/process?view=graph-rest-beta ) entfernt. |
| Ergänzungen        | Beta       | Eigenschaften **aadUserId**, **emailRole**, **isVpn** und **logonIp** zu [userSecurityState](/graph/api/resources/usersecuritystate?view=graph-rest-beta) hinzugefügt.|
|Änderung|Beta| Eigenschaft **logonIpAddress** von **logonIp** in [userSecurityState](/graph/api/resources/usersecuritystate?view=graph-rest-beta) geändert. |
| Ergänzungen        | Beta       | Eigenschaft **wasRunning** zu [vulnerabilityState](/graph/api/resources/vulnerabilitystate?view=graph-rest-beta) hinzugefügt.|
|Löschung|Beta| Eigenschaft **name** aus [vulnerabilityState](/graph/api/resources/vulnerabilitystate?view=graph-rest-beta) entfernt. |

## <a name="july-2018"></a>Juli 2018

### <a name="application-and-serviceprincipal-api-changes"></a>Änderungen an der application- und servicePrincipal-API

| **Änderungstyp** | **Version** | **Beschreibung**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Änderung          | Beta        | The [application](/graph/api/resources/application?view=graph-rest-beta) and [servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-beta) APIs will be updated in preview (beta). The first set of changes will be applied on July 16, 2018. The changes include property renaming and restructuring. Most of the existing properties will not be available until the changes are completed. There will be new properties added. The changes will be released in preview (beta) prior to releasing to v1.0. |

### <a name="directory-apis"></a>Verzeichnis-APIs

| **Änderungstyp** | **Version**   | **Beschreibung**                          |
| :-------------- | :------------ | :--------------------------------------- |
|Änderung|Beta|[chatmessage](/graph/api/resources/chatmessage?view=graph-rest-beta)-Ressource aktualisiert|
|Ergänzungen|Beta|Ressourcentyp [Chat attachment](/graph/api/resources/chatattachment?view=graph-rest-beta) hinzugefügt|
|Ergänzungen|Beta|Ressourcentyp [Chat mention](/graph/api/resources/chatattachment?view=graph-rest-beta) hinzugefügt|
|Ergänzungen|Beta|Ressourcentyp [Chat reaction](/graph/api/resources/chatattachment?view=graph-rest-beta) hinzugefügt|
|Ergänzungen|Beta|[API zum Abrufen aller Kanalnachrichten](/graph/api/channel-list-messages?view=graph-rest-beta) hinzugefügt |
|Ergänzungen|Beta|[API zum Abrufen der Kanalnachricht](/graph/api/channel-get-message?view=graph-rest-beta) hinzugefügt |
|Ergänzungen|Beta|[API zum Abrufen aller Nachrichtenantworten](/graph/api/channel-list-messagereplies?view=graph-rest-beta) hinzugefügt |
|Ergänzungen|Beta|[API zum Abrufen einer Antwort auf eine Nachricht](/graph/api/channel-get-messagereply?view=graph-rest-beta) hinzugefügt |

### <a name="microsoft-teams-apis"></a>Microsoft Teams-APIs
| **Änderungstyp** | **Version**   | **Beschreibung**                          |
| :-------------- | :------------ | :--------------------------------------- |
|Ergänzungen|Beta|Unterstützung für Anwendungsberechtigungen zu [/users/{id}/joinedTeams](/graph/api/user-list-joinedteams?view=graph-rest-beta) hinzugefügt |
|Ergänzungen|Beta|[API zum Abrufen aller Kanalnachrichten](/graph/api/channel-list-messages?view=graph-rest-beta) hinzugefügt |
|Ergänzungen|Beta|[API zum Abrufen der Kanalnachricht](/graph/api/channel-get-message?view=graph-rest-beta) hinzugefügt |
|Ergänzungen|Beta|[API zum Abrufen aller Nachrichtenantworten](/graph/api/channel-list-messagereplies?view=graph-rest-beta) hinzugefügt |
|Ergänzungen|Beta|[API zum Abrufen einer Antwort auf eine Nachricht](/graph/api/channel-get-messagereply?view=graph-rest-beta) hinzugefügt |
|Ergänzungen|Beta|Ressourcentyp [Chat attachment](/graph/api/resources/chatattachment?view=graph-rest-beta) hinzugefügt|
|Ergänzungen|Beta|Ressourcentyp [Chat mention](/graph/api/resources/chatattachment?view=graph-rest-beta) hinzugefügt|
|Ergänzungen|Beta|Ressourcentyp [Chat reaction](/graph/api/resources/chatattachment?view=graph-rest-beta) hinzugefügt|
|Änderung|Beta|[chatmessage](/graph/api/resources/chatmessage?view=graph-rest-beta))-Ressource aktualisiert|
|Löschung|Beta|DELETE /groups/{id}/team/channels/{id} entfernt; verwenden Sie stattdessen DELETE /teams/{id}/channels/{id}. |
|Löschung|Beta|GET /groups/{id}/team/channels/{id} entfernt; verwenden Sie stattdessen GET /teams/{id}/channels/{id}. |
|Löschung|Beta|PATCH /groups/{id}/team/channels/{id} entfernt; verwenden Sie stattdessen PATCH /teams/{id}/channels/{id}. |
|Löschung|Beta|POST /groups/{id}/team/channels/{id}/chatthreads entfernt; verwenden Sie stattdessen POST /teams/{id}/channels/{id}/chatthreads. |
|Löschung|Beta|GET /groups/{id}/team/channels entfernt; verwenden Sie stattdessen GET /teams/{id}/channels. |
|Löschung|Beta|DELETE /groups/{id}/channels/{id} entfernt; verwenden Sie stattdessen DELETE /teams/{id}/channels/{id}. |
|Löschung|Beta|GET /groups/{id}/channels/{id} entfernt; verwenden Sie stattdessen GET /teams/{id}/channels/{id}. |
|Löschung|Beta|PATCH /groups/{id}/channels/{id} entfernt; verwenden Sie stattdessen PATCH /teams/{id}/channels/{id}. |
|Löschung|Beta|POST /groups/{id}/channels/{id}/chatthreads entfernt; verwenden Sie stattdessen POST /teams/{id}/channels/{id}/chatthreads. |
|Löschung|Beta|GET /groups/{id}/channels entfernt; verwenden Sie stattdessen GET /teams/{id}/channels. |
|Löschung|Beta|POST /groups/{id}/team/channels entfernt; verwenden Sie stattdessen POST /teams/{id}/channels. |
|Löschung|Beta|GET /groups/{id}/team entfernt; verwenden Sie stattdessen GET /teams/{id}. |
|Löschung|Beta|PATCH /groups/{id}/team entfernt; verwenden Sie stattdessen PATCH /teams/{id}. |
|Ergänzungen|Beta|API zum [Auflisten aller Teams in der Organisation](teams-list-all-teams.md) hinzugefügt. |

### <a name="outlook-contacts"></a>Outlook-Kontakte
| **Änderungstyp** | **Version**   | **Beschreibung**                          |
|:--------------- |:------------- |:---------------------------------------- |
|Ergänzungen |Beta | Komplexer Typ [typedEmailAddress](/graph/api/resources/typedemailaddress?view=graph-rest-beta) hinzugefügt. |
|Änderung | Beta | Typ der **emailAddresses**-Eigenschaft des [Kontakts wurde](/graph/api/resources/contact?view=graph-rest-beta) zu einer Sammlung von **typedEmailAddress**-Instanzen geändert.|

### <a name="synchronization-apis"></a>Synchronisierungs-APIs

| **Änderungstyp** | **Version**   | **Beschreibung**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Ergänzungen | Beta | Eigenschaft **progress** zu [sychronizationStatus](/graph/api/resources/synchronization-synchronizationstatus?view=graph-rest-beta) hinzugefügt, damit Clients den Fortschritt des Synchronisierungsauftrags überwachen können.|

### <a name="webhooks"></a>Webhooks
| Änderungstyp | Version | Beschreibung                              |
|:------------|:--------|:-----------------------------------------|
| Änderungen | Beta und Version 1.0 | Reduzierte [maximale Abonnmentablaufdauer](/graph/api/resources/subscription?view=graph-rest-1.0#maximum-length-of-subscription-per-resource-type) für [Webhooks](/graph/api/resources/webhooks?view=graph-rest-1.0) bei Laufwerkstammelementen auf 3 Tage. |


## <a name="june-2018"></a>Juni 2018

### <a name="directory-apis"></a>Verzeichnis-APIs

| **Änderungstyp** | **Version**   | **Beschreibung**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Ergänzungen | Alle | Die neuen Anwendungsberechtigungen _Application.ReadWrite.All_ und _Application.ReadWrite.OwnedBy_ ermöglichen der Client-App, Anwendungen und Dienstprinzipale zu erstellen, lesen, aktualisieren und löschen, wie im [Thema zu Berechtigungen](permissions-reference.md#application-resource-permissions) beschrieben. |
| Ergänzungen | v1.0 | Eigenschaften **ageGroup**, **legalAgeGroupClassification** und **ConsentRequiredForMinor** zur Ressource [user](/graph/api/resources/user?view=graph-rest-1.0) hinzugefügt

### <a name="identity-and-access-apis"></a>APIs für Identität und Zugriff

| **Änderungstyp** | **Version**   | **Beschreibung**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Ergänzungen | Beta | Feature [access reviews](/graph/api/resources/accessreviews-root?view=graph-rest-beta) in [Azure AD](/graph/api/resources/azure-ad-overview?view=graph-rest-beta) hinzugefügt. |

### <a name="microsoft-intune-apis"></a>Microsoft Intune-APIs

|Änderungstyp|Version|Beschreibung|
|:---|:---|:---|
|Ergänzungen|v1.0|Die Eigenschaft **connectorServerName** wurde zur Entität [deviceManagementExchangeConnector](/graph/api/resources/intune-onboarding-devicemanagementexchangeconnector?view=graph-rest-1.0) hinzugefügt.|
|Ergänzungen|v1.0|Die Eigenschaften **firewallEnabled**, **firewallBlockAllIncoming** und **firewallEnableStealthMode** wurden der Entität [macOSCompliancePolicy](/graph/api/resources/intune-deviceconfig-macoscompliancepolicy?view=graph-rest-1.0) hinzugefügt.|
|Ergänzungen|v1.0|Das Mitglied **unknown** wurde dem Enum-Typ [iosUpdatesInstallStatus](/graph/api/resources/intune-deviceconfig-iosupdatesinstallstatus?view=graph-rest-1.0) hinzugefügt.|
|Ergänzungen|Beta|Hinzugefügte neue Entitäten:<br/>[androidDeviceOwnerWiFiConfiguration](/graph/api/resources/intune-deviceconfig-androiddeviceownerwificonfiguration?view=graph-rest-beta)<br/>[iosVppAppAssignedDeviceLicense](/graph/api/resources/intune-apps-iosvppappassigneddevicelicense?view=graph-rest-beta)<br/>[iosVppAppAssignedLicense](/graph/api/resources/intune-apps-iosvppappassignedlicense?view=graph-rest-beta)<br/>[iosVppAppAssignedUserLicense](/graph/api/resources/intune-apps-iosvppappassigneduserlicense?view=graph-rest-beta)<br/>[managedDeviceMobileAppConfigurationState](/graph/api/resources/intune-deviceconfig-manageddevicemobileappconfigurationstate?view=graph-rest-beta)<br/>[userPFXCertificate](/graph/api/resources/intune-raimportcerts-userpfxcertificate?view=graph-rest-beta)<br/>[vppTokenLicenseSummary](/graph/api/resources/intune-onboarding-vpptokenlicensesummary?view=graph-rest-beta)<br/>|
|Ergänzungen|Beta|Die folgenden komplexen Typen wurden hinzugefügt:<br/>[iosVppAppRevokeLicensesActionResult](/graph/api/resources/intune-apps-iosvppapprevokelicensesactionresult?view=graph-rest-beta)<br/>|
|Ergänzungen|Beta|Neue Enumerationstypen hinzugefügt:<br/>[androidDeviceOwnerSystemUpdateInstallType](/graph/api/resources/intune-deviceconfig-androiddeviceownersystemupdateinstalltype?view=graph-rest-beta)<br/>[androidDeviceOwnerWiFiSecurityType](/graph/api/resources/intune-deviceconfig-androiddeviceownerwifisecuritytype?view=graph-rest-beta)<br/>[userPfxIntendedPurpose](/graph/api/resources/intune-raimportcerts-userpfxintendedpurpose?view=graph-rest-beta)<br/>[userPfxPaddingScheme](/graph/api/resources/intune-raimportcerts-userpfxpaddingscheme?view=graph-rest-beta)<br/>|
|Ergänzungen|Beta|Die Aktion [createGooglePlayWebToken](/graph/api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-creategoogleplaywebtoken?view=graph-rest-beta) wurde für [androidManagedStoreAccountEnterpriseSettings](/graph/api/resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings?view=graph-rest-beta) hinzugefügt. |
|Ergänzungen|Beta|Die Aktion [revokeAllLicenses](/graph/api/intune-apps-iosvppapp-revokealllicenses?view=graph-rest-beta) wurde für [iosVppApp](/graph/api/resources/intune-apps-iosvppapp?view=graph-rest-beta) hinzugefügt. |
|Ergänzungen|Beta|Die Aktion [revokeUserLicense](/graph/api/intune-apps-iosvppapp-revokeuserlicense?view=graph-rest-beta) wurde für [iosVppApp](/graph/api/resources/intune-apps-iosvppapp?view=graph-rest-beta) hinzugefügt. |
|Ergänzungen|Beta|Die Aktion [revokeDeviceLicense](/graph/api/intune-apps-iosvppapp-revokedevicelicense?view=graph-rest-beta) wurde für [iosVppApp](/graph/api/resources/intune-apps-iosvppapp?view=graph-rest-beta) hinzugefügt. |
|Ergänzungen|Beta|Die Aktion [sendCustomNotificationToCompanyPortal](/graph/api/intune-shared-devicemanagement-sendcustomnotificationtocompanyportal?view=graph-rest-beta) wurde für [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta) hinzugefügt. |
|Ergänzungen|Beta|Die Funktion **getLicensesForApp** wurde zur Sammlung [vppToken](/graph/api/resources/intune-onboarding-vpptoken?view=graph-rest-beta) hinzugefügt. |
|Löschung|Beta|Folgende Enumerationstypen wurden entfernt:<br/>**windowsUpdateInsiderBuildControl**<br/>|
|Ergänzungen|Beta|Die Eigenschaften **systemUpdateWindowStartMinutesAfterMidnight**, **systemUpdateWindowEndMinutesAfterMidnight** und **systemUpdateInstallType** wurden der Entität [androidDeviceOwnerGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration?view=graph-rest-beta) hinzugefügt.|
|Ändern|Beta|Der Typ der folgenden Eigenschaften in der Entität [androidDeviceOwnerGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration?view=graph-rest-beta) wurde geändert:<br/>**passwordMinutesOfInactivityBeforeScreenTimeout** von Int64 in Int32<br/>|
|Ergänzungen|Beta|Die Eigenschaft **customKeyValueData** wurde der Entität [androidForWorkVpnConfiguration](/graph/api/resources/intune-deviceconfig-androidforworkvpnconfiguration?view=graph-rest-beta) hinzugefügt.|
|Ergänzungen|Beta|Die Eigenschaft **customKeyValueData** wurde der Entität [androidVpnConfiguration](/graph/api/resources/intune-deviceconfig-androidvpnconfiguration?view=graph-rest-beta) hinzugefügt.|
|Ergänzungen|Beta|Die Eigenschaft **customKeyValueData** wurde der Entität [androidWorkProfileVpnConfiguration](/graph/api/resources/intune-deviceconfig-androidworkprofilevpnconfiguration?view=graph-rest-beta) hinzugefügt.|
|Ergänzungen|Beta|Die Eigenschaft **customKeyValueData** wurde der Entität [appleVpnConfiguration](/graph/api/resources/intune-deviceconfig-applevpnconfiguration?view=graph-rest-beta) hinzugefügt.|
|Ergänzungen|Beta|Die Eigenschaften **userId** und **userPrincipalName** wurden der Entität [deviceCompliancePolicyState](/graph/api/resources/intune-deviceconfig-devicecompliancepolicystate?view=graph-rest-beta) hinzugefügt.|
|Ergänzungen|Beta|Die Eigenschaften **userId** und **userPrincipalName** wurden der Entität [deviceConfigurationState](/graph/api/resources/intune-deviceconfig-deviceconfigurationstate?view=graph-rest-beta) hinzugefügt.|
|Ergänzungen|Beta|Die Eigenschaft **connectorServerName** wurde zur Entität [deviceManagementExchangeConnector](/graph/api/resources/intune-onboarding-devicemanagementexchangeconnector?view=graph-rest-beta) hinzugefügt.|
|Löschung|Beta|Die Eigenschaft **settingXml** wurde aus der Entität [iosMobileAppConfiguration](/graph/api/resources/intune-apps-iosmobileappconfiguration?view=graph-rest-beta) entfernt.|
|Ergänzungen|Beta|Die Eigenschaften **vppTokenId** und **revokeLicenseActionResults** wurden der Entität [iosVppApp](/graph/api/resources/intune-apps-iosvppapp?view=graph-rest-beta) hinzugefügt.|
|Ergänzungen|Beta|Die Eigenschaften **firewallEnabled**, **firewallBlockAllIncoming** und **firewallEnableStealthMode** wurden der Entität [macOSCompliancePolicy](/graph/api/resources/intune-deviceconfig-macoscompliancepolicy?view=graph-rest-beta) hinzugefügt.|
|Löschung|Beta|Die Eigenschaft **remoteAssistanceSessionErrorString** wurde aus der Entität [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) entfernt.|
|Ergänzungen|Beta|Die Eigenschaften **antivirusRequired** und **antiSpywareRequired** wurden zur Entität [windows10CompliancePolicy](/graph/api/resources/intune-deviceconfig-windows10compliancepolicy?view=graph-rest-beta) hinzugefügt.|
|Ergänzungen|Beta|Die Eigenschaften **defenderOfficeAppsOtherProcessInjection**, **defenderOfficeAppsExecutableContentCreationOrLaunch**, **defenderOfficeAppsLaunchChildProcess**, **defenderOfficeMacroCodeAllowWin32Imports**, **defenderScriptObfuscatedMacroCode**, **defenderScriptDownloadedPayloadExecution**, **defenderProcessCreation**, **defenderUntrustedUSBProcess**, **defenderUntrustedExecutable** und **defenderEmailContentExecution** wurden der Entität [windows10EndpointProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windows10endpointprotectionconfiguration?view=graph-rest-beta) hinzugefügt.|
|Ergänzungen|Beta|Die Eigenschaften **searchDisableLocation**, **inkWorkspaceAccessState**, **defenderPotentiallyUnwantedAppActionSetting** und **defenderCloudExtendedTimeoutInSeconds** wurden der Entität [windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta) hinzugefügt.|
|Ergänzungen|Beta|Die Eigenschaft **updatesMinimumAutoInstallClassification** wurde der Entität [windows81GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows81generalconfiguration?view=graph-rest-beta) hinzugefügt.|
|Löschung|Beta|Die Eigenschaft **previewBuildSetting** wurde aus der Entität [windowsUpdateForBusinessConfiguration](/graph/api/resources/intune-deviceconfig-windowsupdateforbusinessconfiguration?view=graph-rest-beta) entfernt.|
|Ergänzungen|Beta|Die Navigationseigenschaft **userPfxCertificates**wurde der Entität [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta) hinzugefügt.|
|Ergänzungen|Beta|Die Navigationseigenschaft **assignedLicenses** wurde der Entität [iosVppApp](/graph/api/resources/intune-apps-iosvppapp?view=graph-rest-beta) hinzugefügt.|
|Ergänzungen|Beta|Die Navigationseigenschaft **managedDeviceMobileAppConfigurationStates** wurde der Entität [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) hinzugefügt.|
|Ergänzungen|Beta|Die Eigenschaft **websiteList** wurde dem komplexen Typ [iosWebContentFilterSpecificWebsitesAccess](/graph/api/resources/intune-deviceconfig-ioswebcontentfilterspecificwebsitesaccess?view=graph-rest-beta) hinzugefügt.|
|Ergänzungen|Beta|Das Mitglied **androidWorkProfile** wurde dem Enum-Typ [devicePlatformType](/graph/api/resources/intune-deviceconfig-deviceplatformtype?view=graph-rest-beta) hinzugefügt.|
|Ergänzungen|Beta|Das Mitglied **notConfigured** wurde dem Enum-Typ [editionUpgradeLicenseType](/graph/api/resources/intune-deviceconfig-editionupgradelicensetype?view=graph-rest-beta) hinzugefügt.|
|Ergänzungen|Beta|Das Mitglied **unknown** wurde dem Enum-Typ [iosUpdatesInstallStatus](/graph/api/resources/intune-deviceconfig-iosupdatesinstallstatus?view=graph-rest-beta) hinzugefügt.|
|Ergänzungen|Beta|Das Mitglied **userRequestedInstall** wurde dem Enum-Typ [mobileAppActionType](/graph/api/resources/intune-troubleshooting-mobileappactiontype?view=graph-rest-beta) hinzugefügt.|
|Ergänzungen|Beta|Das Mitglied **notConfigured** wurde dem Enum-Typ [windows10EditionType](/graph/api/resources/intune-deviceconfig-windows10editiontype?view=graph-rest-beta) hinzugefügt.

### <a name="microsoft-teams-apis"></a>Microsoft Teams-APIs
| **Änderungstyp** | **Version**   | **Beschreibung**                          |
| :-------------- | :------------ | :--------------------------------------- |
|Ergänzungen         | Beta          | Die Team-APIs [archive](/graph/api/team-archive?view=graph-rest-beta) und [unarchive](/graph/api/team-unarchive?view=graph-rest-beta) wurden hinzugefügt.|
|Ergänzungen         | Beta          | Team-Operation [clone](/graph/api/team-clone?view=graph-rest-beta) wurde hinzugefügt. |
|Ergänzungen         | Beta          | APIs zum Hinzufügen und Entfernen von [Apps](/graph/api/resources/teamsapp?view=graph-rest-beta) wurden zu Teams hinzugefügt. |
|Ändern|Beta|Pfad zur Entität [team](/graph/api/resources/team?view=graph-rest-beta) wurde aktualisiert.|
|Ändern|Beta|Pfad zu Entität [channel](/graph/api/resources/channel?view=graph-rest-beta) aktualisiert.|


### <a name="privileged-identity-management-apis"></a>Privileged Identity Management-APIs

| **Änderungstyp** | **Version**   | **Beschreibung**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Ergänzungen | Beta | Die Entität [privilegedAccess](/graph/api/resources/privilegedaccess?view=graph-rest-beta) wurde hinzugefügt.|
| Ergänzungen | Beta | Die Entität [governanceResource](/graph/api/resources/governanceresource?view=graph-rest-beta) sowie die folgenden Methoden und Aktionen wurden hinzugefügt: <br> [List](/graph/api/governanceresource-list?view=graph-rest-beta) <br> [Get](/graph/api/governanceresource-get?view=graph-rest-beta)<br>|
| Ergänzungen | Beta | Die Entität [governanceSubject](/graph/api/resources/governancesubject?view=graph-rest-beta) wurde hinzugefügt.|
| Ergänzungen | Beta | Die Entität [governanceRoleDefinition](/graph/api/resources/governanceroledefinition?view=graph-rest-beta) sowie die folgenden Methoden und Aktionen wurden hinzugefügt:<br> [List](/graph/api/governanceroledefinition-list?view=graph-rest-beta) <br> [Get](/graph/api/governanceroledefinition-get?view=graph-rest-beta) |
| Ergänzungen | Beta | Die Entität [governanceRoleAssignment](/graph/api/resources/governanceroleassignment?view=graph-rest-beta) sowie die folgenden Methoden und Aktionen wurden hinzugefügt:<br> [List](/graph/api/governanceroleassignment-list?view=graph-rest-beta) <br> [Get](/graph/api/governanceroleassignment-get?view=graph-rest-beta) <br> [Export](/graph/api/governanceroleassignment-export?view=graph-rest-beta) |
| Ergänzungen | Beta | Die Entität [governanceRoleAssignmentRequest](/graph/api/resources/governanceroleassignmentrequest?view=graph-rest-beta) sowie die folgenden Methoden und Aktionen wurden hinzugefügt:<br> [List](/graph/api/governanceroleassignmentrequest-list?view=graph-rest-beta) <br> [Get](/graph/api/governanceroleassignmentrequest-get?view=graph-rest-beta) <br> [Create](/graph/api/governanceroleassignmentrequest-post?view=graph-rest-beta) <br> [Cancel](/graph/api/governanceroleassignmentrequest-cancel?view=graph-rest-beta) <br> [Update](/graph/api/governanceroleassignmentrequest-update?view=graph-rest-beta) |
| Ergänzungen | Beta | Die Entität [governanceRoleSetting](/graph/api/resources/governancerolesetting?view=graph-rest-beta) sowie die folgenden Methoden und Aktionen wurden hinzugefügt:<br> [List](/graph/api/governancerolesetting-list?view=graph-rest-beta) <br> [Get](/graph/api/governancerolesetting-get?view=graph-rest-beta) <br> [Update](/graph/api/governancerolesetting-update?view=graph-rest-beta) |
| Ergänzungen | Beta | Folgende komplexe Typen hinzugefügt: <br> [governancePermission](/graph/api/resources/governancepermission?view=graph-rest-beta) <br> [governanceRoleAssignmentRequestStatus](/graph/api/resources/governanceroleassignmentrequeststatus?view=graph-rest-beta) <br> [governanceRuleSetting](/graph/api/resources/governancerulesetting?view=graph-rest-beta) <br> [governanceSchedule](/graph/api/resources/governanceschedule?view=graph-rest-beta)|

### <a name="security-apis"></a>Sicherheits-APIs

| **Änderungstyp** | **Version**   | **Beschreibung**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Ergänzungen        | Beta        | Neue Enumerationstypen hinzugefügt:<br/>[alertFeedback](/graph/api/resources/alertfeedbackenumtype?view=graph-rest-beta)<br/>[alertStatus](/graph/api/resources/alertstatusenumtype?view=graph-rest-beta)<br/>[alertType](/graph/api/resources/alerttypeenumtype?view=graph-rest-beta)<br/>[applicationPermissionsRequired](/graph/api/resources/applicationpermissionsrequiredenumtype?view=graph-rest-beta)<br/>[logonType](/graph/api/resources/logontypeenumtype?view=graph-rest-beta)<br/>[processIntegrityLevel](/graph/api/resources/processintegritylevelenumtype?view=graph-rest-beta)<br/>[securityNetworkProtocol](/graph/api/resources/securitynetworkprotocolenumtype?view=graph-rest-beta)<br/>[userAccountSecurityType](/graph/api/resources/useraccountsecuritytypeenumtype?view=graph-rest-beta)<br/>

## <a name="may-2018"></a>Mai 2018

### <a name="azure-ad-apis"></a>Azure AD-APIs

| **Änderungstyp** | **Version**   | **Beschreibung**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Änderung           | Beta          | Die **creatorUserId**-Eigenschaft der [subscription](/graph/api/resources/subscription?view=graph-rest-beta)-Entität wurde in **creatorId** geändert, damit ihre Bedeutung deutlicher wird. |

### <a name="directory-apis"></a>Verzeichnis-APIs

| **Änderungstyp** | **Version**   | **Beschreibung**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Ergänzungen        | v1.0        | Die Aktion [Gelöschte Elemente im Besitz eines Benutzers auflisten](/graph/api/directory-deleteditems-user-owned?view=graph-rest-1.0) wurde der Ressource [directory (deleted items)](/graph/api/resources/directory?view=graph-rest-1.0) hinzugefügt. |
| Ergänzungen | Beta | Die [getUserOwnedObjects](/graph/api/directory-deleteditems-user-owned?view=graph-rest-beta)-Funktion wurde der [directory](/graph/api/resources/directory?view=graph-rest-beta)-Ressource hinzugefügt, um die gelöschten Gruppen aufzuführen, die im Besitz eines bestimmten Benutzers sind. |

### <a name="education-api"></a>Bildungs-API

| **Änderungstyp** | **Version**   | **Beschreibung**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Änderung          | v1.0 und Beta | Der Bereich **Members.Read.Hidden** ist erforderlich, um die Auflistung **Members** in einer [educationClass](/graph/api/resources/educationclass?view=graph-rest-1.0)-Entität mithilfe von Nur-App-Token zu lesen oder zu aktualisieren. |
|Änderung           |Beta           |Die zulässigen Werte für den **educationSubmissionStatus**-Typ in der Statuseigenschaft von [educationsubmission](/graph/api/resources/educationsubmission?view=graph-rest-beta) wurden aktualisiert.|
|Änderung           |Beta           |Der komplexe **educationAssignmentIndividualRecipient**-Typ wurde der assignTo-Eigenschaft von [educationAssignment](/graph/api/resources/educationassignment?view=graph-rest-beta) hinzugefügt.|
|Änderung           |Beta           |Die **unsubmittedBy**-, **unsubmittedDate**-, **ReturnedBy**-, **ReturnedDate**-Eigenschaften von [educationSubmission](/graph/api/resources/educationsubmission?view=graph-rest-beta) wurden hinzugefügt.|
|Ergänzungen         |Beta           |Die [return](/graph/api/educationsubmission-return?view=graph-rest-beta)- und [unsubmit](/graph/api/educationsubmission-unsubmit?view=graph-rest-beta)-Aktionen wurden zu [educationSubmission](/graph/api/resources/educationsubmission?view=graph-rest-beta) hinzugefügt.|
|Änderung           |Beta           |Die release- und recall-Aktionen wurden aus [educationSubmission](/graph/api/resources/educationsubmission?view=graph-rest-beta) entfernt.|

### <a name="groups"></a>Gruppen

| **Änderungstyp** | **Version**   | **Beschreibung**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Ergänzungen        | v1.0 und Beta | Eigenschaft **importance** zur Entität [post](/graph/api/resources/post?view=graph-rest-1.0) hinzugefügt. |

### <a name="insights-api"></a>Insights-API

| **Änderungstyp** | **Version**   | **Beschreibung**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Ergänzungen        | Beta          | Entität [settings](/graph/api/resources/user-settings?view=graph-rest-beta) sowie folgende CRUD-Methoden hinzugefügt: <br> [Get](/graph/api/user-get-settings?view=graph-rest-beta) <br> [Update](/graph/api/user-update-settings?view=graph-rest-beta) |

### <a name="microsoft-bookings-api"></a>Microsoft Bookings-API

| **Änderungstyp** | **Version**   | **Beschreibung**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Ergänzungen        | Beta          | Entität [bookingBusiness](/graph/api/resources/bookingbusiness?view=graph-rest-beta) sowie folgende CRUD-Methoden und -Aktionen hinzugefügt: <br> [List](/graph/api/bookingbusiness-list?view=graph-rest-beta) <br> [Create](/graph/api/bookingbusiness-post-bookingbusinesses?view=graph-rest-beta) <br> [Get](/graph/api/bookingbusiness-get?view=graph-rest-beta) <br> [Aktualisieren](/graph/api/bookingbusiness-update?view=graph-rest-beta) <br> [Delete](/graph/api/bookingbusiness-delete?view=graph-rest-beta) <br> [Publish](/graph/api/bookingbusiness-publish?view=graph-rest-beta) <br> [Unpublish](/graph/api/bookingbusiness-unpublish?view=graph-rest-beta) <br> Unter diesem Link erfahren Sie mehr über die Integration mit der [Microsoft Bookings-API](booking-concept-overview.md). |
| Ergänzungen        | Beta          | Entität [bookingAppointment](/graph/api/resources/bookingappointment?view=graph-rest-beta) sowie folgende CRUD-Methoden und -Aktionen hinzugefügt: <br> [List](/graph/api/bookingbusiness-list-appointments?view=graph-rest-beta) <br> [Create](/graph/api/bookingbusiness-post-appointments?view=graph-rest-beta) <br> [Get](/graph/api/bookingappointment-get?view=graph-rest-beta) <br> [Aktualisieren](/graph/api/bookingappointment-update?view=graph-rest-beta) <br> [Delete](/graph/api/bookingappointment-delete?view=graph-rest-beta) <br> [Cancel](/graph/api/bookingappointment-cancel?view=graph-rest-beta) |
| Ergänzungen        | Beta          | Entität [bookingCurrency](/graph/api/resources/bookingcurrency?view=graph-rest-beta) sowie folgende Methoden hinzugefügt: <br> [List](/graph/api/bookingcurrency-list?view=graph-rest-beta) <br> [Get](/graph/api/bookingcurrency-get?view=graph-rest-beta) |
| Ergänzungen        | Beta          | Entität [bookingCustomer](/graph/api/resources/bookingcustomer?view=graph-rest-beta) sowie folgende CRUD-Methoden hinzugefügt: <br> [List](/graph/api/bookingbusiness-list-customers?view=graph-rest-beta) <br> [Create](/graph/api/bookingbusiness-post-customers?view=graph-rest-beta) <br> [Get](/graph/api/bookingcustomer-get?view=graph-rest-beta) <br> [Update](/graph/api/bookingcustomer-update?view=graph-rest-beta) <br> [Delete](/graph/api/bookingcustomer-delete?view=graph-rest-beta)|
| Ergänzungen        | Beta          | Entität [bookingService](/graph/api/resources/bookingservice?view=graph-rest-beta) sowie folgende CRUD-Methoden hinzugefügt: <br> [List](/graph/api/bookingbusiness-list-services?view=graph-rest-beta) <br> [Create](/graph/api/bookingbusiness-post-services?view=graph-rest-beta) <br> [Get](/graph/api/bookingservice-get?view=graph-rest-beta) <br> [Update](/graph/api/bookingservice-update?view=graph-rest-beta) <br> [Delete](/graph/api/bookingservice-delete?view=graph-rest-beta)|
| Ergänzungen        | Beta          | Entität [bookingStaffMember](/graph/api/resources/bookingstaffmember?view=graph-rest-beta) sowie folgende CRUD-Methoden hinzugefügt: <br> [List](/graph/api/bookingbusiness-list-staffmembers?view=graph-rest-beta) <br> [Create](/graph/api/bookingbusiness-post-staffmembers?view=graph-rest-beta) <br> [Get](/graph/api/bookingstaffmember-get?view=graph-rest-beta) <br> [Update](/graph/api/bookingstaffmember-update?view=graph-rest-beta) <br> [Delete](/graph/api/bookingstaffmember-delete?view=graph-rest-beta)|
| Ergänzungen        | Beta          | Folgende komplexe Typen hinzugefügt: <br> [bookingNamedEntity](/graph/api/resources/bookingnamedentity?view=graph-rest-beta) <br> [bookingPerson](/graph/api/resources/bookingperson?view=graph-rest-beta) <br> [bookingReminder](/graph/api/resources/bookingreminder?view=graph-rest-beta) <br> [bookingWorkHours](/graph/api/resources/bookingworkhours?view=graph-rest-beta) <br> [bookingWorkTimeSlot](/graph/api/resources/bookingworktimeslot?view=graph-rest-beta).|

### <a name="microsoft-intune-apis"></a>Microsoft Intune-APIs
|Änderungstyp|Version|Beschreibung|
|:---|:---|:---|
|Ergänzungen|Beta|Hinzugefügte neue Entitäten:<br/>[androidWorkProfileCompliancePolicy](/graph/api/resources/intune-deviceconfig-androidworkprofilecompliancepolicy?view=graph-rest-beta)<br/>[easEmailProfileConfigurationBase](/graph/api/resources/intune-deviceconfig-easemailprofileconfigurationbase?view=graph-rest-beta)<br/>[mobileAppIntentAndState](/graph/api/resources/intune-troubleshooting-mobileappintentandstate?view=graph-rest-beta)<br/>[mobileAppTroubleshootingEvent](/graph/api/resources/intune-troubleshooting-mobileapptroubleshootingevent?view=graph-rest-beta)<br/>[unsupportedDeviceConfiguration](/graph/api/resources/intune-deviceconfig-unsupporteddeviceconfiguration?view=graph-rest-beta)<br/>[windowsKioskConfiguration](/graph/api/resources/intune-deviceconfig-windowskioskconfiguration?view=graph-rest-beta)<br/>|
|Ergänzungen|Beta|Die folgenden komplexen Typen wurden hinzugefügt:<br/>[managedDeviceCleanupSettings](/graph/api/resources/intune-devices-manageddevicecleanupsettings?view=graph-rest-beta)<br/>[mobileAppIntentAndStateDetail](/graph/api/resources/intune-troubleshooting-mobileappintentandstatedetail?view=graph-rest-beta)<br/>[mobileAppTroubleshootingAppPolicyCreationHistory](/graph/api/resources/intune-troubleshooting-mobileapptroubleshootingapppolicycreationhistory?view=graph-rest-beta)<br/>[mobileAppTroubleshootingAppStateHistory](/graph/api/resources/intune-troubleshooting-mobileapptroubleshootingappstatehistory?view=graph-rest-beta)<br/>[mobileAppTroubleshootingAppTargetHistory](/graph/api/resources/intune-troubleshooting-mobileapptroubleshootingapptargethistory?view=graph-rest-beta)<br/>[mobileAppTroubleshootingAppUpdateHistory](/graph/api/resources/intune-troubleshooting-mobileapptroubleshootingappupdatehistory?view=graph-rest-beta)<br/>[mobileAppTroubleshootingDeviceCheckinHistory](/graph/api/resources/intune-troubleshooting-mobileapptroubleshootingdevicecheckinhistory?view=graph-rest-beta)<br/>[mobileAppTroubleshootingHistoryItem](/graph/api/resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem?view=graph-rest-beta)<br/>[unsupportedDeviceConfigurationDetail](/graph/api/resources/intune-deviceconfig-unsupporteddeviceconfigurationdetail?view=graph-rest-beta)<br/>**windowsAutoPilotEnrollmentSettings**<br/>[windowsKioskActiveDirectoryGroup](/graph/api/resources/intune-deviceconfig-windowskioskactivedirectorygroup?view=graph-rest-beta)<br/>[windowsKioskAppBase](/graph/api/resources/intune-deviceconfig-windowskioskappbase?view=graph-rest-beta)<br/>[windowsKioskAppConfiguration](/graph/api/resources/intune-deviceconfig-windowskioskappconfiguration?view=graph-rest-beta)<br/>[windowsKioskAutologon](/graph/api/resources/intune-deviceconfig-windowskioskautologon?view=graph-rest-beta)<br/>[windowsKioskAzureADGroup](/graph/api/resources/intune-deviceconfig-windowskioskazureadgroup?view=graph-rest-beta)<br/>[windowsKioskAzureADUser](/graph/api/resources/intune-deviceconfig-windowskioskazureaduser?view=graph-rest-beta)<br/>[windowsKioskDesktopApp](/graph/api/resources/intune-deviceconfig-windowskioskdesktopapp?view=graph-rest-beta)<br/>[windowsKioskLocalGroup](/graph/api/resources/intune-deviceconfig-windowskiosklocalgroup?view=graph-rest-beta)<br/>[windowsKioskLocalUser](/graph/api/resources/intune-deviceconfig-windowskiosklocaluser?view=graph-rest-beta)<br/>[windowsKioskMultipleApps](/graph/api/resources/intune-deviceconfig-windowskioskmultipleapps?view=graph-rest-beta)<br/>[windowsKioskProfile](/graph/api/resources/intune-deviceconfig-windowskioskprofile?view=graph-rest-beta)<br/>[windowsKioskSingleUWPApp](/graph/api/resources/intune-deviceconfig-windowskiosksingleuwpapp?view=graph-rest-beta)<br/>[windowsKioskUser](/graph/api/resources/intune-deviceconfig-windowskioskuser?view=graph-rest-beta)<br/>[windowsKioskUWPApp](/graph/api/resources/intune-deviceconfig-windowskioskuwpapp?view=graph-rest-beta)<br/>[windowsKioskVisitor](/graph/api/resources/intune-deviceconfig-windowskioskvisitor?view=graph-rest-beta)<br/>|
|Ergänzungen|Beta|Neue Enumerationstypen hinzugefügt:<br/>[defenderScheduleScanDay](/graph/api/resources/intune-deviceconfig-defenderschedulescanday?view=graph-rest-beta)<br/>[defenderSubmitSamplesConsentType](/graph/api/resources/intune-deviceconfig-defendersubmitsamplesconsenttype?view=graph-rest-beta)<br/>[domainNameSource](/graph/api/resources/intune-deviceconfig-domainnamesource?view=graph-rest-beta)<br/>[localSecurityOptionsSmartCardRemovalBehaviorType](/graph/api/resources/intune-deviceconfig-localsecurityoptionssmartcardremovalbehaviortype?view=graph-rest-beta)<br/>[mobileAppActionType](/graph/api/resources/intune-troubleshooting-mobileappactiontype?view=graph-rest-beta)<br/>[mobileAppIntent](/graph/api/resources/intune-troubleshooting-mobileappintent?view=graph-rest-beta)<br/>[roleAssignmentScopeType](/graph/api/resources/intune-rbac-roleassignmentscopetype?view=graph-rest-beta)<br/>[usernameSource](/graph/api/resources/intune-deviceconfig-usernamesource?view=graph-rest-beta)<br/>[windowsDeviceUsageType](/graph/api/resources/intune-enrollment-windowsdeviceusagetype?view=graph-rest-beta)<br/>|
|Ergänzungen|Beta|Die [setDeviceName](/graph/api/intune-devices-manageddevice-setdevicename?view=graph-rest-beta)-Aktion<br/>wurde zu [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) hinzugefügt. |
|Löschung|Beta|Die folgenden Entitäten wurden entfernt:<br/>**depEnrollmentProfile**<br/>**enrollmentProfile**<br/>**importedAppleDeviceIdentity**<br/>**importedAppleDeviceIdentityResult**<br/>|
|Löschung|Beta|Die folgenden komplexen Typen wurden entfernt:<br/>**managementCertificateWithThumbprint**<br/>|
|Löschung|Beta|Folgende Enumerationstypen wurden entfernt:<br/>**depTokenType**<br/>**discoverySource**<br/>**iTunesPairingMode**<br/>|
|Löschung|Beta|Die Aktion „ImportAppleDeviceIdentityList“ wurde aus der [importedAppleDeviceIdentity](/graph/api/resources/intune-corpenrollment-importedappledeviceidentity?view=graph-rest-beta)-Sammlung entfernt. |
|Löschung|Beta|Die [updateDeviceProfileAssignment](/graph/api/intune-corpenrollment-enrollmentprofile-updatedeviceprofileassignment?view=graph-rest-beta)-Aktion wurde auf [enrollmentProfile](/graph/api/resources/intune-corpenrollment-enrollmentprofile?view=graph-rest-beta) entfernt. |
|Löschung|Beta|Die Aktion „setDefaultProfile“ wurde aus [enrollmentProfile](/graph/api/resources/intune-corpenrollment-enrollmentprofile?view=graph-rest-beta) entfernt. |
|Löschung|Beta|Die Aktion „shareForSchoolDataSyncService“ wurde aus [depOnboardingSetting](/graph/api/resources/intune-onboarding-deponboardingsetting?view=graph-rest-beta) entfernt. |
|Löschung|Beta|Die Aktion „unshareForSchoolDataSyncService“ wurde aus [depOnboardingSetting](/graph/api/resources/intune-onboarding-deponboardingsetting?view=graph-rest-beta) entfernt. |
|Löschung|Beta|Funktion „exportMobileConfig](/graph/api/intune_corpenrollment_enrollmentprofile_exportmobileconfig?view=graph-rest-beta) aus [enrollmentProfile](/graph/api/resources/intune-corpenrollment-enrollmentprofile?view=graph-rest-beta) entfernt |
|Ergänzungen|Beta|Die **userDomainNameSource**- und **customDomainName**-Eigenschaften wurden zu der [androidEasEmailProfileConfiguration](/graph/api/resources/intune-deviceconfig-androideasemailprofileconfiguration?view=graph-rest-beta)-Entität hinzugefügt.|
|Ergänzungen|Beta|Eigenschaften **workProfileBlockCamera** und **workProfileBlockCrossProfileContactsSearch** zur Entität [androidForWorkGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration?view=graph-rest-beta) hinzugefügt.|
|Ergänzungen|Beta|Eigenschaften **workProfileBlockCamera** und **workProfileBlockCrossProfileContactsSearch** zur Entität [androidWorkProfileGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration?view=graph-rest-beta) hinzugefügt.|
|Ergänzungen|Beta|Die **thirdPartyKeyboardsBlocked**- und **filterOpenInToOnlyManagedApps**-Eigenschaften zur [defaultManagedAppProtection](/graph/api/resources/intune-mam-defaultmanagedappprotection?view=graph-rest-beta)-Entität hinzugefügt.|
|Ergänzungen|Beta|Eigenschaft **conflictCount** zur Entität [deviceComplianceUserOverview](/graph/api/resources/intune-deviceconfig-devicecomplianceuseroverview?view=graph-rest-beta) hinzugefügt.|
|Ergänzungen|Beta|Eigenschaft **conflictCount** zur Entität [deviceConfigurationUserOverview](/graph/api/resources/intune-deviceconfig-deviceconfigurationuseroverview?view=graph-rest-beta) hinzugefügt.|
|Ergänzungen|Beta|Die **managedDeviceCleanupSettings**-Eigenschaft wurde zur [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta)-Entität hinzugefügt.|
|Löschung|Beta|Die **usernameSource**-Eigenschaft wurde aus der [iosEasEmailProfileConfiguration](/graph/api/resources/intune-deviceconfig-ioseasemailprofileconfiguration?view=graph-rest-beta)-Entität entfernt.|
|Ergänzungen|Beta|Die **thirdPartyKeyboardsBlocked**- und **filterOpenInToOnlyManagedApps**-Eigenschaften zur [iosManagedAppProtection](/graph/api/resources/intune-mam-iosmanagedappprotection?view=graph-rest-beta)-Entität hinzugefügt.|
|Ergänzungen|Beta|Die Eigenschaft **ignoreVersionDetection** wurde zur Entität [macOSLobApp](/graph/api/resources/intune-apps-macoslobapp?view=graph-rest-beta) hinzugefügt.|
|Ergänzungen|Beta|Die **pinRequiredOnLaunchInsteadOfBiometric**- und **pinRequiredInsteadOfBiometricTimeout**-Eigenschaften zur [managedAppProtection](/graph/api/resources/intune-mam-managedappprotection?view=graph-rest-beta)-Entität hinzugefügt.|
|Ergänzungen|Beta|Die **autopilotEnrolled**-, **requireUserEnrollmentApproval**-, **iccid**- und **udid**-Eigenschaften zur [ managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta)-Entität hinzugefügt.|
|Löschung|Beta|**isAutopilotEnrolled**-Eigenschaft aus [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta)-Entität entfernt|
|Ergänzungen|Beta|Eigenschaften **notApplicablePlatformCount** und **conflictCount** zur Entität [managedDeviceMobileAppConfigurationDeviceSummary](/graph/api/resources/intune-apps-manageddevicemobileappconfigurationdevicesummary?view=graph-rest-beta) hinzugefügt|
|Ergänzungen|Beta|Die **conflictCount**-Eigenschaft wurde der [managedDeviceMobileAppConfigurationUserSummary](/graph/api/resources/intune-apps-manageddevicemobileappconfigurationusersummary?view=graph-rest-beta)-Entität hinzugefügt.|
|Ergänzungen|Beta|Die Eigenschaft **scopeType** wurde zur Entität [roleAssignment](/graph/api/resources/intune-rbac-roleassignment?view=graph-rest-beta) hinzugefügt.|
|Löschung|Beta|Die **usernameSource**-Eigenschaft wurde aus der [windows10EasEmailProfileConfiguration](/graph/api/resources/intune-deviceconfig-windows10easemailprofileconfiguration?view=graph-rest-beta)-Entität entfernt.|
|Ergänzungen|Beta|Eigenschaften **localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees**, **localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers**, **localSecurityOptionsDisableServerDigitallySignCommunicationsAlways**, **localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees**, **localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares**, **localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts**, **localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares**, **localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange** und **localSecurityOptionsSmartCardRemovalBehavior** zur Entität [windows10EndpointProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windows10endpointprotectionconfiguration?view=graph-rest-beta) hinzugefügt|
|Ergänzungen|Beta|Eigenschaften **showInstallationProgress**, **blockDeviceSetupRetryByUser**, **allowDeviceResetOnInstallFailure**, **allowLogCollectionOnInstallFailure**, **customErrorMessage**, **installProgressTimeoutInMinutes** und **allowDeviceUseOnInstallFailure** zur Entität [windows10EnrollmentCompletionPageConfiguration](/graph/api/resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration?view=graph-rest-beta) hinzugefügt|
|Löschung|Beta|Eigenschaften **title**, **bodyText**, **moreInfoUrl** und **moreInfoText** aus der Entität [windows10EnrollmentCompletionPageConfiguration](/graph/api/resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration?view=graph-rest-beta) entfernt|
|Ergänzungen|Beta|Eigenschaften **defenderBlockOnAccessProtection**, **defenderScheduleScanDay** und **defenderSubmitSamplesConsentType** zur Entität [windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta) hinzugefügt|
|Ergänzungen|Beta|Eigenschaften **language** und **enrollmentSettings** zur Entität [windowsAutopilotDeploymentProfile](/graph/api/resources/intune-enrollment-windowsautopilotdeploymentprofile?view=graph-rest-beta) hinzugefügt|
|Ergänzungen|Beta|Die Eigenschaft **useDeviceContext** zur Entität [windowsMobileMSI](/graph/api/resources/intune-apps-windowsmobilemsi?view=graph-rest-beta) hinzugefügt|
|Löschung|Beta|Die **usernameSource**-Eigenschaft wurde aus der [windowsPhoneEASEmailProfileConfiguration](/graph/api/resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration?view=graph-rest-beta)-Entität entfernt.|
|Löschung|Beta|Die **localActions**-Navigationseigenschaft wurde aus der [androidCompliancePolicy](/graph/api/resources/intune-deviceconfig-androidcompliancepolicy?view=graph-rest-beta)-Entität entfernt.|
|Löschung|Beta|Die **enrollmentProfiles**- und **importedAppleDeviceIdentities**-Navigationseigenschaften wurden aus der [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta)-Entität entfernt.|
|Ergänzungen|Beta|Die **mobileAppIntentAndStates**- und **mobileAppTroubleshootingEvents**-Navigationseigenschaften wurden zur [user](/graph/api/resources/intune-shared-user?view=graph-rest-beta)-Entität hinzugefügt.|
|Ergänzungen|Beta|Eigenschaften **deviceUsageType** und **skipKeyboardSelectionPage** zum komplexen Typ [outOfBoxExperienceSettings](/graph/api/resources/intune-enrollment-outofboxexperiencesettings?view=graph-rest-beta) hinzugefügt|
|Löschung|Beta|Element **paloAltoGlobalProtect** aus dem Enumerationstyp [androidForWorkVpnConnectionType](/graph/api/resources/intune-deviceconfig-androidforworkvpnconnectiontype?view=graph-rest-beta) entfernt|
|Ergänzungen|Beta|Elemente **samAccountName** und **primarySmtpAddress** wurden zum Enumerationstyp [androidUsernameSource](/graph/api/resources/intune-deviceconfig-androidusernamesource?view=graph-rest-beta) hinzugefügt.|
|Löschung|Beta|Element **paloAltoGlobalProtect** aus dem Enumerationstyp [androidVpnConnectionType](/graph/api/resources/intune-deviceconfig-androidvpnconnectiontype?view=graph-rest-beta) entfernt.|
|Ergänzungen|Beta|Element **paloAltoGlobalProtect** zum Enumerationstyp [windows10VpnConnectionType](/graph/api/resources/intune-deviceconfig-windows10vpnconnectiontype?view=graph-rest-beta) hinzugefügt.|

## <a name="april-2018"></a>April 2018

### <a name="audit-log-api"></a>Überwachungsprotokoll-API

|Änderungstyp|Version|Beschreibung|
|:---|:---|:---|
|Ergänzungen|Beta|Entitäten [directoryAudit](/graph/api/resources/directoryaudit?view=graph-rest-beta) und [signIn](/graph/api/resources/signin?view=graph-rest-beta) hinzugefügt, zwecks Unterstützung einer neuen Überwachungsprotokoll-API. |
|Ergänzungen|Beta|Folgende Ressourcen hinzugefügt, zwecks Unterstützung der Überwachungsprotokoll-API: [appIdentity](/graph/api/resources/appidentity?view=graph-rest-beta), [auditActivityInitiator](/graph/api/resources/auditactivityinitiator?view=graph-rest-beta), [conditionalAccessPolicy](/graph/api/resources/conditionalaccesspolicy?view=graph-rest-beta), [deviceDetail](/graph/api/resources/devicedetail?view=graph-rest-beta), [mfaDetail](/graph/api/resources/mfadetail?view=graph-rest-beta), [modifiedProperty](/graph/api/resources/modifiedproperty?view=graph-rest-beta), [signinLocation](/graph/api/resources/signinlocation?view=graph-rest-beta), [signinStatus](/graph/api/resources/signinstatus?view=graph-rest-beta), [targetResource](/graph/api/resources/targetresource?view=graph-rest-beta), [targetResourceApp](/graph/api/resources/targetresourceapp?view=graph-rest-beta), [targetResourceDevice](/graph/api/resources/targetresourcedevice?view=graph-rest-beta), [targetResourceDirectory](/graph/api/resources/targetresourcedirectory?view=graph-rest-beta), [targetResourceGroup](/graph/api/resources/targetresourcegroup?view=graph-rest-beta), [targetResourceOther](/graph/api/resources/targetresourceother?view=graph-rest-beta), [targetResourcePolicy](/graph/api/resources/targetresourcepolicy?view=graph-rest-beta), [targetResourceRole](/graph/api/resources/targetresourcerole?view=graph-rest-beta), [targetResourceServicePrincipal](/graph/api/resources/targetresourceserviceprincipal?view=graph-rest-beta), [targetResourceUser](/graph/api/resources/targetresourceuser?view=graph-rest-beta), [userIdentity](/graph/api/resources/useridentity?view=graph-rest-beta) |

### <a name="directory-apis"></a>Verzeichnis-APIs

| **Änderungstyp** | **Version** | **Beschreibung**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Ergänzungen        | v1.0        | Komplexer Typ **privacyProfile** zur Entität [organization](/graph/api/resources/organization?view=graph-rest-1.0) hinzugefügt. |
| Ergänzungen        | v1.0        | Komplexe Typen **„legalAgeGroup“, „ageGroup“ und „consentProvidedForMinor“** zur Entität [user](/graph/api/resources/user?view=graph-rest-1.0) hinzugefügt. |
| Ergänzungen        | v1.0        | Unterstützung für Benutzer und Gruppen zu Abonnements von [Webhook](/graph/api/resources/webhooks?view=graph-rest-1.0)-Benachrichtigungen hinzugefügt. |
| Ergänzungen        | Beta        | Aktion zum [Auflisten der gelöschten Elemente eines Benutzers](/graph/api/directory-deleteditems-user-owned?view=graph-rest-beta) zur Ressource [directory (gelöschte Elemente)](/graph/api/resources/directory?view=graph-rest-beta) hinzugefügt. |

### <a name="education-apis"></a>Bildungs-APIs

|Änderungstyp|Version|Beschreibung|
|:---|:---|:---|
|Änderung|Beta|Die reportableIdentifier-Eigenschaft wurde zu [educationsynchronizationerror](/graph/api/resources/educationsynchronizationerror?view=graph-rest-beta) hinzugefügt.|
|Änderung|Beta|Die Antwortoptionen für die [uploadUrl](/graph/api/educationsynchronizationprofile-uploadurl?view=graph-rest-beta)-API wurden aktualisiert.|
|Änderung|Beta|Der Text für die Beschreibung des [educationSynchronizationError](/graph/api/resources/educationsynchronizationerror?view=graph-rest-beta)-Ressourcentyps wurde aktualisiert.|
|Änderung|Beta|Beschreibungstext der API zum [Abrufen von Synchronisierungsfehlern](/graph/api/educationsynchronizationerrors-get?view=graph-rest-beta) aktualisiert.|


### <a name="microsoft-intune-apis"></a>Microsoft Intune-APIs
|Änderungstyp|Version|Beschreibung|
|:---|:---|:---|
|Ergänzungen|v1.0|Neue Entitäten hinzugefügt:<br/>[managedDeviceMobileAppConfigurationDeviceStatus](/graph/api/resources/intune-apps-manageddevicemobileappconfigurationdevicestatus?view=graph-rest-1.0)<br/>|
|Ergänzungen|v1.0|Neue Enumerationstypen hinzugefügt:<br/>[managedDeviceOwnerType](/graph/api/resources/intune-devices-manageddeviceownertype?view=graph-rest-1.0)<br/>|
|Ergänzungen|v1.0|Eigenschaft **managedDeviceOwnerType** zur Entität [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0) hinzugefügt.|
|Ergänzungen|v1.0|Navigationseigenschaft **deviceStatuses** zur Entität [managedDeviceMobileAppConfiguration](/graph/api/resources/intune-apps-manageddevicemobileappconfiguration?view=graph-rest-1.0) hinzugefügt.|
|Ergänzungen|v1.0|Member **androidWorkProfile** zum Enumerationstyp [policyPlatformType](/graph/api/resources/intune-deviceconfig-policyplatformtype?view=graph-rest-1.0) hinzugefügt.|
|Ergänzungen|Beta|Neue Entitäten hinzugefügt:<br/>[androidWorkProfileCertificateProfileBase](/graph/api/resources/intune-deviceconfig-androidworkprofilecertificateprofilebase?view=graph-rest-beta)<br/>[androidWorkProfileCustomConfiguration](/graph/api/resources/intune-deviceconfig-androidworkprofilecustomconfiguration?view=graph-rest-beta)<br/>[androidWorkProfileEasEmailProfileBase](/graph/api/resources/intune-deviceconfig-androidworkprofileeasemailprofilebase?view=graph-rest-beta)<br/>[androidWorkProfileEnterpriseWiFiConfiguration](/graph/api/resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration?view=graph-rest-beta)<br/>[androidWorkProfileGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration?view=graph-rest-beta)<br/>[androidWorkProfileGmailEasConfiguration](/graph/api/resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration?view=graph-rest-beta)<br/>[androidWorkProfileNineWorkEasConfiguration](/graph/api/resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration?view=graph-rest-beta)<br/>[androidWorkProfilePkcsCertificateProfile](/graph/api/resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile?view=graph-rest-beta)<br/>[androidWorkProfileScepCertificateProfile](/graph/api/resources/intune-deviceconfig-androidworkprofilescepcertificateprofile?view=graph-rest-beta)<br/>[androidWorkProfileTrustedRootCertificate](/graph/api/resources/intune-deviceconfig-androidworkprofiletrustedrootcertificate?view=graph-rest-beta)<br/>[androidWorkProfileVpnConfiguration](/graph/api/resources/intune-deviceconfig-androidworkprofilevpnconfiguration?view=graph-rest-beta)<br/>[androidWorkProfileWiFiConfiguration](/graph/api/resources/intune-deviceconfig-androidworkprofilewificonfiguration?view=graph-rest-beta)<br/>[restrictedAppsViolation](/graph/api/resources/intune-deviceconfig-restrictedappsviolation?view=graph-rest-beta)<br/>[windowsAutopilotDeploymentProfileAssignment](/graph/api/resources/intune-enrollment-windowsautopilotdeploymentprofileassignment?view=graph-rest-beta)<br/>|
|Ergänzungen|Beta|Neue komplexe Typen hinzugefügt:<br/>[managedDeviceModelsAndManufacturers](/graph/api/resources/intune-devices-manageddevicemodelsandmanufacturers?view=graph-rest-beta)<br/>[managedDeviceReportedApp](/graph/api/resources/intune-devices-manageddevicereportedapp?view=graph-rest-beta)<br/>[windowsEnrollmentStatusScreenSettings](/graph/api/resources/intune-enrollment-windowsenrollmentstatusscreensettings?view=graph-rest-beta)<br/>|
|Ergänzungen|Beta|Neue Enumerationstypen hinzugefügt:<br/>[androidWorkProfileCrossProfileDataSharingType](/graph/api/resources/intune-deviceconfig-androidworkprofilecrossprofiledatasharingtype?view=graph-rest-beta)<br/>[androidWorkProfileDefaultAppPermissionPolicyType](/graph/api/resources/intune-deviceconfig-androidworkprofiledefaultapppermissionpolicytype?view=graph-rest-beta)<br/>[androidWorkProfileRequiredPasswordType](/graph/api/resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype?view=graph-rest-beta)<br/>[androidWorkProfileVpnConnectionType](/graph/api/resources/intune-deviceconfig-androidworkprofilevpnconnectiontype?view=graph-rest-beta)<br/>[bitLockerRecoveryInformationType](/graph/api/resources/intune-deviceconfig-bitlockerrecoveryinformationtype?view=graph-rest-beta)<br/>[localSecurityOptionsInformationShownOnLockScreenType](/graph/api/resources/intune-deviceconfig-localsecurityoptionsinformationshownonlockscreentype?view=graph-rest-beta)<br/>[managedAppRemediationAction](/graph/api/resources/intune-mam-managedappremediationaction?view=graph-rest-beta)<br/>[managedDeviceOwnerType](/graph/api/resources/intune-devices-manageddeviceownertype?view=graph-rest-beta)<br/>[restrictedAppsState](/graph/api/resources/intune-deviceconfig-restrictedappsstate?view=graph-rest-beta)<br/>[windows10VpnProfileTarget](/graph/api/resources/intune-deviceconfig-windows10vpnprofiletarget?view=graph-rest-beta)<br/>|
|Ergänzungen|Beta|Aktion [playLostModeSound](/graph/api/intune-devices-manageddevice-playlostmodesound?view=graph-rest-beta) zu [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) hinzugefügt. |
|Löschung|Beta|Folgende Enumerationstypen wurden entfernt:<br/>**bitLockerRecoveryinformationType**<br/>**windowsUpdateRestartMode**<br/>|
|Ergänzungen|Beta|Eigenschaften **workProfileBlockScreenCapture** und **workProfileBlockCrossProfileCallerId** zur Entität [androidForWorkGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration?view=graph-rest-beta) hinzugefügt.|
|Ergänzungen|Beta|Eigenschaften **minimumWipePatchVersion**, **allowedAndroidDeviceManufacturers** und **appActionIfAndroidDeviceManufacturerNotAllowed** zur Entität [androidManagedAppProtection](/graph/api/resources/intune-mam-androidmanagedappprotection?view=graph-rest-beta) hinzugefügt.|
|Ergänzungen|Beta|Eigenschaften **minimumWipeSdkVersion**, **minimumWipePatchVersion**, **allowedIosDeviceModels**, **appActionIfIosDeviceModelNotAllowed**, **allowedAndroidDeviceManufacturers** und **appActionIfAndroidDeviceManufacturerNotAllowed** zur Entität [defaultManagedAppProtection](/graph/api/resources/intune-mam-defaultmanagedappprotection?view=graph-rest-beta) hinzugefügt.|
|Ergänzungen|Beta|Eigenschaften **notApplicablePlatformCount** und **conflictCount** zur Entität [deviceComplianceDeviceOverview](/graph/api/resources/intune-deviceconfig-devicecompliancedeviceoverview?view=graph-rest-beta) hinzugefügt.|
|Ergänzungen|Beta|Eigenschaften **notApplicablePlatformCount** und **conflictCount** zur Eigenschaft [deviceConfigurationDeviceOverview](/graph/api/resources/intune-deviceconfig-deviceconfigurationdeviceoverview?view=graph-rest-beta) hinzugefügt.|
|Ergänzungen|Beta|Eigenschaft **accountMoveCompletionDateTime** zur Entität [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta) hinzugefügt.|
|Ergänzungen|Beta|Eigenschaften **minimumWipeSdkVersion**, **allowedIosDeviceModels** und **appActionIfIosDeviceModelNotAllowed** zur Entität [ iosManagedAppProtection](/graph/api/resources/intune-mam-iosmanagedappprotection?view=graph-rest-beta) hinzugefügt.|
|Ergänzungen|Beta|Eigenschaften **minimumWipeOsVersion**, **minimumWipeAppVersion**, **appActionIfDeviceComplianceRequired** und **appActionIfMaximumPinRetriesExceeded** zur Entität [managedAppProtection](/graph/api/resources/intune-mam-managedappprotection?view=graph-rest-beta) hinzugefügt.|
|Ergänzungen|Beta|Eigenschaften **managedDeviceOwnerType**, **preferMdmOverGroupPolicyAppliedDateTime**, **isAutopilotEnrolled** und **requestUserEnrollmentApproval** zur Entität [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) hinzugefügt.|
|Ergänzungen|Beta|Eigenschaft **managedDeviceModelsAndManufacturers** zur Entität [managedDeviceOverview](/graph/api/resources/intune-devices-manageddeviceoverview?view=graph-rest-beta) hinzugefügt.|
|Ergänzungen|Beta|Eigenschaften **localSecurityOptionsMachineInactivityLimitInMinutes**, **localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool**, **localSecurityOptionsInformationShownOnLockScreen**, **defenderSecurityCenterDisableAccountUI**, **defenderSecurityCenterDisableHardwareUI**, **defenderSecurityCenterDisableRansomwareUI**, **defenderSecurityCenterDisableSecureBootUI** und **defenderSecurityCenterDisableTroubleshootingUI** zur Entität [windows10EndpointProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windows10endpointprotectionconfiguration?view=graph-rest-beta) hinzugefügt.|
|Ergänzungen|Beta|Eigenschaften **printerNames**, **printerDefaultName**, **printerBlockAddition** und **searchBlockWebResults** zur Entität [windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta) hinzugefügt.|
|Ergänzungen|Beta|Eigenschaften **profileTarget**, **enableAlwaysOn** und **enableDeviceTunnel** zur Entität [windows10VpnConfiguration](/graph/api/resources/intune-deviceconfig-windows10vpnconfiguration?view=graph-rest-beta) hinzugefügt.|
|Ergänzungen|Beta|Eigenschaft **enrollmentStatusScreenSettings** zur Entität [windowsAutopilotDeploymentProfile](/graph/api/resources/intune-enrollment-windowsautopilotdeploymentprofile?view=graph-rest-beta) hinzugefügt.|
|Ergänzungen|Beta|Navigationseigenschaft **deviceConfigurationRestrictedAppsViolations** zur Entität [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta) hinzugefügt.|
|Ergänzungen|Beta|Navigationseigenschaft **assignments** zur Entität [windowsAutopilotDeploymentProfile](/graph/api/resources/intune-enrollment-windowsautopilotdeploymentprofile?view=graph-rest-beta) hinzugefügt.|
|Ergänzungen|Beta|Navigationseigenschaft **networkAccessConfigurations** zur Entität [windowsDomainJoinConfiguration](/graph/api/resources/intune-deviceconfig-windowsdomainjoinconfiguration?view=graph-rest-beta) hinzugefügt.|
|Löschung|Beta|Eigenschaft **permissions** aus komplexem Typ [auditActor](/graph/api/resources/intune-auditing-auditactor?view=graph-rest-beta) entfernt.|
|Änderung|Beta|Typ der folgenden Eigenschaften des komplexen Typs [bitLockerRecoveryOptions](/graph/api/resources/intune-deviceconfig-bitlockerrecoveryoptions?view=graph-rest-beta) geändert:<br/>**recoveryInformationToStore** von [bitLockerRecoveryinformationType](/graph/api/resources/intune-deviceconfig-bitlockerrecoveryinformationtype?view=graph-rest-beta) in [bitLockerRecoveryInformationType](/graph/api/resources/intune-deviceconfig-bitlockerrecoveryinformationtype?view=graph-rest-beta)<br/>|
|Ergänzungen|Beta|Eigenschaft **deviceInactivityBeforeRetirementInDay** zum komplexen Typ [deviceManagementSettings](/graph/api/resources/intune-deviceconfig-devicemanagementsettings?view=graph-rest-beta) hinzugefügt.|
|Ergänzungen|Beta|Eigenschaft **landingPageCustomizedImage** zum komplexen Typ [intuneBrand](/graph/api/resources/intune-onboarding-intunebrand?view=graph-rest-beta) hinzugefügt.|
|Löschung|Beta|Eigenschaft **ipAddressOrFqdn** aus komplexem Typ [vpnServer](/graph/api/resources/intune-deviceconfig-vpnserver?view=graph-rest-beta) entfernt:|
|Löschung|Beta|Eigenschaft **restartMode** aus komplexem Typ [windowsUpdateScheduledInstall](/graph/api/resources/intune-deviceconfig-windowsupdatescheduledinstall?view=graph-rest-beta) entfernt.|
|Ergänzungen|Beta|Member **paloAltoGlobalProtect** zum Enumerationstyp [androidForWorkVpnConnectionType](/graph/api/resources/intune-deviceconfig-androidforworkvpnconnectiontype?view=graph-rest-beta) hinzugefügt.|
|Ergänzungen|Beta|Member **paloAltoGlobalProtect** zum Enumerationstyp [androidVpnConnectionType](/graph/api/resources/intune-deviceconfig-androidvpnconnectiontype?view=graph-rest-beta) hinzugefügt.|
|Ergänzungen|Beta|Member **paloAltoGlobalProtect** zum Enumerationstyp [appleVpnConnectionType](/graph/api/resources/intune-deviceconfig-applevpnconnectiontype?view=graph-rest-beta) hinzugefügt.|
|Ergänzungen|Beta|Member **androidWorkProfile** zum Enumerationstyp [policyPlatformType](/graph/api/resources/intune-deviceconfig-policyplatformtype?view=graph-rest-beta) hinzugefügt.|

### <a name="microsoft-teams"></a>Microsoft Teams

|Änderungstyp|Version|Beschreibung|
|:---|:---|:---|
|Ergänzungen|Beta|Neue Entität [teamMemberSettings](/graph/api/resources/teammembersettings?view=graph-rest-beta) hinzugefügt.|
|Ergänzungen|Beta|Neue Entität [teamGuestSettings](/graph/api/resources/teamguestsettings?view=graph-rest-beta) hinzugefügt.|
|Ergänzungen|Beta|Neue Entität [teamMessagingSettings](/graph/api/resources/teammessagingsettings?view=graph-rest-beta) hinzugefügt.|
|Ergänzungen|Beta|Neue Entität [teamFunSettings](/graph/api/resources/teamfunsettings?view=graph-rest-beta) hinzugefügt.|
|Ergänzungen|Beta|Neue Operation [Kanal löschen](/graph/api/channel-delete?view=graph-rest-beta) hinzugefügt.|
|Ergänzungen|Beta|Neue Operation [Kanal patchen](/graph/api/channel-patch?view=graph-rest-beta) hinzugefügt.|
|Ergänzungen|Beta|Neue webUrl-Eigenschaft zur [team](/graph/api/resources/team?view=graph-rest-beta)-Ressource hinzugefügt.|
|Ändern|Beta|Pfad zu Entität [channel](/graph/api/resources/channel?view=graph-rest-beta) aktualisiert.|

### <a name="outlook-calendar"></a>Outlook-Kalender

| **Änderungstyp** | **Version**   | **Beschreibung**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Ergänzungen        | v1.0          | **locations**-Eigenschaft zur  [event](/graph/api/resources/event?view=graph-rest-1.0)-Entität zur Unterstützung der Organisation von Ereignissen hinzugefügt, an denen Teilnehmer von mehr als einem Ort teilnehmen können. |
| Ergänzungen        | v1.0          | **locationType**-Eigenschaft zum komplexen Typ [location](/graph/api/resources/location?view=graph-rest-1.0) hinzugefügt. |
| Ergänzungen        | v1.0          | Eigenschaften **uniqueId** und **uniqueIdType** zum komplexen Typ [location](/graph/api/resources/location?view=graph-rest-1.0) hinzugefügt. Diese Eigenschaften dienen zu diesem Zeitpunkt nur der internen Verwendung. |


### <a name="outlook-contacts"></a>Outlook-Kontakte

| **Änderungstyp** | **Version** | **Beschreibung**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Ergänzungen        | v1.0          | Added the **flag** property to the [contact](/graph/api/resources/contact?view=graph-rest-1.0) entity. Added the shared [followupFlag](/graph/api/resources/followupflag?view=graph-rest-1.0) complex type.|


### <a name="outlook-mail"></a>Outlook-Mail

| **Änderungstyp** | **Version** | **Beschreibung**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Ergänzungen        | v1.0          | Added the **flag** property to the [message](/graph/api/resources/message?view=graph-rest-1.0) entity. Added the shared [followupFlag](/graph/api/resources/followupflag?view=graph-rest-1.0) complex type.|
| Ergänzungen        | v1.0        | **internetMessageHeaders**-Eigenschaft zur [message](/graph/api/resources/message?view=graph-rest-1.0)-Entität hinzugefügt. |
| Ergänzungen        | v1.0        | Komplexer Typ [internetMessageHeader](/graph/api/resources/internetmessageheader?view=graph-rest-1.0) hinzugefügt. |
| Ergänzungen        | v1.0        | Added the **messageRules** navigation property to the [mailFolder](/graph/api/resources/mailfolder?view=graph-rest-1.0) entity. **messageRules** is a collection of [messageRule](/graph/api/resources/messagerule?view=graph-rest-1.0) instances. |
| Ergänzungen        | v1.0        | [messageRule](/graph/api/resources/messagerule?view=graph-rest-1.0)-Entität sowie die komplexen Typen [messageRuleActions](/graph/api/resources/messageruleactions?view=graph-rest-1.0), [messageRulePredicates](/graph/api/resources/messagerulepredicates?view=graph-rest-1.0) und [sizeRange](/graph/api/resources/sizerange?view=graph-rest-1.0) hinzugefügt. |
| Ergänzungen        | v1.0        | Folgende CRUD-Vorgänge für Nachrichtenregeln hinzugefügt: [create](/graph/api/mailfolder-post-messagerules?view=graph-rest-1.0), [list](/graph/api/mailfolder-list-messagerules?view=graph-rest-1.0), [get](/graph/api/messagerule-get?view=graph-rest-1.0), [update](/graph/api/messagerule-update?view=graph-rest-1.0) und [delete](/graph/api/messagerule-delete?view=graph-rest-1.0). |
| Ergänzungen | Beta | [mailSearchFolder](/graph/api/resources/mailsearchfolder?view=graph-rest-beta) wurde hinzugefügt. |
| Ergänzungen | Beta | Die folgenden APIs für E-Mail-Suchordner wurden hinzugefügt: [Erstellen](/graph/api/mailsearchfolder-post?view=graph-rest-beta), [Aktualisieren](/graph/api/mailsearchfolder-update?view=graph-rest-beta). |
| Änderung | Beta | Zusätzliche Unterstützung für E-Mail-Suchordner hinzugefügt zu [mailFolder löschen](/graph/api/mailfolder-delete?view=graph-rest-beta), [mailFolder abrufen](/graph/api/mailfolder-get?view=graph-rest-beta) und [Untergeordnete Ordner auflisten](/graph/api/mailfolder-list-childfolders?view=graph-rest-beta). |


### <a name="outlook-user-choices"></a>Auswahlmöglichkeiten für Outlook-Benutzer

| **Änderungstyp** | **Version** | **Beschreibung**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Ergänzungen        | v1.0        | Added the new **masterCategories** navigation property to the [outlookUser](/graph/api/resources/outlookuser?view=graph-rest-1.0) entity. **masterCategories** is a collection of [outlookCategory](/graph/api/resources/outlookcategory?view=graph-rest-1.0) objects. |
| Ergänzungen        | v1.0        | [outlookCategory](/graph/api/resources/outlookcategory?view=graph-rest-1.0)-Entität hinzugefügt. |
| Ergänzungen        | v1.0        | Die folgenden CRUD-Vorgänge für [outlookCategory](/graph/api/resources/outlookcategory?view=graph-rest-1.0) hinzugefügt: [create](/graph/api/outlookuser-post-mastercategories?view=graph-rest-1.0), [get](/graph/api/outlookcategory-get?view=graph-rest-1.0), [update](/graph/api/outlookcategory-update?view=graph-rest-1.0) und [delete](/graph/api/outlookcategory-delete?view=graph-rest-1.0). |
| Ergänzungen        | v1.0        | Neue Funktion [supportedLanguages](/graph/api/outlookuser-supportedlanguages?view=graph-rest-1.0) zur [outlookUser](/graph/api/resources/outlookuser?view=graph-rest-1.0)-Entität hinzugefügt. |
| Ergänzungen        | v1.0        | Neue [supportedTimeZones](/graph/api/outlookuser-supportedtimezones?view=graph-rest-1.0)-Funktion zur [outlookUser](/graph/api/resources/outlookuser?view=graph-rest-1.0)-Entität hinzugefügt. |
|Ergänzungen | v1.0 | Added the new **workingHours** property to [mailboxSettings](/graph/api/resources/mailboxsettings?view=graph-rest-1.0). See [workingHours resource type](/graph/api/resources/workinghours?view=graph-rest-1.0) for information on the supported use cases.|
|Ergänzungen | v1.0 | Folgende neue komplexe Typen hinzugefügt: <br> [workingHours](/graph/api/resources/workinghours?view=graph-rest-1.0) <br> [timeZoneBase](/graph/api/resources/timezonebase?view=graph-rest-1.0) <br> [customTimeZone](/graph/api/resources/customtimezone?view=graph-rest-1.0) <br> [standardTimeZoneOffset](/graph/api/resources/standardtimezoneoffset?view=graph-rest-1.0) <br> [daylightTimeZoneOffset](/graph/api/resources/daylighttimezoneoffset?view=graph-rest-1.0)|


### <a name="project-rome-apis"></a>Project Rome-APIs

| **Änderungstyp** | **Version** | **Beschreibung**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Ergänzungen | v1.0 | API zum [Abrufen der letzten Aktivitäten](/graph/api/projectrome-get-recent-activities?view=graph-rest-1.0) hinzugefügt. |
| Ergänzungen | v1.0 | API zum [Abrufen von Aktivitäten](/graph/api/projectrome-get-activities?view=graph-rest-1.0) hinzugefügt. |
| Ergänzungen | v1.0 | [upsert-Aktivität](/graph/api/projectrome-put-activity?view=graph-rest-1.0) hinzugefügt. |
| Ergänzungen | v1.0 | [Upsert HistoryItem](/graph/api/projectrome-put-historyitem?view=graph-rest-1.0) hinzugefügt. |
| Ergänzungen | v1.0 | [delete-Aktivität](/graph/api/projectrome-delete-activity?view=graph-rest-1.0) hinzugefügt. |
| Ergänzungen | v1.0 | [Upsert HistoryItem](/graph/api/projectrome-delete-historyitem?view=graph-rest-1.0) hinzugefügt. |
| Ergänzungen | v1.0 | [activity](/graph/api/resources/projectrome-activity?view=graph-rest-1.0) hinzugefügt. |
| Ergänzungen | v.10 | [historyItem](/graph/api/resources/projectrome-historyitem?view=graph-rest-1.0) hinzugefügt. |
| Ergänzungen | v1.0 | [visualInfo](/graph/api/resources/projectrome-visualinfo?view=graph-rest-1.0) hinzugefügt. |
| Ergänzungen | v1.0 | [imageInfo](/graph/api/resources/projectrome-imageinfo?view=graph-rest-1.0) hinzugefügt. |
| Ergänzungen | v.10 | [Project Rome-Übersicht](/graph/api/resources/project-rome-overview?view=graph-rest-1.0) hinzugefügt. |
| Änderung | Beta | „deep insert“-Dokumentation zu [upsert-Aktivität](/graph/api/projectrome-put-activity?view=graph-rest-beta) hinzugefügt. |

### <a name="reports-apis"></a>Bericht-APIs
|Änderungstyp|Version|Beschreibung|
|:---|:---|:---|
|Ergänzungen|Beta| Unterstützung für delegierten Zugriff hinzugefügt. |
|Ergänzungen|v1.0| Unterstützung für delegierten Zugriff hinzugefügt. |

### <a name="security-apis"></a>Sicherheits-APIs

| **Änderungstyp** | **Version** | **Beschreibung**              |
| :-------------- | :---------- | :--------------------------------------- |
| Ergänzungen        | Beta       | [Sicherheits-API](/graph/api/resources/security-api-overview?view=graph-rest-beta) wurde hinzugefügt, darunter folgende Ressourcen und Vorgänge:<br/>[Warnung](/graph/api/resources/alert?view=graph-rest-beta) (und verknüpfte Entitäten)<br/>[Warnung erhalten](/graph/api/alert-get?view=graph-rest-beta)<br/>[Warnungen auflisten](/graph/api/alert-list?view=graph-rest-beta)<br/>[Warnung aktualisieren](/graph/api/alert-update?view=graph-rest-beta)<br/><br/>Die folgenden Dokumente zur Unterstützung wurden hinzugefügt:<br/>[Fehler](/graph/api/resources/security-error-codes?view=graph-rest-beta)<br/>[Integrieren mit einem SIEM](security-siemintegration.md)


## <a name="march-2018"></a>März 2018

### <a name="activityfeedservice-apis"></a>ActivityFeedService-APIs

| **Änderungstyp** | **Version** | **Beschreibung**              |
| :-------------- | :---------- | :--------------------------------------- |
| Ergänzungen        | Beta       | [Aktuelle Aktivitäts-API abrufen](/graph/api/projectrome-get-recent-activities?view=graph-rest-beta) hinzugefügt |
| Ergänzungen        | Beta       | [Aktivitäts-API abrufen](/graph/api/projectrome-get-activities?view=graph-rest-beta) hinzugefügt |
| Änderung | Beta | UserActivity.ReadWrite.CreatedByApp-Berechtigung zu [Upsert-Aktivität](/graph/api/projectrome-put-activity?view=graph-rest-beta) hinzugefügt |
| Änderung | Beta | UserActivity.ReadWrite.CreatedByApp-Berechtigung zu [Upsert HistoryItem](/graph/api/projectrome-put-historyitem?view=graph-rest-beta) hinzugefügt |
| Änderung | Beta | UserActivity.ReadWrite.CreatedByApp-Berechtigung zu [Löschaktivität](/graph/api/projectrome-delete-activity?view=graph-rest-beta) hinzugefügt |
| Änderung | Beta | UserActivity.ReadWrite.CreatedByApp-Berechtigung zu [Upsert HistoryItem](/graph/api/projectrome-delete-historyitem?view=graph-rest-beta) hinzugefügt |
| Änderung | Beta | **status**-Eigenschaft zu [Aktivität](/graph/api/resources/projectrome-activity?view=graph-rest-beta) hinzugefügt |
| Änderung | Beta | **activity**-Navigationseigenschaft zu [historyItem](/graph/api/resources/projectrome-historyitem?view=graph-rest-beta) hinzugefügt |
| Ändern | Beta | Neue APIs zu [Project Rome-Übersicht](/graph/api/resources/project-rome-overview?view=graph-rest-beta) hinzugefügt |

### <a name="azure-ad-apis"></a>Azure AD-APIs

|Änderungstyp|Version|Beschreibung|
|:---|:---|:---|
|Änderung|Beta|Die **applicationID**- und **creatorUserID**-Eigenschaften wurden zur [subscription](/graph/api/resources/subscription?view=graph-rest-beta)-Ressource hinzugefügt. |
|Änderung|Beta|Der [list](/graph/api/subscription-list?view=graph-rest-beta)-Vorgang wurde zur [subscription](/graph/api/resources/subscription?view=graph-rest-beta)-Entität hinzugefügt. |

### <a name="data-policy-operations"></a>Datenrichtlinienoperationen

| **Änderungstyp** | **Version** | **Beschreibung**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Ergänzungen        | Beta        | Added new entity [dataPolicyOperation](/graph/api/resources/datapolicyoperation?view=graph-rest-beta). This represents a submitted data policy operation for tracking purposes.
| Ergänzungen        | Beta        | Added the [exportPersonalData](/graph/api/user-exportpersonaldata?view=graph-rest-beta) action on [users](/graph/api/resources/users?view=graph-rest-beta). This action submits a data policy operation request to export personal data stored by Microsoft for a user. |

### <a name="directory-apis"></a>Verzeichnis-APIs

| **Änderungstyp** | **Version** | **Beschreibung**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Ergänzungen        | Beta        | Added the **onPremisesExtensionAttributes** complex type to the [user](/graph/api/resources/user?view=graph-rest-beta) entity. This contains the on-premises AD extension attributes 1-15. |
| Ergänzungen        | Beta        | Komplexer Typ **privacyProfile** zur [organization](/graph/api/resources/organization?view=graph-rest-beta)-Entität hinzugefügt. |
| Ergänzungen        | v1.0        | Unterstützung für die [Wiederherstellung sowie die dauerhafte Löschung von Benutzern und Gruppen](/graph/api/resources/directory?view=graph-rest-1.0) hinzugefügt. |

### <a name="excel-apis"></a>Excel-APIs

| **Änderungstyp** | **Version** | **Beschreibung**                          |
| :-------------- | :---------- | :--------------------------------------- |
|Ändern|v1.0|Added the **legacyId** property to the [Excel Table](/graph/api/resources/table?view=graph-rest-1.0) entity. This will contain the numeric value identifier (string data type) that will remain constact for a given Excel table. This is provided as an additional metadata if the application relied on the legacy identifier used in older Excel client applications. Note: The `id` and `legacyId` property should be treated as an opaque string value and should not be parsed to any other type within your application. |

### <a name="group-lifecycle-policy"></a>Gruppenlebenszyklusrichtlinie

| **Änderungstyp** | **Version** | **Beschreibung**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Ergänzungen        | v1.0        | [groupLifecyclePolicy](/graph/api/resources/grouplifecyclepolicy?view=graph-rest-1.0) hinzugefügt. |
| Ergänzungen        | v1.0        | Folgende APIs wurden für Gruppenlebenszyklusrichtlinie hinzugefügt: [Create](/graph/api/grouplifecyclepolicy-post-grouplifecyclepolicies?view=graph-rest-1.0), [List](/graph/api/grouplifecyclepolicy-list?view=graph-rest-1.0), [Get](/graph/api/grouplifecyclepolicy-get?view=graph-rest-1.0), [Update](/graph/api/grouplifecyclepolicy-update?view=graph-rest-1.0), [Delete](/graph/api/grouplifecyclepolicy-delete?view=graph-rest-1.0), [Add group](/graph/api/grouplifecyclepolicy-addgroup?view=graph-rest-1.0), [Remove group](/graph/api/grouplifecyclepolicy-removegroup?view=graph-rest-1.0). |
| Ergänzungen        | v1.0        | [List groupLifecylePolicies](/graph/api/group-list-grouplifecyclepolicies?view=graph-rest-1.0)-Funktion zu [group](/graph/api/resources/group?view=graph-rest-1.0) hinzugefügt. |
| Ändern | v1.0 | RenewedDateTime-Eigenschaft und [renew](/graph/api/group-renew?view=graph-rest-1.0) zu [group](/graph/api/resources/group?view=graph-rest-1.0) hinzugefügt. |

### <a name="microsoft-intune-apis"></a>Microsoft Intune-APIs

|Änderungstyp|Version|Beschreibung|
|:---|:---|:---|
|Ergänzungen|v1.0|Hinzugefügte neue Entitäten:<br/>[iosMobileAppConfiguration](/graph/api/resources/intune-apps-iosmobileappconfiguration?view=graph-rest-1.0)<br/>[vppToken](/graph/api/resources/intune-onboarding-vpptoken?view=graph-rest-1.0)<br/>|
|Ergänzungen|v1.0|Neue komplexe Typen hinzugefügt:<br/>[appConfigurationSettingItem](/graph/api/resources/intune-apps-appconfigurationsettingitem?view=graph-rest-1.0)<br/>|
|Ergänzungen|v1.0|[syncLicenses](/graph/api/intune-onboarding-vpptoken-synclicenses?view=graph-rest-1.0)-Aktion zu [vppToken](/graph/api/resources/intune-onboarding-vpptoken?view=graph-rest-1.0) hinzugefügt. |
|Ergänzungen|v1.0|**vppTokens**-Navigationseigenschaft zur [deviceAppManagement](/graph/api/resources/intune-shared-deviceappmanagement?view=graph-rest-1.0)-Entität hinzugefügt.|
|Ergänzungen|Beta|Die **managementCertificateExpirationDate**-Eigenschaft wurde zur [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta)-Entität hinzugefügt.|
|Ergänzungen|Beta|Die **enhancedJailBreak**-Eigenschaft wurde zum komplexen [deviceManagementSettings](/graph/api/resources/intune-deviceconfig-devicemanagementsettings?view=graph-rest-beta)-Typ hinzugefügt.|
|Ergänzungen|Beta|Hinzugefügte neue Entitäten:<br/>[androidDeviceOwnerEnrollmentProfile](/graph/api/resources/intune-androidforwork-androiddeviceownerenrollmentprofile?view=graph-rest-beta)<br/>[androidDeviceOwnerGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration?view=graph-rest-beta)<br/>[androidManagedStoreAccountEnterpriseSettings](/graph/api/resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings?view=graph-rest-beta)<br/>[androidManagedStoreAppConfigurationSchema](/graph/api/resources/intune-androidforwork-androidmanagedstoreappconfigurationschema?view=graph-rest-beta)<br/>[dataSharingConsent](/graph/api/resources/intune-devices-datasharingconsent?view=graph-rest-beta)<br/>[deviceConfigurationUserStateSummary](/graph/api/resources/intune-deviceconfig-deviceconfigurationuserstatesummary?view=graph-rest-beta)<br/>[macOSEndpointProtectionConfiguration](/graph/api/resources/intune-deviceconfig-macosendpointprotectionconfiguration?view=graph-rest-beta)<br/>[macOSImportedPFXCertificateProfile](/graph/api/resources/intune-deviceconfig-macosimportedpfxcertificateprofile?view=graph-rest-beta)<br/>[macOSLobApp](/graph/api/resources/intune-apps-macoslobapp?view=graph-rest-beta)<br/>[managedEBookCategory](/graph/api/resources/intune-books-managedebookcategory?view=graph-rest-beta)<br/>[microsoftStoreForBusinessContainedApp](/graph/api/resources/intune-apps-microsoftstoreforbusinesscontainedapp?view=graph-rest-beta)<br/>[mobileContainedApp](/graph/api/resources/intune-apps-mobilecontainedapp?view=graph-rest-beta)<br/>[windowsUniversalAppXContainedApp](/graph/api/resources/intune-apps-windowsuniversalappxcontainedapp?view=graph-rest-beta)<br/>|
|Ergänzungen|Beta|Neue komplexe Typen hinzugefügt:<br/>[androidManagedStoreAppConfigurationSchemaItem](/graph/api/resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitem?view=graph-rest-beta)<br/>[deviceAndAppManagementData](/graph/api/resources/intune-onboarding-deviceandappmanagementdata?view=graph-rest-beta)<br/>[loggedOnUser](/graph/api/resources/intune-devices-loggedonuser?view=graph-rest-beta)<br/>[macOSFirewallApplication](/graph/api/resources/intune-deviceconfig-macosfirewallapplication?view=graph-rest-beta)<br/>[macOSLobChildApp](/graph/api/resources/intune-apps-macoslobchildapp?view=graph-rest-beta)<br/>[macOSMinimumOperatingSystem](/graph/api/resources/intune-apps-macosminimumoperatingsystem?view=graph-rest-beta)<br/>[windowsAppXAppAssignmentSettings](/graph/api/resources/intune-apps-windowsappxappassignmentsettings?view=graph-rest-beta)<br/>[windowsUniversalAppXAppAssignmentSettings](/graph/api/resources/intune-apps-windowsuniversalappxappassignmentsettings?view=graph-rest-beta)<br/>|
|Ergänzungen|Beta|[requestSignupUrl](/graph/api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-requestsignupurl?view=graph-rest-beta)-Aktion wurde für [androidManagedStoreAccountEnterpriseSettings](/graph/api/resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings?view=graph-rest-beta) hinzugefügt |
|Ergänzungen|Beta|[completeSignup](/graph/api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-completesignup?view=graph-rest-beta)-Aktion wurde für [androidManagedStoreAccountEnterpriseSettings](/graph/api/resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings?view=graph-rest-beta) hinzugefügt |
|Ergänzungen|Beta|[syncApps](/graph/api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-syncapps?view=graph-rest-beta)-Aktion wurde für [androidManagedStoreAccountEnterpriseSettings](/graph/api/resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings?view=graph-rest-beta) hinzugefügt |
|Ergänzungen|Beta|[unbind](/graph/api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-unbind?view=graph-rest-beta)-Aktion wurde für [androidManagedStoreAccountEnterpriseSettings](/graph/api/resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings?view=graph-rest-beta) hinzugefügt |
|Ergänzungen|Beta|[revokeToken](/graph/api/intune-androidforwork-androiddeviceownerenrollmentprofile-revoketoken?view=graph-rest-beta)-Aktion für [androidDeviceOwnerEnrollmentProfile](/graph/api/resources/intune-androidforwork-androiddeviceownerenrollmentprofile?view=graph-rest-beta) hinzugefügt |
|Ergänzungen|Beta|[createToken](/graph/api/intune-androidforwork-androiddeviceownerenrollmentprofile-createtoken?view=graph-rest-beta)-Aktion für [androidDeviceOwnerEnrollmentProfile](/graph/api/resources/intune-androidforwork-androiddeviceownerenrollmentprofile?view=graph-rest-beta) hinzugefügt |
|Ergänzungen|Beta|[assign](/graph/api/intune-apps-manageddevicemobileappconfiguration-assign?view=graph-rest-beta)-Aktion zu [managedDeviceMobileAppConfiguration](/graph/api/resources/intune-apps-manageddevicemobileappconfiguration?view=graph-rest-beta) hinzugefügt. |
|Ergänzungen|Beta|[consentToDataSharing](/graph/api/intune-devices-datasharingconsent-consenttodatasharing?view=graph-rest-beta)-Aktion zu [dataSharingConsent](/graph/api/resources/intune-devices-datasharingconsent?view=graph-rest-beta) hinzugefügt |
|Ergänzungen|Beta|[getLoggedOnManagedDevices](/graph/api/intune-devices-user-getloggedonmanageddevices?view=graph-rest-beta)-Funktion für [Benutzer](/graph/api/resources/intune-shared-user?view=graph-rest-beta) hinzugefügt |
|Ergänzungen|Beta|[exportDeviceAndAppManagementData](/graph/api/intune-onboarding-user-exportdeviceandappmanagementdata?view=graph-rest-beta)-Funktion für [user](/graph/api/resources/intune-devices-user?view=graph-rest-beta) hinzugefügt |
|Ergänzungen|Beta|[exportDeviceAndAppManagementData](/graph/api/intune-onboarding-user-exportdeviceandappmanagementdata?view=graph-rest-beta)-Funktion für [user](/graph/api/resources/intune-devices-user?view=graph-rest-beta) hinzugefügt |
|Löschung|Beta|Folgende Entitäten entfernt:<br/>**appleVolumePurchaseProgramToken**<br/>**mdmAppConfigGroupAssignment**<br/>**windows10KioskConfiguration**<br/>|
|Löschung|Beta|[assign](/graph/api/intune-apps-manageddevicemobileappconfiguration-assign?view=graph-rest-beta)-Aktion für [managedDeviceMobileAppConfiguration](/graph/api/resources/intune-apps-manageddevicemobileappconfiguration?view=graph-rest-beta) entfernt. |
|Löschung|Beta|[syncApps](/graph/api/intune-onboarding-applevolumepurchaseprogramtoken-syncapps?view=graph-rest-beta)-Aktion für [appleVolumePurchaseProgramToken](/graph/api/resources/intune-onboarding-applevolumepurchaseprogramtoken?view=graph-rest-beta) entfernt. |
|Ergänzungen|Beta|**workProfileBluetoothEnableContactSharing**-Eigenschaft zur [androidForWorkGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration?view=graph-rest-beta)-Entität hinzugefügt.|
|Ergänzungen|Beta|**intendedPurpose**-Eigenschaft zur [androidForWorkImportedPFXCertificateProfile](/graph/api/resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile?view=graph-rest-beta)-Entität hinzugefügt|
|Ergänzungen|Beta|**intendedPurpose**-Eigenschaft zur [androidImportedPFXCertificateProfile](/graph/api/resources/intune-deviceconfig-androidimportedpfxcertificateprofile?view=graph-rest-beta)-Entität hinzugefügt|
|Ergänzungen|Beta|**intendedPurpose**-Eigenschaft zur [iosImportedPFXCertificateProfile](/graph/api/resources/intune-deviceconfig-iosimportedpfxcertificateprofile?view=graph-rest-beta)-Entität hinzugefügt|
|Ergänzungen|Beta|**encodedSettingXml**-Eigenschaft zur [iosMobileAppConfiguration](/graph/api/resources/intune-apps-iosmobileappconfiguration?view=graph-rest-beta)-Entität hinzugefügt|
|Ergänzungen|Beta|Eigenschaften **managedDeviceId** und **azureADDeviceId** zur [managedAppRegistration](/graph/api/resources/intune-mam-managedappregistration?view=graph-rest-beta)-Entität hinzugefügt|
|Ergänzungen|Beta|**usersLoggedOn**-Eigenschaft zur [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta)-Entität hinzugefügt|
|Löschung|Beta|**lastLoggedOnUserId**-Eigenschaft aus [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta)-Entität entfernt|
|Ergänzungen|Beta|**lastModifiedDateTime**-Eigenschaft zur [managedDeviceOverview](/graph/api/resources/intune-devices-manageddeviceoverview?view=graph-rest-beta)-Entität hinzugefügt|
|Ergänzungen|Beta|**isDependency**-Eigenschaft zur [mobileAppContentFile](/graph/api/resources/intune-apps-mobileappcontentfile?view=graph-rest-beta)-Entität hinzugefügt|
|Ergänzungen|Beta|Eigenschaften **windowsEnabled**, **macEnabled**, **windowsDeviceBlockedOnMissingPartnerData** und **macDeviceBlockedOnMissingPartnerData** zur [mobileThreatDefenseConnector](/graph/api/resources/intune-onboarding-mobilethreatdefenseconnector?view=graph-rest-beta)-Entität hinzugefügt|
|Ergänzungen|Beta|**shouldUninstallOlderVersionsOfOffice**-Eigenschaft zur [officeSuiteApp](/graph/api/resources/intune-apps-officesuiteapp?view=graph-rest-beta)-Entität hinzugefügt|
|Ergänzungen|Beta|**dataSharingConsentGranted**-Eigenschaft zur [vppToken](/graph/api/resources/intune-onboarding-vpptoken?view=graph-rest-beta)-Entität hinzugefügt|
|Ergänzungen|Beta|Eigenschaften **localSecurityOptionsBlockRemoteLogonWithBlankPassword**, **localSecurityOptionsAdministratorAccountName**, **localSecurityOptionsEnableGuestAccount**, **localSecurityOptionsGuestAccountName**, **localSecurityOptionsAllowUndockWithoutHavingToLogon**, **localSecurityOptionsBlockUsersInstallingPrinterDrivers**, **localSecurityOptionsBlockRemoteOpticalDriveAccess**, **localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser**, **localSecurityOptionsMachineInactivityLimit**, **localSecurityOptionsDoNotRequireCtrlAltDel**, **localSecurityOptionsInformationDisplayedOnLockScreen**, **localSecurityOptionsHideLastSignedInUser**, **localSecurityOptionsHideUsernameAtSignIn**, **localSecurityOptionsLogOnMessageTitle**, **localSecurityOptionsLogOnMessageText**, **localSecurityOptionsAllowPKU2UAuthenticationRequests**, **localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager**, **localSecurityOptionsClearVirtualMemoryPageFile**, **localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn**, **localSecurityOptionsAllowUIAccessApplicationElevation**, **localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations**, **localSecurityOptionsOnlyElevateSignedExecutables**, **localSecurityOptionsAdministratorElevationPromptBehavior**, **localSecurityOptionsStandardUserElevationPromptBehavior**, **localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation**, **localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation**, **localSecurityOptionsAllowUIAccessApplicationsForSecureLocations**, **localSecurityOptionsUseAdminApprovalMode**, **localSecurityOptionsUseAdminApprovalModeForAdministrators**, **deviceGuardLocalSystemAuthorityCredentialGuardSettings**, **deviceGuardEnableVirtualizationBasedSecurity** und **deviceGuardEnableSecureBootWithDMA** zur [windows10EndpointProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windows10endpointprotectionconfiguration?view=graph-rest-beta)-Entität hinzugefügt|
|Löschung|Beta|**defenderPasswordProtectedEmailContentExecutionType**-Eigenschaft aus der [windows10EndpointProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windows10endpointprotectionconfiguration?view=graph-rest-beta)-Entität entfernt|
|Ergänzungen|Beta|**intendedPurpose**-Eigenschaft zur [windows10ImportedPFXCertificateProfile](/graph/api/resources/intune-deviceconfig-windows10importedpfxcertificateprofile?view=graph-rest-beta)-Entität hinzugefügt|
|Löschung|Beta|Eigenschaften **printerNames**, **defaultPrinterName** und **blockAddingNewPrinter** aus Entität [windows10SecureAssessmentConfiguration](/graph/api/resources/intune-deviceconfig-windows10secureassessmentconfiguration?view=graph-rest-beta) entfernt|
|Ergänzungen|Beta|**certificateStore**-Eigenschaft zur [windows81SCEPCertificateProfile](/graph/api/resources/intune-deviceconfig-windows81scepcertificateprofile?view=graph-rest-beta)-Entität hinzugefügt|
|Ergänzungen|Beta|**purchaseOrderIdentifier**-Eigenschaft zur [windowsAutopilotDeviceIdentity](/graph/api/resources/intune-enrollment-windowsautopilotdeviceidentity?view=graph-rest-beta)-Entität hinzugefügt|
|Änderung|Beta|Folgende Eigenschaften für [windowsCertificateProfileBase](/graph/api/resources/intune-deviceconfig-windowscertificateprofilebase?view=graph-rest-beta)-Entität geändert:<br/>**SubjectAlternativeNameType** von erforderlich in optional<br/>|
|Ergänzungen|Beta|Eigenschaften **advancedThreatProtectionOnboardingFilename** und **advancedThreatProtectionOffboardingFilename** zur [windowsDefenderAdvancedThreatProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration?view=graph-rest-beta)-Entität hinzugefügt|
|Ergänzungen|Beta|**intendedPurpose**-Eigenschaft zur [windowsPhone81ImportedPFXCertificateProfile](/graph/api/resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile?view=graph-rest-beta)-Entität hinzugefügt|
|Ergänzungen|Beta|Eigenschaften **skipChecksBeforeRestart** und **updateWeeks** zur [windowsUpdateForBusinessConfiguration](/graph/api/resources/intune-deviceconfig-windowsupdateforbusinessconfiguration?view=graph-rest-beta)-Entität hinzugefügt|
|Ergänzungen|Beta|**mobileAppConfigurations**-Navigationseigenschaft zur [deviceAppManagement](/graph/api/resources/intune-apps-deviceappmanagement?view=graph-rest-beta)- Entität hinzugefügt|
|Ergänzungen|Beta|Navigationseigenschaften **androidManagedStoreAccountEnterpriseSettings**, **androidManagedStoreAppConfigurationSchemas**, **androidDeviceOwnerEnrollmentProfiles**, **dataSharingConsents** und **deviceConfigurationUserStateSummaries** zur [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta)-Entität hinzugefügt|
|Löschung|Beta|**deviceSetupConfigurations**-Navigationseigenschaft aus der [deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-beta)-Entität entfernt|
|Löschung|Beta|**assignments**-Navigationseigenschaft aus der [managedDeviceMobileAppConfiguration](/graph/api/resources/intune-apps-manageddevicemobileappconfiguration?view=graph-rest-beta)-Entität entfernt|
|Ergänzungen|Beta|**categories**-Navigationseigenschaft zur [managedEBook](/graph/api/resources/intune-books-managedebook?view=graph-rest-beta)-Entität hinzugefügt|
|Ergänzungen|Beta|**containedApps**-Navigationseigenschaft zur [microsoftStoreForBusinessApp](/graph/api/resources/intune-apps-microsoftstoreforbusinessapp?view=graph-rest-beta)-Entität hinzugefügt|
|Ergänzungen|Beta|**containedApps**-Navigationseigenschaft zur [mobileAppContent](/graph/api/resources/intune-apps-mobileappcontent?view=graph-rest-beta)-Entität hinzugefügt|
|Ergänzungen|Beta|Navigationseigenschaft **committedContainedApps** zur Entität [windowsUniversalAppX](/graph/api/resources/intune-apps-windowsuniversalappx?view=graph-rest-beta) hinzugefügt.|

### <a name="onedrive"></a>OneDrive
|Änderungstyp|Version|Beschreibung|
|:---|:---|:---|
|Ergänzungen|v1.0|Neue Entitäten hinzugefügt:<br/>[baseItemVersion](/graph/api/resources/baseitemversion?view=graph-rest-1.0)<br/>[driveItemVersion](/graph/api/resources/driveitemversion?view=graph-rest-1.0)<br/>[listItemVersion](/graph/api/resources/listitemversion?view=graph-rest-1.0)<br/> |
|Ergänzungen|v1.0|Neue komplexe Typen hinzugefügt:<br/>[publicationFacet](/graph/api/resources/publicationfacet?view=graph-rest-1.0)<br/> |
|Ergänzungen|v1.0|Eigenschaft <b>publication</b> zur Entität [driveItem](/graph/api/resources/driveitem?view=graph-rest-1.0) hinzugefügt. |
|Ergänzungen|v1.0|Navigationseigenschaft <b>versions</b> zur Entität [driveItem](/graph/api/resources/driveitem?view=graph-rest-1.0) hinzugefügt. |
|Ergänzungen|v1.0|Navigationseigenschaft <b>versions</b> zur Entität [listItem](/graph/api/resources/listitem?view=graph-rest-1.0) hinzugefügt. |
|Ergänzungen|v1.0|Eigenschaft <b>root</b> zur Entität [siteCollection](/graph/api/resources/sitecollection?view=graph-rest-1.0) hinzugefügt. |
|Ergänzungen|v1.0|Aktion [restoreVersion](/graph/api/driveitemversion-restore?view=graph-rest-1.0) zur Entität [driveItemVersion](/graph/api/resources/driveitemversion?view=graph-rest-1.0) hinzugefügt. |
|Ergänzungen|v1.0|Aktion [restoreVersion](/graph/api/listitemversion-restore?view=graph-rest-1.0) zur Entität [listItemVersion](/graph/api/resources/listitemversion?view=graph-rest-1.0) hinzugefügt. |


### <a name="onedrive"></a>OneDrive
|Änderungstyp|Version|Beschreibung|
|:---|:---|:---|
|Ergänzungen|Beta|Neuer komplexer Typ hinzugefügt:<br/>[itemPreviewInfo](/graph/api/resources/itempreviewinfo?view=graph-rest-beta)<br/> |
|Ergänzungen|Beta|Eigenschaft <b>name</b> zum komplexen Typ [contentTypeInfo](/graph/api/resources/contenttypeinfo?view=graph-rest-beta) hinzugefügt. |
|Ergänzungen|Beta|Eigenschaft <b>objectType</b> zum komplexen Typ [deleteAction](/graph/api/resources/deleteaction?view=graph-rest-beta) hinzugefügt. |
|Ergänzungen|Beta|Eigenschaft <b>newName</b> zum komplexen Typ [renameAction](/graph/api/resources/renameaction?view=graph-rest-beta) hinzugefügt. |
|Ergänzungen|Beta|Eigenschaft <b>tenantId</b> zum komplexen Typ [sharepointIds](/graph/api/resources/renameaction?view=graph-rest-beta) hinzugefügt. |
|Ergänzungen|Beta|Eigenschaft <b>lastRecordedDateTime</b> zum komplexen Typ [itemActivityTimeSet](/graph/api/resources/itemactivitytimeset?view=graph-rest-beta) hinzugefügt. |
|Ergänzungen|Beta|Aktion [preview](/graph/api/driveitem-preview?view=graph-rest-beta) zur Entität [driveItem](/graph/api/resources/driveitem?view=graph-rest-beta) hinzugefügt. |

### <a name="reports-apis"></a>Bericht-APIs

| **Änderungstyp** | **Version** | **Beschreibung**                          |
| :-------------- | :---------- | :--------------------------------------- |
|Ergänzungen|Beta|Die **siteId**-Eigenschaft wurde der [sharePointSiteUsageDetail](/graph/api/resources/sharepointsiteusagedetail?view=graph-rest-beta)-Entität hinzugefügt.|

### <a name="terms-of-use"></a>Nutzungsbedingungen

| **Änderungstyp** | **Version** | **Beschreibung**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Ergänzungen        | Beta        | Ressourcen [agreement](/graph/api/resources/agreement?view=graph-rest-beta) und [agreementAcceptance](/graph/api/resources/agreementacceptance?view=graph-rest-beta) hinzugefügt. |
| Ergänzungen        | Beta        | Folgende APIs für [agreement](/graph/api/resources/agreement?view=graph-rest-beta) hinzugefügt: [Create](/graph/api/greement-post-agreements?view=graph-rest-beta), [List](/graph/api/agreement-list?view=graph-rest-beta), [Get](/graph/api/agreement-get?view=graph-rest-beta), [Update](/graph/api/agreement-update?view=graph-rest-beta), [Delete](/graph/api/agreement-delete?view=graph-rest-beta). |
| Ergänzungen        | Beta        | [agreementAcceptance](/graph/api/resources/agreementacceptance?view=graph-rest-beta)-Beziehungen zur [user](/graph/api/resources/user?view=graph-rest-beta)-Ressource hinzugefügt. |

## <a name="february-2018"></a>Februar 2018

### <a name="microsoft-intune-apis"></a>Microsoft Intune-APIs
|Änderungstyp|Version|Beschreibung|
|:---|:---|:---|
|Ergänzungen|Beta|Hinzugefügte neue Entitäten:<br/>[androidForWorkImportedPFXCertificateProfile](/graph/api/resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile?view=graph-rest-beta)<br/>[androidImportedPFXCertificateProfile](/graph/api/resources/intune-deviceconfig-androidimportedpfxcertificateprofile?view=graph-rest-beta)<br/>[importedWindowsAutopilotDeviceIdentity](/graph/api/resources/intune-enrollment-importedwindowsautopilotdeviceidentity?view=graph-rest-beta)<br/>[iosImportedPFXCertificateProfile](/graph/api/resources/intune-deviceconfig-iosimportedpfxcertificateprofile?view=graph-rest-beta)<br/>[windows10ImportedPFXCertificateProfile](/graph/api/resources/intune-deviceconfig-windows10importedpfxcertificateprofile?view=graph-rest-beta)<br/>[windows10KioskConfiguration](/graph/api/resources/intune-deviceconfig-windows10kioskconfiguration?view=graph-rest-beta)<br/>[windowsPhone81ImportedPFXCertificateProfile](/graph/api/resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile?view=graph-rest-beta)<br/>|
|Ergänzungen|Beta|Die folgenden komplexen Typen wurden hinzugefügt:<br/>[importedWindowsAutopilotDeviceIdentityState](/graph/api/resources/intune-enrollment-importedwindowsautopilotdeviceidentitystate?view=graph-rest-beta)<br/>|
|Ergänzungen|Beta|Die Funktion [managedDeviceEnrollmentFailureDetails](/graph/api/intune-troubleshooting-reportroot-manageddeviceenrollmentfailuredetails?view=graph-rest-beta) wurde zu [reportRoot](/graph/api/resources/intune-deviceconfig-reportroot?view=graph-rest-beta) hinzugefügt. |
|Ergänzungen|Beta|Die Funktion [managedDeviceEnrollmentFailureDetails](/graph/api/intune-troubleshooting-reportroot-manageddeviceenrollmentfailuredetails?view=graph-rest-beta) wurde zu [reportRoot](/graph/api/resources/intune-deviceconfig-reportroot?view=graph-rest-beta) hinzugefügt. |
|Ergänzungen|Beta|Die Funktion [managedDeviceEnrollmentFailureTrends](/graph/api/intune-troubleshooting-reportroot-manageddeviceenrollmentfailuretrends?view=graph-rest-beta) wurde zu [reportRoot](/graph/api/resources/intune-deviceconfig-reportroot?view=graph-rest-beta) hinzugefügt. |
|Ergänzungen|Beta|Die Funktion [managedDeviceEnrollmentTopFailures](/graph/api/intune-troubleshooting-reportroot-manageddeviceenrollmenttopfailures?view=graph-rest-beta) wurde zu [reportRoot](/graph/api/resources/intune-deviceconfig-reportroot?view=graph-rest-beta) hinzugefügt. |
|Ergänzungen|Beta|Die Funktion [managedDeviceEnrollmentTopFailures](/graph/api/intune-troubleshooting-reportroot-manageddeviceenrollmenttopfailures?view=graph-rest-beta) wurde zu [reportRoot](/graph/api/resources/intune-deviceconfig-reportroot?view=graph-rest-beta) hinzugefügt. |
|Änderung|Beta|Die Eigenschaften **requireAppVerify**, **requireSafetyNetAttestationBasicIntegrity**, **requireSafetyNetAttestationCertifiedDevice**, **requireGooglePlayServices**, **requireUpToDateSecurityProviders** und **requireCompanyPortalAppIntegrity** wurden aus der Entität [androidCompliancePolicy](/graph/api/resources/intune-deviceconfig-androidcompliancepolicy?view=graph-rest-beta) entfernt.|
|Änderung|Beta|Die Eigenschaften **requireAppVerify**, **requireSafetyNetAttestationBasicIntegrity**, **requireSafetyNetAttestationCertifiedDevice**, **requireGooglePlayServices**, **requireUpToDateSecurityProviders** und **requireCompanyPortalAppIntegrity** wurden aus der Entität [androidForWorkCompliancePolicy](/graph/api/resources/intune-deviceconfig-androidforworkcompliancepolicy?view=graph-rest-beta) entfernt.|
|Änderung|Beta|Die Eigenschaften **name**, **modifiedDateTime**, **totalEnrollmentCount** und **qrCode** wurden aus der Entität [androidForWorkEnrollmentProfile](/graph/api/resources/intune-androidforwork-androidforworkenrollmentprofile?view=graph-rest-beta) entfernt.|
|Änderung|Beta|Die Eigenschaften **nonEapAuthenticationMethodForEapTtls**, **nonEapAuthenticationMethodForPeap** und **enableOuterIdentityPrivacy** wurden aus der Entität [androidForWorkEnterpriseWiFiConfiguration](/graph/api/resources/intune-deviceconfig-androidforworkenterprisewificonfiguration?view=graph-rest-beta) entfernt.|
|Änderung|Beta|Die Eigenschaft **workProfileBlockAddingAccounts** wurde zur Entität [androidForWorkGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration?view=graph-rest-beta) hinzugefügt.|
|Änderung|Beta|Die Eigenschaften **blockCrossProfileCopyPaste** und **requireAppVerify** wurden aus der Entität [androidForWorkGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration?view=graph-rest-beta) entfernt.|
|Änderung|Beta|Die Eigenschaft **deviceOwnerManagementEnabled** wurde zur Entität [androidForWorkSettings](/graph/api/resources/intune-androidforwork-androidforworksettings?view=graph-rest-beta) hinzugefügt.|
|Änderung|Beta|Die Eigenschaft **requireAppVerify** wurde aus der Entität [androidGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidgeneraldeviceconfiguration?view=graph-rest-beta) entfernt.|
|Änderung|Beta|Die Eigenschaft **exemptedAppPackages** wurde zur Entität [androidManagedAppProtection](/graph/api/resources/intune-mam-androidmanagedappprotection?view=graph-rest-beta) hinzugefügt.|
|Änderung|Beta|Die Eigenschaften **exemptedAppProtocols** und **exemptedAppPackages** wurden zur Entität [defaultManagedAppProtection](/graph/api/resources/intune-mam-defaultmanagedappprotection?view=graph-rest-beta) hinzugefügt.|
|Änderung|Beta|Die Eigenschaft **exemptedAppProtocols** wurde zur Entität [iosManagedAppProtection](/graph/api/resources/intune-mam-iosmanagedappprotection?view=graph-rest-beta) hinzugefügt.|
|Änderung|Beta|Die Eigenschaft **lastLoggedOnUserId** wurde zur Entität [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) hinzugefügt.|
|Änderung|Beta|Die Eigenschaft **isFrameworkFile** wurde zur Entität [mobileAppContentFile](/graph/api/resources/intune-apps-mobileappcontentfile?view=graph-rest-beta) hinzugefügt.|
|Änderung|Beta|Die Eigenschaft **targetedAppManagementLevels** wurde zur Entität [targetedManagedAppProtection](/graph/api/resources/intune-mam-targetedmanagedappprotection?view=graph-rest-beta) hinzugefügt.|
|Änderung|Beta|Die Eigenschaften **localSecurityOptionsBlockMicrosoftAccounts**, **localSecurityOptionsEnableAdministratorAccount**, **defenderPreventCredentialStealingType**, **defenderProcessCreationType**, **defenderUntrustedUSBProcessType**, **defenderUntrustedExecutableType**, **defenderPasswordProtectedEmailContentExecutionType**, **defenderAdvancedRansomewareProtectionType** und **applicationGuardAllowFileSaveOnHost** wurden zur Entität [windows10EndpointProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windows10endpointprotectionconfiguration?view=graph-rest-beta) hinzugefügt.|
|Änderung|Beta|Die Eigenschaften **edgeFavoritesListLocation** und **edgeBlockEditFavorites** wurden zur Entität [windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta) hinzugefügt.|
|Änderung|Beta|Die Eigenschaften **printerNames**, **defaultPrinterName** und **blockAddingNewPrinter** wurden zur Entität [windows10SecureAssessmentConfiguration](/graph/api/resources/intune-deviceconfig-windows10secureassessmentconfiguration?view=graph-rest-beta) hinzugefügt.|
|Änderung|Beta|Die Navigationseigenschaft **importedWindowsAutopilotDeviceIdentities** wurde zur Entität [deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-beta) hinzugefügt.|
|Änderung|Beta|Die Eigenschaft **shareAPNSData** wurde zum komplexen Typ [adminConsent](/graph/api/resources/intune-devices-adminconsent?view=graph-rest-beta) hinzugefügt.|
|Änderung|Beta|Die Eigenschaft **collectFullIOSAppInventory** wurde aus dem komplexen Typ [adminConsent](/graph/api/resources/intune-devices-adminconsent?view=graph-rest-beta) entfernt.|
|Änderung|Beta|Die Eigenschaft **deviceUsageType** wurde aus dem komplexen Typ [outOfBoxExperienceSettings](/graph/api/resources/intune-enrollment-outofboxexperiencesettings?view=graph-rest-beta) entfernt.|


### <a name="planner-apis"></a>Planner-APIs

|Änderungstyp|Version|Beschreibung|
|:---|:---|:---|
|Ergänzungen|Beta|Die folgenden komplexen Typen wurden hinzugefügt:<br/>[plannerPlanContext](/graph/api/resources/plannerplancontext?view=graph-rest-beta)<br/>[plannerPlanContextDetails](/graph/api/resources/plannerplancontextdetails?view=graph-rest-beta)<br/>[plannerPlanContextCollection](/graph/api/resources/plannerplancontextcollection?view=graph-rest-beta)<br/>[plannerPlanContextDetailsCollection](/graph/api/resources/plannerplancontextdetailscollection?view=graph-rest-beta)<br/>[plannerFavoritePlanReference](/graph/api/resources/plannerfavoriteplanreference?view=graph-rest-beta)<br/>[plannerRecentPlanReference](/graph/api/resources/plannerrecentplanreference?view=graph-rest-beta)<br/>[plannerFavoritePlanReferenceCollection](/graph/api/resources/plannerfavoriteplanreferencecollection?view=graph-rest-beta)<br/>[plannerRecentPlanReferenceCollection](/graph/api/resources/plannerrecentplanreferencecollection?view=graph-rest-beta)|
|Ergänzungen|Beta|Die Eigenschaften `favoritePlanReferences` und `recentPlanReferences` wurden der [plannerUser](/graph/api/resources/planneruser?view=graph-rest-beta)-Entität hinzugefügt. |
|Ergänzungen|Beta|Die Navigationseigenschaften `favoritePlans` und `recentPlans` wurden der [plannerUser](/graph/api/resources/planneruser?view=graph-rest-beta)-Entität hinzugefügt. |
|Ergänzungen|Beta|Die `contexts`-Eigenschaft wurde der [plannerPlan](/graph/api/resources/plannerplan?view=graph-rest-beta)-Entität hinzugefügt. |
|Ergänzungen|Beta|Eigenschaft `contextDetails` zur Entität [plannerPlanDetails](/graph/api/resources/plannerplandetails?view=graph-rest-beta) hinzugefügt. |
|Ergänzungen|Beta|Planner-[Deltaabfrage](/graph/api/planneruser-list-delta?view=graph-rest-beta) hinzugefügt. |

### <a name="reports-apis"></a>Bericht-APIs
| Änderungstyp | Version | Beschreibung                              |
|:------------|:--------|:-----------------------------------------|
| Ergänzungen    | Beta    | Die **activatedOnSharedComputer**-Eigenschaft wurde der [userActivationCounts](/graph/api/resources/useractivationcounts?view=graph-rest-beta)-Entität hinzugefügt.|
| Ergänzungen    | Beta    | Die **sharedComputerActivation**-Eigenschaft wurde der [office365ActivationsUserCounts](/graph/api/resources/office365activationsusercounts?view=graph-rest-beta)-Entität hinzugefügt.|

## <a name="january-2018"></a>Januar 2018

### <a name="education-apis"></a>Bildungs-APIs

|Änderungstyp|Version|Beschreibung|
|:---|:---|:---|
|Ergänzungen|Beta|Zusätzliche Navigationseigenschaften hinzugefügt und Unterstützung für Filter für die [Dienstplan-API](/graph/api/resources/education-overview?view=graph-rest-beta) verbessert.|

### <a name="json-batching"></a>JSON-Batchverarbeitung

|Änderungstyp|Version|Beschreibung|
|:---|:---|:---|
|Ergänzungen|v1.0|Added [JSON batching](json-batching.md) support. Internal request limit set to 20.|
|Änderung|Beta|Das interne Anforderungslimit der [JSON-Batchverarbeitung](json-batching.md) wurde von 5 auf 20 erhöht.|

### <a name="microsoft-intune-apis"></a>Microsoft Intune-APIs
|Änderungstyp|Version|Beschreibung|
|:---|:---|:---|
|Ergänzungen|v1.0|Hinzugefügte neue Entitäten:<br/>[androidCompliancePolicy](/graph/api/resources/intune-deviceconfig-androidcompliancepolicy?view=graph-rest-1.0)<br/>[androidCustomConfiguration](/graph/api/resources/intune-deviceconfig-androidcustomconfiguration?view=graph-rest-1.0)<br/>[androidGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidgeneraldeviceconfiguration?view=graph-rest-1.0)<br/>[androidLobApp](/graph/api/resources/intune-apps-androidlobapp?view=graph-rest-1.0)<br/>[androidManagedAppProtection](/graph/api/resources/intune-mam-androidmanagedappprotection?view=graph-rest-1.0)<br/>[androidManagedAppRegistration](/graph/api/resources/intune-mam-androidmanagedappregistration?view=graph-rest-1.0)<br/>[androidStoreApp](/graph/api/resources/intune-apps-androidstoreapp?view=graph-rest-1.0)<br/>[appleDeviceFeaturesConfigurationBase](/graph/api/resources/intune-deviceconfig-appledevicefeaturesconfigurationbase?view=graph-rest-1.0)<br/>[applePushNotificationCertificate](/graph/api/resources/intune-devices-applepushnotificationcertificate?view=graph-rest-1.0)<br/>[defaultManagedAppProtection](/graph/api/resources/intune-mam-defaultmanagedappprotection?view=graph-rest-1.0)<br/>[detectedApp](/graph/api/resources/intune-devices-detectedapp?view=graph-rest-1.0)<br/>[deviceAndAppManagementRoleAssignment](/graph/api/resources/intune-rbac-deviceandappmanagementroleassignment?view=graph-rest-1.0)<br/>[deviceAndAppManagementRoleDefinition](/graph/api/resources/intune-rbac-deviceandappmanagementroledefinition?view=graph-rest-1.0)<br/>[deviceAppManagement](/graph/api/resources/intune-shared-deviceappmanagement?view=graph-rest-1.0)<br/>[deviceCategory](/graph/api/resources/intune-shared-devicecategory?view=graph-rest-1.0)<br/>[deviceComplianceActionItem](/graph/api/resources/intune-deviceconfig-devicecomplianceactionitem?view=graph-rest-1.0)<br/>[deviceComplianceDeviceOverview](/graph/api/resources/intune-deviceconfig-devicecompliancedeviceoverview?view=graph-rest-1.0)<br/>[deviceComplianceDeviceStatus](/graph/api/resources/intune-deviceconfig-devicecompliancedevicestatus?view=graph-rest-1.0)<br/>[deviceCompliancePolicy](/graph/api/resources/intune-deviceconfig-devicecompliancepolicy?view=graph-rest-1.0)<br/>[deviceCompliancePolicyAssignment](/graph/api/resources/intune-deviceconfig-devicecompliancepolicyassignment?view=graph-rest-1.0)<br/>[deviceCompliancePolicyDeviceStateSummary](/graph/api/resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary?view=graph-rest-1.0)<br/>[deviceCompliancePolicySettingStateSummary](/graph/api/resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary?view=graph-rest-1.0)<br/>[deviceCompliancePolicyState](/graph/api/resources/intune-deviceconfig-devicecompliancepolicystate?view=graph-rest-1.0)<br/>[deviceComplianceScheduledActionForRule](/graph/api/resources/intune-deviceconfig-devicecompliancescheduledactionforrule?view=graph-rest-1.0)<br/>[deviceComplianceSettingState](/graph/api/resources/intune-deviceconfig-devicecompliancesettingstate?view=graph-rest-1.0)<br/>[deviceComplianceUserOverview](/graph/api/resources/intune-deviceconfig-devicecomplianceuseroverview?view=graph-rest-1.0)<br/>[deviceComplianceUserStatus](/graph/api/resources/intune-deviceconfig-devicecomplianceuserstatus?view=graph-rest-1.0)<br/>[deviceConfiguration](/graph/api/resources/intune-deviceconfig-deviceconfiguration?view=graph-rest-1.0)<br/>[deviceConfigurationAssignment](/graph/api/resources/intune-deviceconfig-deviceconfigurationassignment?view=graph-rest-1.0)<br/>[deviceConfigurationDeviceOverview](/graph/api/resources/intune-deviceconfig-deviceconfigurationdeviceoverview?view=graph-rest-1.0)<br/>[deviceConfigurationDeviceStateSummary](/graph/api/resources/intune-deviceconfig-deviceconfigurationdevicestatesummary?view=graph-rest-1.0)<br/>[deviceConfigurationDeviceStatus](/graph/api/resources/intune-deviceconfig-deviceconfigurationdevicestatus?view=graph-rest-1.0)<br/>[deviceConfigurationState](/graph/api/resources/intune-deviceconfig-deviceconfigurationstate?view=graph-rest-1.0)<br/>[deviceConfigurationUserOverview](/graph/api/resources/intune-deviceconfig-deviceconfigurationuseroverview?view=graph-rest-1.0)<br/>[deviceConfigurationUserStatus](/graph/api/resources/intune-deviceconfig-deviceconfigurationuserstatus?view=graph-rest-1.0)<br/>[deviceEnrollmentConfiguration](/graph/api/resources/intune-onboarding-deviceenrollmentconfiguration?view=graph-rest-1.0)<br/>[deviceEnrollmentLimitConfiguration](/graph/api/resources/intune-onboarding-deviceenrollmentlimitconfiguration?view=graph-rest-1.0)<br/>[deviceEnrollmentPlatformRestrictionsConfiguration](/graph/api/resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration?view=graph-rest-1.0)<br/>[deviceEnrollmentWindowsHelloForBusinessConfiguration](/graph/api/resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration?view=graph-rest-1.0)<br/>[deviceInstallState](/graph/api/resources/intune-books-deviceinstallstate?view=graph-rest-1.0)<br/>[deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-1.0)<br/>[deviceManagementExchangeConnector](/graph/api/resources/intune-onboarding-devicemanagementexchangeconnector?view=graph-rest-1.0)<br/>[deviceManagementPartner](/graph/api/resources/intune-onboarding-devicemanagementpartner?view=graph-rest-1.0)<br/>[deviceManagementTroubleshootingEvent](/graph/api/resources/intune-troubleshooting-devicemanagementtroubleshootingevent?view=graph-rest-1.0)<br/>[eBookInstallSummary](/graph/api/resources/intune-books-ebookinstallsummary?view=graph-rest-1.0)<br/>[editionUpgradeConfiguration](/graph/api/resources/intune-deviceconfig-editionupgradeconfiguration?view=graph-rest-1.0)<br/>[enrollmentConfigurationAssignment](/graph/api/resources/intune-onboarding-enrollmentconfigurationassignment?view=graph-rest-1.0)<br/>[enrollmentTroubleshootingEvent](/graph/api/resources/intune-troubleshooting-enrollmenttroubleshootingevent?view=graph-rest-1.0)<br/>[iosCertificateProfile](/graph/api/resources/intune-deviceconfig-ioscertificateprofile?view=graph-rest-1.0)<br/>[iosCompliancePolicy](/graph/api/resources/intune-deviceconfig-ioscompliancepolicy?view=graph-rest-1.0)<br/>[iosCustomConfiguration](/graph/api/resources/intune-deviceconfig-ioscustomconfiguration?view=graph-rest-1.0)<br/>[iosDeviceFeaturesConfiguration](/graph/api/resources/intune-deviceconfig-iosdevicefeaturesconfiguration?view=graph-rest-1.0)<br/>[iosGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-iosgeneraldeviceconfiguration?view=graph-rest-1.0)<br/>[iosLobApp](/graph/api/resources/intune-apps-ioslobapp?view=graph-rest-1.0)<br/>[iosManagedAppProtection](/graph/api/resources/intune-mam-iosmanagedappprotection?view=graph-rest-1.0)<br/>[iosManagedAppRegistration](/graph/api/resources/intune-mam-iosmanagedappregistration?view=graph-rest-1.0)<br/>[iosStoreApp](/graph/api/resources/intune-apps-iosstoreapp?view=graph-rest-1.0)<br/>[iosUpdateConfiguration](/graph/api/resources/intune-deviceconfig-iosupdateconfiguration?view=graph-rest-1.0)<br/>[iosUpdateDeviceStatus](/graph/api/resources/intune-deviceconfig-iosupdatedevicestatus?view=graph-rest-1.0)<br/>[iosVppApp](/graph/api/resources/intune-apps-iosvppapp?view=graph-rest-1.0)<br/>[iosVppEBook](/graph/api/resources/intune-books-iosvppebook?view=graph-rest-1.0)<br/>[iosVppEBookAssignment](/graph/api/resources/intune-books-iosvppebookassignment?view=graph-rest-1.0)<br/>[localizedNotificationMessage](/graph/api/resources/intune-notification-localizednotificationmessage?view=graph-rest-1.0)<br/>[macOSCompliancePolicy](/graph/api/resources/intune-deviceconfig-macoscompliancepolicy?view=graph-rest-1.0)<br/>[macOSCustomConfiguration](/graph/api/resources/intune-deviceconfig-macoscustomconfiguration?view=graph-rest-1.0)<br/>[macOSDeviceFeaturesConfiguration](/graph/api/resources/intune-deviceconfig-macosdevicefeaturesconfiguration?view=graph-rest-1.0)<br/>[macOSGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-macosgeneraldeviceconfiguration?view=graph-rest-1.0)<br/>[macOSOfficeSuiteApp](/graph/api/resources/intune-apps-macosofficesuiteapp?view=graph-rest-1.0)<br/>[managedAndroidLobApp](/graph/api/resources/intune-apps-managedandroidlobapp?view=graph-rest-1.0)<br/>[managedAndroidStoreApp](/graph/api/resources/intune-apps-managedandroidstoreapp?view=graph-rest-1.0)<br/>[managedApp](/graph/api/resources/intune-apps-managedapp?view=graph-rest-1.0)<br/>[managedAppConfiguration](/graph/api/resources/intune-mam-managedappconfiguration?view=graph-rest-1.0)<br/>[managedAppOperation](/graph/api/resources/intune-mam-managedappoperation?view=graph-rest-1.0)<br/>[managedAppPolicy](/graph/api/resources/intune-mam-managedapppolicy?view=graph-rest-1.0)<br/>[managedAppPolicyDeploymentSummary](/graph/api/resources/intune-mam-managedapppolicydeploymentsummary?view=graph-rest-1.0)<br/>[managedAppProtection](/graph/api/resources/intune-mam-managedappprotection?view=graph-rest-1.0)<br/>[managedAppRegistration](/graph/api/resources/intune-mam-managedappregistration?view=graph-rest-1.0)<br/>[managedAppStatus](/graph/api/resources/intune-mam-managedappstatus?view=graph-rest-1.0)<br/>[managedAppStatusRaw](/graph/api/resources/intune-mam-managedappstatusraw?view=graph-rest-1.0)<br/>[managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0)<br/>[managedDeviceMobileAppConfiguration](/graph/api/resources/intune-apps-manageddevicemobileappconfiguration?view=graph-rest-1.0)<br/>[managedDeviceMobileAppConfigurationAssignment](/graph/api/resources/intune-apps-manageddevicemobileappconfigurationassignment?view=graph-rest-1.0)<br/>[managedDeviceMobileAppConfigurationDeviceSummary](/graph/api/resources/intune-apps-manageddevicemobileappconfigurationdevicesummary?view=graph-rest-1.0)<br/>[managedDeviceMobileAppConfigurationUserStatus](/graph/api/resources/intune-apps-manageddevicemobileappconfigurationuserstatus?view=graph-rest-1.0)<br/>[managedDeviceMobileAppConfigurationUserSummary](/graph/api/resources/intune-apps-manageddevicemobileappconfigurationusersummary?view=graph-rest-1.0)<br/>[managedDeviceOverview](/graph/api/resources/intune-devices-manageddeviceoverview?view=graph-rest-1.0)<br/>[managedEBook](/graph/api/resources/intune-books-managedebook?view=graph-rest-1.0)<br/>[managedEBookAssignment](/graph/api/resources/intune-books-managedebookassignment?view=graph-rest-1.0)<br/>[managedIOSLobApp](/graph/api/resources/intune-apps-managedioslobapp?view=graph-rest-1.0)<br/>[managedIOSStoreApp](/graph/api/resources/intune-apps-managediosstoreapp?view=graph-rest-1.0)<br/>[managedMobileApp](/graph/api/resources/intune-mam-managedmobileapp?view=graph-rest-1.0)<br/>[managedMobileLobApp](/graph/api/resources/intune-apps-managedmobilelobapp?view=graph-rest-1.0)<br/>[mdmWindowsInformationProtectionPolicy](/graph/api/resources/intune-mam?view=graph-rest-1.0mwindowsinformationprotectionpolicy)<br/>[microsoftStoreForBusinessApp](/graph/api/resources/intune-apps-microsoftstoreforbusinessapp?view=graph-rest-1.0)<br/>[mobileApp](/graph/api/resources/intune-apps-mobileapp?view=graph-rest-1.0)<br/>[mobileAppAssignment](/graph/api/resources/intune-apps-mobileappassignment?view=graph-rest-1.0)<br/>[mobileAppCategory](/graph/api/resources/intune-apps-mobileappcategory?view=graph-rest-1.0)<br/>[mobileAppContent](/graph/api/resources/intune-apps-mobileappcontent?view=graph-rest-1.0)<br/>[mobileAppContentFile](/graph/api/resources/intune-apps-mobileappcontentfile?view=graph-rest-1.0)<br/>[mobileLobApp](/graph/api/resources/intune-apps-mobilelobapp?view=graph-rest-1.0)<br/>[mobileThreatDefenseConnector](/graph/api/resources/intune-onboarding-mobilethreatdefenseconnector?view=graph-rest-1.0)<br/>[notificationMessageTemplate](/graph/api/resources/intune-notification-notificationmessagetemplate?view=graph-rest-1.0)<br/>[onPremisesConditionalAccessSettings](/graph/api/resources/intune-onboarding-onpremisesconditionalaccesssettings?view=graph-rest-1.0)<br/>[remoteAssistancePartner](/graph/api/resources/intune-remoteassistance-remoteassistancepartner?view=graph-rest-1.0)<br/>[resourceOperation](/graph/api/resources/intune-rbac-resourceoperation?view=graph-rest-1.0)<br/>[roleAssignment](/graph/api/resources/intune-rbac-roleassignment?view=graph-rest-1.0)<br/>[roleDefinition](/graph/api/resources/intune-rbac-roledefinition?view=graph-rest-1.0)<br/>[settingStateDeviceSummary](/graph/api/resources/intune-deviceconfig-settingstatedevicesummary?view=graph-rest-1.0)<br/>[sharedPCConfiguration](/graph/api/resources/intune-deviceconfig-sharedpcconfiguration?view=graph-rest-1.0)<br/>[softwareUpdateStatusSummary](/graph/api/resources/intune-deviceconfig-softwareupdatestatussummary?view=graph-rest-1.0)<br/>[targetedManagedAppConfiguration](/graph/api/resources/intune-mam-targetedmanagedappconfiguration?view=graph-rest-1.0)<br/>targetedManagedAppPolicyAssignment<br/>[targetedManagedAppProtection](/graph/api/resources/intune-mam-targetedmanagedappprotection?view=graph-rest-1.0)<br/>[telecomExpenseManagementPartner](/graph/api/resources/intune-tem-telecomexpensemanagementpartner?view=graph-rest-1.0)<br/>[termsAndConditions](/graph/api/resources/intune-companyterms-termsandconditions?view=graph-rest-1.0)<br/>[termsAndConditionsAcceptanceStatus](/graph/api/resources/intune-companyterms-termsandconditionsacceptancestatus?view=graph-rest-1.0)<br/>[termsAndConditionsAssignment](/graph/api/resources/intune-companyterms-termsandconditionsassignment?view=graph-rest-1.0)<br/>[userInstallStateSummary](/graph/api/resources/intune-books-userinstallstatesummary?view=graph-rest-1.0)<br/>[webApp](/graph/api/resources/intune-apps-webapp?view=graph-rest-1.0)<br/>[windows10CompliancePolicy](/graph/api/resources/intune-deviceconfig-windows10compliancepolicy?view=graph-rest-1.0)<br/>[windows10CustomConfiguration](/graph/api/resources/intune-deviceconfig-windows10customconfiguration?view=graph-rest-1.0)<br/>[windows10EndpointProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windows10endpointprotectionconfiguration?view=graph-rest-1.0)<br/>[windows10EnterpriseModernAppManagementConfiguration](/graph/api/resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration?view=graph-rest-1.0)<br/>[windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-1.0)<br/>[windows10MobileCompliancePolicy](/graph/api/resources/intune-deviceconfig-windows10mobilecompliancepolicy?view=graph-rest-1.0)<br/>[windows10SecureAssessmentConfiguration](/graph/api/resources/intune-deviceconfig-windows10secureassessmentconfiguration?view=graph-rest-1.0)<br/>[windows10TeamGeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10teamgeneralconfiguration?view=graph-rest-1.0)<br/>[windows81CompliancePolicy](/graph/api/resources/intune-deviceconfig-windows81compliancepolicy?view=graph-rest-1.0)<br/>[windows81GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows81generalconfiguration?view=graph-rest-1.0)<br/>[windowsDefenderAdvancedThreatProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration?view=graph-rest-1.0)<br/>[windowsInformationProtection](/graph/api/resources/intune-mam-windowsinformationprotection?view=graph-rest-1.0)<br/>[windowsInformationProtectionAppLearningSummary](/graph/api/resources/intune-wip-windowsinformationprotectionapplearningsummary?view=graph-rest-1.0)<br/>[windowsInformationProtectionAppLockerFile](/graph/api/resources/intune-mam-windowsinformationprotectionapplockerfile?view=graph-rest-1.0)<br/>[windowsInformationProtectionNetworkLearningSummary](/graph/api/resources/intune-wip-windowsinformationprotectionnetworklearningsummary?view=graph-rest-1.0)<br/>[windowsInformationProtectionPolicy](/graph/api/resources/intune-mam-windowsinformationprotectionpolicy?view=graph-rest-1.0)<br/>[windowsMobileMSI](/graph/api/resources/intune-apps-windowsmobilemsi?view=graph-rest-1.0)<br/>[windowsPhone81CompliancePolicy](/graph/api/resources/intune-deviceconfig-windowsphone81compliancepolicy?view=graph-rest-1.0)<br/>[windowsPhone81CustomConfiguration](/graph/api/resources/intune-deviceconfig-windowsphone81customconfiguration?view=graph-rest-1.0)<br/>[windowsPhone81GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windowsphone81generalconfiguration?view=graph-rest-1.0)<br/>[windowsUniversalAppX](/graph/api/resources/intune-apps-windowsuniversalappx?view=graph-rest-1.0)<br/>[windowsUpdateForBusinessConfiguration](/graph/api/resources/intune-deviceconfig-windowsupdateforbusinessconfiguration?view=graph-rest-1.0)<br/>|
|Ergänzungen|v1.0|Die folgenden komplexen Typen wurden hinzugefügt:<br/>[allDevicesAssignmentTarget](/graph/api/resources/intune-shared-alldevicesassignmenttarget?view=graph-rest-1.0)<br/>[allLicensedUsersAssignmentTarget](/graph/api/resources/intune-shared-alllicensedusersassignmenttarget?view=graph-rest-1.0)<br/>[androidMinimumOperatingSystem](/graph/api/resources/intune-apps-androidminimumoperatingsystem?view=graph-rest-1.0)<br/>[androidMobileAppIdentifier](/graph/api/resources/intune-mam-androidmobileappidentifier?view=graph-rest-1.0)<br/>[appListItem](/graph/api/resources/intune-deviceconfig-applistitem?view=graph-rest-1.0)<br/>[bitLockerRemovableDrivePolicy](/graph/api/resources/intune-deviceconfig-bitlockerremovabledrivepolicy?view=graph-rest-1.0)<br/>[configurationManagerClientEnabledFeatures](/graph/api/resources/intune-devices-configurationmanagerclientenabledfeatures?view=graph-rest-1.0)<br/>[defenderDetectedMalwareActions](/graph/api/resources/intune-deviceconfig-defenderdetectedmalwareactions?view=graph-rest-1.0)<br/>[deleteUserFromSharedAppleDeviceActionResult](/graph/api/resources/intune-devices-deleteuserfromsharedappledeviceactionresult?view=graph-rest-1.0)<br/>[deviceActionResult](/graph/api/resources/intune-devices-deviceactionresult?view=graph-rest-1.0)<br/>[deviceAndAppManagementAssignmentTarget](/graph/api/resources/intune-shared-deviceandappmanagementassignmenttarget?view=graph-rest-1.0)<br/>[deviceCompliancePolicySettingState](/graph/api/resources/intune-deviceconfig-devicecompliancepolicysettingstate?view=graph-rest-1.0)<br/>[deviceConfigurationSettingState](/graph/api/resources/intune-deviceconfig-deviceconfigurationsettingstate?view=graph-rest-1.0)<br/>[deviceEnrollmentPlatformRestriction](/graph/api/resources/intune-onboarding-deviceenrollmentplatformrestriction?view=graph-rest-1.0)<br/>[deviceExchangeAccessStateSummary](/graph/api/resources/intune-devices-deviceexchangeaccessstatesummary?view=graph-rest-1.0)<br/>[deviceGeoLocation](/graph/api/resources/intune-devices-devicegeolocation?view=graph-rest-1.0)<br/>[deviceHealthAttestationState](/graph/api/resources/intune-devices-devicehealthattestationstate?view=graph-rest-1.0)<br/>[deviceManagementSettings](/graph/api/resources/intune-deviceconfig-devicemanagementsettings?view=graph-rest-1.0)<br/>[deviceOperatingSystemSummary](/graph/api/resources/intune-devices-deviceoperatingsystemsummary?view=graph-rest-1.0)<br/>[edgeSearchEngine](/graph/api/resources/intune-deviceconfig-edgesearchengine?view=graph-rest-1.0)<br/>[edgeSearchEngineBase](/graph/api/resources/intune-deviceconfig-edgesearchenginebase?view=graph-rest-1.0)<br/>[edgeSearchEngineCustom](/graph/api/resources/intune-deviceconfig-edgesearchenginecustom?view=graph-rest-1.0)<br/>[exclusionGroupAssignmentTarget](/graph/api/resources/intune-shared-exclusiongroupassignmenttarget?view=graph-rest-1.0)<br/>[fileEncryptionInfo](/graph/api/resources/intune-apps-fileencryptioninfo?view=graph-rest-1.0)<br/>[groupAssignmentTarget](/graph/api/resources/intune-shared-groupassignmenttarget?view=graph-rest-1.0)<br/>[intuneBrand](/graph/api/resources/intune-onboarding-intunebrand?view=graph-rest-1.0)<br/>[iosDeviceType](/graph/api/resources/intune-apps-iosdevicetype?view=graph-rest-1.0)<br/>[iosHomeScreenApp](/graph/api/resources/intune-deviceconfig-ioshomescreenapp?view=graph-rest-1.0)<br/>[iosHomeScreenFolder](/graph/api/resources/intune-deviceconfig-ioshomescreenfolder?view=graph-rest-1.0)<br/>[iosHomeScreenFolderPage](/graph/api/resources/intune-deviceconfig-ioshomescreenfolderpage?view=graph-rest-1.0)<br/>[iosHomeScreenItem](/graph/api/resources/intune-deviceconfig-ioshomescreenitem?view=graph-rest-1.0)<br/>[iosHomeScreenPage](/graph/api/resources/intune-deviceconfig-ioshomescreenpage?view=graph-rest-1.0)<br/>[iosLobAppAssignmentSettings](/graph/api/resources/intune-apps-ioslobappassignmentsettings?view=graph-rest-1.0)<br/>[iosMinimumOperatingSystem](/graph/api/resources/intune-apps-iosminimumoperatingsystem?view=graph-rest-1.0)<br/>[iosMobileAppIdentifier](/graph/api/resources/intune-mam-iosmobileappidentifier?view=graph-rest-1.0)<br/>[iosNetworkUsageRule](/graph/api/resources/intune-deviceconfig-iosnetworkusagerule?view=graph-rest-1.0)<br/>[iosNotificationSettings](/graph/api/resources/intune-deviceconfig-iosnotificationsettings?view=graph-rest-1.0)<br/>[iosStoreAppAssignmentSettings](/graph/api/resources/intune-apps-iosstoreappassignmentsettings?view=graph-rest-1.0)<br/>[iosVppAppAssignmentSettings](/graph/api/resources/intune-apps-iosvppappassignmentsettings?view=graph-rest-1.0)<br/>[ipRange](/graph/api/resources/intune-mam-iprange?view=graph-rest-1.0)<br/>[iPv4Range](/graph/api/resources/intune-mam-ipv4range?view=graph-rest-1.0)<br/>[iPv6Range](/graph/api/resources/intune-mam-ipv6range?view=graph-rest-1.0)<br/>[keyValuePair](/graph/api/resources/intune-androidforwork-keyvaluepair?view=graph-rest-1.0)<br/>[locateDeviceActionResult](/graph/api/resources/intune-devices-locatedeviceactionresult?view=graph-rest-1.0)<br/>[managedAppDiagnosticStatus](/graph/api/resources/intune-mam-managedappdiagnosticstatus?view=graph-rest-1.0)<br/>[managedAppPolicyDeploymentSummaryPerApp](/graph/api/resources/intune-mam-managedapppolicydeploymentsummaryperapp?view=graph-rest-1.0)<br/>[mediaContentRatingAustralia](/graph/api/resources/intune-deviceconfig-mediacontentratingaustralia?view=graph-rest-1.0)<br/>[mediaContentRatingCanada](/graph/api/resources/intune-deviceconfig-mediacontentratingcanada?view=graph-rest-1.0)<br/>[mediaContentRatingFrance](/graph/api/resources/intune-deviceconfig-mediacontentratingfrance?view=graph-rest-1.0)<br/>[mediaContentRatingGermany](/graph/api/resources/intune-deviceconfig-mediacontentratinggermany?view=graph-rest-1.0)<br/>[mediaContentRatingIreland](/graph/api/resources/intune-deviceconfig-mediacontentratingireland?view=graph-rest-1.0)<br/>[mediaContentRatingJapan](/graph/api/resources/intune-deviceconfig-mediacontentratingjapan?view=graph-rest-1.0)<br/>[mediaContentRatingNewZealand](/graph/api/resources/intune-deviceconfig-mediacontentratingnewzealand?view=graph-rest-1.0)<br/>[mediaContentRatingUnitedKingdom](/graph/api/resources/intune-deviceconfig-mediacontentratingunitedkingdom?view=graph-rest-1.0)<br/>[mediaContentRatingUnitedStates](/graph/api/resources/intune-deviceconfig-mediacontentratingunitedstates?view=graph-rest-1.0)<br/>[microsoftStoreForBusinessAppAssignmentSettings](/graph/api/resources/intune-apps-microsoftstoreforbusinessappassignmentsettings?view=graph-rest-1.0)<br/>[mimeContent](/graph/api/resources/intune-shared-mimecontent?view=graph-rest-1.0)<br/>[mobileAppAssignmentSettings](/graph/api/resources/intune-apps-mobileappassignmentsettings?view=graph-rest-1.0)<br/>[mobileAppIdentifier](/graph/api/resources/intune-mam-mobileappidentifier?view=graph-rest-1.0)<br/>[omaSetting](/graph/api/resources/intune-deviceconfig-omasetting?view=graph-rest-1.0)<br/>[omaSettingBase64](/graph/api/resources/intune-deviceconfig-omasettingbase64?view=graph-rest-1.0)<br/>[omaSettingBoolean](/graph/api/resources/intune-deviceconfig-omasettingboolean?view=graph-rest-1.0)<br/>[omaSettingDateTime](/graph/api/resources/intune-deviceconfig-omasettingdatetime?view=graph-rest-1.0)<br/>[omaSettingFloatingPoint](/graph/api/resources/intune-deviceconfig-omasettingfloatingpoint?view=graph-rest-1.0)<br/>[omaSettingInteger](/graph/api/resources/intune-deviceconfig-omasettinginteger?view=graph-rest-1.0)<br/>[omaSettingString](/graph/api/resources/intune-deviceconfig-omasettingstring?view=graph-rest-1.0)<br/>[omaSettingStringXml](/graph/api/resources/intune-deviceconfig-omasettingstringxml?view=graph-rest-1.0)<br/>[proxiedDomain](/graph/api/resources/intune-mam-proxieddomain?view=graph-rest-1.0)<br/>[remoteLockActionResult](/graph/api/resources/intune-devices-remotelockactionresult?view=graph-rest-1.0)<br/>[resetPasscodeActionResult](/graph/api/resources/intune-devices-resetpasscodeactionresult?view=graph-rest-1.0)<br/>[resourceAction](/graph/api/resources/intune-rbac-resourceaction?view=graph-rest-1.0)<br/>[rgbColor](/graph/api/resources/intune-onboarding-rgbcolor?view=graph-rest-1.0)<br/>[rolePermission](/graph/api/resources/intune-rbac-rolepermission?view=graph-rest-1.0)<br/>[settingSource](/graph/api/resources/intune-deviceconfig-settingsource?view=graph-rest-1.0)<br/>[sharedPCAccountManagerPolicy](/graph/api/resources/intune-deviceconfig-sharedpcaccountmanagerpolicy?view=graph-rest-1.0)<br/>[updateWindowsDeviceAccountActionParameter](/graph/api/resources/intune-devices-updatewindowsdeviceaccountactionparameter?view=graph-rest-1.0)<br/>[vppLicensingType](/graph/api/resources/intune-apps-vpplicensingtype?view=graph-rest-1.0)<br/>[windows10NetworkProxyServer](/graph/api/resources/intune-deviceconfig-windows10networkproxyserver?view=graph-rest-1.0)<br/>[windowsDefenderScanActionResult](/graph/api/resources/intune-devices-windowsdefenderscanactionresult?view=graph-rest-1.0)<br/>[windowsDeviceAccount](/graph/api/resources/intune-devices-windowsdeviceaccount?view=graph-rest-1.0)<br/>[windowsDeviceADAccount](/graph/api/resources/intune-devices-windowsdeviceadaccount?view=graph-rest-1.0)<br/>[windowsDeviceAzureADAccount](/graph/api/resources/intune-devices-windowsdeviceazureadaccount?view=graph-rest-1.0)<br/>[windowsFirewallNetworkProfile](/graph/api/resources/intune-deviceconfig-windowsfirewallnetworkprofile?view=graph-rest-1.0)<br/>[windowsInformationProtectionApp](/graph/api/resources/intune-mam-windowsinformationprotectionapp?view=graph-rest-1.0)<br/>[windowsInformationProtectionDataRecoveryCertificate](/graph/api/resources/intune-mam-windowsinformationprotectiondatarecoverycertificate?view=graph-rest-1.0)<br/>[windowsInformationProtectionDesktopApp](/graph/api/resources/intune-mam-windowsinformationprotectiondesktopapp?view=graph-rest-1.0)<br/>[windowsInformationProtectionIPRangeCollection](/graph/api/resources/intune-mam-windowsinformationprotectioniprangecollection?view=graph-rest-1.0)<br/>[windowsInformationProtectionProxiedDomainCollection](/graph/api/resources/intune-mam-windowsinformationprotectionproxieddomaincollection?view=graph-rest-1.0)<br/>[windowsInformationProtectionResourceCollection](/graph/api/resources/intune-mam-windowsinformationprotectionresourcecollection?view=graph-rest-1.0)<br/>[windowsInformationProtectionStoreApp](/graph/api/resources/intune-mam-windowsinformationprotectionstoreapp?view=graph-rest-1.0)<br/>[windowsMinimumOperatingSystem](/graph/api/resources/intune-apps-windowsminimumoperatingsystem?view=graph-rest-1.0)<br/>[windowsUpdateActiveHoursInstall](/graph/api/resources/intune-deviceconfig-windowsupdateactivehoursinstall?view=graph-rest-1.0)<br/>[windowsUpdateInstallScheduleType](/graph/api/resources/intune-deviceconfig-windowsupdateinstallscheduletype?view=graph-rest-1.0)<br/>[windowsUpdateScheduledInstall](/graph/api/resources/intune-deviceconfig-windowsupdatescheduledinstall?view=graph-rest-1.0)<br/>|
|Ergänzungen|v1.0|Die [assign](/graph/api/intune-apps-mobileapp-assign?view=graph-rest-1.0)-Aktion wurde zu [mobileApp](/graph/api/resources/intune-apps-mobileapp?view=graph-rest-1.0) hinzugefügt. |
|Ergänzungen|v1.0|Die [commit](/graph/api/intune-apps-mobileappcontentfile-commit?view=graph-rest-1.0)-Aktion wurde zu [MobileAppContentFile](/graph/api/resources/intune-apps-mobileappcontentfile?view=graph-rest-1.0) hinzugefügt. |
|Ergänzungen|v1.0|Die [renewUpload](/graph/api/intune-apps-mobileappcontentfile-renewupload?view=graph-rest-1.0)-Aktion wurde zu [mobileAppContentFile](/graph/api/resources/intune-apps-mobileappcontentfile?view=graph-rest-1.0) hinzugefügt. |
|Ergänzungen|v1.0|Die [retire](/graph/api/intune-devices-manageddevice-retire?view=graph-rest-1.0)-Aktion wurde zu [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0) hinzugefügt. |
|Ergänzungen|v1.0|Die [wipe](/graph/api/intune-devices-manageddevice-wipe?view=graph-rest-1.0)-Aktion wurde zu [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0) hinzugefügt. |
|Ergänzungen|v1.0|Die [resetPasscode](/graph/api/intune-devices-manageddevice-resetpasscode?view=graph-rest-1.0)-Aktion wurde zu [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0) hinzugefügt. |
|Ergänzungen|v1.0|Die [remoteLock](/graph/api/intune-devices-manageddevice-remotelock?view=graph-rest-1.0)-Aktion wurde zu [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0) hinzugefügt. |
|Ergänzungen|v1.0|Die [requestRemoteAssistance](/graph/api/intune-devices-manageddevice-requestremoteassistance?view=graph-rest-1.0)-Aktion wurde zu [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0) hinzugefügt. |
|Ergänzungen|v1.0|Die [disableLostMode](/graph/api/intune-devices-manageddevice-disablelostmode?view=graph-rest-1.0)-Aktion wurde zu [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0) hinzugefügt. |
|Ergänzungen|v1.0|Die [locateDevice](/graph/api/intune-devices-manageddevice-locatedevice?view=graph-rest-1.0)-Aktion wurde zu [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0) hinzugefügt. |
|Ergänzungen|v1.0|Die [bypassActivationLock](/graph/api/intune-devices-manageddevice-bypassactivationlock?view=graph-rest-1.0)-Aktion wurde zu [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0) hinzugefügt. |
|Ergänzungen|v1.0|Die [rebootNow](/graph/api/intune-devices-manageddevice-rebootnow?view=graph-rest-1.0)-Aktion wurde zu [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0) hinzugefügt. |
|Ergänzungen|v1.0|Die [shutDown](/graph/api/intune-devices-manageddevice-shutdown?view=graph-rest-1.0)-Aktion wurde zu [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0) hinzugefügt. |
|Ergänzungen|v1.0|Die [recoverPasscode](/graph/api/intune-devices-manageddevice-recoverpasscode?view=graph-rest-1.0)-Aktion wurde zu [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0) hinzugefügt. |
|Ergänzungen|v1.0|Die [cleanWindowsDevice](/graph/api/intune-devices-manageddevice-cleanwindowsdevice?view=graph-rest-1.0)-Aktion wurde zu [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0) hinzugefügt. |
|Ergänzungen|v1.0|Die [logoutSharedAppleDeviceActiveUser](/graph/api/intune-devices-manageddevice-logoutsharedappledeviceactiveuser?view=graph-rest-1.0)-Aktion wurde zu [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0) hinzugefügt. |
|Ergänzungen|v1.0|Die [deleteUserFromSharedAppleDevice](/graph/api/intune-devices-manageddevice-deleteuserfromsharedappledevice?view=graph-rest-1.0)-Aktion wurde zu [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0) hinzugefügt. |
|Ergänzungen|v1.0|Die [syncDevice](/graph/api/intune-devices-manageddevice-syncdevice?view=graph-rest-1.0)-Aktion wurde zu [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0) hinzugefügt. |
|Ergänzungen|v1.0|Die [windowsDefenderScan](/graph/api/intune-devices-manageddevice-windowsdefenderscan?view=graph-rest-1.0)-Aktion wurde zu [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0) hinzugefügt. |
|Ergänzungen|v1.0|Die [windowsDefenderUpdateSignatures](/graph/api/intune-devices-manageddevice-windowsdefenderupdatesignatures?view=graph-rest-1.0)-Aktion wurde zu [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0) hinzugefügt. |
|Ergänzungen|v1.0|Die [updateWindowsDeviceAccount](/graph/api/intune-devices-manageddevice-updatewindowsdeviceaccount?view=graph-rest-1.0)-Aktion wurde zu [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0) hinzugefügt. |
|Ergänzungen|v1.0|Die [removeAllDevicesFromManagement](/graph/api/intune-devices-user-removealldevicesfrommanagement?view=graph-rest-1.0)-Aktion wurde zu [user](/graph/api/resources/intune-shared-user?view=graph-rest-1.0) hinzugefügt. |
|Ergänzungen|v1.0|Die [assign](/graph/api/intune-deviceconfig-deviceconfiguration-assign?view=graph-rest-1.0)-Aktion wurde zu [deviceConfiguration](/graph/api/resources/intune-deviceconfig-deviceconfiguration?view=graph-rest-1.0) hinzugefügt. |
|Ergänzungen|v1.0|Die [assign](/graph/api/intune-deviceconfig-devicecompliancepolicy-assign?view=graph-rest-1.0)-Aktion wurde [deviceCompliancePolicy](/graph/api/resources/intune-deviceconfig-devicecompliancepolicy?view=graph-rest-1.0) hinzugefügt. |
|Ergänzungen|v1.0|Die [scheduleActionsForRules](/graph/api/intune-deviceconfig-devicecompliancepolicy-scheduleactionsforrules?view=graph-rest-1.0)-Aktion wurde zu [deviceCompliancePolicy](/graph/api/resources/intune-deviceconfig-devicecompliancepolicy?view=graph-rest-1.0) hinzugefügt. |
|Ergänzungen|v1.0|Die [setMobileDeviceManagementAuthority](/graph/api/intune-onboarding-organization-setmobiledevicemanagementauthority?view=graph-rest-1.0)-Aktion wurde zu [organization](/graph/api/resources/intune-onboarding-organization?view=graph-rest-1.0) hinzugefügt. |
|Ergänzungen|v1.0|Die [syncMicrosoftStoreForBusinessApps](/graph/api/intune-onboarding-deviceappmanagement-syncmicrosoftstoreforbusinessapps?view=graph-rest-1.0)-Aktion wurde zu [deviceAppManagement](/graph/api/resources/intune-shared-deviceappmanagement?view=graph-rest-1.0) hinzugefügt. |
|Ergänzungen|v1.0|Die [sync](/graph/api/intune-onboarding-devicemanagementexchangeconnector-sync?view=graph-rest-1.0)-Aktion wurde zu [deviceManagementExchangeConnector](/graph/api/resources/intune-onboarding-devicemanagementexchangeconnector?view=graph-rest-1.0) hinzugefügt. |
|Ergänzungen|v1.0|Die [setPriority](/graph/api/intune-onboarding-deviceenrollmentconfiguration-setpriority?view=graph-rest-1.0)-Aktion wurde zu [deviceEnrollmentConfiguration](/graph/api/resources/intune-onboarding-deviceenrollmentconfiguration?view=graph-rest-1.0) hinzugefügt. |
|Ergänzungen|v1.0|Die [assign](/graph/api/intune-onboarding-deviceenrollmentconfiguration-assign?view=graph-rest-1.0)-Aktion wurde [deviceEnrollmentConfiguration](/graph/api/resources/intune-onboarding-deviceenrollmentconfiguration?view=graph-rest-1.0) hinzugefügt. |
|Ergänzungen|v1.0|Die [assign](/graph/api/intune-mam-targetedmanagedappprotection-assign?view=graph-rest-1.0)-Aktion wurde für [targetedManagedAppProtection](/graph/api/resources/intune-mam-targetedmanagedappprotection?view=graph-rest-1.0) hinzugefügt. |
|Ergänzungen|v1.0|Die [assign](/graph/api/intune-mam-targetedmanagedappconfiguration-assign?view=graph-rest-1.0)-Aktion wurde für [targetedManagedAppConfiguration](/graph/api/resources/intune-mam-targetedmanagedappconfiguration?view=graph-rest-1.0) hinzugefügt. |
|Ergänzungen|v1.0|Die  [assign](/graph/api/intune-mam-windowsinformationprotection-assign?view=graph-rest-1.0)-Aktion wurde für [windowsInformationProtection](/graph/api/resources/intune-mam-windowsinformationprotection?view=graph-rest-1.0) hinzugefügt. |
|Ergänzungen|v1.0|Die [targetApps](/graph/api/intune-mam-managedapppolicy-targetapps?view=graph-rest-1.0)-Aktion wurde zu [managedAppPolicy](/graph/api/resources/intune-mam-managedapppolicy?view=graph-rest-1.0) hinzugefügt. |
|Ergänzungen|v1.0|Die [targetApps](/graph/api/intune-mam-managedappprotection-targetapps?view=graph-rest-1.0)-Aktion wurde zu [managedAppProtection](/graph/api/resources/intune-mam-managedappprotection?view=graph-rest-1.0) hinzugefügt. |
|Ergänzungen|v1.0|Die [targetApps](/graph/api/intune-mam-targetedmanagedappconfiguration-targetapps?view=graph-rest-1.0)-Aktion wurde zu [targetedManagedAppConfiguration](/graph/api/resources/intune-mam-targetedmanagedappconfiguration?view=graph-rest-1.0) hinzugefügt. |
|Ergänzungen|v1.0|Die [wipeManagedAppRegistrationsByDeviceTag](/graph/api/intune-mam-user-wipemanagedappregistrationsbydevicetag?view=graph-rest-1.0)-Aktion wurde zu [user](/graph/api/resources/intune-shared-user?view=graph-rest-1.0) hinzugefügt. |
|Ergänzungen|v1.0|Die [sendTestMessage](/graph/api/intune-notification-notificationmessagetemplate-sendtestmessage?view=graph-rest-1.0)-Aktion wurde auf [notificationMessageTemplate](/graph/api/resources/intune-notification-notificationmessagetemplate?view=graph-rest-1.0) hinzugefügt. |
|Ergänzungen|v1.0|Die [assign](/graph/api/intune-books-managedebook-assign?view=graph-rest-1.0)-Aktion wurde zu [managedEBook](/graph/api/resources/intune-books-managedebook?view=graph-rest-1.0) hinzugefügt. |
|Ergänzungen|v1.0|Die Aktion [beginOnboarding](/graph/api/intune-remoteassistance-remoteassistancepartner-beginonboarding?view=graph-rest-1.0) wurde zu [remoteAssistancePartner](/graph/api/resources/intune-remoteassistance-remoteassistancepartner?view=graph-rest-1.0) hinzugefügt. |
|Ergänzungen|v1.0|Die Aktion [disconnect](/graph/api/intune-remoteassistance-remoteassistancepartner-disconnect?view=graph-rest-1.0) wurde zu [remoteAssistancePartner](/graph/api/resources/intune-remoteassistance-remoteassistancepartner?view=graph-rest-1.0) hinzugefügt. |
|Ergänzungen|v1.0|Die [downloadApplePushNotificationCertificateSigningRequest](/graph/api/intune-devices-applepushnotificationcertificate-downloadapplepushnotificationcertificatesigningrequest?view=graph-rest-1.0)-Funktion wurde zu [applePushNotificationCertificate](/graph/api/resources/intune-devices-applepushnotificationcertificate?view=graph-rest-1.0) hinzugefügt. |
|Ergänzungen|v1.0|Die [deviceConfigurationUserActivity](/graph/api/intune-deviceconfig-reportroot-deviceconfigurationuseractivity?view=graph-rest-1.0)-Funktion wurde zu [reportRoot](/graph/api/resources/intune-deviceconfig-reportroot?view=graph-rest-1.0) hinzugefügt. |
|Ergänzungen|v1.0|Die [deviceConfigurationDeviceActivity](/graph/api/intune-deviceconfig-reportroot-deviceconfigurationdeviceactivity?view=graph-rest-1.0)-Funktion wurde zu [reportRoot](/graph/api/resources/intune-deviceconfig-reportroot?view=graph-rest-1.0) hinzugefügt. |
|Ergänzungen|v1.0|Die [verifyWindowsEnrollmentAutoDiscovery](/graph/api/intune-onboarding-devicemanagement-verifywindowsenrollmentautodiscovery?view=graph-rest-1.0)-Funktion wurde zu [deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-1.0) hinzugefügt. |
|Ergänzungen|v1.0|Die Funktion **getUserIdsWithFlaggedAppRegistration** wurde zu der [managedAppRegistration](/graph/api/resources/intune-mam-managedappregistration?view=graph-rest-1.0)-Sammlung hinzugefügt. |
|Ergänzungen|v1.0|Die [getManagedAppDiagnosticStatuses](/graph/api/intune-mam-user-getmanagedappdiagnosticstatuses?view=graph-rest-1.0)-Funktion wurde zu [user](/graph/api/resources/intune-shared-user?view=graph-rest-1.0) hinzugefügt. |
|Ergänzungen|v1.0|Die [getManagedAppPolicies](/graph/api/intune-mam-user-getmanagedapppolicies?view=graph-rest-1.0)-Funktion wurde zu [user](/graph/api/resources/intune-shared-user?view=graph-rest-1.0) hinzugefügt. |
|Ergänzungen|v1.0|Die [getEffectivePermissions](/graph/api/intune-rbac-devicemanagement-geteffectivepermissions?view=graph-rest-1.0)-Funktion wurde zu [deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-1.0) hinzugefügt. |
|Änderung|v1.0|Die **mobileDeviceManagementAuthority**-Eigenschaft wurde der [organization](/graph/api/resources/intune-onboarding-organization?view=graph-rest-1.0)-Entität hinzugefügt.|
|Änderung|v1.0|Die **deviceEnrollmentLimit**-Eigenschaft wurde der [user](/graph/api/resources/intune-shared-user?view=graph-rest-1.0)-Entität hinzugefügt.|
|Änderung|v1.0|Die Navigationseigenschaften  **managedDevices**, **managedAppRegistrations** und **deviceManagementTroubleshootingEvents** wurden der [user](/graph/api/resources/intune-shared-user?view=graph-rest-1.0)-Entität hinzugefügt.|
|||
|Ergänzungen|Beta|Hinzugefügte neue Entitäten:<br/>[deviceManagementScriptAssignment](/graph/api/resources/intune-devices-devicemanagementscriptassignment?view=graph-rest-beta)<br/>[iosCertificateProfile](/graph/api/resources/intune-deviceconfig-ioscertificateprofile?view=graph-rest-beta)<br/>[windowsInformationProtectionNetworkLearningSummary](/graph/api/resources/intune-wip-windowsinformationprotectionnetworklearningsummary?view=graph-rest-beta)<br/>|
|Ergänzungen|Beta|Die folgenden komplexen Typen wurden hinzugefügt:<br/>[revokeAppleVppLicensesActionResult](/graph/api/resources/intune-devices-revokeapplevpplicensesactionresult?view=graph-rest-beta)<br/>[vppTokenRevokeLicensesActionResult](/graph/api/resources/intune-onboarding-vpptokenrevokelicensesactionresult?view=graph-rest-beta)<br/>|
|Ergänzungen|Beta|Die [revokeTokens](/graph/api/intune-androidforwork-androidforworkenrollmentprofile-revoketoken?view=graph-rest-beta)-Aktion wurde zu [androidForWorkEnrollmentProfile](/graph/api/resources/intune-androidforwork-androidforworkenrollmentprofile?view=graph-rest-beta) hinzugefügt. |
|Ergänzungen|Beta|Die [assign](/graph/api/intune-apps-mobileapp-assign?view=graph-rest-beta)-Aktion wurde zu [mobileApp](/graph/api/resources/intune-apps-mobileapp?view=graph-rest-beta) hinzugefügt. |
|Ergänzungen|Beta|Die [assign](/graph/api/intune-devices-devicemanagementscript-assign?view=graph-rest-beta)-Aktion wurde zu [deviceManagementScript](/graph/api/resources/intune-devices-devicemanagementscript?view=graph-rest-beta) hinzugefügt. |
|Ergänzungen|Beta|Die [RevokeAppleVppLicenses](/graph/api/intune-devices-manageddevice-revokeapplevpplicenses?view=graph-rest-beta)-Aktion wurde zu [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) hinzugefügt. |
|Ergänzungen|Beta|Die [assign](/graph/api/intune-deviceconfig-devicecompliancepolicy-assign?view=graph-rest-beta)-Aktion wurde [deviceCompliancePolicy](/graph/api/resources/intune-deviceconfig-devicecompliancepolicy?view=graph-rest-beta) hinzugefügt. |
|Ergänzungen|Beta|Die [revokeLicenses](/graph/api/intune-onboarding-vpptoken-revokelicenses?view=graph-rest-beta)-Aktion wurde zu [vppToken](/graph/api/resources/intune-onboarding-vpptoken?view=graph-rest-beta) hinzugefügt. |
|Ergänzungen|Beta|Die [wipeManagedAppRegistrationsByDeviceTag](/graph/api/intune-mam-user-wipemanagedappregistrationsbydevicetag?view=graph-rest-beta)-Aktion wurde zu [user](/graph/api/resources/intune-devices-user?view=graph-rest-beta) hinzugefügt. |
|Ergänzungen|Beta|Die Aktion [assign](/graph/api/intune-books-managedebook-assign?view=graph-rest-beta) wurde zu [managedEBook](/graph/api/resources/intune-books-managedebook?view=graph-rest-beta) hinzugefügt |
|Ergänzungen|Beta|Die [getEffectiveDeviceEnrollmentConfigurations](/graph/api/intune-onboarding-user-geteffectivedeviceenrollmentconfigurations?view=graph-rest-beta)-Funktion wurde zu [user](/graph/api/resources/intune-devices-user?view=graph-rest-beta) hinzugefügt. |
|Löschung|Beta|Die folgenden Entitäten wurden entfernt:<br/>**appReportingOverviewStatus**<br/>**complianceSettingStateSummary**<br/>**deviceConfigurationUserStateSummary**<br/>**eBookGroupAssignment**<br/>**eBookVppGroupAssignment**<br/>**mobileAppGroupAssignment**<br/>**mobileAppVppGroupAssignment**<br/>|
|Löschung|Beta|Die folgenden komplexen Typen wurden entfernt:<br/>**androidForWorkAppConfigurationExample**<br/>**androidForWorkAppConfigurationExampleJson**<br/>**appInstallationFailure**<br/>**appsComplianceListItem**<br/>**defaultDeviceEnrollmentRestrictions**<br/>**defaultDeviceEnrollmentWindowsHelloForBusinessSettings**<br/>**deviceEnrollmentPlatformRestrictions**<br/>|
|Änderung|Beta|Die Eigenschaften **securityRequireVerifyApps**, **securityRequireSafetyNetAttestationBasicIntegrity**, **securityRequireSafetyNetAttestationCertifiedDevice**, **securityRequireGooglePlayServices**, **securityRequireUpToDateSecurityProviders** und **securityRequireCompanyPortalAppIntegrity** wurden der [androidCompliancePolicy](/graph/api/resources/intune-deviceconfig-androidcompliancepolicy?view=graph-rest-beta)-Entität hinzugefügt.|
|Änderung|Beta|Die **packageId**-Eigenschaft wurde der [androidForWorkApp](/graph/api/resources/intune-apps-androidforworkapp?view=graph-rest-beta)-Entität hinzugefügt.|
|Änderung|Beta|Der Typ der folgenden Eigenschaften in der [androidForWorkAppConfigurationSchema](/graph/api/resources/intune-androidforwork-androidforworkappconfigurationschema?view=graph-rest-beta)-Entität wurde geändert:<br/>**exampleJson** von [androidForWorkAppConfigurationExample](/graph/api/resources/intune-androidforwork-androidforworkappconfigurationexample?view=graph-rest-beta) in Binär<br/>|
|Änderung|Beta|Die Eigenschaften **securityRequireVerifyApps**, **securityRequireSafetyNetAttestationBasicIntegrity**, **securityRequireSafetyNetAttestationCertifiedDevice**, **securityRequireGooglePlayServices**, **securityRequireUpToDateSecurityProviders** and **securityRequireCompanyPortalAppIntegrity** wurden der [androidCompliancePolicy](/graph/api/resources/intune-deviceconfig-androidforworkcompliancepolicy?view=graph-rest-beta)-Entität hinzugefügt.|
|Änderung|Beta|Die Eigenschaften **displayName**, **lastModifiedDateTime**, **enrolledDeviceCount**, **qrCodeContent** und **qrCodeImage** wurden der[androidForWorkEnrollmentProfile](/graph/api/resources/intune-androidforwork-androidforworkenrollmentprofile?view=graph-rest-beta)-Entität hinzugefügt.|
|Änderung|Beta|Die **IsTokenActive**-Eigenschaft wurde aus der [AndroidForWorkEnrollmentProfile](/graph/api/resources/intune-androidforwork-androidforworkenrollmentprofile?view=graph-rest-beta)-Entität entfernt.|
|Änderung|Beta|Die Eigenschaften **innerAuthenticationProtocolForEapTtls**, **innerAuthenticationProtocolForPeap** und **outerIdentityPrivacyTemporaryValue** wurden zur Entität [androidForWorkEnterpriseWiFiConfiguration](/graph/api/resources/intune-deviceconfig-androidforworkenterprisewificonfiguration?view=graph-rest-beta) hinzugefügt.|
|Änderung|Beta|Die Eigenschaften **workProfileBlockCrossProfileCopyPaste** und **securityRequireVerifyApps** wurden der [androidForWorkGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration?view=graph-rest-beta)-Entität hinzugefügt.|
|Änderung|Beta|Die **securityRequireVerifyApps**-Eigenschaft wurde der [androidGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidgeneraldeviceconfiguration?view=graph-rest-beta)-Entität hinzugefügt.|
|Änderung|Beta|Die Eigenschaften **packageId** und **identityVersion** wurden der [AndroidLobApp](/graph/api/resources/intune-apps-androidlobapp?view=graph-rest-beta)-Entität hinzugefügt.|
|Änderung|Beta|Die **packageId**-Eigenschaft wurde der [androidStoreApp](/graph/api/resources/intune-apps-androidstoreapp?view=graph-rest-beta)-Entität hinzugefügt.|
|Änderung|Beta|Die **faceIdBlocked**-Eigenschaft wurde zur [defaultManagedAppProtection](/graph/api/resources/intune-mam-defaultmanagedappprotection?view=graph-rest-beta)-Entität hinzugefügt.|
|Änderung|Beta|Die **members**-Eigenschaft wurde der [deviceAndAppManagementRoleAssignment](/graph/api/resources/intune-rbac-deviceandappmanagementroleassignment?view=graph-rest-beta)-Entität hinzugefügt.|
|Änderung|Beta|Die **macOSRestriction**-Eigenschaft wurde der [deviceEnrollmentPlatformRestrictionsConfiguration](/graph/api/resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration?view=graph-rest-beta)-Entität hinzugefügt.|
|Änderung|Beta|Die Eigenschaften **whenPartnerDevicesWillBeRemovedDateTime** and **whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime** wurden der [deviceManagementPartner](/graph/api/resources/intune-onboarding-devicemanagementpartner?view=graph-rest-beta)-Entität hinzugefügt.|
|Änderung|Beta|Der Typ der folgenden Eigenschaften wurde in der [deviceManagementScript](/graph/api/resources/intune-devices-devicemanagementscript?view=graph-rest-beta)-Entität geändert:<br/>**scriptContent** von Zeichenfolge in Binär.<br/>|
|Änderung|Beta|Die **smimeEnablePerMessageSwitch**-Eigenschaft wurde der [iosEasEmailProfileConfiguration](/graph/api/resources/intune-deviceconfig-ioseasemailprofileconfiguration?view=graph-rest-beta)-Entität hinzugefügt.|
|Änderung|Beta|Die **identityVersion**-Eigenschaft wurde der [iosLobApp](/graph/api/resources/intune-apps-ioslobapp?view=graph-rest-beta)-Entität hinzugefügt.|
|Änderung|Beta|Die **faceIdBlocked**-Eigenschaft wurde zur [iosManagedAppProtection](/graph/api/resources/intune-mam-iosmanagedappprotection?view=graph-rest-beta)-Entität hinzugefügt.|
|Änderung|Beta|Die Eigenschaften **packageId** und **identityVersion** wurden der [managedAndroidLobApp](/graph/api/resources/intune-apps-managedandroidlobapp?view=graph-rest-beta)-Entität hinzugefügt.|
|Änderung|Beta|Die Eigenschaften **azureADDeviceId** und **remoteAssistanceSessionErrorDetails** wurden der [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta)-Entität hinzugefügt.|
|Änderung|Beta|Die **legacyAppConfiguration**-Eigenschaft wurde aus der [managedDeviceMobileAppConfiguration](/graph/api/resources/intune-apps-manageddevicemobileappconfiguration?view=graph-rest-beta)-Entität entfernt.|
|Änderung|Beta|Die **identityVersion**-Eigenschaft wurde der [managedIOSLobApp](/graph/api/resources/intune-apps-managedioslobapp?view=graph-rest-beta)-Entität hinzugefügt.|
|Änderung|Beta|Die **identityVersion**-Eigenschaft wurde aus der [managedIOSLobApp](/graph/api/resources/intune-apps-managedmobilelobapp?view=graph-rest-beta)-Entität entfernt.|
|Änderung|Beta|Die **publishingState**-Eigenschaft wurde der [mobileApp](/graph/api/resources/intune-apps-mobileapp?view=graph-rest-beta)-Entität hinzugefügt.|
|Änderung|Beta|Die  **installState**-Eigenschaft wurde zur [mobileAppInstallStatus](/graph/api/resources/intune-apps-mobileappinstallstatus?view=graph-rest-beta)-Entität hinzugefügt.|
|Änderung|Beta|Die **identityVersion**-Eigenschaft wurde aus der [mobileLobApp](/graph/api/resources/intune-apps-mobilelobapp?view=graph-rest-beta)-Entität entfernt.|
|Änderung|Beta|Die **allowPartnerToCollectIOSApplicationMetadata**-Eigenschaft wurde der [mobileThreatDefenseConnector](/graph/api/resources/intune-onboarding-mobilethreatdefenseconnector?view=graph-rest-beta)-Entität hinzugefügt.|
|Änderung|Beta|Die **members**-Eigenschaft wurde aus der [roleAssignment](/graph/api/resources/intune-rbac-roleassignment?view=graph-rest-beta)-Entität entfernt.|
|Änderung|Beta|Die **lastModifiedDateTime**-Eigenschaft wurde der [termsAndConditions](/graph/api/resources/intune-companyterms-termsandconditions?view=graph-rest-beta)-Entität hinzugefügt.|
|Änderung|Beta|Die Eigenschaften **deviceThreatProtectionEnabled** und **deviceThreatProtectionRequiredSecurityLevel** wurden der [windows10CompliancePolicy](/graph/api/resources/intune-deviceconfig-windows10compliancepolicy?view=graph-rest-beta)-Entität hinzugefügt.|
|Änderung|Beta|Die Eigenschaft **minimumUpdateAutoInstallClassification** wurde aus der Entität [windows10CompliancePolicy](/graph/api/resources/intune-deviceconfig-windows10compliancepolicy?view=graph-rest-beta) entfernt.|
|Änderung|Beta|Die Eigenschaften **privacyBlockPublishUserActivities** und **privacyBlockActivityFeed** wurden der [windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta)-Entität hinzugefügt.|
|Änderung|Beta|Die **configurationAccountType**-Eigenschaft wurde der [windows10SecureAssessmentConfiguration](/graph/api/resources/intune-deviceconfig-windows10secureassessmentconfiguration?view=graph-rest-beta)-Entität hinzugefügt.|
|Änderung|Beta|Die **trustedNetworkDomains**Eigenschaft wurde aus der Entität [windows10VpnConfiguration](/graph/api/resources/intune-deviceconfig-windows10vpnconfiguration?view=graph-rest-beta) entfernt.|
|Änderung|Beta|Die **minimumUpdateAutoInstallClassification**Eigenschaft wurde aus der Entität [windows81CompliancePolicy](/graph/api/resources/intune-deviceconfig-windows81compliancepolicy?view=graph-rest-beta) entfernt.|
|Änderung|Beta|Die **identityVersion**-Eigenschaft wurde der [windowsAppX](/graph/api/resources/intune-apps-windowsappx?view=graph-rest-beta)-Entität hinzugefügt.|
|Änderung|Beta|Die **daysWithoutContactBeforeUnenroll**-Eigenschaft wurde der [windowsInformationProtectionPolicy](/graph/api/resources/intune-mam-windowsinformationprotectionpolicy?view=graph-rest-beta)-Entität hinzugefügt.|
|Änderung|Beta|Die **identityVersion**-Eigenschaft wurde der [windowsMobileMSI](/graph/api/resources/intune-apps-windowsmobilemsi?view=graph-rest-beta)-Entität hinzugefügt.|
|Änderung|Beta|Die **identityVersion**-Eigenschaft wurde der [windowsPhone81AppX](/graph/api/resources/intune-apps-windowsphone81appx?view=graph-rest-beta)-Entität hinzugefügt.|
|Änderung|Beta|Die **identityVersion**-Eigenschaft wurde der [windowsPhoneXAP](/graph/api/resources/intune-apps-windowsphonexap?view=graph-rest-beta)-Entität hinzugefügt.|
|Änderung|Beta|Die **identityVersion**-Eigenschaft wurde der  [windowsUniversalAppX](/graph/api/resources/intune-apps-windowsuniversalappx?view=graph-rest-beta)-Entität hinzugefügt.|
|Änderung|Beta|Die **domainJoinConfiguration**-Navigationseigenschaft wurde der [activeDirectoryWindowsAutopilotDeploymentProfile](/graph/api/resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile?view=graph-rest-beta)-Entität hinzugefügt.|
|Änderung|Beta|Die **notificationMessageTemplate**-Navigationseigenschaft wurde aus der [deviceComplianceActionItem](/graph/api/resources/intune-deviceconfig-devicecomplianceactionitem?view=graph-rest-beta)-Entität entfernt.|
|Änderung|Beta|Die **groupAssignments**-Navigationseigenschaft wurde aus der [deviceCompliancePolicy](/graph/api/resources/intune-deviceconfig-devicecompliancepolicy?view=graph-rest-beta) -Entität entfernt.|
|Änderung|Beta|Die **windowsInformationProtectionNetworkLearningSummaries**-Navigationseigenschaft wurde der [DeviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-beta)-Entität hinzugefügt.|
|Änderung|Beta|Die **deviceConfigurationUserStateSummaries**-Navigationseigenschaft wurde aus der [deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-beta)-Entität entfernt.|
|Änderung|Beta|Der Typ der folgenden Eigenschaften wurde in der [deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-beta)-Entität geändert:<br/>**roleAssignments** aus der [roleAssignment](/graph/api/resources/intune-rbac-roleassignment?view=graph-rest-beta)-Sammlung in die [deviceAndAppManagementRoleAssignment](/graph/api/resources/intune-rbac-deviceandappmanagementroleassignment?view=graph-rest-beta)-Sammlung<br/>|
|Änderung|Beta|Die **assignments**-Navigationseigenschaft wurde zur [deviceManagementScript](/graph/api/resources/intune-devices-devicemanagementscript?view=graph-rest-beta)-Entität hinzugefügt.|
|Änderung|Beta|Die **smimeEnablePerMessageSwitch**-Navigationseigenschaft wurde der [iosEasEmailProfileConfiguration](/graph/api/resources/intune-deviceconfig-ioseasemailprofileconfiguration?view=graph-rest-beta)-Entität hinzugefügt.|
|Änderung|Beta|Der Typ der folgenden Eigenschaften in der [iosEasEmailProfileConfiguration](/graph/api/resources/intune-deviceconfig-ioseasemailprofileconfiguration?view=graph-rest-beta)-Entität wurde geändert:<br/>**smimeSigningCertificate** von [iosCertificateProfileBase](/graph/api/resources/intune-deviceconfig-ioscertificateprofilebase?view=graph-rest-beta) in [iosCertificateProfile](/graph/api/resources/intune-deviceconfig-ioscertificateprofile?view=graph-rest-beta)<br/>|
|Änderung|Beta|Die **vppToken**-Navigationseigenschaft wurde aus der [iosVppApp](/graph/api/resources/intune-apps-iosvppapp?view=graph-rest-beta)-Entität entfernt.|
|Änderung|Beta|Die **groupAssignments**-Navigationseigenschaft wurde aus der [managedEBook](/graph/api/resources/intune-books-managedebook?view=graph-rest-beta)-Entität entfernt.|
|Änderung|Beta|Die **groupAssignments**-Navigationseigenschaft wurde aus der  [mobileApp](/graph/api/resources/intune-apps-mobileapp?view=graph-rest-beta)-Entität entfernt.|
|Änderung|Beta|Die Navigationseigenschaften **depOnboardingSettings** und **appleVolumePurchaseProgramTokens** wurden aus der [organization](/graph/api/resources/intune-onboarding-organization?view=graph-rest-beta)-Entität entfernt.|
|Änderung|Beta|Die **deviceEnrollmentConfigurations**-Navigationseigenschaft wurde der [user](/graph/api/resources/intune-devices-user?view=graph-rest-beta)-Entität hinzugefügt.|
|Änderung|Beta|Die Eigenschaften **windowsCommercialId** und **windowsCommercialIdLastModifiedTime** wurden aus dem komplexen Typ [deviceManagementSettings](/graph/api/resources/intune-deviceconfig-devicemanagementsettings?view=graph-rest-beta) entfernt.|
|Änderung|Beta|Die **showDisplayNameNextToLogo**-Eigenschaft wurde dem komplexen Typ [intuneBrand](/graph/api/resources/intune-onboarding-intunebrand?view=graph-rest-beta) hinzugefügt.|
|Änderung|Beta|Die **deviceUsageType**-Eigenschaft wurde dem komplexen Typ [outOfBoxExperienceSettings](/graph/api/resources/intune-enrollment-outofboxexperiencesettings?view=graph-rest-beta) hinzugefügt.|
|Änderung|Beta|Die Eigenschaften **supportsUserLicensing** und **supportsDeviceLicensing** wurden dem komplexen Typ [vppLicensingType](/graph/api/resources/intune-apps-vpplicensingtype?view=graph-rest-beta) hinzugefügt.|
|Änderung|Beta|Die **actionMessage**-Eigenschaft wurde aus dem komplexen Typ [vppTokenActionResult](/graph/api/resources/intune-onboarding-vpptokenactionresult?view=graph-rest-beta) entfernt.|

### <a name="reports-apis"></a>Bericht-APIs
| Änderungstyp | Version | Beschreibung                              |
|:------------|:--------|:-----------------------------------------|
| Ergänzungen    | v1.0    | Die folgenden APIs wurden hinzugefügt:<br>[getTeamsUserActivityUserDetail](/graph/api/reportroot-getteamsuseractivityuserdetail?view=graph-rest-1.0)<br>[getTeamsUserActivityCounts](/graph/api/reportroot-getteamsuseractivitycounts?view=graph-rest-1.0)<br>[getTeamsUserActivityUserCounts](/graph/api/reportroot-getteamsuseractivityusercounts?view=graph-rest-1.0)<br>[getTeamsDeviceUsageUserDetail](/graph/api/reportroot-getteamsdeviceusageuserdetail?view=graph-rest-1.0)<br>[getTeamsDeviceUsageUserCounts](/graph/api/reportroot-getteamsdeviceusageusercounts?view=graph-rest-1.0)<br>[getTeamsDeviceUsageDistributionUserCounts](/graph/api/reportroot-getteamsdeviceusagedistributionusercounts?view=graph-rest-1.0) |

## <a name="december-2017"></a>Dezember 2017

### <a name="delta-query"></a>Delta-Abfrage

| Änderungstyp | Version | Beschreibung                              |
|:------------|:--------|:-----------------------------------------|
| Änderung      | v1.0    | Hinzufügen einer optionalen Abfrage-Filterfunktion zu [Benutzer](/graph/api/user-delta?view=graph-rest-1.0) und [Gruppen](/graph/api/group-delta?view=graph-rest-1.0). |

### <a name="microsoft-intune-apis"></a>Microsoft Intune-APIs

|Änderungstyp|Version|Beschreibung|
|:---|:---|:---|
|Ergänzungen|Beta|Hinzugefügte neue Entitäten:<br/>[androidForWorkEnrollmentProfile](/graph/api/resources/intune-androidforwork-androidforworkenrollmentprofile?view=graph-rest-beta)<br/>[deviceAndAppManagementRoleAssignment](/graph/api/resources/intune-rbac-deviceandappmanagementroleassignment?view=graph-rest-beta)<br/>[deviceAndAppManagementRoleDefinition](/graph/api/resources/intune-rbac-deviceandappmanagementroledefinition?view=graph-rest-beta)<br/>[macOSLobApp](/graph/api/resources/intune-apps-macoslobapp?view=graph-rest-beta)<br/>|
|Ergänzungen|Beta|Hinzugefügte neue komplexe Typen:<br/>[resourceAction](/graph/api/resources/intune-rbac-resourceaction?view=graph-rest-beta)<br/>[updateWindowsDeviceAccountActionParameter](/graph/api/resources/intune-devices-updatewindowsdeviceaccountactionparameter?view=graph-rest-beta)<br/>[vppTokenActionResult](/graph/api/resources/intune-onboarding-vpptokenactionresult?view=graph-rest-beta)<br/>[windowsDeviceAADAccount](/graph/api/resources/intune-devices-windowsdeviceaadaccount?view=graph-rest-beta)<br/>[windowsDeviceAccount](/graph/api/resources/intune-devices-windowsdeviceaccount?view=graph-rest-beta)<br/>[windowsDeviceADAccount](/graph/api/resources/intune-devices-windowsdeviceadaccount?view=graph-rest-beta)<br/>|
|Ergänzungen|Beta|Die [revokeTokens](/graph/api/intune-androidforwork-androidforworkenrollmentprofile-revoketokens?view=graph-rest-beta)-Aktion wurde zu [AndroidForWorkEnrollmentProfile](/graph/api/resources/intune-androidforwork-androidforworkenrollmentprofile?view=graph-rest-beta) hinzugefügt. |
|Ergänzungen|Beta|Die [createToken](/graph/api/intune-androidforwork-androidforworkenrollmentprofile-createtoken?view=graph-rest-beta)-Aktion wurde zu [AndroidForWorkEnrollmentProfile](/graph/api/resources/intune-androidforwork-androidforworkenrollmentprofile?view=graph-rest-beta) hinzugefügt. |
|Ergänzungen|Beta|Die Aktion [wipe](/graph/api/intune-devices-manageddevice-wipe?view=graph-rest-beta) wurde zu [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) hinzugefügt. |
|Ergänzungen|Beta|Die [UpdateWindowsDeviceAccount](/graph/api/intune-devices-manageddevice-updatewindowsdeviceaccount?view=graph-rest-beta)-Aktion wurde zu [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) hinzugefügt. |
|Ergänzungen|Beta|Die [revokeLicenses](/graph/api/intune-onboarding-vpptoken-revokelicenses?view=graph-rest-beta)-Aktion wurde zu [vppToken](/graph/api/resources/intune-onboarding-vpptoken?view=graph-rest-beta) hinzugefügt. |
|Ergänzungen|Beta|Die [getDevicePasscode](/graph/api/intune-deviceconfig-devicecompliancepolicy-getdevicepasscode?view=graph-rest-beta)-Funktion wurde zur [deviceCompliancePolicy](/graph/api/resources/intune-deviceconfig-devicecompliancepolicy?view=graph-rest-beta)- Sammlung hinzugefügt. |
|Ergänzungen|Beta|Die [getEffectivePermissions](/graph/api/intune-rbac-devicemanagement-geteffectivepermissions?view=graph-rest-beta)-Funktion wurde zu [deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-beta) hinzugefügt. |
|Löschung|Beta|Die folgenden Entitäten wurden entfernt:<br/>**windowsStoreForBusinessApp**<br/>|
|Löschung|Beta|Die folgenden komplexen Typen wurden entfernt:<br/>**windowsStoreForBusinessAppAssignmentSettings**<br/>|
|Änderung|Beta|Die **dateAndTimeBlockChanges**-Eigenschaft wurde der  [androidGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidgeneraldeviceconfiguration?view=graph-rest-beta)-Entität hinzugefügt.|
|Änderung|Beta|Die Eigenschaft **enableAuthenticationViaCompanyPortal** wurde aus der Entität [depEnrollmentProfile](/graph/api/resources/intune-corpenrollment-depenrollmentprofile?view=graph-rest-beta) entfernt.|
|Änderung|Beta|Die Eigenschaften **windowsStoreForBusinessLastSuccessfulSyncDateTime**, **isEnabledForWindowsStoreForBusiness**, **windowsStoreForBusinessLanguage** und **windowsStoreForBusinessLastCompletedApplicationSyncTime** wurden aus der Entität [DeviceAppManagement](/graph/api/resources/intune-apps-deviceappmanagement?view=graph-rest-beta) entfernt.|
|Änderung|Beta|Die Eigenschaften **maximumDepTokens** und **intuneAccountId** wurden zur Entität [DeviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-beta) hinzugefügt.|
|Änderung|Beta|Die Eigenschaft **enableAuthenticationViaCompanyPortal** wurde zur Entität [depEnrollmentProfile](/graph/api/resources/intune-corpenrollment-enrollmentprofile?view=graph-rest-beta) hinzugefügt.|
|Änderung|Beta|Die Eigenschaften **managedDeviceName** und **partnerReportedThreatState** wurden zur Entität [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) hinzugefügt.|
|Änderung|Beta|Die Eigenschaft **installProgressDisplayLevel** wurde zur Entität [officeSuiteApp](/graph/api/resources/intune-apps-officesuiteapp?view=graph-rest-beta) hinzugefügt.|
|Änderung|Beta|Die Eigenschaft **resourceScopes** wurde zur Entität [roleAssignment](/graph/api/resources/intune-rbac-roleassignment?view=graph-rest-beta) hinzugefügt.|
|Änderung|Beta|die Eigenschaften **rolePermissions** und **isBuiltIn** wurden zur Entität [roleDefinition](/graph/api/resources/intune-rbac-roledefinition?view=graph-rest-beta) hinzugefügt.|
|Änderung|Beta|Die Eigenschaft **tokenActionResults** wurde zur Entität [vppToken](/graph/api/resources/intune-onboarding-vpptoken?view=graph-rest-beta) hinzugefügt.|
|Änderung|Beta|Die Eigenschaft **minimumUpdateAutoInstallClassification** wurde zur Entität [windows10CompliancePolicy](/graph/api/resources/intune-deviceconfig-windows10compliancepolicy?view=graph-rest-beta) hinzugefügt.|
|Änderung|Beta|Die Eigenschaften **defenderSecurityCenterDisableAppBrowserUI**, **defenderSecurityCenterDisableFamilyUI**, **defenderSecurityCenterDisableHealthUI**, **defenderSecurityCenterDisableNetworkUI**, **defenderSecurityCenterDisableVirusUI**, **defenderSecurityCenterOrganizationDisplayName**, **defenderSecurityCenterHelpEmail**, **defenderSecurityCenterHelpPhone**, **defenderSecurityCenterHelpURL**, **defenderSecurityCenterNotificationsFromApp**, **defenderSecurityCenterITContactDisplay** und **applicationGuardAllowVirtualGPU** wurden zur Entität [windows10EndpointProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windows10endpointprotectionconfiguration?view=graph-rest-beta) hinzugefügt.|
|Änderung|Beta|Die Eigenschaften **enableAutomaticRedeployment** und **authenticationAllowFIDODevice** wurden zur Entität [windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta) hinzugefügt.|
|Änderung|Beta|Die Eigenschaft **trustedNetworkDomains** wurde zur Entität [windows10VpnConfiguration](/graph/api/resources/intune-deviceconfig-windows10vpnconfiguration?view=graph-rest-beta) hinzugefügt.|
|Änderung|Beta|Die Eigenschaft **minimumUpdateAutoInstallClassification** wurde zur Entität [windows81CompliancePolicy](/graph/api/resources/intune-deviceconfig-windows81compliancepolicy?view=graph-rest-beta) hinzugefügt.|
|Änderung|Beta|Die Navigationseigenschaft **androidForWorkEnrollmentProfiles** wurde zur Entität [deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-beta) hinzugefügt.|
|Änderung|Beta|Die Eigenschaft **healthAttestationSupportedStatus** wurde zum komplexen Typ [deviceHealthAttestationState](/graph/api/resources/intune-devices-devicehealthattestationstate?view=graph-rest-beta) hinzugefügt.|
|Änderung|Beta|Die Eigenschaften **tpmSpecificationVersion**, **operatingSystemEdition**, **deviceFullQualifiedDomainName**, **deviceGuardVirtualizationBasedSecurityHardwareRequirementState**, **deviceGuardVirtualizationBasedSecurityState** und **deviceGuardLocalSystemAuthorityCredentialGuardState** wurden zum komplexen Typ [hardwareInformation](/graph/api/resources/intune-devices-hardwareinformation?view=graph-rest-beta) hinzugefügt.|
|Änderung|Beta|Die Eigenschaft **vpnConfigurationId** wurde zum komplexen Typ [iosVppAppAssignmentSettings](/graph/api/resources/intune-apps-iosvppappassignmentsettings?view=graph-rest-beta) hinzugefügt.|
|Änderung|Beta|Die Eigenschaft **resourceActions** wurde zum komplexen Typ [rolePermission](/graph/api/resources/intune-rbac-rolepermission?view=graph-rest-beta) hinzugefügt.|

### <a name="reports-apis"></a>Bericht-APIs
| Änderungstyp | Version | Beschreibung                              |
|:------------|:--------|:-----------------------------------------|
| Ergänzungen    | v1.0    | Die folgenden APIs wurden hinzugefügt:<br>[getEmailActivityUserDetail](/graph/api/reportroot-getemailactivityuserdetail?view=graph-rest-1.0)<br>[getEmailActivityCounts](/graph/api/reportroot-getemailactivitycounts?view=graph-rest-1.0)<br>[getEmailActivityUserCounts](/graph/api/reportroot-getemailactivityusercounts?view=graph-rest-1.0)<br>[getEmailAppUsageUserDetail](/graph/api/reportroot-getemailappusageuserdetail?view=graph-rest-1.0)<br>[getEmailAppUsageAppsUserCounts](/graph/api/reportroot-getemailappusageappsusercounts?view=graph-rest-1.0)<br>[getEmailAppUsageUserCounts](/graph/api/reportroot-getemailappusageusercounts?view=graph-rest-1.0)<br>[getEmailAppUsageVersionsUserCounts](/graph/api/reportroot-getemailappusageversionsusercounts?view=graph-rest-1.0)<br>[getMailboxUsageDetail](/graph/api/reportroot-getmailboxusagedetail?view=graph-rest-1.0)<br>[getMailboxUsageMailboxCounts](/graph/api/reportroot-getmailboxusagemailboxcounts?view=graph-rest-1.0)<br>[getMailboxUsageQuotaStatusMailboxCounts](/graph/api/reportroot-getmailboxusagequotastatusmailboxcounts?view=graph-rest-1.0)<br>[getMailboxUsageStorage](/graph/api/reportroot-getmailboxusagestorage?view=graph-rest-1.0)<br>[getOffice365ActivationsUserDetail](/graph/api/reportroot-getoffice365activationsuserdetail?view=graph-rest-1.0)<br>[getOffice365ActivationCounts](/graph/api/reportroot-getoffice365activationcounts?view=graph-rest-1.0)<br>[getOffice365ActivationsUserCounts](/graph/api/reportroot-getoffice365activationsusercounts?view=graph-rest-1.0)<br>[getOffice365ActiveUserDetail](/graph/api/reportroot-getoffice365activeuserdetail?view=graph-rest-1.0)<br>[getOffice365ActiveUserCounts](/graph/api/reportroot-getoffice365activeusercounts?view=graph-rest-1.0)<br>[getOffice365ServicesUserCounts](/graph/api/reportroot-getoffice365servicesusercounts?view=graph-rest-1.0)<br>[getOffice365GroupsActivityDetail](/graph/api/reportroot-getoffice365groupsactivitydetail?view=graph-rest-1.0)<br> [getOffice365GroupsActivityCounts](/graph/api/reportroot-getoffice365groupsactivitycounts?view=graph-rest-1.0)<br>[getOffice365GroupsActivityGroupCounts](/graph/api/reportroot-getoffice365groupsactivitygroupcounts?view=graph-rest-1.0)<br>[getOffice365GroupsActivityStorage](/graph/api/reportroot-getoffice365groupsactivitystorage?view=graph-rest-1.0)<br>[getOffice365GroupsActivityFileCounts](/graph/api/reportroot-getoffice365groupsactivityfilecounts?view=graph-rest-1.0)<br>[getOneDriveActivityUserDetail](/graph/api/reportroot-getonedriveactivityuserdetail?view=graph-rest-1.0)<br>[getOneDriveActivityUserCounts](/graph/api/reportroot-getonedriveactivityusercounts?view=graph-rest-1.0)<br>[getOneDriveActivityFileCounts](/graph/api/reportroot-getonedriveactivityfilecounts?view=graph-rest-1.0)<br>[getOneDriveUsageAccountDetail](/graph/api/reportroot-getonedriveusageaccountdetail?view=graph-rest-1.0)<br>[getOneDriveUsageAccountCounts](/graph/api/reportroot-getonedriveusageaccountcounts?view=graph-rest-1.0)<br>[getOneDriveUsageFileCounts](/graph/api/reportroot-getonedriveusagefilecounts?view=graph-rest-1.0)<br>[getOneDriveUsageStorage](/graph/api/reportroot-getonedriveusagestorage?view=graph-rest-1.0)<br>[getSharePointActivityUserDetail](/graph/api/reportroot-getsharepointactivityuserdetail?view=graph-rest-1.0)<br>[getSharePointActivityFileCounts](/graph/api/reportroot-getsharepointactivityfilecounts?view=graph-rest-1.0)<br>[getSharePointActivityUserCounts](/graph/api/reportroot-getsharepointactivityusercounts?view=graph-rest-1.0)<br>[getSharePointActivityPages](/graph/api/reportroot-getsharepointactivitypages?view=graph-rest-1.0)<br>[getSharePointSiteUsageDetail](/graph/api/reportroot-getsharepointsiteusagedetail?view=graph-rest-1.0)<br>[getSharePointSiteUsageFileCounts](/graph/api/reportroot-getsharepointsiteusagefilecounts?view=graph-rest-1.0)<br>[getSharePointSiteUsageSiteCounts](/graph/api/reportroot-getsharepointsiteusagesitecounts?view=graph-rest-1.0)<br>[getSharePointSiteUsageStorage](/graph/api/reportroot-getsharepointsiteusagestorage?view=graph-rest-1.0)<br>[getSharePointSiteUsagePages](/graph/api/reportroot-getsharepointsiteusagepages?view=graph-rest-1.0)<br>[getSkypeForBusinessActivityUserDetail](/graph/api/reportroot-getskypeforbusinessactivityuserdetail?view=graph-rest-1.0)<br>[getSkypeForBusinessActivityCounts](/graph/api/reportroot-getskypeforbusinessactivitycounts?view=graph-rest-1.0)<br>[getSkypeForBusinessActivityUserCounts](/graph/api/reportroot-getskypeforbusinessactivityusercounts?view=graph-rest-1.0)<br>[getSkypeForBusinessDeviceUsageUserDetail](/graph/api/reportroot-getskypeforbusinessdeviceusageuserdetail?view=graph-rest-1.0)<br>[getSkypeForBusinessDeviceUsageDistributionUserCounts](/graph/api/reportroot-getskypeforbusinessdeviceusagedistributionusercounts?view=graph-rest-1.0)<br>[getSkypeForBusinessDeviceUsageUserCounts](/graph/api/reportroot-getskypeforbusinessdeviceusageusercounts?view=graph-rest-1.0)<br>[getSkypeForBusinessOrganizerActivityCounts](/graph/api/reportroot-getskypeforbusinessorganizeractivitycounts?view=graph-rest-1.0)<br>[getSkypeForBusinessOrganizerActivityUserCounts](/graph/api/reportroot-getskypeforbusinessorganizeractivityusercounts?view=graph-rest-1.0)<br>[getSkypeForBusinessOrganizerActivityMinuteCounts](/graph/api/reportroot-getskypeforbusinessorganizeractivityminutecounts?view=graph-rest-1.0)<br>[getSkypeForBusinessParticipantActivityCounts](/graph/api/reportroot-getskypeforbusinessparticipantactivitycounts?view=graph-rest-1.0)<br>[getSkypeForBusinessParticipantActivityUserCounts](/graph/api/reportroot-getskypeforbusinessparticipantactivityusercounts?view=graph-rest-1.0)<br>[getSkypeForBusinessParticipantActivityMinuteCounts](/graph/api/reportroot-getskypeforbusinessparticipantactivityminutecounts?view=graph-rest-1.0)<br>[getSkypeForBusinessPeerToPeerActivityCounts](/graph/api/reportroot-getskypeforbusinesspeertopeeractivitycounts?view=graph-rest-1.0)<br>[getSkypeForBusinessPeerToPeerActivityUserCounts](/graph/api/reportroot-getskypeforbusinesspeertopeeractivityusercounts?view=graph-rest-1.0)<br>[getSkypeForBusinessPeerToPeerActivityMinuteCounts](/graph/api/reportroot-getskypeforbusinesspeertopeeractivityminutecounts?view=graph-rest-1.0)<br>[getYammerActivityUserDetail](/graph/api/reportroot-getyammeractivityuserdetail?view=graph-rest-1.0)<br>[getYammerActivityCounts](/graph/api/reportroot-getyammeractivitycounts?view=graph-rest-1.0)<br>[getYammerActivityUserCounts](/graph/api/reportroot-getyammeractivityusercounts?view=graph-rest-1.0)<br>[getYammerDeviceUsageUserDetail](/graph/api/reportroot-getyammerdeviceusageuserdetail?view=graph-rest-1.0)<br>[getYammerDeviceUsageDistributionUserCounts](/graph/api/reportroot-getyammerdeviceusagedistributionusercounts?view=graph-rest-1.0)<br>[getYammerDeviceUsageUserCounts](/graph/api/reportroot-getyammerdeviceusageusercounts?view=graph-rest-1.0)<br>[getYammerGroupsActivityDetail](/graph/api/reportroot-getyammergroupsactivitydetail?view=graph-rest-1.0)<br>[getYammerGroupsActivityGroupCounts](/graph/api/reportroot-getyammergroupsactivitygroupcounts?view=graph-rest-1.0)<br>[getYammerGroupsActivityCounts](/graph/api/reportroot-getyammergroupsactivitycounts?view=graph-rest-1.0).|
| Ergänzungen    | Beta    | Die folgenden APIs wurden hinzugefügt:<br>[getTeamsUserActivityUserDetail](/graph/api/reportroot-getteamsuseractivityuserdetail?view=graph-rest-beta)<br>[getTeamsUserActivityCounts](/graph/api/reportroot-getteamsuseractivitycounts?view=graph-rest-beta)<br>[getTeamsUserActivityUserCounts](/graph/api/reportroot-getteamsuseractivityusercounts?view=graph-rest-beta)<br>[getTeamsDeviceUsageUserDetail](/graph/api/reportroot-getteamsdeviceusageuserdetail?view=graph-rest-beta)<br>[getTeamsDeviceUsageUserCounts](/graph/api/reportroot-getteamsdeviceusageusercounts?view=graph-rest-beta)<br>[getTeamsDeviceUsageDistributionUserCounts](/graph/api/reportroot-getteamsdeviceusagedistributionusercounts?view=graph-rest-beta) |

## <a name="november-2017"></a>November 2017

### <a name="azure-ad-synchronization-apis"></a>APIs zur Azure AD-Synchronisierung

| Änderungstyp | Version | Beschreibung                              |
| :---------- | :------ | :--------------------------------------- |
| Ergänzungen    | Beta    | Es wurde Unterstützung für die Azure AD-Identitätssynchronisierung hinzugefügt, einschließlich der folgenden Ressourcen:<br/>[Auftrag](/graph/api/resources/synchronization-synchronizationjob?view=graph-rest-beta)<br/>[Schema](/graph/api/resources/synchronization-synchronizationschema?view=graph-rest-beta)<br/>[Vorlage](/graph/api/resources/synchronization-synchronizationtemplate?view=graph-rest-beta)<br/>In den Themen zu den Ressourcen finden Sie ausführliche Informationen zu den verfügbaren Methoden.|

### <a name="education-apis"></a>Bildungs-APIs

|Änderungstyp|Version|Beschreibung|
|:---|:---|:---|
|Ergänzungen|Beta|Es wurde Unterstützung für Bildungs-APIs hinzugefügt, einschließlich der folgenden Ressourcen:<br/>[Bildungseinrichtungen](/graph/api/resources/educationschool?view=graph-rest-beta)<br/>[Kurse](/graph/api/resources/educationclass?view=graph-rest-beta)<br/>[Benutzer](/graph/api/resources/educationuser?view=graph-rest-beta)<br/>[Aufgaben](/graph/api/resources/educationassignment?view=graph-rest-beta)<br/>[Übermittlungen](/graph/api/resources/educationsubmission?view=graph-rest-beta)<br/>In den Themen zu den Ressourcen finden Sie ausführliche Informationen zu den verfügbaren Methoden.|

### <a name="microsoft-intune-apis"></a>Microsoft Intune-APIs
|Änderungstyp|Version|Beschreibung|
|:---|:---|:---|
|Ergänzungen|Beta|Hinzugefügte neue Entitäten:<br/>[auditEvent](/graph/api/resources/intune-auditing-auditevent?view=graph-rest-beta)<br/>[deviceManagementTroubleshootingEvent](/graph/api/resources/intune-troubleshooting-devicemanagementtroubleshootingevent?view=graph-rest-beta)<br/>[deviceSetupConfiguration](/graph/api/resources/intune-deviceconfig-devicesetupconfiguration?view=graph-rest-beta)<br/>[enrollmentTroubleshootingEvent](/graph/api/resources/intune-troubleshooting-enrollmenttroubleshootingevent?view=graph-rest-beta)<br/>[macOSOfficeSuiteApp](/graph/api/resources/intune-apps-macosofficesuiteapp?view=graph-rest-beta)<br/>[microsoftStoreForBusinessApp](/graph/api/resources/intune-apps-microsoftstoreforbusinessapp?view=graph-rest-beta)<br/>[ndesConnector](/graph/api/resources/intune-deviceconfig-ndesconnector?view=graph-rest-beta)<br/>|
|Ergänzungen|Beta|Hinzugefügte neue komplexe Typen:<br/>[auditActor](/graph/api/resources/intune-auditing-auditactor?view=graph-rest-beta)<br/>[auditProperty](/graph/api/resources/intune-auditing-auditproperty?view=graph-rest-beta)<br/>[auditResource](/graph/api/resources/intune-auditing-auditresource?view=graph-rest-beta)<br/>[bulkManagedDeviceActionResult](/graph/api/resources/intune-devices-bulkmanageddeviceactionresult?view=graph-rest-beta)<br/>[deviceProtectionOverview](/graph/api/resources/intune-devices-deviceprotectionoverview?view=graph-rest-beta)<br/>[microsoftStoreForBusinessAppAssignmentSettings](/graph/api/resources/intune-apps-microsoftstoreforbusinessappassignmentsettings?view=graph-rest-beta)<br/>[operatingSystemVersionRange](/graph/api/resources/intune-deviceconfig-operatingsystemversionrange?view=graph-rest-beta)<br/>[remoteLockActionResult](/graph/api/resources/intune-devices-remotelockactionresult?view=graph-rest-beta)<br/>|
|Ergänzungen|Beta|Die Aktion executeAction wurde zur Sammlung [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) hinzugefügt. |
|Ergänzungen|Beta|Die Aktion [wipe](/graph/api/intune-devices-manageddevice-wipe?view=graph-rest-beta) wurde zu [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) hinzugefügt. |
|Ergänzungen|Beta|Die Aktion [shutDown](/graph/api/intune-devices-manageddevice-shutdown?view=graph-rest-beta) wurde zu [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) hinzugefügt. |
|Ergänzungen|Beta|Die Aktion [assign](/graph/api/intune-deviceconfig-deviceconfiguration-assign?view=graph-rest-beta) wurde zu [deviceConfiguration](/graph/api/resources/intune-deviceconfig-deviceconfiguration?view=graph-rest-beta) hinzugefügt. |
|Ergänzungen|Beta|Die Aktion [syncMicrosoftStoreForBusinessApps](/graph/api/intune-onboarding-deviceappmanagement-syncmicrosoftstoreforbusinessapps?view=graph-rest-beta) wurde zu [deviceAppManagement](/graph/api/resources/intune-apps-deviceappmanagement?view=graph-rest-beta) hinzugefügt. |
|Ergänzungen|Beta|Die Aktion setDefaultProfile wurde zu [enrollmentProfile](/graph/api/resources/intune-corpenrollment-enrollmentprofile?view=graph-rest-beta) hinzugefügt. |
|Ergänzungen|Beta|Die Aktion shareForSchoolDataSyncService wurde zu [depOnboardingSetting](/graph/api/resources/intune-onboarding-deponboardingsetting?view=graph-rest-beta) hinzugefügt. |
|Ergänzungen|Beta|Die Aktion unshareForSchoolDataSyncService wurde zu [depOnboardingSetting](/graph/api/resources/intune-onboarding-deponboardingsetting?view=graph-rest-beta) hinzugefügt. |
|Ergänzungen|Beta|Die Funktion getAuditCategories wurde zur Sammlung [auditEvent](/graph/api/resources/intune-auditing-auditevent?view=graph-rest-beta) hinzugefügt. |
|Ergänzungen|Beta|Die Funktion getAuditActivityTypes wurde zur Sammlung [auditEvent](/graph/api/resources/intune-auditing-auditevent?view=graph-rest-beta) hinzugefügt. |
|Löschung|Beta|Die folgenden Entitäten wurden entfernt:<br/>**mobileAppIdentifierDeployment**<br/>|
|Löschung|Beta|Die folgenden komplexen Typen wurden entfernt:<br/>**windowsInformationProtectionCloudResource**<br/>**windowsInformationProtectionCloudResourceCollection**<br/>|
|Änderung|Beta|Die folgenden Eigenschaften der Entität [androidDeviceComplianceLocalActionLockDeviceWithPasscode](/graph/api/resources/intune-deviceconfig-androiddevicecompliancelocalactionlockdevicewithpasscode?view=graph-rest-beta) wurden geändert:<br/>**passcode** von Erforderlich zu Optional<br/>|
|Änderung|Beta|Die Eigenschaften **microsoftStoreForBusinessLastSuccessfulSyncDateTime**, **isEnabledForMicrosoftStoreForBusiness**, **microsoftStoreForBusinessLanguage** und **microsoftStoreForBusinessLastCompletedApplicationSyncTime** wurden zur Entität [deviceAppManagement](/graph/api/resources/intune-apps-deviceappmanagement?view=graph-rest-beta) hinzugefügt.|
|Änderung|Beta|Die Eigenschaft **target** wurde zur Entität [deviceConfigurationAssignment](/graph/api/resources/intune-deviceconfig-deviceconfigurationassignment?view=graph-rest-beta) hinzugefügt.|
|Änderung|Beta|Die Eigenschaft **deviceProtectionOverview** wurde zur Entität [deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-beta) hinzugefügt.|
|Änderung|Beta|Die Eigenschaften **exchangeAlias** und **exchangeOrganization** wurden zur Entität [deviceManagementExchangeConnector](/graph/api/resources/intune-onboarding-devicemanagementexchangeconnector?view=graph-rest-beta) hinzugefügt.|
|Änderung|Beta|Die Eigenschaften **appStoreUrl** und **minimumSupportedOperatingSystem** wurden zur Entität [managedAndroidStoreApp](/graph/api/resources/intune-apps-managedandroidstoreapp?view=graph-rest-beta) hinzugefügt.|
|Änderung|Beta|Die Eigenschaft **remoteAssistanceSessionErrorString** wurde zur Entität [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) hinzugefügt.|
|Änderung|Beta|Die Eigenschaften **appStoreUrl**, **applicableDeviceType** und **minimumSupportedOperatingSystem** wurden zur Entität [managedIOSStoreApp](/graph/api/resources/intune-apps-managediosstoreapp?view=graph-rest-beta) hinzugefügt.|
|Änderung|Beta|Die Eigenschaften **notApplicableDeviceCount**, **pendingInstallDeviceCount**, **notApplicableUserCount** und **pendingInstallUserCount** wurden zur Entität [mobileAppInstallSummary](/graph/api/resources/intune-apps-mobileappinstallsummary?view=graph-rest-beta) hinzugefügt.|
|Änderung|Beta|Die Eigenschaften **targetedSecurityGroupIds** und **targetedSecurityGroupsCount** wurden aus der Entität [targetedManagedAppConfiguration](/graph/api/resources/intune-mam-targetedmanagedappconfiguration?view=graph-rest-beta) entfernt.|
|Änderung|Beta|Die Eigenschaften **targetedSecurityGroupsCount** und **targetedSecurityGroupIds** wurden aus der Entität [targetedManagedAppProtection](/graph/api/resources/intune-mam-targetedmanagedappprotection?view=graph-rest-beta) entfernt.|
|Änderung|Beta|Die Eigenschaft **validOperatingSystemBuildRanges** wurde zur Entität [windows10CompliancePolicy](/graph/api/resources/intune-deviceconfig-windows10compliancepolicy?view=graph-rest-beta) hinzugefügt.|
|Änderung|Beta|Die Eigenschaften **activeFirewallRequired**, **uacRequired** und **validOperatingSystemBuildRanges** wurden zur Entität [windows10MobileCompliancePolicy](/graph/api/resources/intune-deviceconfig-windows10mobilecompliancepolicy?view=graph-rest-beta) hinzugefügt.|
|Änderung|Beta|Die Eigenschaft **enableExpeditedTelemetryReporting** wurde zur Entität [windowsDefenderAdvancedThreatProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration?view=graph-rest-beta) hinzugefügt.|
|Änderung|Beta|Die Eigenschaften **allowedApps**, **enterpriseCloudResources** und **targetedSecurityGroupIds** wurden aus der Entität [windowsInformationProtection](/graph/api/resources/intune-mam-windowsinformationprotection?view=graph-rest-beta) entfernt.|
|Änderung|Beta|Die Eigenschaft **ignoreVersionDetection** wurde zur Entität [windowsMobileMSI](/graph/api/resources/intune-apps-windowsmobilemsi?view=graph-rest-beta) hinzugefügt.|
|Änderung|Beta|Die Navigationseigenschaft **mobileAppIdentifierDeployments** wurde aus der Entität [androidManagedAppProtection](/graph/api/resources/intune-mam-androidmanagedappprotection?view=graph-rest-beta) entfernt.|
|Änderung|Beta|Die Navigationseigenschaft **mobileAppIdentifierDeployments** wurde aus der Entität [defaultManagedAppProtection](/graph/api/resources/intune-mam-defaultmanagedappprotection?view=graph-rest-beta) entfernt.|
|Änderung|Beta|Die Navigationseigenschaft **assignments** wurde zur Entität [deviceConfiguration](/graph/api/resources/intune-deviceconfig-deviceconfiguration?view=graph-rest-beta) hinzugefügt.|
|Änderung|Beta|Die Navigationseigenschaft **deviceConfiguration** wurde aus der Entität [deviceConfigurationAssignment](/graph/api/resources/intune-deviceconfig-deviceconfigurationassignment?view=graph-rest-beta) entfernt.|
|Änderung|Beta|Die Navigationseigenschaft **deviceConfiguration** wurde zur Entität [deviceConfigurationGroupAssignment](/graph/api/resources/intune-deviceconfig-deviceconfigurationgroupassignment?view=graph-rest-beta) hinzugefügt.|
|Änderung|Beta|Die Navigationseigenschaften **deviceSetupConfigurations**, **ndesConnectors**, **exchangeOnPremisesPolicies**, **conditionalAccessSettings**, **auditEvents** und **troubleshootingEvents** wurden zur Entität [deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-beta) hinzugefügt.|
|Änderung|Beta|Die Navigationseigenschaft **mobileAppIdentifierDeployments** wurde aus der Entität [iosManagedAppProtection](/graph/api/resources/intune-mam-iosmanagedappprotection?view=graph-rest-beta) entfernt.|
|Änderung|Beta|Die Navigationseigenschaft **windowsProtectionState** wurde der Entität [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) hinzugefügt.|
|Änderung|Beta|Die Navigationseigenschaften **mobileAppIdentifierDeployments** und **targetedSecurityGroups** wurden aus der Entität [targetedManagedAppConfiguration](/graph/api/resources/intune-mam-targetedmanagedappconfiguration?view=graph-rest-beta) entfernt.|
|Änderung|Beta|Die Navigationseigenschaft **targetedSecurityGroups** wurde aus der Entität [targetedManagedAppProtection](/graph/api/resources/intune-mam-targetedmanagedappprotection?view=graph-rest-beta) entfernt.|
|Änderung|Beta|Die Navigationseigenschaft **deviceManagementTroubleshootingEvents** wurde zur Entität [user](/graph/api/resources/intune-devices-user?view=graph-rest-beta) hinzugefügt.|
|Ändern|Beta|Die Navigationseigenschaft **allowedAppLockerFiles** wurde aus der Entität [windowsInformationProtection](/graph/api/resources/intune-mam-windowsinformationprotection?view=graph-rest-beta) entfernt.|
|Änderung|Beta|Die Navigationseigenschaft **windowsProtectionState** wurde aus der Entität [windowsManagedDevice](/graph/api/resources/intune-devices-windowsmanageddevice?view=graph-rest-beta) entfernt.|
|Änderung|Beta|Die Eigenschaft **v11_0** wurde zum komplexen Typ [iosMinimumOperatingSystem](/graph/api/resources/intune-apps-iosminimumoperatingsystem?view=graph-rest-beta) hinzugefügt.|
|Ändern|Beta|Die Eigenschaft **denied** wurde zum komplexen Typ [windowsInformationProtectionApp](/graph/api/resources/intune-mam-windowsinformationprotectionapp?view=graph-rest-beta) hinzugefügt.|

### <a name="reports-apis"></a>Bericht-APIs
| Änderungstyp | Version | Beschreibung                              |
| :---------- | :------ | :--------------------------------------- |
| Ergänzungen    | Beta    | Für die folgenden APIs wurde JSON-Unterstützung hinzugefügt:<br>[getEmailActivityUserDetail](/graph/api/reportroot-getemailactivityuserdetail?view=graph-rest-beta)<br>[getEmailActivityCounts](/graph/api/reportroot-getemailactivitycounts?view=graph-rest-beta)<br>[getEmailActivityUserCounts](/graph/api/reportroot-getemailactivityusercounts?view=graph-rest-beta)<br>[getEmailAppUsageUserDetail](/graph/api/reportroot-getemailappusageuserdetail?view=graph-rest-beta)<br>[getEmailAppUsageAppsUserCounts](/graph/api/reportroot-getemailappusageappsusercounts?view=graph-rest-beta)<br>[getEmailAppUsageUserCounts](/graph/api/reportroot-getemailappusageusercounts?view=graph-rest-beta)<br>[getEmailAppUsageVersionsUserCounts](/graph/api/reportroot-getemailappusageversionsusercounts?view=graph-rest-beta)<br>[getMailboxUsageDetail](/graph/api/reportroot-getmailboxusagedetail?view=graph-rest-beta)<br>[getMailboxUsageMailboxCounts](/graph/api/reportroot-getmailboxusagemailboxcounts?view=graph-rest-beta)<br>[getMailboxUsageQuotaStatusMailboxCounts](/graph/api/reportroot-getmailboxusagequotastatusmailboxcounts?view=graph-rest-beta)<br>[getMailboxUsageStorage](/graph/api/reportroot-getmailboxusagestorage?view=graph-rest-beta)<br>[getOffice365ActivationsUserDetail](/graph/api/reportroot-getoffice365activationsuserdetail?view=graph-rest-beta)<br>[getOffice365ActivationCounts](/graph/api/reportroot-getoffice365activationcounts?view=graph-rest-beta)<br>[getOffice365ActivationsUserCounts](/graph/api/reportroot-getoffice365activationsusercounts?view=graph-rest-beta)<br>[getOffice365ActiveUserDetail](/graph/api/reportroot-getoffice365activeuserdetail?view=graph-rest-beta)<br>[getOffice365ActiveUserCounts](/graph/api/reportroot-getoffice365activeusercounts?view=graph-rest-beta)<br>[getOffice365ServicesUserCounts](/graph/api/reportroot-getoffice365servicesusercounts?view=graph-rest-beta)<br>[getOffice365GroupsActivityDetail](/graph/api/reportroot-getoffice365groupsactivitydetail?view=graph-rest-beta)<br> [getOffice365GroupsActivityCounts](/graph/api/reportroot-getoffice365groupsactivitycounts?view=graph-rest-beta)<br>[getOffice365GroupsActivityGroupCounts](/graph/api/reportroot-getoffice365groupsactivitygroupcounts?view=graph-rest-beta)<br>[getOffice365GroupsActivityStorage](/graph/api/reportroot-getoffice365groupsactivitystorage?view=graph-rest-beta)<br>[getOffice365GroupsActivityFileCounts](/graph/api/reportroot-getoffice365groupsactivityfilecounts?view=graph-rest-beta)<br>[getOneDriveActivityUserDetail](/graph/api/reportroot-getonedriveactivityuserdetail?view=graph-rest-beta)<br>[getOneDriveActivityUserCounts](/graph/api/reportroot-getonedriveactivityusercounts?view=graph-rest-beta)<br>[getOneDriveActivityFileCounts](/graph/api/reportroot-getonedriveactivityfilecounts?view=graph-rest-beta)<br>[getOneDriveUsageAccountDetail](/graph/api/reportroot-getonedriveusageaccountdetail?view=graph-rest-beta)<br>[getOneDriveUsageAccountCounts](/graph/api/reportroot-getonedriveusageaccountcounts?view=graph-rest-beta)<br>[getOneDriveUsageFileCounts](/graph/api/reportroot-getonedriveusagefilecounts?view=graph-rest-beta)<br>[getOneDriveUsageStorage](/graph/api/reportroot-getonedriveusagestorage?view=graph-rest-beta)<br>[getSharePointActivityUserDetail](/graph/api/reportroot-getsharepointactivityuserdetail?view=graph-rest-beta)<br>[getSharePointActivityFileCounts](/graph/api/reportroot-getsharepointactivityfilecounts?view=graph-rest-beta)<br>[getSharePointActivityUserCounts](/graph/api/reportroot-getsharepointactivityusercounts?view=graph-rest-beta)<br>[getSharePointActivityPages](/graph/api/reportroot-getsharepointactivitypages?view=graph-rest-beta)<br>[getSharePointSiteUsageDetail](/graph/api/reportroot-getsharepointsiteusagedetail?view=graph-rest-beta)<br>[getSharePointSiteUsageFileCounts](/graph/api/reportroot-getsharepointsiteusagefilecounts?view=graph-rest-beta)<br>[getSharePointSiteUsageSiteCounts](/graph/api/reportroot-getsharepointsiteusagesitecounts?view=graph-rest-beta)<br>[getSharePointSiteUsageStorage](/graph/api/reportroot-getsharepointsiteusagestorage?view=graph-rest-beta)<br>[getSharePointSiteUsagePages](/graph/api/reportroot-getsharepointsiteusagepages?view=graph-rest-beta)<br>[getSkypeForBusinessActivityUserDetail](/graph/api/reportroot-getskypeforbusinessactivityuserdetail?view=graph-rest-beta)<br>[getSkypeForBusinessActivityCounts](/graph/api/reportroot-getskypeforbusinessactivitycounts?view=graph-rest-beta)<br>[getSkypeForBusinessActivityUserCounts](/graph/api/reportroot-getskypeforbusinessactivityusercounts?view=graph-rest-beta)<br>[getSkypeForBusinessDeviceUsageUserDetail](/graph/api/reportroot-getskypeforbusinessdeviceusageuserdetail?view=graph-rest-beta)<br>[getSkypeForBusinessDeviceUsageDistributionUserCounts](/graph/api/reportroot-getskypeforbusinessdeviceusagedistributionusercounts?view=graph-rest-beta)<br>[getSkypeForBusinessDeviceUsageUserCounts](/graph/api/reportroot-getskypeforbusinessdeviceusageusercounts?view=graph-rest-beta)<br>[getSkypeForBusinessOrganizerActivityCounts](/graph/api/reportroot-getskypeforbusinessorganizeractivitycounts?view=graph-rest-beta)<br>[getSkypeForBusinessOrganizerActivityUserCounts](/graph/api/reportroot-getskypeforbusinessorganizeractivityusercounts?view=graph-rest-beta)<br>[getSkypeForBusinessOrganizerActivityMinuteCounts](/graph/api/reportroot-getskypeforbusinessorganizeractivityminutecounts?view=graph-rest-beta)<br>[getSkypeForBusinessParticipantActivityCounts](/graph/api/reportroot-getskypeforbusinessparticipantactivitycounts?view=graph-rest-beta)<br>[getSkypeForBusinessParticipantActivityUserCounts](/graph/api/reportroot-getskypeforbusinessparticipantactivityusercounts?view=graph-rest-beta)<br>[getSkypeForBusinessParticipantActivityMinuteCounts](/graph/api/reportroot-getskypeforbusinessparticipantactivityminutecounts?view=graph-rest-beta)<br>[getSkypeForBusinessPeerToPeerActivityCounts](/graph/api/reportroot-getskypeforbusinesspeertopeeractivitycounts?view=graph-rest-beta)<br>[getSkypeForBusinessPeerToPeerActivityUserCounts](/graph/api/reportroot-getskypeforbusinesspeertopeeractivityusercounts?view=graph-rest-beta)<br>[getSkypeForBusinessPeerToPeerActivityMinuteCounts](/graph/api/reportroot-getskypeforbusinesspeertopeeractivityminutecounts?view=graph-rest-beta)<br>[getYammerActivityUserDetail](/graph/api/reportroot-getyammeractivityuserdetail?view=graph-rest-beta)<br>[getYammerActivityCounts](/graph/api/reportroot-getyammeractivitycounts?view=graph-rest-beta)<br>[getYammerActivityUserCounts](/graph/api/reportroot-getyammeractivityusercounts?view=graph-rest-beta)<br>[getYammerDeviceUsageUserDetail](/graph/api/reportroot-getyammerdeviceusageuserdetail?view=graph-rest-beta)<br>[getYammerDeviceUsageDistributionUserCounts](/graph/api/reportroot-getyammerdeviceusagedistributionusercounts?view=graph-rest-beta)<br>[getYammerDeviceUsageUserCounts](/graph/api/reportroot-getyammerdeviceusageusercounts?view=graph-rest-beta)<br>[getYammerGroupsActivityDetail](/graph/api/reportroot-getyammergroupsactivitydetail?view=graph-rest-beta)<br>[getYammerGroupsActivityGroupCounts](/graph/api/reportroot-getyammergroupsactivitygroupcounts?view=graph-rest-beta)<br>[getYammerGroupsActivityCounts](/graph/api/reportroot-getyammergroupsactivitycounts?view=graph-rest-beta). |

### <a name="webhooks"></a>Webhooks

| Änderungstyp | Version | Beschreibung                              |
|:------------|:--------|:-----------------------------------------|
| Änderungen | Beta und Version 1.0 | Reduced [webhooks](/graph/api/resources/webhooks?view=graph-rest-1.0) [maximum length of subscription expiration time](/graph/api/resources/subscription?view=graph-rest-1.0#maximum-length-of-subscription-per-resource-type) for drive root items. The new value is the supported maximum expiration time for drive root items. |

## <a name="october-2017"></a>Oktober 2017

### <a name="azure-ad-apis"></a>Azure AD-APIs

| Änderungstyp | Version | Beschreibung                              |
| :---------- | :------ | :--------------------------------------- |
|Ergänzungen|Beta|Die [identityProvider](/graph/api/resources/identityprovider?view=graph-rest-beta)-Entität und die Vorgänge [create](/graph/api/identityprovider-post-identityproviders?view=graph-rest-beta), [list](/graph/api/identityprovider-list?view=graph-rest-beta), [get](/graph/api/identityprovider-get?view=graph-rest-beta), [update](/graph/api/identityprovider-update?view=graph-rest-beta) und [delete](/graph/api/identityprovider-delete?view=graph-rest-beta) wurden hinzugefügt.|


### <a name="microsoft-intune-apis"></a>Microsoft Intune-APIs
|Änderungstyp|Version|Beschreibung|
|:---|:---|:---|
|Ergänzungen|Beta|Hinzugefügte neue Entitäten:<br/>[androidDeviceComplianceLocalActionLockDeviceWithPasscode](/graph/api/resources/intune-deviceconfig-androiddevicecompliancelocalactionlockdevicewithpasscode?view=graph-rest-beta)<br/>[iosLobAppProvisioningConfigurationAssignment](/graph/api/resources/intune-apps-ioslobappprovisioningconfigurationassignment?view=graph-rest-beta)<br/>[iosVppEBookAssignment](/graph/api/resources/intune-books-iosvppebookassignment?view=graph-rest-beta)<br/>[managedDeviceMobileAppConfigurationAssignment](/graph/api/resources/intune-apps-manageddevicemobileappconfigurationassignment?view=graph-rest-beta)<br/>[managedEBookAssignment](/graph/api/resources/intune-books-managedebookassignment?view=graph-rest-beta)<br/>[managedMobileApp](/graph/api/resources/intune-mam-managedmobileapp?view=graph-rest-beta)<br/>[mobileAppAssignment](/graph/api/resources/intune-apps-mobileappassignment?view=graph-rest-beta)<br/>[termsAndConditionsAssignment](/graph/api/resources/intune-companyterms-termsandconditionsassignment?view=graph-rest-beta)<br/>[vppToken](/graph/api/resources/intune-onboarding-vpptoken?view=graph-rest-beta)<br/>[windows10PFXImportCertificateProfile](/graph/api/resources/intune-deviceconfig-windows10pfximportcertificateprofile?view=graph-rest-beta)<br/>[windowsAssignedAccessProfile](/graph/api/resources/intune-deviceconfig-windowsassignedaccessprofile?view=graph-rest-beta)<br/>[windowsDomainJoinConfiguration](/graph/api/resources/intune-deviceconfig-windowsdomainjoinconfiguration?view=graph-rest-beta)<br/>|
|Ergänzungen|Beta|Die folgenden komplexen Typen wurden hinzugefügt:<br/>[iosLobAppAssignmentSettings](/graph/api/resources/intune-apps-ioslobappassignmentsettings?view=graph-rest-beta)<br/>[iosSingleSignOnSettings](/graph/api/resources/intune-deviceconfig-iossinglesignonsettings?view=graph-rest-beta)<br/>[iosStoreAppAssignmentSettings](/graph/api/resources/intune-apps-iosstoreappassignmentsettings?view=graph-rest-beta)<br/>[iosVppAppAssignmentSettings](/graph/api/resources/intune-apps-iosvppappassignmentsettings?view=graph-rest-beta)<br/>[mobileAppAssignmentSettings](/graph/api/resources/intune-apps-mobileappassignmentsettings?view=graph-rest-beta)<br/>[proxiedDomain](/graph/api/resources/intune-deviceconfig-proxieddomain?view=graph-rest-beta)<br/>[windowsInformationProtectionProxiedDomainCollection](/graph/api/resources/intune-mam-windowsinformationprotectionproxieddomaincollection?view=graph-rest-beta)<br/>[windowsStoreForBusinessAppAssignmentSettings](/graph/api/resources/intune-apps-windowsstoreforbusinessappassignmentsettings?view=graph-rest-beta)<br/>|
|Ergänzungen|Beta|Die [assign](/graph/api/intune-apps-mobileapp-assign?view=graph-rest-beta)-Aktion wurde zu [mobileApp](/graph/api/resources/intune-apps-mobileapp?view=graph-rest-beta) hinzugefügt. |
|Ergänzungen|Beta|Die [assign](/graph/api/intune-apps-ioslobappprovisioningconfiguration-assign?view=graph-rest-beta)-Aktion wurde zu [iosLobAppProvisioningConfiguration](/graph/api/resources/intune-apps-ioslobappprovisioningconfiguration?view=graph-rest-beta) hinzugefügt. |
|Ergänzungen|Beta|Die [assign](/graph/api/intune-apps-manageddevicemobileappconfiguration-assign?view=graph-rest-beta)-Aktion wurde zu [managedDeviceMobileAppConfiguration](/graph/api/resources/intune-apps-manageddevicemobileappconfiguration?view=graph-rest-beta) hinzugefügt. |
|Ergänzungen|Beta|Die [assign](/graph/api/intune-deviceconfig-devicecompliancepolicy-assign?view=graph-rest-beta)-Aktion wurde [deviceCompliancePolicy](/graph/api/resources/intune-deviceconfig-devicecompliancepolicy?view=graph-rest-beta) hinzugefügt. |
|Ergänzungen|Beta|Die [assignedAccessMultiModeProfiles](/graph/api/intune-deviceconfig-deviceconfiguration-assignedaccessmultimodeprofiles?view=graph-rest-beta)-Aktion wurde zu [deviceConfiguration](/graph/api/resources/intune-deviceconfig-deviceconfiguration?view=graph-rest-beta) hinzugefügt. |
|Ergänzungen|Beta|Die [syncLicenses](/graph/api/intune-onboarding-vpptoken-synclicenses?view=graph-rest-beta)-Aktion wurde zu [vppToken](/graph/api/resources/intune-onboarding-vpptoken?view=graph-rest-beta) hinzugefügt. |
|Ergänzungen|Beta|Die [targetApps](/graph/api/intune-mam-managedapppolicy-targetapps?view=graph-rest-beta)-Aktion wurde zu [managedAppPolicy](/graph/api/resources/intune-mam-managedapppolicy?view=graph-rest-beta) hinzugefügt. |
|Ergänzungen|Beta|Die [targetApps](/graph/api/intune-mam-managedappprotection-targetapps?view=graph-rest-beta)-Aktion wurde zu [managedAppProtection](/graph/api/resources/intune-mam-managedappprotection?view=graph-rest-beta) hinzugefügt. |
|Ergänzungen|Beta|Die [targetApps](/graph/api/intune-mam-targetedmanagedappconfiguration-targetapps?view=graph-rest-beta)-Aktion wurde zu [targetedManagedAppConfiguration](/graph/api/resources/intune-mam-targetedmanagedappconfiguration?view=graph-rest-beta) hinzugefügt. |
|Ergänzungen|Beta|Die [assign](/graph/api/intune-books-managedebook-assign?view=graph-rest-beta)-Aktion wurde zu [managedEBook](/graph/api/resources/intune-books-managedebook?view=graph-rest-beta) hinzugefügt. |
|Löschung|Beta|Die folgenden Entitäten wurden entfernt:<br/>**cloudPkiSubscription**<br/>|
|Löschung|Beta|Die folgenden komplexen Typen wurden entfernt:<br/>**cloudPkiAdministratorCredentials**<br/>**windowsNetworkIsolationCloudResource**<br/>**windowsNetworkIsolationCloudResourceCollection**<br/>**windowsNetworkIsolationIPRangeCollection**<br/>**windowsNetworkIsolationResourceCollection**<br/>|
|Änderung|Beta|Die **gracePeriodInMinutes**-Eigenschaft wurde zur [androidDeviceComplianceLocalActionBase](/graph/api/resources/intune-deviceconfig-androiddevicecompliancelocalactionbase?view=graph-rest-beta)-Entität hinzugefügt.|
|Änderung|Beta|Die **enableSplitTunneling**-Eigenschaft wurde aus der [androidForWorkVpnConfiguration](/graph/api/resources/intune-deviceconfig-androidforworkvpnconfiguration?view=graph-rest-beta)-Entität entfernt.|
|Änderung|Beta|Die **versionName**- und **versionCode**-Eigenschaften wurden zur [androidLobApp](/graph/api/resources/intune-apps-androidlobapp?view=graph-rest-beta)-Entität hinzugefügt.|
|Änderung|Beta|Die **minimumRequiredPatchVersion**- und **minimumWarningPatchVersion**-Eigenschaften wurden zur [androidManagedAppProtection](/graph/api/resources/intune-mam-androidmanagedappprotection?view=graph-rest-beta)-Entität hinzugefügt.|
|Änderung|Beta|Die **minimumRequiredPatchVersion**- und **minimumWarningPatchVersion**-Eigenschaften wurden zur [defaultManagedAppProtection](/graph/api/resources/intune-mam-defaultmanagedappprotection?view=graph-rest-beta)-Entität hinzugefügt.|
|Änderung|Beta|Die **target**-Eigenschaft wurde zur [deviceCompliancePolicyAssignment](/graph/api/resources/intune-deviceconfig-devicecompliancepolicyassignment?view=graph-rest-beta)-Entität hinzugefügt.|
|Änderung|Beta|Die **singleSignOnSettings**-Eigenschaft wurde zur [iosDeviceFeaturesConfiguration](/graph/api/resources/intune-deviceconfig-iosdevicefeaturesconfiguration?view=graph-rest-beta)-Entität hinzugefügt.|
|Änderung|Beta|Die **versionNumber**- und **buildNumber**-Eigenschaften wurden zur [iosLobApp](/graph/api/resources/intune-apps-ioslobapp?view=graph-rest-beta)-Entität hinzugefügt.|
|Änderung|Beta|Die **bundleId**-Eigenschaft wurde zur [iosVppApp](/graph/api/resources/intune-apps-iosvppapp?view=graph-rest-beta)-Entität hinzugefügt.|
|Änderung|Beta|Die Eigenschaft **preSharedKey** wurde zur Entität [iosWiFiConfiguration](/graph/api/resources/intune-deviceconfig-ioswificonfiguration?view=graph-rest-beta) hinzugefügt.|
|Änderung|Beta|Die **versionName**- und **versionCode**-Eigenschaften wurden zur [managedAndroidLobApp](/graph/api/resources/intune-apps-managedandroidlobapp?view=graph-rest-beta)-Entität hinzugefügt.|
|Änderung|Beta|Die **periodBeforePinReset**-Eigenschaft wurde zur [managedAppProtection](/graph/api/resources/intune-mam-managedappprotection?view=graph-rest-beta)-Entität hinzugefügt.|
|Änderung|Beta|Die **subscriberCarrier**-, **meid**-, **totalStorageSpaceInBytes**- und **freeStorageSpaceInBytes**-Eigenschaften wurden zur [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta)-Entität hinzugefügt.|
|Änderung|Beta|Die **enrollmentType**-Eigenschaft wurde aus der [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta)-Entität entfernt.|
|Änderung|Beta|Die **versionNumber**- und **buildNumber**-Eigenschaften wurden zur [managedIOSLobApp](/graph/api/resources/intune-apps-managedioslobapp?view=graph-rest-beta)-Entität hinzugefügt.|
|Änderung|Beta|Die **displayVersion**-Eigenschaft wurde zur [mobileAppInstallStatus](/graph/api/resources/intune-apps-mobileappinstallstatus?view=graph-rest-beta)-Entität hinzugefügt.|
|Änderung|Beta|Die **defaultDeviceEnrollmentRestrictions**-, **defaultDeviceEnrollmentWindowsHelloForBusinessSettings**- und **defaultDeviceEnrollmentLimit**-Eigenschaften wurden aus der [organization](/graph/api/resources/intune-onboarding-organization?view=graph-rest-beta)-Entität entfernt.|
|Änderung|Beta|Die **isAssigned**-Eigenschaft wurde zur [targetedManagedAppConfiguration](/graph/api/resources/intune-mam-targetedmanagedappconfiguration?view=graph-rest-beta)-Entität hinzugefügt.|
|Änderung|Beta|Die **isAssigned**-Eigenschaft wurde zur [targetedManagedAppProtection](/graph/api/resources/intune-mam-targetedmanagedappprotection?view=graph-rest-beta)-Entität hinzugefügt.|
|Änderung|Beta|Die **activeFirewallRequired**-, **uacRequired**-, **defenderEnabled**-, **defenderVersion**-, **signatureOutOfDate**- und **rtpEnabled**-Eigenschaften wurden zur [windows10CompliancePolicy](/graph/api/resources/intune-deviceconfig-windows10compliancepolicy?view=graph-rest-beta)-Entität hinzugefügt.|
|Änderung|Beta|Die **assignedAccessSingleModeUserName**-, **assignedAccessSingleModeAppUserModelId**-, **microsoftAccountSignInAssistantSettings**-, **authenticationAllowSecondaryDevice**-, **cryptographyAllowFipsAlgorithmPolicy**-, **securityBlockAzureADJoinedDevicesAutoEncryption**-, **systemTelemetryProxyServer**-, **inkWorkspaceAccess**-, **inkWorkspaceBlockSuggestedApps**-, **defenderCloudBlockLevel**- und **defenderCloudExtendedTimeout**-Eigenschaften wurden zur [windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta)-Entität hinzugefügt.|
|Änderung|Beta|Die **protectedApps**-, **enterpriseProxiedDomains**- und **isAssigned**-Eigenschaften wurden zur [windowsInformationProtection](/graph/api/resources/intune-mam-windowsinformationprotection?view=graph-rest-beta)-Entität hinzugefügt.|
|Änderung|Beta|Die **productVersion**-Eigenschaft wurde zur [windowsMobileMSI](/graph/api/resources/intune-apps-windowsmobilemsi?view=graph-rest-beta)-Entität hinzugefügt.|
|Änderung|Beta|Die **apps**-Navigationseigenschaft wurde zur [androidManagedAppProtection](/graph/api/resources/intune-mam-androidmanagedappprotection?view=graph-rest-beta)-Entität hinzugefügt.|
|Änderung|Beta|Die **apps**-Navigationseigenschaft wurde zur [defaultManagedAppProtection](/graph/api/resources/intune-mam-defaultmanagedappprotection?view=graph-rest-beta)-Entität hinzugefügt.|
|Änderung|Beta|Die **vppTokens**-Navigationseigenschaft wurde zur [deviceAppManagement](/graph/api/resources/intune-apps-deviceappmanagement?view=graph-rest-beta)-Entität hinzugefügt.|
|Änderung|Beta|Die **assignments**-Navigationseigenschaft wurde zur [deviceCompliancePolicy](/graph/api/resources/intune-deviceconfig-devicecompliancepolicy?view=graph-rest-beta)-Entität hinzugefügt.|
|Änderung|Beta|Die **deviceCompliancePolicy**-Navigationseigenschaft wurde aus der [deviceCompliancePolicyAssignment](/graph/api/resources/intune-deviceconfig-devicecompliancepolicyassignment?view=graph-rest-beta)-Entität entfernt.|
|Änderung|Beta|Die **deviceCompliancePolicy**-Navigationseigenschaft wurde zur [deviceCompliancePolicyGroupAssignment](/graph/api/resources/intune-deviceconfig-devicecompliancepolicygroupassignment?view=graph-rest-beta)-Entität hinzugefügt.|
|Änderung|Beta|Die **identityCertificateForClientAuthentication**-Navigationseigenschaft wurde zur [iosDeviceFeaturesConfiguration](/graph/api/resources/intune-deviceconfig-iosdevicefeaturesconfiguration?view=graph-rest-beta)-Entität hinzugefügt.|
|Änderung|Beta|Die **assignments**-Navigationseigenschaft wurde zur [iosLobAppProvisioningConfiguration](/graph/api/resources/intune-apps-ioslobappprovisioningconfiguration?view=graph-rest-beta)-Entität hinzugefügt.|
|Änderung|Beta|Die **apps**-Navigationseigenschaft wurde zur [iosManagedAppProtection](/graph/api/resources/intune-mam-iosmanagedappprotection?view=graph-rest-beta)-Entität hinzugefügt.|
|Änderung|Beta|Die **assignments**-Navigationseigenschaft wurde zur [managedDeviceMobileAppConfiguration](/graph/api/resources/intune-apps-manageddevicemobileappconfiguration?view=graph-rest-beta)-Entität hinzugefügt.|
|Änderung|Beta|Die **assignments**-Navigationseigenschaft wurde zur [managedEBook](/graph/api/resources/intune-books-managedebook?view=graph-rest-beta)-Entität hinzugefügt.|
|Änderung|Beta|Die **assignments**-Navigationseigenschaft wurde zur [mobileApp](/graph/api/resources/intune-apps-mobileapp?view=graph-rest-beta)-Entität hinzugefügt.|
|Änderung|Beta|Die **apps**-Navigationseigenschaft wurde zur [targetedManagedAppConfiguration](/graph/api/resources/intune-mam-targetedmanagedappconfiguration?view=graph-rest-beta)-Entität hinzugefügt.|
|Änderung|Beta|Die **assignments**-Navigationseigenschaft wurde zur [termsAndConditions](/graph/api/resources/intune-companyterms-termsandconditions?view=graph-rest-beta)-Entität hinzugefügt.|
|Änderung|Beta|Die **assignedAccessMultiModeProfiles**-Navigationseigenschaft wurde zur [windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta)-Entität hinzugefügt.|
|Änderung|Beta|Die **protectedAppLockerFiles**-Navigationseigenschaft wurde zur [windowsInformationProtection](/graph/api/resources/intune-mam-windowsinformationprotection?view=graph-rest-beta)-Entität hinzugefügt.|
|Änderung|Beta|Die **port**- und **forceTls**-Eigenschaften wurden zum komplexen Typ [airPrintDestination](/graph/api/resources/intune-deviceconfig-airprintdestination?view=graph-rest-beta) hinzugefügt.|
|Änderung|Beta|Der Typ der folgenden Eigenschaften im komplexen Typ [deviceCompliancePolicySettingState](/graph/api/resources/intune-deviceconfig-devicecompliancepolicysettingstate?view=graph-rest-beta) wurde geändert:<br/>**errorCode** von Int32 zu Int64<br/>|
|Änderung|Beta|Der Typ der folgenden Eigenschaften im komplexen Typ [deviceConfigurationSettingState](/graph/api/resources/intune-deviceconfig-deviceconfigurationsettingstate?view=graph-rest-beta) wurde geändert:<br/>**errorCode** von Int32 zu Int64<br/>|
|Änderung|Beta|Der Typ der folgenden Eigenschaften im komplexen Typ [windowsNetworkIsolationPolicy](/graph/api/resources/intune-deviceconfig-windowsnetworkisolationpolicy?view=graph-rest-beta) wurde geändert:<br/>**enterpriseCloudResources** von [windowsNetworkIsolationCloudResourceCollection](/graph/api/resources/intune-deviceconfig-windowsnetworkisolationcloudresourcecollection?view=graph-rest-beta) zu [proxiedDomain](/graph/api/resources/intune-deviceconfig-proxieddomain?view=graph-rest-beta)-Sammlung<br/>**enterpriseInternalProxyServers** von „windowsNetworkIsolationResourceCollection“ zu Zeichenfolgensammlung<br/>**enterpriseIPRanges** von „windowsNetworkIsolationIPRangeCollection“ zu [ipRange](/graph/api/resources/intune-deviceconfig-iprange?view=graph-rest-beta)-Sammlung<br/>**enterpriseNetworkDomainNames** von „windowsNetworkIsolationResourceCollection“ zu Zeichenfolgensammlung<br/>**enterpriseProxyServers** von „windowsNetworkIsolationResourceCollection“ zu Zeichenfolgensammlung<br/>**neutralDomainResources** von „windowsNetworkIsolationResourceCollection“ zu Zeichenfolgensammlung<br/>|

### <a name="microsoft-teams-apis"></a>Microsoft Teams-APIs

|Änderungstyp|Version|Beschreibung|
|:---|:---|:---|
|Ergänzungen|Beta|Es wurde eine neue [team](/graph/api/resources/team?view=graph-rest-beta)-Entität hinzugefügt.|
|Ergänzungen|Beta|Der [team](/graph/api/resources/team?view=graph-rest-beta)-Entität wurden [create](/graph/api/team-put-teams?view=graph-rest-beta)-, [get](/graph/api/team-get?view=graph-rest-beta)- und [update](/graph/api/team-update?view=graph-rest-beta)-Vorgänge hinzugefügt.|

### <a name="outlook-messages"></a>Outlook-Nachrichten

| Änderungstyp | Version | Beschreibung                              |
| :---------- | :------ | :--------------------------------------- |
| Änderung          | v1.0 und Beta | This behavior enhancement is about getting a shared mail folder or its message contents, when a user has shared a mail folder with the signed-in user, or has delegated the user's mailbox to the signed-in user. In such situations, an app can specify that user's ID or user principal name to [get that shared mail folder](/graph/api/mailfolder-get?view=graph-rest-1.0), or [get the messages in that shared calendar](/graph/api/user-list-messages?view=graph-rest-1.0), as long as the signed-in user has provided delegated permissions to the app. |


### <a name="outlook-user-choices"></a>Auswahlmöglichkeiten für Outlook-Benutzer

| Änderungstyp | Version | Beschreibung                              |
| :---------- | :------ | :--------------------------------------- |
|Ergänzungen | Beta | Added the new **workingHours** property to [mailboxSettings](/graph/api/resources/mailboxsettings?view=graph-rest-beta). See [workingHours resource type](/graph/api/resources/workinghours?view=graph-rest-beta) for information on the supported use cases.|
|Ergänzungen | Beta | Die folgenden neuen komplexen Typen wurden hinzugefügt: <br> [workingHours](/graph/api/resources/workinghours?view=graph-rest-beta) <br> [timeZoneBase](/graph/api/resources/timezonebase?view=graph-rest-beta) <br> [customTimeZone](/graph/api/resources/customtimezone?view=graph-rest-beta) <br> [standardTimeZoneOffset](/graph/api/resources/standardtimezoneoffset?view=graph-rest-beta) <br> [daylightTimeZoneOffset](/graph/api/resources/daylighttimezoneoffset?view=graph-rest-beta)|


### <a name="reports-apis"></a>Bericht-APIs
| Änderungstyp | Version | Beschreibung                              |
| :---------- | :------ | :--------------------------------------- |
| Änderung      | Beta    | Added the [getEmailActivityUserDetail](/graph/api/reportroot-getemailactivityuserdetail?view=graph-rest-beta), [getEmailActivityCounts](/graph/api/reportroot-getemailactivitycounts?view=graph-rest-beta), and [getEmailActivityUserCounts](/graph/api/reportroot-getemailactivityusercounts?view=graph-rest-beta) APIs. These replaced the EmailActivity API. |
| Änderung      | Beta    | Added the [getEmailAppUsageUserDetail](/graph/api/reportroot-getemailappusageuserdetail?view=graph-rest-beta), [getEmailAppUsageAppsUserCounts](/graph/api/reportroot-getemailappusageappsusercounts?view=graph-rest-beta), [getEmailAppUsageUserCounts](/graph/api/reportroot-getemailappusageusercounts?view=graph-rest-beta), and [getEmailAppUsageVersionsUserCounts](/graph/api/reportroot-getemailappusageversionsusercounts?view=graph-rest-beta) APIs. These replaced the EmailAppUsage API. |
| Änderung      | Beta    | Added the [getMailboxUsageDetail](/graph/api/reportroot-getmailboxusagedetail?view=graph-rest-beta), [getMailboxUsageMailboxCounts](/graph/api/reportroot-getmailboxusagemailboxcounts?view=graph-rest-beta), [getMailboxUsageQuotaStatusMailboxCounts](/graph/api/reportroot-getmailboxusagequotastatusmailboxcounts?view=graph-rest-beta), and [getMailboxUsageStorage](/graph/api/reportroot-getmailboxusagestorage?view=graph-rest-beta) APIs. These replaced the MailboxUsage API. |
| Änderung      | Beta    | Added the [getOffice365ActivationsUserDetail](/graph/api/reportroot-getoffice365activationsuserdetail?view=graph-rest-beta), [getOffice365ActivationCounts](/graph/api/reportroot-getoffice365activationcounts?view=graph-rest-beta), and [getOffice365ActivationsUserCounts](/graph/api/reportroot-getoffice365activationsusercounts?view=graph-rest-beta) APIs. These replaced the Office365Activations API. |
| Änderung      | Beta    | Added the [getOffice365ActiveUserDetail](/graph/api/reportroot-getoffice365activeuserdetail?view=graph-rest-beta), [getOffice365ActiveUserCounts](/graph/api/reportroot-getoffice365activeusercounts?view=graph-rest-beta), and [getOffice365ServicesUserCounts](/graph/api/reportroot-getoffice365servicesusercounts?view=graph-rest-beta) APIs. These replaced the Office365ActiveUser API. |
| Änderung      | Beta    | Added the [getOffice365GroupsActivityDetail](/graph/api/reportroot-getoffice365groupsactivitydetail?view=graph-rest-beta), [getOffice365GroupsActivityCounts](/graph/api/reportroot-getoffice365groupsactivitycounts?view=graph-rest-beta),[getOffice365GroupsActivityGroupCounts](/graph/api/reportroot-getoffice365groupsactivitygroupcounts?view=graph-rest-beta), [getOffice365GroupsActivityStorage](/graph/api/reportroot-getoffice365groupsactivitystorage?view=graph-rest-beta), and [getOffice365GroupsActivityFileCounts](/graph/api/reportroot-getoffice365groupsactivityfilecounts?view=graph-rest-beta) APIs. These replaced the Office365GroupsActivity API. |
| Änderung      | Beta    | Added the [getOneDriveActivityUserDetail](/graph/api/reportroot-getonedriveactivityuserdetail?view=graph-rest-beta), [getOneDriveActivityUserCounts](/graph/api/reportroot-getonedriveactivityusercounts?view=graph-rest-beta), and [getOneDriveActivityFileCounts](/graph/api/reportroot-getonedriveactivityfilecounts?view=graph-rest-beta) APIs. These replaced the OneDriveActivity API. |
| Änderung      | Beta    | Added the [getOneDriveUsageAccountDetail](/graph/api/reportroot-getonedriveusageaccountdetail?view=graph-rest-beta), [getOneDriveUsageAccountCounts](/graph/api/reportroot-getonedriveusageaccountcounts?view=graph-rest-beta), [getOneDriveUsageFileCounts](/graph/api/reportroot-getonedriveusagefilecounts?view=graph-rest-beta), and [getOneDriveUsageStorage](/graph/api/reportroot-getonedriveusagestorage?view=graph-rest-beta) APIs. These replaced the OneDriveUsage API. |
| Änderung      | Beta    | Added the [getSharePointActivityUserDetail](/graph/api/reportroot-getsharepointactivityuserdetail?view=graph-rest-beta), [getSharePointActivityFileCounts](/graph/api/reportroot-getsharepointactivityfilecounts?view=graph-rest-beta), [getSharePointActivityUserCounts](/graph/api/reportroot-getsharepointactivityusercounts?view=graph-rest-beta), and [getSharePointActivityPages](/graph/api/reportroot-getsharepointactivitypages?view=graph-rest-beta) APIs. These replaced the SharePointActivity API. |
| Änderung      | Beta    | Added the [getSharePointSiteUsageDetail](/graph/api/reportroot-getsharepointsiteusagedetail?view=graph-rest-beta), [getSharePointSiteUsageFileCounts](/graph/api/reportroot-getsharepointsiteusagefilecounts?view=graph-rest-beta), [getSharePointSiteUsageSiteCounts](/graph/api/reportroot-getsharepointsiteusagesitecounts?view=graph-rest-beta), [getSharePointSiteUsageStorage](/graph/api/reportroot-getsharepointsiteusagestorage?view=graph-rest-beta), and [getSharePointSiteUsagePages](/graph/api/reportroot-getsharepointsiteusagepages?view=graph-rest-beta) APIs. These replaced the SharePointSiteUsage API. |
| Änderung      | Beta    | Added the [getSkypeForBusinessActivityUserDetail](/graph/api/reportroot-getskypeforbusinessactivityuserdetail?view=graph-rest-beta), [getSkypeForBusinessActivityCounts](/graph/api/reportroot-getskypeforbusinessactivitycounts?view=graph-rest-beta), and [getSkypeForBusinessActivityUserCounts](/graph/api/reportroot-getskypeforbusinessactivityusercounts?view=graph-rest-beta) APIs. These replaced the SfbActivity API. |
| Änderung      | Beta    | Added the [getSkypeForBusinessDeviceUsageUserDetail](/graph/api/reportroot-getskypeforbusinessdeviceusageuserdetail?view=graph-rest-beta), [getSkypeForBusinessDeviceUsageDistributionUserCounts](/graph/api/reportroot-getskypeforbusinessdeviceusagedistributionusercounts?view=graph-rest-beta), and [getSkypeForBusinessDeviceUsageUserCounts](/graph/api/reportroot-getskypeforbusinessdeviceusageusercounts?view=graph-rest-beta) APIs. These replaced the SfbDeviceUsage API. |
| Änderung      | Beta    | Added the [getSkypeForBusinessOrganizerActivityCounts](/graph/api/reportroot-getskypeforbusinessorganizeractivitycounts?view=graph-rest-beta), [getSkypeForBusinessOrganizerActivityUserCounts](/graph/api/reportroot-getskypeforbusinessorganizeractivityusercounts?view=graph-rest-beta), and [getSkypeForBusinessOrganizerActivityMinuteCounts](/graph/api/reportroot-getskypeforbusinessorganizeractivityminutecounts?view=graph-rest-beta) APIs. These replaced the SfbOrganizerActivity API. |
| Änderung      | Beta    | Added the [getSkypeForBusinessParticipantActivityCounts](/graph/api/reportroot-getskypeforbusinessparticipantactivitycounts?view=graph-rest-beta), [getSkypeForBusinessParticipantActivityUserCounts](/graph/api/reportroot-getskypeforbusinessparticipantactivityusercounts?view=graph-rest-beta), and [getSkypeForBusinessParticipantActivityMinuteCounts](/graph/api/reportroot-getskypeforbusinessparticipantactivityminutecounts?view=graph-rest-beta) APIs. These replaced the SfbParticipantActivity API. |
| Änderung      | Beta    | Added the [getSkypeForBusinessPeerToPeerActivityCounts](/graph/api/reportroot-getskypeforbusinesspeertopeeractivitycounts?view=graph-rest-beta), [getSkypeForBusinessPeerToPeerActivityUserCounts](/graph/api/reportroot-getskypeforbusinesspeertopeeractivityusercounts?view=graph-rest-beta), and [getSkypeForBusinessPeerToPeerActivityMinuteCounts](/graph/api/reportroot-getskypeforbusinesspeertopeeractivityminutecounts?view=graph-rest-beta) APIs. These replaced the SfbP2PActivity API. |
| Änderung      | Beta    | Added the [getYammerActivityUserDetail](/graph/api/reportroot-getyammeractivityuserdetail?view=graph-rest-beta), [getYammerActivityCounts](/graph/api/reportroot-getyammeractivitycounts?view=graph-rest-beta), and [getYammerActivityUserCounts](/graph/api/reportroot-getyammeractivityusercounts?view=graph-rest-beta) APIs. These replaced the YammerActivity API. |
| Änderung      | Beta    | Added the [getYammerDeviceUsageUserDetail](/graph/api/reportroot-getyammerdeviceusageuserdetail?view=graph-rest-beta), [getYammerDeviceUsageDistributionUserCounts](/graph/api/reportroot-getyammerdeviceusagedistributionusercounts?view=graph-rest-beta), and [getYammerDeviceUsageUserCounts](/graph/api/reportroot-getyammerdeviceusageusercounts?view=graph-rest-beta) APIs. These replaced the YammerDeviceUsage API. |
| Änderung      | Beta    | Added the [getYammerGroupsActivityDetail](/graph/api/reportroot-getyammergroupsactivitydetail?view=graph-rest-beta), [getYammerGroupsActivityGroupCounts](/graph/api/reportroot-getyammergroupsactivitygroupcounts?view=graph-rest-beta), and [getYammerGroupsActivityCounts](/graph/api/reportroot-getyammergroupsactivitycounts?view=graph-rest-beta) APIs. These replaced the YammerGroupsActivity API. |



## <a name="september-2017"></a>September 2017

### <a name="intune-apis"></a>Intune APIs

| Änderungstyp | Version | Beschreibung                              |
| :---------- | :------ | :--------------------------------------- |
| Ergänzungen    | Beta    | Hinzugefügte neue Entitäten:<br/>[activeDirectoryWindowsAutopilotDeploymentProfile](/graph/api/resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile?view=graph-rest-beta)<br/>[azureADWindowsAutopilotDeploymentProfile](/graph/api/resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile?view=graph-rest-beta)<br/>[deviceEnrollmentConfiguration](/graph/api/resources/intune-onboarding-deviceenrollmentconfiguration?view=graph-rest-beta)<br/>[deviceEnrollmentLimitConfiguration](/graph/api/resources/intune-onboarding-deviceenrollmentlimitconfiguration?view=graph-rest-beta)<br/>[deviceEnrollmentPlatformRestrictionsConfiguration](/graph/api/resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration?view=graph-rest-beta)<br/>[deviceEnrollmentWindowsHelloForBusinessConfiguration](/graph/api/resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration?view=graph-rest-beta)<br/>[deviceManagementPartner](/graph/api/resources/intune-onboarding-devicemanagementpartner?view=graph-rest-beta)<br/>[enrollmentConfigurationAssignment](/graph/api/resources/intune-onboarding-enrollmentconfigurationassignment?view=graph-rest-beta)<br/>[windows10EnrollmentCompletionPageConfiguration](/graph/api/resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration?view=graph-rest-beta)<br/>[windows10NetworkBoundaryConfiguration](/graph/api/resources/intune-deviceconfig-windows10networkboundaryconfiguration?view=graph-rest-beta)<br/>[windowsAutopilotDeploymentProfile](/graph/api/resources/intune-enrollment-windowsautopilotdeploymentprofile?view=graph-rest-beta)<br/>[windowsAutopilotDeviceIdentity](/graph/api/resources/intune-enrollment-windowsautopilotdeviceidentity?view=graph-rest-beta)<br/>[windowsAutopilotSettings](/graph/api/resources/intune-enrollment-windowsautopilotsettings?view=graph-rest-beta)<br/> |
| Ergänzungen    | Beta    | Die folgenden komplexen Typen wurden hinzugefügt:<br/>[adminConsent](/graph/api/resources/intune-devices-adminconsent?view=graph-rest-beta)<br/>[allDevicesAssignmentTarget](/graph/api/resources/intune-shared-alldevicesassignmenttarget?view=graph-rest-beta)<br/>[allLicensedUsersAssignmentTarget](/graph/api/resources/intune-shared-alllicensedusersassignmenttarget?view=graph-rest-beta)<br/>[deviceAndAppManagementAssignmentTarget](/graph/api/resources/intune-shared-deviceandappmanagementassignmenttarget?view=graph-rest-beta)<br/>[deviceEnrollmentPlatformRestriction](/graph/api/resources/intune-onboarding-deviceenrollmentplatformrestriction?view=graph-rest-beta)<br/>[deviceHealthAttestationState](/graph/api/resources/intune-devices-devicehealthattestationstate?view=graph-rest-beta)<br/>[exclusionGroupAssignmentTarget](/graph/api/resources/intune-shared-exclusiongroupassignmenttarget?view=graph-rest-beta)<br/>[groupAssignmentTarget](/graph/api/resources/intune-shared-groupassignmenttarget?view=graph-rest-beta)<br/>[outOfBoxExperienceSettings](/graph/api/resources/intune-enrollment-outofboxexperiencesettings?view=graph-rest-beta)<br/>[windowsFirewallNetworkProfile](/graph/api/resources/intune-deviceconfig-windowsfirewallnetworkprofile?view=graph-rest-beta)<br/>windowsNetworkIsolationCloudResource<br/>windowsNetworkIsolationCloudResourceCollection<br/>windowsNetworkIsolationIPRangeCollection<br/>[windowsNetworkIsolationPolicy](/graph/api/resources/intune-deviceconfig-windowsnetworkisolationpolicy?view=graph-rest-beta)<br/>windowsNetworkIsolationResourceCollection<br/> |
| Ergänzungen    | Beta    | Die [sync](/graph/api/intune-enrollment-windowsautopilotsettings-sync?view=graph-rest-beta)-Aktion wurde [windowsAutopilotSettings](/graph/api/resources/intune-enrollment-windowsautopilotsettings?view=graph-rest-beta) hinzugefügt. |
| Ergänzungen    | Beta    | Die [assign](/graph/api/intune-enrollment-windowsautopilotdeploymentprofile-assign?view=graph-rest-beta)-Aktion wurde [windowsAutopilotDeploymentProfile](/graph/api/resources/intune-enrollment-windowsautopilotdeploymentprofile?view=graph-rest-beta) hinzugefügt. |
| Ergänzungen    | Beta    | Aktion „localActions“ zu [deviceCompliancePolicy](/graph/api/resources/intune-deviceconfig-devicecompliancepolicy?view=graph-rest-beta) hinzugefügt. |
| Ergänzungen    | Beta    | Die [setPriority](/graph/api/intune-onboarding-deviceenrollmentconfiguration-setpriority?view=graph-rest-beta)-Aktion wurde [deviceEnrollmentConfiguration](/graph/api/resources/intune-onboarding-deviceenrollmentconfiguration?view=graph-rest-beta) hinzugefügt. |
| Ergänzungen    | Beta    | Die [assign](/graph/api/intune-onboarding-deviceenrollmentconfiguration-assign?view=graph-rest-beta)-Aktion wurde [deviceEnrollmentConfiguration](/graph/api/resources/intune-onboarding-deviceenrollmentconfiguration?view=graph-rest-beta) hinzugefügt. |
| Ergänzungen    | Beta    | Die uploadDepToken-Aktion wurde der [depOnboardingSetting](/graph/api/resources/intune-onboarding-deponboardingsetting?view=graph-rest-beta)-Sammlung hinzugefügt. |
| Ergänzungen    | Beta    | Die syncWithAppleDeviceEnrollmentProgram-Aktion wurde der [depOnboardingSetting](/graph/api/resources/intune-onboarding-deponboardingsetting?view=graph-rest-beta)-Sammlung hinzugefügt. |
| Ergänzungen    | Beta    | Die updateMobileAppIdentifierDeployments-Aktion wurde zu [managedAppProtection](/graph/api/resources/intune-mam-managedappprotection?view=graph-rest-beta) hinzugefügt. |
| Ergänzungen    | Beta    | Die assign-Aktion wurde für [targetedManagedAppProtection](/graph/api/resources/intune-mam-targetedmanagedappprotection?view=graph-rest-beta) hinzugefügt. |
| Ergänzungen    | Beta    | Die assign-Aktion wurde für [targetedManagedAppConfiguration](/graph/api/resources/intune-mam-targetedmanagedappconfiguration?view=graph-rest-beta) hinzugefügt. |
| Ergänzungen    | Beta    | Die assign-Aktion wurde für [windowsInformationProtection](/graph/api/resources/intune-mam-windowsinformationprotection?view=graph-rest-beta) hinzugefügt. |
| Ergänzungen    | Beta    | Die getEncryptionPublicKey-Funktion wurde für die [depOnboardingSetting](/graph/api/resources/intune-onboarding-deponboardingsetting?view=graph-rest-beta)-Sammlung hinzugefügt |
| Änderung      | Beta    | Die Eigenschaften **requireSafetyNetAttestationBasicIntegrity**, **requireSafetyNetAttestationCertifiedDevice**, **requireGooglePlayServices**, **requireUpToDateSecurityProviders**, **requireCompanyPortalAppIntegrity** und **conditionStatementId** wurden der [androidCompliancePolicy](/graph/api/resources/intune-deviceconfig-androidcompliancepolicy?view=graph-rest-beta)-Entität hinzugefügt. |
| Ändern      | Beta    | Die Eigenschaften **requireAppVerify**, **requireSafetyNetAttestationBasicIntegrity**, **requireSafetyNetAttestationCertifiedDevice**, **requireGooglePlayServices**, **requireUpToDateSecurityProviders** and **requireCompanyPortalAppIntegrity** wurden der [androidForWorkCompliancePolicy](/graph/api/resources/intune-deviceconfig-androidforworkcompliancepolicy?view=graph-rest-beta)-Entität hinzugefügt. |
| Änderung      | Beta    | Die Eigenschaften **blockCrossProfileCopyPaste** und **requireAppVerify** wurden der [androidForWorkGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration?view=graph-rest-beta)-Entität hinzugefügt. |
| Änderung      | Beta    | Die Eigenschaften **kioskModeApps** und **requireAppVerify** wurden der [androidGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidgeneraldeviceconfiguration?view=graph-rest-beta)-Entität hinzugefügt. |
| Änderung      | Beta    | Die **kioskModeManagedApps**-Eigenschaft wurde aus der [androidGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidgeneraldeviceconfiguration?view=graph-rest-beta)-Entität entfernt. |
| Änderung      | Beta    | Die **cloudPkiProvider**-, **createdDateTime**-, **description**-, **lastModifiedDateTime**-, **displayName**-, **syncStatus**-, **lastSyncError**-, **lastSyncDateTime**-, **credentials**-, **trustedRootCertificate**- und **version**-Eigenschaften wurden aus der cloudPkiSubscription-Entität entfernt. |
| Änderung      | Beta    | Die Eigenschaften **assignmentStatus**, **assignmentProgress** und **assignmentErrorMessage** wurden der [deviceConfiguration](/graph/api/resources/intune-deviceconfig-deviceconfiguration?view=graph-rest-beta)-Entität hinzugefügt. |
| Änderung      | Beta    | Die **intuneBrand**-Eigenschaft wurde der [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta)-Entität hinzugefügt. |
| Änderung      | Beta    | Die Eigenschaften **vppTokenOrganizationName**, **vppTokenAccountType** und **vppTokenAppleId** wurden der [iosVppApp](/graph/api/resources/intune-apps-iosvppapp?view=graph-rest-beta)-Entität hinzugefügt. |
| Änderung      | Beta    | Die **deviceEnrollmentType**, **wiFiMacAddress** und **deviceHealthAttestationState**-Eigenschaften wurden der [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta)-Entität hinzugefügt. |
| Änderung      | Beta    | Die **legacyAppConfiguration**-Eigenschaft wurde der [managedDeviceMobileAppConfiguration](/graph/api/resources/intune-apps-manageddevicemobileappconfiguration?view=graph-rest-beta)-Entität hinzugefügt. |
| Änderung      | Beta    | Die **notApplicableCount**-Eigenschaft wurde der [managedDeviceMobileAppConfigurationDeviceSummary](/graph/api/resources/intune-apps-manageddevicemobileappconfigurationdevicesummary?view=graph-rest-beta)-Entität hinzugefügt. |
| Änderung      | Beta    | Die **notApplicableCount**-Eigenschaft wurde der [managedDeviceMobileAppConfigurationUserSummary](/graph/api/resources/intune-apps-manageddevicemobileappconfigurationusersummary?view=graph-rest-beta)-Entität hinzugefügt. |
| Änderung      | Beta    | Die Eigenschaften **firewallBlockStatefulFTP**, **firewallIdleTimeoutForSecurityAssociationInSeconds**, **firewallPreSharedKeyEncodingMethod**, **firewallIPSecExemptionsAllowNeighborDiscovery**, **firewallIPSecExemptionsAllowICMP**, **firewallIPSecExemptionsAllowRouterDiscovery**, **firewallIPSecExemptionsAllowDHCP**, **firewallCertificateRevocationListCheckMethod**, **firewallMergeKeyingModuleSettings**, **firewallPacketQueueingMethod**, **firewallProfileDomain**, **firewallProfilePublic**, **firewallProfilePrivate**, **defenderAttackSurfaceReductionExcludedPaths**, **defenderOfficeAppsOtherProcessInjectionType**, **defenderOfficeAppsExecutableContentCreationOrLaunchType**, **defenderOfficeAppsLaunchChildProcessType**, **defenderOfficeMacroCodeAllowWin32ImportsType**, **defenderScriptObfuscatedMacroCodeType**, **defenderScriptDownloadedPayloadExecutionType**, **defenderEmailContentExecutionType**, **defenderGuardMyFoldersType**, **defenderGuardedFoldersAllowedAppPaths**, **defenderAdditionalGuardedFolders**, **defenderNetworkProtectionType**, **defenderExploitProtectionXml**, **defenderExploitProtectionXmlFileName**, **defenderSecurityCenterBlockExploitProtectionOverride**, **appLockerApplicationControl**, **applicationGuardBlockClipboardSharing**, **applicationGuardAllowPrintToPDF**, **applicationGuardAllowPrintToXPS**, **applicationGuardAllowPrintToLocalPrinters**, **applicationGuardAllowPrintToNetworkPrinters** und **bitLockerDisableWarningForOtherDiskEncryption** wurden der [windows10EndpointProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windows10endpointprotectionconfiguration?view=graph-rest-beta)-Entität hinzugefügt. |
| Änderung      | Beta    | Die Eigenschaften **displayAppListWithGdiDPIScalingTurnedOn**, **displayAppListWithGdiDPIScalingTurnedOff**, **messagingBlockSync**, **messagingBlockMMS** und **messagingBlockRichCommunicationServices** wurden der [windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta)-Entität hinzugefügt. |
| Änderung      | Beta    | Die **bluetoothDeviceName**-Eigenschaft wurde aus der [windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta)-Entität entfernt. |
| Änderung      | Beta    | Die Eigenschaften **deviceAccountBlockExchangeServices**, **deviceAccountEmailAddress**, **deviceAccountExchangeServerAddress**, **deviceAccountRequirePasswordRotation** und **deviceAccountSessionInitiationProtocolAddress** wurden aus der [windows10TeamGeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10teamgeneralconfiguration?view=graph-rest-beta)-Entität entfernt. |
| Änderung      | Beta    | Die **localActions**-Navigationseigenschaft wurde der [androidCompliancePolicy](/graph/api/resources/intune-deviceconfig-androidcompliancepolicy?view=graph-rest-beta)-Entität hinzugefügt. |
| Änderung      | Beta    | Die Navigationseigenschaften **windowsAutopilotSettings**, **windowsAutopilotDeviceIdentities**, **windowsAutopilotDeploymentProfiles**, **deviceEnrollmentConfigurations**, **deviceManagementPartners** und **depOnboardingSettings** wurden der [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta)-Entität hinzugefügt. |
| Änderung      | Beta    | Die **cloudPkiSubscriptions**-Navigationseigenschaft wurde aus der [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta)-Entität entfernt. |
| Änderung      | Beta    | Die **assignments**-Navigationseigenschaft wurde aus der [targetedManagedAppConfiguration](/graph/api/resources/intune-mam-targetedmanagedappconfiguration?view=graph-rest-beta)-Entität entfernt. |
| Änderung      | Beta    | Die **assignments**-Navigationseigenschaft wurde aus der [targetedManagedAppProtection](/graph/api/resources/intune-mam-targetedmanagedappprotection?view=graph-rest-beta)-Entität entfernt. |
| Änderung      | Beta    | Die **assignments**-Navigationseigenschaft wurde aus der [windowsInformationProtection](/graph/api/resources/intune-mam-windowsinformationprotection?view=graph-rest-beta)-Entität entfernt. |

### <a name="onedrive"></a>OneDrive

| **Änderungstyp** | **Version** | **Beschreibung**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Ergänzungen        | v1.0        | Die **system**-Eigenschaft wurde der [Drive][]-Ressource hinzugefügt. |
| Ergänzungen        | v1.0        | Die **list**-Beziehung wurde der [Drive][]-Ressource hinzugefügt. |
| Ergänzungen        | v1.0        | Die **listItem**-Beziehung wurde der [DriveItem][]-Ressource hinzugefügt. |
| Ergänzungen        | v1.0        | Die Beziehungen **list** und **listItem** wurden der [SharedDriveItem][]-Ressource hinzugefügt. |
| Ergänzungen        | v1.0        | Die folgenden komplexen Typen wurden hinzugefügt: [FolderView][]  |
| Ergänzungen        | v1.0        | Die **view**-Eigenschaft wurde dem komplexen Typ [Folder][] hinzugefügt. |
| Ergänzungen        | v1.0        | Die **driveType**-Eigenschaft wurde dem komplexen Typ [ItemReference][] hinzugefügt. |
| Ergänzungen        | v1.0        | Die Eigenschaften **audioBitsPerSample**, **audioChannels**, **audioFormat**, **audioSamplesPerSecond**, **fourCC** und **frameRate** wurden dem komplexen Typ [Video][] hinzugefügt. |
| Ergänzungen        | Beta        | Die **system**-Eigenschaft wurde der [Drive][Drive-beta]-Ressource hinzugefügt. |
| Ergänzungen        | Beta        | Die **activities**-Beziehung wurde der [Drive][Drive-beta]-Ressource hinzugefügt. |
| Ergänzungen        | Beta        | Die **publication**-Eigenschaft wurde der [DriveItem][DriveItem-beta]-Ressource hinzugefügt. |
| Ergänzungen        | Beta        | Die Beziehungen **activities** und **versions** wurden der [DriveItem][DriveItem-beta]-Ressource hinzugefügt. |
| Ergänzungen        | Beta        | Hinzugefügte neue Entitäten: [DriveItemVersion][DriveItemVersion-beta], [ItemActivity][ItemActivity-beta]. |
| Ergänzungen        | Beta        | Die folgenden komplexen Typen wurden hinzugefügt: [CommentAction][CommentAction-beta], [CreateAction][CreateAction-beta], [DeleteAction][DeleteAction-beta], [EditAction][EditAction-beta], [ItemActionSet][ItemActionSet-beta], [ItemActivityTimeSet][ItemActivityTimeSet-beta], [MentionAction][MentionAction-beta], [MoveAction][MoveAction-beta], [PublicationFacet][PublicationFacet-beta], [RenameAction][RenameAction-beta], [RestoreAction][RestoreAction-beta], [ShareAction][ShareAction-beta] und [VersionAction][VersionAction-beta]. |
| Ergänzungen        | Beta        | Die **driveType**-Eigenschaft wurde dem komplexen Typ [ItemReference][ItemReference-beta] hinzugefügt. |
| Löschung        | Beta        | Die **tenantId**-Eigenschaft wurde aus dem komplexen TYp [SharepointIds][SharepointIds-beta] entfernt. |
| Ergänzungen        | v1.0        | Die Eigenschaften **audioBitsPerSample**, **audioChannels**, **audioFormat**, **audioSamplesPerSecond**, **fourCC** und **frameRate** wurden dem komplexen Typ [Video][Video-beta] hinzugefügt. |
| Ergänzungen        | Beta        | Die Aktionen [CheckIn][CheckIn-beta] und [CheckOut][CheckOut-beta]wurden der [DriveItem][DriveItem-beta]-Ressource hinzugefügt. |
| Ergänzungen        | Beta        | Die Eigenschaften **expirationDateTime**, **password**, **message** und **recipients** wurden in der [CreateLink][CreateLink-beta]-Aktion der [DriveItem][DriveItem-beta]-Ressource hinzugefügt. |

[Drive]: /graph/api/resources/drive?view=graph-rest-1.0
[DriveItem]: /graph/api/resources/driveitem?view=graph-rest-1.0
[SharedDriveItem]: /graph/api/resources/shareddriveitem?view=graph-rest-1.0
[FolderView]: /graph/api/resources/folderview?view=graph-rest-1.0
[Folder]: /graph/api/resources/folder?view=graph-rest-1.0
[ItemReference]: /graph/api/resources/itemreference?view=graph-rest-1.0
[Video]: /graph/api/resources/video?view=graph-rest-1.0
[Drive-beta]: /graph/api/resources/drive?view=graph-rest-beta
[DriveItem-beta]: /graph/api/resources/driveitem?view=graph-rest-beta
[DriveItemVersion-beta]: /graph/api/resources/driveitemversion?view=graph-rest-beta
[ItemActivity-beta]: /graph/api/resources/itemactivity?view=graph-rest-beta
[CommentAction-beta]: /graph/api/resources/commentaction?view=graph-rest-beta
[CreateAction-beta]: /graph/api/resources/createaction?view=graph-rest-beta
[DeleteAction-beta]: /graph/api/resources/deleteaction?view=graph-rest-beta
[EditAction-beta]: /graph/api/resources/editaction?view=graph-rest-beta
[ItemActionSet-beta]: /graph/api/resources/itemactionset?view=graph-rest-beta
[ItemActivityTimeSet-beta]: /graph/api/resources/itemactivitytimeset?view=graph-rest-beta
[MentionAction-beta]: /graph/api/resources/mentionaction?view=graph-rest-beta
[MoveAction-beta]: /graph/api/resources/moveaction?view=graph-rest-beta
[PublicationFacet-beta]: /graph/api/resources/publicationfacet?view=graph-rest-beta
[RenameAction-beta]: /graph/api/resources/renameaction?view=graph-rest-beta
[RestoreAction-beta]: /graph/api/resources/restoreaction?view=graph-rest-beta
[ShareAction-beta]: /graph/api/resources/shareaction?view=graph-rest-beta
[VersionAction-beta]: /graph/api/resources/versionaction?view=graph-rest-beta
[ItemReference-beta]: /graph/api/resources/itemreference?view=graph-rest-beta
[SharepointIds-beta]: /graph/api/resources/sharepointids?view=graph-rest-beta
[Video-beta]: /graph/api/resources/video?view=graph-rest-beta
[CheckIn-beta]: /graph/api/driveitem-checkin?view=graph-rest-beta
[CheckOut-beta]: /graph/api/driveitem-checkout?view=graph-rest-beta
[CreateLink-beta]: /graph/api/driveitem-createlink?view=graph-rest-beta


### <a name="outlook-calendar"></a>Outlook-Kalender

| **Änderungstyp** | **Version**   | **Beschreibung**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Ergänzungen        | Beta          | Die Funktionen [findRoomLists](/graph/api/user-findroomlists?view=graph-rest-beta) und [findRooms](/graph/api/user-findrooms?view=graph-rest-beta) wurden der [user](/graph/api/resources/user?view=graph-rest-beta)-Entität hinzugefügt. |
| Ergänzungen        | Beta          | Die **locations**-Eigenschaft wurde der [event](/graph/api/resources/event?view=graph-rest-beta)-Entität zur Unterstützung der Organisation von Ereignissen hinzugefügt, an denen Teilnehmer von mehr als einem Ort teilnehmen können. |
| Ergänzungen        | Beta          | Eigenschaft **locationType** wurde zum komplexen Typ [location](/graph/api/resources/location?view=graph-rest-beta) hinzugefügt. |
| Ergänzungen        | Beta          | Added the **uniqueId** and **uniqueIdType** properties to the [location](/graph/api/resources/location?view=graph-rest-beta) complex type. These properties are only for internal use at this point. |
| Änderung          | v1.0 und Beta | This behavior enhancement is about getting a shared calendar or its event contents, when a user has shared a calendar with the signed-in user, or has delegated the user's mailbox to the signed-in user. In such situations, an app can specify that user's ID or user principal name to [get that shared calendar](/graph/api/calendar-get?view=graph-rest-1.0), or [get the events in that shared calendar](/graph/api/user-list-events?view=graph-rest-1.0), as long as the signed-in user has provided delegated permissions to the app. |

### <a name="outlook-contacts"></a>Outlook-Kontakte

| **Änderungstyp** | **Version**   | **Beschreibung**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Änderung          | v1.0 und Beta | This behavior enhancement is about getting a shared contact folder or its contact contents, when a user has shared a contact folder with the signed-in user, or has delegated the user's mailbox to the signed-in user. In such situations, an app can specify that user's ID or user principal name to [get that shared contact folder](/graph/api/contactfolder-get?view=graph-rest-1.0), or [get the contacts in that shared folder](/graph/api/user-list-contacts?view=graph-rest-1.0), as long as the signed-in user has provided delegated permissions to the app. |

### <a name="outlook-mail"></a>Outlook-Mail

| **Änderungstyp** | **Version** | **Beschreibung**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Ergänzungen        | Beta        | Die **internetMessageHeaders**-Eigenschaft wurde der [message](/graph/api/resources/message?view=graph-rest-beta)-Entität hinzugefügt. |
| Ergänzungen        | Beta        | Der komplexe Typ [internetMessageHeader](/graph/api/resources/internetmessageheader?view=graph-rest-beta) wurde hinzugefügt. |
| Ergänzungen        | Beta        | Added the **messageRules** navigation property to the [mailFolder](/graph/api/resources/mailfolder?view=graph-rest-beta) entity. **messageRules** is a collection of [messageRule](/graph/api/resources/messagerule?view=graph-rest-beta) instances. |
| Ergänzungen        | Beta        | Entität [messageRule](/graph/api/resources/messagerule?view=graph-rest-beta) sowie die komplexen Typen [messageRuleActions](/graph/api/resources/messageruleactions?view=graph-rest-beta), [messageRulePredicates](/graph/api/resources/messagerulepredicates?view=graph-rest-beta) und [sizeRange](/graph/api/resources/sizerange?view=graph-rest-beta) wurden hinzugefügt. |
| Ergänzungen        | Beta        | Die folgenden CRUD-Vorgänge für Nachrichtenregeln wurden hinzugefügt: [create](/graph/api/mailfolder-post-messagerules?view=graph-rest-beta), [list](/graph/api/mailfolder-list-messagerules?view=graph-rest-beta), [get](/graph/api/messagerule-get?view=graph-rest-beta), [update](/graph/api/messagerule-update?view=graph-rest-beta) und [delete](/graph/api/messagerule-delete?view=graph-rest-beta). |


### <a name="outlook-user-choices"></a>Auswahlmöglichkeiten für Outlook-Benutzer

| **Änderungstyp** | **Version** | **Beschreibung**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Ergänzungen        | Beta        | Added the new **masterCategories** navigation property to the [outlookUser](/graph/api/resources/outlookuser?view=graph-rest-beta) entity. **masterCategories** is a collection of [outlookCategory](/graph/api/resources/outlookcategory?view=graph-rest-beta) objects. |
| Ergänzungen        | Beta        | Die [outlookCategory](/graph/api/resources/outlookcategory?view=graph-rest-beta)-Entität wurde hinzugefügt. |
| Ergänzungen        | Beta        | Die folgenden CRUD-Vorgänge für [outlookCategory](/graph/api/resources/outlookcategory?view=graph-rest-beta) wurden hinzugefügt: [create](/graph/api/outlookuser-post-mastercategories?view=graph-rest-beta), [get](/graph/api/outlookcategory-get?view=graph-rest-beta), [update](/graph/api/outlookcategory-update?view=graph-rest-beta) und [delete](/graph/api/outlookcategory-delete?view=graph-rest-beta). |
| Ergänzungen        | Beta        | Die neue Funktion [supportedLanguages](/graph/api/outlookuser-supportedlanguages?view=graph-rest-beta) wurde zur Entität [outlookUser](/graph/api/resources/outlookuser?view=graph-rest-beta) hinzugefügt. |
| Ergänzungen        | Beta        | Die neue [supportedTimeZones](/graph/api/outlookuser-supportedtimezones?view=graph-rest-beta)-Funktion wurde der [outlookUser](/graph/api/resources/outlookuser?view=graph-rest-beta)-Entität hinzugefügt. |


### <a name="sharepoint-lists"></a>SharePoint-Listen

| **Änderungstyp** | **Version** | **Beschreibung**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Ergänzungen        | v1.0        | Hinzugefügte neue Entitäten: [ColumnDefinition][], [ColumnLink][], [ContentType][], [List][], [ListItem][]. |
| Ergänzungen        | v1.0        | Die Beziehungen **columns**, **contentTypes**, **items** und **lists** wurden der [Site][]-Ressource hinzugefügt. |
| Ergänzungen        | v1.0        | Die folgenden komplexen Typen wurden hinzugefügt: [BooleanColumn][], [CalculatedColumn][], [ChoiceColumn][], [ContentTypeInfo][], [ContentTypeOrder][], [CurrencyColumn][], [DateTimeColumn][], [DefaultColumnValue][], [ListInfo][], [LookupColumn][], [NumberColumn][], [PersonOrGroupColumn][], [SystemFacet][], [TextColumn][]. |
| Ergänzungen        | Beta        | Hinzugefügte neue Entitäten: [BaseItemVersion][BaseItemVersion-beta], [ColumnLink][ColumnLink-beta], [ContentType][ContentType-beta], [ListItemVersion][ListItemVersion-beta], |
| Ergänzungen        | Beta        | Die Eigenschaften **columnGroup**, **currency**, **defaultValue** und **displayName** wurden [ColumnDefinition][ColumnDefinition-beta] hinzugefügt. |
| Ergänzungen        | Beta        | Die Eigenschaften **displayName** und **system** wurden der [List][List-beta]-Ressource hinzugefügt. |
| Ergänzungen        | Beta        | Die Beziehungen **activities** und **contentTypes** wurden der [List][List-beta]-Ressource hinzugefügt. |
| Ergänzungen        | Beta        | Die **contentType**-Eigenschaft wurde der [ListItem][ListItem-beta]-Ressource hinzugefügt. |
| Ergänzungen        | Beta        | Die Beziehungen **activities** und **versions** wurden der [ListItem][ListItem-beta]-Ressource hinzugefügt. |
| Ergänzungen        | Beta        | Die **contentType**-Beziehung wurde der [Site][Site-beta]-Ressource hinzugefügt. |
| Ergänzungen        | Beta        | Die **outputType**-Eigenschaft wurde dem [BooleanColumn][BooleanColumn-beta]-Typ hinzugefügt. |
| Ergänzungen        | Beta        | Die folgenden komplexen Typen wurden hinzugefügt: [ContentTypeInfo][ContentTypeInfo-beta], [ContentTypeOrder][ContentTypeOrder-beta], [CurrencyColumn][CurrencyColumn-beta] und [SystemFacet][SystemFacet-beta]. |
| Ergänzungen        | Beta        | Die **contentTypesEnabled**-Eigenschaft wurde dem komplexen Typ [ListInfo] [ ListInfo-beta] hinzugefügt. |
| Ergänzungen        | Beta        | Die **allowUnlimitedLength**-Eigenschaft wurde dem komplexen Typ [LookupColumn][LookupColumn-beta] hinzugefügt. |
| Änderung          | Beta        | Die **allowMultipleValue**-Eigenschaft wurde in **allowMultipleValues** im komplexen Typ [LookupColumn][LookupColumn-beta] umbenannt. |
| Änderung          | Beta        | Die **ChooseFrom**-Eigenschaft wurde in **chooseFromType** im komplexen Datentyp [PersonOrGroupColumn][PersonOrGroupColumn-beta] umbenannt. |
| Löschung        | Beta        | Die **locale**-Eigenschaft wurde aus dem komplexen Typ [NumberColumn][NumberColumn-beta] entfernt. |
| Löschung        | Beta        | Die **enforceUniqueValues**-Eigenschaft wurde aus dem komplexen Typ [PersonOrGroupColumn][PersonOrGroupColumn-beta] entfernt. |

[BaseItemVersion-beta]: /graph/api/resources/baseitemversion?view=graph-rest-beta
[BooleanColumn-beta]:  /graph/api/resources/booleanColumn?view=graph-rest-beta
[BooleanColumn]: /graph/api/resources/booleancolumn?view=graph-rest-1.0
[CalculatedColumn]: /graph/api/resources/calculatedcolumn?view=graph-rest-1.0
[ChoiceColumn]: /graph/api/resources/choicecolumn?view=graph-rest-1.0
[ColumnDefinition-beta]: /graph/api/resources/columndefinition?view=graph-rest-beta
[ColumnDefinition]: /graph/api/resources/columndefinition?view=graph-rest-1.0
[ColumnLink-beta]: /graph/api/resources/columnlink?view=graph-rest-beta
[ColumnLink]: /graph/api/resources/columnlink?view=graph-rest-1.0
[ContentType-beta]: /graph/api/resources/contenttype?view=graph-rest-beta
[ContentType]: /graph/api/resources/contenttype?view=graph-rest-1.0
[ContentTypeInfo-beta]: /graph/api/resources/contenttypeinfo?view=graph-rest-beta
[ContentTypeInfo]: /graph/api/resources/contenttypeinfo?view=graph-rest-1.0
[ContentTypeOrder-beta]: /graph/api/resources/contenttypeorder?view=graph-rest-beta
[ContentTypeOrder]: /graph/api/resources/contenttypeorder?view=graph-rest-1.0
[CurrencyColumn-beta]: /graph/api/resources/currencycolumn?view=graph-rest-beta
[CurrencyColumn]: /graph/api/resources/currencycolumn?view=graph-rest-1.0
[DateTimeColumn]: /graph/api/resources/datetimecolumn?view=graph-rest-1.0
[DefaultColumnValue]: /graph/api/resources/defaultcolumnvalue?view=graph-rest-1.0
[List-beta]: /graph/api/resources/list?view=graph-rest-beta
[List]: /graph/api/resources/list?view=graph-rest-1.0
[ListInfo-beta]: /graph/api/resources/listinfo?view=graph-rest-beta
[ListInfo]: /graph/api/resources/listinfo?view=graph-rest-1.0
[ListItem-beta]: /graph/api/resources/listitem?view=graph-rest-beta
[ListItem]: /graph/api/resources/listitem?view=graph-rest-1.0
[ListItemVersion-beta]: /graph/api/resources/listitemversion?view=graph-rest-beta
[LookupColumn-beta]: /graph/api/resources/lookupcolumn?view=graph-rest-beta
[LookupColumn]: /graph/api/resources/lookupcolumn?view=graph-rest-1.0
[NumberColumn-beta]: /graph/api/resources/numbercolumn?view=graph-rest-beta
[NumberColumn]: /graph/api/resources/numbercolumn?view=graph-rest-1.0
[PersonOrGroupColumn-beta]: /graph/api/resources/personorgroupcolumn?view=graph-rest-beta
[PersonOrGroupColumn]: /graph/api/resources/personorgroupcolumn?view=graph-rest-1.0
[Site-beta]: /graph/api/resources/site?view=graph-rest-beta
[Site]: /graph/api/resources/site?view=graph-rest-1.0
[SystemFacet-beta]: /graph/api/resources/systemfacet?view=graph-rest-beta
[SystemFacet]: /graph/api/resources/systemfacet?view=graph-rest-1.0
[TextColumn]: /graph/api/resources/textcolumn?view=graph-rest-1.0


### <a name="sharepoint-sites"></a>SharePoint-Websites

| **Änderungstyp** | **Version** | **Beschreibung**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Ergänzungen        | Beta        | Die Eigenschaften **dataLocationCode** und **root** wurden dem komplexen Typ  [SiteCollection][SiteCollection-beta] hinzugefügt. |

[SiteCollection-beta]: /graph/api/resources/sitecollection?view=graph-rest-beta


## <a name="august-2017"></a>August 2017

### <a name="group-lifecycle-policy"></a>Gruppenlebenszyklusrichtlinie

| **Änderungstyp** | **Version** | **Beschreibung**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Ergänzungen        | Beta        | [groupLifecyclePolicy](/graph/api/resources/grouplifecyclepolicy?view=graph-rest-beta)-Entität hinzugefügt. |
| Ergänzungen        | Beta        | Folgende APIs wurden für Gruppenlebenszyklusrichtlinie hinzugefügt: [create](/graph/api/grouplifecyclepolicy-post-grouplifecyclepolicies?view=graph-rest-beta), [list](/graph/api/grouplifecyclepolicy-list?view=graph-rest-beta), [get](/graph/api/grouplifecyclepolicy-get?view=graph-rest-beta), [update](/graph/api/grouplifecyclepolicy-update?view=graph-rest-beta), [delete](/graph/api/grouplifecyclepolicy-delete?view=graph-rest-beta), [add group](/graph/api/grouplifecyclepolicy-addgroup?view=graph-rest-beta), [remove group](/graph/api/grouplifecyclepolicy-removegroup?view=graph-rest-beta) und [renew a group](/graph/api/grouplifecyclepolicy-renewgroup?view=graph-rest-beta). |
| Ergänzung        | Beta        | [List groupLifecylePolicies](/graph/api/group-list-grouplifecyclepolicies?view=graph-rest-beta)-Funktion zur [group](/graph/api/resources/group?view=graph-rest-beta)-Entität hinzugefügt. |

### <a name="intune-apis"></a>Intune APIs
| Änderungstyp | Version | Beschreibung                              |
| :---------- | :------ | :--------------------------------------- |
| Ergänzungen    | Beta    | Neue Entität hinzugefügt:<br/>[windowsPrivacyDataAccessControlItem](/graph/api/resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem?view=graph-rest-beta)<br/> |
| Ergänzung    | Beta    | Neue komplexe Typen hinzugefügt:<br/>[configurationManagerClientEnabledFeatures](/graph/api/resources/intune-devices-configurationmanagerclientenabledfeatures?view=graph-rest-beta)<br/>[windowsDefenderScanActionResult](/graph/api/resources/intune-devices-windowsdefenderscanactionresult?view=graph-rest-beta)<br/> |
| Ergänzung    | Beta    | Aktion [windowsDefenderScan](/graph/api/intune-devices-manageddevice-windowsdefenderscan?view=graph-rest-beta) für [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) hinzugefügt. |
| Ergänzung    | Beta    | Aktion [windowsDefenderUpdateSignatures](/graph/api/intune-devices-manageddevice-windowsdefenderupdatesignatures?view=graph-rest-beta) für [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) hinzugefügt. |
| Ergänzung    | Beta    | Aktion [windowsPrivacyAccessControls](/graph/api/intune-deviceconfig-deviceconfiguration-windowsprivacyaccesscontrols?view=graph-rest-beta) für [deviceConfiguration](/graph/api/resources/intune-deviceconfig-deviceconfiguration?view=graph-rest-beta) hinzugefügt. |
| Änderung      | Beta    | Eigenschaft **automaticallyUpdateApps** und Eigenschaft **countryOrRegion** zur Entität [appleVolumePurchaseProgramToken](/graph/api/resources/intune-apps-applevolumepurchaseprogramtoken?view=graph-rest-beta) hinzugefügt. |
| Änderung      | Beta    | Eigenschaft **enableAuthenticationViaCompanyPortal** zur Entität [depEnrollmentProfile](/graph/api/resources/intune-corpenrollment-depenrollmentprofile?view=graph-rest-beta) hinzugefügt. |
| Änderung      | Beta    | Eigenschaft **notificationMessageCCList** zur Entität [deviceComplianceActionItem](/graph/api/resources/intune-deviceconfig-devicecomplianceactionitem?view=graph-rest-beta) hinzugefügt. |
| Änderung      | Beta    | Eigenschaft **notApplicableCount** zur Entität [deviceComplianceDeviceOverview](/graph/api/resources/intune-deviceconfig-devicecompliancedeviceoverview?view=graph-rest-beta) hinzugefügt. |
| Änderung      | Beta    | Eigenschaft **notApplicableCount** zur Entität [deviceComplianceUserOverview](/graph/api/resources/intune-deviceconfig-devicecomplianceuseroverview?view=graph-rest-beta) hinzugefügt. |
| Änderung      | Beta    | Eigenschaft **notApplicableCount** zur Entität [deviceConfigurationDeviceOverview](/graph/api/resources/intune-deviceconfig-deviceconfigurationdeviceoverview?view=graph-rest-beta) hinzugefügt. |
| Änderung      | Beta    | Eigenschaft **notApplicableCount** zur Entität [deviceConfigurationUserOverview](/graph/api/resources/intune-deviceconfig-deviceconfigurationuseroverview?view=graph-rest-beta) hinzugefügt. |
| Änderung      | Beta    | Eigenschaft **configurationManagerClientEnabledFeatures** zur Entität [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) hinzugefügt. |
| Änderung      | Beta    | Eigenschaft **intuneBrand** aus der Entität [organization](/graph/api/resources/intune-onboarding-organization?view=graph-rest-beta) entfernt. |
| Änderung      | Beta    | Eigenschaften **smartScreenEnableInShell**, **smartScreenBlockOverrideForFiles**, **applicationGuardEnabled**, **applicationGuardBlockFileTransfer**, **applicationGuardBlockNonEnterpriseContent**, **applicationGuardAllowPersistence** und **applicationGuardForceAuditing** zur Entität [windows10EndpointProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windows10endpointprotectionconfiguration?view=graph-rest-beta) hinzugefügt. |
| Änderung      | Beta    | Eigenschaften **searchBlockDiacritics**, **searchDisableAutoLanguageDetection**, **searchDisableIndexingEncryptedItems**, **searchEnableRemoteQueries**, **searchDisableUseLocation**, **searchDisableIndexerBackoff**, **searchDisableIndexingRemovableDrive**, **searchEnableAutomaticIndexSizeManangement**, **smartScreenEnableAppInstallControl** und **privacyAdvertisingId** zur Entität [windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta) hinzugefügt. |
| Änderung      | Beta    | Eigenschaft **settingsDeviceName** aus der Entität [windows10TeamGeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10teamgeneralconfiguration?view=graph-rest-beta) entfernt. |
| Änderung      | Beta    | Eigenschaft **restartMode** aus der Entität [windowsUpdateForBusinessConfiguration](/graph/api/resources/intune-deviceconfig-windowsupdateforbusinessconfiguration?view=graph-rest-beta) entfernt. |
| Änderung      | Beta    | Navigationseigenschaften **detectedApps** und **managedDevices** zur Entität [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta) hinzugefügt. |
| Änderung      | Beta    | Navigationseigenschaft **privacyAccessControls** zur Entität [windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta) hinzugefügt. |
| Änderung      | Beta    | Eigenschaft **secureByDefault** zum komplexen Typ [deviceManagementSettings](/graph/api/resources/intune-deviceconfig-devicemanagementsettings?view=graph-rest-beta) hinzugefügt. |
| Änderung      | Beta    | Eigenschaft **restartMode** zum komplexen Typ [windowsUpdateScheduledInstall](/graph/api/resources/intune-deviceconfig-windowsupdatescheduledinstall?view=graph-rest-beta) hinzugefügt. |

### <a name="onenote"></a>OneNote

| **Änderungstyp** | **Version**   | **Beschreibung**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Ergänzungen        | v1.0 und Beta | Die Navigationseigenschaft [onenote](/graph/api/resources/onenote?view=graph-rest-1.0) wurde zu **site** hinzugefügt. |
| Ergänzungen        | Beta          | Die Zielparameter *siteCollectionId* und *siteId* für Kopiervorgänge. Beispiel: [CopyNotebook](/graph/api/notebook-copynotebook?view=graph-rest-1.0). |

### <a name="people"></a>Personen

| **Änderungstyp** | **Version** | **Beschreibung**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Ergänzungen        | v1.0        | [Personen-APIs](/graph/api/resources/person?view=graph-rest-1.0) zu v1.0 hinzugefügt. Weitere Informationen zur Personen-API finden Sie unter [Abrufen von relevanten Informationen über Personen](people-example.md). |
| Ergänzungen        | v1.0        | Added People.Read.All permission. To learn more, please see [Permissions](permissions-reference.md). |
| Ergänzungen        | v1.0        | Die Ressource [personType](/graph/api/resources/persontype?view=graph-rest-1.0) wurde hinzugefügt. |
| Änderung          | v1.0        | Die Ressource [scoredEmailAddress](/graph/api/resources/scoredemailaddress?view=graph-rest-1.0) ersetzt die Ressource **rankedEmailAddress**. |
| Änderung          | v1.0        | Die Ressource [person](/graph/api/resources/person?view=graph-rest-1.0) wurde folgendermaßen aktualisiert:<ul><li>Die Eigenschaft **scoredEmailAddresses** (eine Sammlung des Typs [scoredEmailAddress](/graph/api/resources/scoredemailaddress?view=graph-rest-1.0)) ersetzt die Eigenschaft **emailAddresses**.</li><li>Die Eigenschaft **jobTitle** ersetzt die Eigenschaft **title**.</li><li>Die Eigenschaften **sources** und **mailboxType** wurden entfernt.</li><li>Die Eigenschaft **personType** weist nun  den Typ [personType](/graph/api/resources/persontype?view=graph-rest-1.0) und nicht mehr den Zeichenfolgetyp auf und ersetzt die Funktion der vorherigen **sources**- und **mailboxType**-Eigenschaften.</li><li>Die Eigenschaft **imAddress** wurde hinzugefügt.</li></ul> |
| Löschung        | v1.0        | Die Ressource **personDataSource** wurde entfernt. |

### <a name="user"></a>Benutzer

| **Änderungstyp** | **Version** | **Beschreibung**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Ergänzungen        | Beta        | Die **employeeId**-Eigenschaft wurde zu [user](/graph/api/resources/user?view=graph-rest-beta) hinzugefügt. |

## <a name="july-2017"></a>Juli 2017

### <a name="group-settings"></a>Gruppeneinstellungen

| **Änderungstyp** | **Version** | **Beschreibung**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Ergänzungen        | v1.0        | Unterstützung für Gruppeneinstellungen wurde hinzugefügt.<br/>Neue Ressourcentypen: [groupSetting](/graph/api/resources/groupsetting?view=graph-rest-1.0), [groupSettingTemplate](/graph/api/resources/groupsettingtemplate?view=graph-rest-1.0), [settingValue](/graph/api/resources/settingvalue?view=graph-rest-1.0) und [settingTemplateValue](/graph/api/resources/settingtemplatevalue?view=graph-rest-1.0) |
| Änderung          | v1.0        | Eigenschaft **classification** und Navigationseigenschaft **settings** wurden zu [group](/graph/api/resources/group?view=graph-rest-1.0) hinzugefügt. |

### <a name="intune-apis"></a>Intune APIs

| Typ&nbsp;ändern | Version | Beschreibung                              |
| :--------------- | :------ | :--------------------------------------- |
| Ergänzungen         | Beta    | Die [assign](/graph/api/intune-apps-iosmobileappconfiguration-assign?view=graph-rest-beta)-Aktion wurde zu [iosMobileAppConfiguration](/graph/api/resources/intune-apps-iosmobileappconfiguration?view=graph-rest-beta) hinzugefügt. |
| Ergänzungen         | Beta    | Die [syncDevice](/graph/api/intune-devices-manageddevice-syncdevice?view=graph-rest-beta)-Aktion wurde zu [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) hinzugefügt. |
| Änderung           | Beta    | Die Eigenschaften **appsInstallAllowList**, **appsLaunchBlockList** und **appsHideList** wurden zur Entität [androidGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidgeneraldeviceconfiguration?view=graph-rest-beta) hinzugefügt. |
| Änderung           | Beta    | Die Eigenschaft **disableAppEncryptionIfDeviceEncryptionIsEnabled** wurde zur Entität [androidManagedAppProtection](/graph/api/resources/intune-mam-androidmanagedappprotection?view=graph-rest-beta) hinzugefügt. |
| Änderung           | Beta    | Die Eigenschaft **disableAppEncryptionIfDeviceEncryptionIsEnabled** wurde zur Entität [defaultManagedAppProtection](/graph/api/resources/intune-mam-defaultmanagedappprotection?view=graph-rest-beta) hinzugefügt. |
| Änderung           | Beta    | Die Eigenschaft **complianceGracePeriodExpirationDateTime** wurde zur Entität [deviceComplianceDeviceStatus](/graph/api/resources/intune-deviceconfig-devicecompliancedevicestatus?view=graph-rest-beta) hinzugefügt. |
| Änderung           | Beta    | Die Eigenschaft **complianceGracePeriodExpirationDateTime** wurde zur Entität [deviceComplianceSettingState](/graph/api/resources/intune-deviceconfig-devicecompliancesettingstate?view=graph-rest-beta) hinzugefügt. |
| Änderung           | Beta    | Die Eigenschaft **complianceGracePeriodExpirationDateTime** wurde zur Entität [deviceConfigurationDeviceStatus](/graph/api/resources/intune-deviceconfig-deviceconfigurationdevicestatus?view=graph-rest-beta) hinzugefügt. |
| Änderung           | Beta    | Die Eigenschaft **subscriptions** wurde zur Entität [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta) hinzugefügt. |
| Änderung           | Beta    | Die Eigenschaft **version** wurde zur Entität [deviceManagementExchangeConnector](/graph/api/resources/intune-onboarding-devicemanagementexchangeconnector?view=graph-rest-beta) hinzugefügt. |
| Änderung           | Beta    | Die Eigenschaft **utcTimeOffsetInMinutes** wurde zur Entität [iosUpdateConfiguration](/graph/api/resources/intune-deviceconfig-iosupdateconfiguration?view=graph-rest-beta) hinzugefügt. |
| Änderung           | Beta    | Die Eigenschaft **complianceGracePeriodExpirationDateTime** wurde zur Entität [iosUpdateDeviceStatus](/graph/api/resources/intune-deviceconfig-iosupdatedevicestatus?view=graph-rest-beta) hinzugefügt. |
| Änderung           | Beta    | Die Eigenschaft **preSharedKey** wurde zur Entität [macOSWiFiConfiguration](/graph/api/resources/intune-deviceconfig-macoswificonfiguration?view=graph-rest-beta) hinzugefügt. |
| Änderung           | Beta    | Die Eigenschaften **phoneNumber**, **androidSecurityPatchLevel** und **userDisplayName** wurden zur Entität [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) hinzugefügt. |
| Änderung           | Beta    | Die Eigenschaften **userName**, **deviceModel**, **platform** und **complianceGracePeriodExpirationDateTime** wurden zur Entität [managedDeviceMobileAppConfigurationDeviceStatus](/graph/api/resources/intune-apps-manageddevicemobileappconfigurationdevicestatus?view=graph-rest-beta) hinzugefügt. |
| Änderung           | Beta    | Die Eigenschaft **userPrincipalName** wurde zur Entität [mobileAppInstallStatus](/graph/api/resources/intune-apps-mobileappinstallstatus?view=graph-rest-beta) hinzugefügt. |
| Änderung           | Beta    | Die Eigenschaft **overrideDefaultRule** wurde zur Entität [onPremisesConditionalAccessSettings](/graph/api/resources/intune-onboarding-onpremisesconditionalaccesssettings?view=graph-rest-beta) hinzugefügt. |
| Änderung           | Beta    | Die Eigenschaft **userPrincipalName** wurde zur Entität [userAppInstallStatus](/graph/api/resources/intune-apps-userappinstallstatus?view=graph-rest-beta) hinzugefügt. |
| Änderung           | Beta    | Die Eigenschaften **connectAppBlockAutoLaunch**, **deviceAccountBlockExchangeServices**, **deviceAccountEmailAddress**, **deviceAccountExchangeServerAddress**, **deviceAccountRequirePasswordRotation**, **deviceAccountSessionInitiationProtocolAddress**, **settingsBlockMyMeetingsAndFiles**, **settingsBlockSessionResume**, **settingsBlockSigninSuggestions**, **settingsDefaultVolume**, **settingsScreenTimeoutInMinutes**, **settingsSessionTimeoutInMinutes** und **settingsSleepTimeoutInMinutes** wurden zur Entität [windows10TeamGeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10teamgeneralconfiguration?view=graph-rest-beta) hinzugefügt. |
| Änderung           | Beta    | Die Navigationseigenschaft **deploymentSummary** wurde zur Entität [defaultManagedAppProtection](/graph/api/resources/intune-mam-defaultmanagedappprotection?view=graph-rest-beta) hinzugefügt. |
| Änderung           | Beta    | Die Eigenschaften **settingName**, **userId**, **userName**, **userEmail** und **currentValue** wurden zum komplexen Typ [deviceCompliancePolicySettingState](/graph/api/resources/intune-deviceconfig-devicecompliancepolicysettingstate?view=graph-rest-beta) hinzugefügt. |
| Änderung           | Beta    | Die Eigenschaften **settingName**, **userId**, **userName**, **userEmail** und **currentValue** wurden dem komplexen Typ [deviceConfigurationSettingState](/graph/api/resources/intune-deviceconfig-deviceconfigurationsettingstate?view=graph-rest-beta) hinzugefügt. |
| Änderung           | Beta    | Die Eigenschaft **unknownCount** wurde zum komplexen Typ [deviceOperatingSystemSummary](/graph/api/resources/intune-devices-deviceoperatingsystemsummary?view=graph-rest-beta) hinzugefügt. |



## <a name="june-2017"></a>Juni 2017

### <a name="project-rome"></a>Projekt Rom

| **Änderungstyp** | **Version** | **Beschreibung**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Ergänzungen        | Beta        | Folgende Ressourcen und APIs wurden hinzugefügt:<br/>[Aktivität](/graph/api/resources/projectrome-activity?view=graph-rest-beta)<br/>[Aktivität erstellen oder ersetzen](/graph/api/projectrome-put-activity?view=graph-rest-beta)<br/>[Aktivität löschen](/graph/api/projectrome-delete-activity?view=graph-rest-beta)<br/>[Verlaufselement](/graph/api/resources/projectrome-historyitem?view=graph-rest-beta)<br/>[Verlaufselement erstellen oder ersetzen](/graph/api/projectrome-put-historyitem?view=graph-rest-beta)<br/>[Verlaufselement](/graph/api/projectrome-delete-historyitem?view=graph-rest-beta) löschen |

### <a name="outlook-calendar"></a>Outlook-Kalender

| **Änderungstyp** | **Version** | **Beschreibung**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Ergänzungen        | v1.0        | Die folgenden vier [calendar](/graph/api/resources/calendar?view=graph-rest-1.0)-Eigenschaften wurden auf v1.0 heraufgestuft: **canEdit**, **canShare**, **canViewPrivateItems** und **owner**. |


### <a name="intune-apis"></a>Intune APIs

| Änderungstyp | Version | Beschreibung                              |
| :---------- | :------ | :--------------------------------------- |
| Ergänzungen    | Beta    | Hinzugefügte neue Entitäten:<br/>[defaultDeviceCompliancePolicy](/graph/api/resources/intune-deviceconfig-defaultdevicecompliancepolicy?view=graph-rest-beta)<br/>[deviceConfigurationUserStateSummary](/graph/api/resources/intune-deviceconfig-deviceconfigurationuserstatesummary?view=graph-rest-beta)<br/>[deviceManagementScriptDeviceState](/graph/api/resources/intune-devicefe-devicemanagementscriptdevicestate?view=graph-rest-beta)<br/>[deviceManagementScriptRunSummary](/graph/api/resources/intune-devicefe-devicemanagementscriptrunsummary?view=graph-rest-beta)<br/>[deviceManagementScriptUserState](/graph/api/resources/intune-devicefe-devicemanagementscriptuserstate?view=graph-rest-beta)<br/>[iosUpdateDeviceStatus](/graph/api/resources/intune-deviceconfig-iosupdatedevicestatus?view=graph-rest-beta)<br/>[windowsManagedDevice](/graph/api/resources/intune-devicefe-windowsmanageddevice?view=graph-rest-beta)<br/>[windowsManagementAppHealthState](/graph/api/resources/intune-devicefe-windowsmanagementapphealthstate?view=graph-rest-beta)<br/>[windowsManagementAppHealthSummary](/graph/api/resources/intune-devicefe-windowsmanagementapphealthsummary?view=graph-rest-beta)<br/> |
| Ergänzungen    | Beta    | Die folgenden kompleen Typen wurden hinzugefügt:<br/>[bitLockerFixedDrivePolicy](/graph/api/resources/intune-deviceconfig-bitlockerfixeddrivepolicy?view=graph-rest-beta)<br/>[bitLockerRecoveryOptions](/graph/api/resources/intune-deviceconfig-bitlockerrecoveryoptions?view=graph-rest-beta)<br/>[bitLockerRemovableDrivePolicy](/graph/api/resources/intune-deviceconfig-bitlockerremovabledrivepolicy?view=graph-rest-beta)<br/>[deleteUserFromSharedAppleDeviceActionResult](/graph/api/resources/intune-devicefe-deleteuserfromsharedappledeviceactionresult?view=graph-rest-beta)<br/>[iosNetworkUsageRule](/graph/api/resources/intune-deviceconfig-iosnetworkusagerule?view=graph-rest-beta)<br/> |
| Löschung    | Beta    | Die folgenden Entitäten wurden entfernt:<br/>**deviceManagementScriptState**<br/> |
| Löschung    | Beta    | Die Aktion „wipeByDeviceTag“ für [user](/graph/api/resources/intune-devicefe-user?view=graph-rest-beta) wurde entfernt. |
| Änderung      | Beta    | Die Eigenschaften **innerAuthenticationProtocolForEapTtls**, **innerAuthenticationProtocolForPeap** und **outerIdentityPrivacyTemporaryValue** wurden zur Entität [androidEnterpriseWiFiConfiguration](/graph/api/resources/intune-deviceconfig-androidenterprisewificonfiguration?view=graph-rest-beta) hinzugefügt. |
| Änderung      | Beta    | Die Eigenschaften **nonEapAuthenticationMethodForEapTtls**, **nonEapAuthenticationMethodForPeap** und **enableOuterIdentityPrivacy** wurden von der Entität [androidEnterpriseWiFiConfiguration](/graph/api/resources/intune-deviceconfig-androidenterprisewificonfiguration?view=graph-rest-beta) entfernt. |
| Änderung      | Beta    | Hinzugefügt der **DeployedAppCount** -Eigenschaft können Sie die [AndroidManagedAppProtection](/graph/api/resources/intune-mam-androidmanagedappprotection?view=graph-rest-beta) Entität |
| Änderung      | Beta    | Die Eigenschaften **instanceDisplayName** und **settingPlatform** wurden von er Entität [complianceSettingStateSummary](/graph/api/resources/compliancesettingstatesummary?view=graph-rest-beta) entfernt. |
| Änderung      | Beta    | Die Eigenschaft **deployedAppCount** wurde zur Entität [defaultManagedAppProtection](/graph/api/resources/intune-mam-defaultmanagedappprotection?view=graph-rest-beta) hinzugefügt. |
| Änderung      | Beta    | Die **excludeGroup**-Eigenschaft wurde der [deviceCompliancePolicyGroupAssignment](/graph/api/resources/intune-deviceconfig-devicecompliancepolicygroupassignment?view=graph-rest-beta)-Entität hinzugefügt. |
| Änderung      | Beta    | Die Eigenschaften **instanceDisplayName** und **settingPlatform** wurden von der Entität [deviceCompliancePolicySettingStateSummary](/graph/api/resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary?view=graph-rest-beta) entfernt. |
| Änderung      | Beta    | Die Eigenschaft **devicePlatform** wurde von der Entität [deviceComplianceSettingState](/graph/api/resources/intune-deviceconfig-devicecompliancesettingstate?view=graph-rest-beta) entfernt. |
| Änderung      | Beta    | DieEigenschaften **assignmentStatus**, **assignmentProgress** und **assignmentErrorMessage** wurden zur Entität [deviceConfiguration](/graph/api/resources/intune-deviceconfig-deviceconfiguration?view=graph-rest-beta) hinzugefügt. |
| Änderung      | Beta    | Die Eigenschaft **intuneBrand** wurde zur Entität [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta) hinzugefügt. |
| Änderung      | Beta    | Die Eigenschaften **enforceSignatureCheck** und **fileName** wurden zur Entität [deviceManagementScript](/graph/api/resources/intune-devicefe-devicemanagementscript?view=graph-rest-beta) hinzugefügt. |
| Änderung      | Beta    | Die Eigenschaften **innerAuthenticationProtocolForEapTtls** und **outerIdentityPrivacyTemporaryValue** wurden zur Entität [iosEnterpriseWiFiConfiguration](/graph/api/resources/intune-deviceconfig-iosenterprisewificonfiguration?view=graph-rest-beta) hinzugefügt. |
| Änderung      | Beta    | Die Eigenschaften **nonEapAuthenticationMethodForEapTtls** und **enableOuterIdentityPrivacy** wurden von der Entität [iosEnterpriseWiFiConfiguration](/graph/api/resources/intune-deviceconfig-iosenterprisewificonfiguration?view=graph-rest-beta) entfernt. |
| Änderung      | Beta    | Die Eigenschaften **classroomAppForceUnpromptedScreenObservation**, **keyboardBlockDictation**, **networkUsageRules** und **wiFiConnectOnlyToConfiguredNetworks** wurden zur Entität [iosGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-iosgeneraldeviceconfiguration?view=graph-rest-beta) hinzugefügt. |
| Änderung      | Beta    | Die Eigenschaft **deployedAppCount** wurde zur Entität [iosManagedAppProtection](/graph/api/resources/intune-mam-iosmanagedappprotection?view=graph-rest-beta) hinzugefügt. |
| Änderung      | Beta    | Die Eigenschaft **preSharedKey** wurde zur Entität [iosWiFiConfiguration](/graph/api/resources/intune-deviceconfig-ioswificonfiguration?view=graph-rest-beta) hinzugefügt. |
| Änderung      | Beta    | Die Eigenschaften **innerAuthenticationProtocolForEapTtls** und **outerIdentityPrivacyTemporaryValue** wurden zur Entität [macOSEnterpriseWiFiConfiguration](/graph/api/resources/intune-deviceconfig-macosenterprisewificonfiguration?view=graph-rest-beta) hinzugefügt. |
| Änderung      | Beta    | Die Eigenschaften **nonEapAuthenticationMethodForEapTtls** und **enableOuterIdentityPrivacy** wurden von der Entität [macOSEnterpriseWiFiConfiguration](/graph/api/resources/intune-deviceconfig-macosenterprisewificonfiguration?view=graph-rest-beta) entfernt. |
| Änderung      | Beta    | Die Eigenschaften **lastModifiedTime** und **deployedAppCount** wurden aus der Entität [managedAppPolicy](/graph/api/resources/intune-mam-managedapppolicy?view=graph-rest-beta) entfernt. |
| Änderung      | Beta    | Die Eigenschaft **serialNumber** wurde zur Entität [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) hinzugefügt. |
| Änderung      | Beta    | Die Eigenschaft **managementAgents** wurde von der Entität [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) entfernt. |
| Änderung      | Beta    | Die Eigenschaft **deployedAppCount** wurde zur Entität [targetedManagedAppConfiguration](/graph/api/resources/intune-mam-targetedmanagedappconfiguration?view=graph-rest-beta) hinzugefügt. |
| Änderung      | Beta    | Die Eigenschaften **bitLockerFixedDrivePolicy** und **bitLockerRemovableDrivePolicy** wurden zur Entität [windows10EndpointProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windows10endpointprotectionconfiguration?view=graph-rest-beta) hinzugefügt. |
| Änderung      | Beta    | Die Eigenschaften **enterpriseCloudPrintDiscoveryEndPoint**, **enterpriseCloudPrintOAuthAuthority**, **enterpriseCloudPrintOAuthClientIdentifier**, **enterpriseCloudPrintResourceIdentifier**, **enterpriseCloudPrintDiscoveryMaxLimit**, **enterpriseCloudPrintMopriaDiscoveryResourceIdentifier**, **edgeBlockAddressBarDropdown**, **edgeBlockCompatibilityList**, **edgeClearBrowsingDataOnExit**, **edgeAllowStartPagesModification**, **edgeDisableFirstRunPage**, **edgeBlockLiveTileDataCollection** und **edgeSyncFavoritesWithInternetExplorer** wurden zur Entität [windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta) hinzugefügt. |
| Änderung      | Beta    | Die Eigenschaft **availableVersion** wurde zur Entität [windowsManagementApp](/graph/api/resources/intune-devicefe-windowsmanagementapp?view=graph-rest-beta) hinzugefügt. |
| Änderung      | Beta    | Die Eigenschaften **onboardingStatus**, **deployedVersion** und **lastModifiedTime** wurden von der Entität [windowsManagementApp](/graph/api/resources/intune-devicefe-windowsmanagementapp?view=graph-rest-beta) entfernt. |
| Änderung      | Beta    | Die Eigenschaft **packageIdentityName** wurde zur Entität [windowsStoreForBusinessApp](/graph/api/resources/intune-apps-windowsstoreforbusinessapp?view=graph-rest-beta) hinzugefügt. |
| Änderung      | Beta    | Die Navigationseigenschaften **mobileAppIdentifierDeployments** und **deploymentSummary** wurden zur Entität [androidManagedAppProtection](/graph/api/resources/intune-mam-androidmanagedappprotection?view=graph-rest-beta) hinzugefügt. |
| Änderung      | Beta    | Die Navigationseigenschaft **mobileAppIdentifierDeployments** wurde zur Entität [defaultManagedAppProtection](/graph/api/resources/intune-mam-defaultmanagedappprotection?view=graph-rest-beta) hinzugefügt. |
| Änderung      | Beta    | Die Navigationseigenschaften **deviceConfigurationUserStateSummaries** und **iosUpdateStatuses** wurden zur Entität [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta) hinzugefügt. |
| Änderung      | Beta    | Die Navigationseigenschaft **complianceSettingStateSummaries** wurde von der Entität [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta) entfernt. |
| Änderung      | Beta    | Die Navigationseigenschaften **runSummary**, **deviceRunStates** und **userRunStates** wurden zur Entität [deviceManagementScript](/graph/api/resources/intune-devicefe-devicemanagementscript?view=graph-rest-beta) hinzugefügt. |
| Änderung      | Beta    | Die Navigationseigenschaft **runStates** wurde von der Entität [deviceManagementScript](/graph/api/resources/intune-devicefe-devicemanagementscript?view=graph-rest-beta) entfernt. |
| Änderung      | Beta    | Die Navigationseigenschaften **mobileAppIdentifierDeployments** und **deploymentSummary** wurden zur Entität [iosManagedAppProtection](/graph/api/resources/intune-mam-iosmanagedappprotection?view=graph-rest-beta) hinzugefügt. |
| Änderung      | Beta    | Die Navigationseigenschaften **mobileAppIdentifierDeployments** und **deploymentSummary** wurden von der Entität [managedAppPolicy](/graph/api/resources/intune-mam-managedapppolicy?view=graph-rest-beta) entfernt. |
| Änderung      | Beta    | Die Navigationseigenschaften **mobileAppIdentifierDeployments** und **deploymentSummary** wurden zur Entität [targetedManagedAppConfiguration](/graph/api/resources/intune-mam-targetedmanagedappconfiguration?view=graph-rest-beta) hinzugefügt. |
| Änderung      | Beta    | Die Navigationseigenschaften **healthSummary** und **healthStates** wurden zur Entität [windowsManagementApp](/graph/api/resources/intune-devicefe-windowsmanagementapp?view=graph-rest-beta) hinzugefügt. |
| Änderung      | Beta    | Die Eigenschaften **applicationId**, **appName**, **platformId**, **userFailures** und **deviceFailures** wurden dem komplexen Typ [appInstallationFailure](/graph/api/resources/intune-apps-appinstallationfailure?view=graph-rest-beta) hinzugefügt. |
| Änderung      | Beta    | Die Eigenschaften **encryptionMethod**, **startupAuthenticationRequired**, **startupAuthenticationBlockWithoutTpmChip**, **startupAuthenticationTpmUsage**, **startupAuthenticationTpmPinUsage**, **startupAuthenticationTpmKeyUsage**, **startupAuthenticationTpmPinAndKeyUsage**, **recoveryOptions** und **prebootRecoveryEnableMessageAndUrl** wurden dem komplexen Typ [bitLockerSystemDrivePolicy](/graph/api/resources/intune-deviceconfig-bitlockersyst?view=graph-rest-betarivepolicy) hinzugefügt. |
| Änderung      | Beta    | Die Eigenschaften **settingName**, **userId**, **userName**, **userEmail** und **currentValue** wurden vom komplexen Typ [deviceCompliancePolicySettingState](/graph/api/resources/intune-deviceconfig-devicecompliancepolicysettingstate?view=graph-rest-beta) entfernt. |
| Änderung      | Beta    | Die Eigenschaften **settingName**, **userId**, **userName**, **userEmail** und **currentValue** wurden vom komplexen Typ [deviceConfigurationSettingState](/graph/api/resources/intune-deviceconfig-deviceconfigurationsettingstate?view=graph-rest-beta) entfernt. |
| Änderung      | Beta    | Die Eigenschaften **windowsCommercialId** und **windowsCommercialIdLastModifiedTime** wurden dem komplexen Typ [deviceManagementSettings](/graph/api/resources/intune-deviceconfig-devicemanagementsettings?view=graph-rest-beta) hinzugefügt. |
| Änderung      | Beta    | Die Eigenschaft **address** wurde dem komplexen Typ [vpnServer](/graph/api/resources/intune-deviceconfig-vpnserver?view=graph-rest-beta) hinzugefügt. |


## <a name="may-2017"></a>Mai 2017

### <a name="application-api-changes"></a>Änderungen der Anwendungs-API

| **Änderungstyp** | **Version** | **Beschreibung**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Änderung          | Beta        | Update der Anwendungs-API. Dies ist der erste Satz von Änderungen, einschließlich Umbenennung von Eigenschaften und Umstrukturierung der [application](/graph/api/resources/application?view=graph-rest-beta)-Entität.<br/>**Neue Entitäten:** [api](/graph/api/resources/api?view=graph-rest-beta]), [informationalUrl](/graph/api/resources/informationalurl?view=graph-rest-beta), [installedClient](/graph/api/resources/installedclient?view=graph-rest-beta), [permissionScope](/graph/api/resources/permissionscope?view=graph-rest-beta), [preauthorizedApplication](/graph/api/resources/preauthorizedapplication?view=graph-rest-beta), [web](/graph/api/resources/web?view=graph-rest-beta).<br/>**Entfernte Eigenschaften:** addIns, appRoles, availableToOtherOrganizations, knownClientApplications, oauth2AllowUrlPathMatching, recordConsentConditions.<br/>**Umbenannte Eigenschaften:** appId in id, identifierUris in applicationAliases, availableToOtherTenants in orgRestrictions, mainLogo in logo, oauth2Permissions in publishedPermissionsScopes, publicClient in allowPublicClient, replyUrls in redirectUrls.<br/>**Neue Eigenschaften:** tags. |

### <a name="remove-deprecated-planner-api"></a>Entfernung der veralteten Planner-API
| **Änderungstyp** | **Version** | **Beschreibung**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Löschung        | Beta        | Die folgenden Entitäten wurden entfernt:<br/>**task**<br/>**plan**<br/>**bucket**<br/>**taskDetails**<br/>**planDetails**<br/>**taskBoardTaskFormat**<br/>**planTaskBoard** |

### <a name="project-rome"></a>Projekt Rom

| **Änderungstyp** | **Version** | **Beschreibung**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Ergänzungen        | Beta        | Zusätzliche Unterstützung für Projekt Rom, einschließlich [Abrufen einer Liste der Geräte](/graph/api/user-list-devices?view=graph-rest-beta), [Senden eines Befehls an ein Gerät](/graph/api/send-device-command?view=graph-rest-beta), und [Überprüfen des Status eines Befehls](/graph/api/get-device-command-status?view=graph-rest-beta). |
| Ergänzungen        | Beta        | Zusätzliche Unterstützung für Benutzer[aktivitäten](/graph/api/resources/projectrome-activity?view=graph-rest-beta) und [historyItems](/graph/api/resources/projectrome-historyitem?view=graph-rest-beta), einschließlich [upsert-Vorgängen für eine Aktivität](/graph/api/projectrome-put-activity?view=graph-rest-beta) und [upsert-Vorgängen für ein historyItem](/graph/api/projectrome-put-historyitem?view=graph-rest-beta). |

### <a name="administrative-units-property-changes"></a>Eigenschaftsänderungen für administrative Einheiten

| **Änderungstyp** | **Version** | **Beschreibung**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Änderung          | Beta        | Geänderter Eigenschaftentyp roleMemberInfo in [Identität](/graph/api/resources/identity?view=graph-rest-1.0) für die [scopedRoleMembership](/graph/api/resources/scopedrolemembership?view=graph-rest-beta)-Entität |
| Änderung          | Beta        | Geänderte Navigationseigenschaft  scopedAdministratorOf in scopedRoleMemberOf für die [Benutzer](/graph/api/resources/user?view=graph-rest-beta)-Entität |
| Änderung          | Beta        | Geänderte Navigationseigenschaft  scopedAdministrators in scopedRoleMembers für die [administrativeUnit](/graph/api/resources/administrativeunit?view=graph-rest-beta)-Entität |
| Änderung          | Beta        | Geänderte Navigationseigenschaft  scopedAdministrators in scopedMembers für die [directoryRole](/graph/api/resources/directoryrole?view=graph-rest-beta)-Entität |

### <a name="add-users-and-groups-webhook-support-in-preview"></a>Hinzufügen von Benutzern und Gruppen-Webhook-Unterstützung in der Vorschau

|**Änderungstyp**|**Version**|**Beschreibung**|
|:--------------|:-----------|:--------------|
| Änderung        | Beta       | Zusätzliche Unterstützung zu [Webhooks](/graph/api/resources/webhooks?view=graph-rest-beta) für Benutzer und Gruppen.

### <a name="add-delta-query-to-v10"></a>Delta-Abfrage zu v1.0 hinzufügen

| **Änderungstyp** | **Version** | **Beschreibung**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Ergänzungen        | v1.0        | Add delta function support to v1.0. Add to the following entities to perform [delta query](delta-query-overview.md):<br/>contact<br/>contactFolder<br/>event<br/>group<br/>mailFolder<br/>message<br/>user<br/>Beispiele finden Sie unter Folgendem:<br/>[Inkrementelle Änderungen an Gruppen abrufen](delta-query-groups.md)<br/>[Inkrementelle Änderungen an Nachrichten in einem Ordner abrufen](delta-query-messages.md)<br/>[Inkrementelle Änderungen an Benutzern abrufen](delta-query-users.md) |
| Änderung          | Beta        | Hinzufügen von zusätzlicher optionaler Abfrage-Filterfunktion (anhand der Id) zu [Benutzer](/graph/api/user-delta?view=graph-rest-beta) und [Gruppen](/graph/api/group-delta?view=graph-rest-beta). |

### <a name="added-user-resource-support-for-deleted-items"></a>Unterstützung von hinzugefügte Benutzer Ressourcen für gelöschte Elemente

| **Änderungstyp** | **Version** | **Beschreibung**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Ergänzungen        | Beta        | Es wurde Unterstützung zum [Wiederherstellen und endgültigen Löschen von Benutzern](/graph/api/resources/directory?view=graph-rest-beta) hinzugefügt. |

### <a name="added-onpremisesprovisioningerror"></a>Hinzugefügter OnPremisesProvisioningError

| **Änderungstyp** | **Version** | **Beschreibung**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Ergänzungen        | Beta        | Neue Entität: [OnPremisesProvisioningError](/graph/api/resources/onpremisesprovisioningerror?view=graph-rest-beta) |
| Änderung          | Beta        | Hinzugefügte OnPremisesProvisioningError-Eigenschaft zu [Benutzer](/graph/api/resources/user?view=graph-rest-beta), [Gruppe](/graph/api/resources/group?view=graph-rest-beta), und [Organisationskontakt](/graph/api/resources/orgcontact?view=graph-rest-beta) |

### <a name="added-deleteddatetime-property"></a>Hinzugefügte DeletedDateTime-Eigenschaft

|**Änderungstyp**|**Version**|**Beschreibung**|
|:-------------|:-----------|:--------------|
|Änderung|Beta|Hinzugefügte DeletedDateTime-Eigenschaft zu [Benutzer](/graph/api/resources/user?view=graph-rest-beta)-Entität.
|Änderung|Beta|Hinzugefügte DeletedDateTime-Eigenschaft zu [Gruppen](/graph/api/resources/group?view=graph-rest-beta)-Entität.
|Änderung|Beta|Hinzugefügte DeletedDateTime-Eigenschaft zu [App](/graph/api/resources/application?view=graph-rest-beta)-Entität.

### <a name="added-domain-operations-to-v10"></a>Hinzufügte Domänenvorgängen zu v1.0

| **Änderungstyp** | **Version** | **Beschreibung**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Ergänzungen        | v1.0        | Hinzugefügte Vorgänge in [Domänen](/graph/api/resources/domain?view=graph-rest-1.0)<br/>Neue Entitäten:</br>[domain](/graph/api/resources/domain?view=graph-rest-1.0)<br/>[domainDnsRecord](/graph/api/resources/domaindnsrecord?view=graph-rest-1.0)<br/>[domainDnsCnameRecord](/graph/api/resources/domaindnscnamerecord?view=graph-rest-1.0)<br/>[domainDnsMxRecord](/graph/api/resources/domaindnsmxrecord?view=graph-rest-1.0)<br/>[domainDnsSrvRecord](/graph/api/resources/domaindnssrvrecord?view=graph-rest-1.0)<br/>[domainDnsTxtRecord](/graph/api/resources/domaindnstxtrecord?view=graph-rest-1.0)<br/>[domainDnsUnavailableRecord](/graph/api/resources/domaindnsunavailablerecord?view=graph-rest-1.0)<br/>Neue Aktionen:</br>[überprüfen](/graph/api/domain-verify?view=graph-rest-1.0) |

### <a name="added-contracts-to-v10"></a>Hinzugefügte Verträge zu v1.0

| **Änderungstyp** | **Version** | **Beschreibung**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Ergänzungen        | v1.0        | Neue Entität:</br>[Vertrag](/graph/api/resources/contract?view=graph-rest-1.0) |

### <a name="added-licensedetails-to-v10"></a>Hinzugefügte licenseDetails zu v1.0

| **Änderungstyp** | **Version** | **Beschreibung**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Ergänzungen        | v1.0        | Neue Entität:</br>[licenseDetails](/graph/api/resources/licensedetails?view=graph-rest-1.0) |
| Änderung          | v1.0        | Neue [licensedetails](/graph/api/user-list-licensedetails?view=graph-rest-1.0)-Nagivationseigenschaft für [Benutzer](/graph/api/resources/user?view=graph-rest-1.0) |


### <a name="drive-api"></a>Laufwerk-API

|**Änderungstyp**|**Version**|**Beschreibung**|
|:--------------|:----------|:--------------|
| Ergänzungen | v1.0 | **baseItem**-Ressourcentyp hinzugefügt, bestehend aus grundlegenden Eigenschaften aus **driveItem**.
| Ergänzungen | v1.0 und Beta | **sourceItemId**-Eigenschaft zu **Miniaturansicht** hinzugefügt. <br/> **siteUrl**-Eigenschaft zu **sharepointIds** hinzugefügt. <br/> **sharedBy**- und **sharedDateTime**-Eigenschaften zu **shared** hinzugefügt. <br/> **shared**-Eigenschaft zu **remoteItem** hinzugefügt. <br/> **sharepointIds**-Eigenschaft zu **drive** und **itemReference** hinzugefügt. <br/> **lastAccessedDateTime** zu **fileSystemInfo** hinzugefügt. <br/> **driveItem**- und **site**- Navigationseigenschaften zu **sharedDriveItem** hinzugefügt. <br/> **parentReference**-Eigenschaft zu **baseItem** hinzugefügt.
| Änderung | v1.0 und Beta | **driveItem** und **sharedDriveItem** geändert, um **baseItem** zu übernehmen. <br/> Markierte **Identität** als ein offener Typ.
| Änderung | Beta | **configuratorUrl**- und **webHtml**-Eigenschaften zu **sharingLink** hinzugefügt. <br/> **folderView**-Ressourcentyp und die **Ansicht**-Eigenschaft zu **Ordner**-Ressourcentyp hinzugefügt. <br/> **listItem**-Navigationseigenschaft zu **driveItem** hinzugefügt. <br/> **list**-Navigationseigenschaft zu **drive** hinzugefügt.


### <a name="extensions-open-extensions"></a>Erweiterungen (Offene Erweiterungen)

| **Änderungstyp** | **Version**   | **Beschreibung**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Ergänzungen        | v1.0          | Unterstützung für die [openTypeExtension](/graph/api/resources/opentypeextension?view=graph-rest-1.0) in den folgenden Ressourcen – [Gerät](/graph/api/resources/device?view=graph-rest-1.0), [Gruppe](/graph/api/resources/group?view=graph-rest-1.0),[Organisation](/graph/api/resources/organization?view=graph-rest-1.0), [Benutzer](/graph/api/resources/user?view=graph-rest-1.0). |
| Ergänzungen        | v1.0 und Beta | Wenn der Benutzer mit einem persönlichen Microsoft-Konto angemeldet ist, besteht Unterstützung für offene Erweiterungen in den folgenden Ressourcen – Ereignis, Beitrag, Gruppe, Nachricht, Kontakt und Benutzer. (Dies ist zusätzlich zu diesen Ressourcen, plus Gerät, Gruppe, Organisation und Benutzer, geöffnete Erweiterungen werden unterstützt, wenn der Benutzer sich mit einem Firmen- oder Schul-Konto anmeldet.) |
| Ergänzungen        | v1.0 und Beta | Unterstützung für die `$expand`, um [offene Erweiterungen](/graph/api/opentypeextension-get?view=graph-rest-1.0) in den folgenden Ressourcen zu erhalten: [Gerät](/graph/api/resources/device?view=graph-rest-1.0), [Gruppe](/graph/api/resources/group?view=graph-rest-1.0),[Organisation](/graph/api/resources/organization?view=graph-rest-1.0), [Nachricht](/graph/api/resources/post?view=graph-rest-1.0), [Benutzer](/graph/api/resources/user?view=graph-rest-1.0). |
| Ergänzungen        | Beta          | Unterstützung für `$expand` um [offene Erweiterungen](/graph/api/opentypeextension-get?view=graph-rest-1.0) in [administrativeUnit](/graph/api/resources/administrativeunit?view=graph-rest-beta) zu erhalten. |


### <a name="extensions-schema-extensions"></a>Erweiterungen (Schemaerweiterungen)

| **Änderungstyp** | **Version**   | **Beschreibung**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Ergänzungen        | v1.0          | Neue Ressource [schemaExtension](/graph/api/resources/schemaextension?view=graph-rest-1.0) und CRUD-Methoden zum Verwalten von Erweiterungsdefinitionen für die folgenden Ressourcen: [Kontakt](/graph/api/resources/contact?view=graph-rest-1.0), [Gerät](/graph/api/resources/device?view=graph-rest-1.0), [Ereignis](/graph/api/resources/event?view=graph-rest-1.0), [Gruppe](/graph/api/resources/group?view=graph-rest-1.0), [Nachricht](/graph/api/resources/message?view=graph-rest-1.0), [Organisation](/graph/api/resources/organization?view=graph-rest-1.0), [Beitrag](/graph/api/resources/post?view=graph-rest-1.0), [Benutzer](/graph/api/resources/user?view=graph-rest-1.0). Beachten Sie, dass die Unterstützung für [administrativeUnit](/graph/api/resources/administrativeunit?view=graph-rest-beta) wie zuvor noch auf die Betaversion beschränkt ist. |
| Ergänzungen        | v1.0          | Die vorhandenen BEITRAG-, GET- und PATCH-Methoden der folgenden Ressourcen – [Kontakt](/graph/api/resources/contact?view=graph-rest-1.0), [Gerät](/graph/api/resources/device?view=graph-rest-1.0), [Ereignis](/graph/api/resources/event?view=graph-rest-1.0), [Gruppe](/graph/api/resources/group?view=graph-rest-1.0), [Nachricht](/graph/api/resources/message?view=graph-rest-1.0), [Organisation](/graph/api/resources/organization?view=graph-rest-1.0), [Beitrag](/graph/api/resources/post?view=graph-rest-1.0), [Benutzer](/graph/api/resources/user?view=graph-rest-1.0) - unterstützen jetzt Hinzufügen, Abrufen, und Aktualisieren oder Löschen von benutzerdefinierte Daten als Schemaerweiterungen werden in den entsprechenden Ressourceninstanzen gespeichert. |
| Ergänzungen        | v1.0 und Beta | Sie können nun `$filter` verwenden, um nach Ressourceninstanzen mit Eigenschaften zu suchen, die bestimmten Erweiterungsimmobilienwerten, z. B. Erweiterungsnamen entsprechen. Sehen Sie [Beispiel](extensibility-schema-groups.md#5-get-a-group-and-its-extension-data) für Details. |
| Änderung          | v1.0 und Beta | [Schemaerweiterungsdefinition löschen](/graph/api/schemaextension-delete?view=graph-rest-1.0) wird keinen Einfluss mehr auf den Zugriff von benutzerdefinierten Daten haben, die aufgrund dieser Definition hinzugefügt wurden. |
| Änderung          | v1.0 und Beta | Sie können nun einen Schema-Erweiterungskomplextyp auf Null setzen, um eine Schemaerweiterung aus einer Ressourceninstanz zu entfernen. |


### <a name="group"></a>Gruppe

|**Änderungstyp**|**Version**|**Beschreibung**|
|:--------------|:----------|:--------------|
| Ergänzungen | v1.0 und Beta | Die Navigationseigenschaften**drives** und **sites** wurden zu **group** hinzugefügt.

### <a name="insights-apis"></a>Insights-APIs

|**Änderungstyp**|**Version**|**Beschreibung**|
|:-------------|:-----------|:--------------|
|Ergänzungen|Beta|[Freigegebene API](/graph/api/resources/insights-shared?view=graph-rest-beta) wurde hinzugefügt.<br />Neue Ressourcen:<br />[sharingDetail](/graph/api/resources/insights-sharingdetail?view=graph-rest-beta) <br />[insightIdentity](/graph/api/resources/insights-insightidentity?view=graph-rest-beta) <br />
|Ergänzungen|Beta|[Verwendete API](/graph/api/resources/insights-used?view=graph-rest-beta) wurde hinzugefügt.<br />Neue Ressourcen:<br />[usageDetails](/graph/api/resources/insights-usagedetails?view=graph-rest-beta) <br />
|Änderung|Beta|Neue **Type**-Eigenschaft in der:<br />[resourceVisualization](/graph/api/resources/insights-resourcevisualization?view=graph-rest-beta)-Ressource. <br />
|Löschung|Beta|Die folgenden Entitäten wurden entfernt:<br/>**workingWith**<br/>**trendingAround**<br/>|

### <a name="intune-apis"></a>Intune-APIs

| Änderungstyp | Version | Beschreibung                              |
| :---------- | :------ | :--------------------------------------- |
| Ergänzungen    | Beta    | Neue Entitäten hinzugefügt:<br/>[androidForWorkMobileAppConfiguration](/graph/api/resources/intune-apps-androidforworkmobileappconfiguration?view=graph-rest-beta)<br/>[cartToClassAssociation](/graph/api/resources/intune-deviceconfig-carttoclassassociation?view=graph-rest-beta)<br/>[deviceCompliancePolicySettingStateSummary](/graph/api/resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary?view=graph-rest-beta)<br/>[eBookInstallSummary](/graph/api/resources/intune-books-ebookinstallsummary?view=graph-rest-beta)<br/>[eBookVppGroupAssignment](/graph/api/resources/intune-books-ebookvppgroupassignment?view=graph-rest-beta)<br/>[iosUpdateConfiguration](/graph/api/resources/intune-deviceconfig-iosupdateconfiguration?view=graph-rest-beta)<br/>[remoteAssistancePartner](/graph/api/resources/intune-remoteassistance-remoteassistancepartner?view=graph-rest-beta)<br/>[windows10EndpointProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windows10endpointprotectionconfiguration?view=graph-rest-beta)<br/>[windowsDeviceMalwareState](/graph/api/resources/intune-endpointprotection-windowsdevicemalwarestate?view=graph-rest-beta)<br/>[windowsInformationProtectionAppLearningSummary](/graph/api/resources/intune-wip-windowsinformationprotectionapplearningsummary?view=graph-rest-beta)<br/>[windowsMalwareInformation](/graph/api/resources/intune-endpointprotection-windowsmalwareinformation?view=graph-rest-beta)<br/>[windowsProtectionState](/graph/api/resources/intune-endpointprotection-windowsprotectionstate?view=graph-rest-beta)<br/> |
| Ergänzungen    | Beta    | Neue komplexe Typen hinzugefügt:<br/>[androidPermissionAction](/graph/api/resources/intune-apps-androidpermissionaction?view=graph-rest-beta)<br/>[bitLockerSystemDrivePolicy](/graph/api/resources/intune-deviceconfig-bitlockersyst?view=graph-rest-betarivepolicy)<br/>[defenderDetectedMalwareActions](/graph/api/resources/intune-deviceconfig-defenderdetectedmalwareactions?view=graph-rest-beta)<br/>[settingSource](/graph/api/resources/intune-deviceconfig-settingsource?view=graph-rest-beta)<br/> |
| Ergänzungen    | Beta    | Die Aktion [assign](/graph/api/intune-books-managedebook-assign?view=graph-rest-beta) wurde zu [managedEBook](/graph/api/resources/intune-books-managedebook?view=graph-rest-beta) hinzugefügt |
| Ergänzungen    | Beta    | Die Aktion [beginOnboarding](/graph/api/intune-remoteassistance-remoteassistancepartner-beginonboarding?view=graph-rest-beta) wurde zu [remoteAssistancePartner](/graph/api/resources/intune-remoteassistance-remoteassistancepartner?view=graph-rest-beta) hinzugefügt. |
| Ergänzungen    | Beta    | Die Aktion [disconnect](/graph/api/intune-remoteassistance-remoteassistancepartner-disconnect?view=graph-rest-beta) wurde zu [remoteAssistancePartner](/graph/api/resources/intune-remoteassistance-remoteassistancepartner?view=graph-rest-beta) hinzugefügt. |
| Löschung    | Beta    | Die folgenden Entitäten wurden entfernt:<br/>**outlookTask**<br/>**outlookTaskFolder**<br/>**outlookTaskGroup**<br/>**outlookUser**<br/>**windowsManagementAppHealthState**<br/> |
| Löschung    | Beta    | Die folgenden komplexen Typen wurden entfernt:<br/>**applePushNotificationCertificateSetting**<br/>**eventCreationOptions**<br/> |
| Änderung      | Beta    | Die Eigenschaften **workProfilePasswordBlockFingerprintUnlock**, **workProfilePasswordBlockTrustAgents**, **workProfilePasswordExpirationDays**, **workProfilePasswordMinimumLength**, **workProfilePasswordMinutesOfInactivityBeforeScreenTimeout**, **workProfilePasswordPreviousPasswordBlockCount**, **workProfilePasswordSignInFailureCountBeforeFactoryReset**, **workProfilePasswordRequiredType** und **workProfileRequirePassword** wurden der Entität [androidForWorkGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration?view=graph-rest-beta) hinzugefügt. |
| Änderung      | Beta    | Die Eigenschaft **subjectAlternativeNameFormatString** wurde der Entität [androidForWorkPkcsCertificateProfile](/graph/api/resources/intune-deviceconfig-androidforworkpkcscertificateprofile?view=graph-rest-beta) hinzugefügt. |
| Änderung      | Beta    | Die Eigenschaften **subjectAlternativeNameFormatString** und **subjectAlternativeNameFormatString** wurden der Entität [androidForWorkScepCertificateProfile](/graph/api/resources/intune-deviceconfig-androidforworkscepcertificateprofile?view=graph-rest-beta) hinzugefügt. |
| Änderung      | Beta    | Die Eigenschaft **kioskModeManagedApps** wurde der Entität [androidGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidgeneraldeviceconfiguration?view=graph-rest-beta) hinzugefügt. |
| Änderung      | Beta    | Die Eigenschaft **kioskModeManagedAppId** wurde von der Entität [androidGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidgeneraldeviceconfiguration?view=graph-rest-beta) entfernt. |
| Änderung      | Beta    | Die Eigenschaft **subjectAlternativeNameFormatString** wurde der Entität [androidPkcsCertificateProfile](/graph/api/resources/intune-deviceconfig-androidpkcscertificateprofile?view=graph-rest-beta) hinzugefügt. |
| Änderung      | Beta    | Die Eigenschaften **subjectNameFormatString** und **subjectAlternativeNameFormatString** wurden der Entität [androidScepCertificateProfile](/graph/api/resources/intune-deviceconfig-androidscepcertificateprofile?view=graph-rest-beta) hinzugefügt. |
| Änderung      | Beta    | Die Eigenschaft **hexColor** wurde von der Entität [calendar](/graph/api/resources/calendar?view=graph-rest-beta) entfernt. |
| Änderung      | Beta    | Die Eigenschaften **setting** und **platformType** wurden der Entität [complianceSettingStateSummary](/graph/api/resources/intune-deviceconfig-compliancesettingstatesummary?view=graph-rest-beta) hinzugefügt. |
| Änderung      | Beta    | Die Eigenschaft **windowsManagementAppEnabled** wurde von der Entität [deviceAppManagement](/graph/api/resources/intune-apps-deviceappmanagement?view=graph-rest-beta) entfernt. |
| Änderung      | Beta    | Die Eigenschaften **userName**, **deviceModel** und **platform** wurden der Entität [deviceComplianceDeviceStatus](/graph/api/resources/intune-deviceconfig-devicecompliancedevicestatus?view=graph-rest-beta) hinzugefügt. |
| Änderung      | Beta    | Die Eigenschaften **userPrincipalName** und **deviceModel** wurden der Entität [deviceComplianceSettingState](/graph/api/resources/intune-deviceconfig-devicecompliancesettingstate?view=graph-rest-beta) hinzugefügt. |
| Änderung      | Beta    | Die Eigenschaften **platformType**, **setting**, **userId** und **userEmail** wurden der Entität [deviceComplianceSettingState](/graph/api/resources/intune-deviceconfig-devicecompliancesettingstate?view=graph-rest-beta) hinzugefügt. |
| Änderung      | Beta    | Die Eigenschaft **inGracePeriodCount** wurde der Entität [deviceCompliancePolicyDeviceStateSummary](/graph/api/resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary?view=graph-rest-beta) hinzugefügt. |
| Änderung      | Beta    | Die Eigenschaften **userName**, **deviceModel** und **platform** wurden der Entität [deviceConfigurationDeviceStatus](/graph/api/resources/intune-deviceconfig-deviceconfigurationdevicestatus?view=graph-rest-beta) hinzugefügt. |
| Änderung      | Beta    | Die Eigenschaft **creationOptions** wurde von der Entität [event](/graph/api/resources/event?view=graph-rest-beta) entfernt. |
| Änderung      | Beta    | Die Eigenschaft **isDelegated** wurde von derEntität [eventMessage](/graph/api/resources/eventmessage?view=graph-rest-beta) entfernt. |
| Änderung      | Beta    | Die Eigenschaften **unseenConversationsCount** und **unseenMessagesCount** wurden von der Entität [group](/graph/api/resources/group?view=graph-rest-beta) entfernt. |
| Änderung      | Beta    | Die Eigenschaften **settingXml** und **settings** wurden der Entität [iosMobileAppConfiguration](/graph/api/resources/intune-apps-iosmobileappconfiguration?view=graph-rest-beta) hinzugefügt. |
| Änderung      | Beta    | Die Eigenschaft **subjectAlternativeNameFormatString** wurde der Entität [iosPkcsCertificateProfile](/graph/api/resources/intune-deviceconfig-iospkcscertificateprofile?view=graph-rest-beta) hinzugefügt. |
| Änderung      | Beta    | Die Eigenschaft **subjectAlternativeNameFormatString** wurde der Entität [iosScepCertificateProfile](/graph/api/resources/intune-deviceconfig-iosscepcertificateprofile?view=graph-rest-beta) hinzugefügt. |
| Änderung      | Beta    | Die Eigenschaft **systemIntegrityProtectionEnabled** wurde der Entität [macOSCompliancePolicy](/graph/api/resources/intune-deviceconfig-macoscompliancepolicy?view=graph-rest-beta) hinzugefügt. |
| Änderung      | Beta    | Die Eigenschaft **subjectAlternativeNameFormatString** wurde der Entität [macOSScepCertificateProfile](/graph/api/resources/intune-deviceconfig-macosscepcertificateprofile?view=graph-rest-beta) hinzugefügt. |
| Änderung      | Beta    | Die Eigenschaften **complianceGracePeriodExpirationDateTime**, **userPrincipalName** und **imei** wurden der Entität [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) hinzugefügt. |
| Änderung      | Beta    | Die Eigenschaften **settingXml** und **settings** wurden von der Entität [managedDeviceMobileAppConfiguration](/graph/api/resources/intune-apps-manageddevicemobileappconfiguration?view=graph-rest-beta) entfernt. |
| Änderung      | Beta    | Die Eigenschaften **useSharedComputerActivation**, **updateChannel**, **officePlatformArchitecture** und **localesToInstall** wurden der Entität [officeSuiteApp](/graph/api/resources/intune-apps-officesuiteapp?view=graph-rest-beta) hinzugefügt. |
| Änderung      | Beta    | Die Eigenschaft **applePushNotificationCertificateSetting** wurde von der Entität [organization](/graph/api/resources/intune-onboarding-organization?view=graph-rest-beta) entfernt. |
| Änderung      | Beta    | Die folgenden Eigenschaften für die Entität [post](/graph/api/resources/post?view=graph-rest-beta) wurden geändert:<br/>**sender** von „Optional“ in „Erforderlich“<br/> |
| Änderung      | Beta    | Die Eigenschaften **compliantUserCount**, **nonCompliantUserCount**, **remediatedUserCount**, **errorUserCount**, **unknownUserCount**, **conflictUserCount** und **notApplicableUserCount** wurden der Entität [softwareUpdateStatusSummary](/graph/api/resources/intune-deviceconfig-softwareupdatestatussummary?view=graph-rest-beta) hinzugefügt. |
| Änderung      | Beta    | Die Eigenschaften **bluetoothAllowedServices**, **bluetoothBlockPrePairing**, **cellularData**, **defenderDetectedMalwareActions**, **defenderPotentiallyUnwantedAppAction**, **lockScreenAllowTimeoutConfiguration**, **lockScreenBlockCortana**, **lockScreenBlockToastNotifications**, **lockScreenTimeoutInSeconds**, **passwordBlockSimple**, **privacyAutoAcceptPairingAndConsentPrompts**, **privacyBlockInputPersonalization**, **startMenuHideChangeAccountSettings**, **startMenuHideHibernate**, **startMenuHideLock**, **startMenuHideShutDown**, **startMenuHideSignOut**, **startMenuHideSleep**, **startMenuHideSwitchAccount**, **settingsBlockAppsPage**, **settingsBlockGamingPage**, **windowsSpotlightBlockConsumerSpecificFeatures**, **windowsSpotlightBlocked**, **windowsSpotlightBlockOnActionCenter**, **windowsSpotlightBlockTailoredExperiences**, **windowsSpotlightBlockThirdPartyNotifications**, **windowsSpotlightBlockWelcomeExperience**, **windowsSpotlightBlockWindowsTips**, **windowsSpotlightConfigureOnLockScreen** und **connectedDevicesServiceBlocked** wurden der Entität [windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta) hinzugefügt. |
| Änderung      | Beta    | Die Eigenschaften **automaticUpdateMode**, **automaticUpdateSchedule**, **automaticUpdateTime**, **prereleaseFeatures**, **experienceBlockWindowsSpotlight**, **experienceBlockWindowsTips** und **experienceBlockConsumerSpecificFeatures** wurden von der Entität [windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta) entfernt. |
| Änderung      | Beta    | Die Eigenschaft **subjectAlternativeNameFormatString** wurde der Entität [windows10PkcsCertificateProfile](/graph/api/resources/intune-deviceconfig-windows10pkcscertificateprofile?view=graph-rest-beta) hinzugefügt. |
| Änderung      | Beta    | Die Eigenschaften **subjectNameFormatString** und **subjectAlternativeNameFormatString** wurden der Entität [windows81SCEPCertificateProfile](/graph/api/resources/intune-deviceconfig-windows81scepcertificateprofile?view=graph-rest-beta) hinzugefügt. |
| Änderung      | Beta    | Die Eigenschaften **indexingEncryptedStoresOrItemsBlocked** und **smbAutoEncryptedFileExtensions** wurden der Entität [windowsInformationProtection](/graph/api/resources/intune-mam-windowsinformationprotection?view=graph-rest-beta) hinzugefügt. |
| Änderung      | Beta    | Die folgenden Eigenschaften für die Entität [windowsInformationProtection](/graph/api/resources/intune-mam-windowsinformationprotection?view=graph-rest-beta) wurden geändert:<br/>**rightsManagementServicesTemplateId** von „Erforderlich“ in „Optional“<br/> |
| Änderung      | Beta    | Die folgenden Eigenschaften für die Entität [windowsMobileMSI](/graph/api/resources/intune-apps-windowsmobilemsi?view=graph-rest-beta) wurden geändert:<br/>**productCode** von „Erforderlich“ in „Optional“<br/> |
| Änderung      | Beta    | Die Eigenschaften **subjectNameFormatString** und **subjectAlternativeNameFormatString** wurden der Entität [windowsPhone81SCEPCertificateProfile](/graph/api/resources/intune-deviceconfig-windowsphone81scepcertificateprofile?view=graph-rest-beta) hinzugefügt. |
| Änderung      | Beta    | Die Navigationseigenschaft **mobileAppConfigurations** wurde der Entität [deviceAppManagement](/graph/api/resources/intune-apps-deviceappmanagement?view=graph-rest-beta) hinzugefügt. |
| Änderung      | Beta    | Die Navigationseigenschaften **cartToClassAssociations**, **deviceCompliancePolicySettingStateSummaries**, **remoteAssistancePartners**, **windowsInformationProtectionAppLearningSummaries** und **windowsMalwareInformation** wurden der Entität [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta) hinzugefügt. |
| Änderung      | Beta    | Die Navigationseigenschaft **eBook** wurde der Entität [eBookGroupAssignment](/graph/api/resources/intune-books-ebookgroupassignment?view=graph-rest-beta) hinzugefügt. |
| Änderung      | Beta    | Die Navigationseigenschaft **windowsProtectionState** wurde der Entität [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) hinzugefügt. |
| Änderung      | Beta    | Die Navigationseigenschaft **installSummary** wurde der Entität [managedEBook](/graph/api/resources/intune-books-managedebook?view=graph-rest-beta) hinzugefügt. |
| Änderung      | Beta    | Die Navigationseigenschaft **outlook** wurde von der Entität [user](/graph/api/resources/intune-deviceconfig-user?view=graph-rest-beta) entfernt. |
| Änderung      | Beta    | Die Navigationseigenschaft **healthStates** wurde von der Entität [windowsManagementApp](/graph/api/resources/intune-deviceconfig-windowsmanagementapp?view=graph-rest-beta) entfernt. |
| Änderung      | Beta    | Die Eigenschaft **androidForWorkRestrictions** wurde dem komplexen Typ [defaultDeviceEnrollmentRestrictions](/graph/api/resources/intune-onboarding-defaultdeviceenrollmentrestrictions?view=graph-rest-beta) hinzugefügt. |
| Änderung      | Beta    | Die Eigenschaften **userPrincipalName** und **sources** wurden der Entität [deviceCompliancePolicySettingState](/graph/api/resources/intune-deviceconfig-devicecompliancepolicysettingstate?view=graph-rest-beta) hinzugefügt. |
| Änderung      | Beta    | Die Eigenschaften **userPrincipalName** und **sources** wurden der Entität [deviceConfigurationSettingState](/graph/api/resources/intune-deviceconfig-deviceconfigurationsettingstate?view=graph-rest-beta) hinzugefügt. |
| Änderung      | Beta    | Die Eigenschaften **settingName**, **userId**, **userName**, **userEmail** und **currentValue** wurden dem komplexen Typ [deviceConfigurationSettingState](/graph/api/resources/intune-deviceconfig-deviceconfigurationsettingstate?view=graph-rest-beta) hinzugefügt. |
| Änderung      | Beta    | Die Eigenschaft **archiveFolder** wurde vom komplexen Typ [mailboxSettings](/graph/api/resources/mailboxsettings?view=graph-rest-beta) entfernt. |


### <a name="outlook-calendar"></a>Outlook-Kalender

| **Änderungstyp** | **Version**   | **Beschreibung**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Ergänzungen        | v1.0 und Beta | Für **findMeetingTimes**, neuen Aufzählungswert **uneingeschränkt** hinzugefügt, den Sie als **activityDomain**-Eigenschaft, Teil des **TimeConstraint**- Parameters, spezifizieren. Dies lässt **findMeetingTimes** nach Zeiten suchen, die für die Art der Aktivität geeignet sind, für die Sie planen. Weitere Details im Abschnitt [request body](/graph/api/user-findmeetingtimes?view=graph-rest-1.0#request-body). |
| Ergänzungen        | Beta          | Unterstützung, die einen **event**-Text im Klartext erhält, als Alternative zum Standard-HTML-Format. Siehe [get](/graph/api/event-get?view=graph-rest-beta)- und [list](/graph/api/user-list-events?view=graph-rest-beta)-Ereignisse für Details. |

### <a name="outlook-mail"></a>Outlook-Mail

| **Änderungstyp** | **Version** | **Beschreibung**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Änderung          | Beta        | Unterstützung, die einen **message**-Text im Klartext erhält, als Alternative zum Standard-HTML-Format. Siehe [get](/graph/api/message-get?view=graph-rest-beta)- und [list](/graph/api/user-list-messages?view=graph-rest-beta)-Ereignisse für Details. |


### <a name="outlook-tasks"></a>Outlook-Aufgaben

| **Änderungstyp** | **Version** | **Beschreibung**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Ergänzungen        | Beta        | Neue **Outlook**-Navigationseigenschaft hinzugefügt zu [Benutzer](/graph/api/resources/user?view=graph-rest-beta), um auf Outlook-Aufgaben zuzugreifen. |
| Ergänzungen        | Beta        | Neue Entitäten – [outlookuser](/graph/api/resources/outlookuser?view=graph-rest-beta), [outlookTaskGroup](/graph/api/resources/outlooktaskgroup?view=graph-rest-beta), [outlookTaskFolder](/graph/api/resources/outlooktaskfolder?view=graph-rest-beta), und [outlookTask](/graph/api/resources/outlooktask?view=graph-rest-beta) - und deren Methoden unterstützen, organisieren und zugreifen auf Outlook-Aufgaben. |
| Ergänzung        | Beta        | Outlook-Aufgaben unterstützen Anhänge ([attachment](/graph/api/resources/attachment?view=graph-rest-beta), [fileAttachment](/graph/api/resources/fileattachment?view=graph-rest-beta), [itemAttachment](/graph/api/resources/itemattachment?view=graph-rest-beta) und [referenceAttachment](/graph/api/resources/referenceattachment?view=graph-rest-beta)-Ressourcen). |
| Ergänzungen        | Beta        | Outlook-Aufgaben unterstützen [extended properties](/graph/api/resources/extended-properties-overview?view=graph-rest-beta) ([singleValueLegacyExtendedProperty](/graph/api/resources/singlevaluelegacyextendedproperty?view=graph-rest-beta) und [multiValueLegacyExtendedProperty](/graph/api/resources/multivaluelegacyextendedproperty?view=graph-rest-beta)-Ressourcen). |

### <a name="planner-apis"></a>Planner-APIs

| **Änderungstyp** | **Version** | **Beschreibung**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Ergänzungen        | v1.0        | [Planner-APIs](/graph/api/resources/planner-overview?view=graph-rest-1.0) hinzugefügt<br />Neue Ressourcen:<br />[plannerPlan](/graph/api/resources/plannerplan?view=graph-rest-1.0) <br />[plannerTask](/graph/api/resources/plannertask?view=graph-rest-1.0) <br />[plannerPlanDetails](/graph/api/resources/plannerplandetails?view=graph-rest-1.0) <br />[plannerTaskDetails](/graph/api/resources/plannertaskdetails?view=graph-rest-1.0) <br />[plannerBucket](/graph/api/resources/plannerbucket?view=graph-rest-1.0) <br />[plannerAssignedToTaskBoardTaskFormat](/graph/api/resources/plannerassignedtotaskboardtaskformat?view=graph-rest-1.0) <br />[plannerBucketTaskBoardTaskFormat](/graph/api/resources/plannerbuckettaskboardtaskformat?view=graph-rest-1.0) <br />[plannerProgressTaskBoardTaskFormat](/graph/api/resources/plannerprogresstaskboardtaskformat?view=graph-rest-1.0) |

### <a name="sharepoint-sites"></a>SharePoint-Websites

|**Änderungstyp**|**Version**|**Beschreibung**|
|:--------------|:----------|:--------------|
| Ergänzungen      | v1.0      | Die Website-Ressource ist jetzt im v1.0-Endpunkt erhältlich.<br/> Die **site** und **siteCollection**-Ressourcentypen wurden hinzugefügt.
| Änderung        | Beta      | Das Format des Bezeichners für die **site**-Ressource hat sich geändert. Dies ist eine wichtige Änderung in der Beta-API.
| Entfernt       | Beta      | Die **sharePoint**-Entität aus der Beta-API wurde entfernt. Diese Funktion ist nun über die **sites**-Sammlung erhältlich.

### <a name="sharepoint-lists"></a>SharePoint-Listen

|**Änderungstyp**|**Version**|**Beschreibung**|
|:--------------|:----------|:--------------|
| Änderung | Beta | Entfernt die **sharepoint**-Navigationseigenschaften. Websites werden nun direkt über die **sites**-Navigationseigenschaft abgerufen. <br/> Entfernt die **fieldDefinition**-Ressource. Durch **columnDefinition** ersetzt. <br/> Entfernt die **SiteCollectionId**- und **siteId**-Eigenschaften von **site**. Stattdessen **sharepointIds** verwenden. <br/> Entfernt die **listItemId**-Eigenschaft von **listItem**. Stattdessen **sharepointIds** verwenden. <br/> Die **columnSet**-Eigenschaft von **listItem** zu **fields** umbenannt. <br/> Geänderte **site**-Ressourcen, um den SharePoint-Hostnamen als Teil ihrer ID zu verwenden.
| Ergänzungen | Beta | Die **booleanColumn**-, **calculatedColumn**-, **choiceColumn**-, **dateTimeColumn**-, **lookupColumn**-, **numberColumn**-, **personOrGroupColumn**-, und **textColumn**-Ressourcentypen hinzugefügt. <br/> Die **displayName**-Eigenschaft zu **site** hinzugefügt. <br/> Die **columns**-Navigationseigenschaft zu **site** hinzugefügt. <br/> **list**- und **listItem**- Navigationseigenschaften zu **sharedDriveItem** hinzugefügt. <br/> **sharepointIds**-Eigenschaft zu **list**, **listItem** und **site** hinzugefügt. <br/> **columnDefinition**-Ressourcentyp hinzugefügt.




## <a name="april-2017"></a>April 2017

### <a name="administrative-units-property-changes"></a>Eigenschaftsänderungen für administrative Einheiten

| **Änderungstyp** | **Version** | **Beschreibung**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Änderung          | Beta        | APIs für administrative Einheiten werden in der Vorschau (Beta) aktualisiert. Die erste Gruppe von Änderungen wird am 3. Mai 2017 angewendet. Im Rahmen der Änderungen werden die folgenden Eigenschaften umbenannt:<br />- Komplexer Typ **roleMemberInfo** in komplexen Typ **identity** für die scopedRoleMembership-Entität<br />- Navigationseigenschaft **scopedAdministratorOf** in **scopedRoleMemberOf** für die user-Entität<br />- Navigationseigenschaft **scopedAdministrators** in **scopedRoleMembers** für die administrativeUnit-Entität<br />- Navigationseigenschaft **scopedAdministrators** in **scopedMembers** für die directoryRole-Entität |

### <a name="application-and-serviceprincipal-api-changes"></a>Änderungen an der application- und servicePrincipal-API

| **Änderungstyp** | **Version** | **Beschreibung**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Änderung          | Beta        | Die [application](/graph/api/resources/application?view=graph-rest-beta)- und [servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-beta)-APIs werden in der Vorschau (Beta) aktualisiert. Die erste Gruppe von Änderungen wird am 15. Mai 2017 angewendet. Die Änderungen umfassen Umbenennungen und Umstrukturierungen von Eigenschaften. Einige Eigenschaften (z. B. appRoles und addIns) sind erst verfügbar, wenn die Änderungen abgeschlossen sind. Die Änderungen werden in der Vorschau (Beta) vor der Veröffentlichung in v1.0 veröffentlicht. |

### <a name="added-preview-support-for-cloud-solution-provider-developers"></a>Es wurde Vorschauunterstützung für Entwickler von Cloudlösungsanbietern hinzugefügt.

| **Änderungstyp** | **Version** | **Beschreibung**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Ergänzungen        | Beta        | Es wurden neue Vorschaufunktionen hinzugefügt, damit bereits genehmigte Anwendungen von Cloudlösungsanbieter Microsoft Graph aufrufen. Diese werden in einem neuen [Autorisierungsthema](auth-cloudsolutionprovider.md) beschrieben. |

### <a name="added-onpremises-properties-to-user-entity"></a>Der Benutzerentität wurden onPremises-Eigenschaften hinzugefügt.

| **Änderungstyp** | **Version** | **Beschreibung**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Ergänzungen        | Beta        | Der [user](/graph/api/resources/user?view=graph-rest-beta)-Entität wurden die neuen Eigenschaften onPremises, onPremisesDomainName, OnPremisesSamAccountName und onPremisesUserPrincipalName hinzugefügt. |

### <a name="new-planner-apis-and-an-update-to-the-group-visibility-property"></a>Neue Planner-APIs und ein Update der Eigenschaft für Gruppensichtbarkeit.

| **Änderungstyp** | **Version** | **Beschreibung**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Änderung          | Beta        | **HiddenMembership** wurde als zusätzlicher Wert für die Sichtbarkeitseigenschaft, der [Group](/graph/api/resources/group?view=graph-rest-beta)-Entität hinzugefügt. |
| Ergänzungen        | Beta        | Es wurde eine neue [Planner-API](/graph/api/resources/planner-overview?view=graph-rest-beta) hinzugefügt.<br />Neue Ressourcen:<br />[plannerPlan](/graph/api/resources/plannerplan?view=graph-rest-beta) <br />[plannerTask](/graph/api/resources/plannertask?view=graph-rest-beta) <br />[plannerPlanDetails](/graph/api/resources/plannerplandetails?view=graph-rest-beta) <br />[plannerTaskDetails](/graph/api/resources/plannertaskdetails?view=graph-rest-beta) <br />[plannerBucket](/graph/api/resources/plannerbucket?view=graph-rest-beta) <br />[plannerAssignedToTaskBoardTaskFormat](/graph/api/resources/plannerassignedtotaskboardtaskformat?view=graph-rest-beta) <br />[plannerBucketTaskBoardTaskFormat](/graph/api/resources/plannerbuckettaskboardtaskformat?view=graph-rest-beta) <br />[plannerProgressTaskBoardTaskFormat](/graph/api/resources/plannerprogresstaskboardtaskformat?view=graph-rest-beta) |

### <a name="intune-apis"></a>Intune APIs
| **Änderungstyp** | **Version** | **Beschreibung**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Ergänzungen        | Beta        | Hinzugefügte neue Entitäten:<br/>[androidForWorkCompliancePolicy](/graph/api/resources/intune-deviceconfig-androidforworkcompliancepolicy?view=graph-rest-beta)<br/>[deviceComplianceSettingState](/graph/api/resources/intune-deviceconfig-devicecompliancesettingstate?view=graph-rest-beta)<br/>[deviceInstallState](/graph/api/resources/intune-books-deviceinstallstate?view=graph-rest-beta)<br/>[deviceManagementScript](/graph/api/resources/intune-deviceconfig-devicemanagementscript?view=graph-rest-beta)<br/>[deviceManagementScriptGroupAssignment](/graph/api/resources/intune-deviceconfig-devicemanagementscriptgroupassignment?view=graph-rest-beta)<br/>[deviceManagementScriptState](/graph/api/resources/intune-deviceconfig-devicemanagementscriptstate?view=graph-rest-beta)<br/>[eBookGroupAssignment](/graph/api/resources/intune-books-ebookgroupassignment?view=graph-rest-beta)<br/>[iosVppEBook](/graph/api/resources/intune-books-iosvppebook?view=graph-rest-beta)<br/>[managedEBook](/graph/api/resources/intune-books-managedebook?view=graph-rest-beta)<br/>[userInstallStateSummary](/graph/api/resources/intune-books-userinstallstatesummary?view=graph-rest-beta)<br/>[windowsManagementApp](/graph/api/resources/intune-deviceconfig-windowsmanagementapp?view=graph-rest-beta)<br/>[windowsManagementAppHealthState](/graph/api/resources/intune-deviceconfig-windowsmanagementapphealthstate?view=graph-rest-beta)<br/> |
| Ergänzungen        | Beta        | Die folgenden komplexen Typen wurden hinzugefügt:<br/>[dailySchedule](/graph/api/resources/intune-deviceconfig-dailyschedule?view=graph-rest-beta)<br/>[hourlySchedule](/graph/api/resources/intune-deviceconfig-hourlyschedule?view=graph-rest-beta)<br/>[iosBookmark](/graph/api/resources/intune-deviceconfig-iosbookmark?view=graph-rest-beta)<br/>[iosWebContentFilterAutoFilter](/graph/api/resources/intune-deviceconfig-ioswebcontentfilterautofilter?view=graph-rest-beta)<br/>[iosWebContentFilterBase](/graph/api/resources/intune-deviceconfig-ioswebcontentfilterbase?view=graph-rest-beta)<br/>[iosWebContentFilterSpecificWebsitesAccess](/graph/api/resources/intune-deviceconfig-ioswebcontentfilterspecificwebsitesaccess?view=graph-rest-beta)<br/>[runSchedule](/graph/api/resources/intune-deviceconfig-runschedule?view=graph-rest-beta)<br/>[sharedAppleDeviceUser](/graph/api/resources/intune-deviceconfig-sharedappledeviceuser?view=graph-rest-beta)<br/>[windows10NetworkProxyServer](/graph/api/resources/intune-deviceconfig-windows10networkproxyserver?view=graph-rest-beta)<br/> |
| Ergänzungen        | Beta        | Die [requestRemoteAssistance](/graph/api/intune-devices-manageddevice-requestremoteassistance?view=graph-rest-beta)-Aktion wurde zu [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) hinzugefügt. |
| Ergänzungen        | Beta        | Die [cleanWindowsDevice](/graph/api/intune-devices-manageddevice-cleanwindowsdevice?view=graph-rest-beta)-Aktion wurde zu [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) hinzugefügt. |
| Ergänzungen        | Beta        | Die [logoutSharedAppleDeviceActiveUser](/graph/api/intune-devices-manageddevice-logoutsharedappledeviceactiveuser?view=graph-rest-beta)-Aktion wurde zu [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) hinzugefügt. |
| Ergänzungen        | Beta        | Die [deleteUserFromSharedAppleDevice](/graph/api/intune-devices-manageddevice-deleteuserfromsharedappledevice?view=graph-rest-beta)-Aktion wurde zu [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) hinzugefügt. |
| Ergänzungen        | Beta        | Die [assign](/graph/api/intune-deviceconfig-devicemanagementscript-assign?view=graph-rest-beta)-Aktion wurde zu [deviceManagementScript](/graph/api/resources/intune-deviceconfig-devicemanagementscript?view=graph-rest-beta) hinzugefügt. |
| Ergänzungen        | Beta        | Die [syncLicenses](/graph/api/intune-onboarding-applevolumepurchaseprogramtoken-synclicenses?view=graph-rest-beta)-Aktion wurde zu [appleVolumePurchaseProgramToken](/graph/api/resources/intune-apps-applevolumepurchaseprogramtoken?view=graph-rest-beta) hinzugefügt. |
| Ergänzungen        | Beta        | Die **getTopMobileAppCount**-Funktion wurde der [mobileApp](/graph/api/resources/intune-apps-mobileapp?view=graph-rest-beta)-Sammlung hinzugefügt. |
| Ergänzungen        | Beta        | Die [downloadApplePushNotificationCertificateSigningRequest](/graph/api/intune-deviceconfig-applepushnotificationcertificate-downloadapplepushnotificationcertificatesigningrequest?view=graph-rest-beta)-Funktion wurde zu [applePushNotificationCertificate](/graph/api/resources/intune-deviceconfig-applepushnotificationcertificate?view=graph-rest-beta) hinzugefügt. |
| Ergänzungen        | Beta        | Die [getDeviceComplianceSettingStates](/graph/api/intune-deviceconfig-devicemanagement-getdevicecompliancesettingstates?view=graph-rest-beta)-Funktion wurde zu [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta) hinzugefügt. |
| Ergänzungen        | Beta        | Die [deviceConfigurationUserActivity](/graph/api/intune-deviceconfig-reportroot-deviceconfigurationuseractivity?view=graph-rest-beta)-Funktion wurde zu [reportRoot](/graph/api/resources/intune-deviceconfig-reportroot?view=graph-rest-beta) hinzugefügt. |
| Ergänzungen        | Beta        | Die [deviceConfigurationDeviceActivity](/graph/api/intune-deviceconfig-reportroot-deviceconfigurationdeviceactivity?view=graph-rest-beta)-Funktion wurde zu [reportRoot](/graph/api/resources/intune-deviceconfig-reportroot?view=graph-rest-beta) hinzugefügt. |
| Löschung        | Beta        | Die folgenden komplexen Typen wurden entfernt:<br/>**enterpriseCloudResource**<br/>**windowsInformationProtectionAppRule**<br/>**windowsInformationProtectionAppRuleAppLockerPolicyFileTemplate**<br/>**windowsInformationProtectionAppRuleDesktopTemplate**<br/>**windowsInformationProtectionAppRuleStoreAppTemplate**<br/>**windowsInformationProtectionAppRuleTemplate**<br/>**windowsInformationProtectionCorporateNetworkLocation**<br/>**windowsInformationProtectionProtectedLocation**<br/>**windowsInformationProtectionProtectedLocationEnterpriseCloudResources**<br/>**windowsInformationProtectionProtectedLocationEnterpriseInternalProxyServers**<br/>**windowsInformationProtectionProtectedLocationEnterpriseIPv4Ranges**<br/>**windowsInformationProtectionProtectedLocationEnterpriseIPv6Ranges**<br/>**windowsInformationProtectionProtectedLocationEnterpriseNetworkDomainNames**<br/>**windowsInformationProtectionProtectedLocationEnterpriseProxyServers**<br/>**windowsInformationProtectionProtectedLocationNeutralResources**<br/> |
| Änderung          | Beta        | Die **deviceSharingAllowed**-Eigenschaft wurde der [androidGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidgeneraldeviceconfiguration?view=graph-rest-beta)-Entität hinzugefügt. |
| Änderung          | Beta        | Die **deviceSharingBlocked**-Eigenschaft wurde aus der Entität [androidGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidgeneraldeviceconfiguration?view=graph-rest-beta)-Entität entfernt. |
| Änderung          | Beta        | Die **minimumRequiredSdkVersion**-Eigenschaft wurde der [defaultManagedAppProtection](/graph/api/resources/intune-mam-defaultmanagedappprotection?view=graph-rest-beta)-Entität hinzugefügt. |
| Änderung          | Beta        | Die **windowsManagementAppEnabled**-Eigenschaft wurde der [deviceAppManagement](/graph/api/resources/intune-apps-deviceappmanagement?view=graph-rest-beta)-Entität hinzugefügt. |
| Änderung          | Beta        | Die **notificationTemplateId**-Eigenschaft wurde der [deviceComplianceActionItem](/graph/api/resources/intune-deviceconfig-devicecomplianceactionitem?view=graph-rest-beta)-Entität hinzugefügt. |
| Änderung          | Beta        | Die **excludeGroup**-Eigenschaft wurde der [deviceConfigurationGroupAssignment](/graph/api/resources/intune-deviceconfig-deviceconfigurationgroupassignment?view=graph-rest-beta)-Entität hinzugefügt. |
| Änderung          | Beta        | Die folgenden Eigenschaften in der [iosCustomConfiguration](/graph/api/resources/intune-deviceconfig-ioscustomconfiguration?view=graph-rest-beta)-Entität wurden geändert:<br/>**payloadFileName** von „Erforderlich“ in „Optional“<br/> |
| Änderung          | Beta        | Die **contentFilterSettings**-Eigenschaft wurde der [iosDeviceFeaturesConfiguration](/graph/api/resources/intune-deviceconfig-iosdevicefeaturesconfiguration?view=graph-rest-beta)-Entität hinzugefügt. |
| Änderung          | Beta        | Die Eigenschaften **cellularBlockPersonalHotspot** und **passcodeBlockFingerprintModification** wurden der [iosGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-iosgeneraldeviceconfiguration?view=graph-rest-beta)-Entität hinzugefügt. |
| Änderung          | Beta        | Die **minimumRequiredSdkVersion**-Eigenschaft wurde der [iosManagedAppProtection](/graph/api/resources/intune-mam-iosmanagedappprotection?view=graph-rest-beta)-Entität hinzugefügt. |
| Änderung          | Beta        | Die folgenden Eigenschaften in der [macOSCustomConfiguration](/graph/api/resources/intune-deviceconfig-macoscustomconfiguration?view=graph-rest-beta)-Entität wurden geändert:<br/>**payloadFileName** von „Erforderlich“ in „Optional“<br/> |
| Änderung          | Beta        | Die Eigenschaften **disableAppPinIfDevicePinIsSet**, **minimumRequiredOsVersion**, **minimumWarningOsVersion**, **minimumRequiredAppVersion** und **minimumWarningAppVersion** wurden der [managedAppProtection](/graph/api/resources/intune-mam-managedappprotection?view=graph-rest-beta)-Entität hinzugefügt. |
| Änderung          | Beta        | Die Eigenschaften **remoteAssistanceSessionUrl**, **isEncrypted**, **model** und **manufacturer** wurden der [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta)-Entität hinzugefügt. |
| Änderung          | Beta        | Die folgenden Eigenschaften in der [getMobileAppCount](/graph/api/intune-apps-mobileapp-getmobileappcount?view=graph-rest-beta)-Entität wurden geändert:<br/>**bindingParameter** von **mobileApp** in eine **Sammlung** von *mobileApp*<br/>**status** von einer GUID in eine Zeichenfolge<br/> |
| Änderung          | Beta        | Die **vpnConfigurationId**-Eigenschaft wurde der Entität [mobileAppGroupAssignment](/graph/api/resources/intune-apps-mobileappgroupassignment?view=graph-rest-beta) hinzugefügt. |
| Änderung          | Beta        | Die **fromEmailAddress**-Eigenschaft wurde aus der [mobileAppGroupAssignment](/graph/api/resources/intune-deviceconfig-notificationmessagetemplate?view=graph-rest-beta)-Entität entfernt. |
| Änderung          | Beta        | Die **excludedApps**-Eigenschaft wurde der [officeSuiteApp](/graph/api/resources/intune-apps-officesuiteapp?view=graph-rest-beta)-Entität hinzugefügt. |
| Änderung          | Beta        | Die **excludedOfficeApps**-Eigenschaft wurde aus der [officeSuiteApp](/graph/api/resources/intune-apps-officesuiteapp?view=graph-rest-beta)-Entität entfernt. |
| Änderung          | Beta        | Die **enabled**-Eigenschaft wurde der [sharedPCConfiguration](/graph/api/resources/intune-deviceconfig-sharedpcconfiguration?view=graph-rest-beta)-Entität hinzugefügt. |
| Änderung          | Beta        | Die Eigenschaften **networkProxyApplySettingsDeviceWide**, **networkProxyDisableAutoDetect**, **networkProxyAutomaticConfigurationUrl**, **networkProxyServer**, **bluetoothDeviceName**, **wiFiScanInterval**, **wirelessDisplayBlockProjectionToThisDevice**, **wirelessDisplayBlockUserInputFromReceiver**, **wirelessDisplayRequirePinForPairing**, **experienceBlockDeviceDiscovery**, **experienceBlockErrorDialogWhenNoSIM**, **experienceBlockTaskSwitcher**, **startMenuPinnedFolderDocuments**, **startMenuPinnedFolderDownloads**, **startMenuPinnedFolderFileExplorer**, **startMenuPinnedFolderHomeGroup**, **startMenuPinnedFolderMusic**, **startMenuPinnedFolderNetwork**, **startMenuPinnedFolderPersonalFolder**, **startMenuPinnedFolderPictures**, **startMenuPinnedFolderSettings**, **startMenuPinnedFolderVideos**, **startMenuAppListVisibility**, **startMenuHideFrequentlyUsedApps**, **startMenuHideRecentJumpLists**, **startMenuHideRecentlyAddedApps**, **startMenuHideRestartOptions**, **startMenuHideUserTile**, **startMenuHidePowerButton**, **startMenuLayoutEdgeAssetsXml**, **personalizationDesktopImageUrl** und **personalizationLockScreenImageUrl** wurden der [windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta)-Entität hinzugefügt. |
| Änderung          | Beta        | Der Typ der folgenden Eigenschaften in der [windowsMobileMSI](/graph/api/resources/intune-apps-windowsmobilemsi?view=graph-rest-beta)-Entität wurde geändert:<br/>**productCode** von „GUID“ in „Zeichenfolge“<br/> |
| Änderung          | Beta        | Die folgenden Eigenschaften in der [windowsPhone81AppX](/graph/api/resources/intune-apps-windowsphone81appx?view=graph-rest-beta)-Entität wurden geändert:<br/>**phoneProductIdentifier** von „Erforderlich“ in „Optional“<br/>**phonePublisherId** von „Erforderlich“ in „Optional“<br/> |
| Änderung          | Beta        | Die folgenden Eigenschaften in der [windowsPhone81AppXBundle](/graph/api/resources/intune-apps-windowsphone81appxbundle?view=graph-rest-beta)-Entität wurden geändert:<br/>**appXPackageInformationList** von „Erforderlich“ in „Optional“<br/> |
| Änderung          | Beta        | Die Eigenschaften **productKey** und **licenseType** wurden der [windowsStoreForBusinessApp](/graph/api/resources/intune-apps-windowsstoreforbusinessapp?view=graph-rest-beta)-Entität hinzugefügt. |
| Änderung          | Beta        | Die **previewBuildSetting**-Eigenschaft wurde der [windowsUpdateForBusinessConfiguration](/graph/api/resources/intune-deviceconfig-windowsupdateforbusinessconfiguration?view=graph-rest-beta)-Entität hinzugefügt. |
| Änderung          | Beta        | Die Navigationseigenschaften **windowsManagementApp** und **managedEBooks** wurden der [deviceAppManagement](/graph/api/resources/intune-apps-deviceappmanagement?view=graph-rest-beta)-Entität hinzugefügt. |
| Änderung          | Beta        | Die Navigationseigenschaften **deviceManagementScripts**, **managedDeviceOverview** und **cloudPkiSubscriptions** wurden der [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta)-Entität hinzugefügt. |
| Änderung          | Beta        | Die Eigenschaften **osMinimumVersion** und **osMaximumVersion** wurden dem komplexen Typ [deviceEnrollmentPlatformRestrictions](/graph/api/resources/intune-onboarding-deviceenrollmentplatformrestrictions?view=graph-rest-beta) hinzugefügt. |
| Änderung          | Beta        | Die Eigenschaften **isSharedDevice** und **sharedDeviceCachedUsers** wurden dem komplexen Typ [hardwareInformation](/graph/api/resources/intune-deviceconfig-hardwareinformation?view=graph-rest-beta) hinzugefügt. |
| Änderung          | Beta        | Die folgenden Eigenschaften im komplexen Typ [omaSettingBase64](/graph/api/resources/intune-deviceconfig-omasettingbase64?view=graph-rest-beta) wurden geändert:<br/>**fileName** von „Erforderlich“ in „Optional“<br/> |
| Änderung          | Beta        | Die folgenden Eigenschaften im komplexen Typ [omaSettingStringXml](/graph/api/resources/intune-deviceconfig-omasettingstringxml?view=graph-rest-beta) wurden geändert:<br/>**fileName** von „Erforderlich“ in „Optional“<br/> |

## <a name="march-2017"></a>März 2017

### <a name="intune-apis"></a>Intune APIs

| Änderungstyp | Version | Beschreibung                              |
| :---------- | :------ | :--------------------------------------- |
| Ergänzungen    | Beta    | Hinzugefügte neue Entitäten:<br/>[androidForWorkApp](/graph/api/resources/intune-apps-androidforworkapp?view=graph-rest-beta)<br/>[androidForWorkAppConfigurationSchema](/graph/api/resources/intune-androidforwork-androidforworkappconfigurationschema?view=graph-rest-beta)<br/>[androidForWorkSettings](/graph/api/resources/intune-androidforwork-androidforworksettings?view=graph-rest-beta)<br/>[androidForWorkVpnConfiguration](/graph/api/resources/intune-deviceconfig-androidforworkvpnconfiguration?view=graph-rest-beta)<br/>[applePushNotificationCertificate](/graph/api/resources/intune-deviceconfig-applepushnotificationcertificate?view=graph-rest-beta)<br/>[complianceSettingStateSummary](/graph/api/resources/intune-deviceconfig-compliancesettingstatesummary?view=graph-rest-beta)<br/>[deviceCompliancePolicyDeviceStateSummary](/graph/api/resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary?view=graph-rest-beta)<br/>[deviceCompliancePolicyState](/graph/api/resources/intune-deviceconfig-devicecompliancepolicystate?view=graph-rest-beta)<br/>[deviceConfigurationDeviceStateSummary](/graph/api/resources/intune-deviceconfig-deviceconfigurationdevicestatesummary?view=graph-rest-beta)<br/>[deviceConfigurationState](/graph/api/resources/intune-deviceconfig-deviceconfigurationstate?view=graph-rest-beta)<br/>[enterpriseCodeSigningCertificate](/graph/api/resources/intune-apps-enterprisecodesigningcertificate?view=graph-rest-beta)<br/>[iosEduDeviceConfiguration](/graph/api/resources/intune-deviceconfig-iosedudeviceconfiguration?view=graph-rest-beta)<br/>[managedDeviceCertificateState](/graph/api/resources/intune-devices-manageddevicecertificatestate?view=graph-rest-beta)<br/>[managedDeviceMobileAppConfigurationDeviceSummary](/graph/api/resources/intune-apps-manageddevicemobileappconfigurationdevicesummary?view=graph-rest-beta)<br/>[managedDeviceMobileAppConfigurationUserSummary](/graph/api/resources/intune-apps-manageddevicemobileappconfigurationusersummary?view=graph-rest-beta)<br/>[mdmWindowsInformationProtectionPolicy](/graph/api/resources/intune-mam?view=graph-rest-betamwindowsinformationprotectionpolicy)<br/>[mobileAppInstallSummary](/graph/api/resources/intune-apps-mobileappinstallsummary?view=graph-rest-beta)<br/>[mobileAppProvisioningConfigGroupAssignment](/graph/api/resources/intune-apps-mobileappprovisioningconfiggroupassignment?view=graph-rest-beta)<br/>[mobileThreatDefenseConnector](/graph/api/resources/intune-onboarding-mobilethreatdefenseconnector?view=graph-rest-beta)<br/>[officeSuiteApp](/graph/api/resources/intune-apps-officesuiteapp?view=graph-rest-beta)<br/>[settingStateDeviceSummary](/graph/api/resources/intune-deviceconfig-settingstatedevicesummary?view=graph-rest-beta)<br/>[softwareUpdateStatusSummary](/graph/api/resources/intune-deviceconfig-softwareupdatestatussummary?view=graph-rest-beta)<br/>[symantecCodeSigningCertificate](/graph/api/resources/intune-apps-symanteccodesigningcertificate?view=graph-rest-beta)<br/>[windowsDefenderAdvancedThreatProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration?view=graph-rest-beta)<br/>[windowsInformationProtection](/graph/api/resources/intune-mam-windowsinformationprotection?view=graph-rest-beta)<br/>[windowsInformationProtectionAppLockerFile](/graph/api/resources/intune-mam-windowsinformationprotectionapplockerfile?view=graph-rest-beta)<br/>[windowsInformationProtectionPolicy](/graph/api/resources/intune-mam-windowsinformationprotectionpolicy?view=graph-rest-beta)<br/>[windowsMobileMSI](/graph/api/resources/intune-apps-windowsmobilemsi?view=graph-rest-beta)<br/> |
| Ergänzungen    | Beta    | Die folgenden komplexen Typen wurden hinzugefügt:<br/>[androidForWorkAppConfigurationExample](/graph/api/resources/intune-androidforwork-androidforworkappconfigurationexample?view=graph-rest-beta)<br/>[androidForWorkAppConfigurationExampleJson](/graph/api/resources/intune-androidforwork-androidforworkappconfigurationexamplejson?view=graph-rest-beta)<br/>[androidForWorkAppConfigurationSchemaItem](/graph/api/resources/intune-androidforwork-androidforworkappconfigurationschemaitem?view=graph-rest-beta)<br/>[deviceCompliancePolicySettingState](/graph/api/resources/intune-deviceconfig-devicecompliancepolicysettingstate?view=graph-rest-beta)<br/>[deviceConfigurationSettingState](/graph/api/resources/intune-deviceconfig-deviceconfigurationsettingstate?view=graph-rest-beta)<br/>[deviceExchangeAccessStateSummary](/graph/api/resources/intune-deviceconfig-deviceexchangeaccessstatesummary?view=graph-rest-beta)<br/>[edgeSearchEngine](/graph/api/resources/intune-deviceconfig-edgesearchengine?view=graph-rest-beta)<br/>[edgeSearchEngineBase](/graph/api/resources/intune-deviceconfig-edgesearchenginebase?view=graph-rest-beta)<br/>[edgeSearchEngineCustom](/graph/api/resources/intune-deviceconfig-edgesearchenginecustom?view=graph-rest-beta)<br/>[excludedApps](/graph/api/resources/intune-apps-excludedapps?view=graph-rest-beta)<br/>[iosEduCertificateSettings](/graph/api/resources/intune-deviceconfig-ioseducertificatesettings?view=graph-rest-beta)<br/>[ipRange](/graph/api/resources/intune-deviceconfig-iprange?view=graph-rest-beta)<br/>[windowsInformationProtectionApp](/graph/api/resources/intune-mam-windowsinformationprotectionapp?view=graph-rest-beta)<br/>[windowsInformationProtectionCloudResource](/graph/api/resources/intune-mam-windowsinformationprotectioncloudresource?view=graph-rest-beta)<br/>[windowsInformationProtectionCloudResourceCollection](/graph/api/resources/intune-mam-windowsinformationprotectioncloudresourcecollection?view=graph-rest-beta)<br/>[windowsInformationProtectionDesktopApp](/graph/api/resources/intune-mam-windowsinformationprotectiondesktopapp?view=graph-rest-beta)<br/>[windowsInformationProtectionIPRangeCollection](/graph/api/resources/intune-mam-windowsinformationprotectioniprangecollection?view=graph-rest-beta)<br/>[windowsInformationProtectionResourceCollection](/graph/api/resources/intune-mam-windowsinformationprotectionresourcecollection?view=graph-rest-beta)<br/>[windowsInformationProtectionStoreApp](/graph/api/resources/intune-mam-windowsinformationprotectionstoreapp?view=graph-rest-beta)<br/> |
| Ergänzungen    | Beta    | Die [requestSignupUrl](/graph/api/intune-androidforwork-androidforworksettings-requestsignupurl?view=graph-rest-beta)-Aktion wurde zu [androidForWorkSettings](/graph/api/resources/intune-androidforwork-androidforworksettings?view=graph-rest-beta) hinzugefügt. |
| Ergänzungen    | Beta    | Die [completeSignup](/graph/api/intune-androidforwork-androidforworksettings-completesignup?view=graph-rest-beta)-Aktion wurde zu [androidForWorkSettings](/graph/api/resources/intune-androidforwork-androidforworksettings?view=graph-rest-beta) hinzugefügt. |
| Ergänzungen    | Beta    | Die [syncApps](/graph/api/intune-androidforwork-androidforworksettings-syncapps?view=graph-rest-beta)-Aktion wurde zu [androidForWorkSettings](/graph/api/resources/intune-androidforwork-androidforworksettings?view=graph-rest-beta) hinzugefügt. |
| Ergänzungen    | Beta    | Die [unbind](/graph/api/intune-androidforwork-androidforworksettings-unbind?view=graph-rest-beta)-Aktion wurde zu [androidForWorkSettings](/graph/api/resources/intune-androidforwork-androidforworksettings?view=graph-rest-beta) hinzugefügt. |
| Ergänzungen    | Beta    | Die [assign](/graph/api/intune-apps-ioslobappprovisioningconfiguration-assign?view=graph-rest-beta)-Aktion wurde zu [iosLobAppProvisioningConfiguration](/graph/api/resources/intune-apps-ioslobappprovisioningconfiguration?view=graph-rest-beta) hinzugefügt. |
| Ergänzungen    | Beta    | Die [recoverPasscode](/graph/api/intune-devices-manageddevice-recoverpasscode?view=graph-rest-beta)-Aktion wurde zu [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) hinzugefügt. |
| Ergänzungen    | Beta    | Die [removeApplePushNotificationCertificate](/graph/api/intune-onboarding-organization-removeapplepushnotificationcertificate?view=graph-rest-beta)-Aktion wurde zu [organization](/graph/api/resources/intune-onboarding-organization?view=graph-rest-beta) hinzugefügt. |
| Ergänzungen    | Beta    | Die [updateMobileAppIdentifierDeployments](/graph/api/intune-mam-iosmanagedappprotection-updatemobileappidentifierdeployments?view=graph-rest-beta)-Aktion wurde zu [osManagedAppProtection](/graph/api/resources/intune-mam-iosmanagedappprotection?view=graph-rest-beta) hinzugefügt. |
| Ergänzungen    | Beta    | Die [updateMobileAppIdentifierDeployments](/graph/api/intune-mam-androidmanagedappprotection-updatemobileappidentifierdeployments?view=graph-rest-beta)-Aktion wurde zu [androidManagedAppProtection](/graph/api/resources/intune-mam-androidmanagedappprotection?view=graph-rest-beta) hinzugefügt. |
| Ergänzungen    | Beta    | Die [updateMobileAppIdentifierDeployments](/graph/api/intune-mam-targetedmanagedappconfiguration-updatemobileappidentifierdeployments?view=graph-rest-beta)-Aktion wurde zu [targetedManagedAppConfiguration](/graph/api/resources/intune-mam-targetedmanagedappconfiguration?view=graph-rest-beta) hinzugefügt. |
| Ergänzungen    | Beta    | Die [updateTargetedSecurityGroups](/graph/api/intune-mam-iosmanagedappprotection-updatetargetedsecuritygroups?view=graph-rest-beta)-Aktion wurde zu [iosManagedAppProtection](/graph/api/resources/intune-mam-iosmanagedappprotection?view=graph-rest-beta) hinzugefügt. |
| Ergänzungen    | Beta    | Die [updateTargetedSecurityGroups](/graph/api/intune-mam-androidmanagedappprotection-updatetargetedsecuritygroups?view=graph-rest-beta)-Aktion wurde zu [androidManagedAppProtection](/graph/api/resources/intune-mam-androidmanagedappprotection?view=graph-rest-beta) hinzugefügt. |
| Ergänzungen    | Beta    | Die [updateTargetedSecurityGroups](/graph/api/intune-mam-windowsinformationprotection-updatetargetedsecuritygroups?view=graph-rest-beta)-Aktion wurde zu [windowsInformationProtection](/graph/api/resources/intune-mam-windowsinformationprotection?view=graph-rest-beta) hinzugefügt. |
| Ergänzungen    | Beta    | Die [updateTargetedSecurityGroups](/graph/api/intune-mam-windowsinformationprotection-updatetargetedsecuritygroups?view=graph-rest-beta)-Aktion wurde zu [windowsInformationProtectionPolicy](/graph/api/resources/intune-mam-windowsinformationprotectionpolicy?view=graph-rest-beta) hinzugefügt. |
| Ergänzungen    | Beta    | Die [updateTargetedSecurityGroups](/graph/api/intune-mam?view=graph-rest-betamwindowsinformationprotectionpolicy-updatetargetedsecuritygroups)-Aktion wurde zu [mdmWindowsInformationProtectionPolicy](/graph/api/resources/intune-mam?view=graph-rest-betamwindowsinformationprotectionpolicy) hinzugefügt. |
| Ergänzungen    | Beta    | Die [wipeManagedAppRegistrationByDeviceTag](/graph/api/intune-mam-user-wipemanagedappregistrationbydevicetag?view=graph-rest-beta)-Aktion wurde zu [user](/graph/api/resources/intune-deviceconfig-user?view=graph-rest-beta) hinzugefügt. |
| Ergänzungen    | Beta    | Die [getTopMobileAppCount](/graph/api/intune-apps-mobileapp-gettopmobileapps?view=graph-rest-beta)-Funktion wurde zu [mobileApp](/graph/api/resources/intune-apps-mobileapp?view=graph-rest-beta) hinzugefügt. |
| Ergänzungen    | Beta    | Die [verifyWindowsEnrollmentAutoDiscovery](/graph/api/intune-corpenrollment-devicemanagement-verifywindowsenrollmentautodiscovery?view=graph-rest-beta)-Funktion wurde zu [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta) hinzugefügt. |
| Löschung    | Beta    | Die folgenden Entitäten wurden entfernt:<br/>**appProvisioningConfigGroupAssignment**<br/>**defaultManagedAppConfiguration**<br/>**enterpriseCertificate**<br/>**managedDeviceMobileAppProvisioningConfigurationDeviceStatus**<br/>**symantecCertificate**<br/>**windows10WindowsInformationProtectionConfiguration**<br/> |
| Löschung    | Beta    | Die folgenden komplexen Typen wurden entfernt:<br/>**mobileAppInstallSummary**<br/>**windowsArchitecture**<br/>**windowsDeviceType**<br/> |
| Änderung      | Beta    | Die **webBrowserBlockPopups**-Eigenschaft wurde der  [androidGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidgeneraldeviceconfiguration?view=graph-rest-beta)-Entität hinzugefügt. |
| Änderung      | Beta    | Die Eigenschaft **webBrowserBlockPopups**-Eigenschaft wurde aus der [androidGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidgeneraldeviceconfiguration?view=graph-rest-beta)-Entität entfernt. |
| Änderung      | Beta    | Die **appIdentifier**-Eigenschaft wurde der [androidStoreApp](/graph/api/resources/intune-apps-androidstoreapp?view=graph-rest-beta)-Entität hinzugefügt. |
| Änderung      | Beta    | Die Eigenschaften **applicationCount**, **failedApplicationCount** und **appInstallFailures** wurden aus der [appReportingOverviewStatus](/graph/api/resources/appreportingoverviewstatus?view=graph-rest-beta)-Entität entfernt. |
| Änderung      | Beta    | Die Eigenschaften **sharedIPadMaximumUserCount** und **enableSharedIPad** wurden der [depEnrollmentProfile](/graph/api/resources/intune-corpenrollment-depenrollmentprofile?view=graph-rest-beta)-Entität hinzugefügt. |
| Änderung      | Beta    | Die Eigenschaften **shareTokenWithSchoolDataSyncService** und **lastSyncErrorCode** wurden der [depOnboardingSetting](/graph/api/resources/intune-onboarding-deponboardingsetting?view=graph-rest-beta)-Entität hinzugefügt. |
| Änderung      | Beta    | Die Eigenschaften **pendingCount**, **successCount**, **errorCount**, **failedCount**, **lastUpdateDateTime** und **configurationVersion** wurden der [deviceComplianceDeviceOverview](/graph/api/resources/intune-deviceconfig-devicecompliancedeviceoverview?view=graph-rest-beta)-Entität hinzugefügt. |
| Änderung      | Beta    | Die Eigenschaften **numberOfPendingDevices**, **numberOfSucceededDevices**, **numberOfErrorDevices**, **numberOfFailedDevices**, **lastUpdateTime** und **policyRevision** wurden aus der [deviceComplianceDeviceOverview](/graph/api/resources/intune-deviceconfig-devicecompliancedeviceoverview?view=graph-rest-beta)-Entität entfernt. |
| Änderung      | Beta    | Die Eigenschaften **pendingCount**, **successCount**, **errorCount**, **failedCount**, **lastUpdateDateTime** und **configurationVersion** wurden der [deviceComplianceUserOverview](/graph/api/resources/intune-deviceconfig-devicecomplianceuseroverview?view=graph-rest-beta)-Entität hinzugefügt. |
| Änderung      | Beta    | Die Eigenschaften **numberOfPendingDevices**, **numberOfSucceededDevices**, **numberOfErrorDevices**, **numberOfFailedDevices**, **lastUpdateTime** und **policyRevision** wurden aus der [deviceComplianceUserOverview](/graph/api/resources/intune-deviceconfig-devicecomplianceuseroverview?view=graph-rest-beta)-Entität entfernt. |
| Änderung      | Beta    | Die Eigenschaften **pendingCount**, **successCount**, **errorCount**, **failedCount**, **lastUpdateDateTime** und **configurationVersion** wurden der [deviceConfigurationDeviceOverview](/graph/api/resources/intune-deviceconfig-deviceconfigurationdeviceoverview?view=graph-rest-beta)-Entität hinzugefügt. |
| Änderung      | Beta    | Die Eigenschaften **numberOfPendingDevices**, **numberOfSucceededDevices**, **numberOfErrorDevices**, **numberOfFailedDevices**, **lastUpdateTime** und **policyRevision** wurden aus der [deviceConfigurationDeviceOverview](/graph/api/resources/intune-deviceconfig-deviceconfigurationdeviceoverview?view=graph-rest-beta)-Entität entfernt. |
| Änderung      | Beta    | Die Eigenschaften **pendingCount**, **successCount**, **errorCount**, **failedCount**, **lastUpdateDateTime** und **configurationVersion** wurden der [deviceConfigurationUserOverview](/graph/api/resources/intune-deviceconfig-deviceconfigurationuseroverview?view=graph-rest-beta)-Entität hinzugefügt. |
| Änderung      | Beta    | Die Eigenschaften **numberOfPendingDevices**, **numberOfSucceededDevices**, **numberOfErrorDevices**, **numberOfFailedDevices**, **lastUpdateTime** und **policyRevision** wurden aus der [deviceConfigurationUserOverview](/graph/api/resources/intune-deviceconfig-deviceconfigurationuseroverview?view=graph-rest-beta)-Entität entfernt. |
| Änderung      | Beta    | Die **subscriptionState**-Eigenschaft wurde der [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta)-Entität hinzugefügt. |
| Änderung      | Beta    | Die **managedEmailProfileRequired**-Eigenschaft wurde der [iosCompliancePolicy](/graph/api/resources/intune-deviceconfig-ioscompliancepolicy?view=graph-rest-beta)-Entität hinzugefügt. |
| Änderung      | Beta    | Die **appsSingleAppModeList**-Eigenschaft wurde der [iosGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-iosgeneraldeviceconfiguration?view=graph-rest-beta)-Entität hinzugefügt. |
| Änderung      | Beta    | Die **appsSingleAppModeBundleIds**-Eigenschaft wurde aus der [iosGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-iosgeneraldeviceconfiguration?view=graph-rest-beta)-Entität entfernt. |
| Änderung      | Beta    | Die **expirationDateTime**-Eigenschaft wurde der [iosLobAppProvisioningConfiguration](/graph/api/resources/intune-apps-ioslobappprovisioningconfiguration?view=graph-rest-beta)-Entität hinzugefügt. |
| Änderung      | Beta    | Die **expiration**-Eigenschaft wurde aus der [iosLobAppProvisioningConfiguration](/graph/api/resources/intune-apps-ioslobappprovisioningconfiguration?view=graph-rest-beta)-Entität entfernt. |
| Änderung      | Beta    | Die Eigenschaften **passwordMinimumCharacterSetCount**, **osMinimumVersion**, **osMaximumVersion**, **deviceThreatProtectionEnabled**, **deviceThreatProtectionRequiredSecurityLevel** und **storageRequireEncryption** wurden aus der [macOSCompliancePolicy](/graph/api/resources/intune-deviceconfig-macoscompliancepolicy?view=graph-rest-beta)-Entität entfernt. |
| Änderung      | Beta    | Die **manifest**-Eigenschaft wurde aus der [managedAndroidLobApp](/graph/api/resources/intune-apps-managedandroidlobapp?view=graph-rest-beta)-Entität entfernt. |
| Änderung      | Beta    | Die Eigenschaften **isSupervised**, **exchangeLastSuccessfulSyncDateTime**, **exchangeAccessState** und **exchangeAccessStateReason** wurden der [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta)-Entität hinzugefügt. |
| Änderung      | Beta    | Die **deviceExchangeAccessStateSummary**-Eigenschaft wurde der Entität [managedDeviceOverview](/graph/api/resources/intune-devices-manageddeviceoverview?view=graph-rest-beta)-Entität hinzugefügt. |
| Änderung      | Beta    | Die **manifest**-Eigenschaft  wurde aus der [managedIOSLobApp](/graph/api/resources/intune-apps-managedioslobapp?view=graph-rest-beta)-Entität entfernt. |
| Änderung      | Beta    | Die **installSummary**-Eigenschaft  wurde aus der [mobileApp](/graph/api/resources/intune-apps-mobileapp?view=graph-rest-beta)-Entität entfernt. |
| Änderung      | Beta    | Die **uploadState**-Eigenschaft  wurde der [mobileAppContentFile](/graph/api/resources/intune-apps-mobileappcontentfile?view=graph-rest-beta)-Entität hinzugefügt. |
| Änderung      | Beta    | Die folgenden Eigenschaften  in der Entität [ mobileAppContentFile](/graph/api/resources/intune-apps-mobileappcontentfile?view=graph-rest-beta)-Entität wurden geändert:<br/>**azureStorageUriExpirationDateTime** von „Erforderlich“ zu „Optional“<br/> |
| Änderung      | Beta    | Die Eigenschaften **initiatedByUserPrincipalName**, **deviceOwnerUserPrincipalName**, **deviceIMEI** und **actionState** wurden der [remoteActionAudit](/graph/api/resources/intune-deviceconfig-remoteactionaudit?view=graph-rest-beta)-Entität hinzugefügt. |
| Änderung      | Beta    | Die Eigenschaften **oneDriveDisableFileSync**, **safeSearchFilter**, **edgeSearchEngine**, **settingsBlockSettingsApp**, **settingsBlockSystemPage**, **settingsBlockDevicesPage**, **settingsBlockNetworkInternetPage**, **settingsBlockPersonalizationPage**, **settingsBlockAccountsPage**, **settingsBlockTimeLanguagePage**, **settingsBlockEaseOfAccessPage**, **settingsBlockPrivacyPage**, **settingsBlockUpdateSecurityPage**, **experienceBlockWindowsSpotlight**, **experienceBlockWindowsTips**, **experienceBlockConsumerSpecificFeatures**, **startMenuLayoutXml**, **startMenuMode**, **logonBlockFastUserSwitching** und **startBlockUnpinningAppsFromTaskbar** wurden der [windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta)-Entität hinzugefügt. |
| Änderung      | Beta    | Die Eigenschaften **allowPrinting**, **allowScreenCapture** und **allowTextSuggestion** wurden der [windows10SecureAssessmentConfiguration](/graph/api/resources/intune-deviceconfig-windows10secureassessmentconfiguration?view=graph-rest-beta) Entität hinzugefügt. |
| Änderung      | Beta    | Die Eigenschaften **blockPrinting**, **blockScreenCapture** und **blockTextSuggestion** wurden der [windows10SecureAssessmentConfiguration](/graph/api/resources/intune-deviceconfig-windows10secureassessmentconfiguration?view=graph-rest-beta)-Entität hinzugefügt. |
| Änderung      | Beta    | Die **identityName**-Eigenschaft wurde der [windowsAppX](/graph/api/resources/intune-apps-windowsappx?view=graph-rest-beta)-Entität hinzugefügt. |
| Änderung      | Beta    | Der Typ der folgenden Eigenschaften in der [windowsAppX](/graph/api/resources/intune-apps-windowsappx?view=graph-rest-beta)-Entität wurde geändert:<br/>**applicableArchitectures** von [windowsArchitecture](/graph/api/resources/windowsarchitecture?view=graph-rest-beta) in „Zeichenfolge“<br/> |
| Änderung      | Beta    | Die **identityName**-Eigenschaft wurde der [windowsPhone81AppX](/graph/api/resources/intune-apps-windowsphone81appx?view=graph-rest-beta)-Entität hinzugefügt. |
| Änderung      | Beta    | Der Typ der folgenden Eigenschaften in der  [windowsPhone81AppX](/graph/api/resources/intune-apps-windowsphone81appx?view=graph-rest-beta)-Entität wurde geändert:<br/>**applicableArchitectures** von [windowsArchitecture](/graph/api/resources/windowsarchitecture?view=graph-rest-beta) in „Zeichenfolge“<br/> |
| Änderung      | Beta    | Die Eigenschaften **identityName**, **identityPublisherHash** und **identityResourceIdentifier** wurden der [windowsUniversalAppX](/graph/api/resources/intune-apps-windowsuniversalappx?view=graph-rest-beta)-Entität hinzugefügt. |
| Änderung      | Beta    | Der Typ der folgenden Eigenschaften in der  [windowsUniversalAppX](/graph/api/resources/intune-apps-windowsuniversalappx?view=graph-rest-beta)-Entität wurde geändert:<br/>**applicableArchitectures** von [windowsArchitecture](/graph/api/resources/windowsarchitecture?view=graph-rest-beta) in „Zeichenfolge“<br/>**applicableDeviceTypes** von [windowsDeviceType](/graph/api/resources/windowsdevicetype?view=graph-rest-beta) in „Zeichenfolge“<br/> |
| Änderung      | Beta    | Die **restartMode**-Eigenschaft wurde der [windowsUpdateForBusinessConfiguration](/graph/api/resources/intune-deviceconfig-windowsupdateforbusinessconfiguration?view=graph-rest-beta)-Entität hinzugefügt. |
| Änderung      | Beta    | Die **managedDeviceCertificateStates**-Navigationseigenschaft wurde der [androidForWorkScepCertificateProfile](/graph/api/resources/intune-deviceconfig-androidforworkscepcertificateprofile?view=graph-rest-beta)-Entität hinzugefügt. |
| Änderung      | Beta    | Die **managedDeviceCertificateStates**-Navigationseigenschaft wurde der [androidScepCertificateProfile](/graph/api/resources/intune-deviceconfig-androidscepcertificateprofile?view=graph-rest-beta)-Entität hinzugefügt. |
| Änderung      | Beta    | Die Navigationseigenschaften **enterpriseCodeSigningCertificates**, **symantecCodeSigningCertificate**, **sideLoadingKeys**, **managedAppPolicies**, **iosManagedAppProtections**, **androidManagedAppProtections**, **defaultManagedAppProtections**, **targetedManagedAppConfigurations**, **mdmWindowsInformationProtectionPolicies**, **windowsInformationProtectionPolicies**, **managedAppRegistrations** und **managedAppStatuses** wurden der [deviceAppManagement](/graph/api/resources/intune-apps-deviceappmanagement?view=graph-rest-beta)-Entität hinzugefügt. |
| Änderung      | Beta    | Die Eigenschaften **appReportingOverview**, **enterpriseCerts** und **symantecCert** wurden aus der [deviceAppManagement](/graph/api/resources/intune-apps-deviceappmanagement?view=graph-rest-beta)-Entität entfernt. |
| Änderung      | Beta    | Die **deviceSettingStateSummaries**-Navigationseigenschaft wurde der [deviceCompliancePolicy](/graph/api/resources/intune-deviceconfig-devicecompliancepolicy?view=graph-rest-beta)-Entität hinzugefügt. |
| Änderung      | Beta    | Die **deviceSettingStateSummaries**-Navigationseigenschaft wurde der [deviceConfiguration](/graph/api/resources/intune-deviceconfig-deviceconfiguration?view=graph-rest-beta)-Entität hinzugefügt. |
| Änderung      | Beta    | Die Navigationseigenschaften **termsAndConditions**, **androidForWorkSettings**, **androidForWorkAppConfigurationSchemas**, **applePushNotificationCertificate**, **softwareUpdateStatusSummary**, **deviceCompliancePolicyDeviceStateSummary**, **complianceSettingStateSummaries**, **deviceConfigurationDeviceStateSummaries** und **mobileThreatDefenseConnectors** wurden der [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta)-Entität hinzugefügt. |
| Änderung      | Beta    | Die Navigationseigenschaften **teacherRootCertificates**, **teacherIdentityCertificate**, **studentRootCertificates** und **studentIdentityCertificate** wurden aus der [iosEducationDeviceConfiguration](/graph/api/resources/intune-deviceconfig-ioseducationdeviceconfiguration?view=graph-rest-beta)-Entität entfernt. |
| Änderung      | Beta    | Der Typ der folgenden Eigenschaften in der [iosLobAppProvisioningConfiguration](/graph/api/resources/intune-apps-ioslobappprovisioningconfiguration?view=graph-rest-beta)-Entität wurde geändert:<br/>**deviceStatuses** von [managedDeviceMobileAppProvisioningConfigurationDeviceStatus](/graph/api/resources/manageddevicemobileappprovisioningconfigurationdevicestatus?view=graph-rest-beta)-Sammlung in [managedDeviceMobileAppConfigurationDeviceStatus](/graph/api/resources/intune-apps-manageddevicemobileappconfigurationdevicestatus?view=graph-rest-beta)-Sammlung<br/>**groupAssignments** von [appProvisioningConfigGroupAssignment](/graph/api/resources/appprovisioningconfiggroupassignment?view=graph-rest-beta)-Sammlung in [mobileAppProvisioningConfigGroupAssignment](/graph/api/resources/intune-apps-mobileappprovisioningconfiggroupassignment?view=graph-rest-beta)-Sammlung<br/> |
| Änderung      | Beta    | Die **managedDeviceCertificateStates**-Navigationseigenschaft wurde der [iosScepCertificateProfile](/graph/api/resources/intune-deviceconfig-iosscepcertificateprofile?view=graph-rest-beta)-Entität hinzugefügt. |
| Änderung      | Beta    | Die **managedDeviceCertificateStates**-Navigationseigenschaft wurde der [macOSScepCertificateProfile](/graph/api/resources/intune-deviceconfig-macosscepcertificateprofile?view=graph-rest-beta)-Entität hinzugefügt. |
| Änderung      | Beta    | Die Navigationseigenschaften **deviceConfigurationStates** und **deviceCompliancePolicyStates** wurden der [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta)-Entität hinzugefügt. |
| Änderung      | Beta    | Die Navigationseigenschaften **deviceStatusSummary** und **userStatusSummary** wurden der [managedDeviceMobileAppConfiguration](/graph/api/resources/intune-apps-manageddevicemobileappconfiguration?view=graph-rest-beta)-Entität hinzugefügt. |
| Änderung      | Beta    | Die **installSummary**-Navigationseigenschaft  wurde der [mobileApp](/graph/api/resources/intune-apps-mobileapp?view=graph-rest-beta)-Entität hinzugefügt. |
| Änderung      | Beta    | Die **sideLoadingKeys**-Navigationseigenschaft wurde aus der [organization](/graph/api/resources/intune-onboarding-organization?view=graph-rest-beta)-Entität entfernt. |
| Änderung      | Beta    | Die **managedDeviceCertificateStates**-Navigationseigenschaft wurde der [windows81SCEPCertificateProfile](/graph/api/resources/intune-deviceconfig-windows81scepcertificateprofile?view=graph-rest-beta)-Entität hinzugefügt. |
| Änderung      | Beta    | Die **managedDeviceCertificateStates**-Navigationseigenschaft wurde der [windowsPhone81SCEPCertificateProfile](/graph/api/resources/intune-deviceconfig-windowsphone81scepcertificateprofile?view=graph-rest-beta)-Entität hinzugefügt. |
| Änderung      | Beta    | Die Eigenschaften **applicationId**, **appName**, **platformId**, **userFailures** und **deviceFailures** wurden aus dem komplexen Typ [appInstallationFailure](/graph/api/resources/intune-apps-appinstallationfailure?view=graph-rest-beta) entfernt. |
| Änderung      | Beta    | Die **displayName**-Eigenschaft wurde dem komplexen Typ [iosHomeScreenFolderPage](/graph/api/resources/intune-deviceconfig-ioshomescreenfolderpage?view=graph-rest-beta) hinzugefügt. |
| Änderung      | Beta    | Die **displayName**-Eigenschaft wurde dem komplexen Typ [iosHomeScreenPage](/graph/api/resources/intune-deviceconfig-ioshomescreenpage?view=graph-rest-beta) hinzugefügt. |
| Änderung      | Beta    | Die Eigenschaften **subjectName**, **description**, **expirationDateTime** und **certificate** wurden dem komplexen Typ [windowsInformationProtectionDataRecoveryCertificate](/graph/api/resources/intune-mam-windowsinformationprotectiondatarecoverycertificate?view=graph-rest-beta) hinzugefügt. |
| Änderung      | Beta    | Die Eigenschaften **dataRecoveryCertificate** und **certificateFileName** wurden aus dem komplexen Typ [ wurwindowsInformationProtectionDataRecoveryCertificate](/graph/api/resources/intune-mam-windowsinformationprotectiondatarecoverycertificate?view=graph-rest-beta) entfernt. |
| Änderung      | Beta    | Die **displayName**-Eigenschaft wurde dem komplexen Typ [windowsPackageInformation](/graph/api/resources/intune-apps-windowspackageinformation?view=graph-rest-beta) hinzugefügt. |
| Änderung      | Beta    | Der Typ der folgenden Eigenschaften im komplexen Typ [windowsPackageInformation](/graph/api/resources/intune-apps-windowspackageinformation?view=graph-rest-beta) wurde geändert:<br/>**applicableArchitecture** von [windowsArchitecture](/graph/api/resources/windowsarchitecture?view=graph-rest-beta) in „Zeichenfolge“<br/> |
| Änderung      | Beta    | Die folgenden Eigenschaften im komplexen Typ  [windowsPackageInformation](/graph/api/resources/intune-apps-windowspackageinformation?view=graph-rest-beta) wurden geändert:<br/>**applicableArchitecture** von „Optional“ in „Erforderlich“<br/> |

### <a name="add-contracts-to-microsoft-graph"></a>Hinzufügen von Verträgen zu Microsoft Graph

| **Änderungstyp** | **Version** | **Beschreibung**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Ergänzungen        | Beta        | Neue Ressource</br>[contract](/graph/api/resources/contract?view=graph-rest-beta) |

### <a name="add-domain-operations-to-microsoft-graph"></a>Hinzufügen von Domänenvorgängen zu Microsoft Graph

| **Änderungstyp** | **Version** | **Beschreibung**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Ergänzungen        | Beta        | Funktionen wurden zu [Domänen](/graph/api/resources/domain?view=graph-rest-beta) hinzugefügt.<br/>Neue Entitäten:</br>[domain](/graph/api/resources/domain?view=graph-rest-beta)<br/>[domainDnsRecord](/graph/api/resources/domaindnsrecord?view=graph-rest-beta)<br/>[domainDnsCnameRecord](/graph/api/resources/domaindnscnamerecord?view=graph-rest-beta)<br/>[domainDnsMxRecord](/graph/api/resources/domaindnsmxrecord?view=graph-rest-beta)<br/>[domainDnsSrvRecord](/graph/api/resources/domaindnssrvrecord?view=graph-rest-beta)<br/>[domainDnsTxtRecord](/graph/api/resources/domaindnstxtrecord?view=graph-rest-beta)<br/>[domainDnsUnavailableRecord](/graph/api/resources/domaindnsunavailablerecord?view=graph-rest-beta)<br/>Neue Aktionen:</br>[forceDelete](/graph/api/domain-forcedelete?view=graph-rest-beta)</br>[verify](/graph/api/domain-verify?view=graph-rest-beta) |

### <a name="add-custom-data-to-microsoft-graph-using-schema-extensions"></a>Hinzufügen von benutzerdefinierten Daten zu Microsoft Graph unter Verwendung von Schemaerweiterungen

| **Änderungstyp** | **Version** | **Beschreibung**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Ergänzungen        | Beta        | Erweitern von Microsoft Graph mit Anwendungsdaten unter Verwendung von [Schemaerweiterungen](extensibility-overview.md#schema-extensions).  Dies wird in den folgenden Ressourcen unterstützt:<br/>Administrative Einheit<br/>Kalenderereignis<br/>Gerät<br/>Gruppe<br/>Nachricht<br/>Organisation<br/>Privater Kontakt<br/>Beitrag<br/>user<br/>Sehen Sie sich das folgende Beispiel an:<br/>[Hinzufügen von benutzerdefinierten Daten zu Gruppen mithilfe von Schemaerweiterungen (Preview)](extensibility-schema-groups.md) |
| Ergänzungen        | Beta        | Es wurde eine alternative Möglichkeit zum Erstellen einer Schemaerweiterungsdefinition bereitgestellt, ohne dass eine überprüfte Vanity-.com-Domäne erforderlich ist. Weitere Informationen finden Sie unter [Schemaerweiterungen](extensibility-overview.md#schema-extensions). |

### <a name="add-custom-data-to-microsoft-graph-using-open-extensions"></a>Hinzufügen von benutzerdefinierten Daten zu Microsoft Graph unter Verwendung von offenen Erweiterungen

| **Änderungstyp** | **Version**   | **Beschreibung**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Änderung          | v1.0 und Beta | Die bisherigen „Office 365-Datenerweiterungen“ wurden in „offene Erweiterungen“ umbenannt. |
| Ergänzungen        | Beta          | Es wurden Ressourcen hinzugefügt, die [offene Erweiterungen](extensibility-overview.md#open-extensions) unterstützen: <br/>Administrative Einheit<br/>Gerät<br/>Gruppe<br/>Organisation<br/>Benutzer<br/>Sehen Sie sich das folgende Beispiel an:<br/>[Hinzufügen von benutzerdefinierten Daten zu Benutzern mithilfe offener Erweiterungen (Preview)](extensibility-open-users.md) |

### <a name="directory-apis"></a>Verzeichnis-APIs

| **Änderungstyp** | **Version** | **Beschreibung**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Ergänzungen        | Beta        | Es wurde Unterstützung zum [Wiederherstellen und endgültigen Löschen von Gruppen](/graph/api/resources/directory?view=graph-rest-beta) hinzugefügt.<br/>Neue Entität: Verzeichnis mit deleteditems-Navigationseigenschaft. |
| Ergänzungen        | Beta        | Neue Entität:</br>[Endpunkt](/graph/api/resources/endpoint?view=graph-rest-beta) |
| Änderung          | Beta        | Neue [endpoint](/graph/api/group-list-endpoints?view=graph-rest-beta)-Nagivationseigenschaft in [Gruppen](/graph/api/resources/group?view=graph-rest-beta) |
| Ergänzungen        | Beta        | Neue Entität:</br>[licenseDetails](/graph/api/resources/licensedetails?view=graph-rest-beta) |
| Änderung          | Beta        | Neue [licensedetails](/graph/api/user-list-licensedetails?view=graph-rest-beta)-Nagivationseigenschaft für [Benutzer](/graph/api/resources/user?view=graph-rest-beta) |

### <a name="reports-apis"></a>Bericht-APIs

| **Änderungstyp** | **Version** | **Beschreibung**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Ergänzungen        | Beta        | Die neue Vorschau-API für Office 365-Berichte wurde eingeführt. Sie können sie zum Abrufen von Verwendungsberichten darüber verwenden, wie Personen in Ihrem Unternehmen Office 365-Dienste nutzen. Sie können zum Beispiel identifizieren, wer einen Dienst häufig verwendet und Kontingente erreicht oder wer vielleicht gar keine Office 365-Lizenz benötigt. Weitere Informationen finden Sie unter [Bericht](/graph/api/resources/report?view=graph-rest-beta). |

### <a name="directory-apis"></a>Verzeichnis-APIs

| **Änderungstyp** | **Version** | **Beschreibung**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Ergänzungen        | Beta        | Neue Entität:</br>[contract](/graph/api/resources/contract?view=graph-rest-beta) |

## <a name="february-2017"></a>Februar 2017

### <a name="intune-apis"></a>Intune APIs

| Änderungstyp | Version | Beschreibung                              |
| :---------- | :------ | :--------------------------------------- |
| Ergänzungen    | Beta    | Hinzugefügte neue Entitäten:<br/>[androidForWorkCertificateProfileBase](/graph/api/resources/intune-deviceconfig-androidforworkcertificateprofilebase?view=graph-rest-beta)<br/>[androidForWorkEasEmailProfileBase](/graph/api/resources/intune-deviceconfig-androidforworkeasemailprofilebase?view=graph-rest-beta)<br/>[androidForWorkEnterpriseWiFiConfiguration](/graph/api/resources/intune-deviceconfig-androidforworkenterprisewificonfiguration?view=graph-rest-beta)<br/>[androidForWorkGmailEasConfiguration](/graph/api/resources/intune-deviceconfig-androidforworkgmaileasconfiguration?view=graph-rest-beta)<br/>[androidForWorkNineWorkEasConfiguration](/graph/api/resources/intune-deviceconfig-androidforworknineworkeasconfiguration?view=graph-rest-beta)<br/>[androidForWorkPkcsCertificateProfile](/graph/api/resources/intune-deviceconfig-androidforworkpkcscertificateprofile?view=graph-rest-beta)<br/>[androidForWorkScepCertificateProfile](/graph/api/resources/intune-deviceconfig-androidforworkscepcertificateprofile?view=graph-rest-beta)<br/>[androidForWorkTrustedRootCertificate](/graph/api/resources/intune-deviceconfig-androidforworktrustedrootcertificate?view=graph-rest-beta)<br/>[androidForWorkWiFiConfiguration](/graph/api/resources/intune-deviceconfig-androidforworkwificonfiguration?view=graph-rest-beta)<br/>[appleDeviceFeaturesConfigurationBase](/graph/api/resources/intune-deviceconfig-appledevicefeaturesconfigurationbase?view=graph-rest-beta)<br/>[appProvisioningConfigGroupAssignment](/graph/api/resources/intune-apps-appprovisioningconfiggroupassignment?view=graph-rest-beta)<br/>[deviceComplianceUserOverview](/graph/api/resources/intune-deviceconfig-devicecomplianceuseroverview?view=graph-rest-beta)<br/>[deviceConfigurationUserOverview](/graph/api/resources/intune-deviceconfig-deviceconfigurationuseroverview?view=graph-rest-beta)<br/>[enterpriseCertificate](/graph/api/resources/intune-apps-enterprisecertificate?view=graph-rest-beta)<br/>[iosEducationDeviceConfiguration](/graph/api/resources/intune-deviceconfig-ioseducationdeviceconfiguration?view=graph-rest-beta)<br/>[macOSDeviceFeaturesConfiguration](/graph/api/resources/intune-deviceconfig-macosdevicefeaturesconfiguration?view=graph-rest-beta)<br/>[managedAndroidLobApp](/graph/api/resources/intune-apps-managedandroidlobapp?view=graph-rest-beta)<br/>[managedDeviceMobileAppProvisioningConfigurationDeviceStatus](/graph/api/resources/intune-apps-manageddevicemobileappprovisioningconfigurationdevicestatus?view=graph-rest-beta)<br/>[managedIOSLobApp](/graph/api/resources/intune-apps-managedioslobapp?view=graph-rest-beta)<br/>[managedMobileLobApp](/graph/api/resources/intune-apps-managedmobilelobapp?view=graph-rest-beta)<br/>[symantecCertificate](/graph/api/resources/intune-apps-symanteccertificate?view=graph-rest-beta)<br/>[windowsAppX](/graph/api/resources/intune-apps-windowsappx?view=graph-rest-beta)<br/>[windowsCertificateProfileBase](/graph/api/resources/intune-deviceconfig-windowscertificateprofilebase?view=graph-rest-beta)<br/>[windowsPhone81AppX](/graph/api/resources/intune-apps-windowsphone81appx?view=graph-rest-beta)<br/>[windowsPhone81AppXBundle](/graph/api/resources/intune-apps-windowsphone81appxbundle?view=graph-rest-beta)<br/>[windowsPhoneXAP](/graph/api/resources/intune-apps-windowsphonexap?view=graph-rest-beta)<br/>[windowsUniversalAppX](/graph/api/resources/intune-apps-windowsuniversalappx?view=graph-rest-beta)<br/> |
| Ergänzungen    | Beta    | Die folgenden komplexen Typen wurden hinzugefügt:<br/>[airPrintDestination](/graph/api/resources/intune-deviceconfig-airprintdestination?view=graph-rest-beta)<br/>[windowsArchitecture](/graph/api/resources/intune-apps-windowsarchitecture?view=graph-rest-beta)<br/>[windowsDeviceType](/graph/api/resources/intune-apps-windowsdevicetype?view=graph-rest-beta)<br/>[windowsMinimumOperatingSystem](/graph/api/resources/intune-apps-windowsminimumoperatingsystem?view=graph-rest-beta)<br/>[windowsPackageInformation](/graph/api/resources/intune-apps-windowspackageinformation?view=graph-rest-beta)<br/> |
| Ergänzungen    | Beta    | Die [assign](/graph/api/intune-apps-ioslobappprovisioningconfiguration-assign?view=graph-rest-beta)-Aktion wurde der [iosLobAppProvisioningConfiguration](/graph/api/resources/intune-apps-ioslobappprovisioningconfiguration?view=graph-rest-beta)-Entität hinzugefügt. |
| Ergänzungen    | Beta    | Die [scheduleActionsForRules](/graph/api/intune-deviceconfig-devicecompliancepolicy-scheduleactionsforrules?view=graph-rest-beta)-Aktion wurde der [deviceCompliancePolicy](/graph/api/resources/intune-deviceconfig-devicecompliancepolicy?view=graph-rest-beta)-Entität hinzugefügt. |
| Ergänzungen    | Beta    | Die [updateTargetedSecurityGroups](/graph/api/intune-mam-targetedmanagedappconfiguration-updatetargetedsecuritygroups?view=graph-rest-beta)-Aktion wurde der [targetedManagedAppConfiguration](/graph/api/resources/intune-mam-targetedmanagedappconfiguration?view=graph-rest-beta)-Entität hinzugefügt. |
| Ergänzungen    | Beta    | Die [getScopesForUser](/graph/api/intune-rbac-resourceoperation-getscopesforintune-devices-user?view=graph-rest-beta)-Funktion wurde der [resourceOperation](/graph/api/resources/intune-rbac-resourceoperation?view=graph-rest-beta)-Entität hinzugefügt. |
| Änderung      | Beta    | Die **manifest**-Eigenschaft wurde aus der [androidLobApp](/graph/api/resources/intune-apps-androidlobapp?view=graph-rest-beta)-Entität entfernt. |
| Änderung      | Beta    | Die Eigenschaften **assetTagTemplate**, **lockScreenFootnote**, **homeScreenDockIcons** und **homeScreenPages**wurden der [iosDeviceFeaturesConfiguration](/graph/api/resources/intune-deviceconfig-iosdevicefeaturesconfiguration?view=graph-rest-beta)-Entität hinzugefügt. |
| Änderung      | Beta    | Die Eigenschaften **deviceSharingAssetTagInformation**, **deviceSharingLockScreenFootnote**, **homeScreenLayoutDockIcons** und **homeScreenLayoutPages** wurden aus der [iosDeviceFeaturesConfiguration](/graph/api/resources/intune-deviceconfig-iosdevicefeaturesconfiguration?view=graph-rest-beta)-Entität entfernt. |
| Änderung      | Beta    | Die **appsSingleAppModeBundleIds**-Eigenschaft wurde der [iosGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-iosgeneraldeviceconfiguration?view=graph-rest-beta)-Entität hinzugefügt. |
| Änderung      | Beta    | Die **manifest**-Eigenschaft wurde aus der [iosLobApp](/graph/api/resources/intune-apps-ioslobapp?view=graph-rest-beta)-Entität entfernt. |
| Änderung      | Beta    | Die Eigenschaften **createdDateTime**, **description**, **lastModifiedDateTime**, **displayName** und **version** wurden der [iosLobAppProvisioningConfiguration](/graph/api/resources/intune-apps-ioslobappprovisioningconfiguration?view=graph-rest-beta)-Entität hinzugefügt. |
| Änderung      | Beta    | Die Eigenschaften **createdDateTime** und **lastModifiedDateTime** wurden der [managedAppPolicy](/graph/api/resources/intune-mam-managedapppolicy?view=graph-rest-beta)-Entität hinzugefügt. |
| Änderung      | Beta    | Die **deviceRegistrationState**-Eigenschaft wurde aus der [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta)-Entität entfernt. |
| Änderung      | Beta    | Die **manifest**-Eigenschaft wurde der [mobileAppContentFile](/graph/api/resources/intune-apps-mobileappcontentfile?view=graph-rest-beta)-Entität hinzugefügt. |
| Änderung      | Beta    | Die Eigenschaften **osDescription** und **userName** wurden der [mobileAppInstallStatus](/graph/api/resources/intune-apps-mobileappinstallstatus?view=graph-rest-beta)-Entität hinzugefügt. |
| Änderung      | Beta    | Die **deviceType**-Eigenschaft wurde aus der [mobileAppInstallStatus](/graph/api/resources/intune-apps-mobileappinstallstatus?view=graph-rest-beta)-Entität entfernt. |
| Änderung      | Beta    | Der Typ der folgenden Eigenschaften wurde aus der [mobileAppInstallStatus](/graph/api/resources/intune-apps-mobileappinstallstatus?view=graph-rest-beta)-Entität entfernt:<br/>**mobileAppInstallStatusValue** von „Int32“ in „String“ |
| Änderung      | Beta    | Die Eigenschaften **targetedSecurityGroupIds** und **targetedSecurityGroupsCount** wurden der [targetedManagedAppConfiguration](/graph/api/resources/intune-mam-targetedmanagedappconfiguration?view=graph-rest-beta)-Entität hinzugefügt. |
| Änderung      | Beta    | Die **numberOfTargetedSecurityGroups**-Eigenschaft wurde aus der [targetedManagedAppConfiguration](/graph/api/resources/intune-mam-targetedmanagedappconfiguration?view=graph-rest-beta)-Entität entfernt. |
| Änderung      | Beta    | Die **Id**-Eigenschaft wurde der [user](/graph/api/resources/intune-devices-user?view=graph-rest-beta)-Entität hinzugefügt. |
| Änderung      | Beta    | Die Eigenschaften **renewalThresholdPercentage**, **keyStorageProvider**, **subjectNameFormat**, **subjectAlternativeNameType**, **certificateValidityPeriodValue** und **certificateValidityPeriodScale** wurden aus der [windows10CertificateProfileBase](/graph/api/resources/intune-deviceconfig-windows10certificateprofilebase?view=graph-rest-beta)-Entität entfernt. |
| Änderung      | Beta    | Die Eigenschaften **renewalThresholdPercentage**, **keyStorageProvider**, **subjectNameFormat**, **subjectAlternativeNameType**, **certificateValidityPeriodValue** und **certificateValidityPeriodScale** wurden aus der [windows81CertificateProfileBase](/graph/api/resources/intune-deviceconfig-windows81certificateprofilebase?view=graph-rest-beta)-Entität entfernt. |
| Änderung      | Beta    | Die **applyToWindows10Mobile**-Eigenschaft wurde aus der [windowsPhone81GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windowsphone81generalconfiguration?view=graph-rest-beta)-Entität entfernt. |
| Änderung      | Beta    | Die Navigationseigenschaften **enterpriseCerts**, **iosLobAppProvisioningConfigurations** und **symantecCert** wurden der [deviceAppManagement](/graph/api/resources/intune-apps-deviceappmanagement?view=graph-rest-beta)-Entität hinzugefügt. |
| Änderung      | Beta    | Die **userStatusOverview**-Navigationseigenschaft wurde der [deviceCompliancePolicy](/graph/api/resources/intune-deviceconfig-devicecompliancepolicy?view=graph-rest-beta)-Entität hinzugefügt. |
| Änderung      | Beta    | Die **userStatusOverview**-Navigationseigenschaft wurde der [deviceConfiguration](/graph/api/resources/intune-deviceconfig-deviceconfiguration?view=graph-rest-beta)-Entität hinzugefügt. |
| Änderung      | Beta    | Die Navigationseigenschaften **groupAssignments**, **deviceStatuses** und **userStatuses** wurden der [iosLobAppProvisioningConfiguration](/graph/api/resources/intune-apps-ioslobappprovisioningconfiguration?view=graph-rest-beta)-Entität hinzugefügt. |
| Änderung      | Beta    | Der Typ der folgenden Eigenschaften in der [windows10VpnConfiguration](/graph/api/resources/intune-deviceconfig-windows10vpnconfiguration?view=graph-rest-beta)-Entität wurde geändert:<br/>**identityCertificate** von [windows10CertificateProfileBase](/graph/api/resources/intune-deviceconfig-windows10certificateprofilebase?view=graph-rest-beta) in [windowsCertificateProfileBase](/graph/api/resources/intune-deviceconfig-windowscertificateprofilebase?view=graph-rest-beta) |
| Änderung      | Beta    | Die Eigenschaften **deviceComplianceCheckinThresholdDays** und **isScheduledActionEnabled** wurden dem komplexen Typ [deviceManagementSettings](/graph/api/resources/intune-deviceconfig-devicemanagementsettings?view=graph-rest-beta) hinzugefügt. |
| Änderung      | Beta    | Die Eigenschaften **windowsCommercialId** und **windowsCommercialIdLastModifiedTime** wurden aus dem komplexen Typ [deviceManagementSettings](/graph/api/resources/intune-deviceconfig-devicemanagementsettings?view=graph-rest-beta) entfernt. |
| Änderung      | Beta    | Die Eigenschaften **bundleID**, **appName**, **publisher**, **enabled** und **showOnLockScreen** wurden dem komplexen Typ [iosNotificationSettings](/graph/api/resources/intune-deviceconfig-iosnotificationsettings?view=graph-rest-beta) hinzugefügt. |
| Änderung      | Beta    | Die Eigenschaften **bundleIdentifier**, **notificationsEnabled** und **showInLockScreen** wurden aus dem komplexen Typ [iosNotificationSettings](/graph/api/resources/intune-deviceconfig-iosnotificationsettings?view=graph-rest-beta) entfernt. |



## <a name="january-2017"></a>Januar 2017

### <a name="outlook-calendar"></a>Outlook-Kalender

| **Änderungstyp** | **Version** | **Beschreibung**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Ergänzungen        | v1.0        | Neue Aktion [findMeetingTimes](/graph/api/user-findmeetingtimes?view=graph-rest-1.0) für die [Benutzer](/graph/api/resources/user?view=graph-rest-1.0)-Ressource. |
| Ergänzungen        | v1.0        | Neuer komplexer Typ [attendeeBase](/graph/api/resources/attendeebase?view=graph-rest-1.0), der  aus einer Typeigenschaft für den Teilnehmertyp besteht. |
| Ergänzungen        | v1.0        | Neue komplexe Typen:<br/>[attendeeAvailability](/graph/api/resources/attendeeavailability?view=graph-rest-1.0)<br/>[locationConstraint](/graph/api/resources/locationconstraint?view=graph-rest-1.0) <br/>[locationConstraintItem](/graph/api/resources/locationconstraintitem?view=graph-rest-1.0)<br/>[meetingTimeSuggestion](/graph/api/resources/meetingtimesuggestion?view=graph-rest-1.0)<br/>[meetingTimeSuggestionsResult](/graph/api/resources/meetingtimesuggestionsresult?view=graph-rest-1.0)<br/>[timeConstraint](/graph/api/resources/timeconstraint?view=graph-rest-1.0)<br/>[timeSlot](/graph/api/resources/timeslot?view=graph-rest-1.0) |
| Änderung          | v1.0        | Der komplexe Typ des [Teilnehmers](/graph/api/resources/attendee?view=graph-rest-1.0) wird jetzt von AttendeeBase abgeleitet, der wiederum vom [Empfänger](/graph/api/resources/recipient?view=graph-rest-1.0) abgeleitet wird. Einschließlich die vererbten Eigenschaften besteht es aus denselben **Status**-, **Typ**- und **E-Mail-Adresse**-Eigenschaften wie zuvor. |
| Ergänzungen        | Beta        | hexColor zur [Kalender](/graph/api/resources/calendar?view=graph-rest-beta)-Ressource hinzugefügt. |

### <a name="intune-apis"></a>Intune APIs

| **Änderungstyp** | **Version** | **Beschreibung**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Ergänzungen        | Beta        | Hinzugefügte neue Entitäten: <br/>[appReportingOverviewStatus](/graph/api/resources/intune-apps-appreportingoverviewstatus?view=graph-rest-beta)<br/>[deviceComplianceDeviceOverview](/graph/api/resources/intune-deviceconfig-devicecompliancedeviceoverview?view=graph-rest-beta)<br/>[deviceConfigurationDeviceOverview](/graph/api/resources/intune-deviceconfig-deviceconfigurationdeviceoverview?view=graph-rest-beta)<br/>[deviceManagementExchangeOnpremisesPolicy](/graph/api/resources/intune-onboarding-devicemanagementexchangeonpremisespolicy?view=graph-rest-beta)<br/>[iosDeviceFeaturesConfiguration](/graph/api/resources/intune-deviceconfig-iosdevicefeaturesconfiguration?view=graph-rest-beta)<br/>[iosEducationDeviceConfiguration](/graph/api/resources/intune-deviceconfig-ioseducationdeviceconfiguration?view=graph-rest-beta)<br/>[iosLobAppProvisioningConfiguration](/graph/api/resources/intune-apps-ioslobappprovisioningconfiguration?view=graph-rest-beta)<br/>[onpremisesConditionalAccessSettings](/graph/api/resources/intune-onboarding-onpremisesconditionalaccesssettings?view=graph-rest-beta)<br/>[sharedPCConfiguration](/graph/api/resources/intune-deviceconfig-sharedpcconfiguration?view=graph-rest-beta)<br/>[windows10EnterpriseModernAppManagementConfiguration](/graph/api/resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration?view=graph-rest-beta)<br/>[windows10SecureAssessmentConfiguration](/graph/api/resources/intune-deviceconfig-windows10secureassessmentconfiguration?view=graph-rest-beta)<br/>[windows10WindowsInformationProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windows10windowsinformationprotectionconfiguration?view=graph-rest-beta) |
|Ergänzungen|Beta|Die folgenden kompleen Typen wurden hinzugefügt: <br/> [appInstallationFailure](/graph/api/resources/intune-apps-appinstallationfailure?view=graph-rest-beta)<br/>[enterpriseCloudResource](/graph/api/resources/intune-deviceconfig-enterprisecloudresource?view=graph-rest-beta)<br/>[iosHomeScreenApp](/graph/api/resources/intune-deviceconfig-ioshomescreenapp?view=graph-rest-beta)<br/>[iosHomeScreenFolder](/graph/api/resources/intune-deviceconfig-ioshomescreenfolder?view=graph-rest-beta)<br/>[iosHomeScreenFolderPage](/graph/api/resources/intune-deviceconfig-ioshomescreenfolderpage?view=graph-rest-beta)<br/>[iosHomeScreenItem](/graph/api/resources/intune-deviceconfig-ioshomescreenitem?view=graph-rest-beta)<br/>[iosHomeScreenPage](/graph/api/resources/intune-deviceconfig-ioshomescreenpage?view=graph-rest-beta)<br/>[iosNotificationSettings](/graph/api/resources/intune-deviceconfig-iosnotificationsettings?view=graph-rest-beta)<br/>[iPv6Range](/graph/api/resources/intune-deviceconfig-ipv6range?view=graph-rest-beta)<br/>[sharedPCAccountManagerPolicy](/graph/api/resources/intune-deviceconfig-sharedpcaccountmanagerpolicy?view=graph-rest-beta)<br/>[windowsInformationProtectionAppRule](/graph/api/resources/intune-deviceconfig-windowsinformationprotectionapprule?view=graph-rest-beta)<br/>[windowsInformationProtectionAppRuleAppLockerPolicyFileTemplate](/graph/api/resources/intune-deviceconfig-windowsinformationprotectionappruleapplockerpolicyfiletemplate?view=graph-rest-beta)<br/>[windowsInformationProtectionAppRuleDesktopTemplate](/graph/api/resources/intune-deviceconfig-windowsinformationprotectionappruledesktoptemplate?view=graph-rest-beta)<br/>[windowsInformationProtectionAppRuleStoreAppTemplate](/graph/api/resources/intune-deviceconfig-windowsinformationprotectionapprulestoreapptemplate?view=graph-rest-beta)<br/>[windowsInformationProtectionAppRuleTemplate](/graph/api/resources/intune-deviceconfig-windowsinformationprotectionappruletemplate?view=graph-rest-beta)<br/>[windowsInformationProtectionCorporateNetworkLocation](/graph/api/resources/intune-deviceconfig-windowsinformationprotectioncorporatenetworklocation?view=graph-rest-beta)<br/>[windowsInformationProtectionDataRecoveryCertificate](/graph/api/resources/intune-deviceconfig-windowsinformationprotectiondatarecoverycertificate?view=graph-rest-beta)<br/>[windowsInformationProtectionProtectedLocation](/graph/api/resources/intune-deviceconfig-windowsinformationprotectionprotectedlocation?view=graph-rest-beta)<br/>[windowsInformationProtectionProtectedLocationEnterpriseCloudResources](/graph/api/resources/intune-deviceconfig-windowsinformationprotectionprotectedlocationenterprisecloudresources?view=graph-rest-beta)<br/>[windowsInformationProtectionProtectedLocationEnterpriseInternalProxyServers](/graph/api/resources/intune-deviceconfig-windowsinformationprotectionprotectedlocationenterpriseinternalproxyservers?view=graph-rest-beta)<br/>[windowsInformationProtectionProtectedLocationEnterpriseIPv4Ranges](/graph/api/resources/intune-deviceconfig-windowsinformationprotectionprotectedlocationenterpriseipv4ranges?view=graph-rest-beta)<br/>[windowsInformationProtectionProtectedLocationEnterpriseIPv6Ranges](/graph/api/resources/intune-deviceconfig-windowsinformationprotectionprotectedlocationenterpriseipv6ranges?view=graph-rest-beta)<br/>[windowsInformationProtectionProtectedLocationEnterpriseNetworkDomainNames](/graph/api/resources/intune-deviceconfig-windowsinformationprotectionprotectedlocationenterprisenetworkdomainnames?view=graph-rest-beta)<br/>[windowsInformationProtectionProtectedLocationEnterpriseProxyServers](/graph/api/resources/intune-deviceconfig-windowsinformationprotectionprotectedlocationenterpriseproxyservers?view=graph-rest-beta)<br/>[windowsInformationProtectionProtectedLocationNeutralResources](/graph/api/resources/intune-deviceconfig-windowsinformationprotectionprotectedlocationneutralresources?view=graph-rest-beta)
|Löschung|Beta|Die folgenden komplexen Typen wurden entfernt und durch microsoft.graph.json ersetzt:<br/>managedAppDeploymentSummary <br/>managedAppSummary<br /> |
|Ändern|Beta|Der Eigenschaftentyp „appConfigComplianceStatus“ wurde in den folgenden Entitäten durch „complianceStatus“ ersetzt: <br/>[managedDeviceMobileAppConfigurationDeviceStatus](/graph/api/resources/intune-apps-manageddevicemobileappconfigurationdevicestatus?view=graph-rest-beta)<br/>[managedDeviceMobileAppConfigurationUserStatus](/graph/api/resources/intune-apps-manageddevicemobileappconfigurationuserstatus?view=graph-rest-beta)|
|Änderung|Beta|Für die Ressource [managedAppStatusRaw](/graph/api/resources/intune-mam-managedappstatusraw?view=graph-rest-beta) wurde der Typ des Eigenschafteninhalts von „managedAppSummary“ in „json“ geändert.|
|Änderung|Beta|Die Funktion „getUsersWithFlaggedAppRegistration“ wurde aus der [managedAppRegistration](/graph/api/resources/intune-mam-managedappregistration?view=graph-rest-beta)-Sammlung entfernt.|
|Änderung|Beta|Die Nagivationseigenschaft **vppToken** der [iosVppApp](/graph/api/resources/intune-apps-iosvppapp?view=graph-rest-beta)-Entität wurde so geändert, dass es sich nicht mehr um eine enthaltene Sammlung handelt.|
|Änderung|Beta|Die **deviceStatusOverview**-Eigenschaft wurde den Entitäten [deviceConfiguration](/graph/api/resources/intune-deviceconfig-deviceconfiguration?view=graph-rest-beta) und [deviceCompliancePolicy](/graph/api/resources/intune-deviceconfig-devicecompliancepolicy?view=graph-rest-beta) hinzugefügt.|
|Änderung|Beta|Die **appReportingOverview**-Eigenschaft wurde dem [deviceAppManagement](/graph/api/resources/intune-apps-deviceappmanagement?view=graph-rest-beta)-Singleton hinzugefügt.|
|Änderung|Beta|Die Eigenschaften **deviceDisplayName** und **userPrincipalName** wurden den Entitäten [deviceConfigurationDeviceStatus](/graph/api/resources/intune-deviceconfig-deviceconfigurationdevicestatus?view=graph-rest-beta), [deviceComplianceDeviceStatus](/graph/api/resources/intune-deviceconfig-devicecompliancedevicestatus?view=graph-rest-beta) und [managedDeviceMobileAppConfigurationDeviceStatus](/graph/api/resources/intune-apps-manageddevicemobileappconfigurationdevicestatus?view=graph-rest-beta) hinzugefügt.|
|Änderung|Beta|Die **ruleName**-Eigenschaft wurde der [deviceComplianceScheduledActionForRule](/graph/api/resources/intune-deviceconfig-devicecompliancescheduledactionforrule?view=graph-rest-beta)-Entität hinzugefügt.|
|Änderung|Beta|Die Eigenschaften **devicesCount**, **userDisplayName** und **userPrincipalName** wurden den Entitäten [deviceConfigurationUserStatus](/graph/api/resources/intune-deviceconfig-deviceconfigurationuserstatus?view=graph-rest-beta), [deviceComplianceUserStatus](/graph/api/resources/intune-deviceconfig-devicecomplianceuserstatus?view=graph-rest-beta) und [managedDeviceMobileAppConfigurationUserStatus](/graph/api/resources/intune-apps-manageddevicemobileappconfigurationuserstatus?view=graph-rest-beta) hinzugefügt.|
|Änderung|Beta|Die [notificationMessageTemplates](/graph/api/resources/intune-notification-notificationmessagetemplate?view=graph-rest-beta)-Sammlung wurde dem [deviceManagement](/graph/api/resources/intune-deviceconfig-devicemanagement?view=graph-rest-beta)-Singleton hinzugefügt.|
|Änderung|Beta|Die Eigenschaften **isDefault**, **lastModifiedDateTime**, **locale**, **messageTemplate** und **subject** wurden der [localizedNotificationMessage](/graph/api/resources/intune-deviceconfig-localizednotificationmessage?view=graph-rest-beta)-Entität hinzugefügt.|
|Änderung|Beta|Die Eigenschaften **azureActiveDirectoryDeviceId**, **deviceCategory**, **deviceRegistrationState** und **managementAgent** wurden der [managedDevice](/graph/api/resources/intune-onboarding-manageddevice?view=graph-rest-beta)-Entität hinzugefügt.|
|Änderung|Beta|Die **lastModifiedDateTime**-Eigenschaft wurde der [mobileAppCategory](/graph/api/resources/intune-apps-mobileappcategory?view=graph-rest-beta)-Entität hinzugefügt.|
|Änderung|Beta|Die Eigenschaften **brandingOptions**, **defaultLocale**, **displayName**, **fromEmailAddress**, **lastModifiedDateTime** und **localizedNotificationMessages** wurden der [notificationMessageTemplate](/graph/api/resources/intune-notification-notificationmessagetemplate?view=graph-rest-beta)-Entität hinzugefügt.|
|Änderung|Beta|Die Eigenschaften **appsAllowTrustedAppsSideloading**, **appsBlockWindowsStoreOriginatedApps**, **developerUnlockSetting**, **edgeBlockAccessToAboutFlags**, **edgeBlockDeveloperTools**, **edgeBlockExtensions**, **edgeBlockInPrivateBrowsing**, **edgeFirstRunUrl**, **edgeHomepageUrls**, **gameDvrBlocked**, **settingsBlockAddProvisioningPackage**, **settingsBlockChangeLanguage**, **settingsBlockChangePowerSleep**, **settingsBlockChangeRegion**, **settingsBlockChangeSystemTime**, **settingsBlockEditDeviceName**, **settingsBlockRemoveProvisioningPackage**, **sharedUserAppDataAllowed**, **smartScreenBlockPromptOverride**, **smartScreenBlockPromptOverrideForFiles**, **storageRestrictAppDataToSystemVolume**, **storageRestrictAppInstallToSystemVolume**, **webRtcBlockLocalhostIpAddress**, **windowsStoreBlockAutoUpdate** und **windowsStoreEnablePrivateStoreOnly** wurden der [windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta)-Entität hinzugefügt.|

## <a name="december-2016"></a>Dezember 2016

### <a name="delta-query"></a>Delta-Abfrage

| **Änderungstyp** | **Version** | **Beschreibung**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Ergänzungen        | Beta        | Eine neue Deltafunktion zu folgenden Elemente hinzufügen, um [Delta Abfrage](delta-query-overview.md) auszuführen:<br/>contact<br/>contactFolder<br/>event<br/>group<br/>mailFolder<br/>message<br/>user<br/>Beispiele finden Sie unter Folgendem:<br/>
  [Inkrementelle Änderungen an Gruppen abrufen (Vorschau)](delta-query-groups.md)<br/>[Inkrementelle Änderungen an Nachrichten in einem Ordner abrufen (Vorschau)](delta-query-messages.md)<br/>[Inkrementelle Änderungen an Benutzern abrufen (Vorschau)](delta-query-users.md) |

### <a name="excel-apis"></a>Excel-APIs

| **Änderungstyp** | **Version** | **Beschreibung**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Ergänzungen        | v1.0        | workbookPivotTable-Ressource, refresh- und refreshAll-Aktion für pivotTables, workbookRangeView-Ressource, visibleView-Aktion für den gefilterten Bereich zum Zurückgeben von workbookRangeView an den Benutzer, Abrufen der Sammlung rows und range-Ressource deaktiviert für visibleView, Funktionen columnsAfter, columnsBefore, resizedRange, rowsAbove und rowsBelow deaktiviert für range-Ressource und neue Tabelleneigenschaften hinzugefügt. |

### <a name="intune-apis"></a>Intune APIs

| **Änderungstyp** | **Version** | **Beschreibung**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Ergänzungen        | Beta        | Ressourcen und Methode-APIs für Microsoft Intune hinzugefügt. Dies ist eine große Gruppe von Ressourcen und Methoden, um die öffentliche Vorschau von Intune auf Azure-Portal zu unterstützen. Informationen über den Dienst Intune finden Sie unter der [Intune Dokumentation](https://go.microsoft.com/fwlink/?linkid=836405). Informationen zu den Intune Ressourcen und APIs finden Sie unter [Arbeiten mit Intune in Microsoft Graph](/graph/api/resources/intune-graph-overview?view=graph-rest-beta). |

## <a name="october-2016"></a>Oktober 2016

### <a name="authorization-provider"></a>Autorisierungsanbieter

| **Änderungstyp** | **Version**   | **Beschreibung**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Ergänzungen        | v1.0 und Beta | Der v2-Authentifizierungsendpunkt unterstützt jetzt die OAuth-Clientgenehmigung „_credentials“, die für [Dämone und lange ausgeführte Prozesse in Geschäftsszenarien](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) verwendet werden kann. |
| Ergänzungen        | v1.0 und Beta | Der v2-Authentifizierungsendpunkt unterstützt jetzt [Berechtigungsbereiche, die die Zustimmung des Administrators erfordern](permissions-reference.md), über den [Administratorzustimmungs-Endpunkt](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent#admin-restricted-permissions). |
| Ergänzungen        | v1.0 und Beta | Der v2-Authentifizierungsendpunkt unterstützt jetzt die Administratorzustimmung für alle Benutzer in einem Mandanten über die [Administratorzustimmungs-Endpunkt](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent#admin-restricted-permissions). |

### <a name="invitation-apis"></a>Einladungs-APIs

| **Änderungstyp** | **Version** | **Beschreibung**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Ergänzungen        | Beta        | Die invitedUserType-Eigenschaft wurde dem Einladungsentitätstyp hinzugefügt, der den Typ von Benutzer definiert (**Gast** oder **Mitglied**), der eingeladen wird. |
| Löschung        | Beta        | Die invitedToGroups-Eigenschaft wird am 11.11.2016 aus dem Einladungsentitätstyp entfernt. Dies bedeutet, dass Sie mithilfe dieser API keinen eingeladenen Benutzer mehr zu einer Gruppe hinzufügen können. Verwenden von [API zum Hinzufügen von Mitglieder](/graph/api/group-post-members?view=graph-rest-1.0) zum Hinzufügen eines Benutzers zu einer Gruppe. |

## <a name="september-2016"></a>September 2016

### <a name="azure-ad-application-proxy"></a>Azure AD-Anwendungsproxy

| **Änderungstyp** | **Version** | **Beschreibung**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Ergänzungen        | Beta        | Azure AD-Anwendungsproxy-APIs sind jetzt im Beta-Endpunkt von Microsoft Graph verfügbar. Diese APIs ermöglichen die sichere Veröffentlichung von lokalen Anwendungen für Benutzer außerhalb des Organisationsnetzwerks unter Verwendung von Azure AD als allgemeine Zugriffssteuerebene. Mit den veröffentlichten APIs können Sie Anwendungen schreiben, die verschiedene Aspekte vom Anwendungsproxy abrufen und aktualisieren können, u. a. _Connectors_, _connectorGroups_ und _onPremisesPublishing_-Einstellungen einer Anwendung. |

### <a name="drive"></a>Laufwerk

| **Änderungstyp** | **Version** | **Beschreibung**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Ergänzungen        | Beta        | Die _freigegebene_ Sammlung wurde hinzugefügt, um Zugriff auf freigegebene driveItems über shareId oder Freigabe-URL zu ermöglichen. |
| Ergänzungen        | Beta        | Die _search_-Funktion wurde zu einem Laufwerk hinzugefügt, um mehr Elemente als nur die im Stammordner des Laufwerks durchsuchen zu können. |


### <a name="driveitem"></a>DriveItem

| **Änderungstyp** | **Version** | **Beschreibung**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Ergänzungen        | Beta        | Zusätzliche Unterstützung für _createUploadSession_, sodass Dateien, die größer als 4 MB sind, in OneDrive, OneDrive for Business und SharePoint-Dokumentbibliotheken hochgeladen werden können. |
| Ergänzungen        | Beta        | Die_sharepointIds_-Eigenschaft für driveItem wurde hinzugefügt, mit der die herkömmlichen IDs für SharePoint API für in SharePoint gespeicherte driveItems-Elemente zurückgegeben werden. |
| Ergänzungen        | Beta        | Zusätzliche Eigenschaften für _remoteItem_ hinzugefügt. |
| Ergänzungen        | Beta        | _quickXorHash_-Wert für Dateien in OneDrive for Business hinzugefügt. |
| Ergänzungen        | Beta        | Bereich für _createSharingLink_ hinzugefügt, mit dem Unternehmen freizugebende Links oder anonyme freizugebende Links erstellen können. |

### <a name="extended-properties"></a>Erweiterte Eigenschaften

| **Änderungstyp** | **Version** | **Beschreibung**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Ergänzungen        | v1.0        | [Erweiterte Eigenschaften](/graph/api/resources/extended-properties-overview?view=graph-rest-1.0) werden jetzt von folgenden Ressourcen unterstützt: Nachricht, mailFolder, Ereignis, Kalender, Kontakt, contactFolder, Gruppenereignis, Gruppenkalender, Gruppenbeitrag. |

### <a name="groups"></a>Gruppen

Unterstützung für dynamische Gruppenmitgliedschaft über die öffentliche Vorschau-API hinzugefügt, einschließlich der aufgelisteten Zusätze in der folgenden Tabelle:

| **Änderungstyp** | **Version** | **Beschreibung**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Ergänzungen        | Beta        | Hinzugefügte **membershipRule**-Eigenschaft enthält Regeln, die die Mitgliedschaften für diese Gruppe steuern, wenn es sich bei der Gruppe um eine dynamische Gruppe handelt. |
| Ergänzungen        | Beta        | Die **membershipRuleProcessingState**-Eigenschaft wurde hinzugefügt, mit der gesteuert wird, ob die Verarbeitung dynamischer Mitgliedschaften für diese Gruppe aktiviert oder angehalten ist. |
| Ergänzungen        | Beta        | Legen Sie die **groupTypes**-Eigenschaft so fest, dass sie **„DynamicMembership“** enthält, um die Funktionen der dynamischen Gruppen für diese Gruppe zu erweitern |
| Ergänzungen        | Beta        | Die **preferredLanguage**-Eigenschaft wurde hinzugefügt, um die bevorzugte Sprache für eine Office 365-Gruppe anzugeben. |
| Ergänzungen        | Beta        | Die **theme**-Eigenschaft wurde hinzugefügt, um ein Farbschema für eine Office 365-Gruppe anzugeben. |

### <a name="hybrid-deployment-support"></a>Unterstützung für Hybridbereitstellung

| **Änderungstyp** | **Version** | **Beschreibung**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Ergänzungen        | v1.0        | Apps können Version 1.0 von Outlook-Mail, -Kalender und Kontakte-APIs für den Zugriff auf lokale Postfächer in einer Hybridbereitstellung mit Exchange 2016 mit kumulativem Update 3 (KU3) verwenden. Erfahren Sie mehr über die REST-API-Unterstützung in [Hybridbereitstellungen](hybrid-rest-support.md). **Hinweis:** Wenn Sie diese API-Sets in Version 1.0 verwenden, können Sie jetzt Ihre Apps, einschließlich Produktions-Apps für lokale Postfächer verwenden, die den spezifischen Anforderungen für Hybridbereitstellung entsprechen. Diese Funktion ist derzeit in der Vorschau. |

### <a name="identityriskevents"></a>IdentityRiskEvents

| **Änderungstyp** | **Version** | **Beschreibung**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Änderung          | Beta        | Im Rahmen der Schemaänderungen, bei denen der Typ der zwei location-Eigenschaften durch einen neuen komplexen Typ in dem identityRiskEvents-Endpunkt ersetzt wird, werden die folgenden Eigenschaften für den identityRiskEvents-Endpunkt geändert/hinzugefügt:</br>**location** – geändert von Edm.String zu ComplexType signInLocation.<br/>**previousLocation** – geändert von Edm.String zu ComplexType signInLocation.<br/>**signInLocation** – neuer ComplexType, der Ort, Bundesland, countryOrRegion und geoCoordinates-Eigenschaften enthält.<br/>**geoCoordinates** – neuer ComplexType, der Breiten- und Längengradeigenschaften enthält. |

### <a name="invitation-manager"></a>Einladungs-Manager

| **Änderungstyp** | **Version** | **Beschreibung**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Ergänzungen        | Beta        | Einladungs-Manager-APIs sind jetzt im Beta-Endpunkt von Microsoft Graph verfügbar. Verwenden Sie Einladungs-Manager-APIs, um eine Einladung zum Hinzufügen eines externen Benutzers zu der Organisation zu erstellen. Im Rahmen der Einladung können Sie auch angeben, ob der eingeladene Benutzer zu einer Office 365-Gruppe hinzugefügt werden soll. Weitere Informationen finden Sie im [Einladungs-Manager](/graph/api/resources/invitation?view=graph-rest-beta). |

### <a name="onedrive"></a>OneDrive

| **Änderungstyp** | **Version** | **Beschreibung**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Ergänzungen        | v1.0        | **CreateUploadSession**-Methode für **driveItem** hinzugefügt, die Uploads von großen Dateien und wiederaufnehmbare Uploads ermöglicht. |
| Ergänzungen        | v1.0        | Eigenschaften für das Nachverfolgen von SharePoint-IDs für Elemente aus SharePoint (**sharepointIds**) und eine Eigenschaft zum Identifizieren von Stammordnern (**root**) hinzugefügt. |
| Ergänzungen        | v1.0        | **Shares**-Stammsammlung hinzugefügt, die mit shareIds oder Freigabelinks für den Zugriff auf freigegebene Elemente in OneDrive und SharePoint verwendet werden kann. Gibt den neuen Typ sharedDriveItem zurück. |
| Ergänzungen        | v1.0        | **Invite**-Methode für driveItem zum Hinzufügen von Berechtigungen für Elemente hinzugefügt. |
| Ergänzungen        | v1.0        | **Search**-Methode für das Laufwerk, mit der Elemente im Laufwerk und freigegebene Elemente durchsucht werden können hinzugefügt. |
| Ergänzungen        | v1.0        | **processingMetadata**-Eigenschaft für quickXorHash-Eigenschaft mit komplexem Dateityp für Hashes mit komplexem Typ hinzugefügt. |
| Ergänzungen        | v1.0        | **quickXorHash**-Eigenschaft für Hashes mit komplexem Typ hinzugefügt |

### <a name="outlook-calendar"></a>Outlook-Kalender

| **Änderungstyp** | **Version** | **Beschreibung**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Ergänzungen        | v1.0        | **onlineMeetingUrl**-Eigenschaft zur [Ereignis](/graph/api/resources/event?view=graph-rest-1.0)-Ressource hinzugefügt. |
| Ergänzungen        | Beta        | Die [forward](/graph/api/event-forward?view=graph-rest-beta)-Aktion wurde zur Ereignisressource hinzugefügt. |
| Ergänzungen        | Beta        | Die folgenden Eigenschaften wurden zur [calendar](/graph/api/resources/calendar?view=graph-rest-beta)-Ressource zur Unterstützung der Freigabe von Kalendern hinzugefügt: **canEdit**, **canShare**, **canViewPrivateItems**, **isShared**, **isShareWithMe** und **Besitzer**. |

### <a name="outlook-mail"></a>Outlook-Mail

| **Änderungstyp** | **Version** | **Beschreibung**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Ergänzungen        | v1.0        | [mailboxSettings](/graph/api/resources/mailboxsettings?view=graph-rest-1.0) komplexer Typ, einschließlich der **automaticRepliesSetting**-, **timeZone**- und **Sprache**-Eigenschaften hinzugefügt. |
| Ergänzungen        | v1.0        | **mailboxSettings**-Eigenschaft zur [Benutzer](/graph/api/resources/user?view=graph-rest-1.0)-Ressource hinzugefügt. |
| Ergänzungen        | Beta        | Unterstützung für das Erstellen, Auflisten, Abrufen und Löschen einer oder mehrerer Instanzen von [Erwähnungen](/graph/api/resources/mention?view=graph-rest-beta) in einer Nachricht hinzugefügt. Erwähnungen unterstützen Aufrufe, um die Aufmerksamkeit anderer Benutzer in einer Nachricht zu erhalten. |
| Ergänzungen        | Beta        | Added support for the [getMailTips](/graph/api/user-getmailtips?view=graph-rest-beta) action to get any MailTips for specific recipients. Added the following resources: [automaticRepliesMailTips](/graph/api/resources/automaticrepliesmailtips?view=graph-rest-beta), [mailTips](/graph/api/resources/mailtips?view=graph-rest-beta), [mailTipsError](/graph/api/resources/mailtipserror?view=graph-rest-beta). |

### <a name="query-parameters"></a>Abfrageparameter

| **Änderungstyp** | **Version** | **Beschreibung**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Änderung          | Beta        | Abfrageparameter ohne '$' Präfixe sind ab dem 26.09.2016 unterstützt. Das Präfix '$' in der Abfrageparameter ist optional. Beispiele finden Sie unter [Abfrageparameter ohne $ Präfixe in Microsoft Graph unterstützen](https://dev.office.com/queryparametersinMicrosoftGraph). |

### <a name="sharepoint"></a>SharePoint

| **Änderungstyp** | **Version** | **Beschreibung**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Ergänzungen        | Beta        | Zugriff auf SharePoint-Websites und [-listen nach ID](/graph/api/list-get?view=graph-rest-beta) oder [Pfad/URL](/graph/api/baseitem-getbyurl?view=graph-rest-beta). |
| Ergänzungen        | Beta        | Unterstützung für das [Auflisten, Erstellen, Abrufen und Löschen von Instanzen des listItem-Elements](/graph/api/resources/listitem?view=graph-rest-beta). |

### <a name="users"></a>Benutzer

| **Änderungstyp** | **Version** | **Beschreibung**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Ergänzungen        | Beta        | Schreibgeschützte **refreshTokensValidFromDateTime**-Eigenschaft wurde hinzugefügt, um anzugeben, ab wann die Aktualisierungs- oder Sitzungstoken gültig sind. Alle Token, die vor diesem Zeitpunkt ausgestellt wurden, sind ungültig. Bei jedem Versuch, diese Token zu verwenden, werden Benutzer dazu aufgefordert, sich erneut anzumelden. |
| Ergänzungen        | Beta        | Die **showInAddressList**-Eigenschaft wurde hinzugefügt, mit der gesteuert wird, ob die globale Adressliste von Outlook diesen Benutzer enthalten soll. |
| Ergänzungen        | Beta        | Die **invalidateAllRefreshTokens**-Dienstaktion wurde hinzugefügt, mit der alle Aktualisierungs- und Sitzungstoken des Benutzers, die für Anwendungen ausgestellt wurden, ungültig werden, indem die **refreshTokensValidFromDateTime**-Benutzereigenschaft auf aktuelles Datum und aktuelle Uhrzeit zurückgesetzt wird. |


### <a name="webhooks"></a>Webhooks

| **Änderungstyp** | **Version** | **Beschreibung**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Ergänzungen        | Beta        | Laufwerkstammelemente zu Webhooks als Ressource hinzugefügt, die abonniert werden kann. |

## <a name="august-2016"></a>August 2016

### <a name="contacts"></a>Kontakte

| **Änderungstyp** | **Version** | **Beschreibung**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Ergänzungen        | Beta        | Im Rahmen der Schemaänderungen, bei denen einige Eigenschaften entfernt und entsprechende Sammlungen zu Kontaktendpunkten hinzugefügt wurden, wurden die folgenden Eigenschaften zu Kontaktendpunkten hinzugefügt: _Websites – Collection(ComplexType: Website)_,_Phones – Collection (ComplexType: Phone)_, _PostalAddress – Collection(ComplexType: PhysicalAddress)_. Weitere Informationen finden Sie unter dem Blogeintrag: [Upcoming changes to Contacts and People APIs](https://developer.microsoft.com/office/blogs/upcoming-changes-to-contacts-and-people-apis/). |
| Löschung        | Beta        | Im Rahmen der Schemaänderungen, bei denen einige Eigenschaften entfernt und entsprechende Sammlungen zu Kontaktendpunkten hinzugefügt wurden, wurden die folgenden Eigenschaften von Kontaktendpunkten entfernt: _BusinessHomePage_,_HomePhones_, _MobilePhone1_, _BusinessPhones_, _HomeAddress_, _BusinessAddress_, _OtherAddress_. Weitere Informationen finden Sie unter dem Blogeintrag: [Upcoming changes to Contacts and People APIs](https://developer.microsoft.com/office/blogs/upcoming-changes-to-contacts-and-people-apis/). |

### <a name="excel-apis"></a>Excel-APIs

| **Änderungstyp** | **Version** | **Beschreibung**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Ergänzungen        | v1.0        | Excel REST-API für Microsoft Graph ist nun allgemein verfügbar. Sie können jetzt umfassende und genaue Integrationen mit Excel-Arbeitsmappen in Office 365 erstellen. Weitere Informationen finden Sie unter dem Blogeintrag [Power your apps with the new Excel REST API on the Microsoft Graph](https://developer.microsoft.com/office/blogs/power-your-apps-with-the-new-excel-rest-api/). |

### <a name="people"></a>Kontakte

| **Änderungstyp** | **Version** | **Beschreibung**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Änderung          | Beta        | _WebSite_-Eigenschaft wurde in _Websites_ umbenannt. Weitere Informationen finden Sie unter [Upcoming changes to Contacts and People APIs](https://developer.microsoft.com/office/blogs/upcoming-changes-to-contacts-and-people-apis/). |

### <a name="privileged-identity-management"></a>Privileged Identity Management

| **Änderungstyp** | **Version** | **Beschreibung**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Ergänzungen        | Beta        | REST-APIs für Privileged Identity Management (PIM) sind jetzt im Beta-Endpunkt von Microsoft Graph verfügbar. [Privileged Identity Management](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure) ermöglicht eine Just-In-Time-Aktivierung für privilegierte Azure AD-Rollen wie globaler Administrator, Abrechnungsadministrator usw. Mit den veröffentlichten APIs können Sie Anwendungen schreiben, die privilegierte Rollenzuweisungen abrufen und aktualisieren und Benutzer in Rollen aktivieren. Weitere Informationen finden Sie unter [Microsoft Graph: Azure AD Privileged Identity Management Vorschau-APIs sind verfügbar in Beta](https://developer.microsoft.com/office/blogs/microsoft-graph-azure-ad-privileged-identity-management-apis-beta/) und [Azure AD Privileged Identity Management](/graph/api/resources/privilegedidentitymanagement-root?view=graph-rest-beta). |

## <a name="july-2016"></a>Juli 2016

### <a name="administrative-units"></a>Administrative Einheiten

| **Änderungstyp** | **Version** | **Beschreibung**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Ergänzungen        | Beta        | Die neue Administrative Unites preview API wurde eingeführt. Mit administrativen Einheiten können Organisationen ihre Azure Active Directory-Umgebung aufteilen und administrative Aufgaben auf diese Unterteilungen weitergeben. Unterteilungen können Regionen, Abteilungen, Kostenstellen usw. darstellen. Dies kann jetzt über die Microsoft Graph-API verwaltet werden. |

## <a name="june-2016"></a>Juni 2016

### <a name="identityriskevents"></a>IdentityRiskEvents

|**Änderungstyp**|**Version**|**Beschreibung**|
|:--------------|:-----------|:--------------|
|Ergänzungen|Beta|Die neue  IdentityRiskEvents Vorschau-API wurde eingeführt. Diese API funktioniert in Verbindung mit Azure Active Directory Identity Protection. Sie können Abfrage-Risiko-Ereignissen abfragen, die durch Identity Protection generiert wurden. Weitere Informationen finden Sie unter [Einführung einer neuen Vorschau-API für Microsoft Graph: IdentityRiskEvents](https://developer.microsoft.com/office/blogs/identityriskevents-api-preview/)-Blogeintrag.

### <a name="subscriptions"></a>Abonnements

| **Änderungstyp** | **Version** | **Beschreibung**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Ergänzungen        | Beta        | Nur App-Bereiche werden jetzt für _Mail_- und _Kontakte_-Abonnements unterstützt. |

## <a name="may-2016"></a>Mai 2016

### <a name="calendar"></a>Kalender

|**Änderungstyp**|**Version**|**Beschreibung**|
|:--------------|:-----------|:--------------|
|Änderungen|Beta|Ändert sich zur findmeetingtimes-API. Weitere Informationen finden Sie unter dem Blogeintrag [Microsoft Graph findMeetingTimes API update](https://dev.office.com/microsoft-graph-findmeetingtimes-api-update) Blogbeitrag. Diese Änderung ist seit dem 19. Mai 2016 wirksam.

### <a name="contact"></a>Kontakt

| **Änderungstyp** | **Version** | **Beschreibung**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Ergänzungen        | v1.0        | _Erweiterungen_ hinzugefügt, die einen abstrakten Typ für die Unterstützung des offenen Typs openTypeExtension von OData v4 darstellen. |

### <a name="directory"></a>Verzeichnis

| **Änderungstyp** | **Version** | **Beschreibung**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Änderungen | Beta        | _settingTemplateId_ in _templateId_ umbenannt. Diese Änderung wird ab dem 19. Mai 2016 wirksam. |

### <a name="event"></a>Ereignis

| **Änderungstyp** | **Version** | **Beschreibung**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Ergänzungen        | v1.0        | _Erweiterungen_ hinzugefügt, die einen abstrakten Typ für die Unterstützung des offenen Typs openTypeExtension von OData v4 darstellen. |

### <a name="eventmessages"></a>EventMessages

| **Änderungstyp** | **Version** | **Beschreibung**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Ergänzungen        | v1.0        | _inferenceClassification_ und _Erweiterungen_ zu _eventMessages_ hinzugefügt. |
| Ergänzungen        | Beta        | _responseRequested_ zu _eventMessageRequest_ hinzugefügt. |

### <a name="messages"></a>Nachrichten

| **Änderungstyp** | **Version** | **Beschreibung**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Ergänzungen        | v1.0        | _inferenceClassification_ und _extensions_ zu _Nachrichten_ hinzugefügt. |
| Ergänzungen        | Beta        | _wellknownname_ zu _contactFolder_ hinzugefügt. |

### <a name="post"></a>Beitrag

| **Änderungstyp** | **Version** | **Beschreibung**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Ergänzungen        | v1.0        | _Erweiterungen_ hinzugefügt, die einen abstrakten Typ für die Unterstützung des offenen Typs openTypeExtension von OData v4 darstellen. |

### <a name="user"></a>Benutzer

| **Änderungstyp** | **Version** | **Beschreibung**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Ergänzungen        | v1.0        | _inferenceClassification_-Ressourcentyp hinzugefügt. |
| Ergänzungen        | Beta        | _timeZone_ zu _mailboxsettings_ hinzugefügt.   |
| Ergänzungen        | Beta        | API _findMeetingTimes _ zu _Benutzer_ hinzugefügt.   |

## <a name="april-2016"></a>April 2016

### <a name="general"></a>Allgemein

| **Änderungstyp** | **Version**   | **Beschreibung**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Ergänzungen        | v1.0 und Beta | Unterstützung für Berücksichtigung von _Accept-Encoding:gzip_ hinzugefügt. |
| Ergänzungen        | v1.0          | Added support for cast segment in expand path. For example, 'https://graph.microsoft.com/v1.0/me/messages?$expand=microsoft.graph.eventMessage/event'. |
| Ergänzungen        | Beta          | Unterstützung für PATCH-Anforderung anhand struktureller Eigenschaften hinzugefügt. Beispiel: 'PATCH /me/mailboxSettings'. |
| Ergänzungen        | Beta          | Azure Active Directory dient nun als Alternative für /beta/users/id/photo-Anforderungen, wenn Outlook die Anforderung nicht verarbeiten kann, beispielsweise wenn der Benutzer über keine Postfachlizenz oder der Mandant über kein Exchange Online-Abonnement verfügt. HINWEIS: Diese Alternative steht für GET und PATCH zur Verfügung. |
| Ergänzungen        | Beta          | Added support for cast segment in expand path. For example: 'https://graph.microsoft.com/v1.0/me/messages?$expand=microsoft.graph.eventMessage/event'. |

### <a name="onedrive"></a>OneDrive

| **Änderungstyp** | **Version** | **Beschreibung**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Behebung             | v1.0        | Behebung eines Problems, aufgrund dessen bei createLink-Anforderungen OneDrive den 500-Fehler mit der Meldung „Nicht unterstützter Erweiterungseigenschaftentyp.“ zurückgab. |

## <a name="march-2016"></a>März 2016

### <a name="calendar"></a>Kalender

| **Änderungstyp** | **Version** | **Beschreibung**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Ergänzungen        | Beta        | _singleValueExtendedProperties_ und _multiValueExtendedProperties_-Eigenschaften hinzugefügt. |
| Ergänzungen        | Beta        | _suggestionHint_-Eigenschaft zu _meetingTimeCandidate _ hinzugefügt. |
| Ergänzungen        | Beta        | _locationUri_-Eigenschaft zu _location_ hinzugefügt. |
| Ergänzungen        | Beta        | _type_ und _postOfficeBox_ zu _physicalAddress _ hinzugefügt. |
| Änderung          | Beta        | _findMeetingTimes_ verwendet jetzt den neuen _ReturnSuggestionHints_-Parameter. |
| Änderung          | Beta        | _findMeetingTimes_ gibt jetzt eine Sammlung von _meetingTimeCandidate_ zurück. |

### <a name="drive"></a>Laufwerk

| **Änderungstyp** | **Version**   | **Beschreibung**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Ergänzungen        | v1.0 und Beta | _recent_-Funktion zum Auflisten eines Satzes von Elementen hinzugefügt, die zuletzt von dem angemeldeten Benutzer verwendet wurden. Diese Liste enthält Elemente, die sich in dem Laufwerk des Benutzers befinden sowie Elemente in anderen Laufwerken, auf die dieser Zugriff hat. Beispiel: GET /me/drive/recent. |
| Ergänzungen        | v1.0 und Beta | _sharedWithMe_-Funktion zum Auflisten des Satzes von Elementen hinzugefügt, die für den aktuellen Benutzer freigegeben sind. Beispiel: GET /me/drive/sharedWithMe. |

### <a name="driveitem"></a>DriveItem

| **Änderungstyp** | **Version**   | **Beschreibung**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Ergänzungen        | v1.0 und Beta | _remoteItem_-Typ zum Bereitstellen eines Links zu einem Element in einem anderen Laufwerk hinzugefügt. |
| Ergänzungen        | v1.0 und Beta | _sharingInvitation_-Typ hinzugefügt, um Details zu verknüpften Einladungen zur Freigabe für diese Berechtigung bereitzustellen. |
| Ergänzungen        | v1.0 und Beta | _delta_-Funktion zum Nachverfolgen von Änderungen an Elementen in einem Laufwerk hinzugefügt. Beispiel: GET /me/drive/items/{item-id}/delta |
| Ergänzungen        | v1.0 und Beta | _copy_-Funktion zum Erstellen einer Kopie eines _driveItem_-Elements (einschließlich untergeordneter Elemente) unter einem neuen übergeordneten Element oder unter einem neuen Namen hinzugefügt. Beispiel: POST /me/drive/items/{item-id}/copy |
| Ergänzungen        | v1.0 und Beta | _conflictBehavior_-Instanzattribute sind nun auf _driveItem_ anwendbar. |
|Ergänzungen|Beta|_invite_-Funktion zum Senden einer Einladung zur Freigabe für ein vorhandenes Element hinzugefügt. Mit einer Einladung zur Freigabe werden ein Freigabelink erstellt und eine E-Mail-Nachricht an den Empfänger die Einladung mit dem Freigabelink gesendet. Beispiel: POST /drive/items/{item-id}/invite

### <a name="event"></a>Ereignis

| **Änderungstyp** | **Version** | **Beschreibung**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Ergänzungen        | Beta        | Neue _onlineMeetingUrl_-Eigenschaft und neue _cancel_-Methode hinzugefügt. |

### <a name="event-messages"></a>Ereignismeldungen

| **Änderungstyp** | **Version** | **Beschreibung**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Ergänzungen        | Beta        | _startDateTime_, _endDateTime_, _location_, _type_, _recurrence_, _isOutOfDate_, _conversationIndex_, _unsubscribe_, _unsubscribeData_, _unsubscribeEnabled_ und _flag_-Eigenschaften zum _eventmessage_-Objekt hinzugefügt. |
| Ergänzungen        | Beta        | _singleValueExtendedProperties_ und _multiValueExtendedProperties_-Eigenschaften hinzugefügt. |
| Ergänzungen        | Beta        | Neue _unsubscribe_-Methode hinzugefügt.          |

### <a name="excel"></a>Excel

| **Änderungstyp** | **Version** | **Beschreibung**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Ergänzungen        | Beta        | Es wurden neue REST-APIs für Excel hinzugefügt, mit denen Sie Daten in einer Excel-Arbeitsmappe lesen und ändern können. Sie können nun intelligente Apps erstellen, mit denen Benutzer die in Excel-Arbeitsmappen gespeicherten Inhalte nutzen können, indem Einblicke in die Daten bereitgestellt werden. Profitieren Sie von den Vorteilen der Analysefunktionen von Excel, erstellen Sie Tabellen und Diagramme und extrahieren Sie optisch ansprechende Diagramme, und das alles von Ihrer App aus. Weitere Informationen finden Sie unter [Arbeiten mit Excel in Microsoft Graph](/graph/api/resources/excel?view=graph-rest-beta). |

### <a name="general"></a>Allgemein

| **Änderungstyp** | **Version**   | **Beschreibung**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Ergänzungen        | v1.0 und Beta | Verbesserung von Fehlermeldungen beim Auflösen von Mandantenalias- und abgelehnten JWT-Token (AAD). |
| Ergänzungen        | v1.0 und Beta | Der Ort für den Autorisierungsdienstendpunkt wird jetzt in dem _www-authenticate_-Header zurückgegeben, wenn eine Anforderung mit einem leeren Bearertoken empfangen wird. |
| Ergänzungen        | v1.0 und Beta | The ability to filter on an entity's id property is now fixed. Example: GET https://graph.microsoft.com/v1.0/users?$filter=id+eq+'x'<br/>Previously, any POST requests to service actions and functions require prefixing the action or function name with the microsoft.graph prefix. For example: POST https://graph.microsoft.com/v1.0/me/Microsoft.Graph.getMemberGroups.<br/>The prefix is now no longer required (although it can still be specified). So the following would now also work: POST https://graph.microsoft.com/v1.0/me/getMemberGroups. |
| Änderung          | Beta          | Abonnement-Eigenschaftennamen bereinigt.  |
| Ergänzungen        | Beta          | Wir haben die Möglichkeit zum Ermitteln von (über _directorySettingTemplates_) und Außerkraftsetzen des Standardverhaltens (durch Erstellen einer _Einstellung_ aus der Vorlage) für Entitäten und die zugehörigen Funktionen hinzugefügt. Anfangs konnten die Verhaltensweisen für Office-Gruppen nur über die Vorlage gesteuert werden. |

### <a name="mail-folder"></a>Mail-Ordner

| **Änderungstyp** | **Version** | **Beschreibung**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Ergänzungen        | Beta        | _wellKnownName_- und _userConfigurations_-Eigenschaften hinzugefügt. |
| Ergänzungen        | Beta        | _singleValueExtendedProperties_- und _multiValueExtendedProperties_-Eigenschaften hinzugefügt |

### <a name="messages"></a>Nachrichten

| **Änderungstyp** | **Version**   | **Beschreibung**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Ergänzungen        | v1.0          | _mobilePhone_-Eigenschaft hinzugefügt.            |
| Ergänzungen        | v1.0 und Beta | _internetMessageId_-Eigenschaft hinzugefügt. Die Nachrichten-ID im von [RFC2822](https://www.ietf.org/rfc/rfc2822.txt) angegebenen Format. |
| Ändern          | Beta          | _mobilePhone1_-Eigenschaft in _mobilePhone_ umgenannt. |
| Änderung          | Beta          | _createReply_ und _createReplyAll _ verwenden neue _Message_- und _comment_-Parameter. |
| Änderung          | Beta          | _createForward_ verwendet neue _Message_-, _ToRecipients_- und _comment_-Parameter. |
| Änderung          | Beta          | _reply_, _replyAll_ und _forward_ verwenden neue _Message_-Parameter. |

### <a name="permission"></a>Berechtigung

| **Änderungstyp** | **Version**   | **Beschreibung**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Ergänzungen        | v1.0 und Beta | _sharingInvitation_-Eigenschaft hinzugefügt, um Details zu verknüpften Einladungen zur Freigabe für diese Berechtigung bereitzustellen. |

### <a name="person"></a>Person

| **Änderungstyp** | **Version** | **Beschreibung**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Ergänzungen        | Beta        | - Neue _birthday_-, _personNotes_-, _isFavorite_-, _phones_-, _permission_-, _postalAddresses_-,_websites_-,_yomiCompany_-, _department_-, _profession_-, _mailboxType_- und _personType_-Eigenschaften hinzugefügt. |
| Ergänzungen        | Beta        | Neue Enumerationstypen hinzugefügt: _physicalAddressType_, _webSite_, _phone_ und _webSiteType_. |

### <a name="reference-attachment"></a>Verweisanlage

| **Änderungstyp** | **Version** | **Beschreibung**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Ergänzungen        | Beta        | Neue Eigenschaften hinzugefügt: _sourceUrl_, _providerType_, _thumbnailUrl_, _previewUrl_, _permission_ und _isFolder_. |
| Ergänzungen        | Beta        | _singleValueExtendedProperties_ und _multiValueExtendedProperties_-Eigenschaften hinzugefügt. |
| Ergänzungen        | Beta        | Neue Enumerationstypen _referenceAttachmentProvider_ und _referenceAttachmentPermission_. hinzugefügt. |

### <a name="subscriptions"></a>Abonnements

| **Änderungstyp** | **Endpunkt** | **Beschreibung**                          |
| :-------------- | :----------- | :--------------------------------------- |
| Ergänzungen        | v1.0         | Webhooks are now GA on v1.0 endpoint via the _/Subscriptions_ resource. Create, Read, Renew and Delete subscriptions to receive notifications on data from Outlook and Office 365 group conversations. |

### <a name="user"></a>Benutzer

| **Änderungstyp** | **Version** | **Beschreibung**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Ergänzungen        | Beta        | _mailboxSettings_-Eigenschaft sowie die entsprechenden Typen hinzugefügt. |

## <a name="february-2016"></a>Februar 2016

### <a name="driveitem"></a>DriveItem

| **Änderungstyp** | **Version**   | **Beschreibung**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Ergänzungen        | v1.0 und Beta | Neue _remoteItem_-Eigenschaft für driveItem für Microsoft-Konten. |

### <a name="general"></a>Allgemein

| **Änderungstyp** | **Version**   | **Beschreibung**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Änderung          | v1.0 und Beta | -_/me/drive_ funktioniert nun für Microsoft-Konten und Geschäfts-, Schul- und Uni-Konten. |
| Änderung          | v1.0 und Beta | Laufwerkanforderungen für Konten, deren OneDrive-Speicher bei Bedarf bereitgestellt wurde, funktionieren zuverlässig und können in mehr Szenarien verwendet werden, in denen die SharePoint-Standardwebsites des Mandanten nicht standardmäßige Namen verwenden. |
| Löschung        | Beta          | Verschiedene nicht implementierte Typen aus dem Betaschema zur Anpassung an 1.0 Schema entfernt. |

### <a name="subscriptions"></a>Abonnements

| **Änderungstyp** | **Version** | **Beschreibung**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Ergänzungen        | Beta        | notificationUrl-Validierung bei Abonnement-Erstellung. Weitere Informationen finden Sie unter [Microsoft Graph WebHooks Update - January 2016](https://developer.microsoft.com/office/blogs/Microsoft-Graph-WebHooks-Update-January-2016/). |
| Ergänzungen        | Beta        | Abonnemententitäten können jetzt gelöscht werden: DELETE https://graph.microsoft.com/beta/subscriptions/ |

### <a name="users"></a>Benutzer

| **Änderungstyp** | **Version**   | **Beschreibung**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Änderung          | v1.0 und Beta | _displayName_ wird jetzt für Microsoft-Konten zurückgegeben. |

## <a name="january-2016"></a>Januar 2016

### <a name="contacts"></a>Kontakte

| **Änderungstyp** | **Version** | **Beschreibung**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Ergänzungen        | v1.0        | mobilePhone-Eigenschaft zum Entitätssatz für persönliche Kontakte hinzugefügt. |

### <a name="directoryobjects"></a>directoryObjects

| **Änderungstyp** | **Version**   | **Beschreibung**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Behebung             | v1.0 und Beta | Behebung eines Problems mit Aufrufaktionen, die mit directoryObjects verknüpft sind und zu dem folgenden Fehler führten:  „Der Rückgabetyp des Vorgangs ist mit dem vorgegebenen Entitätssatz nicht möglich“. Dies gilt für die folgenden Aktionen: _microsoft.graph.checkMemberObjects_, _microsoft.graph.getMemberObjects_, _microsoft.graph.checkMemberGroups_, _microsoft.graph.assignLicense_, _microsoft.graph.changePassword_. |

## <a name="december-2015"></a>Dezember 2015

### <a name="contacts"></a>Kontakte

| **Änderungstyp** | **Version** | **Beschreibung**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Ergänzungen        | Beta        | mobilePhone-Eigenschaft zum Entitätssatz für persönliche Kontakte hinzugefügt. |

### <a name="general"></a>Allgemein

| **Änderungstyp** | **Version**   | **Beschreibung**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Behebung             | v1.0 und Beta | Behebung eines Problems mit Anforderungen mit $filter-Ausdrücken, die mehrmals die gleiche Eigenschaft angegebenen haben, was zu dem folgenden 500-Fehler führte: Ein Element mit diesem Schlüssel wurde bereits hinzugefügt. |
| Behebung             | v1.0 und Beta | Behebung eines Problems mit der Groß-/Kleinschreibung für Aktionsparameternamen und -werte. |
| Behebung             | v1.0 und Beta | Behebung eines Problems mit der Verarbeitung von Anforderungen für Nutzlasten mit Nullwerten für einige eingebettete komplexe Eigenschaften, aufgrund dessen ein Fehler mit einer Nullverweisausnahme auftrat. |
| Ergänzungen        | v1.0 und Beta | Unterstützung für das Sortieren und Filtern von komplexen Type-Eigenschaften. |
| Ergänzungen        | v1.0 und Beta | authorization_uri-Eigenschaft in dem www-authenticate-Header einer 401-Antwort hinzugefügt. Dieser URI kann verwendet werden, um den Tokenerwerbfluss zu starten. |
| Ergänzungen        | v1.0 und Beta | Verbesserte Fehlermeldungen für Benutzer und Gruppen. |

### <a name="groups"></a>Gruppen

| **Änderungstyp** | **Version**   | **Beschreibung**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Behebung             | v1.0 und Beta | Behebung eines Problems mit dem Aufruf folgender Gruppenaktionen: _microsoft.graph.addFavorite_, _microsoft.graph.removeFavorite_ and _microsoft.graph.resetUnseenCount_. |

### <a name="messages"></a>Nachrichten

| **Änderungstyp** | **Version** | **Beschreibung**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Ergänzungen        | Beta        | eventMessageRequest-Untertyp der eventMessage- und startDateTime-, endDateTime-, location-, type-, recurrence- und IsOutOfDate-Eigenschaften zum eventMessag-Typ hinzugefügt. |

### <a name="users"></a>Benutzer

| **Änderungstyp** | **Version**   | **Beschreibung**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Behebung             | v1.0 und Beta | Fixed being able to select certain user properties on other users, when referencing the user by user principal name (UPN). For example: https://graph.microsoft.com/v1.0/users/anotherUser@contoso.com?$select=aboutMe |
| Behebung             | v1.0 und Beta | Behebung eines Problems mit dem Aufruf der benutzergebundenen _microsoft.graph.reminderView_-Funktion, aufgrund dessen der folgende Fehler auftrat: „Eine Eigenschaft mit dem Namen 'businessPhones' vom Typ 'Microsoft.OutlookServices.Reminder' konnte nicht gefunden werden.“ |
| Behebung             | v1.0 und Beta | Behebung eines Problems mit der Erstellung und Aktualisierung von Benutzern (POST/PATCH /v1.0/users), aufgrund dessen der 400-Fehler auftrat. |
