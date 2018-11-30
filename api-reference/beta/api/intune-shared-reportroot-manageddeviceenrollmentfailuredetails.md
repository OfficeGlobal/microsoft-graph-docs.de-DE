---
title: ManagedDeviceEnrollmentFailureDetails-Funktion
description: Noch nicht dokumentiert
ms.openlocfilehash: 92a06a4fae5d469759f633698abcf7bff2bfb322
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062395"
---
# <a name="manageddeviceenrollmentfailuredetails-function"></a><span data-ttu-id="bfa35-103">ManagedDeviceEnrollmentFailureDetails-Funktion</span><span class="sxs-lookup"><span data-stu-id="bfa35-103">managedDeviceEnrollmentFailureDetails function</span></span>

> <span data-ttu-id="bfa35-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="bfa35-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bfa35-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="bfa35-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bfa35-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="bfa35-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bfa35-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="bfa35-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="bfa35-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="bfa35-108">Prerequisites</span></span>
<span data-ttu-id="bfa35-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bfa35-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bfa35-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="bfa35-111">Permission type</span></span>|<span data-ttu-id="bfa35-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="bfa35-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bfa35-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="bfa35-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="bfa35-114">&nbsp; &nbsp; **Problembehandlung**</span><span class="sxs-lookup"><span data-stu-id="bfa35-114">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="bfa35-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bfa35-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="bfa35-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="bfa35-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bfa35-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bfa35-117">Not supported.</span></span>|
|<span data-ttu-id="bfa35-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="bfa35-118">Application</span></span>|<span data-ttu-id="bfa35-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bfa35-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bfa35-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="bfa35-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentFailureDetails
```

## <a name="request-headers"></a><span data-ttu-id="bfa35-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="bfa35-121">Request headers</span></span>
|<span data-ttu-id="bfa35-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="bfa35-122">Header</span></span>|<span data-ttu-id="bfa35-123">Wert</span><span class="sxs-lookup"><span data-stu-id="bfa35-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bfa35-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="bfa35-124">Authorization</span></span>|<span data-ttu-id="bfa35-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="bfa35-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bfa35-126">Accept</span><span class="sxs-lookup"><span data-stu-id="bfa35-126">Accept</span></span>|<span data-ttu-id="bfa35-127">application/json</span><span class="sxs-lookup"><span data-stu-id="bfa35-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bfa35-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="bfa35-128">Request body</span></span>
<span data-ttu-id="bfa35-129">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Funktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="bfa35-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="bfa35-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="bfa35-130">Property</span></span>|<span data-ttu-id="bfa35-131">Typ</span><span class="sxs-lookup"><span data-stu-id="bfa35-131">Type</span></span>|<span data-ttu-id="bfa35-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bfa35-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bfa35-133">Filter</span><span class="sxs-lookup"><span data-stu-id="bfa35-133">filter</span></span>|<span data-ttu-id="bfa35-134">String</span><span class="sxs-lookup"><span data-stu-id="bfa35-134">String</span></span>|<span data-ttu-id="bfa35-135">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="bfa35-135">Not yet documented</span></span>|
|<span data-ttu-id="bfa35-136">skipToken</span><span class="sxs-lookup"><span data-stu-id="bfa35-136">skipToken</span></span>|<span data-ttu-id="bfa35-137">String</span><span class="sxs-lookup"><span data-stu-id="bfa35-137">String</span></span>|<span data-ttu-id="bfa35-138">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="bfa35-138">Not yet documented</span></span>|
|<span data-ttu-id="bfa35-139">skip</span><span class="sxs-lookup"><span data-stu-id="bfa35-139">skip</span></span>|<span data-ttu-id="bfa35-140">Int32</span><span class="sxs-lookup"><span data-stu-id="bfa35-140">Int32</span></span>|<span data-ttu-id="bfa35-141">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="bfa35-141">Not yet documented</span></span>|
|<span data-ttu-id="bfa35-142">Nach oben</span><span class="sxs-lookup"><span data-stu-id="bfa35-142">top</span></span>|<span data-ttu-id="bfa35-143">Int32</span><span class="sxs-lookup"><span data-stu-id="bfa35-143">Int32</span></span>|<span data-ttu-id="bfa35-144">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="bfa35-144">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="bfa35-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="bfa35-145">Response</span></span>
<span data-ttu-id="bfa35-146">Bei erfolgreicher Ausführung gibt die Funktion den Antwortcode `200 OK` und einen [Bericht](../resources/intune-shared-report.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="bfa35-146">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bfa35-147">Beispiel</span><span class="sxs-lookup"><span data-stu-id="bfa35-147">Example</span></span>
### <a name="request"></a><span data-ttu-id="bfa35-148">Anforderung</span><span class="sxs-lookup"><span data-stu-id="bfa35-148">Request</span></span>
<span data-ttu-id="bfa35-149">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="bfa35-149">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports/managedDeviceEnrollmentFailureDetails(skip=4,top=3,filter='parameterValue',skipToken='parameterValue')
```

### <a name="response"></a><span data-ttu-id="bfa35-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="bfa35-150">Response</span></span>
<span data-ttu-id="bfa35-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="bfa35-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



