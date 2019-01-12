---
title: deviceAndAppManagementRoleAssignment abrufen
description: Lesen von Eigenschaften und Beziehungen des deviceAndAppManagementRoleAssignment-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8e16bbb45d9d391df9921281cd5739e6ccf4a7d2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27947981"
---
# <a name="get-deviceandappmanagementroleassignment"></a><span data-ttu-id="d9ab1-103">deviceAndAppManagementRoleAssignment abrufen</span><span class="sxs-lookup"><span data-stu-id="d9ab1-103">Get deviceAndAppManagementRoleAssignment</span></span>

> <span data-ttu-id="d9ab1-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="d9ab1-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d9ab1-105">Lesen von Eigenschaften und Beziehungen des [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="d9ab1-105">Read properties and relationships of the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d9ab1-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="d9ab1-106">Prerequisites</span></span>
<span data-ttu-id="d9ab1-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d9ab1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d9ab1-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d9ab1-109">Permission type</span></span>|<span data-ttu-id="d9ab1-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d9ab1-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d9ab1-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d9ab1-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d9ab1-112">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="d9ab1-112">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="d9ab1-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d9ab1-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d9ab1-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d9ab1-114">Not supported.</span></span>|
|<span data-ttu-id="d9ab1-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d9ab1-115">Application</span></span>|<span data-ttu-id="d9ab1-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d9ab1-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d9ab1-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d9ab1-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleAssignments/{deviceAndAppManagementRoleAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d9ab1-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="d9ab1-118">Optional query parameters</span></span>
<span data-ttu-id="d9ab1-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="d9ab1-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="d9ab1-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d9ab1-120">Request headers</span></span>
|<span data-ttu-id="d9ab1-121">Header</span><span class="sxs-lookup"><span data-stu-id="d9ab1-121">Header</span></span>|<span data-ttu-id="d9ab1-122">Wert</span><span class="sxs-lookup"><span data-stu-id="d9ab1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d9ab1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d9ab1-123">Authorization</span></span>|<span data-ttu-id="d9ab1-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="d9ab1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d9ab1-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="d9ab1-125">Accept</span></span>|<span data-ttu-id="d9ab1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d9ab1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d9ab1-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d9ab1-127">Request body</span></span>
<span data-ttu-id="d9ab1-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="d9ab1-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d9ab1-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="d9ab1-129">Response</span></span>
<span data-ttu-id="d9ab1-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="d9ab1-130">If successful, this method returns a `200 OK` response code and [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d9ab1-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d9ab1-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="d9ab1-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d9ab1-132">Request</span></span>
<span data-ttu-id="d9ab1-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d9ab1-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/roleAssignments/{deviceAndAppManagementRoleAssignmentId}
```

### <a name="response"></a><span data-ttu-id="d9ab1-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="d9ab1-134">Response</span></span>
<span data-ttu-id="d9ab1-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d9ab1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 346

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleAssignment",
    "id": "a12e8ebb-8ebb-a12e-bb8e-2ea1bb8e2ea1",
    "displayName": "Display Name value",
    "description": "Description value",
    "resourceScopes": [
      "Resource Scopes value"
    ],
    "members": [
      "Members value"
    ]
  }
}
```



