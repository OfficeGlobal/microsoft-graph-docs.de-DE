---
title: Abrufen von „macOSCompliancePolicy“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs macOSCompliancePolicy.
author: tfitzmac
ms.openlocfilehash: 26e06cb7b633aacc149b4790be99d0fa74b12c67
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27353564"
---
# <a name="get-macoscompliancepolicy"></a><span data-ttu-id="cf293-103">Abrufen von „macOSCompliancePolicy“</span><span class="sxs-lookup"><span data-stu-id="cf293-103">Get macOSCompliancePolicy</span></span>

> <span data-ttu-id="cf293-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="cf293-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cf293-105">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="cf293-105">Read properties and relationships of the [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cf293-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="cf293-106">Prerequisites</span></span>
<span data-ttu-id="cf293-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cf293-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cf293-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="cf293-109">Permission type</span></span>|<span data-ttu-id="cf293-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="cf293-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cf293-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="cf293-111">Delegated (work or school account)</span></span>|<span data-ttu-id="cf293-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="cf293-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="cf293-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="cf293-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cf293-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cf293-114">Not supported.</span></span>|
|<span data-ttu-id="cf293-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="cf293-115">Application</span></span>|<span data-ttu-id="cf293-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cf293-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cf293-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="cf293-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cf293-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="cf293-118">Optional query parameters</span></span>
<span data-ttu-id="cf293-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="cf293-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="cf293-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="cf293-120">Request headers</span></span>
|<span data-ttu-id="cf293-121">Header</span><span class="sxs-lookup"><span data-stu-id="cf293-121">Header</span></span>|<span data-ttu-id="cf293-122">Wert</span><span class="sxs-lookup"><span data-stu-id="cf293-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cf293-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="cf293-123">Authorization</span></span>|<span data-ttu-id="cf293-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="cf293-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cf293-125">Accept</span><span class="sxs-lookup"><span data-stu-id="cf293-125">Accept</span></span>|<span data-ttu-id="cf293-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cf293-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cf293-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="cf293-127">Request body</span></span>
<span data-ttu-id="cf293-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="cf293-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cf293-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="cf293-129">Response</span></span>
<span data-ttu-id="cf293-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="cf293-130">If successful, this method returns a `200 OK` response code and [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cf293-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="cf293-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="cf293-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="cf293-132">Request</span></span>
<span data-ttu-id="cf293-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="cf293-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="cf293-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="cf293-134">Response</span></span>
<span data-ttu-id="cf293-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cf293-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1088

{
  "value": {
    "@odata.type": "#microsoft.graph.macOSCompliancePolicy",
    "id": "ddbadff3-dff3-ddba-f3df-baddf3dfbadd",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "displayName": "Display Name value",
    "version": 7,
    "passwordRequired": true,
    "passwordBlockSimple": true,
    "passwordExpirationDays": 6,
    "passwordMinimumLength": 5,
    "passwordMinutesOfInactivityBeforeLock": 5,
    "passwordPreviousPasswordBlockCount": 2,
    "passwordMinimumCharacterSetCount": 0,
    "passwordRequiredType": "alphanumeric",
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value",
    "systemIntegrityProtectionEnabled": true,
    "deviceThreatProtectionEnabled": true,
    "deviceThreatProtectionRequiredSecurityLevel": "secured",
    "storageRequireEncryption": true,
    "firewallEnabled": true,
    "firewallBlockAllIncoming": true,
    "firewallEnableStealthMode": true
  }
}
```



