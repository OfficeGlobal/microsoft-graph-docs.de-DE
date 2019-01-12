---
title: ManagedDeviceEnrollmentTopFailures-Funktion
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 163a75a2ffa675f939086fecf3e9c4a155352aa1
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27934226"
---
# <a name="manageddeviceenrollmenttopfailures-function"></a><span data-ttu-id="6b39b-103">ManagedDeviceEnrollmentTopFailures-Funktion</span><span class="sxs-lookup"><span data-stu-id="6b39b-103">managedDeviceEnrollmentTopFailures function</span></span>

> <span data-ttu-id="6b39b-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="6b39b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6b39b-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6b39b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6b39b-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="6b39b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6b39b-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="6b39b-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6b39b-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="6b39b-108">Prerequisites</span></span>
<span data-ttu-id="6b39b-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6b39b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6b39b-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6b39b-111">Permission type</span></span>|<span data-ttu-id="6b39b-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6b39b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6b39b-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6b39b-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="6b39b-114">&nbsp; &nbsp; **Problembehandlung**</span><span class="sxs-lookup"><span data-stu-id="6b39b-114">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="6b39b-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b39b-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="6b39b-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6b39b-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6b39b-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6b39b-117">Not supported.</span></span>|
|<span data-ttu-id="6b39b-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6b39b-118">Application</span></span>|<span data-ttu-id="6b39b-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6b39b-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6b39b-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6b39b-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentTopFailures
```

## <a name="request-headers"></a><span data-ttu-id="6b39b-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6b39b-121">Request headers</span></span>
|<span data-ttu-id="6b39b-122">Header</span><span class="sxs-lookup"><span data-stu-id="6b39b-122">Header</span></span>|<span data-ttu-id="6b39b-123">Wert</span><span class="sxs-lookup"><span data-stu-id="6b39b-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6b39b-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="6b39b-124">Authorization</span></span>|<span data-ttu-id="6b39b-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="6b39b-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6b39b-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="6b39b-126">Accept</span></span>|<span data-ttu-id="6b39b-127">application/json</span><span class="sxs-lookup"><span data-stu-id="6b39b-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6b39b-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6b39b-128">Request body</span></span>
<span data-ttu-id="6b39b-129">Geben Sie in der Anforderungs-URL die folgenden Abfrageparameter mit Werten an.</span><span class="sxs-lookup"><span data-stu-id="6b39b-129">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="6b39b-130">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Funktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="6b39b-130">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="6b39b-131">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6b39b-131">Property</span></span>|<span data-ttu-id="6b39b-132">Typ</span><span class="sxs-lookup"><span data-stu-id="6b39b-132">Type</span></span>|<span data-ttu-id="6b39b-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6b39b-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6b39b-134">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="6b39b-134">period</span></span>|<span data-ttu-id="6b39b-135">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6b39b-135">String</span></span>|<span data-ttu-id="6b39b-136">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="6b39b-136">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="6b39b-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="6b39b-137">Response</span></span>
<span data-ttu-id="6b39b-138">Bei erfolgreicher Ausführung gibt die Funktion den Antwortcode `200 OK` und einen [Bericht](../resources/intune-shared-report.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="6b39b-138">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6b39b-139">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6b39b-139">Example</span></span>
### <a name="request"></a><span data-ttu-id="6b39b-140">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6b39b-140">Request</span></span>
<span data-ttu-id="6b39b-141">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6b39b-141">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports/managedDeviceEnrollmentTopFailures(period='parameterValue')
```

### <a name="response"></a><span data-ttu-id="6b39b-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="6b39b-142">Response</span></span>
<span data-ttu-id="6b39b-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6b39b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



