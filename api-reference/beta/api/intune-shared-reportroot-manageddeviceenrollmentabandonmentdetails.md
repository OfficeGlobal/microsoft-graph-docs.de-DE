---
title: managedDeviceEnrollmentAbandonmentDetails-Funktion
description: Metadaten für den Bericht über Registrierungs Verzichts Details
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 67cc5e74b70849df502ea5f00c39e37ed9c55c38
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/14/2019
ms.locfileid: "30571277"
---
# <a name="manageddeviceenrollmentabandonmentdetails-function"></a><span data-ttu-id="85f82-103">managedDeviceEnrollmentAbandonmentDetails-Funktion</span><span class="sxs-lookup"><span data-stu-id="85f82-103">managedDeviceEnrollmentAbandonmentDetails function</span></span>

> <span data-ttu-id="85f82-104">**Wichtig:** APIs unter der/Beta-Version in Microsoft Graph können geändert werden.</span><span class="sxs-lookup"><span data-stu-id="85f82-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="85f82-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="85f82-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="85f82-106">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="85f82-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="85f82-107">Metadaten für den Bericht über Registrierungs Verzichts Details</span><span class="sxs-lookup"><span data-stu-id="85f82-107">Metadata for Enrollment abandonment details report</span></span>
## <a name="prerequisites"></a><span data-ttu-id="85f82-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="85f82-108">Prerequisites</span></span>
<span data-ttu-id="85f82-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="85f82-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="85f82-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="85f82-111">Permission type</span></span>|<span data-ttu-id="85f82-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="85f82-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="85f82-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="85f82-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="85f82-114">&nbsp;&nbsp; **Troublshooting**</span><span class="sxs-lookup"><span data-stu-id="85f82-114">&nbsp; &nbsp; **Troublshooting**</span></span> | <span data-ttu-id="85f82-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="85f82-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="85f82-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="85f82-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="85f82-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="85f82-117">Not supported.</span></span>|
|<span data-ttu-id="85f82-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="85f82-118">Application</span></span>|<span data-ttu-id="85f82-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="85f82-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="85f82-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="85f82-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentAbandonmentDetails
```

## <a name="request-headers"></a><span data-ttu-id="85f82-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="85f82-121">Request headers</span></span>
|<span data-ttu-id="85f82-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="85f82-122">Header</span></span>|<span data-ttu-id="85f82-123">Wert</span><span class="sxs-lookup"><span data-stu-id="85f82-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="85f82-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="85f82-124">Authorization</span></span>|<span data-ttu-id="85f82-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="85f82-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="85f82-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="85f82-126">Accept</span></span>|<span data-ttu-id="85f82-127">application/json</span><span class="sxs-lookup"><span data-stu-id="85f82-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="85f82-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="85f82-128">Request body</span></span>
<span data-ttu-id="85f82-129">Stellen Sie in der URL der Anforderung die folgenden Abfrageparameter mit Werten bereit.</span><span class="sxs-lookup"><span data-stu-id="85f82-129">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="85f82-130">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Funktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="85f82-130">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="85f82-131">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="85f82-131">Property</span></span>|<span data-ttu-id="85f82-132">Typ</span><span class="sxs-lookup"><span data-stu-id="85f82-132">Type</span></span>|<span data-ttu-id="85f82-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="85f82-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="85f82-134">skip</span><span class="sxs-lookup"><span data-stu-id="85f82-134">skip</span></span>|<span data-ttu-id="85f82-135">Int32</span><span class="sxs-lookup"><span data-stu-id="85f82-135">Int32</span></span>|<span data-ttu-id="85f82-136">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="85f82-136">Not yet documented</span></span>|
|<span data-ttu-id="85f82-137">top</span><span class="sxs-lookup"><span data-stu-id="85f82-137">top</span></span>|<span data-ttu-id="85f82-138">Int32</span><span class="sxs-lookup"><span data-stu-id="85f82-138">Int32</span></span>|<span data-ttu-id="85f82-139">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="85f82-139">Not yet documented</span></span>|
|<span data-ttu-id="85f82-140">Filter</span><span class="sxs-lookup"><span data-stu-id="85f82-140">filter</span></span>|<span data-ttu-id="85f82-141">String</span><span class="sxs-lookup"><span data-stu-id="85f82-141">String</span></span>|<span data-ttu-id="85f82-142">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="85f82-142">Not yet documented</span></span>|
|<span data-ttu-id="85f82-143">skipToken</span><span class="sxs-lookup"><span data-stu-id="85f82-143">skipToken</span></span>|<span data-ttu-id="85f82-144">String</span><span class="sxs-lookup"><span data-stu-id="85f82-144">String</span></span>|<span data-ttu-id="85f82-145">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="85f82-145">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="85f82-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="85f82-146">Response</span></span>
<span data-ttu-id="85f82-147">Bei erfolgreicher Ausführung gibt die Funktion den Antwortcode `200 OK` und einen [Bericht](../resources/intune-shared-report.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="85f82-147">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="85f82-148">Beispiel</span><span class="sxs-lookup"><span data-stu-id="85f82-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="85f82-149">Anforderung</span><span class="sxs-lookup"><span data-stu-id="85f82-149">Request</span></span>
<span data-ttu-id="85f82-150">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="85f82-150">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports/managedDeviceEnrollmentAbandonmentDetails(skip=4,top=3,filter='parameterValue',skipToken='parameterValue')
```

### <a name="response"></a><span data-ttu-id="85f82-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="85f82-151">Response</span></span>
<span data-ttu-id="85f82-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="85f82-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





