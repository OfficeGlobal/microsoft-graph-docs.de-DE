---
title: Auflisten von „defaultManagedAppProtection“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs defaultManagedAppProtection auf.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a9e6e614334cf025eec45fc08a4e2289d14c9b95
ms.sourcegitcommit: f58ff560fa02ac95e296375c143b0922fb6a425c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/19/2019
ms.locfileid: "30572446"
---
# <a name="list-defaultmanagedappprotections"></a><span data-ttu-id="3d68b-103">Auflisten von „defaultManagedAppProtection“</span><span class="sxs-lookup"><span data-stu-id="3d68b-103">List defaultManagedAppProtections</span></span>

> <span data-ttu-id="3d68b-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3d68b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3d68b-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="3d68b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3d68b-106">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) auf.</span><span class="sxs-lookup"><span data-stu-id="3d68b-106">List properties and relationships of the [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3d68b-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="3d68b-107">Prerequisites</span></span>
<span data-ttu-id="3d68b-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="3d68b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="3d68b-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3d68b-110">Permission type</span></span>|<span data-ttu-id="3d68b-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3d68b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3d68b-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3d68b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3d68b-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="3d68b-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="3d68b-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3d68b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3d68b-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3d68b-115">Not supported.</span></span>|
|<span data-ttu-id="3d68b-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3d68b-116">Application</span></span>|<span data-ttu-id="3d68b-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3d68b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3d68b-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3d68b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/defaultManagedAppProtections
```

## <a name="request-headers"></a><span data-ttu-id="3d68b-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3d68b-119">Request headers</span></span>
|<span data-ttu-id="3d68b-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="3d68b-120">Header</span></span>|<span data-ttu-id="3d68b-121">Wert</span><span class="sxs-lookup"><span data-stu-id="3d68b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3d68b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3d68b-122">Authorization</span></span>|<span data-ttu-id="3d68b-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="3d68b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3d68b-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="3d68b-124">Accept</span></span>|<span data-ttu-id="3d68b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3d68b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3d68b-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3d68b-126">Request body</span></span>
<span data-ttu-id="3d68b-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="3d68b-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3d68b-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="3d68b-128">Response</span></span>
<span data-ttu-id="3d68b-129">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="3d68b-129">If successful, this method returns a `200 OK` response code and a collection of [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3d68b-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3d68b-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="3d68b-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3d68b-131">Request</span></span>
<span data-ttu-id="3d68b-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3d68b-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/defaultManagedAppProtections
```

### <a name="response"></a><span data-ttu-id="3d68b-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="3d68b-133">Response</span></span>
<span data-ttu-id="3d68b-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3d68b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4092

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
      "allowedOutboundClipboardSharingExceptionLength": 14,
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
      "protectInboundDataFromUnknownSources": true,
      "requiredAndroidSafetyNetDeviceAttestationType": "basicIntegrity",
      "appActionIfAndroidSafetyNetDeviceAttestationFailed": "wipe",
      "requiredAndroidSafetyNetAppsVerificationType": "enabled",
      "appActionIfAndroidSafetyNetAppsVerificationFailed": "wipe"
    }
  ]
}
```




