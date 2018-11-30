---
title: Auflisten von „managedAppProtection“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs managedAppProtection auf.
ms.openlocfilehash: 9d5b1e0f74447533ceef07dbc493ce441b75bd71
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017647"
---
# <a name="list-managedappprotections"></a><span data-ttu-id="87475-103">Auflisten von „managedAppProtection“</span><span class="sxs-lookup"><span data-stu-id="87475-103">List managedAppProtections</span></span>

> <span data-ttu-id="87475-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="87475-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="87475-105">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [managedAppProtection](../resources/intune-mam-managedappprotection.md) auf.</span><span class="sxs-lookup"><span data-stu-id="87475-105">List properties and relationships of the [managedAppProtection](../resources/intune-mam-managedappprotection.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="87475-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="87475-106">Prerequisites</span></span>
<span data-ttu-id="87475-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="87475-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="87475-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="87475-109">Permission type</span></span>|<span data-ttu-id="87475-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="87475-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="87475-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="87475-111">Delegated (work or school account)</span></span>|<span data-ttu-id="87475-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="87475-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="87475-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="87475-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="87475-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="87475-114">Not supported.</span></span>|
|<span data-ttu-id="87475-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="87475-115">Application</span></span>|<span data-ttu-id="87475-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="87475-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="87475-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="87475-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppPolicies
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies
```

## <a name="request-headers"></a><span data-ttu-id="87475-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="87475-118">Request headers</span></span>
|<span data-ttu-id="87475-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="87475-119">Header</span></span>|<span data-ttu-id="87475-120">Wert</span><span class="sxs-lookup"><span data-stu-id="87475-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="87475-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="87475-121">Authorization</span></span>|<span data-ttu-id="87475-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="87475-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="87475-123">Accept</span><span class="sxs-lookup"><span data-stu-id="87475-123">Accept</span></span>|<span data-ttu-id="87475-124">application/json</span><span class="sxs-lookup"><span data-stu-id="87475-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="87475-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="87475-125">Request body</span></span>
<span data-ttu-id="87475-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="87475-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="87475-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="87475-127">Response</span></span>
<span data-ttu-id="87475-128">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [managedAppProtection](../resources/intune-mam-managedappprotection.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="87475-128">If successful, this method returns a `200 OK` response code and a collection of [managedAppProtection](../resources/intune-mam-managedappprotection.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="87475-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="87475-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="87475-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="87475-130">Request</span></span>
<span data-ttu-id="87475-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="87475-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppPolicies
```

### <a name="response"></a><span data-ttu-id="87475-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="87475-132">Response</span></span>
<span data-ttu-id="87475-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="87475-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1715

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedAppProtection",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "id": "a6c064ce-64ce-a6c0-ce64-c0a6ce64c0a6",
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
      "minimumWarningAppVersion": "Minimum Warning App Version value"
    }
  ]
}
```


