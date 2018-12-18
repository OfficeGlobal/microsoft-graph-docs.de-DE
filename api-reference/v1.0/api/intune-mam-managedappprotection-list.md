---
title: Auflisten von „managedAppProtection“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs managedAppProtection auf.
author: tfitzmac
ms.openlocfilehash: ed4ea950c603b8ed8ce6bf350595ca8616bb5343
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27323205"
---
# <a name="list-managedappprotections"></a><span data-ttu-id="f468b-103">Auflisten von „managedAppProtection“</span><span class="sxs-lookup"><span data-stu-id="f468b-103">List managedAppProtections</span></span>

> <span data-ttu-id="f468b-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="f468b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f468b-105">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [managedAppProtection](../resources/intune-mam-managedappprotection.md) auf.</span><span class="sxs-lookup"><span data-stu-id="f468b-105">List properties and relationships of the [managedAppProtection](../resources/intune-mam-managedappprotection.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f468b-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f468b-106">Prerequisites</span></span>
<span data-ttu-id="f468b-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f468b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f468b-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f468b-109">Permission type</span></span>|<span data-ttu-id="f468b-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f468b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f468b-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f468b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f468b-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f468b-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="f468b-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f468b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f468b-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f468b-114">Not supported.</span></span>|
|<span data-ttu-id="f468b-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f468b-115">Application</span></span>|<span data-ttu-id="f468b-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f468b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f468b-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f468b-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppPolicies
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies
```

## <a name="request-headers"></a><span data-ttu-id="f468b-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f468b-118">Request headers</span></span>
|<span data-ttu-id="f468b-119">Header</span><span class="sxs-lookup"><span data-stu-id="f468b-119">Header</span></span>|<span data-ttu-id="f468b-120">Wert</span><span class="sxs-lookup"><span data-stu-id="f468b-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f468b-121">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="f468b-121">Authorization</span></span>|<span data-ttu-id="f468b-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="f468b-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f468b-123">Accept</span><span class="sxs-lookup"><span data-stu-id="f468b-123">Accept</span></span>|<span data-ttu-id="f468b-124">application/json</span><span class="sxs-lookup"><span data-stu-id="f468b-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f468b-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f468b-125">Request body</span></span>
<span data-ttu-id="f468b-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="f468b-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f468b-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="f468b-127">Response</span></span>
<span data-ttu-id="f468b-128">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [managedAppProtection](../resources/intune-mam-managedappprotection.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="f468b-128">If successful, this method returns a `200 OK` response code and a collection of [managedAppProtection](../resources/intune-mam-managedappprotection.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f468b-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f468b-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="f468b-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f468b-130">Request</span></span>
<span data-ttu-id="f468b-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f468b-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppPolicies
```

### <a name="response"></a><span data-ttu-id="f468b-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="f468b-132">Response</span></span>
<span data-ttu-id="f468b-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f468b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



