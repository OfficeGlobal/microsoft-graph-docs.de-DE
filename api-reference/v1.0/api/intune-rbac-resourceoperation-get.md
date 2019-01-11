---
title: resourceOperation abrufen
description: Liest die Eigenschaften und Beziehungen von Objekten des Typs resourceOperation.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 97090b8a93a26d6e28689586602bb065bc7eaba6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27840621"
---
# <a name="get-resourceoperation"></a><span data-ttu-id="eb911-103">resourceOperation abrufen</span><span class="sxs-lookup"><span data-stu-id="eb911-103">Get resourceOperation</span></span>

> <span data-ttu-id="eb911-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="eb911-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="eb911-105">Liest die Eigenschaften und Beziehungen von Objekten des Typs [resourceOperation](../resources/intune-rbac-resourceoperation.md).</span><span class="sxs-lookup"><span data-stu-id="eb911-105">Read properties and relationships of the [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="eb911-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="eb911-106">Prerequisites</span></span>
<span data-ttu-id="eb911-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eb911-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eb911-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="eb911-109">Permission type</span></span>|<span data-ttu-id="eb911-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="eb911-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eb911-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="eb911-111">Delegated (work or school account)</span></span>|<span data-ttu-id="eb911-112">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="eb911-112">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="eb911-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="eb911-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eb911-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="eb911-114">Not supported.</span></span>|
|<span data-ttu-id="eb911-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="eb911-115">Application</span></span>|<span data-ttu-id="eb911-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="eb911-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="eb911-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="eb911-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/resourceOperations/{resourceOperationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="eb911-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="eb911-118">Optional query parameters</span></span>
<span data-ttu-id="eb911-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="eb911-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="eb911-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="eb911-120">Request headers</span></span>
|<span data-ttu-id="eb911-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="eb911-121">Header</span></span>|<span data-ttu-id="eb911-122">Wert</span><span class="sxs-lookup"><span data-stu-id="eb911-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eb911-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="eb911-123">Authorization</span></span>|<span data-ttu-id="eb911-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="eb911-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eb911-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="eb911-125">Accept</span></span>|<span data-ttu-id="eb911-126">application/json</span><span class="sxs-lookup"><span data-stu-id="eb911-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eb911-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="eb911-127">Request body</span></span>
<span data-ttu-id="eb911-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="eb911-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eb911-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="eb911-129">Response</span></span>
<span data-ttu-id="eb911-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [resourceOperation](../resources/intune-rbac-resourceoperation.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="eb911-130">If successful, this method returns a `200 OK` response code and [resourceOperation](../resources/intune-rbac-resourceoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eb911-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="eb911-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="eb911-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="eb911-132">Request</span></span>
<span data-ttu-id="eb911-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="eb911-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/resourceOperations/{resourceOperationId}
```

### <a name="response"></a><span data-ttu-id="eb911-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="eb911-134">Response</span></span>
<span data-ttu-id="eb911-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="eb911-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



