---
title: windows10CompliancePolicy abrufen
description: Liest die Eigenschaften und Beziehungen von Objekten des Typs windows10CompliancePolicy.
ms.openlocfilehash: 7cfb4e289dfc14233590df72a77d339d3c8a2079
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016378"
---
# <a name="get-windows10compliancepolicy"></a><span data-ttu-id="69540-103">windows10CompliancePolicy abrufen</span><span class="sxs-lookup"><span data-stu-id="69540-103">Get windows10CompliancePolicy</span></span>

> <span data-ttu-id="69540-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="69540-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="69540-105">Liest die Eigenschaften und Beziehungen von Objekten des Typs [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="69540-105">Read properties and relationships of the [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="69540-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="69540-106">Prerequisites</span></span>
<span data-ttu-id="69540-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="69540-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="69540-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="69540-109">Permission type</span></span>|<span data-ttu-id="69540-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="69540-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="69540-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="69540-111">Delegated (work or school account)</span></span>|<span data-ttu-id="69540-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="69540-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="69540-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="69540-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="69540-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="69540-114">Not supported.</span></span>|
|<span data-ttu-id="69540-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="69540-115">Application</span></span>|<span data-ttu-id="69540-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="69540-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="69540-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="69540-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="69540-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="69540-118">Optional query parameters</span></span>
<span data-ttu-id="69540-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="69540-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="69540-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="69540-120">Request headers</span></span>
|<span data-ttu-id="69540-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="69540-121">Header</span></span>|<span data-ttu-id="69540-122">Wert</span><span class="sxs-lookup"><span data-stu-id="69540-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="69540-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="69540-123">Authorization</span></span>|<span data-ttu-id="69540-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="69540-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="69540-125">Accept</span><span class="sxs-lookup"><span data-stu-id="69540-125">Accept</span></span>|<span data-ttu-id="69540-126">application/json</span><span class="sxs-lookup"><span data-stu-id="69540-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="69540-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="69540-127">Request body</span></span>
<span data-ttu-id="69540-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="69540-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="69540-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="69540-129">Response</span></span>
<span data-ttu-id="69540-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="69540-130">If successful, this method returns a `200 OK` response code and [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="69540-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="69540-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="69540-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="69540-132">Request</span></span>
<span data-ttu-id="69540-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="69540-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="69540-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="69540-134">Response</span></span>
<span data-ttu-id="69540-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="69540-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1197

{
  "value": {
    "@odata.type": "#microsoft.graph.windows10CompliancePolicy",
    "id": "2919ae62-ae62-2919-62ae-192962ae1929",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "displayName": "Display Name value",
    "version": 7,
    "passwordRequired": true,
    "passwordBlockSimple": true,
    "passwordRequiredToUnlockFromIdle": true,
    "passwordMinutesOfInactivityBeforeLock": 5,
    "passwordExpirationDays": 6,
    "passwordMinimumLength": 5,
    "passwordMinimumCharacterSetCount": 0,
    "passwordRequiredType": "alphanumeric",
    "passwordPreviousPasswordBlockCount": 2,
    "requireHealthyDeviceReport": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value",
    "mobileOsMinimumVersion": "Mobile Os Minimum Version value",
    "mobileOsMaximumVersion": "Mobile Os Maximum Version value",
    "earlyLaunchAntiMalwareDriverEnabled": true,
    "bitLockerEnabled": true,
    "secureBootEnabled": true,
    "codeIntegrityEnabled": true,
    "storageRequireEncryption": true
  }
}
```



