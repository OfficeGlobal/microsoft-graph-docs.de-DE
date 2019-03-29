---
title: ManagementCondition abrufen
description: Lesen von Eigenschaften und Beziehungen des managementCondition-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8c68e295baff14b165d2a3a736af25e8f1ba12ff
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30969463"
---
# <a name="get-managementcondition"></a><span data-ttu-id="77861-103">ManagementCondition abrufen</span><span class="sxs-lookup"><span data-stu-id="77861-103">Get managementCondition</span></span>

> <span data-ttu-id="77861-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="77861-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="77861-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="77861-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="77861-106">Lesen von Eigenschaften und Beziehungen des [managementCondition](../resources/intune-fencing-managementcondition.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="77861-106">Read properties and relationships of the [managementCondition](../resources/intune-fencing-managementcondition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="77861-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="77861-107">Prerequisites</span></span>
<span data-ttu-id="77861-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="77861-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="77861-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="77861-110">Permission type</span></span>|<span data-ttu-id="77861-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="77861-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="77861-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="77861-112">Delegated (work or school account)</span></span>|<span data-ttu-id="77861-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="77861-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="77861-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="77861-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="77861-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="77861-115">Not supported.</span></span>|
|<span data-ttu-id="77861-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="77861-116">Application</span></span>|<span data-ttu-id="77861-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="77861-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="77861-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="77861-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managementConditions/{managementConditionId}
GET /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions/{managementConditionId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="77861-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="77861-119">Optional query parameters</span></span>
<span data-ttu-id="77861-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="77861-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="77861-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="77861-121">Request headers</span></span>
|<span data-ttu-id="77861-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="77861-122">Header</span></span>|<span data-ttu-id="77861-123">Wert</span><span class="sxs-lookup"><span data-stu-id="77861-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="77861-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="77861-124">Authorization</span></span>|<span data-ttu-id="77861-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="77861-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="77861-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="77861-126">Accept</span></span>|<span data-ttu-id="77861-127">application/json</span><span class="sxs-lookup"><span data-stu-id="77861-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="77861-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="77861-128">Request body</span></span>
<span data-ttu-id="77861-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="77861-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="77861-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="77861-130">Response</span></span>
<span data-ttu-id="77861-131">Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und das [managementCondition](../resources/intune-fencing-managementcondition.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="77861-131">If successful, this method returns a `200 OK` response code and [managementCondition](../resources/intune-fencing-managementcondition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="77861-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="77861-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="77861-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="77861-133">Request</span></span>
<span data-ttu-id="77861-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="77861-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managementConditions/{managementConditionId}
```

### <a name="response"></a><span data-ttu-id="77861-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="77861-135">Response</span></span>
<span data-ttu-id="77861-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="77861-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 468

{
  "value": {
    "@odata.type": "#microsoft.graph.managementCondition",
    "id": "5cb49381-9381-5cb4-8193-b45c8193b45c",
    "uniqueName": "Unique Name value",
    "displayName": "Display Name value",
    "description": "Description value",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
    "eTag": "ETag value",
    "applicablePlatforms": [
      "androidForWork"
    ]
  }
}
```




