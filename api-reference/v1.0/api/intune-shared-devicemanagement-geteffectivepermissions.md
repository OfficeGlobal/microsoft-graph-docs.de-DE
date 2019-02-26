---
title: getEffectivePermissions-Funktion
description: Ruft die effektiven Berechtigungen des derzeit authentifizierten Benutzers ab.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: d6c58ae88e2b5cf9a6787529868f8cf9e42879be
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30257351"
---
# <a name="geteffectivepermissions-function"></a><span data-ttu-id="693de-103">getEffectivePermissions-Funktion</span><span class="sxs-lookup"><span data-stu-id="693de-103">getEffectivePermissions function</span></span>

> <span data-ttu-id="693de-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="693de-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="693de-105">Ruft die effektiven Berechtigungen des derzeit authentifizierten Benutzers ab.</span><span class="sxs-lookup"><span data-stu-id="693de-105">Retrieves the effective permissions of the currently authenticated user</span></span>

## <a name="prerequisites"></a><span data-ttu-id="693de-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="693de-106">Prerequisites</span></span>
<span data-ttu-id="693de-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="693de-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="693de-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="693de-109">Permission type</span></span>|<span data-ttu-id="693de-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="693de-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="693de-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="693de-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="693de-112">&nbsp;&nbsp; Rollenbasierte Zugriffssteuerung</span><span class="sxs-lookup"><span data-stu-id="693de-112">&nbsp; &nbsp; Role-based access control</span></span> | <span data-ttu-id="693de-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="693de-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="693de-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="693de-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="693de-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="693de-115">Not supported.</span></span>|
|<span data-ttu-id="693de-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="693de-116">Application</span></span>|<span data-ttu-id="693de-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="693de-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="693de-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="693de-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getEffectivePermissions
```

## <a name="request-headers"></a><span data-ttu-id="693de-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="693de-119">Request headers</span></span>
|<span data-ttu-id="693de-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="693de-120">Header</span></span>|<span data-ttu-id="693de-121">Wert</span><span class="sxs-lookup"><span data-stu-id="693de-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="693de-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="693de-122">Authorization</span></span>|<span data-ttu-id="693de-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="693de-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="693de-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="693de-124">Accept</span></span>|<span data-ttu-id="693de-125">application/json</span><span class="sxs-lookup"><span data-stu-id="693de-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="693de-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="693de-126">Request body</span></span>
<span data-ttu-id="693de-127">Geben Sie in der Anforderungs-URL die folgenden Abfrageparameter mit Werten an.</span><span class="sxs-lookup"><span data-stu-id="693de-127">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="693de-128">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Funktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="693de-128">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="693de-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="693de-129">Property</span></span>|<span data-ttu-id="693de-130">Typ</span><span class="sxs-lookup"><span data-stu-id="693de-130">Type</span></span>|<span data-ttu-id="693de-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="693de-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="693de-132">scope</span><span class="sxs-lookup"><span data-stu-id="693de-132">scope</span></span>|<span data-ttu-id="693de-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="693de-133">String</span></span>|<span data-ttu-id="693de-134">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="693de-134">Not yet documented</span></span>|


## <a name="response"></a><span data-ttu-id="693de-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="693de-135">Response</span></span>
<span data-ttu-id="693de-136">Wenn die Funktion erfolgreich verläuft, werden der Antwortcode `200 OK` und eine [rolePermission](../resources/intune-rbac-rolepermission.md)-Sammlung im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="693de-136">If successful, this function returns a `200 OK` response code and a [rolePermission](../resources/intune-rbac-rolepermission.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="693de-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="693de-137">Example</span></span>
### <a name="request"></a><span data-ttu-id="693de-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="693de-138">Request</span></span>
<span data-ttu-id="693de-139">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="693de-139">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/getEffectivePermissions(scope='parameterValue')
```

### <a name="response"></a><span data-ttu-id="693de-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="693de-140">Response</span></span>
<span data-ttu-id="693de-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="693de-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



