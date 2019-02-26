---
title: AndroidDeviceOwnerGeneralDeviceConfigurations aufListen
description: AufListen von Eigenschaften und Beziehungen der androidDeviceOwnerGeneralDeviceConfiguration-Objekte.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d36484c740d9ced29bf9bea0403639ae3dc9483b
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30146459"
---
# <a name="list-androiddeviceownergeneraldeviceconfigurations"></a><span data-ttu-id="a56d3-103">AndroidDeviceOwnerGeneralDeviceConfigurations aufListen</span><span class="sxs-lookup"><span data-stu-id="a56d3-103">List androidDeviceOwnerGeneralDeviceConfigurations</span></span>

> <span data-ttu-id="a56d3-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a56d3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a56d3-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="a56d3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a56d3-106">AufListen von Eigenschaften und Beziehungen der [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="a56d3-106">List properties and relationships of the [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a56d3-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="a56d3-107">Prerequisites</span></span>
<span data-ttu-id="a56d3-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="a56d3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a56d3-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a56d3-110">Permission type</span></span>|<span data-ttu-id="a56d3-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a56d3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a56d3-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a56d3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a56d3-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a56d3-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="a56d3-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a56d3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a56d3-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a56d3-115">Not supported.</span></span>|
|<span data-ttu-id="a56d3-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a56d3-116">Application</span></span>|<span data-ttu-id="a56d3-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a56d3-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a56d3-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a56d3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a56d3-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a56d3-119">Request headers</span></span>
|<span data-ttu-id="a56d3-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="a56d3-120">Header</span></span>|<span data-ttu-id="a56d3-121">Wert</span><span class="sxs-lookup"><span data-stu-id="a56d3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a56d3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a56d3-122">Authorization</span></span>|<span data-ttu-id="a56d3-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="a56d3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a56d3-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="a56d3-124">Accept</span></span>|<span data-ttu-id="a56d3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a56d3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a56d3-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a56d3-126">Request body</span></span>
<span data-ttu-id="a56d3-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="a56d3-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a56d3-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="a56d3-128">Response</span></span>
<span data-ttu-id="a56d3-129">Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und eine Sammlung von [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) -Objekten im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="a56d3-129">If successful, this method returns a `200 OK` response code and a collection of [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a56d3-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a56d3-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="a56d3-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a56d3-131">Request</span></span>
<span data-ttu-id="a56d3-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a56d3-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="a56d3-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="a56d3-133">Response</span></span>
<span data-ttu-id="a56d3-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a56d3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3014

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidDeviceOwnerGeneralDeviceConfiguration",
      "id": "edad943d-943d-edad-3d94-aded3d94aded",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "supportsScopeTags": true,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "accountsBlockModification": true,
      "appsAllowInstallFromUnknownSources": true,
      "appsAutoUpdatePolicy": "userChoice",
      "appsDefaultPermissionPolicy": "prompt",
      "appsRecommendSkippingFirstUseHints": true,
      "bluetoothBlockConfiguration": true,
      "bluetoothBlockContactSharing": true,
      "cameraBlocked": true,
      "cellularBlockWiFiTethering": true,
      "dataRoamingBlocked": true,
      "dateTimeConfigurationBlocked": true,
      "factoryResetDeviceAdministratorEmails": [
        "Factory Reset Device Administrator Emails value"
      ],
      "factoryResetBlocked": true,
      "kioskModeApps": [
        {
          "@odata.type": "microsoft.graph.appListItem",
          "name": "Name value",
          "publisher": "Publisher value",
          "appStoreUrl": "https://example.com/appStoreUrl/",
          "appId": "App Id value"
        }
      ],
      "kioskModeWallpaperUrl": "https://example.com/kioskModeWallpaperUrl/",
      "kioskModeExitCode": "Kiosk Mode Exit Code value",
      "kioskModeVirtualHomeButtonEnabled": true,
      "microphoneForceMute": true,
      "networkEscapeHatchAllowed": true,
      "nfcBlockOutgoingBeam": true,
      "passwordBlockKeyguard": true,
      "passwordBlockKeyguardFeatures": [
        "camera"
      ],
      "passwordExpirationDays": 6,
      "passwordMinimumLength": 5,
      "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
      "passwordPreviousPasswordCountToBlock": 4,
      "passwordRequiredType": "required",
      "passwordSignInFailureCountBeforeFactoryReset": 12,
      "safeBootBlocked": true,
      "screenCaptureBlocked": true,
      "securityAllowDebuggingFeatures": true,
      "securityRequireVerifyApps": true,
      "statusBarBlocked": true,
      "stayOnModes": [
        "ac"
      ],
      "storageAllowUsb": true,
      "storageBlockExternalMedia": true,
      "storageBlockUsbFileTransfer": true,
      "systemUpdateWindowStartMinutesAfterMidnight": 11,
      "systemUpdateWindowEndMinutesAfterMidnight": 9,
      "systemUpdateInstallType": "postpone",
      "systemWindowsBlocked": true,
      "usersBlockAdd": true,
      "usersBlockRemove": true,
      "volumeBlockAdjustment": true,
      "vpnAlwaysOnPackageIdentifier": "Vpn Always On Package Identifier value",
      "vpnAlwaysOnLockdownMode": true,
      "wifiBlockEditConfigurations": true,
      "wifiBlockEditPolicyDefinedConfigurations": true
    }
  ]
}
```




