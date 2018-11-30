---
title: Liste roleScopeTags
description: Listeneigenschaften und Beziehungen der RoleScopeTag-Objekte.
ms.openlocfilehash: 632c40126197ca7905ad4075c3da7688ed258441
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058757"
---
# <a name="list-rolescopetags"></a><span data-ttu-id="a5ee7-103">Liste roleScopeTags</span><span class="sxs-lookup"><span data-stu-id="a5ee7-103">List roleScopeTags</span></span>

> <span data-ttu-id="a5ee7-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="a5ee7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a5ee7-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a5ee7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a5ee7-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="a5ee7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a5ee7-107">Listeneigenschaften und Beziehungen der [RoleScopeTag](../resources/intune-rbac-rolescopetag.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="a5ee7-107">List properties and relationships of the [roleScopeTag](../resources/intune-rbac-rolescopetag.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a5ee7-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="a5ee7-108">Prerequisites</span></span>
<span data-ttu-id="a5ee7-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a5ee7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a5ee7-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a5ee7-111">Permission type</span></span>|<span data-ttu-id="a5ee7-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a5ee7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a5ee7-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a5ee7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a5ee7-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="a5ee7-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="a5ee7-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a5ee7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a5ee7-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a5ee7-116">Not supported.</span></span>|
|<span data-ttu-id="a5ee7-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a5ee7-117">Application</span></span>|<span data-ttu-id="a5ee7-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a5ee7-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a5ee7-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a5ee7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleScopeTags
GET /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags
```

## <a name="request-headers"></a><span data-ttu-id="a5ee7-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a5ee7-120">Request headers</span></span>
|<span data-ttu-id="a5ee7-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="a5ee7-121">Header</span></span>|<span data-ttu-id="a5ee7-122">Wert</span><span class="sxs-lookup"><span data-stu-id="a5ee7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a5ee7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a5ee7-123">Authorization</span></span>|<span data-ttu-id="a5ee7-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="a5ee7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a5ee7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a5ee7-125">Accept</span></span>|<span data-ttu-id="a5ee7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a5ee7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a5ee7-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a5ee7-127">Request body</span></span>
<span data-ttu-id="a5ee7-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="a5ee7-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a5ee7-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="a5ee7-129">Response</span></span>
<span data-ttu-id="a5ee7-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [RoleScopeTag](../resources/intune-rbac-rolescopetag.md) .</span><span class="sxs-lookup"><span data-stu-id="a5ee7-130">If successful, this method returns a `200 OK` response code and a collection of [roleScopeTag](../resources/intune-rbac-rolescopetag.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a5ee7-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a5ee7-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="a5ee7-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a5ee7-132">Request</span></span>
<span data-ttu-id="a5ee7-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a5ee7-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/roleScopeTags
```

### <a name="response"></a><span data-ttu-id="a5ee7-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="a5ee7-134">Response</span></span>
<span data-ttu-id="a5ee7-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a5ee7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 231

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.roleScopeTag",
      "id": "9ed1e179-e179-9ed1-79e1-d19e79e1d19e",
      "displayName": "Display Name value",
      "description": "Description value"
    }
  ]
}
```





