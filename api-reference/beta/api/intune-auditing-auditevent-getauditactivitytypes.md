---
title: Funktion „getAuditActivityTypes“
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b7e02ebe088be009acee817482674747e2e4b6c1
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30165604"
---
# <a name="getauditactivitytypes-function"></a><span data-ttu-id="1eef6-103">Funktion „getAuditActivityTypes“</span><span class="sxs-lookup"><span data-stu-id="1eef6-103">getAuditActivityTypes function</span></span>

> <span data-ttu-id="1eef6-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1eef6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1eef6-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="1eef6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1eef6-106">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="1eef6-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1eef6-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="1eef6-107">Prerequisites</span></span>
<span data-ttu-id="1eef6-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="1eef6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="1eef6-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1eef6-110">Permission type</span></span>|<span data-ttu-id="1eef6-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1eef6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1eef6-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1eef6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1eef6-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="1eef6-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="1eef6-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1eef6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1eef6-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1eef6-115">Not supported.</span></span>|
|<span data-ttu-id="1eef6-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1eef6-116">Application</span></span>|<span data-ttu-id="1eef6-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1eef6-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1eef6-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1eef6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/auditEvents/getAuditActivityTypes
```

## <a name="request-headers"></a><span data-ttu-id="1eef6-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1eef6-119">Request headers</span></span>
|<span data-ttu-id="1eef6-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="1eef6-120">Header</span></span>|<span data-ttu-id="1eef6-121">Wert</span><span class="sxs-lookup"><span data-stu-id="1eef6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1eef6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1eef6-122">Authorization</span></span>|<span data-ttu-id="1eef6-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="1eef6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1eef6-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="1eef6-124">Accept</span></span>|<span data-ttu-id="1eef6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1eef6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1eef6-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1eef6-126">Request body</span></span>
<span data-ttu-id="1eef6-127">Geben Sie in der Anforderungs-URL die folgenden Abfrageparameter mit Werten an.</span><span class="sxs-lookup"><span data-stu-id="1eef6-127">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="1eef6-128">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Funktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="1eef6-128">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="1eef6-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1eef6-129">Property</span></span>|<span data-ttu-id="1eef6-130">Typ</span><span class="sxs-lookup"><span data-stu-id="1eef6-130">Type</span></span>|<span data-ttu-id="1eef6-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1eef6-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1eef6-132">Kategorie</span><span class="sxs-lookup"><span data-stu-id="1eef6-132">category</span></span>|<span data-ttu-id="1eef6-133">String</span><span class="sxs-lookup"><span data-stu-id="1eef6-133">String</span></span>|<span data-ttu-id="1eef6-134">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="1eef6-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="1eef6-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="1eef6-135">Response</span></span>
<span data-ttu-id="1eef6-136">Bei erfolgreicher Ausführung gibt die Funktion den Antwortcode `200 OK` und eine Collection von Objekten des Typs „String“ im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="1eef6-136">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1eef6-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1eef6-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="1eef6-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1eef6-138">Request</span></span>
<span data-ttu-id="1eef6-139">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1eef6-139">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/auditEvents/getAuditActivityTypes(category='parameterValue')
```

### <a name="response"></a><span data-ttu-id="1eef6-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="1eef6-140">Response</span></span>
<span data-ttu-id="1eef6-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1eef6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 61

{
  "value": [
    "Get Audit Activity Types value"
  ]
}
```




