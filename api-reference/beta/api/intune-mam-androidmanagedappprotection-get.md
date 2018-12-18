---
title: Abrufen von „androidManagedAppProtection“
description: Liest die Eigenschaften und Beziehungen von Objekten des Typs androidManagedAppProtection.
author: tfitzmac
ms.openlocfilehash: 877b7da27203c4fe625d0a5a4a187d62f96d5471
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27340502"
---
# <a name="get-androidmanagedappprotection"></a><span data-ttu-id="e59a6-103">Abrufen von „androidManagedAppProtection“</span><span class="sxs-lookup"><span data-stu-id="e59a6-103">Get androidManagedAppProtection</span></span>

> <span data-ttu-id="e59a6-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="e59a6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e59a6-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e59a6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e59a6-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="e59a6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e59a6-107">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md).</span><span class="sxs-lookup"><span data-stu-id="e59a6-107">Read properties and relationships of the [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e59a6-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="e59a6-108">Prerequisites</span></span>
<span data-ttu-id="e59a6-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e59a6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e59a6-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e59a6-111">Permission type</span></span>|<span data-ttu-id="e59a6-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e59a6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e59a6-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e59a6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e59a6-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="e59a6-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="e59a6-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e59a6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e59a6-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e59a6-116">Not supported.</span></span>|
|<span data-ttu-id="e59a6-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e59a6-117">Application</span></span>|<span data-ttu-id="e59a6-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e59a6-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e59a6-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e59a6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e59a6-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="e59a6-120">Optional query parameters</span></span>
<span data-ttu-id="e59a6-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="e59a6-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="e59a6-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e59a6-122">Request headers</span></span>
|<span data-ttu-id="e59a6-123">Header</span><span class="sxs-lookup"><span data-stu-id="e59a6-123">Header</span></span>|<span data-ttu-id="e59a6-124">Wert</span><span class="sxs-lookup"><span data-stu-id="e59a6-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e59a6-125">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="e59a6-125">Authorization</span></span>|<span data-ttu-id="e59a6-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="e59a6-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e59a6-127">Accept</span><span class="sxs-lookup"><span data-stu-id="e59a6-127">Accept</span></span>|<span data-ttu-id="e59a6-128">application/json</span><span class="sxs-lookup"><span data-stu-id="e59a6-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e59a6-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e59a6-129">Request body</span></span>
<span data-ttu-id="e59a6-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="e59a6-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e59a6-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="e59a6-131">Response</span></span>
<span data-ttu-id="e59a6-132">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="e59a6-132">If successful, this method returns a `200 OK` response code and [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e59a6-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e59a6-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="e59a6-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e59a6-134">Request</span></span>
<span data-ttu-id="e59a6-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e59a6-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}
```

### <a name="response"></a><span data-ttu-id="e59a6-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="e59a6-136">Response</span></span>
<span data-ttu-id="e59a6-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e59a6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2705

{
  "value": {
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
    "minimumWipeOsVersion": "Minimum Wipe Os Version value",
    "minimumWipeAppVersion": "Minimum Wipe App Version value",
    "appActionIfDeviceComplianceRequired": "wipe",
    "appActionIfMaximumPinRetriesExceeded": "wipe",
    "pinRequiredInsteadOfBiometricTimeout": "-PT3M9.8396734S",
    "isAssigned": true,
    "targetedAppManagementLevels": "unmanaged",
    "screenCaptureBlocked": true,
    "disableAppEncryptionIfDeviceEncryptionIsEnabled": true,
    "encryptAppData": true,
    "deployedAppCount": 0,
    "minimumRequiredPatchVersion": "Minimum Required Patch Version value",
    "minimumWarningPatchVersion": "Minimum Warning Patch Version value",
    "exemptedAppPackages": [
      {
        "@odata.type": "microsoft.graph.keyValuePair",
        "name": "Name value",
        "value": "Value value"
      }
    ],
    "minimumWipePatchVersion": "Minimum Wipe Patch Version value",
    "allowedAndroidDeviceManufacturers": "Allowed Android Device Manufacturers value",
    "appActionIfAndroidDeviceManufacturerNotAllowed": "wipe"
  }
}
```





