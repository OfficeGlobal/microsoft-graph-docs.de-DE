---
title: resourceOperation abrufen
description: Liest die Eigenschaften und Beziehungen von Objekten des Typs resourceOperation.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8a312766fb1d81c82ab7d4a94915089f5ae97797
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30978647"
---
# <a name="get-resourceoperation"></a><span data-ttu-id="c6917-103">resourceOperation abrufen</span><span class="sxs-lookup"><span data-stu-id="c6917-103">Get resourceOperation</span></span>

> <span data-ttu-id="c6917-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="c6917-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c6917-105">Liest die Eigenschaften und Beziehungen von Objekten des Typs [resourceOperation](../resources/intune-rbac-resourceoperation.md).</span><span class="sxs-lookup"><span data-stu-id="c6917-105">Read properties and relationships of the [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c6917-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c6917-106">Prerequisites</span></span>
<span data-ttu-id="c6917-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c6917-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c6917-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c6917-109">Permission type</span></span>|<span data-ttu-id="c6917-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c6917-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c6917-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c6917-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c6917-112">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="c6917-112">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="c6917-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c6917-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c6917-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c6917-114">Not supported.</span></span>|
|<span data-ttu-id="c6917-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c6917-115">Application</span></span>|<span data-ttu-id="c6917-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c6917-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c6917-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c6917-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/resourceOperations/{resourceOperationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c6917-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="c6917-118">Optional query parameters</span></span>
<span data-ttu-id="c6917-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="c6917-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c6917-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c6917-120">Request headers</span></span>
|<span data-ttu-id="c6917-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="c6917-121">Header</span></span>|<span data-ttu-id="c6917-122">Wert</span><span class="sxs-lookup"><span data-stu-id="c6917-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c6917-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c6917-123">Authorization</span></span>|<span data-ttu-id="c6917-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c6917-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c6917-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="c6917-125">Accept</span></span>|<span data-ttu-id="c6917-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c6917-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c6917-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c6917-127">Request body</span></span>
<span data-ttu-id="c6917-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="c6917-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c6917-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="c6917-129">Response</span></span>
<span data-ttu-id="c6917-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [resourceOperation](../resources/intune-rbac-resourceoperation.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c6917-130">If successful, this method returns a `200 OK` response code and [resourceOperation](../resources/intune-rbac-resourceoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c6917-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c6917-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="c6917-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c6917-132">Request</span></span>
<span data-ttu-id="c6917-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c6917-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/resourceOperations/{resourceOperationId}
```

### <a name="response"></a><span data-ttu-id="c6917-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="c6917-134">Response</span></span>
<span data-ttu-id="c6917-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c6917-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 256

{
  "value": {
    "@odata.type": "#microsoft.graph.resourceOperation",
    "id": "232b8fee-8fee-232b-ee8f-2b23ee8f2b23",
    "resourceName": "Resource Name value",
    "actionName": "Action Name value",
    "description": "Description value"
  }
}
```



