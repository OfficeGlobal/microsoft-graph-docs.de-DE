---
title: resourceOperations auflisten
description: Listet die Eigenschaften und Beziehungen von Objekten des Typs resourceOperation auf.
ms.openlocfilehash: 7d206eb9eaada3f3947591037fb5129c5662d580
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018604"
---
# <a name="list-resourceoperations"></a><span data-ttu-id="a9cb3-103">resourceOperations auflisten</span><span class="sxs-lookup"><span data-stu-id="a9cb3-103">List resourceOperations</span></span>

> <span data-ttu-id="a9cb3-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="a9cb3-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a9cb3-105">Listet die Eigenschaften und Beziehungen von Objekten des Typs [resourceOperation](../resources/intune-rbac-resourceoperation.md) auf.</span><span class="sxs-lookup"><span data-stu-id="a9cb3-105">List properties and relationships of the [resourceOperation](../resources/intune-rbac-resourceoperation.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a9cb3-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="a9cb3-106">Prerequisites</span></span>
<span data-ttu-id="a9cb3-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a9cb3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a9cb3-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a9cb3-109">Permission type</span></span>|<span data-ttu-id="a9cb3-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a9cb3-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a9cb3-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a9cb3-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a9cb3-112">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="a9cb3-112">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="a9cb3-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a9cb3-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a9cb3-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a9cb3-114">Not supported.</span></span>|
|<span data-ttu-id="a9cb3-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a9cb3-115">Application</span></span>|<span data-ttu-id="a9cb3-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a9cb3-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a9cb3-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a9cb3-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/resourceOperations
```

## <a name="request-headers"></a><span data-ttu-id="a9cb3-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a9cb3-118">Request headers</span></span>
|<span data-ttu-id="a9cb3-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="a9cb3-119">Header</span></span>|<span data-ttu-id="a9cb3-120">Wert</span><span class="sxs-lookup"><span data-stu-id="a9cb3-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a9cb3-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a9cb3-121">Authorization</span></span>|<span data-ttu-id="a9cb3-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="a9cb3-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a9cb3-123">Accept</span><span class="sxs-lookup"><span data-stu-id="a9cb3-123">Accept</span></span>|<span data-ttu-id="a9cb3-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a9cb3-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a9cb3-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a9cb3-125">Request body</span></span>
<span data-ttu-id="a9cb3-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="a9cb3-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a9cb3-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="a9cb3-127">Response</span></span>
<span data-ttu-id="a9cb3-128">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [resourceOperation](../resources/intune-rbac-resourceoperation.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a9cb3-128">If successful, this method returns a `200 OK` response code and a collection of [resourceOperation](../resources/intune-rbac-resourceoperation.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a9cb3-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a9cb3-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="a9cb3-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a9cb3-130">Request</span></span>
<span data-ttu-id="a9cb3-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a9cb3-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/resourceOperations
```

### <a name="response"></a><span data-ttu-id="a9cb3-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="a9cb3-132">Response</span></span>
<span data-ttu-id="a9cb3-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a9cb3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



