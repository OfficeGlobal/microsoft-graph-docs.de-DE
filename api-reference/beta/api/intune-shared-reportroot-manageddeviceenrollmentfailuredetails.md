---
title: ManagedDeviceEnrollmentFailureDetails-Funktion
description: Noch nicht dokumentiert
author: tfitzmac
ms.openlocfilehash: f9dc6f0a1a0a211de1cbfb1443dc4393796bd2d4
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27337583"
---
# <a name="manageddeviceenrollmentfailuredetails-function"></a><span data-ttu-id="a10d6-103">ManagedDeviceEnrollmentFailureDetails-Funktion</span><span class="sxs-lookup"><span data-stu-id="a10d6-103">managedDeviceEnrollmentFailureDetails function</span></span>

> <span data-ttu-id="a10d6-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="a10d6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a10d6-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a10d6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a10d6-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="a10d6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a10d6-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="a10d6-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a10d6-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="a10d6-108">Prerequisites</span></span>
<span data-ttu-id="a10d6-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a10d6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a10d6-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a10d6-111">Permission type</span></span>|<span data-ttu-id="a10d6-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a10d6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a10d6-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a10d6-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="a10d6-114">&nbsp; &nbsp; **Problembehandlung**</span><span class="sxs-lookup"><span data-stu-id="a10d6-114">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="a10d6-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a10d6-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="a10d6-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a10d6-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a10d6-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a10d6-117">Not supported.</span></span>|
|<span data-ttu-id="a10d6-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a10d6-118">Application</span></span>|<span data-ttu-id="a10d6-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a10d6-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a10d6-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a10d6-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentFailureDetails
```

## <a name="request-headers"></a><span data-ttu-id="a10d6-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a10d6-121">Request headers</span></span>
|<span data-ttu-id="a10d6-122">Header</span><span class="sxs-lookup"><span data-stu-id="a10d6-122">Header</span></span>|<span data-ttu-id="a10d6-123">Wert</span><span class="sxs-lookup"><span data-stu-id="a10d6-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a10d6-124">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="a10d6-124">Authorization</span></span>|<span data-ttu-id="a10d6-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="a10d6-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a10d6-126">Accept</span><span class="sxs-lookup"><span data-stu-id="a10d6-126">Accept</span></span>|<span data-ttu-id="a10d6-127">application/json</span><span class="sxs-lookup"><span data-stu-id="a10d6-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a10d6-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a10d6-128">Request body</span></span>
<span data-ttu-id="a10d6-129">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Funktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="a10d6-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="a10d6-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a10d6-130">Property</span></span>|<span data-ttu-id="a10d6-131">Typ</span><span class="sxs-lookup"><span data-stu-id="a10d6-131">Type</span></span>|<span data-ttu-id="a10d6-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a10d6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a10d6-133">Filter</span><span class="sxs-lookup"><span data-stu-id="a10d6-133">filter</span></span>|<span data-ttu-id="a10d6-134">String</span><span class="sxs-lookup"><span data-stu-id="a10d6-134">String</span></span>|<span data-ttu-id="a10d6-135">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="a10d6-135">Not yet documented</span></span>|
|<span data-ttu-id="a10d6-136">skipToken</span><span class="sxs-lookup"><span data-stu-id="a10d6-136">skipToken</span></span>|<span data-ttu-id="a10d6-137">String</span><span class="sxs-lookup"><span data-stu-id="a10d6-137">String</span></span>|<span data-ttu-id="a10d6-138">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="a10d6-138">Not yet documented</span></span>|
|<span data-ttu-id="a10d6-139">skip</span><span class="sxs-lookup"><span data-stu-id="a10d6-139">skip</span></span>|<span data-ttu-id="a10d6-140">Int32</span><span class="sxs-lookup"><span data-stu-id="a10d6-140">Int32</span></span>|<span data-ttu-id="a10d6-141">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="a10d6-141">Not yet documented</span></span>|
|<span data-ttu-id="a10d6-142">Nach oben</span><span class="sxs-lookup"><span data-stu-id="a10d6-142">top</span></span>|<span data-ttu-id="a10d6-143">Int32</span><span class="sxs-lookup"><span data-stu-id="a10d6-143">Int32</span></span>|<span data-ttu-id="a10d6-144">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="a10d6-144">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="a10d6-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="a10d6-145">Response</span></span>
<span data-ttu-id="a10d6-146">Bei erfolgreicher Ausführung gibt die Funktion den Antwortcode `200 OK` und einen [Bericht](../resources/intune-shared-report.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="a10d6-146">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a10d6-147">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a10d6-147">Example</span></span>
### <a name="request"></a><span data-ttu-id="a10d6-148">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a10d6-148">Request</span></span>
<span data-ttu-id="a10d6-149">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a10d6-149">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports/managedDeviceEnrollmentFailureDetails(skip=4,top=3,filter='parameterValue',skipToken='parameterValue')
```

### <a name="response"></a><span data-ttu-id="a10d6-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="a10d6-150">Response</span></span>
<span data-ttu-id="a10d6-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a10d6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



