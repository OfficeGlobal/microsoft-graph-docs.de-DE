---
title: deviceCompliancePolicyDeviceStateSummary abrufen
description: Lesen von Beziehungen und Eigenschaften des deviceCompliancePolicyDeviceStateSummary-Objekts.
author: tfitzmac
ms.openlocfilehash: a4d0c97f94b7dd92f735cdec80d0acf9826ab4ba
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27330163"
---
# <a name="get-devicecompliancepolicydevicestatesummary"></a><span data-ttu-id="89014-103">deviceCompliancePolicyDeviceStateSummary abrufen</span><span class="sxs-lookup"><span data-stu-id="89014-103">Get deviceCompliancePolicyDeviceStateSummary</span></span>

> <span data-ttu-id="89014-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="89014-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="89014-105">Lesen von Beziehungen und Eigenschaften des [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="89014-105">Read properties and relationships of the [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="89014-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="89014-106">Prerequisites</span></span>
<span data-ttu-id="89014-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="89014-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="89014-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="89014-109">Permission type</span></span>|<span data-ttu-id="89014-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="89014-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="89014-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="89014-111">Delegated (work or school account)</span></span>|<span data-ttu-id="89014-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="89014-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="89014-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="89014-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="89014-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="89014-114">Not supported.</span></span>|
|<span data-ttu-id="89014-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="89014-115">Application</span></span>|<span data-ttu-id="89014-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="89014-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="89014-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="89014-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicyDeviceStateSummary
```

## <a name="optional-query-parameters"></a><span data-ttu-id="89014-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="89014-118">Optional query parameters</span></span>
<span data-ttu-id="89014-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="89014-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="89014-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="89014-120">Request headers</span></span>
|<span data-ttu-id="89014-121">Header</span><span class="sxs-lookup"><span data-stu-id="89014-121">Header</span></span>|<span data-ttu-id="89014-122">Wert</span><span class="sxs-lookup"><span data-stu-id="89014-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="89014-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="89014-123">Authorization</span></span>|<span data-ttu-id="89014-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="89014-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="89014-125">Accept</span><span class="sxs-lookup"><span data-stu-id="89014-125">Accept</span></span>|<span data-ttu-id="89014-126">application/json</span><span class="sxs-lookup"><span data-stu-id="89014-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="89014-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="89014-127">Request body</span></span>
<span data-ttu-id="89014-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="89014-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="89014-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="89014-129">Response</span></span>
<span data-ttu-id="89014-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="89014-130">If successful, this method returns a `200 OK` response code and [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="89014-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="89014-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="89014-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="89014-132">Request</span></span>
<span data-ttu-id="89014-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="89014-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicyDeviceStateSummary
```

### <a name="response"></a><span data-ttu-id="89014-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="89014-134">Response</span></span>
<span data-ttu-id="89014-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="89014-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 439

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceCompliancePolicyDeviceStateSummary",
    "inGracePeriodCount": 2,
    "configManagerCount": 2,
    "id": "8c4de8a7-e8a7-8c4d-a7e8-4d8ca7e84d8c",
    "unknownDeviceCount": 2,
    "notApplicableDeviceCount": 8,
    "compliantDeviceCount": 4,
    "remediatedDeviceCount": 5,
    "nonCompliantDeviceCount": 7,
    "errorDeviceCount": 0,
    "conflictDeviceCount": 3
  }
}
```



