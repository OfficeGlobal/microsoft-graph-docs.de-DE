# <a name="changelog-for-microsoft-graph"></a>Änderungsprotokoll für Microsoft Graph

Dieses Änderungsprotokoll deckt alle Änderungen in Microsoft Graph ab, einschließlich der Version 1.0 und des Beta-Endpunkts von Microsoft Graph-APIs.  

Ausführliche Informationen zu bekannten Problemen mit Microsoft Graph-APIs finden Sie unter [Bekannte Probleme](known_issues.md).

## <a name="august-2017"></a>August 2017

### <a name="onenote"></a>OneNote

|**Änderungstyp**|**Version**|**Beschreibung**|
|:-------------|:-----------|:--------------|
| Ergänzungen | v1.0 und Beta | Die Navigationseigenschaft [onenote](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/onenote.md) wurde zu **site** hinzugefügt.  |
| Ergänzungen | Beta | Die Zielparameter *siteCollectionId* und *siteId* für Kopiervorgänge. Beispiel: [CopyNotebook](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/api/notebook_copynotebook.md). |


## <a name="july-2017"></a>Juli 2017

### <a name="group-settings"></a>Gruppeneinstellungen

|**Änderungstyp**|**Version**|**Beschreibung**|
|:-------------|:-----------|:--------------|
| Ergänzungen     | v1.0       | Unterstützung für Gruppeneinstellungen wurde hinzugefügt.<br/>Neue Ressourcentypen: [groupSetting](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/groupsetting.md), [groupSettingTemplate](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/groupsettingtemplate.md), [settingValue](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/settingvalue.md) und [settingTemplateValue](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/settingtemplatevalue.md) |
| Änderung       | v1.0       | Eigenschaft **classification** und Navigationseigenschaft **settings** wurden zu [group](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/group.md) hinzugefügt. |

### <a name="intune-apis"></a>Intune APIs

|Typ&nbsp;ändern|Version|Beschreibung|
|:---|:---|:---|
|Ergänzungen|Beta|Die [assign](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_apps_iosmobileappconfiguration_assign.md)-Aktion wurde zu [iosMobileAppConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_iosmobileappconfiguration) hinzugefügt. |
|Ergänzungen|Beta|Die [syncDevice](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_devices_manageddevice_syncdevice.md)-Aktion wurde zu [managedDevice](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_manageddevice) hinzugefügt. |
|Änderung|Beta|Die Eigenschaften **appsInstallAllowList**, **appsLaunchBlockList** und **appsHideList** wurden zur Entität [androidGeneralDeviceConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidgeneraldeviceconfiguration) hinzugefügt.|
|Änderung|Beta|Die Eigenschaft **disableAppEncryptionIfDeviceEncryptionIsEnabled** wurde zur Entität [androidManagedAppProtection](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_androidmanagedappprotection) hinzugefügt.|
|Änderung|Beta|Die Eigenschaft **disableAppEncryptionIfDeviceEncryptionIsEnabled** wurde zur Entität [defaultManagedAppProtection](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_defaultmanagedappprotection) hinzugefügt.|
|Änderung|Beta|Die Eigenschaft **complianceGracePeriodExpirationDateTime** wurde zur Entität [deviceComplianceDeviceStatus](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancedevicestatus) hinzugefügt.|
|Änderung|Beta|Die Eigenschaft **complianceGracePeriodExpirationDateTime** wurde zur Entität [deviceComplianceSettingState](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancesettingstate) hinzugefügt.|
|Änderung|Beta|Die Eigenschaft **complianceGracePeriodExpirationDateTime** wurde zur Entität [deviceConfigurationDeviceStatus](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationdevicestatus) hinzugefügt.|
|Änderung|Beta|Die Eigenschaft **subscriptions** wurde zur Entität [deviceManagement](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_androidforwork_devicemanagement) hinzugefügt.|
|Änderung|Beta|Die Eigenschaft **version** wurde zur Entität [deviceManagementExchangeConnector](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_onboarding_devicemanagementexchangeconnector) hinzugefügt.|
|Änderung|Beta|Die Eigenschaft **utcTimeOffsetInMinutes** wurde zur Entität [iosUpdateConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosupdateconfiguration) hinzugefügt.|
|Änderung|Beta|Die Eigenschaft **complianceGracePeriodExpirationDateTime** wurde zur Entität [iosUpdateDeviceStatus](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosupdatedevicestatus) hinzugefügt.|
|Änderung|Beta|Die Eigenschaft **preSharedKey** wurde zur Entität [macOSWiFiConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_macoswificonfiguration) hinzugefügt.|
|Änderung|Beta|Die Eigenschaften **phoneNumber**, **androidSecurityPatchLevel** und **userDisplayName** wurden zur Entität [managedDevice](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_manageddevice) hinzugefügt.|
|Änderung|Beta|Die Eigenschaften **userName**, **deviceModel**, **platform** und **complianceGracePeriodExpirationDateTime** wurden zur Entität [managedDeviceMobileAppConfigurationDeviceStatus](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_manageddevicemobileappconfigurationdevicestatus) hinzugefügt.|
|Änderung|Beta|Die Eigenschaft **userPrincipalName** wurde zur Entität [mobileAppInstallStatus](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_mobileappinstallstatus) hinzugefügt.|
|Änderung|Beta|Die Eigenschaft **overrideDefaultRule** wurde zur Entität [onPremisesConditionalAccessSettings](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_onboarding_onpremisesconditionalaccesssettings) hinzugefügt.|
|Änderung|Beta|Die Eigenschaft **userPrincipalName** wurde zur Entität [userAppInstallStatus](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_userappinstallstatus) hinzugefügt.|
|Änderung|Beta|Die Eigenschaften **connectAppBlockAutoLaunch**, **deviceAccountBlockExchangeServices**, **deviceAccountEmailAddress**, **deviceAccountExchangeServerAddress**, **deviceAccountRequirePasswordRotation**, **deviceAccountSessionInitiationProtocolAddress**, **settingsBlockMyMeetingsAndFiles**, **settingsBlockSessionResume**, **settingsBlockSigninSuggestions**, **settingsDefaultVolume**, **settingsScreenTimeoutInMinutes**, **settingsSessionTimeoutInMinutes** und **settingsSleepTimeoutInMinutes** wurden zur Entität [windows10TeamGeneralConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10teamgeneralconfiguration) hinzugefügt.|
|Änderung|Beta|Die Navigationseigenschaft **deploymentSummary** wurde zur Entität [defaultManagedAppProtection](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_defaultmanagedappprotection) hinzugefügt.|
|Änderung|Beta|Die Eigenschaften **settingName**, **userId**, **userName**, **userEmail** und **currentValue** wurden zum komplexen Typ [deviceCompliancePolicySettingState](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancepolicysettingstate) hinzugefügt.|
|Änderung|Beta|Die Eigenschaften **settingName**, **userId**, **userName**, **userEmail** und **currentValue** wurden dem komplexen Typ [deviceConfigurationSettingState](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationsettingstate) hinzugefügt.|
|Änderung|Beta|Die Eigenschaft **unknownCount** wurde zum komplexen Typ [deviceOperatingSystemSummary](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_devices_deviceoperatingsystemsummary) hinzugefügt.|



## <a name="june-2017"></a>Juni 2017

### <a name="project-rome"></a>Projekt Rom

|**Änderungstyp**|**Version**|**Beschreibung**|
|:-------------|:-----------|:--------------|
|Ergänzungen|Beta|Folgende Ressourcen und APIs wurden hinzugefügt:<br/>[Aktivität](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/projectrome_activity)<br/>[Aktivität erstellen oder ersetzen](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/projectrome_put_activity)<br/>[Aktivität löschen](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/projectrome_delete_activity)<br/>[Verlaufselement](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/projectrome_historyitem)<br/>[Verlaufselement erstellen oder ersetzen](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/projectrome_put_historyitem)<br/>[Verlaufselement](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/projectrome_delete_historyitem) löschen|

### <a name="outlook-calendar"></a>Outlook-Kalender

