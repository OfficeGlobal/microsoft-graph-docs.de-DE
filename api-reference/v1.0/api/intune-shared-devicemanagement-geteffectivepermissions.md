---
title: getEffectivePermissions-Funktion
description: Ruft die effektiven Berechtigungen des derzeit authentifizierten Benutzers ab.
ms.openlocfilehash: 0d07045c4db64f6bb9418907cea618480d959522
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018494"
---
# <a name="geteffectivepermissions-function"></a><span data-ttu-id="9618f-103">getEffectivePermissions-Funktion</span><span class="sxs-lookup"><span data-stu-id="9618f-103">getEffectivePermissions function</span></span>

> <span data-ttu-id="9618f-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="9618f-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9618f-105">Ruft die effektiven Berechtigungen des derzeit authentifizierten Benutzers ab.</span><span class="sxs-lookup"><span data-stu-id="9618f-105">Retrieves the effective permissions of the currently authenticated user</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9618f-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="9618f-106">Prerequisites</span></span>
<span data-ttu-id="9618f-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9618f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9618f-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9618f-109">Permission type</span></span>|<span data-ttu-id="9618f-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9618f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9618f-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9618f-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="9618f-112">&nbsp;&nbsp; Rollenbasierte Zugriffssteuerung</span><span class="sxs-lookup"><span data-stu-id="9618f-112">&nbsp; &nbsp; Role-based access control</span></span> | <span data-ttu-id="9618f-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="9618f-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="9618f-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9618f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9618f-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9618f-115">Not supported.</span></span>|
|<span data-ttu-id="9618f-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9618f-116">Application</span></span>|<span data-ttu-id="9618f-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9618f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9618f-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9618f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getEffectivePermissions
```

## <a name="request-headers"></a><span data-ttu-id="9618f-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9618f-119">Request headers</span></span>
|<span data-ttu-id="9618f-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="9618f-120">Header</span></span>|<span data-ttu-id="9618f-121">Wert</span><span class="sxs-lookup"><span data-stu-id="9618f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9618f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9618f-122">Authorization</span></span>|<span data-ttu-id="9618f-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="9618f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9618f-124">Accept</span><span class="sxs-lookup"><span data-stu-id="9618f-124">Accept</span></span>|<span data-ttu-id="9618f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9618f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9618f-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9618f-126">Request body</span></span>
<span data-ttu-id="9618f-127">Geben Sie in der Anforderungs-URL die folgenden Abfrageparameter mit Werten an.</span><span class="sxs-lookup"><span data-stu-id="9618f-127">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="9618f-128">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Funktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="9618f-128">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="9618f-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9618f-129">Property</span></span>|<span data-ttu-id="9618f-130">Typ</span><span class="sxs-lookup"><span data-stu-id="9618f-130">Type</span></span>|<span data-ttu-id="9618f-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9618f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9618f-132">scope</span><span class="sxs-lookup"><span data-stu-id="9618f-132">scope</span></span>|<span data-ttu-id="9618f-133">String</span><span class="sxs-lookup"><span data-stu-id="9618f-133">String</span></span>|<span data-ttu-id="9618f-134">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="9618f-134">Not yet documented</span></span>|


## <a name="response"></a><span data-ttu-id="9618f-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="9618f-135">Response</span></span>
<span data-ttu-id="9618f-136">Wenn die Funktion erfolgreich verläuft, werden der Antwortcode `200 OK` und eine [rolePermission](../resources/intune-rbac-rolepermission.md)-Sammlung im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9618f-136">If successful, this function returns a `200 OK` response code and a [rolePermission](../resources/intune-rbac-rolepermission.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9618f-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9618f-137">Example</span></span>
### <a name="request"></a><span data-ttu-id="9618f-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9618f-138">Request</span></span>
<span data-ttu-id="9618f-139">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9618f-139">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/getEffectivePermissions(scope='parameterValue')
```

### <a name="response"></a><span data-ttu-id="9618f-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="9618f-140">Response</span></span>
<span data-ttu-id="9618f-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9618f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 471

{
  "value": [
    {
      "@odata.type": "microsoft.graph.rolePermission",
      "actions": [
        "Actions value"
      ],
      "resourceActions": [
        {
          "@odata.type": "microsoft.graph.resourceAction",
          "allowedResourceActions": [
            "Allowed Resource Actions value"
          ],
          "notAllowedResourceActions": [
            "Not Allowed Resource Actions value"
          ]
        }
      ]
    }
  ]
}
```


