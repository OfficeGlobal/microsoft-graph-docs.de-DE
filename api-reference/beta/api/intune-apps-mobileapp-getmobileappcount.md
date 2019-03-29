---
title: getMobileAppCount-Funktion
description: Noch nicht dokumentiert.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 45cc09a26d6cb4f8b25da5e3ef914d257bba2e73
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30984856"
---
# <a name="getmobileappcount-function"></a><span data-ttu-id="f8060-103">getMobileAppCount-Funktion</span><span class="sxs-lookup"><span data-stu-id="f8060-103">getMobileAppCount function</span></span>

> <span data-ttu-id="f8060-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f8060-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f8060-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="f8060-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f8060-106">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="f8060-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f8060-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f8060-107">Prerequisites</span></span>
<span data-ttu-id="f8060-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f8060-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f8060-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f8060-110">Permission type</span></span>|<span data-ttu-id="f8060-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f8060-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f8060-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f8060-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f8060-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f8060-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="f8060-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f8060-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f8060-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f8060-115">Not supported.</span></span>|
|<span data-ttu-id="f8060-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f8060-116">Application</span></span>|<span data-ttu-id="f8060-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f8060-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f8060-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f8060-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/getMobileAppCount
```

## <a name="request-headers"></a><span data-ttu-id="f8060-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f8060-119">Request headers</span></span>
|<span data-ttu-id="f8060-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="f8060-120">Header</span></span>|<span data-ttu-id="f8060-121">Wert</span><span class="sxs-lookup"><span data-stu-id="f8060-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f8060-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f8060-122">Authorization</span></span>|<span data-ttu-id="f8060-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="f8060-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f8060-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="f8060-124">Accept</span></span>|<span data-ttu-id="f8060-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f8060-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f8060-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f8060-126">Request body</span></span>
<span data-ttu-id="f8060-127">Stellen Sie in der URL der Anforderung die folgenden Abfrageparameter mit Werten bereit.</span><span class="sxs-lookup"><span data-stu-id="f8060-127">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="f8060-128">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Funktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="f8060-128">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="f8060-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f8060-129">Property</span></span>|<span data-ttu-id="f8060-130">Typ</span><span class="sxs-lookup"><span data-stu-id="f8060-130">Type</span></span>|<span data-ttu-id="f8060-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f8060-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f8060-132">status</span><span class="sxs-lookup"><span data-stu-id="f8060-132">status</span></span>|<span data-ttu-id="f8060-133">String</span><span class="sxs-lookup"><span data-stu-id="f8060-133">String</span></span>|<span data-ttu-id="f8060-134">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="f8060-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="f8060-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="f8060-135">Response</span></span>
<span data-ttu-id="f8060-136">Bei erfolgreicher Ausführung gibt die Funktion den `200 OK` Antwortcode und ein Int64 im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="f8060-136">If successful, this function returns a `200 OK` response code and a Int64 in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f8060-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f8060-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="f8060-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f8060-138">Request</span></span>
<span data-ttu-id="f8060-139">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f8060-139">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/getMobileAppCount(status='parameterValue')
```

### <a name="response"></a><span data-ttu-id="f8060-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="f8060-140">Response</span></span>
<span data-ttu-id="f8060-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f8060-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 18

{
  "value": 1
}
```




