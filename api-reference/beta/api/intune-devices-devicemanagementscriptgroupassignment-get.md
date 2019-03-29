---
title: DeviceManagementScriptGroupAssignment abrufen
description: Lesen von Eigenschaften und Beziehungen des deviceManagementScriptGroupAssignment-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 76496e2e861e00a559a090985eef88530a03142f
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30958256"
---
# <a name="get-devicemanagementscriptgroupassignment"></a><span data-ttu-id="fbf9a-103">DeviceManagementScriptGroupAssignment abrufen</span><span class="sxs-lookup"><span data-stu-id="fbf9a-103">Get deviceManagementScriptGroupAssignment</span></span>

> <span data-ttu-id="fbf9a-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="fbf9a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fbf9a-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="fbf9a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fbf9a-106">Lesen von Eigenschaften und Beziehungen des [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="fbf9a-106">Read properties and relationships of the [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fbf9a-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="fbf9a-107">Prerequisites</span></span>
<span data-ttu-id="fbf9a-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fbf9a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fbf9a-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="fbf9a-110">Permission type</span></span>|<span data-ttu-id="fbf9a-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="fbf9a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fbf9a-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="fbf9a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fbf9a-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="fbf9a-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="fbf9a-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="fbf9a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fbf9a-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fbf9a-115">Not supported.</span></span>|
|<span data-ttu-id="fbf9a-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="fbf9a-116">Application</span></span>|<span data-ttu-id="fbf9a-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fbf9a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fbf9a-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="fbf9a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/groupAssignments/{deviceManagementScriptGroupAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fbf9a-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="fbf9a-119">Optional query parameters</span></span>
<span data-ttu-id="fbf9a-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="fbf9a-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fbf9a-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="fbf9a-121">Request headers</span></span>
|<span data-ttu-id="fbf9a-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="fbf9a-122">Header</span></span>|<span data-ttu-id="fbf9a-123">Wert</span><span class="sxs-lookup"><span data-stu-id="fbf9a-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fbf9a-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="fbf9a-124">Authorization</span></span>|<span data-ttu-id="fbf9a-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="fbf9a-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fbf9a-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="fbf9a-126">Accept</span></span>|<span data-ttu-id="fbf9a-127">application/json</span><span class="sxs-lookup"><span data-stu-id="fbf9a-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fbf9a-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="fbf9a-128">Request body</span></span>
<span data-ttu-id="fbf9a-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="fbf9a-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fbf9a-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="fbf9a-130">Response</span></span>
<span data-ttu-id="fbf9a-131">Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und das [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="fbf9a-131">If successful, this method returns a `200 OK` response code and [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fbf9a-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="fbf9a-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="fbf9a-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="fbf9a-133">Request</span></span>
<span data-ttu-id="fbf9a-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="fbf9a-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/groupAssignments/{deviceManagementScriptGroupAssignmentId}
```

### <a name="response"></a><span data-ttu-id="fbf9a-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="fbf9a-135">Response</span></span>
<span data-ttu-id="fbf9a-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fbf9a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 198

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementScriptGroupAssignment",
    "id": "ecd2357d-357d-ecd2-7d35-d2ec7d35d2ec",
    "targetGroupId": "Target Group Id value"
  }
}
```




