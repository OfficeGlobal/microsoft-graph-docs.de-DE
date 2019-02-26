---
title: managedDeviceEnrollmentTopFailures-Funktion
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 2cdc523507964f87863131ef114b102f383524a8
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30250453"
---
# <a name="manageddeviceenrollmenttopfailures-function"></a><span data-ttu-id="86141-103">managedDeviceEnrollmentTopFailures-Funktion</span><span class="sxs-lookup"><span data-stu-id="86141-103">managedDeviceEnrollmentTopFailures function</span></span>

> <span data-ttu-id="86141-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="86141-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="86141-105">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="86141-105">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="86141-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="86141-106">Prerequisites</span></span>
<span data-ttu-id="86141-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="86141-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="86141-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="86141-109">Permission type</span></span>|<span data-ttu-id="86141-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="86141-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="86141-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="86141-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="86141-112">&nbsp;&nbsp; Problembehandlung</span><span class="sxs-lookup"><span data-stu-id="86141-112">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="86141-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="86141-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="86141-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="86141-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="86141-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="86141-115">Not supported.</span></span>|
|<span data-ttu-id="86141-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="86141-116">Application</span></span>|<span data-ttu-id="86141-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="86141-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="86141-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="86141-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentTopFailures
```

## <a name="request-headers"></a><span data-ttu-id="86141-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="86141-119">Request headers</span></span>
|<span data-ttu-id="86141-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="86141-120">Header</span></span>|<span data-ttu-id="86141-121">Wert</span><span class="sxs-lookup"><span data-stu-id="86141-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="86141-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="86141-122">Authorization</span></span>|<span data-ttu-id="86141-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="86141-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="86141-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="86141-124">Accept</span></span>|<span data-ttu-id="86141-125">application/json</span><span class="sxs-lookup"><span data-stu-id="86141-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="86141-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="86141-126">Request body</span></span>
<span data-ttu-id="86141-127">Geben Sie in der Anforderungs-URL die folgenden Abfrageparameter mit Werten an.</span><span class="sxs-lookup"><span data-stu-id="86141-127">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="86141-128">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Funktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="86141-128">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="86141-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="86141-129">Property</span></span>|<span data-ttu-id="86141-130">Typ</span><span class="sxs-lookup"><span data-stu-id="86141-130">Type</span></span>|<span data-ttu-id="86141-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="86141-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="86141-132">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="86141-132">period</span></span>|<span data-ttu-id="86141-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="86141-133">String</span></span>|<span data-ttu-id="86141-134">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="86141-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="86141-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="86141-135">Response</span></span>
<span data-ttu-id="86141-136">Bei erfolgreicher Ausführung gibt die Funktion den Antwortcode `200 OK` und einen [Bericht](../resources/intune-shared-report.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="86141-136">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="86141-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="86141-137">Example</span></span>
### <a name="request"></a><span data-ttu-id="86141-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="86141-138">Request</span></span>
<span data-ttu-id="86141-139">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="86141-139">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1/reports/managedDeviceEnrollmentTopFailures(period='parameterValue')
```

### <a name="response"></a><span data-ttu-id="86141-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="86141-140">Response</span></span>
<span data-ttu-id="86141-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="86141-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




