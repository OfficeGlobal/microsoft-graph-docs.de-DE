---
title: Abrufen von „roleAssignment“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs roleAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 286d049507deab8e31af5ca96458394e12818853
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30260389"
---
# <a name="get-roleassignment"></a><span data-ttu-id="c3360-103">Abrufen von „roleAssignment“</span><span class="sxs-lookup"><span data-stu-id="c3360-103">Get roleAssignment</span></span>

> <span data-ttu-id="c3360-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="c3360-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c3360-105">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="c3360-105">Read properties and relationships of the [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c3360-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c3360-106">Prerequisites</span></span>
<span data-ttu-id="c3360-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="c3360-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="c3360-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c3360-109">Permission type</span></span>|<span data-ttu-id="c3360-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c3360-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c3360-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c3360-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c3360-112">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="c3360-112">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="c3360-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c3360-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c3360-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c3360-114">Not supported.</span></span>|
|<span data-ttu-id="c3360-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c3360-115">Application</span></span>|<span data-ttu-id="c3360-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c3360-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c3360-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c3360-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c3360-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="c3360-118">Optional query parameters</span></span>
<span data-ttu-id="c3360-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="c3360-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c3360-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c3360-120">Request headers</span></span>
|<span data-ttu-id="c3360-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="c3360-121">Header</span></span>|<span data-ttu-id="c3360-122">Wert</span><span class="sxs-lookup"><span data-stu-id="c3360-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c3360-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c3360-123">Authorization</span></span>|<span data-ttu-id="c3360-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c3360-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c3360-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="c3360-125">Accept</span></span>|<span data-ttu-id="c3360-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c3360-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c3360-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c3360-127">Request body</span></span>
<span data-ttu-id="c3360-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="c3360-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c3360-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="c3360-129">Response</span></span>
<span data-ttu-id="c3360-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [roleAssignment](../resources/intune-rbac-roleassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="c3360-130">If successful, this method returns a `200 OK` response code and [roleAssignment](../resources/intune-rbac-roleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c3360-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c3360-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="c3360-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c3360-132">Request</span></span>
<span data-ttu-id="c3360-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c3360-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}
```

### <a name="response"></a><span data-ttu-id="c3360-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="c3360-134">Response</span></span>
<span data-ttu-id="c3360-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c3360-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 275

{
  "value": {
    "@odata.type": "#microsoft.graph.roleAssignment",
    "id": "b3234d24-4d24-b323-244d-23b3244d23b3",
    "displayName": "Display Name value",
    "description": "Description value",
    "resourceScopes": [
      "Resource Scopes value"
    ]
  }
}
```



