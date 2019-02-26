---
title: Abrufen von „defaultManagedAppProtection“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs defaultManagedAppProtection.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0fb8c90f80b67ce85e4d6292b8823aefa5d0f529
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30261383"
---
# <a name="get-defaultmanagedappprotection"></a><span data-ttu-id="d66f4-103">Abrufen von „defaultManagedAppProtection“</span><span class="sxs-lookup"><span data-stu-id="d66f4-103">Get defaultManagedAppProtection</span></span>

> <span data-ttu-id="d66f4-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="d66f4-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d66f4-105">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md).</span><span class="sxs-lookup"><span data-stu-id="d66f4-105">Read properties and relationships of the [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d66f4-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="d66f4-106">Prerequisites</span></span>
<span data-ttu-id="d66f4-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="d66f4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="d66f4-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d66f4-109">Permission type</span></span>|<span data-ttu-id="d66f4-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d66f4-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d66f4-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d66f4-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d66f4-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="d66f4-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="d66f4-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d66f4-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d66f4-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d66f4-114">Not supported.</span></span>|
|<span data-ttu-id="d66f4-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d66f4-115">Application</span></span>|<span data-ttu-id="d66f4-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d66f4-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d66f4-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d66f4-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/defaultManagedAppProtections/{defaultManagedAppProtectionId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d66f4-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="d66f4-118">Optional query parameters</span></span>
<span data-ttu-id="d66f4-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="d66f4-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d66f4-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d66f4-120">Request headers</span></span>
|<span data-ttu-id="d66f4-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="d66f4-121">Header</span></span>|<span data-ttu-id="d66f4-122">Wert</span><span class="sxs-lookup"><span data-stu-id="d66f4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d66f4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d66f4-123">Authorization</span></span>|<span data-ttu-id="d66f4-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="d66f4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d66f4-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="d66f4-125">Accept</span></span>|<span data-ttu-id="d66f4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d66f4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d66f4-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d66f4-127">Request body</span></span>
<span data-ttu-id="d66f4-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="d66f4-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d66f4-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="d66f4-129">Response</span></span>
<span data-ttu-id="d66f4-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="d66f4-130">If successful, this method returns a `200 OK` response code and [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d66f4-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d66f4-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="d66f4-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d66f4-132">Request</span></span>
<span data-ttu-id="d66f4-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d66f4-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/defaultManagedAppProtections/{defaultManagedAppProtectionId}
```

### <a name="response"></a><span data-ttu-id="d66f4-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="d66f4-134">Response</span></span>
<span data-ttu-id="d66f4-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d66f4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



