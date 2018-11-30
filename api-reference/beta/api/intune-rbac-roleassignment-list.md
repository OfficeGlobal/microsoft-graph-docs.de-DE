---
title: roleAssignments auflisten
description: Auflisten von Eigenschaften und Beziehungen der roleAssignment-Objekte.
ms.openlocfilehash: adfc95650fb316adbd6c9cf5944539708834eefb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066060"
---
# <a name="list-roleassignments"></a><span data-ttu-id="90b18-103">roleAssignments auflisten</span><span class="sxs-lookup"><span data-stu-id="90b18-103">List roleAssignments</span></span>

> <span data-ttu-id="90b18-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="90b18-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="90b18-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="90b18-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="90b18-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="90b18-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="90b18-107">Auflisten von Eigenschaften und Beziehungen der [roleAssignment](../resources/intune-rbac-roleassignment.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="90b18-107">List properties and relationships of the [roleAssignment](../resources/intune-rbac-roleassignment.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="90b18-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="90b18-108">Prerequisites</span></span>
<span data-ttu-id="90b18-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="90b18-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="90b18-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="90b18-111">Permission type</span></span>|<span data-ttu-id="90b18-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="90b18-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="90b18-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="90b18-113">Delegated (work or school account)</span></span>|<span data-ttu-id="90b18-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="90b18-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="90b18-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="90b18-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="90b18-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="90b18-116">Not supported.</span></span>|
|<span data-ttu-id="90b18-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="90b18-117">Application</span></span>|<span data-ttu-id="90b18-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="90b18-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="90b18-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="90b18-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="90b18-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="90b18-120">Request headers</span></span>
|<span data-ttu-id="90b18-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="90b18-121">Header</span></span>|<span data-ttu-id="90b18-122">Wert</span><span class="sxs-lookup"><span data-stu-id="90b18-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="90b18-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="90b18-123">Authorization</span></span>|<span data-ttu-id="90b18-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="90b18-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="90b18-125">Accept</span><span class="sxs-lookup"><span data-stu-id="90b18-125">Accept</span></span>|<span data-ttu-id="90b18-126">application/json</span><span class="sxs-lookup"><span data-stu-id="90b18-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="90b18-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="90b18-127">Request body</span></span>
<span data-ttu-id="90b18-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="90b18-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="90b18-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="90b18-129">Response</span></span>
<span data-ttu-id="90b18-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [roleAssignment](../resources/intune-rbac-roleassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="90b18-130">If successful, this method returns a `200 OK` response code and a collection of [roleAssignment](../resources/intune-rbac-roleassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="90b18-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="90b18-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="90b18-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="90b18-132">Request</span></span>
<span data-ttu-id="90b18-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="90b18-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments
```

### <a name="response"></a><span data-ttu-id="90b18-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="90b18-134">Response</span></span>
<span data-ttu-id="90b18-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="90b18-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 403

{
  "value": [
    {
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
  ]
}
```





