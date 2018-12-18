---
title: windows81CompliancePolicy abrufen
description: Liest die Eigenschaften und Beziehungen von Objekten des Typs windows81CompliancePolicy.
author: tfitzmac
ms.openlocfilehash: 5e191baa2d981b2721c6a271f075cdd9f5184354
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27329743"
---
# <a name="get-windows81compliancepolicy"></a><span data-ttu-id="1c051-103">windows81CompliancePolicy abrufen</span><span class="sxs-lookup"><span data-stu-id="1c051-103">Get windows81CompliancePolicy</span></span>

> <span data-ttu-id="1c051-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="1c051-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1c051-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1c051-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1c051-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="1c051-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1c051-107">Liest die Eigenschaften und Beziehungen von Objekten des Typs [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="1c051-107">Read properties and relationships of the [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1c051-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="1c051-108">Prerequisites</span></span>
<span data-ttu-id="1c051-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1c051-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1c051-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1c051-111">Permission type</span></span>|<span data-ttu-id="1c051-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1c051-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1c051-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1c051-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1c051-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="1c051-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="1c051-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1c051-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1c051-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1c051-116">Not supported.</span></span>|
|<span data-ttu-id="1c051-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1c051-117">Application</span></span>|<span data-ttu-id="1c051-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1c051-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1c051-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1c051-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1c051-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="1c051-120">Optional query parameters</span></span>
<span data-ttu-id="1c051-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="1c051-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="1c051-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1c051-122">Request headers</span></span>
|<span data-ttu-id="1c051-123">Header</span><span class="sxs-lookup"><span data-stu-id="1c051-123">Header</span></span>|<span data-ttu-id="1c051-124">Wert</span><span class="sxs-lookup"><span data-stu-id="1c051-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1c051-125">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="1c051-125">Authorization</span></span>|<span data-ttu-id="1c051-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="1c051-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1c051-127">Accept</span><span class="sxs-lookup"><span data-stu-id="1c051-127">Accept</span></span>|<span data-ttu-id="1c051-128">application/json</span><span class="sxs-lookup"><span data-stu-id="1c051-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1c051-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1c051-129">Request body</span></span>
<span data-ttu-id="1c051-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="1c051-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1c051-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="1c051-131">Response</span></span>
<span data-ttu-id="1c051-132">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das  [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1c051-132">If successful, this method returns a `200 OK` response code and [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1c051-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1c051-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="1c051-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1c051-134">Request</span></span>
<span data-ttu-id="1c051-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1c051-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="1c051-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="1c051-136">Response</span></span>
<span data-ttu-id="1c051-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1c051-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 897

{
  "value": {
    "@odata.type": "#microsoft.graph.windows81CompliancePolicy",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "id": "6bb4b7e0-b7e0-6bb4-e0b7-b46be0b7b46b",
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
    "passwordMinimumCharacterSetCount": 0,
    "passwordRequiredType": "alphanumeric",
    "passwordPreviousPasswordBlockCount": 2,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value",
    "storageRequireEncryption": true
  }
}
```





