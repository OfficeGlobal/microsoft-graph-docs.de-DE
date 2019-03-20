---
title: managedDeviceEnrollmentFailureDetails-Funktion
description: Noch nicht dokumentiert.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 0dff0f10c1bcfbed9bb79bcf6566bb6a329521b5
ms.sourcegitcommit: f58ff560fa02ac95e296375c143b0922fb6a425c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/19/2019
ms.locfileid: "30572292"
---
# <a name="manageddeviceenrollmentfailuredetails-function"></a><span data-ttu-id="57459-103">managedDeviceEnrollmentFailureDetails-Funktion</span><span class="sxs-lookup"><span data-stu-id="57459-103">managedDeviceEnrollmentFailureDetails function</span></span>

> <span data-ttu-id="57459-104">**Wichtig:** APIs unter der/Beta-Version in Microsoft Graph können geändert werden.</span><span class="sxs-lookup"><span data-stu-id="57459-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="57459-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="57459-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="57459-106">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="57459-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="57459-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="57459-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="57459-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="57459-108">Prerequisites</span></span>
<span data-ttu-id="57459-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="57459-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="57459-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="57459-111">Permission type</span></span>|<span data-ttu-id="57459-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="57459-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="57459-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="57459-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="57459-114">&nbsp; &nbsp; **Problembehandlung**</span><span class="sxs-lookup"><span data-stu-id="57459-114">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="57459-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57459-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="57459-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="57459-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="57459-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="57459-117">Not supported.</span></span>|
|<span data-ttu-id="57459-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="57459-118">Application</span></span>|<span data-ttu-id="57459-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="57459-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="57459-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="57459-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentFailureDetails
```

## <a name="request-headers"></a><span data-ttu-id="57459-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="57459-121">Request headers</span></span>
|<span data-ttu-id="57459-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="57459-122">Header</span></span>|<span data-ttu-id="57459-123">Wert</span><span class="sxs-lookup"><span data-stu-id="57459-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="57459-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="57459-124">Authorization</span></span>|<span data-ttu-id="57459-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="57459-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="57459-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="57459-126">Accept</span></span>|<span data-ttu-id="57459-127">application/json</span><span class="sxs-lookup"><span data-stu-id="57459-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="57459-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="57459-128">Request body</span></span>
<span data-ttu-id="57459-129">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Funktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="57459-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="57459-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="57459-130">Property</span></span>|<span data-ttu-id="57459-131">Typ</span><span class="sxs-lookup"><span data-stu-id="57459-131">Type</span></span>|<span data-ttu-id="57459-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="57459-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="57459-133">Filter</span><span class="sxs-lookup"><span data-stu-id="57459-133">filter</span></span>|<span data-ttu-id="57459-134">String</span><span class="sxs-lookup"><span data-stu-id="57459-134">String</span></span>|<span data-ttu-id="57459-135">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="57459-135">Not yet documented</span></span>|
|<span data-ttu-id="57459-136">skipToken</span><span class="sxs-lookup"><span data-stu-id="57459-136">skipToken</span></span>|<span data-ttu-id="57459-137">String</span><span class="sxs-lookup"><span data-stu-id="57459-137">String</span></span>|<span data-ttu-id="57459-138">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="57459-138">Not yet documented</span></span>|
|<span data-ttu-id="57459-139">skip</span><span class="sxs-lookup"><span data-stu-id="57459-139">skip</span></span>|<span data-ttu-id="57459-140">Int32</span><span class="sxs-lookup"><span data-stu-id="57459-140">Int32</span></span>|<span data-ttu-id="57459-141">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="57459-141">Not yet documented</span></span>|
|<span data-ttu-id="57459-142">top</span><span class="sxs-lookup"><span data-stu-id="57459-142">top</span></span>|<span data-ttu-id="57459-143">Int32</span><span class="sxs-lookup"><span data-stu-id="57459-143">Int32</span></span>|<span data-ttu-id="57459-144">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="57459-144">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="57459-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="57459-145">Response</span></span>
<span data-ttu-id="57459-146">Bei erfolgreicher Ausführung gibt die Funktion den Antwortcode `200 OK` und einen [Bericht](../resources/intune-shared-report.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="57459-146">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="57459-147">Beispiel</span><span class="sxs-lookup"><span data-stu-id="57459-147">Example</span></span>
### <a name="request"></a><span data-ttu-id="57459-148">Anforderung</span><span class="sxs-lookup"><span data-stu-id="57459-148">Request</span></span>
<span data-ttu-id="57459-149">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="57459-149">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports/managedDeviceEnrollmentFailureDetails(skip=4,top=3,filter='parameterValue',skipToken='parameterValue')
```

### <a name="response"></a><span data-ttu-id="57459-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="57459-150">Response</span></span>
<span data-ttu-id="57459-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="57459-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



