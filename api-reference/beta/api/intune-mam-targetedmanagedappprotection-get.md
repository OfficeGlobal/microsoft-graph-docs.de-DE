---
title: targetedManagedAppProtection abrufen
description: Liest die Eigenschaften und Beziehungen von Objekten des Typs targetedManagedAppProtection.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ac41c395a90d163437362513b2c69ce9a5ede4fb
ms.sourcegitcommit: f58ff560fa02ac95e296375c143b0922fb6a425c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/19/2019
ms.locfileid: "30572551"
---
# <a name="get-targetedmanagedappprotection"></a><span data-ttu-id="5e710-103">targetedManagedAppProtection abrufen</span><span class="sxs-lookup"><span data-stu-id="5e710-103">Get targetedManagedAppProtection</span></span>

> <span data-ttu-id="5e710-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5e710-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5e710-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="5e710-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5e710-106">Liest die Eigenschaften und Beziehungen von Objekten des Typs [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md).</span><span class="sxs-lookup"><span data-stu-id="5e710-106">Read properties and relationships of the [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5e710-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="5e710-107">Prerequisites</span></span>
<span data-ttu-id="5e710-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="5e710-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="5e710-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5e710-110">Permission type</span></span>|<span data-ttu-id="5e710-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5e710-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5e710-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5e710-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5e710-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="5e710-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="5e710-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5e710-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5e710-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5e710-115">Not supported.</span></span>|
|<span data-ttu-id="5e710-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5e710-116">Application</span></span>|<span data-ttu-id="5e710-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5e710-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5e710-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5e710-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppPolicies/{managedAppPolicyId}
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies/{managedAppPolicyId}
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies/{managedAppPolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5e710-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="5e710-119">Optional query parameters</span></span>
<span data-ttu-id="5e710-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="5e710-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5e710-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5e710-121">Request headers</span></span>
|<span data-ttu-id="5e710-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="5e710-122">Header</span></span>|<span data-ttu-id="5e710-123">Wert</span><span class="sxs-lookup"><span data-stu-id="5e710-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5e710-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="5e710-124">Authorization</span></span>|<span data-ttu-id="5e710-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="5e710-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5e710-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="5e710-126">Accept</span></span>|<span data-ttu-id="5e710-127">application/json</span><span class="sxs-lookup"><span data-stu-id="5e710-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5e710-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5e710-128">Request body</span></span>
<span data-ttu-id="5e710-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="5e710-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5e710-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="5e710-130">Response</span></span>
<span data-ttu-id="5e710-131">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5e710-131">If successful, this method returns a `200 OK` response code and [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5e710-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5e710-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="5e710-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5e710-133">Request</span></span>
<span data-ttu-id="5e710-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5e710-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppPolicies/{managedAppPolicyId}
```

### <a name="response"></a><span data-ttu-id="5e710-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="5e710-135">Response</span></span>
<span data-ttu-id="5e710-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5e710-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2135

{
  "value": {
    "@odata.type": "#microsoft.graph.targetedManagedAppProtection",
    "displayName": "Display Name value",
    "description": "Description value",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
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
    "minimumWipeOsVersion": "Minimum Wipe Os Version value",
    "minimumWipeAppVersion": "Minimum Wipe App Version value",
    "appActionIfDeviceComplianceRequired": "wipe",
    "appActionIfMaximumPinRetriesExceeded": "wipe",
    "pinRequiredInsteadOfBiometricTimeout": "-PT3M9.8396734S",
    "allowedOutboundClipboardSharingExceptionLength": 14,
    "isAssigned": true,
    "targetedAppManagementLevels": "unmanaged"
  }
}
```




