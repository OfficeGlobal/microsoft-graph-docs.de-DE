---
title: Auflisten von „windows10GeneralConfiguration“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs windows10GeneralConfiguration auf.
ms.openlocfilehash: 01e7aa2744574e8e3ca97c66746ea53e9a30888c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058835"
---
# <a name="list-windows10generalconfigurations"></a><span data-ttu-id="3fdf9-103">Auflisten von „windows10GeneralConfiguration“</span><span class="sxs-lookup"><span data-stu-id="3fdf9-103">List windows10GeneralConfigurations</span></span>

> <span data-ttu-id="3fdf9-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="3fdf9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3fdf9-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3fdf9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3fdf9-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="3fdf9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3fdf9-107">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) auf.</span><span class="sxs-lookup"><span data-stu-id="3fdf9-107">List properties and relationships of the [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3fdf9-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="3fdf9-108">Prerequisites</span></span>
<span data-ttu-id="3fdf9-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3fdf9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3fdf9-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3fdf9-111">Permission type</span></span>|<span data-ttu-id="3fdf9-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3fdf9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3fdf9-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3fdf9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3fdf9-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="3fdf9-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="3fdf9-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3fdf9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3fdf9-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3fdf9-116">Not supported.</span></span>|
|<span data-ttu-id="3fdf9-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3fdf9-117">Application</span></span>|<span data-ttu-id="3fdf9-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3fdf9-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3fdf9-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3fdf9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="3fdf9-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3fdf9-120">Request headers</span></span>
|<span data-ttu-id="3fdf9-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="3fdf9-121">Header</span></span>|<span data-ttu-id="3fdf9-122">Wert</span><span class="sxs-lookup"><span data-stu-id="3fdf9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3fdf9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3fdf9-123">Authorization</span></span>|<span data-ttu-id="3fdf9-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="3fdf9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3fdf9-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3fdf9-125">Accept</span></span>|<span data-ttu-id="3fdf9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3fdf9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3fdf9-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3fdf9-127">Request body</span></span>
<span data-ttu-id="3fdf9-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="3fdf9-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3fdf9-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="3fdf9-129">Response</span></span>
<span data-ttu-id="3fdf9-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="3fdf9-130">If successful, this method returns a `200 OK` response code and a collection of [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3fdf9-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3fdf9-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="3fdf9-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3fdf9-132">Request</span></span>
<span data-ttu-id="3fdf9-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3fdf9-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="3fdf9-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="3fdf9-134">Response</span></span>
<span data-ttu-id="3fdf9-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3fdf9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 13491

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windows10GeneralConfiguration",
      "id": "a4235d71-5d71-a423-715d-23a4715d23a4",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "supportsScopeTags": true,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "windows10AppsForceUpdateSchedule": {
        "@odata.type": "microsoft.graph.windows10AppsForceUpdateSchedule",
        "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
        "recurrence": "daily",
        "runImmediatelyIfAfterStartDateTime": true
      },
      "enableAutomaticRedeployment": true,
      "assignedAccessSingleModeUserName": "Assigned Access Single Mode User Name value",
      "assignedAccessSingleModeAppUserModelId": "Assigned Access Single Mode App User Model Id value",
      "microsoftAccountSignInAssistantSettings": "disabled",
      "authenticationAllowSecondaryDevice": true,
      "authenticationAllowFIDODevice": true,
      "cryptographyAllowFipsAlgorithmPolicy": true,
      "displayAppListWithGdiDPIScalingTurnedOn": [
        "Display App List With Gdi DPIScaling Turned On value"
      ],
      "displayAppListWithGdiDPIScalingTurnedOff": [
        "Display App List With Gdi DPIScaling Turned Off value"
      ],
      "enterpriseCloudPrintDiscoveryEndPoint": "Enterprise Cloud Print Discovery End Point value",
      "enterpriseCloudPrintOAuthAuthority": "Enterprise Cloud Print OAuth Authority value",
      "enterpriseCloudPrintOAuthClientIdentifier": "Enterprise Cloud Print OAuth Client Identifier value",
      "enterpriseCloudPrintResourceIdentifier": "Enterprise Cloud Print Resource Identifier value",
      "enterpriseCloudPrintDiscoveryMaxLimit": 5,
      "enterpriseCloudPrintMopriaDiscoveryResourceIdentifier": "Enterprise Cloud Print Mopria Discovery Resource Identifier value",
      "messagingBlockSync": true,
      "messagingBlockMMS": true,
      "messagingBlockRichCommunicationServices": true,
      "printerNames": [
        "Printer Names value"
      ],
      "printerDefaultName": "Printer Default Name value",
      "printerBlockAddition": true,
      "searchBlockDiacritics": true,
      "searchDisableAutoLanguageDetection": true,
      "searchDisableIndexingEncryptedItems": true,
      "searchEnableRemoteQueries": true,
      "searchDisableUseLocation": true,
      "searchDisableLocation": true,
      "searchDisableIndexerBackoff": true,
      "searchDisableIndexingRemovableDrive": true,
      "searchEnableAutomaticIndexSizeManangement": true,
      "searchBlockWebResults": true,
      "securityBlockAzureADJoinedDevicesAutoEncryption": true,
      "diagnosticsDataSubmissionMode": "none",
      "oneDriveDisableFileSync": true,
      "systemTelemetryProxyServer": "System Telemetry Proxy Server value",
      "inkWorkspaceAccess": "enabled",
      "inkWorkspaceAccessState": "blocked",
      "inkWorkspaceBlockSuggestedApps": true,
      "smartScreenEnableAppInstallControl": true,
      "personalizationDesktopImageUrl": "https://example.com/personalizationDesktopImageUrl/",
      "personalizationLockScreenImageUrl": "https://example.com/personalizationLockScreenImageUrl/",
      "bluetoothAllowedServices": [
        "Bluetooth Allowed Services value"
      ],
      "bluetoothBlockAdvertising": true,
      "bluetoothBlockDiscoverableMode": true,
      "bluetoothBlockPrePairing": true,
      "edgeBlockAutofill": true,
      "edgeBlocked": true,
      "edgeCookiePolicy": "allow",
      "edgeBlockDeveloperTools": true,
      "edgeBlockSendingDoNotTrackHeader": true,
      "edgeBlockExtensions": true,
      "edgeBlockInPrivateBrowsing": true,
      "edgeBlockJavaScript": true,
      "edgeBlockPasswordManager": true,
      "edgeBlockAddressBarDropdown": true,
      "edgeBlockCompatibilityList": true,
      "edgeClearBrowsingDataOnExit": true,
      "edgeAllowStartPagesModification": true,
      "edgeDisableFirstRunPage": true,
      "edgeBlockLiveTileDataCollection": true,
      "edgeSyncFavoritesWithInternetExplorer": true,
      "edgeFavoritesListLocation": "Edge Favorites List Location value",
      "edgeBlockEditFavorites": true,
      "cellularBlockDataWhenRoaming": true,
      "cellularBlockVpn": true,
      "cellularBlockVpnWhenRoaming": true,
      "cellularData": "required",
      "defenderBlockEndUserAccess": true,
      "defenderDaysBeforeDeletingQuarantinedMalware": 12,
      "defenderDetectedMalwareActions": {
        "@odata.type": "microsoft.graph.defenderDetectedMalwareActions",
        "lowSeverity": "clean",
        "moderateSeverity": "clean",
        "highSeverity": "clean",
        "severeSeverity": "clean"
      },
      "defenderSystemScanSchedule": "everyday",
      "defenderFilesAndFoldersToExclude": [
        "Defender Files And Folders To Exclude value"
      ],
      "defenderFileExtensionsToExclude": [
        "Defender File Extensions To Exclude value"
      ],
      "defenderScanMaxCpu": 2,
      "defenderMonitorFileActivity": "disable",
      "defenderPotentiallyUnwantedAppAction": "block",
      "defenderPotentiallyUnwantedAppActionSetting": "enable",
      "defenderProcessesToExclude": [
        "Defender Processes To Exclude value"
      ],
      "defenderPromptForSampleSubmission": "alwaysPrompt",
      "defenderRequireBehaviorMonitoring": true,
      "defenderRequireCloudProtection": true,
      "defenderRequireNetworkInspectionSystem": true,
      "defenderRequireRealTimeMonitoring": true,
      "defenderScanArchiveFiles": true,
      "defenderScanDownloads": true,
      "defenderScanNetworkFiles": true,
      "defenderScanIncomingMail": true,
      "defenderScanMappedNetworkDrivesDuringFullScan": true,
      "defenderScanRemovableDrivesDuringFullScan": true,
      "defenderScanScriptsLoadedInInternetExplorer": true,
      "defenderSignatureUpdateIntervalInHours": 6,
      "defenderScanType": "disabled",
      "defenderScheduledScanTime": "11:59:10.9990000",
      "defenderScheduledQuickScanTime": "11:58:49.3840000",
      "defenderCloudBlockLevel": "high",
      "defenderCloudExtendedTimeout": 12,
      "defenderCloudExtendedTimeoutInSeconds": 5,
      "defenderBlockOnAccessProtection": true,
      "defenderScheduleScanDay": "monday",
      "defenderSubmitSamplesConsentType": "alwaysPrompt",
      "lockScreenAllowTimeoutConfiguration": true,
      "lockScreenBlockActionCenterNotifications": true,
      "lockScreenBlockCortana": true,
      "lockScreenBlockToastNotifications": true,
      "lockScreenTimeoutInSeconds": 10,
      "passwordBlockSimple": true,
      "passwordExpirationDays": 6,
      "passwordMinimumLength": 5,
      "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
      "passwordMinimumCharacterSetCount": 0,
      "passwordPreviousPasswordBlockCount": 2,
      "passwordRequired": true,
      "passwordRequireWhenResumeFromIdleState": true,
      "passwordRequiredType": "alphanumeric",
      "passwordSignInFailureCountBeforeFactoryReset": 12,
      "passwordMinimumAgeInDays": 8,
      "privacyAdvertisingId": "blocked",
      "privacyAutoAcceptPairingAndConsentPrompts": true,
      "privacyBlockInputPersonalization": true,
      "privacyBlockPublishUserActivities": true,
      "privacyBlockActivityFeed": true,
      "startBlockUnpinningAppsFromTaskbar": true,
      "startMenuAppListVisibility": "collapse",
      "startMenuHideChangeAccountSettings": true,
      "startMenuHideFrequentlyUsedApps": true,
      "startMenuHideHibernate": true,
      "startMenuHideLock": true,
      "startMenuHidePowerButton": true,
      "startMenuHideRecentJumpLists": true,
      "startMenuHideRecentlyAddedApps": true,
      "startMenuHideRestartOptions": true,
      "startMenuHideShutDown": true,
      "startMenuHideSignOut": true,
      "startMenuHideSleep": true,
      "startMenuHideSwitchAccount": true,
      "startMenuHideUserTile": true,
      "startMenuLayoutEdgeAssetsXml": "c3RhcnRNZW51TGF5b3V0RWRnZUFzc2V0c1htbA==",
      "startMenuLayoutXml": "c3RhcnRNZW51TGF5b3V0WG1s",
      "startMenuMode": "fullScreen",
      "startMenuPinnedFolderDocuments": "hide",
      "startMenuPinnedFolderDownloads": "hide",
      "startMenuPinnedFolderFileExplorer": "hide",
      "startMenuPinnedFolderHomeGroup": "hide",
      "startMenuPinnedFolderMusic": "hide",
      "startMenuPinnedFolderNetwork": "hide",
      "startMenuPinnedFolderPersonalFolder": "hide",
      "startMenuPinnedFolderPictures": "hide",
      "startMenuPinnedFolderSettings": "hide",
      "startMenuPinnedFolderVideos": "hide",
      "settingsBlockSettingsApp": true,
      "settingsBlockSystemPage": true,
      "settingsBlockDevicesPage": true,
      "settingsBlockNetworkInternetPage": true,
      "settingsBlockPersonalizationPage": true,
      "settingsBlockAccountsPage": true,
      "settingsBlockTimeLanguagePage": true,
      "settingsBlockEaseOfAccessPage": true,
      "settingsBlockPrivacyPage": true,
      "settingsBlockUpdateSecurityPage": true,
      "settingsBlockAppsPage": true,
      "settingsBlockGamingPage": true,
      "windowsSpotlightBlockConsumerSpecificFeatures": true,
      "windowsSpotlightBlocked": true,
      "windowsSpotlightBlockOnActionCenter": true,
      "windowsSpotlightBlockTailoredExperiences": true,
      "windowsSpotlightBlockThirdPartyNotifications": true,
      "windowsSpotlightBlockWelcomeExperience": true,
      "windowsSpotlightBlockWindowsTips": true,
      "windowsSpotlightConfigureOnLockScreen": "disabled",
      "networkProxyApplySettingsDeviceWide": true,
      "networkProxyDisableAutoDetect": true,
      "networkProxyAutomaticConfigurationUrl": "https://example.com/networkProxyAutomaticConfigurationUrl/",
      "networkProxyServer": {
        "@odata.type": "microsoft.graph.windows10NetworkProxyServer",
        "address": "Address value",
        "exceptions": [
          "Exceptions value"
        ],
        "useForLocalAddresses": true
      },
      "accountsBlockAddingNonMicrosoftAccountEmail": true,
      "antiTheftModeBlocked": true,
      "bluetoothBlocked": true,
      "cameraBlocked": true,
      "connectedDevicesServiceBlocked": true,
      "certificatesBlockManualRootCertificateInstallation": true,
      "copyPasteBlocked": true,
      "cortanaBlocked": true,
      "deviceManagementBlockFactoryResetOnMobile": true,
      "deviceManagementBlockManualUnenroll": true,
      "safeSearchFilter": "strict",
      "edgeBlockPopups": true,
      "edgeBlockSearchSuggestions": true,
      "edgeBlockSendingIntranetTrafficToInternetExplorer": true,
      "edgeRequireSmartScreen": true,
      "edgeEnterpriseModeSiteListLocation": "Edge Enterprise Mode Site List Location value",
      "edgeFirstRunUrl": "https://example.com/edgeFirstRunUrl/",
      "edgeSearchEngine": {
        "@odata.type": "microsoft.graph.edgeSearchEngineBase"
      },
      "edgeHomepageUrls": [
        "Edge Homepage Urls value"
      ],
      "edgeBlockAccessToAboutFlags": true,
      "smartScreenBlockPromptOverride": true,
      "smartScreenBlockPromptOverrideForFiles": true,
      "webRtcBlockLocalhostIpAddress": true,
      "internetSharingBlocked": true,
      "settingsBlockAddProvisioningPackage": true,
      "settingsBlockRemoveProvisioningPackage": true,
      "settingsBlockChangeSystemTime": true,
      "settingsBlockEditDeviceName": true,
      "settingsBlockChangeRegion": true,
      "settingsBlockChangeLanguage": true,
      "settingsBlockChangePowerSleep": true,
      "locationServicesBlocked": true,
      "microsoftAccountBlocked": true,
      "microsoftAccountBlockSettingsSync": true,
      "nfcBlocked": true,
      "resetProtectionModeBlocked": true,
      "screenCaptureBlocked": true,
      "storageBlockRemovableStorage": true,
      "storageRequireMobileDeviceEncryption": true,
      "usbBlocked": true,
      "voiceRecordingBlocked": true,
      "wiFiBlockAutomaticConnectHotspots": true,
      "wiFiBlocked": true,
      "wiFiBlockManualConfiguration": true,
      "wiFiScanInterval": 0,
      "wirelessDisplayBlockProjectionToThisDevice": true,
      "wirelessDisplayBlockUserInputFromReceiver": true,
      "wirelessDisplayRequirePinForPairing": true,
      "windowsStoreBlocked": true,
      "appsAllowTrustedAppsSideloading": "blocked",
      "windowsStoreBlockAutoUpdate": true,
      "developerUnlockSetting": "blocked",
      "sharedUserAppDataAllowed": true,
      "appsBlockWindowsStoreOriginatedApps": true,
      "windowsStoreEnablePrivateStoreOnly": true,
      "storageRestrictAppDataToSystemVolume": true,
      "storageRestrictAppInstallToSystemVolume": true,
      "gameDvrBlocked": true,
      "experienceBlockDeviceDiscovery": true,
      "experienceBlockErrorDialogWhenNoSIM": true,
      "experienceBlockTaskSwitcher": true,
      "logonBlockFastUserSwitching": true,
      "tenantLockdownRequireNetworkDuringOutOfBoxExperience": true,
      "appManagementMSIAllowUserControlOverInstall": true,
      "appManagementMSIAlwaysInstallWithElevatedPrivileges": true,
      "dataProtectionBlockDirectMemoryAccess": true
    }
  ]
}
```




