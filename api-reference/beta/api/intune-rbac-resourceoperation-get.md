---
title: resourceOperation abrufen
description: Liest die Eigenschaften und Beziehungen von Objekten des Typs resourceOperation.
author: tfitzmac
ms.openlocfilehash: 15aaa29f5a3563129722bf5c3ad7f14efa2fd655
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27317290"
---
# <a name="get-resourceoperation"></a><span data-ttu-id="9f94b-103">resourceOperation abrufen</span><span class="sxs-lookup"><span data-stu-id="9f94b-103">Get resourceOperation</span></span>

> <span data-ttu-id="9f94b-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="9f94b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9f94b-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9f94b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9f94b-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="9f94b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9f94b-107">Liest die Eigenschaften und Beziehungen von Objekten des Typs [resourceOperation](../resources/intune-rbac-resourceoperation.md).</span><span class="sxs-lookup"><span data-stu-id="9f94b-107">Read properties and relationships of the [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9f94b-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="9f94b-108">Prerequisites</span></span>
<span data-ttu-id="9f94b-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9f94b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9f94b-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9f94b-111">Permission type</span></span>|<span data-ttu-id="9f94b-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9f94b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9f94b-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9f94b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9f94b-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="9f94b-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="9f94b-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9f94b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9f94b-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9f94b-116">Not supported.</span></span>|
|<span data-ttu-id="9f94b-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9f94b-117">Application</span></span>|<span data-ttu-id="9f94b-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9f94b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9f94b-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9f94b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/resourceOperations/{resourceOperationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9f94b-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="9f94b-120">Optional query parameters</span></span>
<span data-ttu-id="9f94b-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="9f94b-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="9f94b-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9f94b-122">Request headers</span></span>
|<span data-ttu-id="9f94b-123">Header</span><span class="sxs-lookup"><span data-stu-id="9f94b-123">Header</span></span>|<span data-ttu-id="9f94b-124">Wert</span><span class="sxs-lookup"><span data-stu-id="9f94b-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9f94b-125">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="9f94b-125">Authorization</span></span>|<span data-ttu-id="9f94b-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="9f94b-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9f94b-127">Accept</span><span class="sxs-lookup"><span data-stu-id="9f94b-127">Accept</span></span>|<span data-ttu-id="9f94b-128">application/json</span><span class="sxs-lookup"><span data-stu-id="9f94b-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9f94b-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9f94b-129">Request body</span></span>
<span data-ttu-id="9f94b-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="9f94b-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9f94b-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="9f94b-131">Response</span></span>
<span data-ttu-id="9f94b-132">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [resourceOperation](../resources/intune-rbac-resourceoperation.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9f94b-132">If successful, this method returns a `200 OK` response code and [resourceOperation](../resources/intune-rbac-resourceoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9f94b-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9f94b-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="9f94b-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9f94b-134">Request</span></span>
<span data-ttu-id="9f94b-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9f94b-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/resourceOperations/{resourceOperationId}
```

### <a name="response"></a><span data-ttu-id="9f94b-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="9f94b-136">Response</span></span>
<span data-ttu-id="9f94b-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9f94b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 331

{
  "value": {
    "@odata.type": "#microsoft.graph.resourceOperation",
    "id": "232b8fee-8fee-232b-ee8f-2b23ee8f2b23",
    "resource": "Resource value",
    "resourceName": "Resource Name value",
    "actionName": "Action Name value",
    "description": "Description value",
    "enabledForScopeValidation": true
  }
}
```





