---
title: targetedManagedAppProtection abrufen
description: Liest die Eigenschaften und Beziehungen von Objekten des Typs targetedManagedAppProtection.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: bead70fec32c878b350c0b8ae65b5c0683e4dad0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27930656"
---
# <a name="get-targetedmanagedappprotection"></a><span data-ttu-id="68751-103">targetedManagedAppProtection abrufen</span><span class="sxs-lookup"><span data-stu-id="68751-103">Get targetedManagedAppProtection</span></span>

> <span data-ttu-id="68751-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="68751-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="68751-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="68751-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="68751-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="68751-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="68751-107">Liest die Eigenschaften und Beziehungen von Objekten des Typs [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md).</span><span class="sxs-lookup"><span data-stu-id="68751-107">Read properties and relationships of the [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="68751-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="68751-108">Prerequisites</span></span>
<span data-ttu-id="68751-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="68751-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="68751-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="68751-111">Permission type</span></span>|<span data-ttu-id="68751-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="68751-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="68751-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="68751-113">Delegated (work or school account)</span></span>|<span data-ttu-id="68751-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="68751-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="68751-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="68751-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="68751-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="68751-116">Not supported.</span></span>|
|<span data-ttu-id="68751-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="68751-117">Application</span></span>|<span data-ttu-id="68751-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="68751-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="68751-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="68751-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppPolicies/{managedAppPolicyId}
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies/{managedAppPolicyId}
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies/{managedAppPolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="68751-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="68751-120">Optional query parameters</span></span>
<span data-ttu-id="68751-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="68751-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="68751-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="68751-122">Request headers</span></span>
|<span data-ttu-id="68751-123">Header</span><span class="sxs-lookup"><span data-stu-id="68751-123">Header</span></span>|<span data-ttu-id="68751-124">Wert</span><span class="sxs-lookup"><span data-stu-id="68751-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="68751-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="68751-125">Authorization</span></span>|<span data-ttu-id="68751-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="68751-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="68751-127">Annehmen</span><span class="sxs-lookup"><span data-stu-id="68751-127">Accept</span></span>|<span data-ttu-id="68751-128">application/json</span><span class="sxs-lookup"><span data-stu-id="68751-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="68751-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="68751-129">Request body</span></span>
<span data-ttu-id="68751-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="68751-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="68751-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="68751-131">Response</span></span>
<span data-ttu-id="68751-132">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="68751-132">If successful, this method returns a `200 OK` response code and [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="68751-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="68751-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="68751-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="68751-134">Request</span></span>
<span data-ttu-id="68751-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="68751-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppPolicies/{managedAppPolicyId}
```

### <a name="response"></a><span data-ttu-id="68751-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="68751-136">Response</span></span>
<span data-ttu-id="68751-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="68751-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





