---
title: targetedManagedAppProtections auflisten
description: Listet die Eigenschaften und Beziehungen von Objekten des Typs targetedManagedAppProtection auf.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: deb27f6f85f6454cddedafb6cc6ad41e242252b2
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30262195"
---
# <a name="list-targetedmanagedappprotections"></a><span data-ttu-id="d4e24-103">targetedManagedAppProtections auflisten</span><span class="sxs-lookup"><span data-stu-id="d4e24-103">List targetedManagedAppProtections</span></span>

> <span data-ttu-id="d4e24-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="d4e24-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d4e24-105">Listet die Eigenschaften und Beziehungen von Objekten des Typs [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md) auf.</span><span class="sxs-lookup"><span data-stu-id="d4e24-105">List properties and relationships of the [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d4e24-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="d4e24-106">Prerequisites</span></span>
<span data-ttu-id="d4e24-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="d4e24-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="d4e24-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d4e24-109">Permission type</span></span>|<span data-ttu-id="d4e24-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d4e24-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d4e24-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d4e24-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d4e24-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="d4e24-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="d4e24-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d4e24-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d4e24-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d4e24-114">Not supported.</span></span>|
|<span data-ttu-id="d4e24-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d4e24-115">Application</span></span>|<span data-ttu-id="d4e24-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d4e24-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d4e24-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d4e24-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppPolicies
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies
```

## <a name="request-headers"></a><span data-ttu-id="d4e24-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d4e24-118">Request headers</span></span>
|<span data-ttu-id="d4e24-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="d4e24-119">Header</span></span>|<span data-ttu-id="d4e24-120">Wert</span><span class="sxs-lookup"><span data-stu-id="d4e24-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d4e24-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d4e24-121">Authorization</span></span>|<span data-ttu-id="d4e24-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="d4e24-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d4e24-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="d4e24-123">Accept</span></span>|<span data-ttu-id="d4e24-124">application/json</span><span class="sxs-lookup"><span data-stu-id="d4e24-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d4e24-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d4e24-125">Request body</span></span>
<span data-ttu-id="d4e24-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="d4e24-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d4e24-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="d4e24-127">Response</span></span>
<span data-ttu-id="d4e24-128">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d4e24-128">If successful, this method returns a `200 OK` response code and a collection of [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d4e24-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d4e24-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="d4e24-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d4e24-130">Request</span></span>
<span data-ttu-id="d4e24-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d4e24-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppPolicies
```

### <a name="response"></a><span data-ttu-id="d4e24-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="d4e24-132">Response</span></span>
<span data-ttu-id="d4e24-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d4e24-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1750

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.targetedManagedAppProtection",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "id": "b6b92266-2266-b6b9-6622-b9b66622b9b6",
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
      "isAssigned": true
    }
  ]
}
```



