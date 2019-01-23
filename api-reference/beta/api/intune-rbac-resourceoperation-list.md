---
title: resourceOperations auflisten
description: Listet die Eigenschaften und Beziehungen von Objekten des Typs resourceOperation auf.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c263445c4083b70bf6d9ea11950c9d756f4fae1a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396679"
---
# <a name="list-resourceoperations"></a><span data-ttu-id="d9b04-103">resourceOperations auflisten</span><span class="sxs-lookup"><span data-stu-id="d9b04-103">List resourceOperations</span></span>

> <span data-ttu-id="d9b04-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="d9b04-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d9b04-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d9b04-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d9b04-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d9b04-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d9b04-107">Listet die Eigenschaften und Beziehungen von Objekten des Typs [resourceOperation](../resources/intune-rbac-resourceoperation.md) auf.</span><span class="sxs-lookup"><span data-stu-id="d9b04-107">List properties and relationships of the [resourceOperation](../resources/intune-rbac-resourceoperation.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d9b04-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="d9b04-108">Prerequisites</span></span>
<span data-ttu-id="d9b04-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="d9b04-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="d9b04-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d9b04-111">Permission type</span></span>|<span data-ttu-id="d9b04-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d9b04-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d9b04-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d9b04-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d9b04-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="d9b04-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="d9b04-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d9b04-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d9b04-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d9b04-116">Not supported.</span></span>|
|<span data-ttu-id="d9b04-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d9b04-117">Application</span></span>|<span data-ttu-id="d9b04-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d9b04-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d9b04-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d9b04-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/resourceOperations
```

## <a name="request-headers"></a><span data-ttu-id="d9b04-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d9b04-120">Request headers</span></span>
|<span data-ttu-id="d9b04-121">Header</span><span class="sxs-lookup"><span data-stu-id="d9b04-121">Header</span></span>|<span data-ttu-id="d9b04-122">Wert</span><span class="sxs-lookup"><span data-stu-id="d9b04-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d9b04-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="d9b04-123">Authorization</span></span>|<span data-ttu-id="d9b04-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="d9b04-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d9b04-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="d9b04-125">Accept</span></span>|<span data-ttu-id="d9b04-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d9b04-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d9b04-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d9b04-127">Request body</span></span>
<span data-ttu-id="d9b04-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="d9b04-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d9b04-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="d9b04-129">Response</span></span>
<span data-ttu-id="d9b04-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [resourceOperation](../resources/intune-rbac-resourceoperation.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d9b04-130">If successful, this method returns a `200 OK` response code and a collection of [resourceOperation](../resources/intune-rbac-resourceoperation.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d9b04-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d9b04-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="d9b04-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d9b04-132">Request</span></span>
<span data-ttu-id="d9b04-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d9b04-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/resourceOperations
```

### <a name="response"></a><span data-ttu-id="d9b04-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="d9b04-134">Response</span></span>
<span data-ttu-id="d9b04-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d9b04-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 359

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.resourceOperation",
      "id": "232b8fee-8fee-232b-ee8f-2b23ee8f2b23",
      "resource": "Resource value",
      "resourceName": "Resource Name value",
      "actionName": "Action Name value",
      "description": "Description value",
      "enabledForScopeValidation": true
    }
  ]
}
```




