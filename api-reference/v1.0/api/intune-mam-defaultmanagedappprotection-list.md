---
title: Auflisten von „defaultManagedAppProtection“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs defaultManagedAppProtection auf.
ms.openlocfilehash: 12e4f948ab808150ca602bc0f0b21591540e080c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018670"
---
# <a name="list-defaultmanagedappprotections"></a><span data-ttu-id="6db6f-103">Auflisten von „defaultManagedAppProtection“</span><span class="sxs-lookup"><span data-stu-id="6db6f-103">List defaultManagedAppProtections</span></span>

> <span data-ttu-id="6db6f-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="6db6f-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6db6f-105">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) auf.</span><span class="sxs-lookup"><span data-stu-id="6db6f-105">List properties and relationships of the [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6db6f-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="6db6f-106">Prerequisites</span></span>
<span data-ttu-id="6db6f-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6db6f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6db6f-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6db6f-109">Permission type</span></span>|<span data-ttu-id="6db6f-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6db6f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6db6f-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6db6f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6db6f-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="6db6f-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="6db6f-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6db6f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6db6f-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6db6f-114">Not supported.</span></span>|
|<span data-ttu-id="6db6f-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6db6f-115">Application</span></span>|<span data-ttu-id="6db6f-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6db6f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6db6f-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6db6f-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/defaultManagedAppProtections
```

## <a name="request-headers"></a><span data-ttu-id="6db6f-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6db6f-118">Request headers</span></span>
|<span data-ttu-id="6db6f-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="6db6f-119">Header</span></span>|<span data-ttu-id="6db6f-120">Wert</span><span class="sxs-lookup"><span data-stu-id="6db6f-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6db6f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="6db6f-121">Authorization</span></span>|<span data-ttu-id="6db6f-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="6db6f-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6db6f-123">Accept</span><span class="sxs-lookup"><span data-stu-id="6db6f-123">Accept</span></span>|<span data-ttu-id="6db6f-124">application/json</span><span class="sxs-lookup"><span data-stu-id="6db6f-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6db6f-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6db6f-125">Request body</span></span>
<span data-ttu-id="6db6f-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="6db6f-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6db6f-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="6db6f-127">Response</span></span>
<span data-ttu-id="6db6f-128">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="6db6f-128">If successful, this method returns a `200 OK` response code and a collection of [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6db6f-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6db6f-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="6db6f-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6db6f-130">Request</span></span>
<span data-ttu-id="6db6f-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6db6f-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/defaultManagedAppProtections
```

### <a name="response"></a><span data-ttu-id="6db6f-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="6db6f-132">Response</span></span>
<span data-ttu-id="6db6f-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6db6f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2380

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.defaultManagedAppProtection",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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
      "faceIdBlocked": true
    }
  ]
}
```


