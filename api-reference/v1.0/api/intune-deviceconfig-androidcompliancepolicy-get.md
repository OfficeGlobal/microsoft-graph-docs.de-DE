---
title: Abrufen von „androidCompliancePolicy“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs androidCompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 76ba793c2fb3c76ff238981e5b0dae9f14088d09
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30986663"
---
# <a name="get-androidcompliancepolicy"></a><span data-ttu-id="18fb9-103">Abrufen von „androidCompliancePolicy“</span><span class="sxs-lookup"><span data-stu-id="18fb9-103">Get androidCompliancePolicy</span></span>

> <span data-ttu-id="18fb9-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="18fb9-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="18fb9-105">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="18fb9-105">Read properties and relationships of the [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="18fb9-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="18fb9-106">Prerequisites</span></span>
<span data-ttu-id="18fb9-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="18fb9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="18fb9-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="18fb9-109">Permission type</span></span>|<span data-ttu-id="18fb9-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="18fb9-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="18fb9-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="18fb9-111">Delegated (work or school account)</span></span>|<span data-ttu-id="18fb9-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="18fb9-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="18fb9-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="18fb9-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="18fb9-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="18fb9-114">Not supported.</span></span>|
|<span data-ttu-id="18fb9-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="18fb9-115">Application</span></span>|<span data-ttu-id="18fb9-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="18fb9-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="18fb9-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="18fb9-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="18fb9-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="18fb9-118">Optional query parameters</span></span>
<span data-ttu-id="18fb9-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="18fb9-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="18fb9-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="18fb9-120">Request headers</span></span>
|<span data-ttu-id="18fb9-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="18fb9-121">Header</span></span>|<span data-ttu-id="18fb9-122">Wert</span><span class="sxs-lookup"><span data-stu-id="18fb9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="18fb9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="18fb9-123">Authorization</span></span>|<span data-ttu-id="18fb9-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="18fb9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="18fb9-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="18fb9-125">Accept</span></span>|<span data-ttu-id="18fb9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="18fb9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="18fb9-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="18fb9-127">Request body</span></span>
<span data-ttu-id="18fb9-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="18fb9-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="18fb9-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="18fb9-129">Response</span></span>
<span data-ttu-id="18fb9-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="18fb9-130">If successful, this method returns a `200 OK` response code and [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="18fb9-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="18fb9-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="18fb9-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="18fb9-132">Request</span></span>
<span data-ttu-id="18fb9-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="18fb9-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="18fb9-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="18fb9-134">Response</span></span>
<span data-ttu-id="18fb9-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="18fb9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1406

{
  "value": {
    "@odata.type": "#microsoft.graph.androidCompliancePolicy",
    "id": "752c820f-820f-752c-0f82-2c750f822c75",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "displayName": "Display Name value",
    "version": 7,
    "passwordRequired": true,
    "passwordMinimumLength": 5,
    "passwordRequiredType": "alphabetic",
    "passwordMinutesOfInactivityBeforeLock": 5,
    "passwordExpirationDays": 6,
    "passwordPreviousPasswordBlockCount": 2,
    "securityPreventInstallAppsFromUnknownSources": true,
    "securityDisableUsbDebugging": true,
    "securityRequireVerifyApps": true,
    "deviceThreatProtectionEnabled": true,
    "deviceThreatProtectionRequiredSecurityLevel": "secured",
    "securityBlockJailbrokenDevices": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value",
    "minAndroidSecurityPatchLevel": "Min Android Security Patch Level value",
    "storageRequireEncryption": true,
    "securityRequireSafetyNetAttestationBasicIntegrity": true,
    "securityRequireSafetyNetAttestationCertifiedDevice": true,
    "securityRequireGooglePlayServices": true,
    "securityRequireUpToDateSecurityProviders": true,
    "securityRequireCompanyPortalAppIntegrity": true
  }
}
```



