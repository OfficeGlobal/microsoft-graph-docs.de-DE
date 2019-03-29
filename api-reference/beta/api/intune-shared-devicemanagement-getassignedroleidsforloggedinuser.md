---
title: getAssignedRoleIdsForLoggedInUser-Funktion
description: Ruft die zugewiesenen Rollendefinitionen und Rollenzuweisungen des derzeit authentifizierten Benutzers ab.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: c8d1618aeece15fc482d0d850f8938d45cb53edd
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30981370"
---
# <a name="getassignedroleidsforloggedinuser-function"></a><span data-ttu-id="5533d-103">getAssignedRoleIdsForLoggedInUser-Funktion</span><span class="sxs-lookup"><span data-stu-id="5533d-103">getAssignedRoleIdsForLoggedInUser function</span></span>

> <span data-ttu-id="5533d-104">**Wichtig:** APIs unter der/Beta-Version in Microsoft Graph können geändert werden.</span><span class="sxs-lookup"><span data-stu-id="5533d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="5533d-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5533d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5533d-106">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="5533d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5533d-107">Ruft die zugewiesenen Rollendefinitionen und Rollenzuweisungen des derzeit authentifizierten Benutzers ab.</span><span class="sxs-lookup"><span data-stu-id="5533d-107">Retrieves the assigned role definitions and role assignments of the currently authenticated user.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5533d-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="5533d-108">Prerequisites</span></span>
<span data-ttu-id="5533d-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5533d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5533d-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5533d-111">Permission type</span></span>|<span data-ttu-id="5533d-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5533d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5533d-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5533d-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="5533d-114">&nbsp; &nbsp; **Rollenbasierte Zugriffssteuerung (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="5533d-114">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="5533d-115">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="5533d-115">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="5533d-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5533d-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5533d-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5533d-117">Not supported.</span></span>|
|<span data-ttu-id="5533d-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5533d-118">Application</span></span>|<span data-ttu-id="5533d-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5533d-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5533d-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5533d-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getAssignedRoleIdsForLoggedInUser
```

## <a name="request-headers"></a><span data-ttu-id="5533d-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5533d-121">Request headers</span></span>
|<span data-ttu-id="5533d-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="5533d-122">Header</span></span>|<span data-ttu-id="5533d-123">Wert</span><span class="sxs-lookup"><span data-stu-id="5533d-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5533d-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="5533d-124">Authorization</span></span>|<span data-ttu-id="5533d-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="5533d-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5533d-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="5533d-126">Accept</span></span>|<span data-ttu-id="5533d-127">application/json</span><span class="sxs-lookup"><span data-stu-id="5533d-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5533d-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5533d-128">Request body</span></span>
<span data-ttu-id="5533d-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="5533d-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5533d-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="5533d-130">Response</span></span>
<span data-ttu-id="5533d-131">Bei erfolgreicher Ausführung gibt die Funktion den `200 OK` Antwortcode und eine **deviceAndAppManagementAssignedRoleId** im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="5533d-131">If successful, this function returns a `200 OK` response code and a **deviceAndAppManagementAssignedRoleId** in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5533d-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5533d-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="5533d-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5533d-133">Request</span></span>
<span data-ttu-id="5533d-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5533d-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/getAssignedRoleIdsForLoggedInUser
```

### <a name="response"></a><span data-ttu-id="5533d-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="5533d-135">Response</span></span>
<span data-ttu-id="5533d-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5533d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





