---
title: targetedManagedAppProtection abrufen
description: Liest die Eigenschaften und Beziehungen von Objekten des Typs targetedManagedAppProtection.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 32bab1e9ace1e6569109014a09aea637565fa782
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30958193"
---
# <a name="get-targetedmanagedappprotection"></a><span data-ttu-id="abaf4-103">targetedManagedAppProtection abrufen</span><span class="sxs-lookup"><span data-stu-id="abaf4-103">Get targetedManagedAppProtection</span></span>

> <span data-ttu-id="abaf4-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="abaf4-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="abaf4-105">Liest die Eigenschaften und Beziehungen von Objekten des Typs [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md).</span><span class="sxs-lookup"><span data-stu-id="abaf4-105">Read properties and relationships of the [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="abaf4-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="abaf4-106">Prerequisites</span></span>
<span data-ttu-id="abaf4-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="abaf4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="abaf4-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="abaf4-109">Permission type</span></span>|<span data-ttu-id="abaf4-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="abaf4-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="abaf4-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="abaf4-111">Delegated (work or school account)</span></span>|<span data-ttu-id="abaf4-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="abaf4-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="abaf4-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="abaf4-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="abaf4-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="abaf4-114">Not supported.</span></span>|
|<span data-ttu-id="abaf4-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="abaf4-115">Application</span></span>|<span data-ttu-id="abaf4-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="abaf4-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="abaf4-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="abaf4-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppPolicies/{managedAppPolicyId}
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies/{managedAppPolicyId}
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies/{managedAppPolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="abaf4-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="abaf4-118">Optional query parameters</span></span>
<span data-ttu-id="abaf4-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="abaf4-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="abaf4-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="abaf4-120">Request headers</span></span>
|<span data-ttu-id="abaf4-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="abaf4-121">Header</span></span>|<span data-ttu-id="abaf4-122">Wert</span><span class="sxs-lookup"><span data-stu-id="abaf4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="abaf4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="abaf4-123">Authorization</span></span>|<span data-ttu-id="abaf4-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="abaf4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="abaf4-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="abaf4-125">Accept</span></span>|<span data-ttu-id="abaf4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="abaf4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="abaf4-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="abaf4-127">Request body</span></span>
<span data-ttu-id="abaf4-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="abaf4-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="abaf4-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="abaf4-129">Response</span></span>
<span data-ttu-id="abaf4-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="abaf4-130">If successful, this method returns a `200 OK` response code and [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="abaf4-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="abaf4-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="abaf4-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="abaf4-132">Request</span></span>
<span data-ttu-id="abaf4-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="abaf4-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppPolicies/{managedAppPolicyId}
```

### <a name="response"></a><span data-ttu-id="abaf4-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="abaf4-134">Response</span></span>
<span data-ttu-id="abaf4-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="abaf4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1664

{
  "value": {
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
}
```



