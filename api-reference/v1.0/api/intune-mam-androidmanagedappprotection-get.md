---
title: Abrufen von „androidManagedAppProtection“
description: Liest die Eigenschaften und Beziehungen von Objekten des Typs androidManagedAppProtection.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 40fc43036a4bd6deed7d4bb7f05eb9d6866b9fae
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27825039"
---
# <a name="get-androidmanagedappprotection"></a><span data-ttu-id="5c11f-103">Abrufen von „androidManagedAppProtection“</span><span class="sxs-lookup"><span data-stu-id="5c11f-103">Get androidManagedAppProtection</span></span>

> <span data-ttu-id="5c11f-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="5c11f-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5c11f-105">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md).</span><span class="sxs-lookup"><span data-stu-id="5c11f-105">Read properties and relationships of the [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5c11f-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="5c11f-106">Prerequisites</span></span>
<span data-ttu-id="5c11f-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5c11f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5c11f-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5c11f-109">Permission type</span></span>|<span data-ttu-id="5c11f-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5c11f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5c11f-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5c11f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5c11f-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="5c11f-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="5c11f-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5c11f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5c11f-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5c11f-114">Not supported.</span></span>|
|<span data-ttu-id="5c11f-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5c11f-115">Application</span></span>|<span data-ttu-id="5c11f-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5c11f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5c11f-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5c11f-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5c11f-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="5c11f-118">Optional query parameters</span></span>
<span data-ttu-id="5c11f-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="5c11f-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="5c11f-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5c11f-120">Request headers</span></span>
|<span data-ttu-id="5c11f-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="5c11f-121">Header</span></span>|<span data-ttu-id="5c11f-122">Wert</span><span class="sxs-lookup"><span data-stu-id="5c11f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5c11f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5c11f-123">Authorization</span></span>|<span data-ttu-id="5c11f-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="5c11f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5c11f-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="5c11f-125">Accept</span></span>|<span data-ttu-id="5c11f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5c11f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5c11f-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5c11f-127">Request body</span></span>
<span data-ttu-id="5c11f-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="5c11f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5c11f-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="5c11f-129">Response</span></span>
<span data-ttu-id="5c11f-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="5c11f-130">If successful, this method returns a `200 OK` response code and [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5c11f-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5c11f-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="5c11f-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5c11f-132">Request</span></span>
<span data-ttu-id="5c11f-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5c11f-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}
```

### <a name="response"></a><span data-ttu-id="5c11f-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="5c11f-134">Response</span></span>
<span data-ttu-id="5c11f-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5c11f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1967

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
    "isAssigned": true,
    "screenCaptureBlocked": true,
    "disableAppEncryptionIfDeviceEncryptionIsEnabled": true,
    "encryptAppData": true,
    "deployedAppCount": 0,
    "minimumRequiredPatchVersion": "Minimum Required Patch Version value",
    "minimumWarningPatchVersion": "Minimum Warning Patch Version value"
  }
}
```



