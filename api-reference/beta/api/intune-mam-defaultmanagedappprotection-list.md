---
title: Auflisten von „defaultManagedAppProtection“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs defaultManagedAppProtection auf.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 4cfcc6ff44cf818ea4e197e3c5393996d0785ddc
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29411365"
---
# <a name="list-defaultmanagedappprotections"></a><span data-ttu-id="35dbd-103">Auflisten von „defaultManagedAppProtection“</span><span class="sxs-lookup"><span data-stu-id="35dbd-103">List defaultManagedAppProtections</span></span>

> <span data-ttu-id="35dbd-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="35dbd-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="35dbd-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="35dbd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="35dbd-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="35dbd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="35dbd-107">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) auf.</span><span class="sxs-lookup"><span data-stu-id="35dbd-107">List properties and relationships of the [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="35dbd-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="35dbd-108">Prerequisites</span></span>
<span data-ttu-id="35dbd-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="35dbd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="35dbd-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="35dbd-111">Permission type</span></span>|<span data-ttu-id="35dbd-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="35dbd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="35dbd-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="35dbd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="35dbd-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="35dbd-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="35dbd-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="35dbd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="35dbd-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="35dbd-116">Not supported.</span></span>|
|<span data-ttu-id="35dbd-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="35dbd-117">Application</span></span>|<span data-ttu-id="35dbd-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="35dbd-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="35dbd-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="35dbd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/defaultManagedAppProtections
```

## <a name="request-headers"></a><span data-ttu-id="35dbd-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="35dbd-120">Request headers</span></span>
|<span data-ttu-id="35dbd-121">Header</span><span class="sxs-lookup"><span data-stu-id="35dbd-121">Header</span></span>|<span data-ttu-id="35dbd-122">Wert</span><span class="sxs-lookup"><span data-stu-id="35dbd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="35dbd-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="35dbd-123">Authorization</span></span>|<span data-ttu-id="35dbd-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="35dbd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="35dbd-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="35dbd-125">Accept</span></span>|<span data-ttu-id="35dbd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="35dbd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="35dbd-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="35dbd-127">Request body</span></span>
<span data-ttu-id="35dbd-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="35dbd-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="35dbd-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="35dbd-129">Response</span></span>
<span data-ttu-id="35dbd-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="35dbd-130">If successful, this method returns a `200 OK` response code and a collection of [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="35dbd-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="35dbd-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="35dbd-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="35dbd-132">Request</span></span>
<span data-ttu-id="35dbd-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="35dbd-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/defaultManagedAppProtections
```

### <a name="response"></a><span data-ttu-id="35dbd-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="35dbd-134">Response</span></span>
<span data-ttu-id="35dbd-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="35dbd-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3754

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.defaultManagedAppProtection",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "id": "77064c51-4c51-7706-514c-0677514c0677",
      "version": "Version value",
      "periodOfflineBeforeAccessCheck": "-PT17.1357909S",
      "periodOnlineBeforeAccessCheck": "PT35.0018757S",
      "allowedInboundDataTransferSources": "managedApps",
      "allowedOutboundDataTransferDestinations": "managedApps",
      "organizationalCredentialsRequired": true,
      "allowedOutboundClipboardSharingLevel": "managedAppsWithPasteIn",
      "dataBackupBlocked": true,
      "deviceComplianceRequired": true,
      "managedBrowserToOpenLinksRequired": true,
      "saveAsBlocked": true,
      "periodOfflineBeforeWipeIsEnforced": "-PT3M22.1587532S",
      "pinRequired": true,
      "maximumPinRetries": 1,
      "simplePinBlocked": true,
      "minimumPinLength": 0,
      "pinCharacterSet": "alphanumericAndSymbol",
      "periodBeforePinReset": "PT3M29.6631862S",
      "allowedDataStorageLocations": [
        "sharePoint"
      ],
      "contactSyncBlocked": true,
      "printBlocked": true,
      "fingerprintBlocked": true,
      "disableAppPinIfDevicePinIsSet": true,
      "minimumRequiredOsVersion": "Minimum Required Os Version value",
      "minimumWarningOsVersion": "Minimum Warning Os Version value",
      "minimumRequiredAppVersion": "Minimum Required App Version value",
      "minimumWarningAppVersion": "Minimum Warning App Version value",
      "minimumWipeOsVersion": "Minimum Wipe Os Version value",
      "minimumWipeAppVersion": "Minimum Wipe App Version value",
      "appActionIfDeviceComplianceRequired": "wipe",
      "appActionIfMaximumPinRetriesExceeded": "wipe",
      "pinRequiredInsteadOfBiometricTimeout": "-PT3M9.8396734S",
      "appDataEncryptionType": "afterDeviceRestart",
      "screenCaptureBlocked": true,
      "encryptAppData": true,
      "disableAppEncryptionIfDeviceEncryptionIsEnabled": true,
      "minimumRequiredSdkVersion": "Minimum Required Sdk Version value",
      "customSettings": [
        {
          "@odata.type": "microsoft.graph.keyValuePair",
          "name": "Name value",
          "value": "Value value"
        }
      ],
      "deployedAppCount": 0,
      "minimumRequiredPatchVersion": "Minimum Required Patch Version value",
      "minimumWarningPatchVersion": "Minimum Warning Patch Version value",
      "exemptedAppProtocols": [
        {
          "@odata.type": "microsoft.graph.keyValuePair",
          "name": "Name value",
          "value": "Value value"
        }
      ],
      "exemptedAppPackages": [
        {
          "@odata.type": "microsoft.graph.keyValuePair",
          "name": "Name value",
          "value": "Value value"
        }
      ],
      "faceIdBlocked": true,
      "minimumWipeSdkVersion": "Minimum Wipe Sdk Version value",
      "minimumWipePatchVersion": "Minimum Wipe Patch Version value",
      "allowedIosDeviceModels": "Allowed Ios Device Models value",
      "appActionIfIosDeviceModelNotAllowed": "wipe",
      "allowedAndroidDeviceManufacturers": "Allowed Android Device Manufacturers value",
      "appActionIfAndroidDeviceManufacturerNotAllowed": "wipe",
      "thirdPartyKeyboardsBlocked": true,
      "filterOpenInToOnlyManagedApps": true,
      "disableProtectionOfManagedOutboundOpenInData": true,
      "protectInboundDataFromUnknownSources": true
    }
  ]
}
```




