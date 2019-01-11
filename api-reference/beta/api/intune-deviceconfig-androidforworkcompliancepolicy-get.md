---
title: Abrufen von androidForWorkCompliancePolicy
description: Lesen Sie Eigenschaften und Beziehungen des AndroidForWorkCompliancePolicy-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 326b610cef5cfec723d6035736e59c7e43b04560
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27817542"
---
# <a name="get-androidforworkcompliancepolicy"></a><span data-ttu-id="adc3b-103">Abrufen von androidForWorkCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="adc3b-103">Get androidForWorkCompliancePolicy</span></span>

> <span data-ttu-id="adc3b-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="adc3b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="adc3b-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="adc3b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="adc3b-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="adc3b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="adc3b-107">Lesen Sie Eigenschaften und Beziehungen des [AndroidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="adc3b-107">Read properties and relationships of the [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="adc3b-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="adc3b-108">Prerequisites</span></span>
<span data-ttu-id="adc3b-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="adc3b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="adc3b-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="adc3b-111">Permission type</span></span>|<span data-ttu-id="adc3b-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="adc3b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="adc3b-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="adc3b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="adc3b-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="adc3b-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="adc3b-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="adc3b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="adc3b-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="adc3b-116">Not supported.</span></span>|
|<span data-ttu-id="adc3b-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="adc3b-117">Application</span></span>|<span data-ttu-id="adc3b-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="adc3b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="adc3b-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="adc3b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="adc3b-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="adc3b-120">Optional query parameters</span></span>
<span data-ttu-id="adc3b-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="adc3b-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="adc3b-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="adc3b-122">Request headers</span></span>
|<span data-ttu-id="adc3b-123">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="adc3b-123">Header</span></span>|<span data-ttu-id="adc3b-124">Wert</span><span class="sxs-lookup"><span data-stu-id="adc3b-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="adc3b-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="adc3b-125">Authorization</span></span>|<span data-ttu-id="adc3b-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="adc3b-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="adc3b-127">Annehmen</span><span class="sxs-lookup"><span data-stu-id="adc3b-127">Accept</span></span>|<span data-ttu-id="adc3b-128">application/json</span><span class="sxs-lookup"><span data-stu-id="adc3b-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="adc3b-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="adc3b-129">Request body</span></span>
<span data-ttu-id="adc3b-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="adc3b-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="adc3b-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="adc3b-131">Response</span></span>
<span data-ttu-id="adc3b-132">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [AndroidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="adc3b-132">If successful, this method returns a `200 OK` response code and [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="adc3b-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="adc3b-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="adc3b-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="adc3b-134">Request</span></span>
<span data-ttu-id="adc3b-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="adc3b-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="adc3b-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="adc3b-136">Response</span></span>
<span data-ttu-id="adc3b-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="adc3b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1481

{
  "value": {
    "@odata.type": "#microsoft.graph.androidForWorkCompliancePolicy",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "id": "a8d667bd-67bd-a8d6-bd67-d6a8bd67d6a8",
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





