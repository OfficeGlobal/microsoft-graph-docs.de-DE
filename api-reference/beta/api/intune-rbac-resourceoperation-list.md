---
title: resourceOperations auflisten
description: Listet die Eigenschaften und Beziehungen von Objekten des Typs resourceOperation auf.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 555862ec61d17aa11afd3da6d957f9bf0ce03966
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30983421"
---
# <a name="list-resourceoperations"></a><span data-ttu-id="6650f-103">resourceOperations auflisten</span><span class="sxs-lookup"><span data-stu-id="6650f-103">List resourceOperations</span></span>

> <span data-ttu-id="6650f-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6650f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6650f-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="6650f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6650f-106">Listet die Eigenschaften und Beziehungen von Objekten des Typs [resourceOperation](../resources/intune-rbac-resourceoperation.md) auf.</span><span class="sxs-lookup"><span data-stu-id="6650f-106">List properties and relationships of the [resourceOperation](../resources/intune-rbac-resourceoperation.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6650f-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="6650f-107">Prerequisites</span></span>
<span data-ttu-id="6650f-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6650f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6650f-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6650f-110">Permission type</span></span>|<span data-ttu-id="6650f-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6650f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6650f-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6650f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6650f-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="6650f-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="6650f-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6650f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6650f-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6650f-115">Not supported.</span></span>|
|<span data-ttu-id="6650f-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6650f-116">Application</span></span>|<span data-ttu-id="6650f-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6650f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6650f-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6650f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/resourceOperations
```

## <a name="request-headers"></a><span data-ttu-id="6650f-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6650f-119">Request headers</span></span>
|<span data-ttu-id="6650f-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="6650f-120">Header</span></span>|<span data-ttu-id="6650f-121">Wert</span><span class="sxs-lookup"><span data-stu-id="6650f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6650f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6650f-122">Authorization</span></span>|<span data-ttu-id="6650f-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="6650f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6650f-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="6650f-124">Accept</span></span>|<span data-ttu-id="6650f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6650f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6650f-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6650f-126">Request body</span></span>
<span data-ttu-id="6650f-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="6650f-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6650f-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="6650f-128">Response</span></span>
<span data-ttu-id="6650f-129">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [resourceOperation](../resources/intune-rbac-resourceoperation.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6650f-129">If successful, this method returns a `200 OK` response code and a collection of [resourceOperation](../resources/intune-rbac-resourceoperation.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6650f-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6650f-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="6650f-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6650f-131">Request</span></span>
<span data-ttu-id="6650f-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6650f-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/resourceOperations
```

### <a name="response"></a><span data-ttu-id="6650f-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="6650f-133">Response</span></span>
<span data-ttu-id="6650f-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6650f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




