---
title: resourceOperations auflisten
description: Listet die Eigenschaften und Beziehungen von Objekten des Typs resourceOperation auf.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: de7a4abbc9d08cadc0b5f8c213730d166b8bbdfa
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30263427"
---
# <a name="list-resourceoperations"></a><span data-ttu-id="40be6-103">resourceOperations auflisten</span><span class="sxs-lookup"><span data-stu-id="40be6-103">List resourceOperations</span></span>

> <span data-ttu-id="40be6-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="40be6-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="40be6-105">Listet die Eigenschaften und Beziehungen von Objekten des Typs [resourceOperation](../resources/intune-rbac-resourceoperation.md) auf.</span><span class="sxs-lookup"><span data-stu-id="40be6-105">List properties and relationships of the [resourceOperation](../resources/intune-rbac-resourceoperation.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="40be6-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="40be6-106">Prerequisites</span></span>
<span data-ttu-id="40be6-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="40be6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="40be6-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="40be6-109">Permission type</span></span>|<span data-ttu-id="40be6-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="40be6-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="40be6-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="40be6-111">Delegated (work or school account)</span></span>|<span data-ttu-id="40be6-112">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="40be6-112">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="40be6-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="40be6-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="40be6-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="40be6-114">Not supported.</span></span>|
|<span data-ttu-id="40be6-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="40be6-115">Application</span></span>|<span data-ttu-id="40be6-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="40be6-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="40be6-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="40be6-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/resourceOperations
```

## <a name="request-headers"></a><span data-ttu-id="40be6-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="40be6-118">Request headers</span></span>
|<span data-ttu-id="40be6-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="40be6-119">Header</span></span>|<span data-ttu-id="40be6-120">Wert</span><span class="sxs-lookup"><span data-stu-id="40be6-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="40be6-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="40be6-121">Authorization</span></span>|<span data-ttu-id="40be6-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="40be6-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="40be6-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="40be6-123">Accept</span></span>|<span data-ttu-id="40be6-124">application/json</span><span class="sxs-lookup"><span data-stu-id="40be6-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="40be6-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="40be6-125">Request body</span></span>
<span data-ttu-id="40be6-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="40be6-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="40be6-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="40be6-127">Response</span></span>
<span data-ttu-id="40be6-128">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [resourceOperation](../resources/intune-rbac-resourceoperation.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="40be6-128">If successful, this method returns a `200 OK` response code and a collection of [resourceOperation](../resources/intune-rbac-resourceoperation.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="40be6-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="40be6-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="40be6-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="40be6-130">Request</span></span>
<span data-ttu-id="40be6-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="40be6-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/resourceOperations
```

### <a name="response"></a><span data-ttu-id="40be6-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="40be6-132">Response</span></span>
<span data-ttu-id="40be6-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="40be6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 280

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.resourceOperation",
      "id": "232b8fee-8fee-232b-ee8f-2b23ee8f2b23",
      "resourceName": "Resource Name value",
      "actionName": "Action Name value",
      "description": "Description value"
    }
  ]
}
```



