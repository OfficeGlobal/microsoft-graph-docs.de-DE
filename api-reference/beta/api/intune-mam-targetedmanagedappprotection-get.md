---
title: targetedManagedAppProtection abrufen
description: Liest die Eigenschaften und Beziehungen von Objekten des Typs targetedManagedAppProtection.
ms.openlocfilehash: da57858b9ba896d36eba3f92d54adc4ba7689b3a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064486"
---
# <a name="get-targetedmanagedappprotection"></a><span data-ttu-id="6dad8-103">targetedManagedAppProtection abrufen</span><span class="sxs-lookup"><span data-stu-id="6dad8-103">Get targetedManagedAppProtection</span></span>

> <span data-ttu-id="6dad8-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="6dad8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6dad8-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6dad8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6dad8-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="6dad8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6dad8-107">Liest die Eigenschaften und Beziehungen von Objekten des Typs [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md).</span><span class="sxs-lookup"><span data-stu-id="6dad8-107">Read properties and relationships of the [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6dad8-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="6dad8-108">Prerequisites</span></span>
<span data-ttu-id="6dad8-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6dad8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6dad8-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6dad8-111">Permission type</span></span>|<span data-ttu-id="6dad8-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6dad8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6dad8-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6dad8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6dad8-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="6dad8-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="6dad8-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6dad8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6dad8-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6dad8-116">Not supported.</span></span>|
|<span data-ttu-id="6dad8-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6dad8-117">Application</span></span>|<span data-ttu-id="6dad8-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6dad8-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6dad8-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6dad8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppPolicies/{managedAppPolicyId}
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies/{managedAppPolicyId}
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies/{managedAppPolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6dad8-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="6dad8-120">Optional query parameters</span></span>
<span data-ttu-id="6dad8-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="6dad8-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="6dad8-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6dad8-122">Request headers</span></span>
|<span data-ttu-id="6dad8-123">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="6dad8-123">Header</span></span>|<span data-ttu-id="6dad8-124">Wert</span><span class="sxs-lookup"><span data-stu-id="6dad8-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6dad8-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="6dad8-125">Authorization</span></span>|<span data-ttu-id="6dad8-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="6dad8-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6dad8-127">Accept</span><span class="sxs-lookup"><span data-stu-id="6dad8-127">Accept</span></span>|<span data-ttu-id="6dad8-128">application/json</span><span class="sxs-lookup"><span data-stu-id="6dad8-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6dad8-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6dad8-129">Request body</span></span>
<span data-ttu-id="6dad8-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="6dad8-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6dad8-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="6dad8-131">Response</span></span>
<span data-ttu-id="6dad8-132">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6dad8-132">If successful, this method returns a `200 OK` response code and [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6dad8-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6dad8-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="6dad8-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6dad8-134">Request</span></span>
<span data-ttu-id="6dad8-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6dad8-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppPolicies/{managedAppPolicyId}
```

### <a name="response"></a><span data-ttu-id="6dad8-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="6dad8-136">Response</span></span>
<span data-ttu-id="6dad8-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6dad8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2008

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
    "minimumWipeOsVersion": "Minimum Wipe Os Version value",
    "minimumWipeAppVersion": "Minimum Wipe App Version value",
    "appActionIfDeviceComplianceRequired": "wipe",
    "appActionIfMaximumPinRetriesExceeded": "wipe",
    "pinRequiredInsteadOfBiometricTimeout": "-PT3M9.8396734S",
    "isAssigned": true,
    "targetedAppManagementLevels": "unmanaged"
  }
}
```





