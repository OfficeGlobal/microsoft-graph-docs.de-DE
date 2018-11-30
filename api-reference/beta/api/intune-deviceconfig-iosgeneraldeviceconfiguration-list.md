---
title: Auflisten von „iosGeneralDeviceConfiguration“
description: Listet die Eigenschaften und Beziehungen der macOSGeneralDeviceConfiguration-Objekte auf.
ms.openlocfilehash: c7ccd1c93c2ec163f984a13239c8bd93ed91e6eb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060780"
---
# <a name="list-iosgeneraldeviceconfigurations"></a><span data-ttu-id="c18f3-103">Auflisten von „iosGeneralDeviceConfiguration“</span><span class="sxs-lookup"><span data-stu-id="c18f3-103">List iosGeneralDeviceConfigurations</span></span>

> <span data-ttu-id="c18f3-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="c18f3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c18f3-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c18f3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c18f3-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="c18f3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c18f3-107">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) auf.</span><span class="sxs-lookup"><span data-stu-id="c18f3-107">List properties and relationships of the [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c18f3-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c18f3-108">Prerequisites</span></span>
<span data-ttu-id="c18f3-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c18f3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c18f3-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c18f3-111">Permission type</span></span>|<span data-ttu-id="c18f3-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c18f3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c18f3-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c18f3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c18f3-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c18f3-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="c18f3-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c18f3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c18f3-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c18f3-116">Not supported.</span></span>|
|<span data-ttu-id="c18f3-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c18f3-117">Application</span></span>|<span data-ttu-id="c18f3-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c18f3-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c18f3-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c18f3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="c18f3-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c18f3-120">Request headers</span></span>
|<span data-ttu-id="c18f3-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="c18f3-121">Header</span></span>|<span data-ttu-id="c18f3-122">Wert</span><span class="sxs-lookup"><span data-stu-id="c18f3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c18f3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c18f3-123">Authorization</span></span>|<span data-ttu-id="c18f3-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c18f3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c18f3-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c18f3-125">Accept</span></span>|<span data-ttu-id="c18f3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c18f3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c18f3-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c18f3-127">Request body</span></span>
<span data-ttu-id="c18f3-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="c18f3-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c18f3-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="c18f3-129">Response</span></span>
<span data-ttu-id="c18f3-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="c18f3-130">If successful, this method returns a `200 OK` response code and a collection of [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c18f3-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c18f3-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="c18f3-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c18f3-132">Request</span></span>
<span data-ttu-id="c18f3-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c18f3-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="c18f3-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="c18f3-134">Response</span></span>
<span data-ttu-id="c18f3-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c18f3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 9581

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosGeneralDeviceConfiguration",
      "id": "ebba5202-5202-ebba-0252-baeb0252baeb",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "supportsScopeTags": true,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "accountBlockModification": true,
      "activationLockAllowWhenSupervised": true,
      "airDropBlocked": true,
      "airDropForceUnmanagedDropTarget": true,
      "airPlayForcePairingPasswordForOutgoingRequests": true,
      "appleWatchBlockPairing": true,
      "appleWatchForceWristDetection": true,
      "appleNewsBlocked": true,
      "appsSingleAppModeList": [
        {
          "@odata.type": "microsoft.graph.appListItem",
          "name": "Name value",
          "publisher": "Publisher value",
          "appStoreUrl": "https://example.com/appStoreUrl/",
          "appId": "App Id value"
        }
      ],
      "appsVisibilityList": [
        {
          "@odata.type": "microsoft.graph.appListItem",
          "name": "Name value",
          "publisher": "Publisher value",
          "appStoreUrl": "https://example.com/appStoreUrl/",
          "appId": "App Id value"
        }
      ],
      "appsVisibilityListType": "appsInListCompliant",
      "appStoreBlockAutomaticDownloads": true,
      "appStoreBlocked": true,
      "appStoreBlockInAppPurchases": true,
      "appStoreBlockUIAppInstallation": true,
      "appStoreRequirePassword": true,
      "bluetoothBlockModification": true,
      "cameraBlocked": true,
      "cellularBlockDataRoaming": true,
      "cellularBlockGlobalBackgroundFetchWhileRoaming": true,
      "cellularBlockPerAppDataModification": true,
      "cellularBlockPersonalHotspot": true,
      "cellularBlockVoiceRoaming": true,
      "certificatesBlockUntrustedTlsCertificates": true,
      "classroomAppBlockRemoteScreenObservation": true,
      "classroomAppForceUnpromptedScreenObservation": true,
      "compliantAppsList": [
        {
          "@odata.type": "microsoft.graph.appListItem",
          "name": "Name value",
          "publisher": "Publisher value",
          "appStoreUrl": "https://example.com/appStoreUrl/",
          "appId": "App Id value"
        }
      ],
      "compliantAppListType": "appsInListCompliant",
      "configurationProfileBlockChanges": true,
      "definitionLookupBlocked": true,
      "deviceBlockEnableRestrictions": true,
      "deviceBlockEraseContentAndSettings": true,
      "deviceBlockNameModification": true,
      "diagnosticDataBlockSubmission": true,
      "diagnosticDataBlockSubmissionModification": true,
      "documentsBlockManagedDocumentsInUnmanagedApps": true,
      "documentsBlockUnmanagedDocumentsInManagedApps": true,
      "emailInDomainSuffixes": [
        "Email In Domain Suffixes value"
      ],
      "enterpriseAppBlockTrust": true,
      "enterpriseAppBlockTrustModification": true,
      "faceTimeBlocked": true,
      "findMyFriendsBlocked": true,
      "gamingBlockGameCenterFriends": true,
      "gamingBlockMultiplayer": true,
      "gameCenterBlocked": true,
      "hostPairingBlocked": true,
      "iBooksStoreBlocked": true,
      "iBooksStoreBlockErotica": true,
      "iCloudBlockActivityContinuation": true,
      "iCloudBlockBackup": true,
      "iCloudBlockDocumentSync": true,
      "iCloudBlockManagedAppsSync": true,
      "iCloudBlockPhotoLibrary": true,
      "iCloudBlockPhotoStreamSync": true,
      "iCloudBlockSharedPhotoStream": true,
      "iCloudRequireEncryptedBackup": true,
      "iTunesBlockExplicitContent": true,
      "iTunesBlockMusicService": true,
      "iTunesBlockRadio": true,
      "keyboardBlockAutoCorrect": true,
      "keyboardBlockDictation": true,
      "keyboardBlockPredictive": true,
      "keyboardBlockShortcuts": true,
      "keyboardBlockSpellCheck": true,
      "kioskModeAllowAssistiveSpeak": true,
      "kioskModeAllowAssistiveTouchSettings": true,
      "kioskModeAllowAutoLock": true,
      "kioskModeAllowColorInversionSettings": true,
      "kioskModeAllowRingerSwitch": true,
      "kioskModeAllowScreenRotation": true,
      "kioskModeAllowSleepButton": true,
      "kioskModeAllowTouchscreen": true,
      "kioskModeAllowVoiceOverSettings": true,
      "kioskModeAllowVolumeButtons": true,
      "kioskModeBlockVolumeButtons": true,
      "kioskModeAllowZoomSettings": true,
      "kioskModeAppStoreUrl": "https://example.com/kioskModeAppStoreUrl/",
      "kioskModeBuiltInAppId": "Kiosk Mode Built In App Id value",
      "kioskModeRequireAssistiveTouch": true,
      "kioskModeRequireColorInversion": true,
      "kioskModeRequireMonoAudio": true,
      "kioskModeRequireVoiceOver": true,
      "kioskModeRequireZoom": true,
      "kioskModeManagedAppId": "Kiosk Mode Managed App Id value",
      "lockScreenBlockControlCenter": true,
      "lockScreenBlockNotificationView": true,
      "lockScreenBlockPassbook": true,
      "lockScreenBlockTodayView": true,
      "mediaContentRatingAustralia": {
        "@odata.type": "microsoft.graph.mediaContentRatingAustralia",
        "movieRating": "allBlocked",
        "tvRating": "allBlocked"
      },
      "mediaContentRatingCanada": {
        "@odata.type": "microsoft.graph.mediaContentRatingCanada",
        "movieRating": "allBlocked",
        "tvRating": "allBlocked"
      },
      "mediaContentRatingFrance": {
        "@odata.type": "microsoft.graph.mediaContentRatingFrance",
        "movieRating": "allBlocked",
        "tvRating": "allBlocked"
      },
      "mediaContentRatingGermany": {
        "@odata.type": "microsoft.graph.mediaContentRatingGermany",
        "movieRating": "allBlocked",
        "tvRating": "allBlocked"
      },
      "mediaContentRatingIreland": {
        "@odata.type": "microsoft.graph.mediaContentRatingIreland",
        "movieRating": "allBlocked",
        "tvRating": "allBlocked"
      },
      "mediaContentRatingJapan": {
        "@odata.type": "microsoft.graph.mediaContentRatingJapan",
        "movieRating": "allBlocked",
        "tvRating": "allBlocked"
      },
      "mediaContentRatingNewZealand": {
        "@odata.type": "microsoft.graph.mediaContentRatingNewZealand",
        "movieRating": "allBlocked",
        "tvRating": "allBlocked"
      },
      "mediaContentRatingUnitedKingdom": {
        "@odata.type": "microsoft.graph.mediaContentRatingUnitedKingdom",
        "movieRating": "allBlocked",
        "tvRating": "allBlocked"
      },
      "mediaContentRatingUnitedStates": {
        "@odata.type": "microsoft.graph.mediaContentRatingUnitedStates",
        "movieRating": "allBlocked",
        "tvRating": "allBlocked"
      },
      "networkUsageRules": [
        {
          "@odata.type": "microsoft.graph.iosNetworkUsageRule",
          "managedApps": [
            {
              "@odata.type": "microsoft.graph.appListItem",
              "name": "Name value",
              "publisher": "Publisher value",
              "appStoreUrl": "https://example.com/appStoreUrl/",
              "appId": "App Id value"
            }
          ],
          "cellularDataBlockWhenRoaming": true,
          "cellularDataBlocked": true
        }
      ],
      "mediaContentRatingApps": "allBlocked",
      "messagesBlocked": true,
      "notificationsBlockSettingsModification": true,
      "passcodeBlockFingerprintUnlock": true,
      "passcodeBlockFingerprintModification": true,
      "passcodeBlockModification": true,
      "passcodeBlockSimple": true,
      "passcodeExpirationDays": 6,
      "passcodeMinimumLength": 5,
      "passcodeMinutesOfInactivityBeforeLock": 5,
      "passcodeMinutesOfInactivityBeforeScreenTimeout": 14,
      "passcodeMinimumCharacterSetCount": 0,
      "passcodePreviousPasscodeBlockCount": 2,
      "passcodeSignInFailureCountBeforeWipe": 4,
      "passcodeRequiredType": "alphanumeric",
      "passcodeRequired": true,
      "podcastsBlocked": true,
      "safariBlockAutofill": true,
      "safariBlockJavaScript": true,
      "safariBlockPopups": true,
      "safariBlocked": true,
      "safariCookieSettings": "blockAlways",
      "safariManagedDomains": [
        "Safari Managed Domains value"
      ],
      "safariPasswordAutoFillDomains": [
        "Safari Password Auto Fill Domains value"
      ],
      "safariRequireFraudWarning": true,
      "screenCaptureBlocked": true,
      "siriBlocked": true,
      "siriBlockedWhenLocked": true,
      "siriBlockUserGeneratedContent": true,
      "siriRequireProfanityFilter": true,
      "spotlightBlockInternetResults": true,
      "voiceDialingBlocked": true,
      "wallpaperBlockModification": true,
      "wiFiConnectOnlyToConfiguredNetworks": true,
      "classroomForceRequestPermissionToLeaveClasses": true,
      "keychainBlockCloudSync": true,
      "pkiBlockOTAUpdates": true,
      "privacyForceLimitAdTracking": true,
      "enterpriseBookBlockBackup": true,
      "enterpriseBookBlockMetadataSync": true,
      "airPrintBlocked": true,
      "airPrintBlockCredentialsStorage": true,
      "airPrintForceTrustedTLS": true,
      "airPrintBlockiBeaconDiscovery": true,
      "blockSystemAppRemoval": true,
      "vpnBlockCreation": true
    }
  ]
}
```




