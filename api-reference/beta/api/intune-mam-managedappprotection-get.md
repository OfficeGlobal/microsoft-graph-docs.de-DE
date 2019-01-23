---
title: Abrufen von „managedAppProtection“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs managedAppProtection.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8264fdb0c6172cd0cb61b00589bcb3471c9c6e89
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29411337"
---
# <a name="get-managedappprotection"></a><span data-ttu-id="810dd-103">Abrufen von „managedAppProtection“</span><span class="sxs-lookup"><span data-stu-id="810dd-103">Get managedAppProtection</span></span>

> <span data-ttu-id="810dd-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="810dd-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="810dd-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="810dd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="810dd-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="810dd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="810dd-107">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span><span class="sxs-lookup"><span data-stu-id="810dd-107">Read properties and relationships of the [managedAppProtection](../resources/intune-mam-managedappprotection.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="810dd-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="810dd-108">Prerequisites</span></span>
<span data-ttu-id="810dd-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="810dd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="810dd-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="810dd-111">Permission type</span></span>|<span data-ttu-id="810dd-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="810dd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="810dd-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="810dd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="810dd-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="810dd-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="810dd-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="810dd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="810dd-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="810dd-116">Not supported.</span></span>|
|<span data-ttu-id="810dd-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="810dd-117">Application</span></span>|<span data-ttu-id="810dd-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="810dd-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="810dd-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="810dd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppPolicies/{managedAppPolicyId}
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies/{managedAppPolicyId}
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies/{managedAppPolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="810dd-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="810dd-120">Optional query parameters</span></span>
<span data-ttu-id="810dd-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="810dd-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="810dd-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="810dd-122">Request headers</span></span>
|<span data-ttu-id="810dd-123">Header</span><span class="sxs-lookup"><span data-stu-id="810dd-123">Header</span></span>|<span data-ttu-id="810dd-124">Wert</span><span class="sxs-lookup"><span data-stu-id="810dd-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="810dd-125">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="810dd-125">Authorization</span></span>|<span data-ttu-id="810dd-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="810dd-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="810dd-127">Annehmen</span><span class="sxs-lookup"><span data-stu-id="810dd-127">Accept</span></span>|<span data-ttu-id="810dd-128">application/json</span><span class="sxs-lookup"><span data-stu-id="810dd-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="810dd-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="810dd-129">Request body</span></span>
<span data-ttu-id="810dd-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="810dd-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="810dd-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="810dd-131">Response</span></span>
<span data-ttu-id="810dd-132">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [managedAppProtection](../resources/intune-mam-managedappprotection.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="810dd-132">If successful, this method returns a `200 OK` response code and [managedAppProtection](../resources/intune-mam-managedappprotection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="810dd-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="810dd-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="810dd-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="810dd-134">Request</span></span>
<span data-ttu-id="810dd-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="810dd-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppPolicies/{managedAppPolicyId}
```

### <a name="response"></a><span data-ttu-id="810dd-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="810dd-136">Response</span></span>
<span data-ttu-id="810dd-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="810dd-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1994

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
    "pinRequiredInsteadOfBiometricTimeout": "-PT3M9.8396734S"
  }
}
```




