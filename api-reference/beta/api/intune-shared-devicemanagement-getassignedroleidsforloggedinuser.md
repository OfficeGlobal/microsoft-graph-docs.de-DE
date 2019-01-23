---
title: GetAssignedRoleIdsForLoggedInUser-Funktion
description: Ruft die zugewiesenen Rollendefinitionen und rollenzuweisungen des aktuell authentifizierten Benutzers ab.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: c8d1618aeece15fc482d0d850f8938d45cb53edd
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29408292"
---
# <a name="getassignedroleidsforloggedinuser-function"></a><span data-ttu-id="48424-103">GetAssignedRoleIdsForLoggedInUser-Funktion</span><span class="sxs-lookup"><span data-stu-id="48424-103">getAssignedRoleIdsForLoggedInUser function</span></span>

> <span data-ttu-id="48424-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="48424-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="48424-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="48424-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="48424-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="48424-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="48424-107">Ruft die zugewiesenen Rollendefinitionen und rollenzuweisungen des aktuell authentifizierten Benutzers ab.</span><span class="sxs-lookup"><span data-stu-id="48424-107">Retrieves the assigned role definitions and role assignments of the currently authenticated user.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="48424-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="48424-108">Prerequisites</span></span>
<span data-ttu-id="48424-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="48424-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="48424-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="48424-111">Permission type</span></span>|<span data-ttu-id="48424-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="48424-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="48424-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="48424-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="48424-114">&nbsp;&nbsp; **Role-based Access Control (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="48424-114">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="48424-115">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="48424-115">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="48424-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="48424-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="48424-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="48424-117">Not supported.</span></span>|
|<span data-ttu-id="48424-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="48424-118">Application</span></span>|<span data-ttu-id="48424-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="48424-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="48424-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="48424-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getAssignedRoleIdsForLoggedInUser
```

## <a name="request-headers"></a><span data-ttu-id="48424-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="48424-121">Request headers</span></span>
|<span data-ttu-id="48424-122">Header</span><span class="sxs-lookup"><span data-stu-id="48424-122">Header</span></span>|<span data-ttu-id="48424-123">Wert</span><span class="sxs-lookup"><span data-stu-id="48424-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="48424-124">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="48424-124">Authorization</span></span>|<span data-ttu-id="48424-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="48424-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="48424-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="48424-126">Accept</span></span>|<span data-ttu-id="48424-127">application/json</span><span class="sxs-lookup"><span data-stu-id="48424-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="48424-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="48424-128">Request body</span></span>
<span data-ttu-id="48424-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="48424-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="48424-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="48424-130">Response</span></span>
<span data-ttu-id="48424-131">Wenn erfolgreich, diese Funktion gibt eine `200 OK` Antwortcode und eine **DeviceAndAppManagementAssignedRoleId** im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="48424-131">If successful, this function returns a `200 OK` response code and a **deviceAndAppManagementAssignedRoleId** in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="48424-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="48424-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="48424-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="48424-133">Request</span></span>
<span data-ttu-id="48424-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="48424-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/getAssignedRoleIdsForLoggedInUser
```

### <a name="response"></a><span data-ttu-id="48424-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="48424-135">Response</span></span>
<span data-ttu-id="48424-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="48424-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





