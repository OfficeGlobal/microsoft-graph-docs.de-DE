---
title: getRoleScopeTagsByResource-Funktion
description: Noch nicht dokumentiert.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ea20330fadc4db5a3ed814450b34b660ba230789
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/14/2019
ms.locfileid: "30571291"
---
# <a name="getrolescopetagsbyresource-function"></a><span data-ttu-id="6f865-103">getRoleScopeTagsByResource-Funktion</span><span class="sxs-lookup"><span data-stu-id="6f865-103">getRoleScopeTagsByResource function</span></span>

> <span data-ttu-id="6f865-104">**Wichtig:** APIs unter der/Beta-Version in Microsoft Graph können geändert werden.</span><span class="sxs-lookup"><span data-stu-id="6f865-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="6f865-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6f865-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6f865-106">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="6f865-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6f865-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="6f865-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6f865-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="6f865-108">Prerequisites</span></span>
<span data-ttu-id="6f865-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="6f865-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="6f865-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6f865-111">Permission type</span></span>|<span data-ttu-id="6f865-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6f865-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6f865-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6f865-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="6f865-114">&nbsp; &nbsp; **Rollenbasierte Zugriffssteuerung**</span><span class="sxs-lookup"><span data-stu-id="6f865-114">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="6f865-115">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="6f865-115">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="6f865-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6f865-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6f865-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6f865-117">Not supported.</span></span>|
|<span data-ttu-id="6f865-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6f865-118">Application</span></span>|<span data-ttu-id="6f865-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6f865-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6f865-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6f865-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getRoleScopeTagsByResource
```

## <a name="request-headers"></a><span data-ttu-id="6f865-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6f865-121">Request headers</span></span>
|<span data-ttu-id="6f865-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="6f865-122">Header</span></span>|<span data-ttu-id="6f865-123">Wert</span><span class="sxs-lookup"><span data-stu-id="6f865-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6f865-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="6f865-124">Authorization</span></span>|<span data-ttu-id="6f865-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="6f865-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6f865-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="6f865-126">Accept</span></span>|<span data-ttu-id="6f865-127">application/json</span><span class="sxs-lookup"><span data-stu-id="6f865-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6f865-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6f865-128">Request body</span></span>
<span data-ttu-id="6f865-129">Stellen Sie in der URL der Anforderung die folgenden Abfrageparameter mit Werten bereit.</span><span class="sxs-lookup"><span data-stu-id="6f865-129">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="6f865-130">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Funktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="6f865-130">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="6f865-131">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6f865-131">Property</span></span>|<span data-ttu-id="6f865-132">Typ</span><span class="sxs-lookup"><span data-stu-id="6f865-132">Type</span></span>|<span data-ttu-id="6f865-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6f865-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6f865-134">resource</span><span class="sxs-lookup"><span data-stu-id="6f865-134">resource</span></span>|<span data-ttu-id="6f865-135">String</span><span class="sxs-lookup"><span data-stu-id="6f865-135">String</span></span>|<span data-ttu-id="6f865-136">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="6f865-136">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="6f865-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="6f865-137">Response</span></span>
<span data-ttu-id="6f865-138">Bei erfolgreicher Ausführung gibt die Funktion den `200 OK` Antwortcode und eine [roleScopeTag](../resources/intune-rbac-rolescopetag.md) -Auflistung im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="6f865-138">If successful, this function returns a `200 OK` response code and a [roleScopeTag](../resources/intune-rbac-rolescopetag.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6f865-139">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6f865-139">Example</span></span>
### <a name="request"></a><span data-ttu-id="6f865-140">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6f865-140">Request</span></span>
<span data-ttu-id="6f865-141">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6f865-141">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/getRoleScopeTagsByResource(resource='parameterValue')
```

### <a name="response"></a><span data-ttu-id="6f865-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="6f865-142">Response</span></span>
<span data-ttu-id="6f865-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6f865-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



