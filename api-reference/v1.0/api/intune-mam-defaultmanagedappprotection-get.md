---
title: Abrufen von „defaultManagedAppProtection“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs defaultManagedAppProtection.
author: tfitzmac
ms.openlocfilehash: 9d2b7a72f4adec0616533092ec8001d89a55dd13
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27309464"
---
# <a name="get-defaultmanagedappprotection"></a><span data-ttu-id="e64e9-103">Abrufen von „defaultManagedAppProtection“</span><span class="sxs-lookup"><span data-stu-id="e64e9-103">Get defaultManagedAppProtection</span></span>

> <span data-ttu-id="e64e9-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="e64e9-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e64e9-105">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md).</span><span class="sxs-lookup"><span data-stu-id="e64e9-105">Read properties and relationships of the [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e64e9-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="e64e9-106">Prerequisites</span></span>
<span data-ttu-id="e64e9-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e64e9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e64e9-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e64e9-109">Permission type</span></span>|<span data-ttu-id="e64e9-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e64e9-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e64e9-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e64e9-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e64e9-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="e64e9-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="e64e9-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e64e9-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e64e9-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e64e9-114">Not supported.</span></span>|
|<span data-ttu-id="e64e9-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e64e9-115">Application</span></span>|<span data-ttu-id="e64e9-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e64e9-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e64e9-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e64e9-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/defaultManagedAppProtections/{defaultManagedAppProtectionId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e64e9-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="e64e9-118">Optional query parameters</span></span>
<span data-ttu-id="e64e9-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="e64e9-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="e64e9-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e64e9-120">Request headers</span></span>
|<span data-ttu-id="e64e9-121">Header</span><span class="sxs-lookup"><span data-stu-id="e64e9-121">Header</span></span>|<span data-ttu-id="e64e9-122">Wert</span><span class="sxs-lookup"><span data-stu-id="e64e9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e64e9-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="e64e9-123">Authorization</span></span>|<span data-ttu-id="e64e9-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="e64e9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e64e9-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e64e9-125">Accept</span></span>|<span data-ttu-id="e64e9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e64e9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e64e9-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e64e9-127">Request body</span></span>
<span data-ttu-id="e64e9-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="e64e9-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e64e9-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="e64e9-129">Response</span></span>
<span data-ttu-id="e64e9-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="e64e9-130">If successful, this method returns a `200 OK` response code and [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e64e9-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e64e9-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="e64e9-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e64e9-132">Request</span></span>
<span data-ttu-id="e64e9-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e64e9-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/defaultManagedAppProtections/{defaultManagedAppProtectionId}
```

### <a name="response"></a><span data-ttu-id="e64e9-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="e64e9-134">Response</span></span>
<span data-ttu-id="e64e9-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e64e9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2264

{
  "value": {
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
}
```



