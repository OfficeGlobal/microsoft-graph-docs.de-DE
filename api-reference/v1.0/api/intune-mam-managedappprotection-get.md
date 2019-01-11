---
title: Abrufen von „managedAppProtection“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs managedAppProtection.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 2c4c0c9e077965268aa700068bde8bdd53953eb4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27830597"
---
# <a name="get-managedappprotection"></a><span data-ttu-id="b73fc-103">Abrufen von „managedAppProtection“</span><span class="sxs-lookup"><span data-stu-id="b73fc-103">Get managedAppProtection</span></span>

> <span data-ttu-id="b73fc-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="b73fc-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b73fc-105">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span><span class="sxs-lookup"><span data-stu-id="b73fc-105">Read properties and relationships of the [managedAppProtection](../resources/intune-mam-managedappprotection.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b73fc-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b73fc-106">Prerequisites</span></span>
<span data-ttu-id="b73fc-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b73fc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b73fc-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b73fc-109">Permission type</span></span>|<span data-ttu-id="b73fc-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b73fc-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b73fc-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b73fc-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b73fc-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="b73fc-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="b73fc-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b73fc-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b73fc-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b73fc-114">Not supported.</span></span>|
|<span data-ttu-id="b73fc-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b73fc-115">Application</span></span>|<span data-ttu-id="b73fc-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b73fc-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b73fc-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b73fc-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppPolicies/{managedAppPolicyId}
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies/{managedAppPolicyId}
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies/{managedAppPolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b73fc-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="b73fc-118">Optional query parameters</span></span>
<span data-ttu-id="b73fc-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="b73fc-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="b73fc-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b73fc-120">Request headers</span></span>
|<span data-ttu-id="b73fc-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="b73fc-121">Header</span></span>|<span data-ttu-id="b73fc-122">Wert</span><span class="sxs-lookup"><span data-stu-id="b73fc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b73fc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b73fc-123">Authorization</span></span>|<span data-ttu-id="b73fc-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b73fc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b73fc-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="b73fc-125">Accept</span></span>|<span data-ttu-id="b73fc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b73fc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b73fc-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b73fc-127">Request body</span></span>
<span data-ttu-id="b73fc-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="b73fc-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b73fc-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="b73fc-129">Response</span></span>
<span data-ttu-id="b73fc-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [managedAppProtection](../resources/intune-mam-managedappprotection.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="b73fc-130">If successful, this method returns a `200 OK` response code and [managedAppProtection](../resources/intune-mam-managedappprotection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b73fc-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b73fc-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="b73fc-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b73fc-132">Request</span></span>
<span data-ttu-id="b73fc-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b73fc-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppPolicies/{managedAppPolicyId}
```

### <a name="response"></a><span data-ttu-id="b73fc-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="b73fc-134">Response</span></span>
<span data-ttu-id="b73fc-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b73fc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1631

{
  "value": {
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
}
```



