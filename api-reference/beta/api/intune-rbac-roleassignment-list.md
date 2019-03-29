---
title: roleAssignments auflisten
description: Auflisten von Eigenschaften und Beziehungen der roleAssignment-Objekte.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e83729a78bd5230f447c2542bcdcf3e59a6ba928
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30957899"
---
# <a name="list-roleassignments"></a><span data-ttu-id="22445-103">roleAssignments auflisten</span><span class="sxs-lookup"><span data-stu-id="22445-103">List roleAssignments</span></span>

> <span data-ttu-id="22445-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="22445-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="22445-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="22445-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="22445-106">Auflisten von Eigenschaften und Beziehungen der [roleAssignment](../resources/intune-rbac-roleassignment.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="22445-106">List properties and relationships of the [roleAssignment](../resources/intune-rbac-roleassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="22445-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="22445-107">Prerequisites</span></span>
<span data-ttu-id="22445-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="22445-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="22445-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="22445-110">Permission type</span></span>|<span data-ttu-id="22445-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="22445-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="22445-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="22445-112">Delegated (work or school account)</span></span>|<span data-ttu-id="22445-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="22445-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="22445-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="22445-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="22445-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="22445-115">Not supported.</span></span>|
|<span data-ttu-id="22445-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="22445-116">Application</span></span>|<span data-ttu-id="22445-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="22445-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="22445-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="22445-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="22445-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="22445-119">Request headers</span></span>
|<span data-ttu-id="22445-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="22445-120">Header</span></span>|<span data-ttu-id="22445-121">Wert</span><span class="sxs-lookup"><span data-stu-id="22445-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="22445-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="22445-122">Authorization</span></span>|<span data-ttu-id="22445-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="22445-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="22445-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="22445-124">Accept</span></span>|<span data-ttu-id="22445-125">application/json</span><span class="sxs-lookup"><span data-stu-id="22445-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="22445-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="22445-126">Request body</span></span>
<span data-ttu-id="22445-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="22445-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="22445-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="22445-128">Response</span></span>
<span data-ttu-id="22445-129">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [roleAssignment](../resources/intune-rbac-roleassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="22445-129">If successful, this method returns a `200 OK` response code and a collection of [roleAssignment](../resources/intune-rbac-roleassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="22445-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="22445-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="22445-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="22445-131">Request</span></span>
<span data-ttu-id="22445-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="22445-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments
```

### <a name="response"></a><span data-ttu-id="22445-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="22445-133">Response</span></span>
<span data-ttu-id="22445-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="22445-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 403

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.roleAssignment",
      "id": "b3234d24-4d24-b323-244d-23b3244d23b3",
      "displayName": "Display Name value",
      "description": "Description value",
      "scopeMembers": [
        "Scope Members value"
      ],
      "scopeType": "allDevices",
      "resourceScopes": [
        "Resource Scopes value"
      ]
    }
  ]
}
```




