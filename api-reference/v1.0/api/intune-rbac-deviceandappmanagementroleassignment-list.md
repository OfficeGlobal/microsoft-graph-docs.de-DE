---
title: Auflisten von „deviceAndAppManagementRoleAssignment“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs deviceAndAppManagementRoleAssignment auf.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 199794d8971214577b1a5e64e4b890aa643d60b8
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30989526"
---
# <a name="list-deviceandappmanagementroleassignments"></a><span data-ttu-id="2e46d-103">Auflisten von „deviceAndAppManagementRoleAssignment“</span><span class="sxs-lookup"><span data-stu-id="2e46d-103">List deviceAndAppManagementRoleAssignments</span></span>

> <span data-ttu-id="2e46d-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="2e46d-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2e46d-105">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) auf.</span><span class="sxs-lookup"><span data-stu-id="2e46d-105">List properties and relationships of the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2e46d-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="2e46d-106">Prerequisites</span></span>
<span data-ttu-id="2e46d-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2e46d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2e46d-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2e46d-109">Permission type</span></span>|<span data-ttu-id="2e46d-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2e46d-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2e46d-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2e46d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2e46d-112">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="2e46d-112">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="2e46d-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2e46d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2e46d-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2e46d-114">Not supported.</span></span>|
|<span data-ttu-id="2e46d-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2e46d-115">Application</span></span>|<span data-ttu-id="2e46d-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2e46d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2e46d-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2e46d-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="2e46d-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2e46d-118">Request headers</span></span>
|<span data-ttu-id="2e46d-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="2e46d-119">Header</span></span>|<span data-ttu-id="2e46d-120">Wert</span><span class="sxs-lookup"><span data-stu-id="2e46d-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2e46d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="2e46d-121">Authorization</span></span>|<span data-ttu-id="2e46d-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="2e46d-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2e46d-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="2e46d-123">Accept</span></span>|<span data-ttu-id="2e46d-124">application/json</span><span class="sxs-lookup"><span data-stu-id="2e46d-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2e46d-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2e46d-125">Request body</span></span>
<span data-ttu-id="2e46d-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="2e46d-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2e46d-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="2e46d-127">Response</span></span>
<span data-ttu-id="2e46d-128">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="2e46d-128">If successful, this method returns a `200 OK` response code and a collection of [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2e46d-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2e46d-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="2e46d-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2e46d-130">Request</span></span>
<span data-ttu-id="2e46d-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2e46d-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/roleAssignments
```

### <a name="response"></a><span data-ttu-id="2e46d-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="2e46d-132">Response</span></span>
<span data-ttu-id="2e46d-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2e46d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 380

{
  "value": [
    {
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
  ]
}
```



