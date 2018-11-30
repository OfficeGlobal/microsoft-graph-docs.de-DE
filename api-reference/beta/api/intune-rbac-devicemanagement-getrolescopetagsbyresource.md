---
title: GetRoleScopeTagsByResource-Funktion
description: Noch nicht dokumentiert
ms.openlocfilehash: 10c440464224877865e74d9c9fe1750088241af7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064421"
---
# <a name="getrolescopetagsbyresource-function"></a><span data-ttu-id="0957c-103">GetRoleScopeTagsByResource-Funktion</span><span class="sxs-lookup"><span data-stu-id="0957c-103">getRoleScopeTagsByResource function</span></span>

> <span data-ttu-id="0957c-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="0957c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0957c-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0957c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0957c-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="0957c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0957c-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="0957c-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0957c-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="0957c-108">Prerequisites</span></span>
<span data-ttu-id="0957c-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0957c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0957c-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0957c-111">Permission type</span></span>|<span data-ttu-id="0957c-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0957c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0957c-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0957c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0957c-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="0957c-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="0957c-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0957c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0957c-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0957c-116">Not supported.</span></span>|
|<span data-ttu-id="0957c-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0957c-117">Application</span></span>|<span data-ttu-id="0957c-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0957c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0957c-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0957c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getRoleScopeTagsByResource
```

## <a name="request-headers"></a><span data-ttu-id="0957c-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0957c-120">Request headers</span></span>
|<span data-ttu-id="0957c-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="0957c-121">Header</span></span>|<span data-ttu-id="0957c-122">Wert</span><span class="sxs-lookup"><span data-stu-id="0957c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0957c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0957c-123">Authorization</span></span>|<span data-ttu-id="0957c-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="0957c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0957c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0957c-125">Accept</span></span>|<span data-ttu-id="0957c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0957c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0957c-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0957c-127">Request body</span></span>
<span data-ttu-id="0957c-128">Geben Sie in der Anforderungs-URL die folgenden Abfrageparameter mit Werten an.</span><span class="sxs-lookup"><span data-stu-id="0957c-128">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="0957c-129">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Funktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="0957c-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="0957c-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0957c-130">Property</span></span>|<span data-ttu-id="0957c-131">Typ</span><span class="sxs-lookup"><span data-stu-id="0957c-131">Type</span></span>|<span data-ttu-id="0957c-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0957c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0957c-133">resource</span><span class="sxs-lookup"><span data-stu-id="0957c-133">resource</span></span>|<span data-ttu-id="0957c-134">String</span><span class="sxs-lookup"><span data-stu-id="0957c-134">String</span></span>|<span data-ttu-id="0957c-135">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="0957c-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="0957c-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="0957c-136">Response</span></span>
<span data-ttu-id="0957c-137">Wenn erfolgreich, diese Funktion gibt eine `200 OK` Antwortcode und eine [RoleScopeTag](../resources/intune-rbac-rolescopetag.md) -Auflistung im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="0957c-137">If successful, this function returns a `200 OK` response code and a [roleScopeTag](../resources/intune-rbac-rolescopetag.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0957c-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0957c-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="0957c-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0957c-139">Request</span></span>
<span data-ttu-id="0957c-140">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0957c-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/getRoleScopeTagsByResource(resource='parameterValue')
```

### <a name="response"></a><span data-ttu-id="0957c-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="0957c-141">Response</span></span>
<span data-ttu-id="0957c-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0957c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





