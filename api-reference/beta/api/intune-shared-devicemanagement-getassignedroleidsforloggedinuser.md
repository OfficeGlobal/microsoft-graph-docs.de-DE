---
title: GetAssignedRoleIdsForLoggedInUser-Funktion
description: Ruft die zugewiesenen Rollendefinitionen und rollenzuweisungen des aktuell authentifizierten Benutzers ab.
ms.openlocfilehash: c97e701bfd35961d9fb15022500bb06727c7e89a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060692"
---
# <a name="getassignedroleidsforloggedinuser-function"></a><span data-ttu-id="d3063-103">GetAssignedRoleIdsForLoggedInUser-Funktion</span><span class="sxs-lookup"><span data-stu-id="d3063-103">getAssignedRoleIdsForLoggedInUser function</span></span>

> <span data-ttu-id="d3063-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="d3063-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d3063-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d3063-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d3063-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="d3063-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d3063-107">Ruft die zugewiesenen Rollendefinitionen und rollenzuweisungen des aktuell authentifizierten Benutzers ab.</span><span class="sxs-lookup"><span data-stu-id="d3063-107">Retrieves the assigned role definitions and role assignments of the currently authenticated user.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d3063-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="d3063-108">Prerequisites</span></span>
<span data-ttu-id="d3063-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d3063-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d3063-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d3063-111">Permission type</span></span>|<span data-ttu-id="d3063-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d3063-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d3063-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d3063-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="d3063-114">&nbsp;&nbsp; **Role-based Access Control (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="d3063-114">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="d3063-115">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="d3063-115">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="d3063-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d3063-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d3063-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d3063-117">Not supported.</span></span>|
|<span data-ttu-id="d3063-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d3063-118">Application</span></span>|<span data-ttu-id="d3063-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d3063-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d3063-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d3063-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getAssignedRoleIdsForLoggedInUser
```

## <a name="request-headers"></a><span data-ttu-id="d3063-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d3063-121">Request headers</span></span>
|<span data-ttu-id="d3063-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="d3063-122">Header</span></span>|<span data-ttu-id="d3063-123">Wert</span><span class="sxs-lookup"><span data-stu-id="d3063-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d3063-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="d3063-124">Authorization</span></span>|<span data-ttu-id="d3063-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="d3063-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d3063-126">Accept</span><span class="sxs-lookup"><span data-stu-id="d3063-126">Accept</span></span>|<span data-ttu-id="d3063-127">application/json</span><span class="sxs-lookup"><span data-stu-id="d3063-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d3063-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d3063-128">Request body</span></span>
<span data-ttu-id="d3063-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="d3063-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d3063-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="d3063-130">Response</span></span>
<span data-ttu-id="d3063-131">Wenn erfolgreich, diese Funktion gibt eine `200 OK` Antwortcode und eine [DeviceAndAppManagementAssignedRoleIds](../resources/intune-rbac-deviceandappmanagementassignedroleids.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="d3063-131">If successful, this function returns a `200 OK` response code and a [deviceAndAppManagementAssignedRoleIds](../resources/intune-rbac-deviceandappmanagementassignedroleids.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d3063-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d3063-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="d3063-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d3063-133">Request</span></span>
<span data-ttu-id="d3063-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d3063-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/getAssignedRoleIdsForLoggedInUser
```

### <a name="response"></a><span data-ttu-id="d3063-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="d3063-135">Response</span></span>
<span data-ttu-id="d3063-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d3063-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





