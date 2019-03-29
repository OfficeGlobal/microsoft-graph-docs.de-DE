---
title: deviceComplianceDeviceOverview abrufen
description: Lesen von Eigenschaften und Beziehungen des deviceComplianceDeviceOverview-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6819d575529343b0290e1a3518fe4f1781db1207
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30975427"
---
# <a name="get-devicecompliancedeviceoverview"></a><span data-ttu-id="157b6-103">deviceComplianceDeviceOverview abrufen</span><span class="sxs-lookup"><span data-stu-id="157b6-103">Get deviceComplianceDeviceOverview</span></span>

> <span data-ttu-id="157b6-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="157b6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="157b6-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="157b6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="157b6-106">Lesen von Eigenschaften und Beziehungen des [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="157b6-106">Read properties and relationships of the [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="157b6-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="157b6-107">Prerequisites</span></span>
<span data-ttu-id="157b6-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="157b6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="157b6-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="157b6-110">Permission type</span></span>|<span data-ttu-id="157b6-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="157b6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="157b6-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="157b6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="157b6-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="157b6-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="157b6-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="157b6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="157b6-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="157b6-115">Not supported.</span></span>|
|<span data-ttu-id="157b6-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="157b6-116">Application</span></span>|<span data-ttu-id="157b6-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="157b6-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="157b6-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="157b6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatusOverview
```

## <a name="optional-query-parameters"></a><span data-ttu-id="157b6-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="157b6-119">Optional query parameters</span></span>
<span data-ttu-id="157b6-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="157b6-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="157b6-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="157b6-121">Request headers</span></span>
|<span data-ttu-id="157b6-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="157b6-122">Header</span></span>|<span data-ttu-id="157b6-123">Wert</span><span class="sxs-lookup"><span data-stu-id="157b6-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="157b6-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="157b6-124">Authorization</span></span>|<span data-ttu-id="157b6-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="157b6-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="157b6-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="157b6-126">Accept</span></span>|<span data-ttu-id="157b6-127">application/json</span><span class="sxs-lookup"><span data-stu-id="157b6-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="157b6-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="157b6-128">Request body</span></span>
<span data-ttu-id="157b6-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="157b6-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="157b6-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="157b6-130">Response</span></span>
<span data-ttu-id="157b6-131">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="157b6-131">If successful, this method returns a `200 OK` response code and [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="157b6-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="157b6-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="157b6-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="157b6-133">Request</span></span>
<span data-ttu-id="157b6-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="157b6-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatusOverview
```

### <a name="response"></a><span data-ttu-id="157b6-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="157b6-135">Response</span></span>
<span data-ttu-id="157b6-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="157b6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




