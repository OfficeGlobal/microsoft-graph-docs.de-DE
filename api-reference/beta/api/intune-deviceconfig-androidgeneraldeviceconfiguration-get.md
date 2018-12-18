---
title: androidGeneralDeviceConfiguration abrufen
description: Lesen von Eigenschaften und Beziehungen des androidGeneralDeviceConfiguration-Objekts.
author: tfitzmac
ms.openlocfilehash: e78ee24729232ff690197a6934fa6ad1e367ba99
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27345227"
---
# <a name="get-androidgeneraldeviceconfiguration"></a><span data-ttu-id="cc7c6-103">androidGeneralDeviceConfiguration abrufen</span><span class="sxs-lookup"><span data-stu-id="cc7c6-103">Get androidGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="cc7c6-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="cc7c6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cc7c6-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="cc7c6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cc7c6-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="cc7c6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cc7c6-107">Lesen von Eigenschaften und Beziehungen des [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="cc7c6-107">Read properties and relationships of the [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cc7c6-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="cc7c6-108">Prerequisites</span></span>
<span data-ttu-id="cc7c6-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cc7c6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cc7c6-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="cc7c6-111">Permission type</span></span>|<span data-ttu-id="cc7c6-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="cc7c6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cc7c6-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="cc7c6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cc7c6-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="cc7c6-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="cc7c6-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="cc7c6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cc7c6-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cc7c6-116">Not supported.</span></span>|
|<span data-ttu-id="cc7c6-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="cc7c6-117">Application</span></span>|<span data-ttu-id="cc7c6-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cc7c6-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cc7c6-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="cc7c6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cc7c6-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="cc7c6-120">Optional query parameters</span></span>
<span data-ttu-id="cc7c6-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="cc7c6-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="cc7c6-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="cc7c6-122">Request headers</span></span>
|<span data-ttu-id="cc7c6-123">Header</span><span class="sxs-lookup"><span data-stu-id="cc7c6-123">Header</span></span>|<span data-ttu-id="cc7c6-124">Wert</span><span class="sxs-lookup"><span data-stu-id="cc7c6-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cc7c6-125">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="cc7c6-125">Authorization</span></span>|<span data-ttu-id="cc7c6-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="cc7c6-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cc7c6-127">Accept</span><span class="sxs-lookup"><span data-stu-id="cc7c6-127">Accept</span></span>|<span data-ttu-id="cc7c6-128">application/json</span><span class="sxs-lookup"><span data-stu-id="cc7c6-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cc7c6-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="cc7c6-129">Request body</span></span>
<span data-ttu-id="cc7c6-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="cc7c6-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cc7c6-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="cc7c6-131">Response</span></span>
<span data-ttu-id="cc7c6-132">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cc7c6-132">If successful, this method returns a `200 OK` response code and [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cc7c6-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="cc7c6-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="cc7c6-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="cc7c6-134">Request</span></span>
<span data-ttu-id="cc7c6-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="cc7c6-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="cc7c6-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="cc7c6-136">Response</span></span>
<span data-ttu-id="cc7c6-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cc7c6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3552

{
  "value": {
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
}
```





