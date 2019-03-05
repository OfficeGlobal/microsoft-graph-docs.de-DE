---
title: resourceOperation abrufen
description: Liest die Eigenschaften und Beziehungen von Objekten des Typs resourceOperation.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2231990e4d82e96af495960a2df53a65f8ef6fcf
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30252021"
---
# <a name="get-resourceoperation"></a><span data-ttu-id="5bf6e-103">resourceOperation abrufen</span><span class="sxs-lookup"><span data-stu-id="5bf6e-103">Get resourceOperation</span></span>

> <span data-ttu-id="5bf6e-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="5bf6e-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5bf6e-105">Liest die Eigenschaften und Beziehungen von Objekten des Typs [resourceOperation](../resources/intune-rbac-resourceoperation.md).</span><span class="sxs-lookup"><span data-stu-id="5bf6e-105">Read properties and relationships of the [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5bf6e-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="5bf6e-106">Prerequisites</span></span>
<span data-ttu-id="5bf6e-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="5bf6e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="5bf6e-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5bf6e-109">Permission type</span></span>|<span data-ttu-id="5bf6e-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5bf6e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5bf6e-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5bf6e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5bf6e-112">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="5bf6e-112">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="5bf6e-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5bf6e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5bf6e-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5bf6e-114">Not supported.</span></span>|
|<span data-ttu-id="5bf6e-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5bf6e-115">Application</span></span>|<span data-ttu-id="5bf6e-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5bf6e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5bf6e-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5bf6e-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/resourceOperations/{resourceOperationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5bf6e-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="5bf6e-118">Optional query parameters</span></span>
<span data-ttu-id="5bf6e-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="5bf6e-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5bf6e-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5bf6e-120">Request headers</span></span>
|<span data-ttu-id="5bf6e-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="5bf6e-121">Header</span></span>|<span data-ttu-id="5bf6e-122">Wert</span><span class="sxs-lookup"><span data-stu-id="5bf6e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5bf6e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5bf6e-123">Authorization</span></span>|<span data-ttu-id="5bf6e-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="5bf6e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5bf6e-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="5bf6e-125">Accept</span></span>|<span data-ttu-id="5bf6e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5bf6e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5bf6e-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5bf6e-127">Request body</span></span>
<span data-ttu-id="5bf6e-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="5bf6e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5bf6e-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="5bf6e-129">Response</span></span>
<span data-ttu-id="5bf6e-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [resourceOperation](../resources/intune-rbac-resourceoperation.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5bf6e-130">If successful, this method returns a `200 OK` response code and [resourceOperation](../resources/intune-rbac-resourceoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5bf6e-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5bf6e-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="5bf6e-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5bf6e-132">Request</span></span>
<span data-ttu-id="5bf6e-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5bf6e-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/resourceOperations/{resourceOperationId}
```

### <a name="response"></a><span data-ttu-id="5bf6e-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="5bf6e-134">Response</span></span>
<span data-ttu-id="5bf6e-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5bf6e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



