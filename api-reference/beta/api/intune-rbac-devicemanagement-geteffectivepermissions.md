---
title: getEffectivePermissions-Funktion
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 18c3774515cfd680e87b84828591313e67aab60a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27885540"
---
# <a name="geteffectivepermissions-function"></a><span data-ttu-id="b03bc-103">getEffectivePermissions-Funktion</span><span class="sxs-lookup"><span data-stu-id="b03bc-103">getEffectivePermissions function</span></span>

> <span data-ttu-id="b03bc-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b03bc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b03bc-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b03bc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b03bc-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="b03bc-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b03bc-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="b03bc-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b03bc-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b03bc-108">Prerequisites</span></span>
<span data-ttu-id="b03bc-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b03bc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b03bc-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b03bc-111">Permission type</span></span>|<span data-ttu-id="b03bc-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b03bc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b03bc-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b03bc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b03bc-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="b03bc-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="b03bc-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b03bc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b03bc-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b03bc-116">Not supported.</span></span>|
|<span data-ttu-id="b03bc-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b03bc-117">Application</span></span>|<span data-ttu-id="b03bc-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b03bc-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b03bc-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b03bc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getEffectivePermissions
```

## <a name="request-headers"></a><span data-ttu-id="b03bc-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b03bc-120">Request headers</span></span>
|<span data-ttu-id="b03bc-121">Header</span><span class="sxs-lookup"><span data-stu-id="b03bc-121">Header</span></span>|<span data-ttu-id="b03bc-122">Wert</span><span class="sxs-lookup"><span data-stu-id="b03bc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b03bc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b03bc-123">Authorization</span></span>|<span data-ttu-id="b03bc-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b03bc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b03bc-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="b03bc-125">Accept</span></span>|<span data-ttu-id="b03bc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b03bc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b03bc-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b03bc-127">Request body</span></span>
<span data-ttu-id="b03bc-128">Geben Sie in der Anforderungs-URL die folgenden Abfrageparameter mit Werten an.</span><span class="sxs-lookup"><span data-stu-id="b03bc-128">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="b03bc-129">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Funktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="b03bc-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="b03bc-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b03bc-130">Property</span></span>|<span data-ttu-id="b03bc-131">Typ</span><span class="sxs-lookup"><span data-stu-id="b03bc-131">Type</span></span>|<span data-ttu-id="b03bc-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b03bc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b03bc-133">scope</span><span class="sxs-lookup"><span data-stu-id="b03bc-133">scope</span></span>|<span data-ttu-id="b03bc-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b03bc-134">String</span></span>|<span data-ttu-id="b03bc-135">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="b03bc-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="b03bc-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="b03bc-136">Response</span></span>
<span data-ttu-id="b03bc-137">Wenn die Funktion erfolgreich verläuft, werden der Antwortcode `200 OK` und eine [rolePermission](../resources/intune-rbac-rolepermission.md)-Sammlung im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b03bc-137">If successful, this function returns a `200 OK` response code and a [rolePermission](../resources/intune-rbac-rolepermission.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b03bc-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b03bc-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="b03bc-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b03bc-139">Request</span></span>
<span data-ttu-id="b03bc-140">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b03bc-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/getEffectivePermissions(scope='parameterValue')
```

### <a name="response"></a><span data-ttu-id="b03bc-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="b03bc-141">Response</span></span>
<span data-ttu-id="b03bc-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b03bc-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





