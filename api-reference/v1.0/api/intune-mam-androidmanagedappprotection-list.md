---
title: Auflisten von „androidManagedAppProtection“
description: Listet die Eigenschaften und Beziehungen von Objekten des Typs androidManagedAppProtection auf.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d433477e6cee4283879dc1f83409346c7b09769d
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30263042"
---
# <a name="list-androidmanagedappprotections"></a><span data-ttu-id="706c8-103">Auflisten von „androidManagedAppProtection“</span><span class="sxs-lookup"><span data-stu-id="706c8-103">List androidManagedAppProtections</span></span>

> <span data-ttu-id="706c8-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="706c8-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="706c8-105">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) auf.</span><span class="sxs-lookup"><span data-stu-id="706c8-105">List properties and relationships of the [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="706c8-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="706c8-106">Prerequisites</span></span>
<span data-ttu-id="706c8-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="706c8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="706c8-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="706c8-109">Permission type</span></span>|<span data-ttu-id="706c8-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="706c8-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="706c8-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="706c8-111">Delegated (work or school account)</span></span>|<span data-ttu-id="706c8-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="706c8-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="706c8-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="706c8-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="706c8-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="706c8-114">Not supported.</span></span>|
|<span data-ttu-id="706c8-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="706c8-115">Application</span></span>|<span data-ttu-id="706c8-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="706c8-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="706c8-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="706c8-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/androidManagedAppProtections
```

## <a name="request-headers"></a><span data-ttu-id="706c8-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="706c8-118">Request headers</span></span>
|<span data-ttu-id="706c8-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="706c8-119">Header</span></span>|<span data-ttu-id="706c8-120">Wert</span><span class="sxs-lookup"><span data-stu-id="706c8-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="706c8-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="706c8-121">Authorization</span></span>|<span data-ttu-id="706c8-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="706c8-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="706c8-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="706c8-123">Accept</span></span>|<span data-ttu-id="706c8-124">application/json</span><span class="sxs-lookup"><span data-stu-id="706c8-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="706c8-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="706c8-125">Request body</span></span>
<span data-ttu-id="706c8-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="706c8-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="706c8-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="706c8-127">Response</span></span>
<span data-ttu-id="706c8-128">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="706c8-128">If successful, this method returns a `200 OK` response code and a collection of [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="706c8-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="706c8-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="706c8-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="706c8-130">Request</span></span>
<span data-ttu-id="706c8-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="706c8-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/androidManagedAppProtections
```

### <a name="response"></a><span data-ttu-id="706c8-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="706c8-132">Response</span></span>
<span data-ttu-id="706c8-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="706c8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2065

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidManagedAppProtection",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "id": "cf517ced-7ced-cf51-ed7c-51cfed7c51cf",
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
      "isAssigned": true,
      "screenCaptureBlocked": true,
      "disableAppEncryptionIfDeviceEncryptionIsEnabled": true,
      "encryptAppData": true,
      "deployedAppCount": 0,
      "minimumRequiredPatchVersion": "Minimum Required Patch Version value",
      "minimumWarningPatchVersion": "Minimum Warning Patch Version value"
    }
  ]
}
```



