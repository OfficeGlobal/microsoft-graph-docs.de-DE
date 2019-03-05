---
title: Abrufen von „managedAppProtection“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs managedAppProtection.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0a4e04162a6ce235a9a84f5677f65bb0caa2a15e
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30252343"
---
# <a name="get-managedappprotection"></a><span data-ttu-id="bcd34-103">Abrufen von „managedAppProtection“</span><span class="sxs-lookup"><span data-stu-id="bcd34-103">Get managedAppProtection</span></span>

> <span data-ttu-id="bcd34-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="bcd34-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bcd34-105">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span><span class="sxs-lookup"><span data-stu-id="bcd34-105">Read properties and relationships of the [managedAppProtection](../resources/intune-mam-managedappprotection.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bcd34-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="bcd34-106">Prerequisites</span></span>
<span data-ttu-id="bcd34-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="bcd34-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="bcd34-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="bcd34-109">Permission type</span></span>|<span data-ttu-id="bcd34-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="bcd34-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bcd34-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="bcd34-111">Delegated (work or school account)</span></span>|<span data-ttu-id="bcd34-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="bcd34-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="bcd34-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="bcd34-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bcd34-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bcd34-114">Not supported.</span></span>|
|<span data-ttu-id="bcd34-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="bcd34-115">Application</span></span>|<span data-ttu-id="bcd34-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bcd34-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bcd34-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="bcd34-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppPolicies/{managedAppPolicyId}
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies/{managedAppPolicyId}
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies/{managedAppPolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bcd34-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="bcd34-118">Optional query parameters</span></span>
<span data-ttu-id="bcd34-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="bcd34-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bcd34-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="bcd34-120">Request headers</span></span>
|<span data-ttu-id="bcd34-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="bcd34-121">Header</span></span>|<span data-ttu-id="bcd34-122">Wert</span><span class="sxs-lookup"><span data-stu-id="bcd34-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bcd34-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bcd34-123">Authorization</span></span>|<span data-ttu-id="bcd34-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="bcd34-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bcd34-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="bcd34-125">Accept</span></span>|<span data-ttu-id="bcd34-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bcd34-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bcd34-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="bcd34-127">Request body</span></span>
<span data-ttu-id="bcd34-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="bcd34-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bcd34-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="bcd34-129">Response</span></span>
<span data-ttu-id="bcd34-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [managedAppProtection](../resources/intune-mam-managedappprotection.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="bcd34-130">If successful, this method returns a `200 OK` response code and [managedAppProtection](../resources/intune-mam-managedappprotection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bcd34-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="bcd34-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="bcd34-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="bcd34-132">Request</span></span>
<span data-ttu-id="bcd34-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="bcd34-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppPolicies/{managedAppPolicyId}
```

### <a name="response"></a><span data-ttu-id="bcd34-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="bcd34-134">Response</span></span>
<span data-ttu-id="bcd34-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="bcd34-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



