---
title: Abrufen von „androidCompliancePolicy“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs androidCompliancePolicy.
author: tfitzmac
ms.openlocfilehash: a3e9657e472a58a41e335321685c7a6cb7ac8bb9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27354306"
---
# <a name="get-androidcompliancepolicy"></a><span data-ttu-id="0b633-103">Abrufen von „androidCompliancePolicy“</span><span class="sxs-lookup"><span data-stu-id="0b633-103">Get androidCompliancePolicy</span></span>

> <span data-ttu-id="0b633-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="0b633-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0b633-105">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="0b633-105">Read properties and relationships of the [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0b633-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="0b633-106">Prerequisites</span></span>
<span data-ttu-id="0b633-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0b633-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0b633-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0b633-109">Permission type</span></span>|<span data-ttu-id="0b633-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0b633-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0b633-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0b633-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0b633-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="0b633-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="0b633-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0b633-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0b633-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0b633-114">Not supported.</span></span>|
|<span data-ttu-id="0b633-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0b633-115">Application</span></span>|<span data-ttu-id="0b633-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0b633-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0b633-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0b633-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0b633-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="0b633-118">Optional query parameters</span></span>
<span data-ttu-id="0b633-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="0b633-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="0b633-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0b633-120">Request headers</span></span>
|<span data-ttu-id="0b633-121">Header</span><span class="sxs-lookup"><span data-stu-id="0b633-121">Header</span></span>|<span data-ttu-id="0b633-122">Wert</span><span class="sxs-lookup"><span data-stu-id="0b633-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0b633-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="0b633-123">Authorization</span></span>|<span data-ttu-id="0b633-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="0b633-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0b633-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0b633-125">Accept</span></span>|<span data-ttu-id="0b633-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0b633-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0b633-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0b633-127">Request body</span></span>
<span data-ttu-id="0b633-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="0b633-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0b633-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="0b633-129">Response</span></span>
<span data-ttu-id="0b633-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="0b633-130">If successful, this method returns a `200 OK` response code and [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0b633-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0b633-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="0b633-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0b633-132">Request</span></span>
<span data-ttu-id="0b633-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0b633-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="0b633-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="0b633-134">Response</span></span>
<span data-ttu-id="0b633-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0b633-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



