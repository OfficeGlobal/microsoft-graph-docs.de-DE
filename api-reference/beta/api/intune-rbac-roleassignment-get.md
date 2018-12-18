---
title: Abrufen von „roleAssignment“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs roleAssignment.
author: tfitzmac
ms.openlocfilehash: 73b06e6a3a2105edadcfae0799413ae9baa8bc2c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27354432"
---
# <a name="get-roleassignment"></a><span data-ttu-id="87c08-103">Abrufen von „roleAssignment“</span><span class="sxs-lookup"><span data-stu-id="87c08-103">Get roleAssignment</span></span>

> <span data-ttu-id="87c08-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="87c08-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="87c08-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="87c08-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="87c08-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="87c08-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="87c08-107">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="87c08-107">Read properties and relationships of the [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="87c08-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="87c08-108">Prerequisites</span></span>
<span data-ttu-id="87c08-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="87c08-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="87c08-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="87c08-111">Permission type</span></span>|<span data-ttu-id="87c08-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="87c08-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="87c08-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="87c08-113">Delegated (work or school account)</span></span>|<span data-ttu-id="87c08-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="87c08-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="87c08-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="87c08-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="87c08-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="87c08-116">Not supported.</span></span>|
|<span data-ttu-id="87c08-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="87c08-117">Application</span></span>|<span data-ttu-id="87c08-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="87c08-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="87c08-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="87c08-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="87c08-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="87c08-120">Optional query parameters</span></span>
<span data-ttu-id="87c08-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="87c08-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="87c08-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="87c08-122">Request headers</span></span>
|<span data-ttu-id="87c08-123">Header</span><span class="sxs-lookup"><span data-stu-id="87c08-123">Header</span></span>|<span data-ttu-id="87c08-124">Wert</span><span class="sxs-lookup"><span data-stu-id="87c08-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="87c08-125">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="87c08-125">Authorization</span></span>|<span data-ttu-id="87c08-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="87c08-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="87c08-127">Accept</span><span class="sxs-lookup"><span data-stu-id="87c08-127">Accept</span></span>|<span data-ttu-id="87c08-128">application/json</span><span class="sxs-lookup"><span data-stu-id="87c08-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="87c08-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="87c08-129">Request body</span></span>
<span data-ttu-id="87c08-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="87c08-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="87c08-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="87c08-131">Response</span></span>
<span data-ttu-id="87c08-132">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [roleAssignment](../resources/intune-rbac-roleassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="87c08-132">If successful, this method returns a `200 OK` response code and [roleAssignment](../resources/intune-rbac-roleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="87c08-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="87c08-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="87c08-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="87c08-134">Request</span></span>
<span data-ttu-id="87c08-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="87c08-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}
```

### <a name="response"></a><span data-ttu-id="87c08-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="87c08-136">Response</span></span>
<span data-ttu-id="87c08-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="87c08-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 367

{
  "value": {
    "@odata.type": "#microsoft.graph.roleAssignment",
    "id": "b3234d24-4d24-b323-244d-23b3244d23b3",
    "displayName": "Display Name value",
    "description": "Description value",
    "scopeMembers": [
      "Scope Members value"
    ],
    "scopeType": "allDevices",
    "resourceScopes": [
      "Resource Scopes value"
    ]
  }
}
```





