---
title: deviceCompliancePolicyDeviceStateSummary abrufen
description: Lesen von Beziehungen und Eigenschaften des deviceCompliancePolicyDeviceStateSummary-Objekts.
ms.openlocfilehash: ceaca2909281ad3fd39c281ae9c348f3e0aa0b2c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060218"
---
# <a name="get-devicecompliancepolicydevicestatesummary"></a><span data-ttu-id="8d2b4-103">deviceCompliancePolicyDeviceStateSummary abrufen</span><span class="sxs-lookup"><span data-stu-id="8d2b4-103">Get deviceCompliancePolicyDeviceStateSummary</span></span>

> <span data-ttu-id="8d2b4-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="8d2b4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8d2b4-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8d2b4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8d2b4-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="8d2b4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8d2b4-107">Lesen von Beziehungen und Eigenschaften des [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="8d2b4-107">Read properties and relationships of the [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8d2b4-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="8d2b4-108">Prerequisites</span></span>
<span data-ttu-id="8d2b4-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8d2b4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8d2b4-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8d2b4-111">Permission type</span></span>|<span data-ttu-id="8d2b4-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8d2b4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8d2b4-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8d2b4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8d2b4-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="8d2b4-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="8d2b4-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8d2b4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8d2b4-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8d2b4-116">Not supported.</span></span>|
|<span data-ttu-id="8d2b4-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8d2b4-117">Application</span></span>|<span data-ttu-id="8d2b4-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8d2b4-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8d2b4-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8d2b4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicyDeviceStateSummary
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8d2b4-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="8d2b4-120">Optional query parameters</span></span>
<span data-ttu-id="8d2b4-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="8d2b4-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="8d2b4-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8d2b4-122">Request headers</span></span>
|<span data-ttu-id="8d2b4-123">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="8d2b4-123">Header</span></span>|<span data-ttu-id="8d2b4-124">Wert</span><span class="sxs-lookup"><span data-stu-id="8d2b4-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8d2b4-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="8d2b4-125">Authorization</span></span>|<span data-ttu-id="8d2b4-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="8d2b4-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8d2b4-127">Accept</span><span class="sxs-lookup"><span data-stu-id="8d2b4-127">Accept</span></span>|<span data-ttu-id="8d2b4-128">application/json</span><span class="sxs-lookup"><span data-stu-id="8d2b4-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8d2b4-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8d2b4-129">Request body</span></span>
<span data-ttu-id="8d2b4-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="8d2b4-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8d2b4-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="8d2b4-131">Response</span></span>
<span data-ttu-id="8d2b4-132">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8d2b4-132">If successful, this method returns a `200 OK` response code and [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8d2b4-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8d2b4-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="8d2b4-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8d2b4-134">Request</span></span>
<span data-ttu-id="8d2b4-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8d2b4-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicyDeviceStateSummary
```

### <a name="response"></a><span data-ttu-id="8d2b4-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="8d2b4-136">Response</span></span>
<span data-ttu-id="8d2b4-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8d2b4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





