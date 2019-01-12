---
title: windows81CompliancePolicy abrufen
description: Liest die Eigenschaften und Beziehungen von Objekten des Typs windows81CompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 664249c28c4a03b4fa7c721d300aed65c716cf43
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27977815"
---
# <a name="get-windows81compliancepolicy"></a><span data-ttu-id="f23be-103">windows81CompliancePolicy abrufen</span><span class="sxs-lookup"><span data-stu-id="f23be-103">Get windows81CompliancePolicy</span></span>

> <span data-ttu-id="f23be-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f23be-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f23be-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f23be-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f23be-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="f23be-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f23be-107">Liest die Eigenschaften und Beziehungen von Objekten des Typs [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f23be-107">Read properties and relationships of the [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f23be-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f23be-108">Prerequisites</span></span>
<span data-ttu-id="f23be-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f23be-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f23be-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f23be-111">Permission type</span></span>|<span data-ttu-id="f23be-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f23be-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f23be-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f23be-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f23be-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f23be-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="f23be-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f23be-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f23be-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f23be-116">Not supported.</span></span>|
|<span data-ttu-id="f23be-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f23be-117">Application</span></span>|<span data-ttu-id="f23be-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f23be-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f23be-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f23be-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f23be-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="f23be-120">Optional query parameters</span></span>
<span data-ttu-id="f23be-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f23be-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="f23be-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f23be-122">Request headers</span></span>
|<span data-ttu-id="f23be-123">Header</span><span class="sxs-lookup"><span data-stu-id="f23be-123">Header</span></span>|<span data-ttu-id="f23be-124">Wert</span><span class="sxs-lookup"><span data-stu-id="f23be-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f23be-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="f23be-125">Authorization</span></span>|<span data-ttu-id="f23be-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="f23be-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f23be-127">Annehmen</span><span class="sxs-lookup"><span data-stu-id="f23be-127">Accept</span></span>|<span data-ttu-id="f23be-128">application/json</span><span class="sxs-lookup"><span data-stu-id="f23be-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f23be-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f23be-129">Request body</span></span>
<span data-ttu-id="f23be-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="f23be-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f23be-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="f23be-131">Response</span></span>
<span data-ttu-id="f23be-132">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das  [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f23be-132">If successful, this method returns a `200 OK` response code and [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f23be-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f23be-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="f23be-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f23be-134">Request</span></span>
<span data-ttu-id="f23be-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f23be-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="f23be-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="f23be-136">Response</span></span>
<span data-ttu-id="f23be-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f23be-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





