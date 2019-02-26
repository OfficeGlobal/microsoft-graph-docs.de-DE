---
title: deviceAndAppManagementRoleAssignment abrufen
description: Lesen von Eigenschaften und Beziehungen des deviceAndAppManagementRoleAssignment-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 72be2b21df823e76faac3106a142b5bbfb446f29
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30163427"
---
# <a name="get-deviceandappmanagementroleassignment"></a><span data-ttu-id="64597-103">deviceAndAppManagementRoleAssignment abrufen</span><span class="sxs-lookup"><span data-stu-id="64597-103">Get deviceAndAppManagementRoleAssignment</span></span>

> <span data-ttu-id="64597-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="64597-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="64597-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="64597-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="64597-106">Lesen von Eigenschaften und Beziehungen des [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="64597-106">Read properties and relationships of the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="64597-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="64597-107">Prerequisites</span></span>
<span data-ttu-id="64597-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="64597-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="64597-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="64597-110">Permission type</span></span>|<span data-ttu-id="64597-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="64597-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="64597-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="64597-112">Delegated (work or school account)</span></span>|<span data-ttu-id="64597-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="64597-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="64597-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="64597-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="64597-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="64597-115">Not supported.</span></span>|
|<span data-ttu-id="64597-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="64597-116">Application</span></span>|<span data-ttu-id="64597-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="64597-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="64597-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="64597-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleAssignments/{deviceAndAppManagementRoleAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="64597-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="64597-119">Optional query parameters</span></span>
<span data-ttu-id="64597-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="64597-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="64597-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="64597-121">Request headers</span></span>
|<span data-ttu-id="64597-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="64597-122">Header</span></span>|<span data-ttu-id="64597-123">Wert</span><span class="sxs-lookup"><span data-stu-id="64597-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="64597-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="64597-124">Authorization</span></span>|<span data-ttu-id="64597-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="64597-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="64597-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="64597-126">Accept</span></span>|<span data-ttu-id="64597-127">application/json</span><span class="sxs-lookup"><span data-stu-id="64597-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="64597-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="64597-128">Request body</span></span>
<span data-ttu-id="64597-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="64597-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="64597-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="64597-130">Response</span></span>
<span data-ttu-id="64597-131">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="64597-131">If successful, this method returns a `200 OK` response code and [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="64597-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="64597-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="64597-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="64597-133">Request</span></span>
<span data-ttu-id="64597-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="64597-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/roleAssignments/{deviceAndAppManagementRoleAssignmentId}
```

### <a name="response"></a><span data-ttu-id="64597-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="64597-135">Response</span></span>
<span data-ttu-id="64597-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="64597-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 438

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleAssignment",
    "id": "a12e8ebb-8ebb-a12e-bb8e-2ea1bb8e2ea1",
    "displayName": "Display Name value",
    "description": "Description value",
    "scopeMembers": [
      "Scope Members value"
    ],
    "scopeType": "allDevices",
    "resourceScopes": [
      "Resource Scopes value"
    ],
    "members": [
      "Members value"
    ]
  }
}
```




