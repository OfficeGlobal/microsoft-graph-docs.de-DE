---
title: ManagedDeviceEnrollmentFailureDetails-Funktion
description: Noch nicht dokumentiert
ms.openlocfilehash: c5e68453cb1655e4018156ac207b60e4145e571a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27019060"
---
# <a name="manageddeviceenrollmentfailuredetails-function"></a><span data-ttu-id="1143e-103">ManagedDeviceEnrollmentFailureDetails-Funktion</span><span class="sxs-lookup"><span data-stu-id="1143e-103">managedDeviceEnrollmentFailureDetails function</span></span>

> <span data-ttu-id="1143e-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="1143e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1143e-105">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="1143e-105">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1143e-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="1143e-106">Prerequisites</span></span>
<span data-ttu-id="1143e-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1143e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1143e-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1143e-109">Permission type</span></span>|<span data-ttu-id="1143e-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1143e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1143e-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1143e-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="1143e-112">&nbsp;&nbsp; Problembehandlung</span><span class="sxs-lookup"><span data-stu-id="1143e-112">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="1143e-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1143e-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="1143e-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1143e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1143e-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1143e-115">Not supported.</span></span>|
|<span data-ttu-id="1143e-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1143e-116">Application</span></span>|<span data-ttu-id="1143e-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1143e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1143e-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1143e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentFailureDetails
```

## <a name="request-headers"></a><span data-ttu-id="1143e-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1143e-119">Request headers</span></span>
|<span data-ttu-id="1143e-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="1143e-120">Header</span></span>|<span data-ttu-id="1143e-121">Wert</span><span class="sxs-lookup"><span data-stu-id="1143e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1143e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1143e-122">Authorization</span></span>|<span data-ttu-id="1143e-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="1143e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1143e-124">Accept</span><span class="sxs-lookup"><span data-stu-id="1143e-124">Accept</span></span>|<span data-ttu-id="1143e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1143e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1143e-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1143e-126">Request body</span></span>
<span data-ttu-id="1143e-127">Geben Sie in der Anforderungs-URL die folgenden Abfrageparameter mit Werten an.</span><span class="sxs-lookup"><span data-stu-id="1143e-127">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="1143e-128">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Funktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="1143e-128">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="1143e-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1143e-129">Property</span></span>|<span data-ttu-id="1143e-130">Typ</span><span class="sxs-lookup"><span data-stu-id="1143e-130">Type</span></span>|<span data-ttu-id="1143e-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1143e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1143e-132">skip</span><span class="sxs-lookup"><span data-stu-id="1143e-132">skip</span></span>|<span data-ttu-id="1143e-133">Int32</span><span class="sxs-lookup"><span data-stu-id="1143e-133">Int32</span></span>|<span data-ttu-id="1143e-134">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="1143e-134">Not yet documented</span></span>|
|<span data-ttu-id="1143e-135">Nach oben</span><span class="sxs-lookup"><span data-stu-id="1143e-135">top</span></span>|<span data-ttu-id="1143e-136">Int32</span><span class="sxs-lookup"><span data-stu-id="1143e-136">Int32</span></span>|<span data-ttu-id="1143e-137">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="1143e-137">Not yet documented</span></span>|
|<span data-ttu-id="1143e-138">filter</span><span class="sxs-lookup"><span data-stu-id="1143e-138">filter</span></span>|<span data-ttu-id="1143e-139">String</span><span class="sxs-lookup"><span data-stu-id="1143e-139">String</span></span>|<span data-ttu-id="1143e-140">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="1143e-140">Not yet documented</span></span>|
|<span data-ttu-id="1143e-141">skipToken</span><span class="sxs-lookup"><span data-stu-id="1143e-141">skipToken</span></span>|<span data-ttu-id="1143e-142">String</span><span class="sxs-lookup"><span data-stu-id="1143e-142">String</span></span>|<span data-ttu-id="1143e-143">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="1143e-143">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="1143e-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="1143e-144">Response</span></span>
<span data-ttu-id="1143e-145">Bei erfolgreicher Ausführung gibt die Funktion den Antwortcode `200 OK` und einen [Bericht](../resources/intune-shared-report.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="1143e-145">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1143e-146">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1143e-146">Example</span></span>
### <a name="request"></a><span data-ttu-id="1143e-147">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1143e-147">Request</span></span>
<span data-ttu-id="1143e-148">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1143e-148">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1/reports/managedDeviceEnrollmentFailureDetails(skip=4,top=3,filter='parameterValue',skipToken='parameterValue')
```

### <a name="response"></a><span data-ttu-id="1143e-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="1143e-149">Response</span></span>
<span data-ttu-id="1143e-150">Der Kürze halber werden möglicherweise im Response-Objekt dargestellten abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="1143e-150">The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="1143e-151">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1143e-151">All of the properties will be returned from an actual call.</span></span>

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




