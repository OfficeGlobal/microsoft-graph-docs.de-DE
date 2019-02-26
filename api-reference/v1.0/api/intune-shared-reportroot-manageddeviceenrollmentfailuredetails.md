---
title: managedDeviceEnrollmentFailureDetails-Funktion
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: c234181bb70ca0df11cff01b67eb7d6fa60e27ca
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30262993"
---
# <a name="manageddeviceenrollmentfailuredetails-function"></a><span data-ttu-id="bdea8-103">managedDeviceEnrollmentFailureDetails-Funktion</span><span class="sxs-lookup"><span data-stu-id="bdea8-103">managedDeviceEnrollmentFailureDetails function</span></span>

> <span data-ttu-id="bdea8-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="bdea8-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bdea8-105">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="bdea8-105">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bdea8-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="bdea8-106">Prerequisites</span></span>
<span data-ttu-id="bdea8-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bdea8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bdea8-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="bdea8-109">Permission type</span></span>|<span data-ttu-id="bdea8-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="bdea8-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bdea8-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="bdea8-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="bdea8-112">&nbsp;&nbsp; Problembehandlung</span><span class="sxs-lookup"><span data-stu-id="bdea8-112">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="bdea8-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bdea8-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="bdea8-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="bdea8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bdea8-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bdea8-115">Not supported.</span></span>|
|<span data-ttu-id="bdea8-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="bdea8-116">Application</span></span>|<span data-ttu-id="bdea8-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bdea8-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bdea8-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="bdea8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentFailureDetails
```

## <a name="request-headers"></a><span data-ttu-id="bdea8-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="bdea8-119">Request headers</span></span>
|<span data-ttu-id="bdea8-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="bdea8-120">Header</span></span>|<span data-ttu-id="bdea8-121">Wert</span><span class="sxs-lookup"><span data-stu-id="bdea8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bdea8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="bdea8-122">Authorization</span></span>|<span data-ttu-id="bdea8-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="bdea8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bdea8-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="bdea8-124">Accept</span></span>|<span data-ttu-id="bdea8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="bdea8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bdea8-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="bdea8-126">Request body</span></span>
<span data-ttu-id="bdea8-127">Geben Sie in der Anforderungs-URL die folgenden Abfrageparameter mit Werten an.</span><span class="sxs-lookup"><span data-stu-id="bdea8-127">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="bdea8-128">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Funktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="bdea8-128">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="bdea8-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="bdea8-129">Property</span></span>|<span data-ttu-id="bdea8-130">Typ</span><span class="sxs-lookup"><span data-stu-id="bdea8-130">Type</span></span>|<span data-ttu-id="bdea8-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bdea8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bdea8-132">skip</span><span class="sxs-lookup"><span data-stu-id="bdea8-132">skip</span></span>|<span data-ttu-id="bdea8-133">Int32</span><span class="sxs-lookup"><span data-stu-id="bdea8-133">Int32</span></span>|<span data-ttu-id="bdea8-134">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="bdea8-134">Not yet documented</span></span>|
|<span data-ttu-id="bdea8-135">top</span><span class="sxs-lookup"><span data-stu-id="bdea8-135">top</span></span>|<span data-ttu-id="bdea8-136">Int32</span><span class="sxs-lookup"><span data-stu-id="bdea8-136">Int32</span></span>|<span data-ttu-id="bdea8-137">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="bdea8-137">Not yet documented</span></span>|
|<span data-ttu-id="bdea8-138">filter</span><span class="sxs-lookup"><span data-stu-id="bdea8-138">filter</span></span>|<span data-ttu-id="bdea8-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bdea8-139">String</span></span>|<span data-ttu-id="bdea8-140">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="bdea8-140">Not yet documented</span></span>|
|<span data-ttu-id="bdea8-141">skipToken</span><span class="sxs-lookup"><span data-stu-id="bdea8-141">skipToken</span></span>|<span data-ttu-id="bdea8-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bdea8-142">String</span></span>|<span data-ttu-id="bdea8-143">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="bdea8-143">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="bdea8-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="bdea8-144">Response</span></span>
<span data-ttu-id="bdea8-145">Bei erfolgreicher Ausführung gibt die Funktion den Antwortcode `200 OK` und einen [Bericht](../resources/intune-shared-report.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="bdea8-145">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bdea8-146">Beispiel</span><span class="sxs-lookup"><span data-stu-id="bdea8-146">Example</span></span>
### <a name="request"></a><span data-ttu-id="bdea8-147">Anforderung</span><span class="sxs-lookup"><span data-stu-id="bdea8-147">Request</span></span>
<span data-ttu-id="bdea8-148">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="bdea8-148">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1/reports/managedDeviceEnrollmentFailureDetails(skip=4,top=3,filter='parameterValue',skipToken='parameterValue')
```

### <a name="response"></a><span data-ttu-id="bdea8-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="bdea8-149">Response</span></span>
<span data-ttu-id="bdea8-150">Das hier gezeigte Antwortobjekt kann zur Kürze abgeschnitten werden.</span><span class="sxs-lookup"><span data-stu-id="bdea8-150">The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="bdea8-151">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="bdea8-151">All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 123

{
  "value": {
    "@odata.type": "microsoft.graph.report",
    "content": "<Unknown Primitive Type Edm.Stream>"
  }
}
```




