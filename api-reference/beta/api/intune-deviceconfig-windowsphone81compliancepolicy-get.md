---
title: Abrufen von „windowsPhone81CompliancePolicy“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs windowsPhone81CompliancePolicy.
ms.openlocfilehash: d68ac6dea545787dd3aa9fab7440e3febbf4a183
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060093"
---
# <a name="get-windowsphone81compliancepolicy"></a><span data-ttu-id="872d4-103">Abrufen von „windowsPhone81CompliancePolicy“</span><span class="sxs-lookup"><span data-stu-id="872d4-103">Get windowsPhone81CompliancePolicy</span></span>

> <span data-ttu-id="872d4-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="872d4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="872d4-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="872d4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="872d4-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="872d4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="872d4-107">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="872d4-107">Read properties and relationships of the [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="872d4-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="872d4-108">Prerequisites</span></span>
<span data-ttu-id="872d4-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="872d4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="872d4-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="872d4-111">Permission type</span></span>|<span data-ttu-id="872d4-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="872d4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="872d4-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="872d4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="872d4-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="872d4-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="872d4-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="872d4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="872d4-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="872d4-116">Not supported.</span></span>|
|<span data-ttu-id="872d4-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="872d4-117">Application</span></span>|<span data-ttu-id="872d4-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="872d4-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="872d4-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="872d4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="872d4-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="872d4-120">Optional query parameters</span></span>
<span data-ttu-id="872d4-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="872d4-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="872d4-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="872d4-122">Request headers</span></span>
|<span data-ttu-id="872d4-123">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="872d4-123">Header</span></span>|<span data-ttu-id="872d4-124">Wert</span><span class="sxs-lookup"><span data-stu-id="872d4-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="872d4-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="872d4-125">Authorization</span></span>|<span data-ttu-id="872d4-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="872d4-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="872d4-127">Accept</span><span class="sxs-lookup"><span data-stu-id="872d4-127">Accept</span></span>|<span data-ttu-id="872d4-128">application/json</span><span class="sxs-lookup"><span data-stu-id="872d4-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="872d4-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="872d4-129">Request body</span></span>
<span data-ttu-id="872d4-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="872d4-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="872d4-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="872d4-131">Response</span></span>
<span data-ttu-id="872d4-132">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="872d4-132">If successful, this method returns a `200 OK` response code and [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="872d4-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="872d4-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="872d4-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="872d4-134">Request</span></span>
<span data-ttu-id="872d4-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="872d4-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="872d4-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="872d4-136">Response</span></span>
<span data-ttu-id="872d4-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="872d4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 902

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsPhone81CompliancePolicy",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "id": "e6021ad4-1ad4-e602-d41a-02e6d41a02e6",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "displayName": "Display Name value",
    "version": 7,
    "passwordBlockSimple": true,
    "passwordExpirationDays": 6,
    "passwordMinimumLength": 5,
    "passwordMinutesOfInactivityBeforeLock": 5,
    "passwordMinimumCharacterSetCount": 0,
    "passwordRequiredType": "alphanumeric",
    "passwordPreviousPasswordBlockCount": 2,
    "passwordRequired": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value",
    "storageRequireEncryption": true
  }
}
```




