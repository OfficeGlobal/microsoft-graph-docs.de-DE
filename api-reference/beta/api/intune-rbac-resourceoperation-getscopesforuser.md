---
title: getScopesForUser-Funktion
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 39d7899d5f95ce8808ce4f1dc978aa3a0115bee8
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30161845"
---
# <a name="getscopesforuser-function"></a><span data-ttu-id="40d9c-103">getScopesForUser-Funktion</span><span class="sxs-lookup"><span data-stu-id="40d9c-103">getScopesForUser function</span></span>

> <span data-ttu-id="40d9c-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="40d9c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="40d9c-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="40d9c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="40d9c-106">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="40d9c-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="40d9c-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="40d9c-107">Prerequisites</span></span>
<span data-ttu-id="40d9c-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="40d9c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="40d9c-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="40d9c-110">Permission type</span></span>|<span data-ttu-id="40d9c-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="40d9c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="40d9c-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="40d9c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="40d9c-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="40d9c-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="40d9c-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="40d9c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="40d9c-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="40d9c-115">Not supported.</span></span>|
|<span data-ttu-id="40d9c-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="40d9c-116">Application</span></span>|<span data-ttu-id="40d9c-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="40d9c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="40d9c-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="40d9c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/resourceOperations/{resourceOperationId}/getScopesForUser
```

## <a name="request-headers"></a><span data-ttu-id="40d9c-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="40d9c-119">Request headers</span></span>
|<span data-ttu-id="40d9c-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="40d9c-120">Header</span></span>|<span data-ttu-id="40d9c-121">Wert</span><span class="sxs-lookup"><span data-stu-id="40d9c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="40d9c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="40d9c-122">Authorization</span></span>|<span data-ttu-id="40d9c-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="40d9c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="40d9c-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="40d9c-124">Accept</span></span>|<span data-ttu-id="40d9c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="40d9c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="40d9c-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="40d9c-126">Request body</span></span>
<span data-ttu-id="40d9c-127">Geben Sie in der Anforderungs-URL die folgenden Abfrageparameter mit Werten an.</span><span class="sxs-lookup"><span data-stu-id="40d9c-127">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="40d9c-128">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Funktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="40d9c-128">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="40d9c-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="40d9c-129">Property</span></span>|<span data-ttu-id="40d9c-130">Typ</span><span class="sxs-lookup"><span data-stu-id="40d9c-130">Type</span></span>|<span data-ttu-id="40d9c-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="40d9c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="40d9c-132">UserID</span><span class="sxs-lookup"><span data-stu-id="40d9c-132">userid</span></span>|<span data-ttu-id="40d9c-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="40d9c-133">String</span></span>|<span data-ttu-id="40d9c-134">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="40d9c-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="40d9c-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="40d9c-135">Response</span></span>
<span data-ttu-id="40d9c-136">Bei erfolgreicher Ausführung gibt die Funktion den Antwortcode `200 OK` und eine Collection von Objekten des Typs „String“ im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="40d9c-136">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="40d9c-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="40d9c-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="40d9c-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="40d9c-138">Request</span></span>
<span data-ttu-id="40d9c-139">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="40d9c-139">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/resourceOperations/{resourceOperationId}/getScopesForUser(userid='parameterValue')
```

### <a name="response"></a><span data-ttu-id="40d9c-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="40d9c-140">Response</span></span>
<span data-ttu-id="40d9c-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="40d9c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 56

{
  "value": [
    "Get Scopes For User value"
  ]
}
```




