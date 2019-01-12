---
title: GetAssignedRoleIdsForLoggedInUser-Funktion
description: Ruft die zugewiesenen Rollendefinitionen und rollenzuweisungen des aktuell authentifizierten Benutzers ab.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b74991cfa2bd7a099adfd333129c16c796c5f9bd
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27924629"
---
# <a name="getassignedroleidsforloggedinuser-function"></a><span data-ttu-id="9274b-103">GetAssignedRoleIdsForLoggedInUser-Funktion</span><span class="sxs-lookup"><span data-stu-id="9274b-103">getAssignedRoleIdsForLoggedInUser function</span></span>

> <span data-ttu-id="9274b-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="9274b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9274b-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9274b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9274b-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="9274b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9274b-107">Ruft die zugewiesenen Rollendefinitionen und rollenzuweisungen des aktuell authentifizierten Benutzers ab.</span><span class="sxs-lookup"><span data-stu-id="9274b-107">Retrieves the assigned role definitions and role assignments of the currently authenticated user.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9274b-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="9274b-108">Prerequisites</span></span>
<span data-ttu-id="9274b-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9274b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9274b-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9274b-111">Permission type</span></span>|<span data-ttu-id="9274b-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9274b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9274b-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9274b-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="9274b-114">&nbsp;&nbsp; **Role-based Access Control (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="9274b-114">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="9274b-115">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="9274b-115">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="9274b-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9274b-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9274b-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9274b-117">Not supported.</span></span>|
|<span data-ttu-id="9274b-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9274b-118">Application</span></span>|<span data-ttu-id="9274b-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9274b-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9274b-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9274b-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getAssignedRoleIdsForLoggedInUser
```

## <a name="request-headers"></a><span data-ttu-id="9274b-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9274b-121">Request headers</span></span>
|<span data-ttu-id="9274b-122">Header</span><span class="sxs-lookup"><span data-stu-id="9274b-122">Header</span></span>|<span data-ttu-id="9274b-123">Wert</span><span class="sxs-lookup"><span data-stu-id="9274b-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9274b-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="9274b-124">Authorization</span></span>|<span data-ttu-id="9274b-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="9274b-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9274b-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="9274b-126">Accept</span></span>|<span data-ttu-id="9274b-127">application/json</span><span class="sxs-lookup"><span data-stu-id="9274b-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9274b-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9274b-128">Request body</span></span>
<span data-ttu-id="9274b-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="9274b-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9274b-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="9274b-130">Response</span></span>
<span data-ttu-id="9274b-131">Wenn erfolgreich, diese Funktion gibt eine `200 OK` Antwortcode und eine [DeviceAndAppManagementAssignedRoleIds](../resources/intune-rbac-deviceandappmanagementassignedroleids.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="9274b-131">If successful, this function returns a `200 OK` response code and a [deviceAndAppManagementAssignedRoleIds](../resources/intune-rbac-deviceandappmanagementassignedroleids.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9274b-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9274b-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="9274b-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9274b-133">Request</span></span>
<span data-ttu-id="9274b-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9274b-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/getAssignedRoleIdsForLoggedInUser
```

### <a name="response"></a><span data-ttu-id="9274b-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="9274b-135">Response</span></span>
<span data-ttu-id="9274b-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9274b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 263

{
  "value": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignedRoleIds",
    "roleDefinitionIds": [
      "df52f163-f163-df52-63f1-52df63f152df"
    ],
    "roleAssignmentIds": [
      "1f35d53d-d53d-1f35-3dd5-351f3dd5351f"
    ]
  }
}
```





