---
title: Auflisten von „androidGeneralDeviceConfiguration“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs androidGeneralDeviceConfiguration auf.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 783e64977611a66661ebfee01bee9ec475a27ce1
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30983953"
---
# <a name="list-androidgeneraldeviceconfigurations"></a><span data-ttu-id="6aca3-103">Auflisten von „androidGeneralDeviceConfiguration“</span><span class="sxs-lookup"><span data-stu-id="6aca3-103">List androidGeneralDeviceConfigurations</span></span>

> <span data-ttu-id="6aca3-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6aca3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6aca3-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="6aca3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6aca3-106">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) auf.</span><span class="sxs-lookup"><span data-stu-id="6aca3-106">List properties and relationships of the [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6aca3-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="6aca3-107">Prerequisites</span></span>
<span data-ttu-id="6aca3-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6aca3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6aca3-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6aca3-110">Permission type</span></span>|<span data-ttu-id="6aca3-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6aca3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6aca3-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6aca3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6aca3-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="6aca3-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="6aca3-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6aca3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6aca3-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6aca3-115">Not supported.</span></span>|
|<span data-ttu-id="6aca3-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6aca3-116">Application</span></span>|<span data-ttu-id="6aca3-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6aca3-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6aca3-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6aca3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="6aca3-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6aca3-119">Request headers</span></span>
|<span data-ttu-id="6aca3-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="6aca3-120">Header</span></span>|<span data-ttu-id="6aca3-121">Wert</span><span class="sxs-lookup"><span data-stu-id="6aca3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6aca3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6aca3-122">Authorization</span></span>|<span data-ttu-id="6aca3-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="6aca3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6aca3-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="6aca3-124">Accept</span></span>|<span data-ttu-id="6aca3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6aca3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6aca3-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6aca3-126">Request body</span></span>
<span data-ttu-id="6aca3-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="6aca3-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6aca3-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="6aca3-128">Response</span></span>
<span data-ttu-id="6aca3-129">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="6aca3-129">If successful, this method returns a `200 OK` response code and a collection of [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6aca3-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6aca3-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="6aca3-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6aca3-131">Request</span></span>
<span data-ttu-id="6aca3-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6aca3-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="6aca3-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="6aca3-133">Response</span></span>
<span data-ttu-id="6aca3-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6aca3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3766

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidGeneralDeviceConfiguration",
      "id": "9e00d534-d534-9e00-34d5-009e34d5009e",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "supportsScopeTags": true,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "appsBlockClipboardSharing": true,
      "appsBlockCopyPaste": true,
      "appsBlockYouTube": true,
      "bluetoothBlocked": true,
      "cameraBlocked": true,
      "cellularBlockDataRoaming": true,
      "cellularBlockMessaging": true,
      "cellularBlockVoiceRoaming": true,
      "cellularBlockWiFiTethering": true,
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
      "diagnosticDataBlockSubmission": true,
      "locationServicesBlocked": true,
      "googleAccountBlockAutoSync": true,
      "googlePlayStoreBlocked": true,
      "kioskModeBlockSleepButton": true,
      "kioskModeBlockVolumeButtons": true,
      "dateAndTimeBlockChanges": true,
      "kioskModeApps": [
        {
          "@odata.type": "microsoft.graph.appListItem",
          "name": "Name value",
          "publisher": "Publisher value",
          "appStoreUrl": "https://example.com/appStoreUrl/",
          "appId": "App Id value"
        }
      ],
      "nfcBlocked": true,
      "passwordBlockFingerprintUnlock": true,
      "passwordBlockTrustAgents": true,
      "passwordExpirationDays": 6,
      "passwordMinimumLength": 5,
      "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
      "passwordPreviousPasswordBlockCount": 2,
      "passwordSignInFailureCountBeforeFactoryReset": 12,
      "passwordRequiredType": "alphabetic",
      "passwordRequired": true,
      "powerOffBlocked": true,
      "factoryResetBlocked": true,
      "screenCaptureBlocked": true,
      "deviceSharingAllowed": true,
      "storageBlockGoogleBackup": true,
      "storageBlockRemovableStorage": true,
      "storageRequireDeviceEncryption": true,
      "storageRequireRemovableStorageEncryption": true,
      "voiceAssistantBlocked": true,
      "voiceDialingBlocked": true,
      "webBrowserBlockPopups": true,
      "webBrowserBlockAutofill": true,
      "webBrowserBlockJavaScript": true,
      "webBrowserBlocked": true,
      "webBrowserCookieSettings": "blockAlways",
      "wiFiBlocked": true,
      "appsInstallAllowList": [
        {
          "@odata.type": "microsoft.graph.appListItem",
          "name": "Name value",
          "publisher": "Publisher value",
          "appStoreUrl": "https://example.com/appStoreUrl/",
          "appId": "App Id value"
        }
      ],
      "appsLaunchBlockList": [
        {
          "@odata.type": "microsoft.graph.appListItem",
          "name": "Name value",
          "publisher": "Publisher value",
          "appStoreUrl": "https://example.com/appStoreUrl/",
          "appId": "App Id value"
        }
      ],
      "appsHideList": [
        {
          "@odata.type": "microsoft.graph.appListItem",
          "name": "Name value",
          "publisher": "Publisher value",
          "appStoreUrl": "https://example.com/appStoreUrl/",
          "appId": "App Id value"
        }
      ],
      "securityRequireVerifyApps": true
    }
  ]
}
```




