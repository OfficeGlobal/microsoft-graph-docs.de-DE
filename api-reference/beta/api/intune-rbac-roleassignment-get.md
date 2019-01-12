---
title: Abrufen von „roleAssignment“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs roleAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e3879e1f0817b6f4da1ccc939825160cd8ed1f00
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27938685"
---
# <a name="get-roleassignment"></a><span data-ttu-id="e7c02-103">Abrufen von „roleAssignment“</span><span class="sxs-lookup"><span data-stu-id="e7c02-103">Get roleAssignment</span></span>

> <span data-ttu-id="e7c02-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="e7c02-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e7c02-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e7c02-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e7c02-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="e7c02-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e7c02-107">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="e7c02-107">Read properties and relationships of the [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e7c02-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="e7c02-108">Prerequisites</span></span>
<span data-ttu-id="e7c02-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e7c02-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e7c02-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e7c02-111">Permission type</span></span>|<span data-ttu-id="e7c02-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e7c02-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e7c02-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e7c02-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e7c02-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="e7c02-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="e7c02-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e7c02-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e7c02-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e7c02-116">Not supported.</span></span>|
|<span data-ttu-id="e7c02-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e7c02-117">Application</span></span>|<span data-ttu-id="e7c02-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e7c02-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e7c02-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e7c02-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e7c02-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="e7c02-120">Optional query parameters</span></span>
<span data-ttu-id="e7c02-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="e7c02-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="e7c02-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e7c02-122">Request headers</span></span>
|<span data-ttu-id="e7c02-123">Header</span><span class="sxs-lookup"><span data-stu-id="e7c02-123">Header</span></span>|<span data-ttu-id="e7c02-124">Wert</span><span class="sxs-lookup"><span data-stu-id="e7c02-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e7c02-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="e7c02-125">Authorization</span></span>|<span data-ttu-id="e7c02-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="e7c02-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e7c02-127">Annehmen</span><span class="sxs-lookup"><span data-stu-id="e7c02-127">Accept</span></span>|<span data-ttu-id="e7c02-128">application/json</span><span class="sxs-lookup"><span data-stu-id="e7c02-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e7c02-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e7c02-129">Request body</span></span>
<span data-ttu-id="e7c02-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="e7c02-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e7c02-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="e7c02-131">Response</span></span>
<span data-ttu-id="e7c02-132">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [roleAssignment](../resources/intune-rbac-roleassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="e7c02-132">If successful, this method returns a `200 OK` response code and [roleAssignment](../resources/intune-rbac-roleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e7c02-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e7c02-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="e7c02-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e7c02-134">Request</span></span>
<span data-ttu-id="e7c02-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e7c02-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}
```

### <a name="response"></a><span data-ttu-id="e7c02-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="e7c02-136">Response</span></span>
<span data-ttu-id="e7c02-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e7c02-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





