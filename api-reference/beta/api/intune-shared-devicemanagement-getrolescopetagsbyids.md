---
title: GetRoleScopeTagsByIds-Funktion
description: Noch nicht dokumentiert
ms.openlocfilehash: 67722ad61a71f8d8572a95c5972992d4e0818931
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063313"
---
# <a name="getrolescopetagsbyids-function"></a><span data-ttu-id="4839d-103">GetRoleScopeTagsByIds-Funktion</span><span class="sxs-lookup"><span data-stu-id="4839d-103">getRoleScopeTagsByIds function</span></span>

> <span data-ttu-id="4839d-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="4839d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4839d-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4839d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4839d-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="4839d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4839d-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="4839d-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4839d-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="4839d-108">Prerequisites</span></span>
<span data-ttu-id="4839d-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4839d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4839d-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4839d-111">Permission type</span></span>|<span data-ttu-id="4839d-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4839d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4839d-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4839d-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="4839d-114">&nbsp;&nbsp; **Role-based Access Control (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="4839d-114">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="4839d-115">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="4839d-115">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="4839d-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4839d-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4839d-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4839d-117">Not supported.</span></span>|
|<span data-ttu-id="4839d-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4839d-118">Application</span></span>|<span data-ttu-id="4839d-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4839d-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4839d-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4839d-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getRoleScopeTagsByIds
```

## <a name="request-headers"></a><span data-ttu-id="4839d-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4839d-121">Request headers</span></span>
|<span data-ttu-id="4839d-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="4839d-122">Header</span></span>|<span data-ttu-id="4839d-123">Wert</span><span class="sxs-lookup"><span data-stu-id="4839d-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4839d-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="4839d-124">Authorization</span></span>|<span data-ttu-id="4839d-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="4839d-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4839d-126">Accept</span><span class="sxs-lookup"><span data-stu-id="4839d-126">Accept</span></span>|<span data-ttu-id="4839d-127">application/json</span><span class="sxs-lookup"><span data-stu-id="4839d-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4839d-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4839d-128">Request body</span></span>
<span data-ttu-id="4839d-129">Geben Sie in der Anforderungs-URL die folgenden Abfrageparameter mit Werten an.</span><span class="sxs-lookup"><span data-stu-id="4839d-129">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="4839d-130">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Funktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="4839d-130">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="4839d-131">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4839d-131">Property</span></span>|<span data-ttu-id="4839d-132">Typ</span><span class="sxs-lookup"><span data-stu-id="4839d-132">Type</span></span>|<span data-ttu-id="4839d-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4839d-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4839d-134">ids</span><span class="sxs-lookup"><span data-stu-id="4839d-134">ids</span></span>|<span data-ttu-id="4839d-135">String-Sammlung</span><span class="sxs-lookup"><span data-stu-id="4839d-135">String collection</span></span>|<span data-ttu-id="4839d-136">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="4839d-136">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="4839d-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="4839d-137">Response</span></span>
<span data-ttu-id="4839d-138">Wenn erfolgreich, diese Funktion gibt eine `200 OK` Antwortcode und eine [RoleScopeTag](../resources/intune-rbac-rolescopetag.md) -Auflistung im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="4839d-138">If successful, this function returns a `200 OK` response code and a [roleScopeTag](../resources/intune-rbac-rolescopetag.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4839d-139">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4839d-139">Example</span></span>
### <a name="request"></a><span data-ttu-id="4839d-140">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4839d-140">Request</span></span>
<span data-ttu-id="4839d-141">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4839d-141">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/getRoleScopeTagsByIds(ids=[
  "Ids value"
])
```

### <a name="response"></a><span data-ttu-id="4839d-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="4839d-142">Response</span></span>
<span data-ttu-id="4839d-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4839d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



