---
title: Abrufen von „managedAppProtection“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs managedAppProtection.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 16f6672d7ec9ba6a1f9140c85e881cb679dde8f7
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30975098"
---
# <a name="get-managedappprotection"></a><span data-ttu-id="0fbc8-103">Abrufen von „managedAppProtection“</span><span class="sxs-lookup"><span data-stu-id="0fbc8-103">Get managedAppProtection</span></span>

> <span data-ttu-id="0fbc8-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0fbc8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0fbc8-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="0fbc8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0fbc8-106">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span><span class="sxs-lookup"><span data-stu-id="0fbc8-106">Read properties and relationships of the [managedAppProtection](../resources/intune-mam-managedappprotection.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0fbc8-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="0fbc8-107">Prerequisites</span></span>
<span data-ttu-id="0fbc8-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0fbc8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0fbc8-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0fbc8-110">Permission type</span></span>|<span data-ttu-id="0fbc8-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0fbc8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0fbc8-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0fbc8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0fbc8-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="0fbc8-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="0fbc8-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0fbc8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0fbc8-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0fbc8-115">Not supported.</span></span>|
|<span data-ttu-id="0fbc8-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0fbc8-116">Application</span></span>|<span data-ttu-id="0fbc8-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0fbc8-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0fbc8-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0fbc8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppPolicies/{managedAppPolicyId}
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies/{managedAppPolicyId}
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies/{managedAppPolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0fbc8-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="0fbc8-119">Optional query parameters</span></span>
<span data-ttu-id="0fbc8-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="0fbc8-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0fbc8-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0fbc8-121">Request headers</span></span>
|<span data-ttu-id="0fbc8-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="0fbc8-122">Header</span></span>|<span data-ttu-id="0fbc8-123">Wert</span><span class="sxs-lookup"><span data-stu-id="0fbc8-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0fbc8-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="0fbc8-124">Authorization</span></span>|<span data-ttu-id="0fbc8-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="0fbc8-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0fbc8-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="0fbc8-126">Accept</span></span>|<span data-ttu-id="0fbc8-127">application/json</span><span class="sxs-lookup"><span data-stu-id="0fbc8-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0fbc8-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0fbc8-128">Request body</span></span>
<span data-ttu-id="0fbc8-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="0fbc8-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0fbc8-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="0fbc8-130">Response</span></span>
<span data-ttu-id="0fbc8-131">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [managedAppProtection](../resources/intune-mam-managedappprotection.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="0fbc8-131">If successful, this method returns a `200 OK` response code and [managedAppProtection](../resources/intune-mam-managedappprotection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0fbc8-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0fbc8-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="0fbc8-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0fbc8-133">Request</span></span>
<span data-ttu-id="0fbc8-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0fbc8-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppPolicies/{managedAppPolicyId}
```

### <a name="response"></a><span data-ttu-id="0fbc8-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="0fbc8-135">Response</span></span>
<span data-ttu-id="0fbc8-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0fbc8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2053

{
  "value": {
    "@odata.type": "#microsoft.graph.managedAppProtection",
    "displayName": "Display Name value",
    "description": "Description value",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
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
    "minimumWarningAppVersion": "Minimum Warning App Version value",
    "minimumWipeOsVersion": "Minimum Wipe Os Version value",
    "minimumWipeAppVersion": "Minimum Wipe App Version value",
    "appActionIfDeviceComplianceRequired": "wipe",
    "appActionIfMaximumPinRetriesExceeded": "wipe",
    "pinRequiredInsteadOfBiometricTimeout": "-PT3M9.8396734S",
    "allowedOutboundClipboardSharingExceptionLength": 14
  }
}
```




