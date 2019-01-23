---
title: GetRoleScopeTagsByResource-Funktion
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 4729aa6fdc6dd63acead2c9d1225c05d881706df
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425652"
---
# <a name="getrolescopetagsbyresource-function"></a><span data-ttu-id="74a4b-103">GetRoleScopeTagsByResource-Funktion</span><span class="sxs-lookup"><span data-stu-id="74a4b-103">getRoleScopeTagsByResource function</span></span>

> <span data-ttu-id="74a4b-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="74a4b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="74a4b-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="74a4b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="74a4b-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="74a4b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="74a4b-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="74a4b-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="74a4b-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="74a4b-108">Prerequisites</span></span>
<span data-ttu-id="74a4b-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="74a4b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="74a4b-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="74a4b-111">Permission type</span></span>|<span data-ttu-id="74a4b-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="74a4b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="74a4b-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="74a4b-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="74a4b-114">&nbsp;&nbsp; **Role-based Access Control (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="74a4b-114">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="74a4b-115">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="74a4b-115">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="74a4b-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="74a4b-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="74a4b-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="74a4b-117">Not supported.</span></span>|
|<span data-ttu-id="74a4b-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="74a4b-118">Application</span></span>|<span data-ttu-id="74a4b-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="74a4b-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="74a4b-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="74a4b-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getRoleScopeTagsByResource
```

## <a name="request-headers"></a><span data-ttu-id="74a4b-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="74a4b-121">Request headers</span></span>
|<span data-ttu-id="74a4b-122">Header</span><span class="sxs-lookup"><span data-stu-id="74a4b-122">Header</span></span>|<span data-ttu-id="74a4b-123">Wert</span><span class="sxs-lookup"><span data-stu-id="74a4b-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="74a4b-124">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="74a4b-124">Authorization</span></span>|<span data-ttu-id="74a4b-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="74a4b-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="74a4b-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="74a4b-126">Accept</span></span>|<span data-ttu-id="74a4b-127">application/json</span><span class="sxs-lookup"><span data-stu-id="74a4b-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="74a4b-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="74a4b-128">Request body</span></span>
<span data-ttu-id="74a4b-129">Geben Sie in der Anforderungs-URL die folgenden Abfrageparameter mit Werten an.</span><span class="sxs-lookup"><span data-stu-id="74a4b-129">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="74a4b-130">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Funktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="74a4b-130">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="74a4b-131">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="74a4b-131">Property</span></span>|<span data-ttu-id="74a4b-132">Typ</span><span class="sxs-lookup"><span data-stu-id="74a4b-132">Type</span></span>|<span data-ttu-id="74a4b-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="74a4b-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="74a4b-134">resource</span><span class="sxs-lookup"><span data-stu-id="74a4b-134">resource</span></span>|<span data-ttu-id="74a4b-135">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="74a4b-135">String</span></span>|<span data-ttu-id="74a4b-136">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="74a4b-136">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="74a4b-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="74a4b-137">Response</span></span>
<span data-ttu-id="74a4b-138">Wenn erfolgreich, diese Funktion gibt eine `200 OK` Antwortcode und eine [RoleScopeTag](../resources/intune-rbac-rolescopetag.md) -Auflistung im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="74a4b-138">If successful, this function returns a `200 OK` response code and a [roleScopeTag](../resources/intune-rbac-rolescopetag.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="74a4b-139">Beispiel</span><span class="sxs-lookup"><span data-stu-id="74a4b-139">Example</span></span>
### <a name="request"></a><span data-ttu-id="74a4b-140">Anforderung</span><span class="sxs-lookup"><span data-stu-id="74a4b-140">Request</span></span>
<span data-ttu-id="74a4b-141">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="74a4b-141">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/getRoleScopeTagsByResource(resource='parameterValue')
```

### <a name="response"></a><span data-ttu-id="74a4b-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="74a4b-142">Response</span></span>
<span data-ttu-id="74a4b-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="74a4b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