|**Änderungstyp**|**Version**|**Beschreibung**|
|:-------------|:-----------|:--------------|
|Ergänzungen|v1.0|Die folgenden vier [calendar](https://graph.microsoft.io/en-us/docs/api-reference/v1.0/resources/calendar)-Eigenschaften wurden auf v1.0 heraufgestuft: **canEdit**, **canShare**, **canViewPrivateItems** und **owner**.|


### <a name="intune-apis"></a>Intune APIs

|Änderungstyp|Version|Beschreibung|
|:---|:---|:---|
|Ergänzungen|Beta|Hinzugefügte neue Entitäten:<br/>[defaultDeviceCompliancePolicy](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_defaultdevicecompliancepolicy)<br/>[deviceConfigurationUserStateSummary](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationuserstatesummary)<br/>[deviceManagementScriptDeviceState](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_devicefe_devicemanagementscriptdevicestate)<br/>[deviceManagementScriptRunSummary](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_devicefe_devicemanagementscriptrunsummary)<br/>[deviceManagementScriptUserState](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_devicefe_devicemanagementscriptuserstate)<br/>[iosUpdateDeviceStatus](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosupdatedevicestatus)<br/>[windowsManagedDevice](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_devicefe_windowsmanageddevice)<br/>[windowsManagementAppHealthState](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_devicefe_windowsmanagementapphealthstate)<br/>[windowsManagementAppHealthSummary](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_devicefe_windowsmanagementapphealthsummary)<br/>|
|Ergänzungen|Beta|Die folgenden kompleen Typen wurden hinzugefügt:<br/>[bitLockerFixedDrivePolicy](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_bitlockerfixeddrivepolicy)<br/>[bitLockerRecoveryOptions](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_bitlockerrecoveryoptions)<br/>[bitLockerRemovableDrivePolicy](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_bitlockerremovabledrivepolicy)<br/>[deleteUserFromSharedAppleDeviceActionResult](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_devicefe_deleteuserfromsharedappledeviceactionresult)<br/>[iosNetworkUsageRule](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosnetworkusagerule)<br/>|
|Löschung|Beta|Die folgenden Entitäten wurden entfernt:<br/>**deviceManagementScriptState**<br/>|
|Löschung|Beta|Die Aktion „wipeByDeviceTag“ für [user](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_devicefe_user) wurde entfernt. |
|Änderung|Beta|Die Eigenschaften **innerAuthenticationProtocolForEapTtls**, **innerAuthenticationProtocolForPeap** und **outerIdentityPrivacyTemporaryValue** wurden zur Entität [androidEnterpriseWiFiConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidenterprisewificonfiguration) hinzugefügt.|
|Änderung|Beta|Die Eigenschaften **nonEapAuthenticationMethodForEapTtls**, **nonEapAuthenticationMethodForPeap** und **enableOuterIdentityPrivacy** wurden von der Entität [androidEnterpriseWiFiConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidenterprisewificonfiguration) entfernt.|
|Änderung|Beta|Hinzugefügt der **DeployedAppCount** -Eigenschaft können Sie die [AndroidManagedAppProtection](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_androidmanagedappprotection) Entität|
|Änderung|Beta|Die Eigenschaften **instanceDisplayName** und **settingPlatform** wurden von er Entität [complianceSettingStateSummary](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/complianceSettingStateSummary) entfernt.|
|Änderung|Beta|Die Eigenschaft **deployedAppCount** wurde zur Entität [defaultManagedAppProtection](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_defaultmanagedappprotection) hinzugefügt.|
|Änderung|Beta|Die **excludeGroup**-Eigenschaft wurde der [deviceCompliancePolicyGroupAssignment](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancepolicygroupassignment)-Entität hinzugefügt.|
|Änderung|Beta|Die Eigenschaften **instanceDisplayName** und **settingPlatform** wurden von der Entität [deviceCompliancePolicySettingStateSummary](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary) entfernt.|
|Änderung|Beta|Die Eigenschaft **devicePlatform** wurde von der Entität [deviceComplianceSettingState](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancesettingstate) entfernt.|
|Änderung|Beta|DieEigenschaften **assignmentStatus**, **assignmentProgress** und **assignmentErrorMessage** wurden zur Entität [deviceConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfiguration) hinzugefügt.|
|Änderung|Beta|Die Eigenschaft **intuneBrand** wurde zur Entität [deviceManagement](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_androidforwork_devicemanagement) hinzugefügt.|
|Änderung|Beta|Die Eigenschaften **enforceSignatureCheck** und **fileName** wurden zur Entität [deviceManagementScript](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_devicefe_devicemanagementscript) hinzugefügt.|
|Änderung|Beta|Die Eigenschaften **innerAuthenticationProtocolForEapTtls** und **outerIdentityPrivacyTemporaryValue** wurden zur Entität [iosEnterpriseWiFiConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosenterprisewificonfiguration) hinzugefügt.|
|Änderung|Beta|Die Eigenschaften **nonEapAuthenticationMethodForEapTtls** und **enableOuterIdentityPrivacy** wurden von der Entität [iosEnterpriseWiFiConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosenterprisewificonfiguration) entfernt.|
|Änderung|Beta|Die Eigenschaften **classroomAppForceUnpromptedScreenObservation**, **keyboardBlockDictation**, **networkUsageRules** und **wiFiConnectOnlyToConfiguredNetworks** wurden zur Entität [iosGeneralDeviceConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosgeneraldeviceconfiguration) hinzugefügt.|
|Änderung|Beta|Die Eigenschaft **deployedAppCount** wurde zur Entität [iosManagedAppProtection](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_iosmanagedappprotection) hinzugefügt.|
|Änderung|Beta|Die Eigenschaft **preSharedKey** wurde zur Entität [iosWiFiConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioswificonfiguration) hinzugefügt.|
|Änderung|Beta|Die Eigenschaften **innerAuthenticationProtocolForEapTtls** und **outerIdentityPrivacyTemporaryValue** wurden zur Entität [macOSEnterpriseWiFiConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_macosenterprisewificonfiguration) hinzugefügt.|
|Änderung|Beta|Die Eigenschaften **nonEapAuthenticationMethodForEapTtls** und **enableOuterIdentityPrivacy** wurden von der Entität [macOSEnterpriseWiFiConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_macosenterprisewificonfiguration) entfernt.|
|Änderung|Beta|Die Eigenschaften **lastModifiedTime** und **deployedAppCount** wurden aus der Entität [managedAppPolicy](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_managedapppolicy) entfernt.|
|Änderung|Beta|Die Eigenschaft **serialNumber** wurde zur Entität [managedDevice](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_manageddevice) hinzugefügt.|
|Änderung|Beta|Die Eigenschaft **managementAgents** wurde von der Entität [managedDevice](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_manageddevice) entfernt.|
|Änderung|Beta|Die Eigenschaft **deployedAppCount** wurde zur Entität [targetedManagedAppConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_targetedmanagedappconfiguration) hinzugefügt.|
|Änderung|Beta|Die Eigenschaften **bitLockerFixedDrivePolicy** und **bitLockerRemovableDrivePolicy** wurden zur Entität [windows10EndpointProtectionConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10endpointprotectionconfiguration) hinzugefügt.|
|Änderung|Beta|Die Eigenschaften **enterpriseCloudPrintDiscoveryEndPoint**, **enterpriseCloudPrintOAuthAuthority**, **enterpriseCloudPrintOAuthClientIdentifier**, **enterpriseCloudPrintResourceIdentifier**, **enterpriseCloudPrintDiscoveryMaxLimit**, **enterpriseCloudPrintMopriaDiscoveryResourceIdentifier**, **edgeBlockAddressBarDropdown**, **edgeBlockCompatibilityList**, **edgeClearBrowsingDataOnExit**, **edgeAllowStartPagesModification**, **edgeDisableFirstRunPage**, **edgeBlockLiveTileDataCollection** und **edgeSyncFavoritesWithInternetExplorer** wurden zur Entität [windows10GeneralConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10generalconfiguration) hinzugefügt.|
|Änderung|Beta|Die Eigenschaft **availableVersion** wurde zur Entität [windowsManagementApp](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_devicefe_windowsmanagementapp) hinzugefügt.|
|Änderung|Beta|Die Eigenschaften **onboardingStatus**, **deployedVersion** und **lastModifiedTime** wurden von der Entität [windowsManagementApp](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_devicefe_windowsmanagementapp) entfernt.|
|Änderung|Beta|Die Eigenschaft **packageIdentityName** wurde zur Entität [windowsStoreForBusinessApp](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_windowsstoreforbusinessapp) hinzugefügt.|
|Änderung|Beta|Die Navigationseigenschaften **mobileAppIdentifierDeployments** und **deploymentSummary** wurden zur Entität [androidManagedAppProtection](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_androidmanagedappprotection) hinzugefügt.|
|Änderung|Beta|Die Navigationseigenschaft **mobileAppIdentifierDeployments** wurde zur Entität [defaultManagedAppProtection](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_defaultmanagedappprotection) hinzugefügt.|
|Änderung|Beta|Die Navigationseigenschaften **deviceConfigurationUserStateSummaries** und **iosUpdateStatuses** wurden zur Entität [deviceManagement](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_androidforwork_devicemanagement) hinzugefügt.|
|Änderung|Beta|Die Navigationseigenschaft **complianceSettingStateSummaries** wurde von der Entität [deviceManagement](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_androidforwork_devicemanagement) entfernt.|
|Änderung|Beta|Die Navigationseigenschaften **runSummary**, **deviceRunStates** und **userRunStates** wurden zur Entität [deviceManagementScript](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_devicefe_devicemanagementscript) hinzugefügt.|
|Änderung|Beta|Die Navigationseigenschaft **runStates** wurde von der Entität [deviceManagementScript](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_devicefe_devicemanagementscript) entfernt.|
|Änderung|Beta|Die Navigationseigenschaften **mobileAppIdentifierDeployments** und **deploymentSummary** wurden zur Entität [iosManagedAppProtection](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_iosmanagedappprotection) hinzugefügt.|
|Änderung|Beta|Die Navigationseigenschaften **mobileAppIdentifierDeployments** und **deploymentSummary** wurden von der Entität [managedAppPolicy](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_managedapppolicy) entfernt.|
|Änderung|Beta|Die Navigationseigenschaften **mobileAppIdentifierDeployments** und **deploymentSummary** wurden zur Entität [targetedManagedAppConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_targetedmanagedappconfiguration) hinzugefügt.|
|Änderung|Beta|Die Navigationseigenschaften **healthSummary** und **healthStates** wurden zur Entität [windowsManagementApp](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_devicefe_windowsmanagementapp) hinzugefügt.|
|Änderung|Beta|Die Eigenschaften **applicationId**, **appName**, **platformId**, **userFailures** und **deviceFailures** wurden dem komplexen Typ [appInstallationFailure](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_appinstallationfailure) hinzugefügt.|
|Änderung|Beta|Die Eigenschaften **encryptionMethod**, **startupAuthenticationRequired**, **startupAuthenticationBlockWithoutTpmChip**, **startupAuthenticationTpmUsage**, **startupAuthenticationTpmPinUsage**, **startupAuthenticationTpmKeyUsage**, **startupAuthenticationTpmPinAndKeyUsage**, **recoveryOptions** und **prebootRecoveryEnableMessageAndUrl** wurden dem komplexen Typ [bitLockerSystemDrivePolicy](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_bitlockersystemdrivepolicy) hinzugefügt.|
|Änderung|Beta|Die Eigenschaften **settingName**, **userId**, **userName**, **userEmail** und **currentValue** wurden vom komplexen Typ [deviceCompliancePolicySettingState](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancepolicysettingstate) entfernt.|
|Änderung|Beta|Die Eigenschaften **settingName**, **userId**, **userName**, **userEmail** und **currentValue** wurden vom komplexen Typ [deviceConfigurationSettingState](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationsettingstate) entfernt.|
|Änderung|Beta|Die Eigenschaften **windowsCommercialId** und **windowsCommercialIdLastModifiedTime** wurden dem komplexen Typ [deviceManagementSettings](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicemanagementsettings) hinzugefügt.|
|Änderung|Beta|Die Eigenschaft **address** wurde dem komplexen Typ [vpnServer](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_vpnserver) hinzugefügt.|


## <a name="may-2017"></a>Mai 2017

### <a name="application-api-changes"></a>Änderungen der Anwendungs-API

|**Änderungstyp**|**Version**|**Beschreibung**|
|:-------------|:-----------|:--------------|
|Änderung|Beta| Update der Anwendungs-API. Dies ist der erste Satz von Änderungen, einschließlich Umbenennung von Eigenschaften und Umstrukturierung der [application](https://graph.microsoft.io/en-us/docs/api-reference/beta/resources/application)-Entität.<br/>**Neue Entitäten:** [api](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/api]), [informationalUrl](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/informationalUrl), [installedClient](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/installedclient), [permissionScope](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/permissionscope), [preauthorizedApplication](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/preauthorizedapplication), [web](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/web).<br/>**Entfernte Eigenschaften:** addIns, appRoles, availableToOtherOrganizations, knownClientApplications, oauth2AllowUrlPathMatching, recordConsentConditions.<br/>**Umbenannte Eigenschaften:** appId in id, identifierUris in applicationAliases, availableToOtherTenants in orgRestrictions, mainLogo in logo, oauth2Permissions in publishedPermissionsScopes, publicClient in allowPublicClient, replyUrls in redirectUrls.<br/>**Neue Eigenschaften:** tags. |

### <a name="remove-deprecated-planner-api"></a>Entfernung der veralteten Planner-API
|**Änderungstyp**|**Version**|**Beschreibung**|
|:--------------|:-----------|:-------------|
|Löschung|Beta|Die folgenden Entitäten wurden entfernt:<br/>**task**<br/>**plan**<br/>**bucket**<br/>**taskDetails**<br/>**planDetails**<br/>**taskBoardTaskFormat**<br/>**planTaskBoard**|

### <a name="project-rome"></a>Projekt Rom

|**Änderungstyp**|**Version**|**Beschreibung**|
|:--------------|:-----------|:-------------|
|Ergänzungen|Beta|Zusätzliche Unterstützung für Projekt Rom, einschließlich [Abrufen einer Liste der Geräte](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/user_list_devices), [Senden eines Befehls an ein Gerät](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/send_device_command), und [Überprüfen des Status eines Befehls](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/get_device_command_status).|
|Ergänzungen|Beta|Zusätzliche Unterstützung für Benutzer[aktivitäten](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/projectrome_activity) und [historyItems](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/projectrome_historyitem), einschließlich [upsert-Vorgängen für eine Aktivität](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/projectrome_put_activity) und [upsert-Vorgängen für ein historyItem](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/projectrome_put_historyitem).|

### <a name="administrative-units-property-changes"></a>Eigenschaftsänderungen für administrative Einheiten

|**Änderungstyp**|**Version**|**Beschreibung**|
|:--------------|:-----------|:--------------|
| Änderung        | Beta       | Geänderter Eigenschaftentyp roleMemberInfo in [Identität](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/identity) für die [scopedRoleMembership](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/scopedrolemembership)-Entität |
| Änderung        | Beta       | Geänderte Navigationseigenschaft  scopedAdministratorOf in scopedRoleMemberOf für die [Benutzer](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/user)-Entität |
| Änderung        | Beta       | Geänderte Navigationseigenschaft  scopedAdministrators in scopedRoleMembers für die [administrativeUnit](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/administrativeunit)-Entität |
| Änderung        | Beta       | Geänderte Navigationseigenschaft  scopedAdministrators in scopedMembers für die [directoryRole](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/directoryrole)-Entität |

### <a name="add-users-and-groups-webhook-support-in-preview"></a>Hinzufügen von Benutzern und Gruppen-Webhook-Unterstützung in der Vorschau

|**Änderungstyp**|**Version**|**Beschreibung**|
|:--------------|:-----------|:--------------|
| Änderung        | Beta       | Zusätzliche Unterstützung zu [Webhooks](https://developer.microsoft.com/graph/docs/api-reference/beta/resources/webhooks) für Benutzer und Gruppen.

### <a name="add-delta-query-to-v10"></a>Delta-Abfrage zu v1.0 hinzufügen

|**Änderungstyp**|**Version**|**Beschreibung**|
|:--------------|:-----------|:--------------|
| Ergänzungen      | v1.0       | Delta-Funktion-Support zu V1.0 hinzufügen Zu folgenden Entitäten hinzufügen, um [Delta-Abfrage](https://developer.microsoft.com/en-us/graph/docs/concepts/delta_query_overview) auszuführen:<br/>contact<br/>contactFolder<br/>event<br/>group<br/>mailFolder<br/>message<br/>user<br/>Beispiele finden Sie unter Folgendem:<br/>[Inkrementelle Änderungen an Gruppen abrufen](https://developer.microsoft.com/en-us/graph/docs/concepts/delta_query_groups)<br/>[Inkrementelle Änderungen an Nachrichten in einem Ordner abrufen](https://developer.microsoft.com/en-us/graph/docs/concepts/delta_query_messages)<br/>[Inkrementelle Änderungen an Benutzern abrufen](https://developer.microsoft.com/en-us/graph/docs/concepts/delta_query_users)|
| Änderung        | Beta       | Hinzufügen von zusätzlicher optionaler Abfrage-Filterfunktion (anhand der Id) zu [Benutzer](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/user_delta) und [Gruppen](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/group_delta). |

### <a name="added-user-resource-support-for-deleted-items"></a>Unterstützung von hinzugefügte Benutzer Ressourcen für gelöschte Elemente

|**Änderungstyp**|**Version**|**Beschreibung**|
|:--------------|:-----------|:--------------|
| Ergänzungen      | Beta       | Es wurde Unterstützung zum [Wiederherstellen und endgültigen Löschen von Benutzern](https://graph.microsoft.io/en-us/docs/api-reference/beta/resources/directory) hinzugefügt. |

### <a name="added-onpremisesprovisioningerror"></a>Hinzugefügter OnPremisesProvisioningError

|**Änderungstyp**|**Version**|**Beschreibung**|
|:--------------|:-----------|:--------------|
| Ergänzungen      | Beta       | Neue Entität: [OnPremisesProvisioningError](https://graph.microsoft.io/en-us/docs/api-reference/beta/resources/onpremisesprovisioningerror) |
| Änderung        | Beta       | Hinzugefügte OnPremisesProvisioningError-Eigenschaft zu [Benutzer](https://graph.microsoft.io/en-us/docs/api-reference/beta/resources/user), [Gruppe](https://graph.microsoft.io/en-us/docs/api-reference/beta/resources/group), und [Organisationskontakt](https://graph.microsoft.io/en-us/docs/api-reference/beta/resources/orgcontact) |

### <a name="added-deleteddatetime-property"></a>Hinzugefügte DeletedDateTime-Eigenschaft

|**Änderungstyp**|**Version**|**Beschreibung**|
|:-------------|:-----------|:--------------|
|Änderung|Beta|Hinzugefügte DeletedDateTime-Eigenschaft zu [Benutzer](https://graph.microsoft.io/en-us/docs/api-reference/beta/resources/user)-Entität.
|Änderung|Beta|Hinzugefügte DeletedDateTime-Eigenschaft zu [Gruppen](https://graph.microsoft.io/en-us/docs/api-reference/beta/resources/group)-Entität.
|Änderung|Beta|Hinzugefügte DeletedDateTime-Eigenschaft zu [App](https://graph.microsoft.io/en-us/docs/api-reference/beta/resources/application)-Entität.

### <a name="added-domain-operations-to-v10"></a>Hinzufügte Domänenvorgängen zu v1.0

|**Änderungstyp**|**Version**|**Beschreibung**|
|:-------------|:-----------|:--------------|
|Ergänzungen|V1.0|Hinzugefügte Vorgänge in [Domänen](https://graph.microsoft.io/en-us/docs/api-reference/v1.0/resources/domain)<br/>Neue Entitäten:</br>[domain](https://graph.microsoft.io/en-us/docs/api-reference/v1.0/resources/domain)<br/>[domainDnsRecord](https://graph.microsoft.io/en-us/docs/api-reference/v1.0/resources/domaindnsrecord)<br/>[domainDnsCnameRecord](https://graph.microsoft.io/en-us/docs/api-reference/v1.0/resources/domainDnsCnameRecord)<br/>[domainDnsMxRecord](https://graph.microsoft.io/en-us/docs/api-reference/v1.0/resources/domainDnsMxRecord)<br/>[domainDnsSrvRecord](https://graph.microsoft.io/en-us/docs/api-reference/v1.0/resources/domainDnsSrvRecord)<br/>[domainDnsTxtRecord](https://graph.microsoft.io/en-us/docs/api-reference/v1.0/resources/domainDnsTxtRecord)<br/>[domainDnsUnavailableRecord](https://graph.microsoft.io/en-us/docs/api-reference/v1.0/resources/domainDnsUnavailableRecord)<br/>Neue Aktionen:</br>[überprüfen](https://graph.microsoft.io/en-us/docs/api-reference/v1.0/api/domain_verify) |

### <a name="added-contracts-to-v10"></a>Hinzugefügte Verträge zu v1.0

|**Änderungstyp**|**Version**|**Beschreibung**|
|:-------------|:-----------|:--------------|
|Ergänzungen|V1.0|Neue Entität:</br>[Vertrag](https://graph.microsoft.io/en-us/docs/api-reference/v1.0/resources/contract) |

### <a name="added-licensedetails-to-v10"></a>Hinzugefügte licenseDetails zu v1.0

|**Änderungstyp**|**Version**|**Beschreibung**|
|:-------------|:-----------|:--------------|
|Ergänzungen|v1.0|Neue Entität:</br>[licenseDetails](https://graph.microsoft.io/en-us/docs/api-reference/v1.0/resources/licensedetails) |
|Änderung  |v1.0|Neue [licensedetails](https://graph.microsoft.io/en-us/docs/api-reference/v1.0/api/user_list_licensedetails)-Nagivationseigenschaft für [Benutzer](https://graph.microsoft.io/en-us/docs/api-reference/v1.0/resources/user) |


### <a name="drive-api"></a>Laufwerk-API

|**Änderungstyp**|**Version**|**Beschreibung**|
|:--------------|:----------|:--------------|
| Ergänzungen | v1.0 | **baseItem**-Ressourcentyp hinzugefügt, bestehend aus grundlegenden Eigenschaften aus **driveItem**.
| Ergänzungen | v1.0 und Beta | **sourceItemId**-Eigenschaft zu **Miniaturansicht** hinzugefügt. <br/> **siteUrl**-Eigenschaft zu **sharepointIds** hinzugefügt. <br/> **sharedBy**- und **sharedDateTime**-Eigenschaften zu **shared** hinzugefügt. <br/> **shared**-Eigenschaft zu **remoteItem** hinzugefügt. <br/> **sharepointIds**-Eigenschaft zu **drive** und **itemReference** hinzugefügt. <br/> **lastAccessedDateTime** zu **fileSystemInfo** hinzugefügt. <br/> **driveItem**- und **site**- Navigationseigenschaften zu **sharedDriveItem** hinzugefügt. <br/> **parentReference**-Eigenschaft zu **baseItem** hinzugefügt.
| Änderung | v1.0 und Beta | **driveItem** und **sharedDriveItem** geändert, um **baseItem** zu übernehmen. <br/> Markierte **Identität** als ein offener Typ.
| Änderung | Beta | **configuratorUrl**- und **webHtml**-Eigenschaften zu **sharingLink** hinzugefügt. <br/> **folderView**-Ressourcentyp und die **Ansicht**-Eigenschaft zu **Ordner**-Ressourcentyp hinzugefügt. <br/> **listItem**-Navigationseigenschaft zu **driveItem** hinzugefügt. <br/> **list**-Navigationseigenschaft zu **drive** hinzugefügt.


### <a name="extensions-open-extensions"></a>Erweiterungen (Offene Erweiterungen)

|**Änderungstyp**|**Version**|**Beschreibung**|
|:-------------|:-----------|:--------------|
|Ergänzungen|v1.0| Unterstützung für die [openTypeExtension](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/opentypeextension) in den folgenden Ressourcen – [Gerät](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/device), [Gruppe](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/group),[Organisation](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/organization), [Benutzer](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/user). |
|Ergänzungen|v1.0 und Beta|Wenn der Benutzer mit einem persönlichen Microsoft-Konto angemeldet ist, besteht Unterstützung für offene Erweiterungen in den folgenden Ressourcen – Ereignis, Beitrag, Gruppe, Nachricht, Kontakt und Benutzer. (Dies ist zusätzlich zu diesen Ressourcen, plus Gerät, Gruppe, Organisation und Benutzer, geöffnete Erweiterungen werden unterstützt, wenn der Benutzer sich mit einem Firmen- oder Schul-Konto anmeldet.)|
|Ergänzungen|v1.0 und Beta|Unterstützung für die `$expand`, um [offene Erweiterungen](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/api/opentypeextension_get) in den folgenden Ressourcen zu erhalten: [Gerät](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/device), [Gruppe](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/group),[Organisation](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/organization), [Nachricht](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/post), [Benutzer](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/user).|
|Ergänzungen|Beta|Unterstützung für `$expand` um [offene Erweiterungen](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/api/opentypeextension_get) in [administrativeUnit](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/administrativeunit) zu erhalten.|


### <a name="extensions-schema-extensions"></a>Erweiterungen (Schemaerweiterungen) 

|**Änderungstyp**|**Version**|**Beschreibung**|
|:-------------|:-----------|:--------------|
|Ergänzungen|v1.0|Neue Ressource [schemaExtension](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/schemaextension) und CRUD-Methoden zum Verwalten von Erweiterungsdefinitionen für die folgenden Ressourcen: [Kontakt](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/contact), [Gerät](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/device), [Ereignis](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/event), [Gruppe](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/group), [Nachricht](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/message), [Organisation](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/organization), [Beitrag](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/post), [Benutzer](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/user). Beachten Sie, dass die Unterstützung für [administrativeUnit](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/administrativeunit) wie zuvor noch auf die Betaversion beschränkt ist.|
|Ergänzungen|v1.0|Die vorhandenen BEITRAG-, GET- und PATCH-Methoden der folgenden Ressourcen – [Kontakt](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/contact), [Gerät](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/device), [Ereignis](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/event), [Gruppe](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/group), [Nachricht](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/message), [Organisation](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/organization), [Beitrag](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/post), [Benutzer](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/user) - unterstützen jetzt Hinzufügen, Abrufen, und Aktualisieren oder Löschen von benutzerdefinierte Daten als Schemaerweiterungen werden in den entsprechenden Ressourceninstanzen gespeichert.|
|Ergänzungen|v1.0 und Beta| Sie können nun `$filter` verwenden, um nach Ressourceninstanzen mit Eigenschaften zu suchen, die bestimmten Erweiterungsimmobilienwerten, z. B. Erweiterungsnamen entsprechen. Sehen Sie [Beispiel](https://devx.microsoft-tst.com/en-us/graph/docs/concepts/extensibility_schema_groups#5-get-a-group-and-its-extension-data) für Details. |
|Änderung|v1.0 und Beta| [Schemaerweiterungsdefinition löschen](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/api/schemaextension_delete) wird keinen Einfluss mehr auf den Zugriff von benutzerdefinierten Daten haben, die aufgrund dieser Definition hinzugefügt wurden. |
|Änderung|v1.0 und Beta| Sie können nun einen Schema-Erweiterungskomplextyp auf Null setzen, um eine Schemaerweiterung aus einer Ressourceninstanz zu entfernen. |


### <a name="group"></a>Gruppe

|**Änderungstyp**|**Version**|**Beschreibung**|
|:--------------|:----------|:--------------|
| Ergänzungen | v1.0 und Beta | Die Navigationseigenschaften**drives** und **sites** wurden zu **group** hinzugefügt.

### <a name="insights-apis"></a>Insights-APIs

|**Änderungstyp**|**Version**|**Beschreibung**| 
|:-------------|:-----------|:--------------|
|Ergänzungen|Beta|[Freigegebene API](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/insights_shared) wurde hinzugefügt.<br />Neue Ressourcen:<br />[sharingDetail](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/insights_sharingdetail) <br />[insightIdentity](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/insights_insightidentity) <br />
|Ergänzungen|Beta|[Verwendete API](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/insights_used) wurde hinzugefügt.<br />Neue Ressourcen:<br />[usageDetails](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/insights_usagedetails) <br />
|Änderung|Beta|Neue **Type**-Eigenschaft in der:<br />[resourceVisualization](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/insights_resourcevisualization)-Ressource. <br />
|Löschung|Beta|Die folgenden Entitäten wurden entfernt:<br/>**workingWith**<br/>**trendingAround**<br/>|

### <a name="intune-apis"></a>Intune-APIs

|Änderungstyp|Version|Beschreibung|
|:---|:---|:---|
|Ergänzungen|Beta|Neue Entitäten hinzugefügt:<br/>[androidForWorkMobileAppConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_androidforworkmobileappconfiguration)<br/>[cartToClassAssociation](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_carttoclassassociation)<br/>[deviceCompliancePolicySettingStateSummary](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary)<br/>[eBookInstallSummary](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_books_ebookinstallsummary)<br/>[eBookVppGroupAssignment](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_books_ebookvppgroupassignment)<br/>[iosUpdateConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosupdateconfiguration)<br/>[remoteAssistancePartner](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_remoteassistance_remoteassistancepartner)<br/>[windows10EndpointProtectionConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10endpointprotectionconfiguration)<br/>[windowsDeviceMalwareState](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_endpointprotection_windowsdevicemalwarestate)<br/>[windowsInformationProtectionAppLearningSummary](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_wip_windowsinformationprotectionapplearningsummary)<br/>[windowsMalwareInformation](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_endpointprotection_windowsmalwareinformation)<br/>[windowsProtectionState](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_endpointprotection_windowsprotectionstate)<br/>|
|Ergänzungen|Beta|Neue komplexe Typen hinzugefügt:<br/>[androidPermissionAction](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_androidpermissionaction)<br/>[bitLockerSystemDrivePolicy](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_bitlockersystemdrivepolicy)<br/>[defenderDetectedMalwareActions](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_defenderdetectedmalwareactions)<br/>[settingSource](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_settingsource)<br/>|
|Ergänzungen|Beta|Die Aktion [assign](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_books_managedebook_assign) wurde zu [managedEBook](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_books_managedebook) hinzugefügt |
|Ergänzungen|Beta|Die Aktion [beginOnboarding](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_remoteassistance_remoteassistancepartner_beginonboarding) wurde zu [remoteAssistancePartner](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_remoteassistance_remoteassistancepartner) hinzugefügt. |
|Ergänzungen|Beta|Die Aktion [disconnect](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_remoteassistance_remoteassistancepartner_disconnect) wurde zu [remoteAssistancePartner](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_remoteassistance_remoteassistancepartner) hinzugefügt. |
|Löschung|Beta|Die folgenden Entitäten wurden entfernt:<br/>**outlookTask**<br/>**outlookTaskFolder**<br/>**outlookTaskGroup**<br/>**outlookUser**<br/>**windowsManagementAppHealthState**<br/>|
|Löschung|Beta|Die folgenden komplexen Typen wurden entfernt:<br/>**applePushNotificationCertificateSetting**<br/>**eventCreationOptions**<br/>|
|Änderung|Beta|Die Eigenschaften **workProfilePasswordBlockFingerprintUnlock**, **workProfilePasswordBlockTrustAgents**, **workProfilePasswordExpirationDays**, **workProfilePasswordMinimumLength**, **workProfilePasswordMinutesOfInactivityBeforeScreenTimeout**, **workProfilePasswordPreviousPasswordBlockCount**, **workProfilePasswordSignInFailureCountBeforeFactoryReset**, **workProfilePasswordRequiredType** und **workProfileRequirePassword** wurden der Entität [androidForWorkGeneralDeviceConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidforworkgeneraldeviceconfiguration) hinzugefügt.|
|Änderung|Beta|Die Eigenschaft **subjectAlternativeNameFormatString** wurde der Entität [androidForWorkPkcsCertificateProfile](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidforworkpkcscertificateprofile) hinzugefügt.|
|Änderung|Beta|Die Eigenschaften **subjectAlternativeNameFormatString** und **subjectAlternativeNameFormatString** wurden der Entität [androidForWorkScepCertificateProfile](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidforworkscepcertificateprofile) hinzugefügt.|
|Änderung|Beta|Die Eigenschaft **kioskModeManagedApps** wurde der Entität [androidGeneralDeviceConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidgeneraldeviceconfiguration) hinzugefügt.|
|Änderung|Beta|Die Eigenschaft **kioskModeManagedAppId** wurde von der Entität [androidGeneralDeviceConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidgeneraldeviceconfiguration) entfernt.|
|Änderung|Beta|Die Eigenschaft **subjectAlternativeNameFormatString** wurde der Entität [androidPkcsCertificateProfile](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidpkcscertificateprofile) hinzugefügt.|
|Änderung|Beta|Die Eigenschaften **subjectNameFormatString** und **subjectAlternativeNameFormatString** wurden der Entität [androidScepCertificateProfile](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidscepcertificateprofile) hinzugefügt.|
|Änderung|Beta|Die Eigenschaft **hexColor** wurde von der Entität [calendar](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/calendar) entfernt.|
|Änderung|Beta|Die Eigenschaften **setting** und **platformType** wurden der Entität [complianceSettingStateSummary](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_compliancesettingstatesummary) hinzugefügt.|
|Änderung|Beta|Die Eigenschaft **windowsManagementAppEnabled** wurde von der Entität [deviceAppManagement](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_deviceappmanagement) entfernt.|
|Änderung|Beta|Die Eigenschaften **userName**, **deviceModel** und **platform** wurden der Entität [deviceComplianceDeviceStatus](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancedevicestatus) hinzugefügt.|
|Änderung|Beta|Die Eigenschaften **userPrincipalName** und **deviceModel** wurden der Entität [deviceComplianceSettingState](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancesettingstate) hinzugefügt.|
|Änderung|Beta|Die Eigenschaften **platformType**, **setting**, **userId** und **userEmail** wurden der Entität [deviceComplianceSettingState](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancesettingstate) hinzugefügt.|
|Änderung|Beta|Die Eigenschaft **inGracePeriodCount** wurde der Entität [deviceCompliancePolicyDeviceStateSummary](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary) hinzugefügt.|
|Änderung|Beta|Die Eigenschaften **userName**, **deviceModel** und **platform** wurden der Entität [deviceConfigurationDeviceStatus](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationdevicestatus) hinzugefügt.|
|Änderung|Beta|Die Eigenschaft **creationOptions** wurde von der Entität [event](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/event) entfernt.|
|Änderung|Beta|Die Eigenschaft **isDelegated** wurde von derEntität [eventMessage](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/eventMessage) entfernt.|
|Änderung|Beta|Die Eigenschaften **unseenConversationsCount** und **unseenMessagesCount** wurden von der Entität [group](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/group) entfernt.|
|Änderung|Beta|Die Eigenschaften **settingXml** und **settings** wurden der Entität [iosMobileAppConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_iosmobileappconfiguration) hinzugefügt.|
|Änderung|Beta|Die Eigenschaft **subjectAlternativeNameFormatString** wurde der Entität [iosPkcsCertificateProfile](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_iospkcscertificateprofile) hinzugefügt.|
|Änderung|Beta|Die Eigenschaft **subjectAlternativeNameFormatString** wurde der Entität [iosScepCertificateProfile](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosscepcertificateprofile) hinzugefügt.|
|Änderung|Beta|Die Eigenschaft **systemIntegrityProtectionEnabled** wurde der Entität [macOSCompliancePolicy](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_macoscompliancepolicy) hinzugefügt.|
|Änderung|Beta|Die Eigenschaft **subjectAlternativeNameFormatString** wurde der Entität [macOSScepCertificateProfile](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_macosscepcertificateprofile) hinzugefügt.|
|Änderung|Beta|Die Eigenschaften **complianceGracePeriodExpirationDateTime**, **userPrincipalName** und **imei** wurden der Entität [managedDevice](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_manageddevice) hinzugefügt.|
|Änderung|Beta|Die Eigenschaften **settingXml** und **settings** wurden von der Entität [managedDeviceMobileAppConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_manageddevicemobileappconfiguration) entfernt.|
|Änderung|Beta|Die Eigenschaften **useSharedComputerActivation**, **updateChannel**, **officePlatformArchitecture** und **localesToInstall** wurden der Entität [officeSuiteApp](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_officesuiteapp) hinzugefügt.|
|Änderung|Beta|Die Eigenschaft **applePushNotificationCertificateSetting** wurde von der Entität [organization](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_onboarding_organization) entfernt.|
|Änderung|Beta|Die folgenden Eigenschaften für die Entität [post](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/post) wurden geändert:<br/>**sender** von „Optional“ in „Erforderlich“<br/>|
|Änderung|Beta|Die Eigenschaften **compliantUserCount**, **nonCompliantUserCount**, **remediatedUserCount**, **errorUserCount**, **unknownUserCount**, **conflictUserCount** und **notApplicableUserCount** wurden der Entität [softwareUpdateStatusSummary](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_softwareupdatestatussummary) hinzugefügt.|
|Änderung|Beta|Die Eigenschaften **bluetoothAllowedServices**, **bluetoothBlockPrePairing**, **cellularData**, **defenderDetectedMalwareActions**, **defenderPotentiallyUnwantedAppAction**, **lockScreenAllowTimeoutConfiguration**, **lockScreenBlockCortana**, **lockScreenBlockToastNotifications**, **lockScreenTimeoutInSeconds**, **passwordBlockSimple**, **privacyAutoAcceptPairingAndConsentPrompts**, **privacyBlockInputPersonalization**, **startMenuHideChangeAccountSettings**, **startMenuHideHibernate**, **startMenuHideLock**, **startMenuHideShutDown**, **startMenuHideSignOut**, **startMenuHideSleep**, **startMenuHideSwitchAccount**, **settingsBlockAppsPage**, **settingsBlockGamingPage**, **windowsSpotlightBlockConsumerSpecificFeatures**, **windowsSpotlightBlocked**, **windowsSpotlightBlockOnActionCenter**, **windowsSpotlightBlockTailoredExperiences**, **windowsSpotlightBlockThirdPartyNotifications**, **windowsSpotlightBlockWelcomeExperience**, **windowsSpotlightBlockWindowsTips**, **windowsSpotlightConfigureOnLockScreen** und **connectedDevicesServiceBlocked** wurden der Entität [windows10GeneralConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10generalconfiguration) hinzugefügt.|
|Änderung|Beta|Die Eigenschaften **automaticUpdateMode**, **automaticUpdateSchedule**, **automaticUpdateTime**, **prereleaseFeatures**, **experienceBlockWindowsSpotlight**, **experienceBlockWindowsTips** und **experienceBlockConsumerSpecificFeatures** wurden von der Entität [windows10GeneralConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10generalconfiguration) entfernt.|
|Änderung|Beta|Die Eigenschaft **subjectAlternativeNameFormatString** wurde der Entität [windows10PkcsCertificateProfile](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10pkcscertificateprofile) hinzugefügt.|
|Änderung|Beta|Die Eigenschaften **subjectNameFormatString** und **subjectAlternativeNameFormatString** wurden der Entität [windows81SCEPCertificateProfile](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows81scepcertificateprofile) hinzugefügt.|
|Änderung|Beta|Die Eigenschaften **indexingEncryptedStoresOrItemsBlocked** und **smbAutoEncryptedFileExtensions** wurden der Entität [windowsInformationProtection](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotection) hinzugefügt.|
|Änderung|Beta|Die folgenden Eigenschaften für die Entität [windowsInformationProtection](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotection) wurden geändert:<br/>**rightsManagementServicesTemplateId** von „Erforderlich“ in „Optional“<br/>|
|Änderung|Beta|Die folgenden Eigenschaften für die Entität [windowsMobileMSI](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_windowsmobilemsi) wurden geändert:<br/>**productCode** von „Erforderlich“ in „Optional“<br/>|
|Änderung|Beta|Die Eigenschaften **subjectNameFormatString** und **subjectAlternativeNameFormatString** wurden der Entität [windowsPhone81SCEPCertificateProfile](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsphone81scepcertificateprofile) hinzugefügt.|
|Änderung|Beta|Die Navigationseigenschaft **mobileAppConfigurations** wurde der Entität [deviceAppManagement](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_deviceappmanagement) hinzugefügt.|
|Änderung|Beta|Die Navigationseigenschaften **cartToClassAssociations**, **deviceCompliancePolicySettingStateSummaries**, **remoteAssistancePartners**, **windowsInformationProtectionAppLearningSummaries** und **windowsMalwareInformation** wurden der Entität [deviceManagement](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_androidforwork_devicemanagement) hinzugefügt.|
|Änderung|Beta|Die Navigationseigenschaft **eBook** wurde der Entität [eBookGroupAssignment](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_books_ebookgroupassignment) hinzugefügt.|
|Änderung|Beta|Die Navigationseigenschaft **windowsProtectionState** wurde der Entität [managedDevice](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_manageddevice) hinzugefügt.|
|Änderung|Beta|Die Navigationseigenschaft **installSummary** wurde der Entität [managedEBook](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_books_managedebook) hinzugefügt.|
|Änderung|Beta|Die Navigationseigenschaft **outlook** wurde von der Entität [user](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_user) entfernt.|
|Änderung|Beta|Die Navigationseigenschaft **healthStates** wurde von der Entität [windowsManagementApp](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsmanagementapp) entfernt.|
|Änderung|Beta|Die Eigenschaft **androidForWorkRestrictions** wurde dem komplexen Typ [defaultDeviceEnrollmentRestrictions](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_onboarding_defaultdeviceenrollmentrestrictions) hinzugefügt.|
|Änderung|Beta|Die Eigenschaften **userPrincipalName** und **sources** wurden der Entität [deviceCompliancePolicySettingState](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancepolicysettingstate) hinzugefügt.|
|Änderung|Beta|Die Eigenschaften **userPrincipalName** und **sources** wurden der Entität [deviceConfigurationSettingState](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationsettingstate) hinzugefügt.|
|Änderung|Beta|Die Eigenschaften **settingName**, **userId**, **userName**, **userEmail** und **currentValue** wurden dem komplexen Typ [deviceConfigurationSettingState](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationsettingstate) hinzugefügt.|
|Änderung|Beta|Die Eigenschaft **archiveFolder** wurde vom komplexen Typ [mailboxSettings](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/mailboxSettings) entfernt.|


### <a name="outlook-calendar"></a>Outlook-Kalender

|**Änderungstyp**|**Version**|**Beschreibung**|
|:-------------|:-----------|:--------------|
|Ergänzungen|v1.0 und Beta|Für **findMeetingTimes**, neuen Aufzählungswert **uneingeschränkt** hinzugefügt, den Sie als **activityDomain**-Eigenschaft, Teil des **TimeConstraint**- Parameters, spezifizieren. Dies lässt **findMeetingTimes** nach Zeiten suchen, die für die Art der Aktivität geeignet sind, für die Sie planen. Weitere Details im Abschnitt [request body](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/api/user_findmeetingtimes#request-body).|
|Ergänzungen|Beta|Unterstützung, die einen **event**-Text im Klartext erhält, als Alternative zum Standard-HTML-Format. Siehe [get](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/event_get)- und [list](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/user_list_events)-Ereignisse für Details.|

### <a name="outlook-mail"></a>Outlook-Mail

|**Änderungstyp**|**Version**|**Beschreibung**|
|:-------------|:-----------|:--------------|
|Änderung|Beta|Unterstützung, die einen **message**-Text im Klartext erhält, als Alternative zum Standard-HTML-Format. Siehe [get](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/message_get)- und [list](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/user_list_messages)-Ereignisse für Details.|


### <a name="outlook-tasks"></a>Outlook-Aufgaben

|**Änderungstyp**|**Version**|**Beschreibung**|
|:-------------|:-----------|:--------------|
|Ergänzungen|Beta|Neue **Outlook**-Navigationseigenschaft hinzugefügt zu [Benutzer](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/user), um auf Outlook-Aufgaben zuzugreifen.|
|Ergänzungen|Beta|Neue Entitäten – [outlookuser](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/outlookuser), [outlookTaskGroup](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/outlooktaskgroup), [outlookTaskFolder](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/outlooktaskfolder), und [outlookTask](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/outlooktask) - und deren Methoden unterstützen, organisieren und zugreifen auf Outlook-Aufgaben. | 
|Ergänzungen|Beta|Outlook-Aufgaben unterstützen Anhänge ([attachment](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/attachment), [fileAttachment](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/fileattachment), [itemAttachment](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/itemattachment) und [referenceAttachment](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/referenceattachment)-Ressourcen). |
|Ergänzungen|Beta|Outlook-Aufgaben unterstützen [extended properties](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/extended-properties-overview) ([singleValueLegacyExtendedProperty](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/singlevaluelegacyextendedproperty) und [multiValueLegacyExtendedProperty](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/multivaluelegacyextendedproperty)-Ressourcen). |

### <a name="planner-apis"></a>Planner-APIs

|**Änderungstyp**|**Version**|**Beschreibung**| 
|:-------------|:-----------|:--------------|
|Ergänzungen|v1.0|[Planner-APIs](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/planner_overview) hinzugefügt<br />Neue Ressourcen:<br />[plannerPlan](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/plannerPlan) <br />[plannerTask](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/plannerTask) <br />[plannerPlanDetails](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/plannerPlanDetails) <br />[plannerTaskDetails](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/plannerTaskDetails) <br />[plannerBucket](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/plannerBucket) <br />[plannerAssignedToTaskBoardTaskFormat](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/plannerassignedtotaskboardtaskformat) <br />[plannerBucketTaskBoardTaskFormat](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/plannerbuckettaskboardtaskformat) <br />[plannerProgressTaskBoardTaskFormat](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/plannerprogresstaskboardtaskformat) | 

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

|**Änderungstyp**|**Version**|**Beschreibung**|
|:-------------|:-----------|:--------------|
|Änderung|Beta| APIs für administrative Einheiten werden in der Vorschau (Beta) aktualisiert. Die erste Gruppe von Änderungen wird am 3. Mai 2017 angewendet. Im Rahmen der Änderungen werden die folgenden Eigenschaften umbenannt:<br />- Komplexer Typ **roleMemberInfo** in komplexen Typ **identity** für die scopedRoleMembership-Entität<br />- Navigationseigenschaft **scopedAdministratorOf** in **scopedRoleMemberOf** für die user-Entität<br />- Navigationseigenschaft **scopedAdministrators** in **scopedRoleMembers** für die administrativeUnit-Entität<br />- Navigationseigenschaft **scopedAdministrators** in **scopedMembers** für die directoryRole-Entität |

### <a name="application-and-serviceprincipal-api-changes"></a>Änderungen an der application- und servicePrincipal-API

|**Änderungstyp**|**Version**|**Beschreibung**|
|:-------------|:-----------|:--------------|
|Änderung|Beta| Die [application](https://graph.microsoft.io/en-us/docs/api-reference/beta/resources/application)- und [servicePrincipal](https://graph.microsoft.io/en-us/docs/api-reference/beta/resources/serviceprincipal)-APIs werden in der Vorschau (Beta) aktualisiert. Die erste Gruppe von Änderungen wird am 15. Mai 2017 angewendet. Die Änderungen umfassen Umbenennungen und Umstrukturierungen von Eigenschaften. Einige Eigenschaften (z. B. appRoles und addIns) sind erst verfügbar, wenn die Änderungen abgeschlossen sind. Die Änderungen werden in der Vorschau (Beta) vor der Veröffentlichung in v1.0 veröffentlicht. |

### <a name="added-preview-support-for-cloud-solution-provider-developers"></a>Es wurde Vorschauunterstützung für Entwickler von Cloudlösungsanbietern hinzugefügt.

|**Änderungstyp**|**Version**|**Beschreibung**|
|:-------------|:-----------|:--------------|
|Ergänzungen|Beta|Es wurden neue Vorschaufunktionen hinzugefügt, damit bereits genehmigte Anwendungen von Cloudlösungsanbieter Microsoft Graph aufrufen. Diese werden in einem neuen [Autorisierungsthema](https://graph.microsoft.io/en-us/docs/concepts/auth_cloudsolutionprovider) beschrieben. |

### <a name="added-onpremises-properties-to-user-entity"></a>Der Benutzerentität wurden onPremises-Eigenschaften hinzugefügt.

|**Änderungstyp**|**Version**|**Beschreibung**|
|:-------------|:-----------|:--------------|
|Ergänzungen|Beta|Der [user](https://graph.microsoft.io/en-us/docs/api-reference/beta/resources/user)-Entität wurden die neuen Eigenschaften onPremises, onPremisesDomainName, OnPremisesSamAccountName und onPremisesUserPrincipalName hinzugefügt. |

### <a name="new-planner-apis-and-an-update-to-the-group-visibility-property"></a>Neue Planner-APIs und ein Update der Eigenschaft für Gruppensichtbarkeit.

|**Änderungstyp**|**Version**|**Beschreibung**|
|:-------------|:-----------|:--------------|
|Änderung|Beta|**HiddenMembership** wurde als zusätzlicher Wert für die Sichtbarkeitseigenschaft, der [Group](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/group)-Entität hinzugefügt. |
|Ergänzungen|Beta|Es wurde eine neue [Planner-API](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/planner_overview) hinzugefügt.<br />Neue Ressourcen:<br />[plannerPlan](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/plannerPlan) <br />[plannerTask](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/plannerTask) <br />[plannerPlanDetails](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/plannerPlanDetails) <br />[plannerTaskDetails](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/plannerTaskDetails) <br />[plannerBucket](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/plannerBucket) <br />[plannerAssignedToTaskBoardTaskFormat](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/plannerassignedtotaskboardtaskformat) <br />[plannerBucketTaskBoardTaskFormat](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/plannerbuckettaskboardtaskformat) <br />[plannerProgressTaskBoardTaskFormat](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/plannerprogresstaskboardtaskformat) | 

### <a name="intune-apis"></a>Intune APIs
|**Änderungstyp**|**Version**|**Beschreibung**|
|:---|:---|:---|
|Ergänzungen|Beta|Hinzugefügte neue Entitäten:<br/>[androidForWorkCompliancePolicy](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidforworkcompliancepolicy)<br/>[deviceComplianceSettingState](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancesettingstate)<br/>[deviceInstallState](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_books_deviceinstallstate)<br/>[deviceManagementScript](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicemanagementscript)<br/>[deviceManagementScriptGroupAssignment](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicemanagementscriptgroupassignment)<br/>[deviceManagementScriptState](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicemanagementscriptstate)<br/>[eBookGroupAssignment](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_books_ebookgroupassignment)<br/>[iosVppEBook](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_books_iosvppebook)<br/>[managedEBook](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_books_managedebook)<br/>[userInstallStateSummary](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_books_userinstallstatesummary)<br/>[windowsManagementApp](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsmanagementapp)<br/>[windowsManagementAppHealthState](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsmanagementapphealthstate)<br/>|
|Ergänzungen|Beta|Die folgenden komplexen Typen wurden hinzugefügt:<br/>[dailySchedule](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_dailyschedule)<br/>[hourlySchedule](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_hourlyschedule)<br/>[iosBookmark](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosbookmark)<br/>[iosWebContentFilterAutoFilter](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioswebcontentfilterautofilter)<br/>[iosWebContentFilterBase](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioswebcontentfilterbase)<br/>[iosWebContentFilterSpecificWebsitesAccess](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioswebcontentfilterspecificwebsitesaccess)<br/>[runSchedule](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_runschedule)<br/>[sharedAppleDeviceUser](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_sharedappledeviceuser)<br/>[windows10NetworkProxyServer](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10networkproxyserver)<br/>|
|Ergänzungen|Beta|Die [requestRemoteAssistance](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_deviceconfig_manageddevice_requestremoteassistance)-Aktion wurde zu [managedDevice](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_manageddevice) hinzugefügt. |
|Ergänzungen|Beta|Die [cleanWindowsDevice](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_deviceconfig_manageddevice_cleanwindowsdevice)-Aktion wurde zu [managedDevice](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_manageddevice) hinzugefügt. |
|Ergänzungen|Beta|Die [logoutSharedAppleDeviceActiveUser](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_deviceconfig_manageddevice_logoutsharedappledeviceactiveuser)-Aktion wurde zu [managedDevice](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_manageddevice) hinzugefügt. |
|Ergänzungen|Beta|Die [deleteUserFromSharedAppleDevice](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_deviceconfig_manageddevice_deleteuserfromsharedappledevice)-Aktion wurde zu [managedDevice](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_manageddevice) hinzugefügt. |
|Ergänzungen|Beta|Die [assign](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_deviceconfig_devicemanagementscript_assign)-Aktion wurde zu [deviceManagementScript](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicemanagementscript) hinzugefügt. |
|Ergänzungen|Beta|Die [syncLicenses](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_onboarding_applevolumepurchaseprogramtoken_synclicenses)-Aktion wurde zu [appleVolumePurchaseProgramToken](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_applevolumepurchaseprogramtoken) hinzugefügt. |
|Ergänzungen|Beta|Die **getTopMobileAppCount**-Funktion wurde der [mobileApp](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_mobileapp)-Sammlung hinzugefügt. |
|Ergänzungen|Beta|Die [downloadApplePushNotificationCertificateSigningRequest](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_deviceconfig_applepushnotificationcertificate_downloadapplepushnotificationcertificatesigningrequest)-Funktion wurde zu [applePushNotificationCertificate](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_applepushnotificationcertificate) hinzugefügt. |
|Ergänzungen|Beta|Die [getDeviceComplianceSettingStates](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_deviceconfig_devicemanagement_getdevicecompliancesettingstates)-Funktion wurde zu [deviceManagement](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_androidforwork_devicemanagement) hinzugefügt. |
|Ergänzungen|Beta|Die [deviceConfigurationUserActivity](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_deviceconfig_reportroot_deviceconfigurationuseractivity)-Funktion wurde zu [reportRoot](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_reportroot) hinzugefügt. |
|Ergänzungen|Beta|Die [deviceConfigurationDeviceActivity](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_deviceconfig_reportroot_deviceconfigurationdeviceactivity)-Funktion wurde zu [reportRoot](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_reportroot) hinzugefügt. |
|Löschung|Beta|Die folgenden komplexen Typen wurden entfernt:<br/>**enterpriseCloudResource**<br/>**windowsInformationProtectionAppRule**<br/>**windowsInformationProtectionAppRuleAppLockerPolicyFileTemplate**<br/>**windowsInformationProtectionAppRuleDesktopTemplate**<br/>**windowsInformationProtectionAppRuleStoreAppTemplate**<br/>**windowsInformationProtectionAppRuleTemplate**<br/>**windowsInformationProtectionCorporateNetworkLocation**<br/>**windowsInformationProtectionProtectedLocation**<br/>**windowsInformationProtectionProtectedLocationEnterpriseCloudResources**<br/>**windowsInformationProtectionProtectedLocationEnterpriseInternalProxyServers**<br/>**windowsInformationProtectionProtectedLocationEnterpriseIPv4Ranges**<br/>**windowsInformationProtectionProtectedLocationEnterpriseIPv6Ranges**<br/>**windowsInformationProtectionProtectedLocationEnterpriseNetworkDomainNames**<br/>**windowsInformationProtectionProtectedLocationEnterpriseProxyServers**<br/>**windowsInformationProtectionProtectedLocationNeutralResources**<br/>|
|Änderung|Beta|Die **deviceSharingAllowed**-Eigenschaft wurde der [androidGeneralDeviceConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidgeneraldeviceconfiguration)-Entität hinzugefügt.|
|Änderung|Beta|Die **deviceSharingBlocked**-Eigenschaft wurde aus der Entität [androidGeneralDeviceConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidgeneraldeviceconfiguration)-Entität entfernt.|
|Änderung|Beta|Die **minimumRequiredSdkVersion**-Eigenschaft wurde der [defaultManagedAppProtection](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_defaultmanagedappprotection)-Entität hinzugefügt.|
|Änderung|Beta|Die **windowsManagementAppEnabled**-Eigenschaft wurde der [deviceAppManagement](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_deviceappmanagement)-Entität hinzugefügt.|
|Änderung|Beta|Die **notificationTemplateId**-Eigenschaft wurde der [deviceComplianceActionItem](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecomplianceactionitem)-Entität hinzugefügt.|
|Änderung|Beta|Die **excludeGroup**-Eigenschaft wurde der [deviceConfigurationGroupAssignment](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationgroupassignment)-Entität hinzugefügt.|
|Änderung|Beta|Die folgenden Eigenschaften in der [iosCustomConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioscustomconfiguration)-Entität wurden geändert:<br/>**payloadFileName** von „Erforderlich“ in „Optional“<br/>|
|Änderung|Beta|Die **contentFilterSettings**-Eigenschaft wurde der [iosDeviceFeaturesConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosdevicefeaturesconfiguration)-Entität hinzugefügt.|
|Änderung|Beta|Die Eigenschaften **cellularBlockPersonalHotspot** und **passcodeBlockFingerprintModification** wurden der [iosGeneralDeviceConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosgeneraldeviceconfiguration)-Entität hinzugefügt.|
|Änderung|Beta|Die **minimumRequiredSdkVersion**-Eigenschaft wurde der [iosManagedAppProtection](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_iosmanagedappprotection)-Entität hinzugefügt.|
|Änderung|Beta|Die folgenden Eigenschaften in der [macOSCustomConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_macoscustomconfiguration)-Entität wurden geändert:<br/>**payloadFileName** von „Erforderlich“ in „Optional“<br/>|
|Änderung|Beta|Die Eigenschaften **disableAppPinIfDevicePinIsSet**, **minimumRequiredOsVersion**, **minimumWarningOsVersion**, **minimumRequiredAppVersion** und **minimumWarningAppVersion** wurden der [managedAppProtection](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_managedappprotection)-Entität hinzugefügt.|
|Änderung|Beta|Die Eigenschaften **remoteAssistanceSessionUrl**, **isEncrypted**, **model** und **manufacturer** wurden der [managedDevice](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_manageddevice)-Entität hinzugefügt.|
|Änderung|Beta|Die folgenden Eigenschaften in der [getMobileAppCount](https://developer.microsoft.com/en-us/graph/docs/docs/api-reference/beta/api/intune_apps_mobileapp_getmobileappcount)-Entität wurden geändert:<br/>**bindingParameter** von **mobileApp** in eine **Sammlung** von *mobileApp*<br/>**status** von einer GUID in eine Zeichenfolge<br/>|
|Änderung|Beta|Die **vpnConfigurationId**-Eigenschaft wurde der Entität [mobileAppGroupAssignment](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_mobileappgroupassignment) hinzugefügt.|
|Änderung|Beta|Die **fromEmailAddress**-Eigenschaft wurde aus der [mobileAppGroupAssignment](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_notificationmessagetemplate)-Entität entfernt.|
|Änderung|Beta|Die **excludedApps**-Eigenschaft wurde der [officeSuiteApp](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_officesuiteapp)-Entität hinzugefügt.|
|Änderung|Beta|Die **excludedOfficeApps**-Eigenschaft wurde aus der [officeSuiteApp](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_officesuiteapp)-Entität entfernt.|
|Änderung|Beta|Die **enabled**-Eigenschaft wurde der [sharedPCConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_sharedpcconfiguration)-Entität hinzugefügt.|
|Änderung|Beta|Die Eigenschaften **networkProxyApplySettingsDeviceWide**, **networkProxyDisableAutoDetect**, **networkProxyAutomaticConfigurationUrl**, **networkProxyServer**, **bluetoothDeviceName**, **wiFiScanInterval**, **wirelessDisplayBlockProjectionToThisDevice**, **wirelessDisplayBlockUserInputFromReceiver**, **wirelessDisplayRequirePinForPairing**, **experienceBlockDeviceDiscovery**, **experienceBlockErrorDialogWhenNoSIM**, **experienceBlockTaskSwitcher**, **startMenuPinnedFolderDocuments**, **startMenuPinnedFolderDownloads**, **startMenuPinnedFolderFileExplorer**, **startMenuPinnedFolderHomeGroup**, **startMenuPinnedFolderMusic**, **startMenuPinnedFolderNetwork**, **startMenuPinnedFolderPersonalFolder**, **startMenuPinnedFolderPictures**, **startMenuPinnedFolderSettings**, **startMenuPinnedFolderVideos**, **startMenuAppListVisibility**, **startMenuHideFrequentlyUsedApps**, **startMenuHideRecentJumpLists**, **startMenuHideRecentlyAddedApps**, **startMenuHideRestartOptions**, **startMenuHideUserTile**, **startMenuHidePowerButton**, **startMenuLayoutEdgeAssetsXml**, **personalizationDesktopImageUrl** und **personalizationLockScreenImageUrl** wurden der [windows10GeneralConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10generalconfiguration)-Entität hinzugefügt.|
|Änderung|Beta|Der Typ der folgenden Eigenschaften in der [windowsMobileMSI](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_windowsmobilemsi)-Entität wurde geändert:<br/>**productCode** von „GUID“ in „Zeichenfolge“<br/>|
|Änderung|Beta|Die folgenden Eigenschaften in der [windowsPhone81AppX](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_windowsphone81appx)-Entität wurden geändert:<br/>**phoneProductIdentifier** von „Erforderlich“ in „Optional“<br/>**phonePublisherId** von „Erforderlich“ in „Optional“<br/>|
|Änderung|Beta|Die folgenden Eigenschaften in der [windowsPhone81AppXBundle](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_windowsphone81appxbundle)-Entität wurden geändert:<br/>**appXPackageInformationList** von „Erforderlich“ in „Optional“<br/>|
|Änderung|Beta|Die Eigenschaften **productKey** und **licenseType** wurden der [windowsStoreForBusinessApp](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_windowsstoreforbusinessapp)-Entität hinzugefügt.|
|Änderung|Beta|Die **previewBuildSetting**-Eigenschaft wurde der [windowsUpdateForBusinessConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsupdateforbusinessconfiguration)-Entität hinzugefügt.|
|Änderung|Beta|Die Navigationseigenschaften **windowsManagementApp** und **managedEBooks** wurden der [deviceAppManagement](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_deviceappmanagement)-Entität hinzugefügt.|
|Änderung|Beta|Die Navigationseigenschaften **deviceManagementScripts**, **managedDeviceOverview** und **cloudPkiSubscriptions** wurden der [deviceManagement](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_androidforwork_devicemanagement)-Entität hinzugefügt.|
|Änderung|Beta|Die Eigenschaften **osMinimumVersion** und **osMaximumVersion** wurden dem komplexen Typ [deviceEnrollmentPlatformRestrictions](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_onboarding_deviceenrollmentplatformrestrictions) hinzugefügt.|
|Änderung|Beta|Die Eigenschaften **isSharedDevice** und **sharedDeviceCachedUsers** wurden dem komplexen Typ [hardwareInformation](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_hardwareinformation) hinzugefügt.|
|Änderung|Beta|Die folgenden Eigenschaften im komplexen Typ [omaSettingBase64](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_omasettingbase64) wurden geändert:<br/>**fileName** von „Erforderlich“ in „Optional“<br/>|
|Änderung|Beta|Die folgenden Eigenschaften im komplexen Typ [omaSettingStringXml](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_omasettingstringxml) wurden geändert:<br/>**fileName** von „Erforderlich“ in „Optional“<br/>|

## <a name="march-2017"></a>März 2017

### <a name="intune-apis"></a>Intune APIs

|Änderungstyp|Version|Beschreibung|
|:---|:---|:---|
|Ergänzungen|Beta|Hinzugefügte neue Entitäten:<br/>[androidForWorkApp](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_androidforworkapp)<br/>[androidForWorkAppConfigurationSchema](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_androidforwork_androidforworkappconfigurationschema)<br/>[androidForWorkSettings](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_androidforwork_androidforworksettings)<br/>[androidForWorkVpnConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidforworkvpnconfiguration)<br/>[applePushNotificationCertificate](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_applepushnotificationcertificate)<br/>[complianceSettingStateSummary](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_compliancesettingstatesummary)<br/>[deviceCompliancePolicyDeviceStateSummary](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary)<br/>[deviceCompliancePolicyState](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancepolicystate)<br/>[deviceConfigurationDeviceStateSummary](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationdevicestatesummary)<br/>[deviceConfigurationState](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationstate)<br/>[enterpriseCodeSigningCertificate](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_enterprisecodesigningcertificate)<br/>[iosEduDeviceConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosedudeviceconfiguration)<br/>[managedDeviceCertificateState](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_manageddevicecertificatestate)<br/>[managedDeviceMobileAppConfigurationDeviceSummary](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_manageddevicemobileappconfigurationdevicesummary)<br/>[managedDeviceMobileAppConfigurationUserSummary](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_manageddevicemobileappconfigurationusersummary)<br/>[mdmWindowsInformationProtectionPolicy](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_mdmwindowsinformationprotectionpolicy)<br/>[mobileAppInstallSummary](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_mobileappinstallsummary)<br/>[mobileAppProvisioningConfigGroupAssignment](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_mobileappprovisioningconfiggroupassignment)<br/>[mobileThreatDefenseConnector](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_onboarding_mobilethreatdefenseconnector)<br/>[officeSuiteApp](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_officesuiteapp)<br/>[settingStateDeviceSummary](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_settingstatedevicesummary)<br/>[softwareUpdateStatusSummary](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_softwareupdatestatussummary)<br/>[symantecCodeSigningCertificate](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_symanteccodesigningcertificate)<br/>[windowsDefenderAdvancedThreatProtectionConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsdefenderadvancedthreatprotectionconfiguration)<br/>[windowsInformationProtection](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotection)<br/>[windowsInformationProtectionAppLockerFile](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotectionapplockerfile)<br/>[windowsInformationProtectionPolicy](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotectionpolicy)<br/>[windowsMobileMSI](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_windowsmobilemsi)<br/>|
|Ergänzungen|Beta|Die folgenden komplexen Typen wurden hinzugefügt:<br/>[androidForWorkAppConfigurationExample](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_androidforwork_androidforworkappconfigurationexample)<br/>[androidForWorkAppConfigurationExampleJson](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_androidforwork_androidforworkappconfigurationexamplejson)<br/>[androidForWorkAppConfigurationSchemaItem](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_androidforwork_androidforworkappconfigurationschemaitem)<br/>[deviceCompliancePolicySettingState](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancepolicysettingstate)<br/>[deviceConfigurationSettingState](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationsettingstate)<br/>[deviceExchangeAccessStateSummary](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceexchangeaccessstatesummary)<br/>[edgeSearchEngine](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_edgesearchengine)<br/>[edgeSearchEngineBase](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_edgesearchenginebase)<br/>[edgeSearchEngineCustom](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_edgesearchenginecustom)<br/>[excludedApps](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_excludedapps)<br/>[iosEduCertificateSettings](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioseducertificatesettings)<br/>[ipRange](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_iprange)<br/>[windowsInformationProtectionApp](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotectionapp)<br/>[windowsInformationProtectionCloudResource](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotectioncloudresource)<br/>[windowsInformationProtectionCloudResourceCollection](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotectioncloudresourcecollection)<br/>[windowsInformationProtectionDesktopApp](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotectiondesktopapp)<br/>[windowsInformationProtectionIPRangeCollection](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotectioniprangecollection)<br/>[windowsInformationProtectionResourceCollection](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotectionresourcecollection)<br/>[windowsInformationProtectionStoreApp](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotectionstoreapp)<br/>|
|Ergänzungen|Beta|Die [requestSignupUrl](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_androidforwork_androidforworksettings_requestsignupurl)-Aktion wurde zu [androidForWorkSettings](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_androidforwork_androidforworksettings) hinzugefügt. |
|Ergänzungen|Beta|Die [completeSignup](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_androidforwork_androidforworksettings_completesignup)-Aktion wurde zu [androidForWorkSettings](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_androidforwork_androidforworksettings) hinzugefügt. |
|Ergänzungen|Beta|Die [syncApps](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_androidforwork_androidforworksettings_syncapps)-Aktion wurde zu [androidForWorkSettings](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_androidforwork_androidforworksettings) hinzugefügt. |
|Ergänzungen|Beta|Die [unbind](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_androidforwork_androidforworksettings_unbind)-Aktion wurde zu [androidForWorkSettings](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_androidforwork_androidforworksettings) hinzugefügt. |
|Ergänzungen|Beta|Die [assign](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_apps_ioslobappprovisioningconfiguration_assign)-Aktion wurde zu [iosLobAppProvisioningConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_ioslobappprovisioningconfiguration) hinzugefügt. |
|Ergänzungen|Beta|Die [recoverPasscode](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_deviceconfig_manageddevice_recoverpasscode)-Aktion wurde zu [managedDevice](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_manageddevice) hinzugefügt. |
|Ergänzungen|Beta|Die [removeApplePushNotificationCertificate](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_onboarding_organization_removeapplepushnotificationcertificate)-Aktion wurde zu [organization](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_onboarding_organization) hinzugefügt. |
|Ergänzungen|Beta|Die [updateMobileAppIdentifierDeployments](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_mam_iosmanagedappprotection_updatemobileappidentifierdeployments)-Aktion wurde zu [osManagedAppProtection](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_iosmanagedappprotection) hinzugefügt. |
|Ergänzungen|Beta|Die [updateMobileAppIdentifierDeployments](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_mam_androidmanagedappprotection_updatemobileappidentifierdeployments)-Aktion wurde zu [androidManagedAppProtection](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_androidmanagedappprotection) hinzugefügt. |
|Ergänzungen|Beta|Die [updateMobileAppIdentifierDeployments](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_mam_targetedmanagedappconfiguration_updatemobileappidentifierdeployments)-Aktion wurde zu [targetedManagedAppConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_targetedmanagedappconfiguration) hinzugefügt. |
|Ergänzungen|Beta|Die [updateTargetedSecurityGroups](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_mam_iosmanagedappprotection_updatetargetedsecuritygroups)-Aktion wurde zu [iosManagedAppProtection](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_iosmanagedappprotection) hinzugefügt. |
|Ergänzungen|Beta|Die [updateTargetedSecurityGroups](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_mam_androidmanagedappprotection_updatetargetedsecuritygroups)-Aktion wurde zu [androidManagedAppProtection](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_androidmanagedappprotection) hinzugefügt. |
|Ergänzungen|Beta|Die [updateTargetedSecurityGroups](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_mam_windowsinformationprotection_updatetargetedsecuritygroups)-Aktion wurde zu [windowsInformationProtection](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotection) hinzugefügt. |
|Ergänzungen|Beta|Die [updateTargetedSecurityGroups](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_mam_windowsinformationprotection_updatetargetedsecuritygroups)-Aktion wurde zu [windowsInformationProtectionPolicy](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotectionpolicy) hinzugefügt. |
|Ergänzungen|Beta|Die [updateTargetedSecurityGroups](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_mam_mdmwindowsinformationprotectionpolicy_updatetargetedsecuritygroups)-Aktion wurde zu [mdmWindowsInformationProtectionPolicy](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_mdmwindowsinformationprotectionpolicy) hinzugefügt. |
|Ergänzungen|Beta|Die [wipeManagedAppRegistrationByDeviceTag](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_mam_user_wipemanagedappregistrationbydevicetag)-Aktion wurde zu [user](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_user) hinzugefügt. |
|Ergänzungen|Beta|Die [getTopMobileAppCount](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_apps_mobileapp_gettopmobileapps)-Funktion wurde zu [mobileApp](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_mobileapp) hinzugefügt. |
|Ergänzungen|Beta|Die [verifyWindowsEnrollmentAutoDiscovery](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_corpenrollment_devicemanagement_verifywindowsenrollmentautodiscovery)-Funktion wurde zu [deviceManagement](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_androidforwork_devicemanagement) hinzugefügt. |
|Löschung|Beta|Die folgenden Entitäten wurden entfernt:<br/>**appProvisioningConfigGroupAssignment**<br/>**defaultManagedAppConfiguration**<br/>**enterpriseCertificate**<br/>**managedDeviceMobileAppProvisioningConfigurationDeviceStatus**<br/>**symantecCertificate**<br/>**windows10WindowsInformationProtectionConfiguration**<br/>|
|Löschung|Beta|Die folgenden komplexen Typen wurden entfernt:<br/>**mobileAppInstallSummary**<br/>**windowsArchitecture**<br/>**windowsDeviceType**<br/>|
|Änderung|Beta|Die **webBrowserBlockPopups**-Eigenschaft wurde der  [androidGeneralDeviceConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidgeneraldeviceconfiguration)-Entität hinzugefügt.|
|Änderung|Beta|Die Eigenschaft **webBrowserBlockPopups**-Eigenschaft wurde aus der [androidGeneralDeviceConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidgeneraldeviceconfiguration)-Entität entfernt.|
|Änderung|Beta|Die **appIdentifier**-Eigenschaft wurde der [androidStoreApp](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_androidstoreapp)-Entität hinzugefügt.|
|Änderung|Beta|Die Eigenschaften **applicationCount**, **failedApplicationCount** und **appInstallFailures** wurden aus der [appReportingOverviewStatus](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/appReportingOverviewStatus)-Entität entfernt.|
|Änderung|Beta|Die Eigenschaften **sharedIPadMaximumUserCount** und **enableSharedIPad** wurden der [depEnrollmentProfile](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_corpenrollment_depenrollmentprofile)-Entität hinzugefügt.|
|Änderung|Beta|Die Eigenschaften **shareTokenWithSchoolDataSyncService** und **lastSyncErrorCode** wurden der [depOnboardingSetting](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_onboarding_deponboardingsetting)-Entität hinzugefügt.|
|Änderung|Beta|Die Eigenschaften **pendingCount**, **successCount**, **errorCount**, **failedCount**, **lastUpdateDateTime** und **configurationVersion** wurden der [deviceComplianceDeviceOverview](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancedeviceoverview)-Entität hinzugefügt.|
|Änderung|Beta|Die Eigenschaften **numberOfPendingDevices**, **numberOfSucceededDevices**, **numberOfErrorDevices**, **numberOfFailedDevices**, **lastUpdateTime** und **policyRevision** wurden aus der [deviceComplianceDeviceOverview](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancedeviceoverview)-Entität entfernt.|
|Änderung|Beta|Die Eigenschaften **pendingCount**, **successCount**, **errorCount**, **failedCount**, **lastUpdateDateTime** und **configurationVersion** wurden der [deviceComplianceUserOverview](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecomplianceuseroverview)-Entität hinzugefügt.|
|Änderung|Beta|Die Eigenschaften **numberOfPendingDevices**, **numberOfSucceededDevices**, **numberOfErrorDevices**, **numberOfFailedDevices**, **lastUpdateTime** und **policyRevision** wurden aus der [deviceComplianceUserOverview](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecomplianceuseroverview)-Entität entfernt.|
|Änderung|Beta|Die Eigenschaften **pendingCount**, **successCount**, **errorCount**, **failedCount**, **lastUpdateDateTime** und **configurationVersion** wurden der [deviceConfigurationDeviceOverview](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationdeviceoverview)-Entität hinzugefügt.|
|Änderung|Beta|Die Eigenschaften **numberOfPendingDevices**, **numberOfSucceededDevices**, **numberOfErrorDevices**, **numberOfFailedDevices**, **lastUpdateTime** und **policyRevision** wurden aus der [deviceConfigurationDeviceOverview](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationdeviceoverview)-Entität entfernt.|
|Änderung|Beta|Die Eigenschaften **pendingCount**, **successCount**, **errorCount**, **failedCount**, **lastUpdateDateTime** und **configurationVersion** wurden der [deviceConfigurationUserOverview](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationuseroverview)-Entität hinzugefügt.|
|Änderung|Beta|Die Eigenschaften **numberOfPendingDevices**, **numberOfSucceededDevices**, **numberOfErrorDevices**, **numberOfFailedDevices**, **lastUpdateTime** und **policyRevision** wurden aus der [deviceConfigurationUserOverview](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationuseroverview)-Entität entfernt.|
|Änderung|Beta|Die **subscriptionState**-Eigenschaft wurde der [deviceManagement](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_androidforwork_devicemanagement)-Entität hinzugefügt.|
|Änderung|Beta|Die **managedEmailProfileRequired**-Eigenschaft wurde der [iosCompliancePolicy](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioscompliancepolicy)-Entität hinzugefügt.|
|Änderung|Beta|Die **appsSingleAppModeList**-Eigenschaft wurde der [iosGeneralDeviceConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosgeneraldeviceconfiguration)-Entität hinzugefügt.|
|Änderung|Beta|Die **appsSingleAppModeBundleIds**-Eigenschaft wurde aus der [iosGeneralDeviceConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosgeneraldeviceconfiguration)-Entität entfernt.|
|Änderung|Beta|Die **expirationDateTime**-Eigenschaft wurde der [iosLobAppProvisioningConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_ioslobappprovisioningconfiguration)-Entität hinzugefügt.|
|Änderung|Beta|Die **expiration**-Eigenschaft wurde aus der [iosLobAppProvisioningConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_ioslobappprovisioningconfiguration)-Entität entfernt.|
|Änderung|Beta|Die Eigenschaften **passwordMinimumCharacterSetCount**, **osMinimumVersion**, **osMaximumVersion**, **deviceThreatProtectionEnabled**, **deviceThreatProtectionRequiredSecurityLevel** und **storageRequireEncryption** wurden aus der [macOSCompliancePolicy](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_macoscompliancepolicy)-Entität entfernt.|
|Änderung|Beta|Die **manifest**-Eigenschaft wurde aus der [managedAndroidLobApp](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_managedandroidlobapp)-Entität entfernt.|
|Änderung|Beta|Die Eigenschaften **isSupervised**, **exchangeLastSuccessfulSyncDateTime**, **exchangeAccessState** und **exchangeAccessStateReason** wurden der [managedDevice](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_manageddevice)-Entität hinzugefügt.|
|Änderung|Beta|Die **deviceExchangeAccessStateSummary**-Eigenschaft wurde der Entität [managedDeviceOverview](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_manageddeviceoverview)-Entität hinzugefügt.|
|Änderung|Beta|Die **manifest**-Eigenschaft  wurde aus der [managedIOSLobApp](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_managedioslobapp)-Entität entfernt.|
|Änderung|Beta|Die **installSummary**-Eigenschaft  wurde aus der [mobileApp](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_mobileapp)-Entität entfernt.|
|Änderung|Beta|Die **uploadState**-Eigenschaft  wurde der [mobileAppContentFile](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_mobileappcontentfile)-Entität hinzugefügt.|
|Änderung|Beta|Die folgenden Eigenschaften  in der Entität [ mobileAppContentFile](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_mobileappcontentfile)-Entität wurden geändert:<br/>**azureStorageUriExpirationDateTime** von „Erforderlich“ zu „Optional“<br/>|
|Änderung|Beta|Die Eigenschaften **initiatedByUserPrincipalName**, **deviceOwnerUserPrincipalName**, **deviceIMEI** und **actionState** wurden der [remoteActionAudit](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_remoteactionaudit)-Entität hinzugefügt.|
|Änderung|Beta|Die Eigenschaften **oneDriveDisableFileSync**, **safeSearchFilter**, **edgeSearchEngine**, **settingsBlockSettingsApp**, **settingsBlockSystemPage**, **settingsBlockDevicesPage**, **settingsBlockNetworkInternetPage**, **settingsBlockPersonalizationPage**, **settingsBlockAccountsPage**, **settingsBlockTimeLanguagePage**, **settingsBlockEaseOfAccessPage**, **settingsBlockPrivacyPage**, **settingsBlockUpdateSecurityPage**, **experienceBlockWindowsSpotlight**, **experienceBlockWindowsTips**, **experienceBlockConsumerSpecificFeatures**, **startMenuLayoutXml**, **startMenuMode**, **logonBlockFastUserSwitching** und **startBlockUnpinningAppsFromTaskbar** wurden der [windows10GeneralConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10generalconfiguration)-Entität hinzugefügt.|
|Änderung|Beta|Die Eigenschaften **allowPrinting**, **allowScreenCapture** und **allowTextSuggestion** wurden der [windows10SecureAssessmentConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10secureassessmentconfiguration) Entität hinzugefügt.|
|Änderung|Beta|Die Eigenschaften **blockPrinting**, **blockScreenCapture** und **blockTextSuggestion** wurden der [windows10SecureAssessmentConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10secureassessmentconfiguration)-Entität hinzugefügt.|
|Änderung|Beta|Die **identityName**-Eigenschaft wurde der [windowsAppX](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_windowsappx)-Entität hinzugefügt.|
|Änderung|Beta|Der Typ der folgenden Eigenschaften in der [windowsAppX](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_windowsappx)-Entität wurde geändert:<br/>**applicableArchitectures** von [windowsArchitecture](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/windowsArchitecture) in „Zeichenfolge“<br/>|
|Änderung|Beta|Die **identityName**-Eigenschaft wurde der [windowsPhone81AppX](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_windowsphone81appx)-Entität hinzugefügt.|
|Änderung|Beta|Der Typ der folgenden Eigenschaften in der  [windowsPhone81AppX](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_windowsphone81appx)-Entität wurde geändert:<br/>**applicableArchitectures** von [windowsArchitecture](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/windowsArchitecture) in „Zeichenfolge“<br/>|
|Änderung|Beta|Die Eigenschaften **identityName**, **identityPublisherHash** und **identityResourceIdentifier** wurden der [windowsUniversalAppX](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_windowsuniversalappx)-Entität hinzugefügt.|
|Änderung|Beta|Der Typ der folgenden Eigenschaften in der  [windowsUniversalAppX](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_windowsuniversalappx)-Entität wurde geändert:<br/>**applicableArchitectures** von [windowsArchitecture](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/windowsArchitecture) in „Zeichenfolge“<br/>**applicableDeviceTypes** von [windowsDeviceType](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/windowsDeviceType) in „Zeichenfolge“<br/>|
|Änderung|Beta|Die **restartMode**-Eigenschaft wurde der [windowsUpdateForBusinessConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsupdateforbusinessconfiguration)-Entität hinzugefügt.|
|Änderung|Beta|Die **managedDeviceCertificateStates**-Navigationseigenschaft wurde der [androidForWorkScepCertificateProfile](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidforworkscepcertificateprofile)-Entität hinzugefügt.|
|Änderung|Beta|Die **managedDeviceCertificateStates**-Navigationseigenschaft wurde der [androidScepCertificateProfile](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidscepcertificateprofile)-Entität hinzugefügt.|
|Änderung|Beta|Die Navigationseigenschaften **enterpriseCodeSigningCertificates**, **symantecCodeSigningCertificate**, **sideLoadingKeys**, **managedAppPolicies**, **iosManagedAppProtections**, **androidManagedAppProtections**, **defaultManagedAppProtections**, **targetedManagedAppConfigurations**, **mdmWindowsInformationProtectionPolicies**, **windowsInformationProtectionPolicies**, **managedAppRegistrations** und **managedAppStatuses** wurden der [deviceAppManagement](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_deviceappmanagement)-Entität hinzugefügt.|
|Änderung|Beta|Die Eigenschaften **appReportingOverview**, **enterpriseCerts** und **symantecCert** wurden aus der [deviceAppManagement](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_deviceappmanagement)-Entität entfernt.|
|Änderung|Beta|Die **deviceSettingStateSummaries**-Navigationseigenschaft wurde der [deviceCompliancePolicy](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancepolicy)-Entität hinzugefügt.|
|Änderung|Beta|Die **deviceSettingStateSummaries**-Navigationseigenschaft wurde der [deviceConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfiguration)-Entität hinzugefügt.|
|Änderung|Beta|Die Navigationseigenschaften **termsAndConditions**, **androidForWorkSettings**, **androidForWorkAppConfigurationSchemas**, **applePushNotificationCertificate**, **softwareUpdateStatusSummary**, **deviceCompliancePolicyDeviceStateSummary**, **complianceSettingStateSummaries**, **deviceConfigurationDeviceStateSummaries** und **mobileThreatDefenseConnectors** wurden der [deviceManagement](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_androidforwork_devicemanagement)-Entität hinzugefügt.|
|Änderung|Beta|Die Navigationseigenschaften **teacherRootCertificates**, **teacherIdentityCertificate**, **studentRootCertificates** und **studentIdentityCertificate** wurden aus der [iosEducationDeviceConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioseducationdeviceconfiguration)-Entität entfernt.|
|Änderung|Beta|Der Typ der folgenden Eigenschaften in der [iosLobAppProvisioningConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_ioslobappprovisioningconfiguration)-Entität wurde geändert:<br/>**deviceStatuses** von [managedDeviceMobileAppProvisioningConfigurationDeviceStatus](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/managedDeviceMobileAppProvisioningConfigurationDeviceStatus)-Sammlung in [managedDeviceMobileAppConfigurationDeviceStatus](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_manageddevicemobileappconfigurationdevicestatus)-Sammlung<br/>**groupAssignments** von [appProvisioningConfigGroupAssignment](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/appProvisioningConfigGroupAssignment)-Sammlung in [mobileAppProvisioningConfigGroupAssignment](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_mobileappprovisioningconfiggroupassignment)-Sammlung<br/>|
|Änderung|Beta|Die **managedDeviceCertificateStates**-Navigationseigenschaft wurde der [iosScepCertificateProfile](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosscepcertificateprofile)-Entität hinzugefügt.|
|Änderung|Beta|Die **managedDeviceCertificateStates**-Navigationseigenschaft wurde der [macOSScepCertificateProfile](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_macosscepcertificateprofile)-Entität hinzugefügt.|
|Änderung|Beta|Die Navigationseigenschaften **deviceConfigurationStates** und **deviceCompliancePolicyStates** wurden der [managedDevice](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_manageddevice)-Entität hinzugefügt.|
|Änderung|Beta|Die Navigationseigenschaften **deviceStatusSummary** und **userStatusSummary** wurden der [managedDeviceMobileAppConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_manageddevicemobileappconfiguration)-Entität hinzugefügt.|
|Änderung|Beta|Die **installSummary**-Navigationseigenschaft  wurde der [mobileApp](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_mobileapp)-Entität hinzugefügt.|
|Änderung|Beta|Die **sideLoadingKeys**-Navigationseigenschaft wurde aus der [organization](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_onboarding_organization)-Entität entfernt.|
|Änderung|Beta|Die **managedDeviceCertificateStates**-Navigationseigenschaft wurde der [windows81SCEPCertificateProfile](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows81scepcertificateprofile)-Entität hinzugefügt.|
|Änderung|Beta|Die **managedDeviceCertificateStates**-Navigationseigenschaft wurde der [windowsPhone81SCEPCertificateProfile](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsphone81scepcertificateprofile)-Entität hinzugefügt.|
|Änderung|Beta|Die Eigenschaften **applicationId**, **appName**, **platformId**, **userFailures** und **deviceFailures** wurden aus dem komplexen Typ [appInstallationFailure](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_appinstallationfailure) entfernt.|
|Änderung|Beta|Die **displayName**-Eigenschaft wurde dem komplexen Typ [iosHomeScreenFolderPage](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioshomescreenfolderpage) hinzugefügt.|
|Änderung|Beta|Die **displayName**-Eigenschaft wurde dem komplexen Typ [iosHomeScreenPage](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioshomescreenpage) hinzugefügt.|
|Änderung|Beta|Die Eigenschaften **subjectName**, **description**, **expirationDateTime** und **certificate** wurden dem komplexen Typ [windowsInformationProtectionDataRecoveryCertificate](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotectiondatarecoverycertificate) hinzugefügt.|
|Änderung|Beta|Die Eigenschaften **dataRecoveryCertificate** und **certificateFileName** wurden aus dem komplexen Typ [ wurwindowsInformationProtectionDataRecoveryCertificate](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotectiondatarecoverycertificate) entfernt.|
|Änderung|Beta|Die **displayName**-Eigenschaft wurde dem komplexen Typ [windowsPackageInformation](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_windowspackageinformation) hinzugefügt.|
|Änderung|Beta|Der Typ der folgenden Eigenschaften im komplexen Typ [windowsPackageInformation](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_windowspackageinformation) wurde geändert:<br/>**applicableArchitecture** von [windowsArchitecture](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/windowsArchitecture) in „Zeichenfolge“<br/>|
|Änderung|Beta|Die folgenden Eigenschaften im komplexen Typ  [windowsPackageInformation](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_windowspackageinformation) wurden geändert:<br/>**applicableArchitecture** von „Optional“ in „Erforderlich“<br/>|

### <a name="add-contracts-to-microsoft-graph"></a>Hinzufügen von Verträgen zu Microsoft Graph

|**Änderungstyp**|**Version**|**Beschreibung**|
|:-------------|:-----------|:--------------|
|Ergänzungen|Beta|Neue Ressource</br>[contract](https://graph.microsoft.io/en-us/docs/api-reference/beta/resources/contract) |

### <a name="add-domain-operations-to-microsoft-graph"></a>Hinzufügen von Domänenvorgängen zu Microsoft Graph

|**Änderungstyp**|**Version**|**Beschreibung**|
|:-------------|:-----------|:--------------|
|Ergänzungen|Beta|Funktionen wurden zu [Domänen](https://graph.microsoft.io/en-us/docs/api-reference/beta/resources/domain) hinzugefügt.<br/>Neue Entitäten:</br>[domain](https://graph.microsoft.io/en-us/docs/api-reference/beta/resources/domain)<br/>[domainDnsRecord](https://graph.microsoft.io/en-us/docs/api-reference/beta/resources/domaindnsrecord)<br/>[domainDnsCnameRecord](https://graph.microsoft.io/en-us/docs/api-reference/beta/resources/domainDnsCnameRecord)<br/>[domainDnsMxRecord](https://graph.microsoft.io/en-us/docs/api-reference/beta/resources/domainDnsMxRecord)<br/>[domainDnsSrvRecord](https://graph.microsoft.io/en-us/docs/api-reference/beta/resources/domainDnsSrvRecord)<br/>[domainDnsTxtRecord](https://graph.microsoft.io/en-us/docs/api-reference/beta/resources/domainDnsTxtRecord)<br/>[domainDnsUnavailableRecord](https://graph.microsoft.io/en-us/docs/api-reference/beta/resources/domainDnsUnavailableRecord)<br/>Neue Aktionen:</br>[forceDelete](https://graph.microsoft.io/en-us/docs/api-reference/beta/api/domain_forcedelete)</br>[verify](https://graph.microsoft.io/en-us/docs/api-reference/beta/api/domain_verify) |

### <a name="add-custom-data-to-microsoft-graph-using-schema-extensions"></a>Hinzufügen von benutzerdefinierten Daten zu Microsoft Graph unter Verwendung von Schemaerweiterungen

|**Änderungstyp**|**Version**|**Beschreibung**|
|:-------------|:-----------|:--------------|
|Ergänzungen|Beta|Erweitern von Microsoft Graph mit Anwendungsdaten unter Verwendung von [Schemaerweiterungen](https://developer.microsoft.com/en-us/graph/docs/concepts/extensibility_overview#schema-extensions-preview).  Dies wird in den folgenden Ressourcen unterstützt:<br/>Administrative Einheit<br/>Kalenderereignis<br/>Gerät<br/>Gruppe<br/>Nachricht<br/>Organisation<br/>Privater Kontakt<br/>Beitrag<br/>Benutzer<br/>Sehen Sie sich das folgende Beispiel an:<br/>[Hinzufügen von benutzerdefinierten Daten zu Gruppen mithilfe von Schemaerweiterungen (Preview)](https://developer.microsoft.com/en-us/graph/docs/concepts/extensibility_schema_groups)|
|Ergänzungen|Beta|Es wurde eine alternative Möglichkeit zum Erstellen einer Schemaerweiterungsdefinition bereitgestellt, ohne dass eine überprüfte Vanity-.com-Domäne erforderlich ist. Weitere Informationen finden Sie unter [Schemaerweiterungen](https://developer.microsoft.com/en-us/graph/docs/concepts/extensibility_overview#schema-extensions-preview).|

### <a name="add-custom-data-to-microsoft-graph-using-open-extensions"></a>Hinzufügen von benutzerdefinierten Daten zu Microsoft Graph unter Verwendung von offenen Erweiterungen

|**Änderungstyp**|**Version**|**Beschreibung**|
|:-------------|:-----------|:--------------|
|Änderung| v1.0 und Beta | Die bisherigen „Office 365-Datenerweiterungen“ wurden in „offene Erweiterungen“ umbenannt. |
|Ergänzungen|Beta|Es wurden Ressourcen hinzugefügt, die [offene Erweiterungen](https://developer.microsoft.com/en-us/graph/docs/concepts/extensibility_overview#open-extensions) unterstützen: <br/>Administrative Einheit<br/>Gerät<br/>Gruppe<br/>Organisation<br/>Benutzer<br/>Sehen Sie sich das folgende Beispiel an:<br/>[Hinzufügen von benutzerdefinierten Daten zu Benutzern mithilfe offener Erweiterungen (Preview)](https://developer.microsoft.com/en-us/graph/docs/concepts/extensibility_open_users)|

### <a name="directory-apis"></a>Verzeichnis-APIs

|**Änderungstyp**|**Version**|**Beschreibung**|
|:-------------|:-----------|:--------------|
|Ergänzungen|Beta|Es wurde Unterstützung zum [Wiederherstellen und endgültigen Löschen von Gruppen](https://graph.microsoft.io/en-us/docs/api-reference/beta/resources/directory) hinzugefügt.<br/>Neue Entität: Verzeichnis mit deleteditems-Navigationseigenschaft. |
|Ergänzungen|Beta|Neue Entität:</br>[Endpunkt](https://graph.microsoft.io/en-us/docs/api-reference/beta/resources/endpoint) |
|Änderung  |Beta|Neue [endpoint](https://graph.microsoft.io/en-us/docs/api-reference/beta/api/group_list_endpoints)-Nagivationseigenschaft in [Gruppen](https://graph.microsoft.io/en-us/docs/api-reference/beta/resources/group) |
|Ergänzungen|Beta|Neue Entität:</br>[licenseDetails](https://graph.microsoft.io/en-us/docs/api-reference/beta/resources/licensedetails) |
|Änderung  |Beta|Neue [licensedetails](https://graph.microsoft.io/en-us/docs/api-reference/beta/api/user_list_licensedetails)-Nagivationseigenschaft für [Benutzer](https://graph.microsoft.io/en-us/docs/api-reference/beta/resources/user) |

### <a name="reports-apis"></a>Bericht-APIs

|**Änderungstyp**|**Version**|**Beschreibung**|
|:-------------|:-----------|:--------------|
|Ergänzungen|Beta|Die neue Vorschau-API für Office 365-Berichte wurde eingeführt. Sie können sie zum Abrufen von Verwendungsberichten darüber verwenden, wie Personen in Ihrem Unternehmen Office 365-Dienste nutzen. Sie können zum Beispiel identifizieren, wer einen Dienst häufig verwendet und Kontingente erreicht oder wer vielleicht gar keine Office 365-Lizenz benötigt. Weitere Informationen finden Sie unter [Bericht](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/report).|

### <a name="directory-apis"></a>Verzeichnis-APIs

|**Änderungstyp**|**Version**|**Beschreibung**|
|:-------------|:-----------|:--------------|
|Ergänzungen|Beta|Neue Entität:</br>[contract](https://graph.microsoft.io/en-us/docs/api-reference/beta/resources/contract) |

## <a name="february-2017"></a>Februar 2017

### <a name="intune-apis"></a>Intune APIs

|Änderungstyp|Version|Beschreibung|
|:---|:---|:---|
|Ergänzungen|Beta|Hinzugefügte neue Entitäten:<br/>[androidForWorkCertificateProfileBase](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidforworkcertificateprofilebase)<br/>[androidForWorkEasEmailProfileBase](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidforworkeasemailprofilebase)<br/>[androidForWorkEnterpriseWiFiConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidforworkenterprisewificonfiguration)<br/>[androidForWorkGmailEasConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidforworkgmaileasconfiguration)<br/>[androidForWorkNineWorkEasConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidforworknineworkeasconfiguration)<br/>[androidForWorkPkcsCertificateProfile](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidforworkpkcscertificateprofile)<br/>[androidForWorkScepCertificateProfile](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidforworkscepcertificateprofile)<br/>[androidForWorkTrustedRootCertificate](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidforworktrustedrootcertificate)<br/>[androidForWorkWiFiConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidforworkwificonfiguration)<br/>[appleDeviceFeaturesConfigurationBase](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_appledevicefeaturesconfigurationbase)<br/>[appProvisioningConfigGroupAssignment](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_appprovisioningconfiggroupassignment)<br/>[deviceComplianceUserOverview](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecomplianceuseroverview)<br/>[deviceConfigurationUserOverview](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationuseroverview)<br/>[enterpriseCertificate](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_enterprisecertificate)<br/>[iosEducationDeviceConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioseducationdeviceconfiguration)<br/>[macOSDeviceFeaturesConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_macosdevicefeaturesconfiguration)<br/>[managedAndroidLobApp](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_managedandroidlobapp)<br/>[managedDeviceMobileAppProvisioningConfigurationDeviceStatus](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_manageddevicemobileappprovisioningconfigurationdevicestatus)<br/>[managedIOSLobApp](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_managedioslobapp)<br/>[managedMobileLobApp](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_managedmobilelobapp)<br/>[symantecCertificate](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_symanteccertificate)<br/>[windowsAppX](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_windowsappx)<br/>[windowsCertificateProfileBase](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowscertificateprofilebase)<br/>[windowsPhone81AppX](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_windowsphone81appx)<br/>[windowsPhone81AppXBundle](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_windowsphone81appxbundle)<br/>[windowsPhoneXAP](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_windowsphonexap)<br/>[windowsUniversalAppX](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_windowsuniversalappx)<br/>|
|Ergänzungen|Beta|Die folgenden komplexen Typen wurden hinzugefügt:<br/>[airPrintDestination](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_airprintdestination)<br/>[windowsArchitecture](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_windowsarchitecture)<br/>[windowsDeviceType](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_windowsdevicetype)<br/>[windowsMinimumOperatingSystem](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_windowsminimumoperatingsystem)<br/>[windowsPackageInformation](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_windowspackageinformation)<br/>|
|Ergänzungen|Beta|Die [assign](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_apps_ioslobappprovisioningconfiguration_assign)-Aktion wurde der [iosLobAppProvisioningConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_ioslobappprovisioningconfiguration)-Entität hinzugefügt.|
|Ergänzungen|Beta|Die [scheduleActionsForRules](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_deviceconfig_devicecompliancepolicy_scheduleactionsforrules)-Aktion wurde der [deviceCompliancePolicy](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancepolicy)-Entität hinzugefügt.|
|Ergänzungen|Beta|Die [updateTargetedSecurityGroups](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_mam_targetedmanagedappconfiguration_updatetargetedsecuritygroups)-Aktion wurde der [targetedManagedAppConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_targetedmanagedappconfiguration)-Entität hinzugefügt.|
|Ergänzungen|Beta|Die [getScopesForUser](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_rbac_resourceoperation_getscopesforintune_devices_user)-Funktion wurde der [resourceOperation](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_rbac_resourceoperation)-Entität hinzugefügt.|
|Änderung|Beta|Die **manifest**-Eigenschaft wurde aus der [androidLobApp](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_androidlobapp)-Entität entfernt.|
|Änderung|Beta|Die Eigenschaften **assetTagTemplate**, **lockScreenFootnote**, **homeScreenDockIcons** und **homeScreenPages**wurden der [iosDeviceFeaturesConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosdevicefeaturesconfiguration)-Entität hinzugefügt.|
|Änderung|Beta|Die Eigenschaften **deviceSharingAssetTagInformation**, **deviceSharingLockScreenFootnote**, **homeScreenLayoutDockIcons** und **homeScreenLayoutPages** wurden aus der [iosDeviceFeaturesConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosdevicefeaturesconfiguration)-Entität entfernt.|
|Änderung|Beta|Die **appsSingleAppModeBundleIds**-Eigenschaft wurde der [iosGeneralDeviceConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosgeneraldeviceconfiguration)-Entität hinzugefügt.|
|Änderung|Beta|Die **manifest**-Eigenschaft wurde aus der [iosLobApp](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_ioslobapp)-Entität entfernt.|
|Änderung|Beta|Die Eigenschaften **createdDateTime**, **description**, **lastModifiedDateTime**, **displayName** und **version** wurden der [iosLobAppProvisioningConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_ioslobappprovisioningconfiguration)-Entität hinzugefügt.|
|Änderung|Beta|Die Eigenschaften **createdDateTime** und **lastModifiedDateTime** wurden der [managedAppPolicy](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_managedapppolicy)-Entität hinzugefügt.|
|Änderung|Beta|Die **deviceRegistrationState**-Eigenschaft wurde aus der [managedDevice](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_devices_manageddevice)-Entität entfernt.|
|Änderung|Beta|Die **manifest**-Eigenschaft wurde der [mobileAppContentFile](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_mobileappcontentfile)-Entität hinzugefügt.|
|Änderung|Beta|Die Eigenschaften **osDescription** und **userName** wurden der [mobileAppInstallStatus](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_mobileappinstallstatus)-Entität hinzugefügt.|
|Änderung|Beta|Die **deviceType**-Eigenschaft wurde aus der [mobileAppInstallStatus](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_mobileappinstallstatus)-Entität entfernt.|
|Änderung|Beta|Der Typ der folgenden Eigenschaften wurde aus der [mobileAppInstallStatus](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_mobileappinstallstatus)-Entität entfernt:<br/>**mobileAppInstallStatusValue** von „Int32“ in „String“|
|Änderung|Beta|Die Eigenschaften **targetedSecurityGroupIds** und **targetedSecurityGroupsCount** wurden der [targetedManagedAppConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_targetedmanagedappconfiguration)-Entität hinzugefügt.|
|Änderung|Beta|Die **numberOfTargetedSecurityGroups**-Eigenschaft wurde aus der [targetedManagedAppConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_targetedmanagedappconfiguration)-Entität entfernt.|
|Änderung|Beta|Die **Id**-Eigenschaft wurde der [user](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_devices_user)-Entität hinzugefügt.|
|Änderung|Beta|Die Eigenschaften **renewalThresholdPercentage**, **keyStorageProvider**, **subjectNameFormat**, **subjectAlternativeNameType**, **certificateValidityPeriodValue** und **certificateValidityPeriodScale** wurden aus der [windows10CertificateProfileBase](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10certificateprofilebase)-Entität entfernt.|
|Änderung|Beta|Die Eigenschaften **renewalThresholdPercentage**, **keyStorageProvider**, **subjectNameFormat**, **subjectAlternativeNameType**, **certificateValidityPeriodValue** und **certificateValidityPeriodScale** wurden aus der [windows81CertificateProfileBase](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows81certificateprofilebase)-Entität entfernt.|
|Änderung|Beta|Die **applyToWindows10Mobile**-Eigenschaft wurde aus der [windowsPhone81GeneralConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsphone81generalconfiguration)-Entität entfernt.|
|Änderung|Beta|Die Navigationseigenschaften **enterpriseCerts**, **iosLobAppProvisioningConfigurations** und **symantecCert** wurden der [deviceAppManagement](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_deviceappmanagement)-Entität hinzugefügt.|
|Änderung|Beta|Die **userStatusOverview**-Navigationseigenschaft wurde der [deviceCompliancePolicy](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancepolicy)-Entität hinzugefügt.|
|Änderung|Beta|Die **userStatusOverview**-Navigationseigenschaft wurde der [deviceConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfiguration)-Entität hinzugefügt.|
|Änderung|Beta|Die Navigationseigenschaften **groupAssignments**, **deviceStatuses** und **userStatuses** wurden der [iosLobAppProvisioningConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_ioslobappprovisioningconfiguration)-Entität hinzugefügt.|
|Änderung|Beta|Der Typ der folgenden Eigenschaften in der [windows10VpnConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10vpnconfiguration)-Entität wurde geändert:<br/>
  **identityCertificate** von [windows10CertificateProfileBase](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10certificateprofilebase) in [windowsCertificateProfileBase](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowscertificateprofilebase)|
|Änderung|Beta|Die Eigenschaften **deviceComplianceCheckinThresholdDays** und **isScheduledActionEnabled** wurden dem komplexen Typ [deviceManagementSettings](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicemanagementsettings) hinzugefügt.|
|Änderung|Beta|Die Eigenschaften **windowsCommercialId** und **windowsCommercialIdLastModifiedTime** wurden aus dem komplexen Typ [deviceManagementSettings](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicemanagementsettings) entfernt.|
|Änderung|Beta|Die Eigenschaften **bundleID**, **appName**, **publisher**, **enabled** und **showOnLockScreen** wurden dem komplexen Typ [iosNotificationSettings](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosnotificationsettings) hinzugefügt.|
|Änderung|Beta|Die Eigenschaften **bundleIdentifier**, **notificationsEnabled** und **showInLockScreen** wurden aus dem komplexen Typ [iosNotificationSettings](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosnotificationsettings) entfernt.|



## <a name="january-2017"></a>Januar 2017

### <a name="outlook-calendar"></a>Outlook-Kalender

|**Änderungstyp**|**Version**|**Beschreibung**|
|:-------------|:-----------|:--------------|
|Ergänzungen|v1.0|Neue Aktion [findMeetingTimes](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/api/user_findmeetingtimes) für die [Benutzer](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/user)-Ressource.|
|Ergänzungen|v1.0|Neuer komplexer Typ [attendeeBase](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/attendeebase), der  aus einer Typeigenschaft für den Teilnehmertyp besteht.|
|Ergänzungen|v1.0|Neue komplexe Typen:<br/>[attendeeAvailability](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/attendeeavailability)<br/>[locationConstraint](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/locationconstraint) <br/>[locationConstraintItem](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/locationconstraintitem)<br/>[meetingTimeSuggestion](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/meetingtimesuggestion)<br/>[meetingTimeSuggestionsResult](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/meetingtimesuggestionsresult)<br/>[timeConstraint](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/timeconstraint)<br/>[timeSlot](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/timeslot)|
|Änderung|v1.0|Der komplexe Typ des [Teilnehmers](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/attendee) wird jetzt von AttendeeBase abgeleitet, der wiederum vom [Empfänger](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/recipient) abgeleitet wird. Einschließlich die vererbten Eigenschaften besteht es aus denselben **Status**-, **Typ**- und **E-Mail-Adresse**-Eigenschaften wie zuvor.|
|Ergänzungen|Beta|hexColor zur [Kalender](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/calendar)-Ressource hinzugefügt.|

### <a name="intune-apis"></a>Intune APIs

|**Änderungstyp**|**Version**|**Beschreibung**|
|:-------------|:-----------|:--------------|
|Ergänzungen|Beta|Hinzugefügte neue Entitäten: <br/>[appReportingOverviewStatus](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_appreportingoverviewstatus)<br/>[deviceComplianceDeviceOverview](https://developer.microsoft.com/en-us/graph/docs//api-reference/beta/resources/intune_deviceconfig_devicecompliancedeviceoverview)<br/>[deviceConfigurationDeviceOverview](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationdeviceoverview)<br/>[deviceManagementExchangeOnpremisesPolicy](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_onboarding_devicemanagementexchangeonpremisespolicy)<br/>[iosDeviceFeaturesConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosdevicefeaturesconfiguration)<br/>[iosEducationDeviceConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioseducationdeviceconfiguration)<br/>[iosLobAppProvisioningConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_ioslobappprovisioningconfiguration)<br/>[onpremisesConditionalAccessSettings](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_onboarding_onpremisesconditionalaccesssettings)<br/>[sharedPCConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_sharedpcconfiguration)<br/>[windows10EnterpriseModernAppManagementConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10enterprisemodernappmanagementconfiguration)<br/>[windows10SecureAssessmentConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10secureassessmentconfiguration)<br/>[windows10WindowsInformationProtectionConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10windowsinformationprotectionconfiguration)|
|Ergänzungen|Beta|Die folgenden kompleen Typen wurden hinzugefügt: <br/> [appInstallationFailure](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_appinstallationfailure)<br/>[enterpriseCloudResource](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_enterprisecloudresource)<br/>[iosHomeScreenApp](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioshomescreenapp)<br/>[iosHomeScreenFolder](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioshomescreenfolder)<br/>[iosHomeScreenFolderPage](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioshomescreenfolderpage)<br/>[iosHomeScreenItem](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioshomescreenitem)<br/>[iosHomeScreenPage](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioshomescreenpage)<br/>[iosNotificationSettings](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosnotificationsettings)<br/>[iPv6Range](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_ipv6range)<br/>[sharedPCAccountManagerPolicy](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_sharedpcaccountmanagerpolicy)<br/>[windowsInformationProtectionAppRule](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsinformationprotectionapprule)<br/>[windowsInformationProtectionAppRuleAppLockerPolicyFileTemplate](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsinformationprotectionappruleapplockerpolicyfiletemplate)<br/>[windowsInformationProtectionAppRuleDesktopTemplate](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsinformationprotectionappruledesktoptemplate)<br/>[windowsInformationProtectionAppRuleStoreAppTemplate](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsinformationprotectionapprulestoreapptemplate)<br/>[windowsInformationProtectionAppRuleTemplate](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsinformationprotectionappruletemplate)<br/>[windowsInformationProtectionCorporateNetworkLocation](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsinformationprotectioncorporatenetworklocation)<br/>[windowsInformationProtectionDataRecoveryCertificate](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsinformationprotectiondatarecoverycertificate)<br/>[windowsInformationProtectionProtectedLocation](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsinformationprotectionprotectedlocation)<br/>[windowsInformationProtectionProtectedLocationEnterpriseCloudResources](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsinformationprotectionprotectedlocationenterprisecloudresources)<br/>[windowsInformationProtectionProtectedLocationEnterpriseInternalProxyServers](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsinformationprotectionprotectedlocationenterpriseinternalproxyservers)<br/>[windowsInformationProtectionProtectedLocationEnterpriseIPv4Ranges](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsinformationprotectionprotectedlocationenterpriseipv4ranges)<br/>[windowsInformationProtectionProtectedLocationEnterpriseIPv6Ranges](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsinformationprotectionprotectedlocationenterpriseipv6ranges)<br/>[windowsInformationProtectionProtectedLocationEnterpriseNetworkDomainNames](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsinformationprotectionprotectedlocationenterprisenetworkdomainnames)<br/>[windowsInformationProtectionProtectedLocationEnterpriseProxyServers](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsinformationprotectionprotectedlocationenterpriseproxyservers)<br/>[windowsInformationProtectionProtectedLocationNeutralResources](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsinformationprotectionprotectedlocationneutralresources)
|Löschung|Beta|Die folgenden komplexen Typen wurden entfernt und durch microsoft.graph.json ersetzt:<br/>managedAppDeploymentSummary <br/>managedAppSummary<br /> |
|Ändern|Beta|Der Eigenschaftentyp „appConfigComplianceStatus“ wurde in den folgenden Entitäten durch „complianceStatus“ ersetzt: <br/>[managedDeviceMobileAppConfigurationDeviceStatus](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_manageddevicemobileappconfigurationdevicestatus)<br/>[managedDeviceMobileAppConfigurationUserStatus](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_manageddevicemobileappconfigurationuserstatus)|
|Änderung|Beta|Für die Ressource [managedAppStatusRaw](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_managedappstatusraw) wurde der Typ des Eigenschafteninhalts von „managedAppSummary“ in „json“ geändert.|
|Änderung|Beta|Die Funktion „getUsersWithFlaggedAppRegistration“ wurde aus der [managedAppRegistration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_managedappregistration)-Sammlung entfernt.|
|Änderung|Beta|Die Nagivationseigenschaft **vppToken** der [iosVppApp](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_iosvppapp)-Entität wurde so geändert, dass es sich nicht mehr um eine enthaltene Sammlung handelt.|
|Änderung|Beta|Die **deviceStatusOverview**-Eigenschaft wurde den Entitäten [deviceConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfiguration) und [deviceCompliancePolicy](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancepolicy) hinzugefügt.|
|Änderung|Beta|Die **appReportingOverview**-Eigenschaft wurde dem [deviceAppManagement](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_deviceappmanagement)-Singleton hinzugefügt.|
|Änderung|Beta|Die Eigenschaften **deviceDisplayName** und **userPrincipalName** wurden den Entitäten [deviceConfigurationDeviceStatus](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationdevicestatus), [deviceComplianceDeviceStatus](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancedevicestatus) und [managedDeviceMobileAppConfigurationDeviceStatus](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_manageddevicemobileappconfigurationdevicestatus) hinzugefügt.|
|Änderung|Beta|Die **ruleName**-Eigenschaft wurde der [deviceComplianceScheduledActionForRule](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancescheduledactionforrule)-Entität hinzugefügt.|
|Änderung|Beta|Die Eigenschaften **devicesCount**, **userDisplayName** und **userPrincipalName** wurden den Entitäten [deviceConfigurationUserStatus](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationuserstatus), [deviceComplianceUserStatus](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecomplianceuserstatus) und [managedDeviceMobileAppConfigurationUserStatus](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_manageddevicemobileappconfigurationuserstatus) hinzugefügt.|
|Änderung|Beta|Die [notificationMessageTemplates](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_notification_notificationmessagetemplate)-Sammlung wurde dem [deviceManagement](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicemanagement)-Singleton hinzugefügt.|
|Änderung|Beta|Die Eigenschaften **isDefault**, **lastModifiedDateTime**, **locale**, **messageTemplate** und **subject** wurden der [localizedNotificationMessage](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_localizednotificationmessage)-Entität hinzugefügt.|
|Änderung|Beta|Die Eigenschaften **azureActiveDirectoryDeviceId**, **deviceCategory**, **deviceRegistrationState** und **managementAgent** wurden der [managedDevice](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_onboarding_manageddevice)-Entität hinzugefügt.|
|Änderung|Beta|Die **lastModifiedDateTime**-Eigenschaft wurde der [mobileAppCategory](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_mobileappcategory)-Entität hinzugefügt.|
|Änderung|Beta|Die Eigenschaften **brandingOptions**, **defaultLocale**, **displayName**, **fromEmailAddress**, **lastModifiedDateTime** und **localizedNotificationMessages** wurden der [notificationMessageTemplate](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_notification_notificationmessagetemplate)-Entität hinzugefügt.|
|Änderung|Beta|Die Eigenschaften **appsAllowTrustedAppsSideloading**, **appsBlockWindowsStoreOriginatedApps**, **developerUnlockSetting**, **edgeBlockAccessToAboutFlags**, **edgeBlockDeveloperTools**, **edgeBlockExtensions**, **edgeBlockInPrivateBrowsing**, **edgeFirstRunUrl**, **edgeHomepageUrls**, **gameDvrBlocked**, **settingsBlockAddProvisioningPackage**, **settingsBlockChangeLanguage**, **settingsBlockChangePowerSleep**, **settingsBlockChangeRegion**, **settingsBlockChangeSystemTime**, **settingsBlockEditDeviceName**, **settingsBlockRemoveProvisioningPackage**, **sharedUserAppDataAllowed**, **smartScreenBlockPromptOverride**, **smartScreenBlockPromptOverrideForFiles**, **storageRestrictAppDataToSystemVolume**, **storageRestrictAppInstallToSystemVolume**, **webRtcBlockLocalhostIpAddress**, **windowsStoreBlockAutoUpdate** und **windowsStoreEnablePrivateStoreOnly** wurden der [windows10GeneralConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10generalconfiguration)-Entität hinzugefügt.|

## <a name="december-2016"></a>Dezember 2016

### <a name="delta-query"></a>Delta-Abfrage

|**Änderungstyp**|**Version**|**Beschreibung**|
|:-------------|:-----------|:--------------|
|Ergänzungen|Beta|Eine neue Deltafunktion zu folgenden Elemente hinzufügen, um [Delta Abfrage](https://developer.microsoft.com/en-us/graph/docs/concepts/delta_query_overview) auszuführen:<br/>contact<br/>contactFolder<br/>event<br/>group<br/>mailFolder<br/>message<br/>user<br/>Beispiele finden Sie unter Folgendem:<br/>
  [Inkrementelle Änderungen an Gruppen abrufen (Vorschau)](https://developer.microsoft.com/en-us/graph/docs/concepts/delta_query_groups)<br/>
  [Inkrementelle Änderungen an Nachrichten in einem Ordner abrufen (Vorschau)](https://developer.microsoft.com/en-us/graph/docs/concepts/delta_query_messages)<br/>
  [Inkrementelle Änderungen an Benutzern abrufen (Vorschau)](https://developer.microsoft.com/en-us/graph/docs/concepts/delta_query_users)|

### <a name="excel-apis"></a>Excel-APIs

|**Änderungstyp**|**Version**|**Beschreibung**|
|:-------------|:-----------|:--------------|
|Ergänzungen|v1.0|workbookPivotTable-Ressource, refresh- und refreshAll-Aktion für pivotTables, workbookRangeView-Ressource, visibleView-Aktion für den gefilterten Bereich zum Zurückgeben von workbookRangeView an den Benutzer, Abrufen der Sammlung rows und range-Ressource deaktiviert für visibleView, Funktionen columnsAfter, columnsBefore, resizedRange, rowsAbove und rowsBelow deaktiviert für range-Ressource und neue Tabelleneigenschaften hinzugefügt.|

### <a name="intune-apis"></a>Intune APIs

|**Änderungstyp**|**Version**|**Beschreibung**|
|:-------------|:-----------|:--------------|
|Ergänzungen|Beta|Ressourcen und Methode-APIs für Microsoft Intune hinzugefügt. Dies ist eine große Gruppe von Ressourcen und Methoden, um die öffentliche Vorschau von Intune auf Azure-Portal zu unterstützen. Informationen über den Dienst Intune finden Sie unter der [Intune Dokumentation](https://go.microsoft.com/fwlink/?linkid=836405). Informationen zu den Intune Ressourcen und APIs finden Sie unter [Arbeiten mit Intune in Microsoft Graph](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_graph_overview).|

## <a name="october-2016"></a>Oktober 2016

### <a name="authorization-provider"></a>Autorisierungsanbieter

|**Änderungstyp**|**Version**|**Beschreibung**|
|:-------------|:-----------|:--------------|
|Ergänzungen|v1.0 und Beta|Der v2-Authentifizierungsendpunkt unterstützt jetzt die OAuth-Clientgenehmigung „_credentials“, die für [Dämone und lange ausgeführte Prozesse in Geschäftsszenarien](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-protocols-oauth-client-creds/) verwendet werden kann.|
|Ergänzungen|v1.0 und Beta|Der v2-Authentifizierungsendpunkt unterstützt jetzt [Berechtigungsbereiche, die die Zustimmung des Administrators erfordern](http://developer.microsoft.com/en-us/graph/docs/concepts/permissions_reference), über den [Administratorzustimmungs-Endpunkt](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-scopes/#admin-restricted-scopes).|
|Ergänzungen|v1.0 und Beta|Der v2-Authentifizierungsendpunkt unterstützt jetzt die Administratorzustimmung für alle Benutzer in einem Mandanten über die [Administratorzustimmungs-Endpunkt](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-scopes/#admin-restricted-scopes).|

### <a name="invitation-apis"></a>Einladungs-APIs

|**Änderungstyp**|**Version**|**Beschreibung**|
|:-------------|:-----------|:--------------|
|Ergänzungen|Beta|Die invitedUserType-Eigenschaft wurde dem Einladungsentitätstyp hinzugefügt, der den Typ von Benutzer definiert (**Gast** oder **Mitglied**), der eingeladen wird.|
|Löschung|Beta|Die invitedToGroups-Eigenschaft wird am 11.11.2016 aus dem Einladungsentitätstyp entfernt. Dies bedeutet, dass Sie mithilfe dieser API keinen eingeladenen Benutzer mehr zu einer Gruppe hinzufügen können. Verwenden von [API zum Hinzufügen von Mitglieder](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/api/group_post_members) zum Hinzufügen eines Benutzers zu einer Gruppe.|

## <a name="september-2016"></a>September 2016

### <a name="azure-ad-application-proxy"></a>Azure AD-Anwendungsproxy

|**Änderungstyp**|**Version**|**Beschreibung**|
|:--------------|:-----------|:--------------|
|Ergänzungen|Beta|Azure AD-Anwendungsproxy-APIs sind jetzt im Beta-Endpunkt von Microsoft Graph verfügbar. Diese APIs ermöglichen die sichere Veröffentlichung von lokalen Anwendungen für Benutzer außerhalb des Organisationsnetzwerks unter Verwendung von Azure AD als allgemeine Zugriffssteuerebene. Mit den veröffentlichten APIs können Sie Anwendungen schreiben, die verschiedene Aspekte vom Anwendungsproxy abrufen und aktualisieren können, u. a. _Connectors_, _connectorGroups_ und _onPremisesPublishing_-Einstellungen einer Anwendung.|

### <a name="drive"></a>Laufwerk

|**Änderungstyp**|**Version**|**Beschreibung**|
|:--------------|:-----------|:--------------|
|Ergänzungen|Beta|Die _freigegebene_ Sammlung wurde hinzugefügt, um Zugriff auf freigegebene driveItems über shareId oder Freigabe-URL zu ermöglichen.|
|Ergänzungen|Beta|Die _search_-Funktion wurde zu einem Laufwerk hinzugefügt, um mehr Elemente als nur die im Stammordner des Laufwerks durchsuchen zu können.|


### <a name="driveitem"></a>DriveItem

|**Änderungstyp**|**Version**|**Beschreibung**|
|:--------------|:-----------|:--------------|
|Ergänzungen|Beta|Zusätzliche Unterstützung für _createUploadSession_, sodass Dateien, die größer als 4 MB sind, in OneDrive, OneDrive for Business und SharePoint-Dokumentbibliotheken hochgeladen werden können.|
|Ergänzungen|Beta|Die_sharepointIds_-Eigenschaft für driveItem wurde hinzugefügt, mit der die herkömmlichen IDs für SharePoint API für in SharePoint gespeicherte driveItems-Elemente zurückgegeben werden.|
|Ergänzungen|Beta|Zusätzliche Eigenschaften für _remoteItem_ hinzugefügt.|
|Ergänzungen|Beta|_quickXorHash_-Wert für Dateien in OneDrive for Business hinzugefügt.|
|Ergänzungen|Beta|Bereich für _createSharingLink_ hinzugefügt, mit dem Unternehmen freizugebende Links oder anonyme freizugebende Links erstellen können.|

### <a name="extended-properties"></a>Erweiterte Eigenschaften

|**Änderungstyp**|**Version**|**Beschreibung**|
|:--------------|:-----------|:--------------|
|Ergänzungen|v1.0|
  [Erweiterte Eigenschaften](http://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/extended-properties-overview) werden jetzt von folgenden Ressourcen unterstützt: Nachricht, mailFolder, Ereignis, Kalender, Kontakt, contactFolder, Gruppenereignis, Gruppenkalender, Gruppenbeitrag.|

### <a name="groups"></a>Gruppen

Unterstützung für dynamische Gruppenmitgliedschaft über die öffentliche Vorschau-API hinzugefügt, einschließlich der aufgelisteten Zusätze in der folgenden Tabelle:

|**Änderungstyp**|**Version**|**Beschreibung**|
|:--------------|:-----------|:--------------|
|Ergänzungen|Beta|Hinzugefügte **membershipRule**-Eigenschaft enthält Regeln, die die Mitgliedschaften für diese Gruppe steuern, wenn es sich bei der Gruppe um eine dynamische Gruppe handelt.|
|Ergänzungen|Beta|Die **membershipRuleProcessingState**-Eigenschaft wurde hinzugefügt, mit der gesteuert wird, ob die Verarbeitung dynamischer Mitgliedschaften für diese Gruppe aktiviert oder angehalten ist.|
|Ergänzungen|Beta|Legen Sie die **groupTypes**-Eigenschaft so fest, dass sie **„DynamicMembership“** enthält, um die Funktionen der dynamischen Gruppen für diese Gruppe zu erweitern|
|Ergänzungen|Beta|Die **preferredLanguage**-Eigenschaft wurde hinzugefügt, um die bevorzugte Sprache für eine Office 365-Gruppe anzugeben.|
|Ergänzungen|Beta|Die **theme**-Eigenschaft wurde hinzugefügt, um ein Farbschema für eine Office 365-Gruppe anzugeben.|

### <a name="hybrid-deployment-support"></a>Unterstützung für Hybridbereitstellung

|**Änderungstyp**|**Version**|**Beschreibung**|
|:--------------|:-----------|:--------------|
|Ergänzungen|v1.0|Apps können Version 1.0 von Outlook-Mail, -Kalender und Kontakte-APIs für den Zugriff auf lokale Postfächer in einer Hybridbereitstellung mit Exchange 2016 mit kumulativem Update 3 (KU3) verwenden. Erfahren Sie mehr über die REST-API-Unterstützung in [Hybridbereitstellungen](https://developer.microsoft.com/en-us/graph/docs/overview/hybrid_rest_support). **Hinweis:** Wenn Sie diese API-Sets in Version 1.0 verwenden, können Sie jetzt Ihre Apps, einschließlich Produktions-Apps für lokale Postfächer verwenden, die den spezifischen Anforderungen für Hybridbereitstellung entsprechen. Diese Funktion ist derzeit in der Vorschau.|

### <a name="identityriskevents"></a>IdentityRiskEvents

|**Änderungstyp**|**Version**|**Beschreibung**|
|:--------------|:-----------|:--------------|
|Änderung|Beta|Im Rahmen der Schemaänderungen, bei denen der Typ der zwei location-Eigenschaften durch einen neuen komplexen Typ in dem identityRiskEvents-Endpunkt ersetzt wird, werden die folgenden Eigenschaften für den identityRiskEvents-Endpunkt geändert/hinzugefügt:</br>**location** – geändert von Edm.String zu ComplexType signInLocation.<br/>**previousLocation** – geändert von Edm.String zu ComplexType signInLocation.<br/>**signInLocation** – neuer ComplexType, der Ort, Bundesland, countryOrRegion und geoCoordinates-Eigenschaften enthält.<br/>**geoCoordinates** – neuer ComplexType, der Breiten- und Längengradeigenschaften enthält.|

### <a name="invitation-manager"></a>Einladungs-Manager

|**Änderungstyp**|**Version**|**Beschreibung**|
|:--------------|:-----------|:--------------|
|Ergänzungen|Beta|Einladungs-Manager-APIs sind jetzt im Beta-Endpunkt von Microsoft Graph verfügbar. Verwenden Sie Einladungs-Manager-APIs, um eine Einladung zum Hinzufügen eines externen Benutzers zu der Organisation zu erstellen. Im Rahmen der Einladung können Sie auch angeben, ob der eingeladene Benutzer zu einer Office 365-Gruppe hinzugefügt werden soll. Weitere Informationen finden Sie im [Einladungs-Manager](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/invitation).|

### <a name="onedrive"></a>OneDrive

|**Änderungstyp**|**Version**|**Beschreibung**|
|:--------------|:-----------|:--------------|
|Ergänzungen|v1.0|**CreateUploadSession**-Methode für **driveItem** hinzugefügt, die Uploads von großen Dateien und wiederaufnehmbare Uploads ermöglicht.|
|Ergänzungen|v1.0|Eigenschaften für das Nachverfolgen von SharePoint-IDs für Elemente aus SharePoint (**sharepointIds**) und eine Eigenschaft zum Identifizieren von Stammordnern (**root**) hinzugefügt.|
|Ergänzungen|v1.0|**Shares**-Stammsammlung hinzugefügt, die mit shareIds oder Freigabelinks für den Zugriff auf freigegebene Elemente in OneDrive und SharePoint verwendet werden kann. Gibt den neuen Typ sharedDriveItem zurück.|
|Ergänzungen|v1.0|**Invite**-Methode für driveItem zum Hinzufügen von Berechtigungen für Elemente hinzugefügt. |
|Ergänzungen|v1.0|**Search**-Methode für das Laufwerk, mit der Elemente im Laufwerk und freigegebene Elemente durchsucht werden können hinzugefügt. |
|Ergänzungen|v1.0|**processingMetadata**-Eigenschaft für quickXorHash-Eigenschaft mit komplexem Dateityp für Hashes mit komplexem Typ hinzugefügt. |
|Ergänzungen|v1.0|**quickXorHash**-Eigenschaft für Hashes mit komplexem Typ hinzugefügt |

### <a name="outlook-calendar"></a>Outlook-Kalender

|**Änderungstyp**|**Version**|**Beschreibung**|
|:--------------|:-----------|:--------------|
|Ergänzungen|v1.0|
  **onlineMeetingUrl**-Eigenschaft zur [Ereignis](http://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/event)-Ressource hinzugefügt.|
|Ergänzungen|Beta|Die [forward](http://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/event_forward)-Aktion wurde zur Ereignisressource hinzugefügt.|
|Ergänzungen|Beta|Die folgenden Eigenschaften wurden zur [calendar](http://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/calendar)-Ressource zur Unterstützung der Freigabe von Kalendern hinzugefügt: **canEdit**, **canShare**, **canViewPrivateItems**, **isShared**, **isShareWithMe** und **Besitzer**.|

### <a name="outlook-mail"></a>Outlook-Mail

|**Änderungstyp**|**Version**|**Beschreibung**|
|:--------------|:-----------|:--------------|
|Ergänzungen|v1.0|
  [mailboxSettings](http://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/mailboxsettings) komplexer Typ, einschließlich der **automaticRepliesSetting**-, **timeZone**- und **Sprache**-Eigenschaften hinzugefügt.|
|Ergänzungen|v1.0|
  **mailboxSettings**-Eigenschaft zur [Benutzer](http://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/user)-Ressource hinzugefügt.|
|Ergänzungen|Beta|Unterstützung für das Erstellen, Auflisten, Abrufen und Löschen einer oder mehrerer Instanzen von [Erwähnungen](http://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/mention) in einer Nachricht hinzugefügt. Erwähnungen unterstützen Aufrufe, um die Aufmerksamkeit anderer Benutzer in einer Nachricht zu erhalten.|
|Ergänzungen|Beta|Unterstützung für die [getMailTips](http://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/user_getmailtips)-Aktion, um beliebige MailTips für bestimmte Empfänger zu erhalten hinzugefügt. Folgende Ressourcen wurden hinzugefügt: automaticRepliesMailTips, mailTips, mailTipsError.|

### <a name="query-parameters"></a>Abfrageparameter

|**Änderungstyp**|**Version**|**Beschreibung**|
|:--------------|:-----------|:--------------|
|Änderung|Beta|Abfrageparameter ohne '$' Präfixe sind ab dem 26.09.2016 unterstützt. Das Präfix '$' in der Abfrageparameter ist optional. Beispiele finden Sie unter [Abfrageparameter ohne $ Präfixe in Microsoft Graph unterstützen](http://dev.office.com/queryparametersinMicrosoftGraph).|

### <a name="sharepoint"></a>SharePoint

|**Änderungstyp**|**Version**|**Beschreibung**|
|:--------------|:-----------|:--------------|
|Ergänzungen|Beta|Zugriff auf SharePoint-Websites und [-listen nach ID](http://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/list_get) oder [Pfad/URL](http://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/baseitem_getbyurl).|
|Ergänzungen|Beta|Unterstützung für das [Auflisten, Erstellen, Abrufen und Löschen von Instanzen des listItem-Elements](http://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/listitem).|

### <a name="users"></a>Benutzer

|**Änderungstyp**|**Version**|**Beschreibung**|
|:--------------|:-----------|:--------------|
|Ergänzungen|Beta|Schreibgeschützte **refreshTokensValidFromDateTime**-Eigenschaft wurde hinzugefügt, um anzugeben, ab wann die Aktualisierungs- oder Sitzungstoken gültig sind. Alle Token, die vor diesem Zeitpunkt ausgestellt wurden, sind ungültig. Bei jedem Versuch, diese Token zu verwenden, werden Benutzer dazu aufgefordert, sich erneut anzumelden.|
|Ergänzungen|Beta|Die **showInAddressList**-Eigenschaft wurde hinzugefügt, mit der gesteuert wird, ob die globale Adressliste von Outlook diesen Benutzer enthalten soll.|
|Ergänzungen|Beta|Die **invalidateAllRefreshTokens**-Dienstaktion wurde hinzugefügt, mit der alle Aktualisierungs- und Sitzungstoken des Benutzers, die für Anwendungen ausgestellt wurden, ungültig werden, indem die **refreshTokensValidFromDateTime**-Benutzereigenschaft auf aktuelles Datum und aktuelle Uhrzeit zurückgesetzt wird.|


### <a name="webhooks"></a>Webhooks

|**Änderungstyp**|**Version**|**Beschreibung**|
|:--------------|:-----------|:--------------|
|Ergänzungen|Beta|Laufwerkstammelemente zu Webhooks als Ressource hinzugefügt, die abonniert werden kann.|

## <a name="august-2016"></a>August 2016

### <a name="contacts"></a>Kontakte

|**Änderungstyp**|**Version**|**Beschreibung**|
|:--------------|:-----------|:--------------|
|Ergänzungen|Beta|Im Rahmen der Schemaänderungen, bei denen einige Eigenschaften entfernt und entsprechende Sammlungen zu Kontaktendpunkten hinzugefügt wurden, wurden die folgenden Eigenschaften zu Kontaktendpunkten hinzugefügt: _Websites – Collection(ComplexType: Website)_,_Phones – Collection (ComplexType: Phone)_, _PostalAddress – Collection(ComplexType: PhysicalAddress)_. Weitere Informationen finden Sie unter dem Blogeintrag: [Upcoming changes to Contacts and People APIs](https://blogs.msdn.microsoft.com/exchangedev/2016/06/09/upcoming-changes-to-contacts-and-people-apis/).|
|Löschung|Beta|Im Rahmen der Schemaänderungen, bei denen einige Eigenschaften entfernt und entsprechende Sammlungen zu Kontaktendpunkten hinzugefügt wurden, wurden die folgenden Eigenschaften von Kontaktendpunkten entfernt: _BusinessHomePage_,_HomePhones_, _MobilePhone1_, _BusinessPhones_, _HomeAddress_, _BusinessAddress_, _OtherAddress_. Weitere Informationen finden Sie unter dem Blogeintrag: [Upcoming changes to Contacts and People APIs](https://blogs.msdn.microsoft.com/exchangedev/2016/06/09/upcoming-changes-to-contacts-and-people-apis/).|

### <a name="excel-apis"></a>Excel-APIs

|**Änderungstyp**|**Version**|**Beschreibung**|
|:--------------|:-----------|:--------------|
|Ergänzungen|v1.0|Excel REST-API für Microsoft Graph ist nun allgemein verfügbar. Sie können jetzt umfassende und genaue Integrationen mit Excel-Arbeitsmappen in Office 365 erstellen. Weitere Informationen finden Sie unter dem Blogeintrag [Power your apps with the new Excel REST API on the Microsoft Graph](http://dev.office.com/blogs/power-your-apps-with-the-new-excel-rest-api).|

### <a name="people"></a>Kontakte

|**Änderungstyp**|**Version**|**Beschreibung**|
|:--------------|:-----------|:--------------|
|Änderung|Beta|_WebSite_-Eigenschaft wurde in _Websites_ umbenannt. Weitere Informationen finden Sie unter [Upcoming changes to Contacts and People APIs](https://blogs.msdn.microsoft.com/exchangedev/2016/06/09/upcoming-changes-to-contacts-and-people-apis/).|

### <a name="privileged-identity-management"></a>Privileged Identity Management

|**Änderungstyp**|**Version**|**Beschreibung**|
|:--------------|:-----------|:--------------|
|Ergänzungen|Beta|REST-APIs für Privileged Identity Management (PIM) sind jetzt im Beta-Endpunkt von Microsoft Graph verfügbar. [Privileged Identity Management](https://azure.microsoft.com/en-us/documentation/articles/active-directory-privileged-identity-management-configure/) ermöglicht eine Just-In-Time-Aktivierung für privilegierte Azure AD-Rollen wie globaler Administrator, Abrechnungsadministrator usw. Mit den veröffentlichten APIs können Sie Anwendungen schreiben, die privilegierte Rollenzuweisungen abrufen und aktualisieren und Benutzer in Rollen aktivieren. Weitere Informationen finden Sie unter [Microsoft Graph: Azure AD Privileged Identity Management Vorschau-APIs sind verfügbar in Beta](http://dev.office.com/blogs/microsoft-graph-azure-ad-privileged-identity-management-apis-beta) und [Azure AD Privileged Identity Management](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/privilegedidentitymanagement_root).|

## <a name="july-2016"></a>Juli 2016

### <a name="administrative-units"></a>Administrative Einheiten

|**Änderungstyp**|**Version**|**Beschreibung**|
|:--------------|:-----------|:--------------|
|Ergänzungen|Beta|Die neue Administrative Unites preview API wurde eingeführt. Mit administrativen Einheiten können Organisationen ihre Azure Active Directory-Umgebung aufteilen und administrative Aufgaben auf diese Unterteilungen weitergeben. Unterteilungen können Regionen, Abteilungen, Kostenstellen usw. darstellen. Dies kann jetzt über die Microsoft Graph-API verwaltet werden.|

## <a name="june-2016"></a>Juni 2016

### <a name="identityriskevents"></a>IdentityRiskEvents

|**Änderungstyp**|**Version**|**Beschreibung**|
|:--------------|:-----------|:--------------|
|Ergänzungen|Beta|Die neue  IdentityRiskEvents Vorschau-API wurde eingeführt. Diese API funktioniert in Verbindung mit Azure Active Directory Identity Protection. Sie können Abfrage-Risiko-Ereignissen abfragen, die durch Identity Protection generiert wurden. Weitere Informationen finden Sie unter [Einführung einer neuen Vorschau-API für Microsoft Graph: IdentityRiskEvents](http://dev.office.com/blogs/identityriskevents-api-preview)-Blogeintrag.

### <a name="subscriptions"></a>Abonnements

|**Änderungstyp**|**Version**|**Beschreibung**|
|:--------------|:-----------|:--------------|
|Ergänzungen|Beta|Nur App-Bereiche werden jetzt für _Mail_- und _Kontakte_-Abonnements unterstützt.|

## <a name="may-2016"></a>Mai 2016

### <a name="calendar"></a>Kalender

|**Änderungstyp**|**Version**|**Beschreibung**|
|:--------------|:-----------|:--------------|
|Änderungen|Beta|Ändert sich zur findmeetingtimes-API. Weitere Informationen finden Sie unter dem Blogeintrag [Microsoft Graph findMeetingTimes API update](http://dev.office.com/microsoft-graph-findmeetingtimes-api-update) Blogbeitrag. Diese Änderung ist seit dem 19. Mai 2016 wirksam.

### <a name="contact"></a>Kontakt

|**Änderungstyp**|**Version**|**Beschreibung**|
|:--------------|:-----------|:--------------|
|Ergänzungen|v1.0|_Erweiterungen_ hinzugefügt, die einen abstrakten Typ für die Unterstützung des offenen Typs openTypeExtension von OData v4 darstellen.|

### <a name="directory"></a>Verzeichnis

|**Änderungstyp**|**Version**|**Beschreibung**|
|:--------------|:-----------|:--------------|
|Änderungen|Beta|_settingTemplateId_ in _templateId_ umbenannt. Diese Änderung wird ab dem 19. Mai 2016 wirksam.|

### <a name="event"></a>Ereignis

|**Änderungstyp**|**Version**|**Beschreibung**|
|:--------------|:-----------|:--------------|
|Ergänzungen|v1.0|_Erweiterungen_ hinzugefügt, die einen abstrakten Typ für die Unterstützung des offenen Typs openTypeExtension von OData v4 darstellen.|

### <a name="eventmessages"></a>EventMessages

|**Änderungstyp**|**Version**|**Beschreibung**|
|:--------------|:-----------|:--------------|
|Ergänzungen|v1.0|_inferenceClassification_ und _Erweiterungen_ zu _eventMessages_ hinzugefügt.|
|Ergänzungen|Beta|_responseRequested_ zu _eventMessageRequest_ hinzugefügt.|

### <a name="messages"></a>Nachrichten

|**Änderungstyp**|**Version**|**Beschreibung**|
|:--------------|:-----------|:--------------|
|Ergänzungen|v1.0|_inferenceClassification_ und _extensions_ zu _Nachrichten_ hinzugefügt.|
|Ergänzungen|Beta|_wellknownname_ zu _contactFolder_ hinzugefügt.|Ändert sich zu _findmeetingtimes_-API. Weitere Informationen finden Sie unter dem Blogeintrag [Microsoft Graph findMeetingTimes API update](http://dev.office.com/microsoft-graph-findmeetingtimes-api-update) Blogbeitrag. Diese Änderung wird ab dem 19. Mai 2016 wirksam.|

### <a name="post"></a>Beitrag

|**Änderungstyp**|**Version**|**Beschreibung**|
|:--------------|:-----------|:--------------|
|Ergänzungen|v1.0|_Erweiterungen_ hinzugefügt, die einen abstrakten Typ für die Unterstützung des offenen Typs openTypeExtension von OData v4 darstellen.|

### <a name="user"></a>Benutzer

|**Änderungstyp**|**Version**|**Beschreibung**|
|:--------------|:-----------|:--------------|
|Ergänzungen|v1.0|_inferenceClassification_-Ressourcentyp hinzugefügt.|
|Ergänzungen|Beta|_timeZone_ zu _mailboxsettings_ hinzugefügt.|
|Ergänzungen|Beta|API _findMeetingTimes _ zu _Benutzer_ hinzugefügt.|

## <a name="april-2016"></a>April 2016

### <a name="general"></a>Allgemein

|**Änderungstyp**|**Version**|**Beschreibung**|
|:--------------|:-----------|:--------------|
|Ergänzungen|v1.0 und Beta|Unterstützung für Berücksichtigung von _Accept-Encoding:gzip_ hinzugefügt.|
|Ergänzungen|v1.0|Unterstützung für Castsegment im erweiterten Pfad hinzugefügt. Beispiel: https://graph.microsoft.com/v1.0/me/messages?$expand=microsoft.graph.eventMessage/event|
|Ergänzungen|Beta|Unterstützung für PATCH-Anforderung anhand struktureller Eigenschaften hinzugefügt. Beispiel: 'PATCH /me/mailboxSettings'.|
|Ergänzungen|Beta|Azure Active Directory dient nun als Alternative für /beta/users/id/photo-Anforderungen, wenn Outlook die Anforderung nicht verarbeiten kann, beispielsweise wenn der Benutzer über keine Postfachlizenz oder der Mandant über kein Exchange Online-Abonnement verfügt. HINWEIS: Diese Alternative steht für GET und PATCH zur Verfügung.|
|Ergänzungen|Beta|Unterstützung für Castsegment im erweiterten Pfad hinzugefügt. Beispiel: https://graph.microsoft.com/v1.0/me/messages?$expand=microsoft.graph.eventMessage/event|

### <a name="onedrive"></a>OneDrive

|**Änderungstyp**|**Version**|**Beschreibung**|
|:--------------|:-----------|:--------------|
|Behebung|v1.0|Behebung eines Problems, aufgrund dessen bei createLink-Anforderungen OneDrive den 500-Fehler mit der Meldung „Nicht unterstützter Erweiterungseigenschaftentyp.“ zurückgab.|

## <a name="march-2016"></a>März 2016

### <a name="calendar"></a>Kalender

|**Änderungstyp**|**Version**|**Beschreibung**|
|:--------------|:-----------|:--------------|
|Ergänzungen|Beta|_singleValueExtendedProperties_ und _multiValueExtendedProperties_-Eigenschaften hinzugefügt.|
|Ergänzungen|Beta|_suggestionHint_-Eigenschaft zu _meetingTimeCandidate _ hinzugefügt.|
|Ergänzungen|Beta|_locationUri_-Eigenschaft zu _location_ hinzugefügt.|
|Ergänzungen|Beta|_type_ und _postOfficeBox_ zu _physicalAddress _ hinzugefügt.|
|Änderung|Beta|_findMeetingTimes_ verwendet jetzt den neuen _ReturnSuggestionHints_-Parameter.|
|Änderung|Beta|_findMeetingTimes_ gibt jetzt eine Sammlung von _meetingTimeCandidate_ zurück.|

### <a name="drive"></a>Laufwerk

|**Änderungstyp**|**Version**|**Beschreibung**|
|:--------------|:-----------|:--------------|
|Ergänzungen|v1.0 und Beta|_recent_-Funktion zum Auflisten eines Satzes von Elementen hinzugefügt, die zuletzt von dem angemeldeten Benutzer verwendet wurden. Diese Liste enthält Elemente, die sich in dem Laufwerk des Benutzers befinden sowie Elemente in anderen Laufwerken, auf die dieser Zugriff hat. Beispiel: GET /me/drive/recent.|
|Ergänzungen|v1.0 und Beta|_sharedWithMe_-Funktion zum Auflisten des Satzes von Elementen hinzugefügt, die für den aktuellen Benutzer freigegeben sind. Beispiel: GET /me/drive/sharedWithMe.|

### <a name="driveitem"></a>DriveItem

|**Änderungstyp**|**Version**|**Beschreibung**|
|:--------------|:-----------|:--------------|
|Ergänzungen|v1.0 und Beta|_remoteItem_-Typ zum Bereitstellen eines Links zu einem Element in einem anderen Laufwerk hinzugefügt.|
|Ergänzungen|v1.0 und Beta|_sharingInvitation_-Typ hinzugefügt, um Details zu verknüpften Einladungen zur Freigabe für diese Berechtigung bereitzustellen.|
|Ergänzungen|v1.0 und Beta|_delta_-Funktion zum Nachverfolgen von Änderungen an Elementen in einem Laufwerk hinzugefügt. Beispiel: GET /me/drive/items/{item-id}/delta|
|Ergänzungen|v1.0 und Beta|_copy_-Funktion zum Erstellen einer Kopie eines _driveItem_-Elements (einschließlich untergeordneter Elemente) unter einem neuen übergeordneten Element oder unter einem neuen Namen hinzugefügt. Beispiel: POST /me/drive/items/{item-id}/copy|
|Ergänzungen|v1.0 und Beta|_conflictBehavior_-Instanzattribute sind nun auf _driveItem_ anwendbar.|
|Ergänzungen|Beta|_invite_-Funktion zum Senden einer Einladung zur Freigabe für ein vorhandenes Element hinzugefügt. Mit einer Einladung zur Freigabe werden ein Freigabelink erstellt und eine E-Mail-Nachricht an den Empfänger die Einladung mit dem Freigabelink gesendet. Beispiel: POST /drive/items/{item-id}/invite

### <a name="event"></a>Ereignis

|**Änderungstyp**|**Version**|**Beschreibung**|
|:--------------|:-----------|:--------------|
|Ergänzungen|Beta|Neue _onlineMeetingUrl_-Eigenschaft und neue _cancel_-Methode hinzugefügt.|

### <a name="event-messages"></a>Ereignismeldungen

|**Änderungstyp**|**Version**|**Beschreibung**|
|:--------------|:-----------|:--------------|
|Ergänzungen|Beta|_startDateTime_, _endDateTime_, _location_, _type_, _recurrence_, _isOutOfDate_, _conversationIndex_, _unsubscribe_, _unsubscribeData_, _unsubscribeEnabled_ und _flag_-Eigenschaften zum _eventmessage_-Objekt hinzugefügt.|
|Ergänzungen|Beta|_singleValueExtendedProperties_ und _multiValueExtendedProperties_-Eigenschaften hinzugefügt.|
|Ergänzungen|Beta|Neue _unsubscribe_-Methode hinzugefügt.|

### <a name="excel"></a>Excel

|**Änderungstyp**|**Version**|**Beschreibung**|
|:--------------|:-----------|:--------------|
|Ergänzungen|Beta|Es wurden neue REST-APIs für Excel hinzugefügt, mit denen Sie Daten in einer Excel-Arbeitsmappe lesen und ändern können. Sie können nun intelligente Apps erstellen, mit denen Benutzer die in Excel-Arbeitsmappen gespeicherten Inhalte nutzen können, indem Einblicke in die Daten bereitgestellt werden. Profitieren Sie von den Vorteilen der Analysefunktionen von Excel, erstellen Sie Tabellen und Diagramme und extrahieren Sie optisch ansprechende Diagramme, und das alles von Ihrer App aus. Weitere Informationen finden Sie unter [Arbeiten mit Excel in Microsoft Graph](http://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/excel).|

### <a name="general"></a>Allgemein

|**Änderungstyp**|**Version**|**Beschreibung**|
|:--------------|:-----------|:--------------|
|Ergänzungen|v1.0 und Beta|Verbesserung von Fehlermeldungen beim Auflösen von Mandantenalias- und abgelehnten JWT-Token (AAD).|
|Ergänzungen|v1.0 und Beta|Der Ort für den Autorisierungsdienstendpunkt wird jetzt in dem _www-authenticate_-Header zurückgegeben, wenn eine Anforderung mit einem leeren Bearertoken empfangen wird.|
|Ergänzungen|v1.0 und Beta|Die Funktion zum Filtern nach ID-Eigenschaft einer Entität wurde repariert. Beispiel: GET https://graph.microsoft.com/v1.0/users?$filter=id+eq+'x'<br/>Bisher musste bei allen POST-Anforderungen für Dienstaktionen und Funktionen der Aktion oder dem Funktionsnamen ein Präfix mithilfe von microsoft.graph vorangestellt werden. Beispiel: POST https://graph.microsoft.com/v1.0/me/Microsoft.Graph.getMemberGroups<br/>Das Präfix ist nun nicht mehr erforderlich (obwohl es immer noch angegeben werden kann). Folgendes würde jetzt daher funktionieren: POST https://graph.microsoft.com/v1.0/me/getMemberGroups|
|Ändern|Beta|Abonnement-Eigenschaftennamen bereinigt.|
|Ergänzungen|Beta|Wir haben die Möglichkeit zum Ermitteln von (über _directorySettingTemplates_) und Außerkraftsetzen des Standardverhaltens (durch Erstellen einer _Einstellung_ aus der Vorlage) für Entitäten und die zugehörigen Funktionen hinzugefügt. Anfangs konnten die Verhaltensweisen für Office-Gruppen nur über die Vorlage gesteuert werden.|

### <a name="mail-folder"></a>Mail-Ordner

|**Änderungstyp**|**Version**|**Beschreibung**|
|:--------------|:-----------|:--------------|
|Ergänzungen|Beta|_wellKnownName_- und _userConfigurations_-Eigenschaften hinzugefügt.|
|Ergänzungen|Beta|_singleValueExtendedProperties_- und _multiValueExtendedProperties_-Eigenschaften hinzugefügt|

### <a name="messages"></a>Nachrichten

|**Änderungstyp**|**Version**|**Beschreibung**|
|:--------------|:-----------|:--------------|
|Ergänzungen|v1.0|_mobilePhone_-Eigenschaft hinzugefügt.|
|Ergänzungen|v1.0 und Beta|_internetMessageId_-Eigenschaft hinzugefügt. Die Nachrichten-ID im von [RFC2822](http://www.ietf.org/rfc/rfc2822.txt) angegebenen Format.|
|Ändern|Beta|_mobilePhone1_-Eigenschaft in _mobilePhone_ umgenannt.|
|Änderung|Beta|_createReply_ und _createReplyAll _ verwenden neue _Message_- und _comment_-Parameter.|
|Änderung|Beta|_createForward_ verwendet neue _Message_-, _ToRecipients_- und _comment_-Parameter.|
|Änderung|Beta|_reply_, _replyAll_ und _forward_ verwenden neue _Message_-Parameter.|

### <a name="permission"></a>Berechtigung

|**Änderungstyp**|**Version**|**Beschreibung**|
|:--------------|:-----------|:--------------|
|Ergänzungen|v1.0 und Beta|_sharingInvitation_-Eigenschaft hinzugefügt, um Details zu verknüpften Einladungen zur Freigabe für diese Berechtigung bereitzustellen.|

### <a name="person"></a>Person

|**Änderungstyp**|**Version**|**Beschreibung**|
|:--------------|:-----------|:--------------|
|Ergänzungen|Beta|- Neue _birthday_-, _personNotes_-, _isFavorite_-, _phones_-, _permission_-, _postalAddresses_-,_websites_-,_yomiCompany_-, _department_-, _profession_-, _mailboxType_- und _personType_-Eigenschaften hinzugefügt.|
|Ergänzungen|Beta|Neue Enumerationstypen hinzugefügt: _physicalAddressType_, _webSite_, _phone_ und _webSiteType_.|

### <a name="reference-attachment"></a>Verweisanlage

|**Änderungstyp**|**Version**|**Beschreibung**|
|:--------------|:-----------|:--------------|
|Ergänzungen|Beta|Neue Eigenschaften hinzugefügt: _sourceUrl_, _providerType_, _thumbnailUrl_, _previewUrl_, _permission_ und _isFolder_.|
|Ergänzungen|Beta|_singleValueExtendedProperties_ und _multiValueExtendedProperties_-Eigenschaften hinzugefügt.|
|Ergänzungen|Beta|Neue Enumerationstypen _referenceAttachmentProvider_ und _referenceAttachmentPermission_. hinzugefügt.|

### <a name="subscriptions"></a>Abonnements

|**Änderungstyp**|**Endpunkt**|**Beschreibung**|
|:--------------|:-----------|:--------------|
|Ergänzungen|v1.0|Webhooks sind jetzt allgemein für Version 1.0 von Endpunkt über die _/Subscriptions_-Ressource verfügbar. Erstellen, Lesen, Aktualisieren und Löschen Sie Abonnements, um Benachrichtigungen zu Daten aus Outlook und Office 365-Gruppenunterhaltungen zu erhalten.|

### <a name="user"></a>Benutzer

|**Änderungstyp**|**Version**|**Beschreibung**|
|:--------------|:-----------|:--------------|
|Ergänzungen|Beta|_mailboxSettings_-Eigenschaft sowie die entsprechenden Typen hinzugefügt.|

## <a name="february-2016"></a>Februar 2016

### <a name="driveitem"></a>DriveItem

|**Änderungstyp**|**Version**|**Beschreibung**|
|:--------------|:-----------|:--------------|
|Ergänzungen|v1.0 und Beta|Neue _remoteItem_-Eigenschaft für driveItem für Microsoft-Konten.|

### <a name="general"></a>Allgemein

|**Änderungstyp**|**Version**|**Beschreibung**|
|:--------------|:-----------|:--------------|
|Änderung|v1.0 und Beta|-_/me/drive_ funktioniert nun für Microsoft-Konten und Geschäfts-, Schul- und Uni-Konten.|
|Änderung|v1.0 und Beta|Laufwerkanforderungen für Konten, deren OneDrive-Speicher bei Bedarf bereitgestellt wurde, funktionieren zuverlässig und können in mehr Szenarien verwendet werden, in denen die SharePoint-Standardwebsites des Mandanten nicht standardmäßige Namen verwenden.|
|Löschung|Beta|Verschiedene nicht implementierte Typen aus dem Betaschema zur Anpassung an 1.0 Schema entfernt.|

### <a name="subscriptions"></a>Abonnements

|**Änderungstyp**|**Version**|**Beschreibung**|
|:--------------|:-----------|:--------------|
|Ergänzungen|Beta|notificationUrl-Validierung bei Abonnement-Erstellung. Weitere Informationen finden Sie unter [Microsoft Graph WebHooks Update - January 2016](http://dev.office.com/blogs/Microsoft-Graph-WebHooks-Update-January-2016).|
|Ergänzungen|Beta|Abonnemententitäten können jetzt gelöscht werden: LÖSCHEN https://graph.microsoft.com/beta/subscriptions/|

### <a name="users"></a>Benutzer

|**Änderungstyp**|**Version**|**Beschreibung**|
|:--------------|:-----------|:--------------|
|Änderung|v1.0 und Beta|_displayName_ wird jetzt für Microsoft-Konten zurückgegeben.|

## <a name="january-2016"></a>Januar 2016

### <a name="contacts"></a>Kontakte

|**Änderungstyp**|**Version**|**Beschreibung**|
|:--------------|:-----------|:--------------|
|Ergänzungen|v1.0|mobilePhone-Eigenschaft zum Entitätssatz für persönliche Kontakte hinzugefügt.|

### <a name="directoryobjects"></a>directoryObjects

|**Änderungstyp**|**Version**|**Beschreibung**|
|:--------------|:-----------|:--------------|
|Behebung|v1.0 und Beta|Behebung eines Problems mit Aufrufaktionen, die mit directoryObjects verknüpft sind und zu dem folgenden Fehler führten:  „Der Rückgabetyp des Vorgangs ist mit dem vorgegebenen Entitätssatz nicht möglich“. Dies gilt für die folgenden Aktionen: _microsoft.graph.checkMemberObjects_, _microsoft.graph.getMemberObjects_, _microsoft.graph.checkMemberGroups_, _microsoft.graph.assignLicense_, _microsoft.graph.changePassword_.|

## <a name="december-2015"></a>Dezember 2015

### <a name="contacts"></a>Kontakte

|**Änderungstyp**|**Version**|**Beschreibung**|
|:--------------|:-----------|:--------------|
|Ergänzungen|Beta|mobilePhone-Eigenschaft zum Entitätssatz für persönliche Kontakte hinzugefügt.|

### <a name="general"></a>Allgemein

|**Änderungstyp**|**Version**|**Beschreibung**|
|:--------------|:-----------|:--------------|
|Behebung|v1.0 und Beta|Behebung eines Problems mit Anforderungen mit $filter-Ausdrücken, die mehrmals die gleiche Eigenschaft angegebenen haben, was zu dem folgenden 500-Fehler führte: Ein Element mit diesem Schlüssel wurde bereits hinzugefügt.|
|Behebung|v1.0 und Beta|Behebung eines Problems mit der Groß-/Kleinschreibung für Aktionsparameternamen und -werte.|
|Behebung|v1.0 und Beta|Behebung eines Problems mit der Verarbeitung von Anforderungen für Nutzlasten mit Nullwerten für einige eingebettete komplexe Eigenschaften, aufgrund dessen ein Fehler mit einer Nullverweisausnahme auftrat.|
|Ergänzungen|v1.0 und Beta|Unterstützung für das Sortieren und Filtern von komplexen Type-Eigenschaften.|
|Ergänzungen|v1.0 und Beta|authorization_uri-Eigenschaft in dem www-authenticate-Header einer 401-Antwort hinzugefügt. Dieser URI kann verwendet werden, um den Tokenerwerbfluss zu starten.|
|Ergänzungen|v1.0 und Beta|Verbesserte Fehlermeldungen für Benutzer und Gruppen.|

### <a name="groups"></a>Gruppen

|**Änderungstyp**|**Version**|**Beschreibung**|
|:--------------|:-----------|:--------------|
|Behebung|v1.0 und Beta|Behebung eines Problems mit dem Aufruf folgender Gruppenaktionen: _microsoft.graph.addFavorite_, _microsoft.graph.removeFavorite_ and _microsoft.graph.resetUnseenCount_.|

### <a name="messages"></a>Nachrichten

|**Änderungstyp**|**Version**|**Beschreibung**|
|:--------------|:-----------|:--------------|
|Ergänzungen|Beta|eventMessageRequest-Untertyp der eventMessage- und startDateTime-, endDateTime-, location-, type-, recurrence- und IsOutOfDate-Eigenschaften zum eventMessag-Typ hinzugefügt.|

### <a name="users"></a>Benutzer

|**Änderungstyp**|**Version**|**Beschreibung**|
|:--------------|:-----------|:--------------|
|Behebung|v1.0 und Beta|Behebung eines Problems, aufgrund dessen bestimmte Benutzereigenschaften von anderen Benutzern nicht ausgewählt werden konnten, wenn auf den Benutzer mithilfe des Benutzerprinzipalnamens (UPN) verwiesen wurde. Beispiel: https://graph.microsoft.com/v1.0/users/anotherUser@contoso.com?$select=aboutMe|
|Behebung|v1.0 und Beta|Behebung eines Problems mit dem Aufruf der benutzergebundenen _microsoft.graph.reminderView_-Funktion, aufgrund dessen der folgende Fehler auftrat: „Eine Eigenschaft mit dem Namen 'businessPhones' vom Typ 'Microsoft.OutlookServices.Reminder' konnte nicht gefunden werden.“|
|Behebung|v1.0 und Beta|Behebung eines Problems mit der Erstellung und Aktualisierung von Benutzern (POST/PATCH /v1.0/users), aufgrund dessen der 400-Fehler auftrat.|
