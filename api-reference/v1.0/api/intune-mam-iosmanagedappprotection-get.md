---
title: Abrufen von „iosManagedAppProtection“
description: Liest die Eigenschaften und Beziehungen von Objekten des Typs iosManagedAppProtection.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: a7aa184c28c3ca8b02fd5c8d090334cb01f1c479
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27881144"
---
# <a name="get-iosmanagedappprotection"></a><span data-ttu-id="05748-103">Abrufen von „iosManagedAppProtection“</span><span class="sxs-lookup"><span data-stu-id="05748-103">Get iosManagedAppProtection</span></span>

> <span data-ttu-id="05748-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="05748-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="05748-105">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md).</span><span class="sxs-lookup"><span data-stu-id="05748-105">Read properties and relationships of the [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="05748-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="05748-106">Prerequisites</span></span>
<span data-ttu-id="05748-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="05748-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="05748-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="05748-109">Permission type</span></span>|<span data-ttu-id="05748-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="05748-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="05748-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="05748-111">Delegated (work or school account)</span></span>|<span data-ttu-id="05748-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="05748-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="05748-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="05748-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="05748-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="05748-114">Not supported.</span></span>|
|<span data-ttu-id="05748-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="05748-115">Application</span></span>|<span data-ttu-id="05748-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="05748-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="05748-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="05748-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="05748-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="05748-118">Optional query parameters</span></span>
<span data-ttu-id="05748-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="05748-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="05748-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="05748-120">Request headers</span></span>
|<span data-ttu-id="05748-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="05748-121">Header</span></span>|<span data-ttu-id="05748-122">Wert</span><span class="sxs-lookup"><span data-stu-id="05748-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="05748-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="05748-123">Authorization</span></span>|<span data-ttu-id="05748-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="05748-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="05748-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="05748-125">Accept</span></span>|<span data-ttu-id="05748-126">application/json</span><span class="sxs-lookup"><span data-stu-id="05748-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="05748-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="05748-127">Request body</span></span>
<span data-ttu-id="05748-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="05748-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="05748-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="05748-129">Response</span></span>
<span data-ttu-id="05748-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="05748-130">If successful, this method returns a `200 OK` response code and [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="05748-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="05748-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="05748-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="05748-132">Request</span></span>
<span data-ttu-id="05748-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="05748-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}
```

### <a name="response"></a><span data-ttu-id="05748-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="05748-134">Response</span></span>
<span data-ttu-id="05748-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="05748-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1839

{
  "value": {
    "@odata.type": "#microsoft.graph.iosManagedAppProtection",
    "displayName": "Display Name value",
    "description": "Description value",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "id": "5bc789cb-89cb-5bc7-cb89-c75bcb89c75b",
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
    "appDataEncryptionType": "afterDeviceRestart",
    "minimumRequiredSdkVersion": "Minimum Required Sdk Version value",
    "deployedAppCount": 0,
    "faceIdBlocked": true
  }
}
```



