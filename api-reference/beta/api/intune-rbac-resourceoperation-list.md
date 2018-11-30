---
title: resourceOperations auflisten
description: Listet die Eigenschaften und Beziehungen von Objekten des Typs resourceOperation auf.
ms.openlocfilehash: 7110a16e2713e950d5018d4904272feddbd56dec
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062357"
---
# <a name="list-resourceoperations"></a><span data-ttu-id="04b41-103">resourceOperations auflisten</span><span class="sxs-lookup"><span data-stu-id="04b41-103">List resourceOperations</span></span>

> <span data-ttu-id="04b41-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="04b41-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="04b41-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="04b41-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="04b41-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="04b41-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="04b41-107">Listet die Eigenschaften und Beziehungen von Objekten des Typs [resourceOperation](../resources/intune-rbac-resourceoperation.md) auf.</span><span class="sxs-lookup"><span data-stu-id="04b41-107">List properties and relationships of the [resourceOperation](../resources/intune-rbac-resourceoperation.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="04b41-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="04b41-108">Prerequisites</span></span>
<span data-ttu-id="04b41-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="04b41-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="04b41-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="04b41-111">Permission type</span></span>|<span data-ttu-id="04b41-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="04b41-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="04b41-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="04b41-113">Delegated (work or school account)</span></span>|<span data-ttu-id="04b41-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="04b41-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="04b41-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="04b41-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="04b41-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="04b41-116">Not supported.</span></span>|
|<span data-ttu-id="04b41-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="04b41-117">Application</span></span>|<span data-ttu-id="04b41-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="04b41-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="04b41-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="04b41-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/resourceOperations
```

## <a name="request-headers"></a><span data-ttu-id="04b41-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="04b41-120">Request headers</span></span>
|<span data-ttu-id="04b41-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="04b41-121">Header</span></span>|<span data-ttu-id="04b41-122">Wert</span><span class="sxs-lookup"><span data-stu-id="04b41-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="04b41-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="04b41-123">Authorization</span></span>|<span data-ttu-id="04b41-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="04b41-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="04b41-125">Accept</span><span class="sxs-lookup"><span data-stu-id="04b41-125">Accept</span></span>|<span data-ttu-id="04b41-126">application/json</span><span class="sxs-lookup"><span data-stu-id="04b41-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="04b41-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="04b41-127">Request body</span></span>
<span data-ttu-id="04b41-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="04b41-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="04b41-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="04b41-129">Response</span></span>
<span data-ttu-id="04b41-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [resourceOperation](../resources/intune-rbac-resourceoperation.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="04b41-130">If successful, this method returns a `200 OK` response code and a collection of [resourceOperation](../resources/intune-rbac-resourceoperation.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="04b41-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="04b41-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="04b41-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="04b41-132">Request</span></span>
<span data-ttu-id="04b41-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="04b41-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/resourceOperations
```

### <a name="response"></a><span data-ttu-id="04b41-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="04b41-134">Response</span></span>
<span data-ttu-id="04b41-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="04b41-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 359

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.resourceOperation",
      "id": "232b8fee-8fee-232b-ee8f-2b23ee8f2b23",
      "resource": "Resource value",
      "resourceName": "Resource Name value",
      "actionName": "Action Name value",
      "description": "Description value",
      "enabledForScopeValidation": true
    }
  ]
}
```





