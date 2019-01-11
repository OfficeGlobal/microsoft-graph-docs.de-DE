---
title: targetedManagedAppProtection abrufen
description: Liest die Eigenschaften und Beziehungen von Objekten des Typs targetedManagedAppProtection.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 4ce2aa3bf61564a1c6b249679ddd7a6fecd9a052
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27878603"
---
# <a name="get-targetedmanagedappprotection"></a><span data-ttu-id="36457-103">targetedManagedAppProtection abrufen</span><span class="sxs-lookup"><span data-stu-id="36457-103">Get targetedManagedAppProtection</span></span>

> <span data-ttu-id="36457-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="36457-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="36457-105">Liest die Eigenschaften und Beziehungen von Objekten des Typs [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md).</span><span class="sxs-lookup"><span data-stu-id="36457-105">Read properties and relationships of the [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="36457-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="36457-106">Prerequisites</span></span>
<span data-ttu-id="36457-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="36457-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="36457-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="36457-109">Permission type</span></span>|<span data-ttu-id="36457-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="36457-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="36457-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="36457-111">Delegated (work or school account)</span></span>|<span data-ttu-id="36457-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="36457-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="36457-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="36457-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="36457-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="36457-114">Not supported.</span></span>|
|<span data-ttu-id="36457-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="36457-115">Application</span></span>|<span data-ttu-id="36457-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="36457-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="36457-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="36457-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppPolicies/{managedAppPolicyId}
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies/{managedAppPolicyId}
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies/{managedAppPolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="36457-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="36457-118">Optional query parameters</span></span>
<span data-ttu-id="36457-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="36457-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="36457-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="36457-120">Request headers</span></span>
|<span data-ttu-id="36457-121">Header</span><span class="sxs-lookup"><span data-stu-id="36457-121">Header</span></span>|<span data-ttu-id="36457-122">Wert</span><span class="sxs-lookup"><span data-stu-id="36457-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="36457-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="36457-123">Authorization</span></span>|<span data-ttu-id="36457-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="36457-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="36457-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="36457-125">Accept</span></span>|<span data-ttu-id="36457-126">application/json</span><span class="sxs-lookup"><span data-stu-id="36457-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="36457-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="36457-127">Request body</span></span>
<span data-ttu-id="36457-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="36457-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="36457-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="36457-129">Response</span></span>
<span data-ttu-id="36457-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="36457-130">If successful, this method returns a `200 OK` response code and [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="36457-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="36457-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="36457-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="36457-132">Request</span></span>
<span data-ttu-id="36457-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="36457-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppPolicies/{managedAppPolicyId}
```

### <a name="response"></a><span data-ttu-id="36457-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="36457-134">Response</span></span>
<span data-ttu-id="36457-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="36457-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



