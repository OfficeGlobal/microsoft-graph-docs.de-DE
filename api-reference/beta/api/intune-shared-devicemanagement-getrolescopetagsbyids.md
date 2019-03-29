---
title: getRoleScopeTagsByIds-Funktion
description: Noch nicht dokumentiert.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 764bfd10fdfde445d38dbf5eb4f2552f02a8231f
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30981930"
---
# <a name="getrolescopetagsbyids-function"></a><span data-ttu-id="b4393-103">getRoleScopeTagsByIds-Funktion</span><span class="sxs-lookup"><span data-stu-id="b4393-103">getRoleScopeTagsByIds function</span></span>

> <span data-ttu-id="b4393-104">**Wichtig:** APIs unter der/Beta-Version in Microsoft Graph können geändert werden.</span><span class="sxs-lookup"><span data-stu-id="b4393-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b4393-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b4393-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b4393-106">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="b4393-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b4393-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="b4393-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b4393-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b4393-108">Prerequisites</span></span>
<span data-ttu-id="b4393-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b4393-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b4393-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b4393-111">Permission type</span></span>|<span data-ttu-id="b4393-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b4393-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b4393-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b4393-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="b4393-114">&nbsp; &nbsp; **Rollenbasierte Zugriffssteuerung (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="b4393-114">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="b4393-115">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="b4393-115">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="b4393-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b4393-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b4393-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b4393-117">Not supported.</span></span>|
|<span data-ttu-id="b4393-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b4393-118">Application</span></span>|<span data-ttu-id="b4393-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b4393-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b4393-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b4393-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getRoleScopeTagsByIds
```

## <a name="request-headers"></a><span data-ttu-id="b4393-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b4393-121">Request headers</span></span>
|<span data-ttu-id="b4393-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="b4393-122">Header</span></span>|<span data-ttu-id="b4393-123">Wert</span><span class="sxs-lookup"><span data-stu-id="b4393-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b4393-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="b4393-124">Authorization</span></span>|<span data-ttu-id="b4393-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b4393-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b4393-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="b4393-126">Accept</span></span>|<span data-ttu-id="b4393-127">application/json</span><span class="sxs-lookup"><span data-stu-id="b4393-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b4393-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b4393-128">Request body</span></span>
<span data-ttu-id="b4393-129">Stellen Sie in der URL der Anforderung die folgenden Abfrageparameter mit Werten bereit.</span><span class="sxs-lookup"><span data-stu-id="b4393-129">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="b4393-130">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Funktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="b4393-130">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="b4393-131">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b4393-131">Property</span></span>|<span data-ttu-id="b4393-132">Typ</span><span class="sxs-lookup"><span data-stu-id="b4393-132">Type</span></span>|<span data-ttu-id="b4393-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b4393-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b4393-134">ids</span><span class="sxs-lookup"><span data-stu-id="b4393-134">ids</span></span>|<span data-ttu-id="b4393-135">String collection</span><span class="sxs-lookup"><span data-stu-id="b4393-135">String collection</span></span>|<span data-ttu-id="b4393-136">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="b4393-136">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="b4393-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="b4393-137">Response</span></span>
<span data-ttu-id="b4393-138">Bei erfolgreicher Ausführung gibt die Funktion den `200 OK` Antwortcode und eine [roleScopeTag](../resources/intune-rbac-rolescopetag.md) -Auflistung im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="b4393-138">If successful, this function returns a `200 OK` response code and a [roleScopeTag](../resources/intune-rbac-rolescopetag.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b4393-139">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b4393-139">Example</span></span>
### <a name="request"></a><span data-ttu-id="b4393-140">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b4393-140">Request</span></span>
<span data-ttu-id="b4393-141">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b4393-141">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/getRoleScopeTagsByIds(ids=[
  "Ids value"
])
```

### <a name="response"></a><span data-ttu-id="b4393-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="b4393-142">Response</span></span>
<span data-ttu-id="b4393-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b4393-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



