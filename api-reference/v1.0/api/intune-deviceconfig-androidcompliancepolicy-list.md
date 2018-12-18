---
title: Auflisten von „androidCompliancePolicy“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs androidCompliancePolicy auf.
author: tfitzmac
ms.openlocfilehash: 8d231c2578ebeb3a88372dbc765806a67bdeff3c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27313706"
---
# <a name="list-androidcompliancepolicies"></a><span data-ttu-id="740ce-103">Auflisten von „androidCompliancePolicy“</span><span class="sxs-lookup"><span data-stu-id="740ce-103">List androidCompliancePolicies</span></span>

> <span data-ttu-id="740ce-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="740ce-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="740ce-105">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) auf.</span><span class="sxs-lookup"><span data-stu-id="740ce-105">List properties and relationships of the [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="740ce-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="740ce-106">Prerequisites</span></span>
<span data-ttu-id="740ce-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="740ce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="740ce-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="740ce-109">Permission type</span></span>|<span data-ttu-id="740ce-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="740ce-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="740ce-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="740ce-111">Delegated (work or school account)</span></span>|<span data-ttu-id="740ce-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="740ce-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="740ce-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="740ce-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="740ce-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="740ce-114">Not supported.</span></span>|
|<span data-ttu-id="740ce-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="740ce-115">Application</span></span>|<span data-ttu-id="740ce-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="740ce-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="740ce-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="740ce-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="740ce-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="740ce-118">Request headers</span></span>
|<span data-ttu-id="740ce-119">Header</span><span class="sxs-lookup"><span data-stu-id="740ce-119">Header</span></span>|<span data-ttu-id="740ce-120">Wert</span><span class="sxs-lookup"><span data-stu-id="740ce-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="740ce-121">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="740ce-121">Authorization</span></span>|<span data-ttu-id="740ce-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="740ce-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="740ce-123">Accept</span><span class="sxs-lookup"><span data-stu-id="740ce-123">Accept</span></span>|<span data-ttu-id="740ce-124">application/json</span><span class="sxs-lookup"><span data-stu-id="740ce-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="740ce-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="740ce-125">Request body</span></span>
<span data-ttu-id="740ce-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="740ce-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="740ce-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="740ce-127">Response</span></span>
<span data-ttu-id="740ce-128">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="740ce-128">If successful, this method returns a `200 OK` response code and a collection of [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="740ce-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="740ce-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="740ce-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="740ce-130">Request</span></span>
<span data-ttu-id="740ce-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="740ce-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="740ce-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="740ce-132">Response</span></span>
<span data-ttu-id="740ce-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="740ce-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1476

{
  "value": [
    {
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
  ]
}
```



