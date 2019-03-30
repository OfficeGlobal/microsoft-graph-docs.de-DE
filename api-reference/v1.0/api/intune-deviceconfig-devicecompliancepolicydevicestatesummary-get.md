---
title: deviceCompliancePolicyDeviceStateSummary abrufen
description: Lesen von Beziehungen und Eigenschaften des deviceCompliancePolicyDeviceStateSummary-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1d04a543079db2e33d774eca17ed288292ebf3ab
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30968126"
---
# <a name="get-devicecompliancepolicydevicestatesummary"></a><span data-ttu-id="429ca-103">deviceCompliancePolicyDeviceStateSummary abrufen</span><span class="sxs-lookup"><span data-stu-id="429ca-103">Get deviceCompliancePolicyDeviceStateSummary</span></span>

> <span data-ttu-id="429ca-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="429ca-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="429ca-105">Lesen von Beziehungen und Eigenschaften des [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="429ca-105">Read properties and relationships of the [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="429ca-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="429ca-106">Prerequisites</span></span>
<span data-ttu-id="429ca-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="429ca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="429ca-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="429ca-109">Permission type</span></span>|<span data-ttu-id="429ca-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="429ca-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="429ca-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="429ca-111">Delegated (work or school account)</span></span>|<span data-ttu-id="429ca-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="429ca-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="429ca-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="429ca-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="429ca-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="429ca-114">Not supported.</span></span>|
|<span data-ttu-id="429ca-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="429ca-115">Application</span></span>|<span data-ttu-id="429ca-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="429ca-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="429ca-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="429ca-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicyDeviceStateSummary
```

## <a name="optional-query-parameters"></a><span data-ttu-id="429ca-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="429ca-118">Optional query parameters</span></span>
<span data-ttu-id="429ca-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="429ca-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="429ca-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="429ca-120">Request headers</span></span>
|<span data-ttu-id="429ca-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="429ca-121">Header</span></span>|<span data-ttu-id="429ca-122">Wert</span><span class="sxs-lookup"><span data-stu-id="429ca-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="429ca-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="429ca-123">Authorization</span></span>|<span data-ttu-id="429ca-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="429ca-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="429ca-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="429ca-125">Accept</span></span>|<span data-ttu-id="429ca-126">application/json</span><span class="sxs-lookup"><span data-stu-id="429ca-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="429ca-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="429ca-127">Request body</span></span>
<span data-ttu-id="429ca-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="429ca-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="429ca-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="429ca-129">Response</span></span>
<span data-ttu-id="429ca-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="429ca-130">If successful, this method returns a `200 OK` response code and [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="429ca-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="429ca-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="429ca-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="429ca-132">Request</span></span>
<span data-ttu-id="429ca-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="429ca-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicyDeviceStateSummary
```

### <a name="response"></a><span data-ttu-id="429ca-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="429ca-134">Response</span></span>
<span data-ttu-id="429ca-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="429ca-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



