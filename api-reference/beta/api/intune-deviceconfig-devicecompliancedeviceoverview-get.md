---
title: deviceComplianceDeviceOverview abrufen
description: Lesen von Eigenschaften und Beziehungen des deviceComplianceDeviceOverview-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 55fbce5619b1283207bacf5182de7d2c2c6eb896
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27979187"
---
# <a name="get-devicecompliancedeviceoverview"></a><span data-ttu-id="9b27b-103">deviceComplianceDeviceOverview abrufen</span><span class="sxs-lookup"><span data-stu-id="9b27b-103">Get deviceComplianceDeviceOverview</span></span>

> <span data-ttu-id="9b27b-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="9b27b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9b27b-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9b27b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9b27b-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="9b27b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9b27b-107">Lesen von Eigenschaften und Beziehungen des [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="9b27b-107">Read properties and relationships of the [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9b27b-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="9b27b-108">Prerequisites</span></span>
<span data-ttu-id="9b27b-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9b27b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9b27b-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9b27b-111">Permission type</span></span>|<span data-ttu-id="9b27b-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9b27b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9b27b-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9b27b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9b27b-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="9b27b-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="9b27b-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9b27b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9b27b-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9b27b-116">Not supported.</span></span>|
|<span data-ttu-id="9b27b-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9b27b-117">Application</span></span>|<span data-ttu-id="9b27b-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9b27b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9b27b-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9b27b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatusOverview
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9b27b-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="9b27b-120">Optional query parameters</span></span>
<span data-ttu-id="9b27b-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="9b27b-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="9b27b-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9b27b-122">Request headers</span></span>
|<span data-ttu-id="9b27b-123">Header</span><span class="sxs-lookup"><span data-stu-id="9b27b-123">Header</span></span>|<span data-ttu-id="9b27b-124">Wert</span><span class="sxs-lookup"><span data-stu-id="9b27b-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9b27b-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="9b27b-125">Authorization</span></span>|<span data-ttu-id="9b27b-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="9b27b-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9b27b-127">Annehmen</span><span class="sxs-lookup"><span data-stu-id="9b27b-127">Accept</span></span>|<span data-ttu-id="9b27b-128">application/json</span><span class="sxs-lookup"><span data-stu-id="9b27b-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9b27b-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9b27b-129">Request body</span></span>
<span data-ttu-id="9b27b-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="9b27b-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9b27b-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="9b27b-131">Response</span></span>
<span data-ttu-id="9b27b-132">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9b27b-132">If successful, this method returns a `200 OK` response code and [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9b27b-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9b27b-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="9b27b-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9b27b-134">Request</span></span>
<span data-ttu-id="9b27b-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9b27b-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatusOverview
```

### <a name="response"></a><span data-ttu-id="9b27b-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="9b27b-136">Response</span></span>
<span data-ttu-id="9b27b-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9b27b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 432

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceComplianceDeviceOverview",
    "id": "886f167b-167b-886f-7b16-6f887b166f88",
    "pendingCount": 12,
    "notApplicableCount": 2,
    "notApplicablePlatformCount": 10,
    "successCount": 12,
    "errorCount": 10,
    "failedCount": 11,
    "conflictCount": 13,
    "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
    "configurationVersion": 4
  }
}
```





