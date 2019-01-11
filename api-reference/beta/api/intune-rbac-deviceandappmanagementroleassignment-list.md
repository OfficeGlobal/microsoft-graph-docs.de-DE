---
title: Auflisten von „deviceAndAppManagementRoleAssignment“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs deviceAndAppManagementRoleAssignment auf.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 8dc9307ed69c977b3d312f63e3d2a1e1ed9814b5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27848405"
---
# <a name="list-deviceandappmanagementroleassignments"></a><span data-ttu-id="a8df1-103">Auflisten von „deviceAndAppManagementRoleAssignment“</span><span class="sxs-lookup"><span data-stu-id="a8df1-103">List deviceAndAppManagementRoleAssignments</span></span>

> <span data-ttu-id="a8df1-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="a8df1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a8df1-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a8df1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a8df1-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="a8df1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a8df1-107">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) auf.</span><span class="sxs-lookup"><span data-stu-id="a8df1-107">List properties and relationships of the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a8df1-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="a8df1-108">Prerequisites</span></span>
<span data-ttu-id="a8df1-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a8df1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a8df1-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a8df1-111">Permission type</span></span>|<span data-ttu-id="a8df1-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a8df1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a8df1-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a8df1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a8df1-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="a8df1-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="a8df1-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a8df1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a8df1-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a8df1-116">Not supported.</span></span>|
|<span data-ttu-id="a8df1-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a8df1-117">Application</span></span>|<span data-ttu-id="a8df1-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a8df1-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a8df1-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a8df1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="a8df1-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a8df1-120">Request headers</span></span>
|<span data-ttu-id="a8df1-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="a8df1-121">Header</span></span>|<span data-ttu-id="a8df1-122">Wert</span><span class="sxs-lookup"><span data-stu-id="a8df1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a8df1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a8df1-123">Authorization</span></span>|<span data-ttu-id="a8df1-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="a8df1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a8df1-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="a8df1-125">Accept</span></span>|<span data-ttu-id="a8df1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a8df1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a8df1-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a8df1-127">Request body</span></span>
<span data-ttu-id="a8df1-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="a8df1-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a8df1-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="a8df1-129">Response</span></span>
<span data-ttu-id="a8df1-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="a8df1-130">If successful, this method returns a `200 OK` response code and a collection of [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a8df1-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a8df1-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="a8df1-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a8df1-132">Request</span></span>
<span data-ttu-id="a8df1-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a8df1-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/roleAssignments
```

### <a name="response"></a><span data-ttu-id="a8df1-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="a8df1-134">Response</span></span>
<span data-ttu-id="a8df1-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a8df1-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 480

{
  "value": [
    {
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
  ]
}
```





