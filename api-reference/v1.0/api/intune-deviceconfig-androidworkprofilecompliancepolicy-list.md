---
title: Liste androidWorkProfileCompliancePolicies
description: Listeneigenschaften und Beziehungen der AndroidWorkProfileCompliancePolicy-Objekte.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 43b4959d3d32535d9e8e22dd9ea5a3dc07a0ca1f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27856749"
---
# <a name="list-androidworkprofilecompliancepolicies"></a><span data-ttu-id="9234f-103">Liste androidWorkProfileCompliancePolicies</span><span class="sxs-lookup"><span data-stu-id="9234f-103">List androidWorkProfileCompliancePolicies</span></span>

> <span data-ttu-id="9234f-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="9234f-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9234f-105">Listeneigenschaften und Beziehungen der [AndroidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="9234f-105">List properties and relationships of the [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9234f-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="9234f-106">Prerequisites</span></span>
<span data-ttu-id="9234f-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9234f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9234f-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9234f-109">Permission type</span></span>|<span data-ttu-id="9234f-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9234f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9234f-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9234f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9234f-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="9234f-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="9234f-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9234f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9234f-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9234f-114">Not supported.</span></span>|
|<span data-ttu-id="9234f-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9234f-115">Application</span></span>|<span data-ttu-id="9234f-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9234f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9234f-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9234f-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="9234f-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9234f-118">Request headers</span></span>
|<span data-ttu-id="9234f-119">Header</span><span class="sxs-lookup"><span data-stu-id="9234f-119">Header</span></span>|<span data-ttu-id="9234f-120">Wert</span><span class="sxs-lookup"><span data-stu-id="9234f-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9234f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="9234f-121">Authorization</span></span>|<span data-ttu-id="9234f-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="9234f-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9234f-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="9234f-123">Accept</span></span>|<span data-ttu-id="9234f-124">application/json</span><span class="sxs-lookup"><span data-stu-id="9234f-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9234f-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9234f-125">Request body</span></span>
<span data-ttu-id="9234f-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="9234f-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9234f-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="9234f-127">Response</span></span>
<span data-ttu-id="9234f-128">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [AndroidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="9234f-128">If successful, this method returns a `200 OK` response code and a collection of [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9234f-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9234f-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="9234f-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9234f-130">Request</span></span>
<span data-ttu-id="9234f-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9234f-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="9234f-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="9234f-132">Response</span></span>
<span data-ttu-id="9234f-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9234f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1487

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidWorkProfileCompliancePolicy",
      "id": "4e385271-5271-4e38-7152-384e7152384e",
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
  ]
}
```



