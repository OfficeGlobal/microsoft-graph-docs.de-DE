---
title: deviceConfigurationDeviceOverview abrufen
description: Lesen von Eigenschaften und Beziehungen des deviceConfigurationDeviceOverview-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 966187ff9815559d62a94f5baf64702116e88b5a
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30258051"
---
# <a name="get-deviceconfigurationdeviceoverview"></a><span data-ttu-id="e89eb-103">deviceConfigurationDeviceOverview abrufen</span><span class="sxs-lookup"><span data-stu-id="e89eb-103">Get deviceConfigurationDeviceOverview</span></span>

> <span data-ttu-id="e89eb-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="e89eb-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e89eb-105">Lesen von Eigenschaften und Beziehungen des [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="e89eb-105">Read properties and relationships of the [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e89eb-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="e89eb-106">Prerequisites</span></span>
<span data-ttu-id="e89eb-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="e89eb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="e89eb-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e89eb-109">Permission type</span></span>|<span data-ttu-id="e89eb-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e89eb-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e89eb-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e89eb-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e89eb-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e89eb-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="e89eb-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e89eb-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e89eb-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e89eb-114">Not supported.</span></span>|
|<span data-ttu-id="e89eb-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e89eb-115">Application</span></span>|<span data-ttu-id="e89eb-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e89eb-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e89eb-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e89eb-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatusOverview
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e89eb-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="e89eb-118">Optional query parameters</span></span>
<span data-ttu-id="e89eb-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="e89eb-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e89eb-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e89eb-120">Request headers</span></span>
|<span data-ttu-id="e89eb-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="e89eb-121">Header</span></span>|<span data-ttu-id="e89eb-122">Wert</span><span class="sxs-lookup"><span data-stu-id="e89eb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e89eb-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e89eb-123">Authorization</span></span>|<span data-ttu-id="e89eb-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="e89eb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e89eb-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="e89eb-125">Accept</span></span>|<span data-ttu-id="e89eb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e89eb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e89eb-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e89eb-127">Request body</span></span>
<span data-ttu-id="e89eb-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="e89eb-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e89eb-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="e89eb-129">Response</span></span>
<span data-ttu-id="e89eb-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e89eb-130">If successful, this method returns a `200 OK` response code and [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e89eb-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e89eb-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="e89eb-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e89eb-132">Request</span></span>
<span data-ttu-id="e89eb-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e89eb-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatusOverview
```

### <a name="response"></a><span data-ttu-id="e89eb-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="e89eb-134">Response</span></span>
<span data-ttu-id="e89eb-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e89eb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 370

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceConfigurationDeviceOverview",
    "id": "62d48e3a-8e3a-62d4-3a8e-d4623a8ed462",
    "pendingCount": 12,
    "notApplicableCount": 2,
    "successCount": 12,
    "errorCount": 10,
    "failedCount": 11,
    "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
    "configurationVersion": 4
  }
}
```



