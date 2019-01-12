---
title: targetedManagedAppProtections auflisten
description: Listet die Eigenschaften und Beziehungen von Objekten des Typs targetedManagedAppProtection auf.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 62dd9729bf7f0cd1bad48dd738a07b2c232ec4f7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27939525"
---
# <a name="list-targetedmanagedappprotections"></a><span data-ttu-id="23db4-103">targetedManagedAppProtections auflisten</span><span class="sxs-lookup"><span data-stu-id="23db4-103">List targetedManagedAppProtections</span></span>

> <span data-ttu-id="23db4-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="23db4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="23db4-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="23db4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="23db4-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="23db4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="23db4-107">Listet die Eigenschaften und Beziehungen von Objekten des Typs [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md) auf.</span><span class="sxs-lookup"><span data-stu-id="23db4-107">List properties and relationships of the [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="23db4-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="23db4-108">Prerequisites</span></span>
<span data-ttu-id="23db4-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="23db4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="23db4-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="23db4-111">Permission type</span></span>|<span data-ttu-id="23db4-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="23db4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="23db4-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="23db4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="23db4-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="23db4-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="23db4-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="23db4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="23db4-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="23db4-116">Not supported.</span></span>|
|<span data-ttu-id="23db4-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="23db4-117">Application</span></span>|<span data-ttu-id="23db4-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="23db4-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="23db4-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="23db4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppPolicies
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies
```

## <a name="request-headers"></a><span data-ttu-id="23db4-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="23db4-120">Request headers</span></span>
|<span data-ttu-id="23db4-121">Header</span><span class="sxs-lookup"><span data-stu-id="23db4-121">Header</span></span>|<span data-ttu-id="23db4-122">Wert</span><span class="sxs-lookup"><span data-stu-id="23db4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="23db4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="23db4-123">Authorization</span></span>|<span data-ttu-id="23db4-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="23db4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="23db4-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="23db4-125">Accept</span></span>|<span data-ttu-id="23db4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="23db4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="23db4-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="23db4-127">Request body</span></span>
<span data-ttu-id="23db4-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="23db4-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="23db4-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="23db4-129">Response</span></span>
<span data-ttu-id="23db4-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="23db4-130">If successful, this method returns a `200 OK` response code and a collection of [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="23db4-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="23db4-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="23db4-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="23db4-132">Request</span></span>
<span data-ttu-id="23db4-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="23db4-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppPolicies
```

### <a name="response"></a><span data-ttu-id="23db4-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="23db4-134">Response</span></span>
<span data-ttu-id="23db4-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="23db4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2106

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
      "minimumWipeOsVersion": "Minimum Wipe Os Version value",
      "minimumWipeAppVersion": "Minimum Wipe App Version value",
      "appActionIfDeviceComplianceRequired": "wipe",
      "appActionIfMaximumPinRetriesExceeded": "wipe",
      "pinRequiredInsteadOfBiometricTimeout": "-PT3M9.8396734S",
      "isAssigned": true,
      "targetedAppManagementLevels": "unmanaged"
    }
  ]
}
```





