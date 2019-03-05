---
title: roleAssignments auflisten
description: Auflisten von Eigenschaften und Beziehungen der roleAssignment-Objekte.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 02914ed308a0b1f13f3480b0ea52284f08e13e91
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30258212"
---
# <a name="list-roleassignments"></a><span data-ttu-id="a4a71-103">roleAssignments auflisten</span><span class="sxs-lookup"><span data-stu-id="a4a71-103">List roleAssignments</span></span>

> <span data-ttu-id="a4a71-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="a4a71-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a4a71-105">Auflisten von Eigenschaften und Beziehungen der [roleAssignment](../resources/intune-rbac-roleassignment.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="a4a71-105">List properties and relationships of the [roleAssignment](../resources/intune-rbac-roleassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a4a71-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="a4a71-106">Prerequisites</span></span>
<span data-ttu-id="a4a71-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="a4a71-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a4a71-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a4a71-109">Permission type</span></span>|<span data-ttu-id="a4a71-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a4a71-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a4a71-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a4a71-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a4a71-112">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="a4a71-112">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="a4a71-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a4a71-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a4a71-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a4a71-114">Not supported.</span></span>|
|<span data-ttu-id="a4a71-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a4a71-115">Application</span></span>|<span data-ttu-id="a4a71-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a4a71-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a4a71-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a4a71-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="a4a71-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a4a71-118">Request headers</span></span>
|<span data-ttu-id="a4a71-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="a4a71-119">Header</span></span>|<span data-ttu-id="a4a71-120">Wert</span><span class="sxs-lookup"><span data-stu-id="a4a71-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a4a71-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a4a71-121">Authorization</span></span>|<span data-ttu-id="a4a71-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="a4a71-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a4a71-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="a4a71-123">Accept</span></span>|<span data-ttu-id="a4a71-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a4a71-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a4a71-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a4a71-125">Request body</span></span>
<span data-ttu-id="a4a71-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="a4a71-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a4a71-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="a4a71-127">Response</span></span>
<span data-ttu-id="a4a71-128">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [roleAssignment](../resources/intune-rbac-roleassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="a4a71-128">If successful, this method returns a `200 OK` response code and a collection of [roleAssignment](../resources/intune-rbac-roleassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a4a71-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a4a71-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="a4a71-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a4a71-130">Request</span></span>
<span data-ttu-id="a4a71-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a4a71-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments
```

### <a name="response"></a><span data-ttu-id="a4a71-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="a4a71-132">Response</span></span>
<span data-ttu-id="a4a71-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a4a71-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 303

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.roleAssignment",
      "id": "b3234d24-4d24-b323-244d-23b3244d23b3",
      "displayName": "Display Name value",
      "description": "Description value",
      "resourceScopes": [
        "Resource Scopes value"
      ]
    }
  ]
}
```



