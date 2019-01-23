---
title: targetedManagedAppProtection abrufen
description: Liest die Eigenschaften und Beziehungen von Objekten des Typs targetedManagedAppProtection.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 45c8114683735e1e48064995bb674897bc8a0fd0
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415523"
---
# <a name="get-targetedmanagedappprotection"></a><span data-ttu-id="7bac3-103">targetedManagedAppProtection abrufen</span><span class="sxs-lookup"><span data-stu-id="7bac3-103">Get targetedManagedAppProtection</span></span>

> <span data-ttu-id="7bac3-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="7bac3-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="7bac3-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7bac3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7bac3-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="7bac3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7bac3-107">Liest die Eigenschaften und Beziehungen von Objekten des Typs [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md).</span><span class="sxs-lookup"><span data-stu-id="7bac3-107">Read properties and relationships of the [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7bac3-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="7bac3-108">Prerequisites</span></span>
<span data-ttu-id="7bac3-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="7bac3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="7bac3-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7bac3-111">Permission type</span></span>|<span data-ttu-id="7bac3-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7bac3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7bac3-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7bac3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7bac3-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="7bac3-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="7bac3-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7bac3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7bac3-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7bac3-116">Not supported.</span></span>|
|<span data-ttu-id="7bac3-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7bac3-117">Application</span></span>|<span data-ttu-id="7bac3-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7bac3-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7bac3-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7bac3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppPolicies/{managedAppPolicyId}
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies/{managedAppPolicyId}
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies/{managedAppPolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7bac3-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="7bac3-120">Optional query parameters</span></span>
<span data-ttu-id="7bac3-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="7bac3-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7bac3-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7bac3-122">Request headers</span></span>
|<span data-ttu-id="7bac3-123">Header</span><span class="sxs-lookup"><span data-stu-id="7bac3-123">Header</span></span>|<span data-ttu-id="7bac3-124">Wert</span><span class="sxs-lookup"><span data-stu-id="7bac3-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7bac3-125">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="7bac3-125">Authorization</span></span>|<span data-ttu-id="7bac3-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="7bac3-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7bac3-127">Annehmen</span><span class="sxs-lookup"><span data-stu-id="7bac3-127">Accept</span></span>|<span data-ttu-id="7bac3-128">application/json</span><span class="sxs-lookup"><span data-stu-id="7bac3-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7bac3-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7bac3-129">Request body</span></span>
<span data-ttu-id="7bac3-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="7bac3-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7bac3-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="7bac3-131">Response</span></span>
<span data-ttu-id="7bac3-132">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7bac3-132">If successful, this method returns a `200 OK` response code and [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7bac3-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7bac3-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="7bac3-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7bac3-134">Request</span></span>
<span data-ttu-id="7bac3-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7bac3-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppPolicies/{managedAppPolicyId}
```

### <a name="response"></a><span data-ttu-id="7bac3-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="7bac3-136">Response</span></span>
<span data-ttu-id="7bac3-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7bac3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2076

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
    "isAssigned": true,
    "targetedAppManagementLevels": "unmanaged"
  }
}
```




