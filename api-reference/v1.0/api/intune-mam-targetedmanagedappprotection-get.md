---
title: targetedManagedAppProtection abrufen
description: Liest die Eigenschaften und Beziehungen von Objekten des Typs targetedManagedAppProtection.
ms.openlocfilehash: f86cf0efafc54d17c6f27443c1e89caccaf49787
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27019565"
---
# <a name="get-targetedmanagedappprotection"></a><span data-ttu-id="e4944-103">targetedManagedAppProtection abrufen</span><span class="sxs-lookup"><span data-stu-id="e4944-103">Get targetedManagedAppProtection</span></span>

> <span data-ttu-id="e4944-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="e4944-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e4944-105">Liest die Eigenschaften und Beziehungen von Objekten des Typs [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md).</span><span class="sxs-lookup"><span data-stu-id="e4944-105">Read properties and relationships of the [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e4944-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="e4944-106">Prerequisites</span></span>
<span data-ttu-id="e4944-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e4944-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e4944-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e4944-109">Permission type</span></span>|<span data-ttu-id="e4944-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e4944-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e4944-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e4944-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e4944-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="e4944-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="e4944-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e4944-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e4944-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e4944-114">Not supported.</span></span>|
|<span data-ttu-id="e4944-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e4944-115">Application</span></span>|<span data-ttu-id="e4944-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e4944-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e4944-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e4944-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppPolicies/{managedAppPolicyId}
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies/{managedAppPolicyId}
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies/{managedAppPolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e4944-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="e4944-118">Optional query parameters</span></span>
<span data-ttu-id="e4944-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="e4944-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="e4944-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e4944-120">Request headers</span></span>
|<span data-ttu-id="e4944-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="e4944-121">Header</span></span>|<span data-ttu-id="e4944-122">Wert</span><span class="sxs-lookup"><span data-stu-id="e4944-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e4944-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e4944-123">Authorization</span></span>|<span data-ttu-id="e4944-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="e4944-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e4944-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e4944-125">Accept</span></span>|<span data-ttu-id="e4944-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e4944-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e4944-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e4944-127">Request body</span></span>
<span data-ttu-id="e4944-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="e4944-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e4944-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="e4944-129">Response</span></span>
<span data-ttu-id="e4944-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e4944-130">If successful, this method returns a `200 OK` response code and [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e4944-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e4944-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="e4944-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e4944-132">Request</span></span>
<span data-ttu-id="e4944-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e4944-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppPolicies/{managedAppPolicyId}
```

### <a name="response"></a><span data-ttu-id="e4944-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="e4944-134">Response</span></span>
<span data-ttu-id="e4944-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e4944-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



