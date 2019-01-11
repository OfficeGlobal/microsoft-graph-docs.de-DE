---
title: ManagedDeviceEnrollmentTopFailures-Funktion
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 4e9ff98c2ddc55110026153c854d91901ffd2335
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27882971"
---
# <a name="manageddeviceenrollmenttopfailures-function"></a><span data-ttu-id="9c7ea-103">ManagedDeviceEnrollmentTopFailures-Funktion</span><span class="sxs-lookup"><span data-stu-id="9c7ea-103">managedDeviceEnrollmentTopFailures function</span></span>

> <span data-ttu-id="9c7ea-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="9c7ea-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9c7ea-105">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="9c7ea-105">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9c7ea-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="9c7ea-106">Prerequisites</span></span>
<span data-ttu-id="9c7ea-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9c7ea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9c7ea-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9c7ea-109">Permission type</span></span>|<span data-ttu-id="9c7ea-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9c7ea-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9c7ea-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9c7ea-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="9c7ea-112">&nbsp;&nbsp; Problembehandlung</span><span class="sxs-lookup"><span data-stu-id="9c7ea-112">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="9c7ea-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9c7ea-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="9c7ea-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9c7ea-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9c7ea-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9c7ea-115">Not supported.</span></span>|
|<span data-ttu-id="9c7ea-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9c7ea-116">Application</span></span>|<span data-ttu-id="9c7ea-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9c7ea-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9c7ea-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9c7ea-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentTopFailures
```

## <a name="request-headers"></a><span data-ttu-id="9c7ea-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9c7ea-119">Request headers</span></span>
|<span data-ttu-id="9c7ea-120">Header</span><span class="sxs-lookup"><span data-stu-id="9c7ea-120">Header</span></span>|<span data-ttu-id="9c7ea-121">Wert</span><span class="sxs-lookup"><span data-stu-id="9c7ea-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9c7ea-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9c7ea-122">Authorization</span></span>|<span data-ttu-id="9c7ea-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="9c7ea-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9c7ea-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="9c7ea-124">Accept</span></span>|<span data-ttu-id="9c7ea-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9c7ea-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9c7ea-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9c7ea-126">Request body</span></span>
<span data-ttu-id="9c7ea-127">Geben Sie in der Anforderungs-URL die folgenden Abfrageparameter mit Werten an.</span><span class="sxs-lookup"><span data-stu-id="9c7ea-127">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="9c7ea-128">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Funktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="9c7ea-128">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="9c7ea-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9c7ea-129">Property</span></span>|<span data-ttu-id="9c7ea-130">Typ</span><span class="sxs-lookup"><span data-stu-id="9c7ea-130">Type</span></span>|<span data-ttu-id="9c7ea-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9c7ea-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9c7ea-132">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="9c7ea-132">period</span></span>|<span data-ttu-id="9c7ea-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9c7ea-133">String</span></span>|<span data-ttu-id="9c7ea-134">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="9c7ea-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="9c7ea-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="9c7ea-135">Response</span></span>
<span data-ttu-id="9c7ea-136">Bei erfolgreicher Ausführung gibt die Funktion den Antwortcode `200 OK` und einen [Bericht](../resources/intune-shared-report.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="9c7ea-136">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9c7ea-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9c7ea-137">Example</span></span>
### <a name="request"></a><span data-ttu-id="9c7ea-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9c7ea-138">Request</span></span>
<span data-ttu-id="9c7ea-139">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9c7ea-139">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1/reports/managedDeviceEnrollmentTopFailures(period='parameterValue')
```

### <a name="response"></a><span data-ttu-id="9c7ea-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="9c7ea-140">Response</span></span>
<span data-ttu-id="9c7ea-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9c7ea-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




