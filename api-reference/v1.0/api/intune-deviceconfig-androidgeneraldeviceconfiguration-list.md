---
title: Auflisten von „androidGeneralDeviceConfiguration“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs androidGeneralDeviceConfiguration auf.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 388569bc9c7b808f7389a37b62528fdc7c740d00
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30251405"
---
# <a name="list-androidgeneraldeviceconfigurations"></a><span data-ttu-id="41e28-103">Auflisten von „androidGeneralDeviceConfiguration“</span><span class="sxs-lookup"><span data-stu-id="41e28-103">List androidGeneralDeviceConfigurations</span></span>

> <span data-ttu-id="41e28-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="41e28-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="41e28-105">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) auf.</span><span class="sxs-lookup"><span data-stu-id="41e28-105">List properties and relationships of the [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="41e28-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="41e28-106">Prerequisites</span></span>
<span data-ttu-id="41e28-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="41e28-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="41e28-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="41e28-109">Permission type</span></span>|<span data-ttu-id="41e28-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="41e28-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="41e28-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="41e28-111">Delegated (work or school account)</span></span>|<span data-ttu-id="41e28-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="41e28-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="41e28-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="41e28-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="41e28-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="41e28-114">Not supported.</span></span>|
|<span data-ttu-id="41e28-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="41e28-115">Application</span></span>|<span data-ttu-id="41e28-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="41e28-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="41e28-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="41e28-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="41e28-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="41e28-118">Request headers</span></span>
|<span data-ttu-id="41e28-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="41e28-119">Header</span></span>|<span data-ttu-id="41e28-120">Wert</span><span class="sxs-lookup"><span data-stu-id="41e28-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="41e28-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="41e28-121">Authorization</span></span>|<span data-ttu-id="41e28-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="41e28-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="41e28-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="41e28-123">Accept</span></span>|<span data-ttu-id="41e28-124">application/json</span><span class="sxs-lookup"><span data-stu-id="41e28-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="41e28-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="41e28-125">Request body</span></span>
<span data-ttu-id="41e28-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="41e28-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="41e28-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="41e28-127">Response</span></span>
<span data-ttu-id="41e28-128">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="41e28-128">If successful, this method returns a `200 OK` response code and a collection of [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="41e28-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="41e28-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="41e28-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="41e28-130">Request</span></span>
<span data-ttu-id="41e28-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="41e28-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="41e28-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="41e28-132">Response</span></span>
<span data-ttu-id="41e28-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="41e28-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3618

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidGeneralDeviceConfiguration",
      "id": "9e00d534-d534-9e00-34d5-009e34d5009e",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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



