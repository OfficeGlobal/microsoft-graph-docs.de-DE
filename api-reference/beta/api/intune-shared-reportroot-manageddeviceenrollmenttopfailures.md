---
title: managedDeviceEnrollmentTopFailures-Funktion
description: Noch nicht dokumentiert.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 0730f98e1cd46b78091eb4ff44f6c08c52d2db8a
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/14/2019
ms.locfileid: "30570921"
---
# <a name="manageddeviceenrollmenttopfailures-function"></a><span data-ttu-id="7b8b2-103">managedDeviceEnrollmentTopFailures-Funktion</span><span class="sxs-lookup"><span data-stu-id="7b8b2-103">managedDeviceEnrollmentTopFailures function</span></span>

> <span data-ttu-id="7b8b2-104">**Wichtig:** APIs unter der/Beta-Version in Microsoft Graph können geändert werden.</span><span class="sxs-lookup"><span data-stu-id="7b8b2-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="7b8b2-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7b8b2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7b8b2-106">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="7b8b2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7b8b2-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="7b8b2-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7b8b2-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="7b8b2-108">Prerequisites</span></span>
<span data-ttu-id="7b8b2-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="7b8b2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="7b8b2-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7b8b2-111">Permission type</span></span>|<span data-ttu-id="7b8b2-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7b8b2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7b8b2-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7b8b2-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="7b8b2-114">&nbsp; &nbsp; **Problembehandlung**</span><span class="sxs-lookup"><span data-stu-id="7b8b2-114">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="7b8b2-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7b8b2-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="7b8b2-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7b8b2-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7b8b2-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7b8b2-117">Not supported.</span></span>|
|<span data-ttu-id="7b8b2-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7b8b2-118">Application</span></span>|<span data-ttu-id="7b8b2-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7b8b2-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7b8b2-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7b8b2-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentTopFailures
```

## <a name="request-headers"></a><span data-ttu-id="7b8b2-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7b8b2-121">Request headers</span></span>
|<span data-ttu-id="7b8b2-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="7b8b2-122">Header</span></span>|<span data-ttu-id="7b8b2-123">Wert</span><span class="sxs-lookup"><span data-stu-id="7b8b2-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7b8b2-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="7b8b2-124">Authorization</span></span>|<span data-ttu-id="7b8b2-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="7b8b2-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7b8b2-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="7b8b2-126">Accept</span></span>|<span data-ttu-id="7b8b2-127">application/json</span><span class="sxs-lookup"><span data-stu-id="7b8b2-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7b8b2-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7b8b2-128">Request body</span></span>
<span data-ttu-id="7b8b2-129">Stellen Sie in der URL der Anforderung die folgenden Abfrageparameter mit Werten bereit.</span><span class="sxs-lookup"><span data-stu-id="7b8b2-129">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="7b8b2-130">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Funktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="7b8b2-130">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="7b8b2-131">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7b8b2-131">Property</span></span>|<span data-ttu-id="7b8b2-132">Typ</span><span class="sxs-lookup"><span data-stu-id="7b8b2-132">Type</span></span>|<span data-ttu-id="7b8b2-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7b8b2-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7b8b2-134">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="7b8b2-134">period</span></span>|<span data-ttu-id="7b8b2-135">String</span><span class="sxs-lookup"><span data-stu-id="7b8b2-135">String</span></span>|<span data-ttu-id="7b8b2-136">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="7b8b2-136">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="7b8b2-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="7b8b2-137">Response</span></span>
<span data-ttu-id="7b8b2-138">Bei erfolgreicher Ausführung gibt die Funktion den Antwortcode `200 OK` und einen [Bericht](../resources/intune-shared-report.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="7b8b2-138">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7b8b2-139">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7b8b2-139">Example</span></span>
### <a name="request"></a><span data-ttu-id="7b8b2-140">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7b8b2-140">Request</span></span>
<span data-ttu-id="7b8b2-141">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7b8b2-141">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports/managedDeviceEnrollmentTopFailures(period='parameterValue')
```

### <a name="response"></a><span data-ttu-id="7b8b2-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="7b8b2-142">Response</span></span>
<span data-ttu-id="7b8b2-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7b8b2-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



