---
title: deviceAndAppManagementRoleAssignment abrufen
description: Lesen von Eigenschaften und Beziehungen des deviceAndAppManagementRoleAssignment-Objekts.
ms.openlocfilehash: 9791019c586b322c96506059ab36bc7c6705c980
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017656"
---
# <a name="get-deviceandappmanagementroleassignment"></a><span data-ttu-id="ed016-103">deviceAndAppManagementRoleAssignment abrufen</span><span class="sxs-lookup"><span data-stu-id="ed016-103">Get deviceAndAppManagementRoleAssignment</span></span>

> <span data-ttu-id="ed016-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="ed016-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ed016-105">Lesen von Eigenschaften und Beziehungen des [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="ed016-105">Read properties and relationships of the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ed016-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="ed016-106">Prerequisites</span></span>
<span data-ttu-id="ed016-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ed016-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ed016-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ed016-109">Permission type</span></span>|<span data-ttu-id="ed016-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ed016-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ed016-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ed016-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ed016-112">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="ed016-112">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="ed016-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ed016-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ed016-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ed016-114">Not supported.</span></span>|
|<span data-ttu-id="ed016-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ed016-115">Application</span></span>|<span data-ttu-id="ed016-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ed016-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ed016-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ed016-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleAssignments/{deviceAndAppManagementRoleAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ed016-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="ed016-118">Optional query parameters</span></span>
<span data-ttu-id="ed016-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="ed016-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="ed016-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ed016-120">Request headers</span></span>
|<span data-ttu-id="ed016-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="ed016-121">Header</span></span>|<span data-ttu-id="ed016-122">Wert</span><span class="sxs-lookup"><span data-stu-id="ed016-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ed016-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ed016-123">Authorization</span></span>|<span data-ttu-id="ed016-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="ed016-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ed016-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ed016-125">Accept</span></span>|<span data-ttu-id="ed016-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ed016-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ed016-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ed016-127">Request body</span></span>
<span data-ttu-id="ed016-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="ed016-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ed016-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="ed016-129">Response</span></span>
<span data-ttu-id="ed016-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="ed016-130">If successful, this method returns a `200 OK` response code and [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ed016-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ed016-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="ed016-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ed016-132">Request</span></span>
<span data-ttu-id="ed016-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ed016-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/roleAssignments/{deviceAndAppManagementRoleAssignmentId}
```

### <a name="response"></a><span data-ttu-id="ed016-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="ed016-134">Response</span></span>
<span data-ttu-id="ed016-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ed016-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



