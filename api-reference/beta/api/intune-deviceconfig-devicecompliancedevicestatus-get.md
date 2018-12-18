---
title: Abrufen von „deviceComplianceDeviceStatus“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs deviceComplianceDeviceStatus.
author: tfitzmac
ms.openlocfilehash: c41c07ac3ae19fd3b09fc8209fd166fb2538fef5
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27321896"
---
# <a name="get-devicecompliancedevicestatus"></a><span data-ttu-id="78fec-103">Abrufen von „deviceComplianceDeviceStatus“</span><span class="sxs-lookup"><span data-stu-id="78fec-103">Get deviceComplianceDeviceStatus</span></span>

> <span data-ttu-id="78fec-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="78fec-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="78fec-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="78fec-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="78fec-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="78fec-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="78fec-107">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="78fec-107">Read properties and relationships of the [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="78fec-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="78fec-108">Prerequisites</span></span>
<span data-ttu-id="78fec-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="78fec-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="78fec-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="78fec-111">Permission type</span></span>|<span data-ttu-id="78fec-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="78fec-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="78fec-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="78fec-113">Delegated (work or school account)</span></span>|<span data-ttu-id="78fec-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="78fec-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="78fec-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="78fec-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="78fec-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="78fec-116">Not supported.</span></span>|
|<span data-ttu-id="78fec-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="78fec-117">Application</span></span>|<span data-ttu-id="78fec-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="78fec-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="78fec-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="78fec-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses/{deviceComplianceDeviceStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="78fec-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="78fec-120">Optional query parameters</span></span>
<span data-ttu-id="78fec-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="78fec-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="78fec-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="78fec-122">Request headers</span></span>
|<span data-ttu-id="78fec-123">Header</span><span class="sxs-lookup"><span data-stu-id="78fec-123">Header</span></span>|<span data-ttu-id="78fec-124">Wert</span><span class="sxs-lookup"><span data-stu-id="78fec-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="78fec-125">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="78fec-125">Authorization</span></span>|<span data-ttu-id="78fec-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="78fec-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="78fec-127">Accept</span><span class="sxs-lookup"><span data-stu-id="78fec-127">Accept</span></span>|<span data-ttu-id="78fec-128">application/json</span><span class="sxs-lookup"><span data-stu-id="78fec-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="78fec-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="78fec-129">Request body</span></span>
<span data-ttu-id="78fec-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="78fec-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="78fec-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="78fec-131">Response</span></span>
<span data-ttu-id="78fec-132">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="78fec-132">If successful, this method returns a `200 OK` response code and [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="78fec-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="78fec-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="78fec-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="78fec-134">Request</span></span>
<span data-ttu-id="78fec-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="78fec-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses/{deviceComplianceDeviceStatusId}
```

### <a name="response"></a><span data-ttu-id="78fec-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="78fec-136">Response</span></span>
<span data-ttu-id="78fec-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="78fec-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 532

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceComplianceDeviceStatus",
    "id": "c6c78124-8124-c6c7-2481-c7c62481c7c6",
    "deviceDisplayName": "Device Display Name value",
    "userName": "User Name value",
    "deviceModel": "Device Model value",
    "platform": 8,
    "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
    "status": "notApplicable",
    "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
    "userPrincipalName": "User Principal Name value"
  }
}
```





