---
title: Auflisten von „androidGeneralDeviceConfiguration“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs androidGeneralDeviceConfiguration auf.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 0d8ba32deed7098c721cba7595692aebdee140f3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27983814"
---
# <a name="list-androidgeneraldeviceconfigurations"></a><span data-ttu-id="10d30-103">Auflisten von „androidGeneralDeviceConfiguration“</span><span class="sxs-lookup"><span data-stu-id="10d30-103">List androidGeneralDeviceConfigurations</span></span>

> <span data-ttu-id="10d30-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="10d30-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="10d30-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="10d30-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="10d30-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="10d30-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="10d30-107">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) auf.</span><span class="sxs-lookup"><span data-stu-id="10d30-107">List properties and relationships of the [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="10d30-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="10d30-108">Prerequisites</span></span>
<span data-ttu-id="10d30-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="10d30-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="10d30-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="10d30-111">Permission type</span></span>|<span data-ttu-id="10d30-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="10d30-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="10d30-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="10d30-113">Delegated (work or school account)</span></span>|<span data-ttu-id="10d30-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="10d30-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="10d30-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="10d30-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="10d30-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="10d30-116">Not supported.</span></span>|
|<span data-ttu-id="10d30-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="10d30-117">Application</span></span>|<span data-ttu-id="10d30-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="10d30-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="10d30-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="10d30-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="10d30-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="10d30-120">Request headers</span></span>
|<span data-ttu-id="10d30-121">Header</span><span class="sxs-lookup"><span data-stu-id="10d30-121">Header</span></span>|<span data-ttu-id="10d30-122">Wert</span><span class="sxs-lookup"><span data-stu-id="10d30-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="10d30-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="10d30-123">Authorization</span></span>|<span data-ttu-id="10d30-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="10d30-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="10d30-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="10d30-125">Accept</span></span>|<span data-ttu-id="10d30-126">application/json</span><span class="sxs-lookup"><span data-stu-id="10d30-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="10d30-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="10d30-127">Request body</span></span>
<span data-ttu-id="10d30-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="10d30-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="10d30-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="10d30-129">Response</span></span>
<span data-ttu-id="10d30-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="10d30-130">If successful, this method returns a `200 OK` response code and a collection of [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="10d30-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="10d30-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="10d30-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="10d30-132">Request</span></span>
<span data-ttu-id="10d30-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="10d30-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="10d30-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="10d30-134">Response</span></span>
<span data-ttu-id="10d30-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="10d30-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





