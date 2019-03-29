---
title: Funktion „getAuditActivityTypes“
description: Noch nicht dokumentiert.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7e326bcc85a64a98d8ec302ab425e0fbae258eb5
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30979270"
---
# <a name="getauditactivitytypes-function"></a><span data-ttu-id="5b44f-103">Funktion „getAuditActivityTypes“</span><span class="sxs-lookup"><span data-stu-id="5b44f-103">getAuditActivityTypes function</span></span>

> <span data-ttu-id="5b44f-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5b44f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5b44f-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="5b44f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5b44f-106">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="5b44f-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5b44f-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="5b44f-107">Prerequisites</span></span>
<span data-ttu-id="5b44f-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5b44f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5b44f-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5b44f-110">Permission type</span></span>|<span data-ttu-id="5b44f-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5b44f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5b44f-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5b44f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5b44f-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="5b44f-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="5b44f-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5b44f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5b44f-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5b44f-115">Not supported.</span></span>|
|<span data-ttu-id="5b44f-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5b44f-116">Application</span></span>|<span data-ttu-id="5b44f-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5b44f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5b44f-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5b44f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/auditEvents/getAuditActivityTypes
```

## <a name="request-headers"></a><span data-ttu-id="5b44f-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5b44f-119">Request headers</span></span>
|<span data-ttu-id="5b44f-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="5b44f-120">Header</span></span>|<span data-ttu-id="5b44f-121">Wert</span><span class="sxs-lookup"><span data-stu-id="5b44f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5b44f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5b44f-122">Authorization</span></span>|<span data-ttu-id="5b44f-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="5b44f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5b44f-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="5b44f-124">Accept</span></span>|<span data-ttu-id="5b44f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5b44f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5b44f-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5b44f-126">Request body</span></span>
<span data-ttu-id="5b44f-127">Stellen Sie in der URL der Anforderung die folgenden Abfrageparameter mit Werten bereit.</span><span class="sxs-lookup"><span data-stu-id="5b44f-127">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="5b44f-128">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Funktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="5b44f-128">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="5b44f-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5b44f-129">Property</span></span>|<span data-ttu-id="5b44f-130">Typ</span><span class="sxs-lookup"><span data-stu-id="5b44f-130">Type</span></span>|<span data-ttu-id="5b44f-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5b44f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5b44f-132">Kategorie</span><span class="sxs-lookup"><span data-stu-id="5b44f-132">category</span></span>|<span data-ttu-id="5b44f-133">String</span><span class="sxs-lookup"><span data-stu-id="5b44f-133">String</span></span>|<span data-ttu-id="5b44f-134">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="5b44f-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="5b44f-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="5b44f-135">Response</span></span>
<span data-ttu-id="5b44f-136">Wenn die Funktion erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Zeichenfolge-Sammlung im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5b44f-136">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5b44f-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5b44f-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="5b44f-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5b44f-138">Request</span></span>
<span data-ttu-id="5b44f-139">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5b44f-139">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/auditEvents/getAuditActivityTypes(category='parameterValue')
```

### <a name="response"></a><span data-ttu-id="5b44f-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="5b44f-140">Response</span></span>
<span data-ttu-id="5b44f-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5b44f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




