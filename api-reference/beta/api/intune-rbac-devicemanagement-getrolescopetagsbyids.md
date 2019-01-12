---
title: GetRoleScopeTagsByIds-Funktion
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 4eeb89d0b3636ad20f9b59ad1ee9db867e5481e8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27929704"
---
# <a name="getrolescopetagsbyids-function"></a><span data-ttu-id="e32c3-103">GetRoleScopeTagsByIds-Funktion</span><span class="sxs-lookup"><span data-stu-id="e32c3-103">getRoleScopeTagsByIds function</span></span>

> <span data-ttu-id="e32c3-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="e32c3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e32c3-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e32c3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e32c3-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="e32c3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e32c3-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="e32c3-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e32c3-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="e32c3-108">Prerequisites</span></span>
<span data-ttu-id="e32c3-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e32c3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e32c3-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e32c3-111">Permission type</span></span>|<span data-ttu-id="e32c3-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e32c3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e32c3-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e32c3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e32c3-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="e32c3-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="e32c3-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e32c3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e32c3-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e32c3-116">Not supported.</span></span>|
|<span data-ttu-id="e32c3-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e32c3-117">Application</span></span>|<span data-ttu-id="e32c3-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e32c3-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e32c3-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e32c3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getRoleScopeTagsByIds
```

## <a name="request-headers"></a><span data-ttu-id="e32c3-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e32c3-120">Request headers</span></span>
|<span data-ttu-id="e32c3-121">Header</span><span class="sxs-lookup"><span data-stu-id="e32c3-121">Header</span></span>|<span data-ttu-id="e32c3-122">Wert</span><span class="sxs-lookup"><span data-stu-id="e32c3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e32c3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e32c3-123">Authorization</span></span>|<span data-ttu-id="e32c3-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="e32c3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e32c3-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="e32c3-125">Accept</span></span>|<span data-ttu-id="e32c3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e32c3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e32c3-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e32c3-127">Request body</span></span>
<span data-ttu-id="e32c3-128">Geben Sie in der Anforderungs-URL die folgenden Abfrageparameter mit Werten an.</span><span class="sxs-lookup"><span data-stu-id="e32c3-128">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="e32c3-129">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Funktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="e32c3-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="e32c3-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e32c3-130">Property</span></span>|<span data-ttu-id="e32c3-131">Typ</span><span class="sxs-lookup"><span data-stu-id="e32c3-131">Type</span></span>|<span data-ttu-id="e32c3-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e32c3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e32c3-133">ids</span><span class="sxs-lookup"><span data-stu-id="e32c3-133">ids</span></span>|<span data-ttu-id="e32c3-134">String-Sammlung</span><span class="sxs-lookup"><span data-stu-id="e32c3-134">String collection</span></span>|<span data-ttu-id="e32c3-135">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="e32c3-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="e32c3-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="e32c3-136">Response</span></span>
<span data-ttu-id="e32c3-137">Wenn erfolgreich, diese Funktion gibt eine `200 OK` Antwortcode und eine [RoleScopeTag](../resources/intune-rbac-rolescopetag.md) -Auflistung im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="e32c3-137">If successful, this function returns a `200 OK` response code and a [roleScopeTag](../resources/intune-rbac-rolescopetag.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e32c3-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e32c3-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="e32c3-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e32c3-139">Request</span></span>
<span data-ttu-id="e32c3-140">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e32c3-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/getRoleScopeTagsByIds(ids=[
  "Ids value"
])
```

### <a name="response"></a><span data-ttu-id="e32c3-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="e32c3-141">Response</span></span>
<span data-ttu-id="e32c3-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e32c3-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





