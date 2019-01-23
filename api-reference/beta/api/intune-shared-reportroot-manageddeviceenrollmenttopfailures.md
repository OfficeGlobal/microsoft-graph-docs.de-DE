---
title: ManagedDeviceEnrollmentTopFailures-Funktion
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: edc44099ed325455b3bd94b01aa1cec9b9582c0e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29407263"
---
# <a name="manageddeviceenrollmenttopfailures-function"></a><span data-ttu-id="244b0-103">ManagedDeviceEnrollmentTopFailures-Funktion</span><span class="sxs-lookup"><span data-stu-id="244b0-103">managedDeviceEnrollmentTopFailures function</span></span>

> <span data-ttu-id="244b0-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="244b0-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="244b0-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="244b0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="244b0-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="244b0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="244b0-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="244b0-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="244b0-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="244b0-108">Prerequisites</span></span>
<span data-ttu-id="244b0-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="244b0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="244b0-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="244b0-111">Permission type</span></span>|<span data-ttu-id="244b0-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="244b0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="244b0-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="244b0-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="244b0-114">&nbsp; &nbsp; **Problembehandlung**</span><span class="sxs-lookup"><span data-stu-id="244b0-114">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="244b0-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="244b0-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="244b0-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="244b0-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="244b0-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="244b0-117">Not supported.</span></span>|
|<span data-ttu-id="244b0-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="244b0-118">Application</span></span>|<span data-ttu-id="244b0-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="244b0-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="244b0-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="244b0-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentTopFailures
```

## <a name="request-headers"></a><span data-ttu-id="244b0-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="244b0-121">Request headers</span></span>
|<span data-ttu-id="244b0-122">Header</span><span class="sxs-lookup"><span data-stu-id="244b0-122">Header</span></span>|<span data-ttu-id="244b0-123">Wert</span><span class="sxs-lookup"><span data-stu-id="244b0-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="244b0-124">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="244b0-124">Authorization</span></span>|<span data-ttu-id="244b0-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="244b0-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="244b0-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="244b0-126">Accept</span></span>|<span data-ttu-id="244b0-127">application/json</span><span class="sxs-lookup"><span data-stu-id="244b0-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="244b0-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="244b0-128">Request body</span></span>
<span data-ttu-id="244b0-129">Geben Sie in der Anforderungs-URL die folgenden Abfrageparameter mit Werten an.</span><span class="sxs-lookup"><span data-stu-id="244b0-129">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="244b0-130">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Funktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="244b0-130">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="244b0-131">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="244b0-131">Property</span></span>|<span data-ttu-id="244b0-132">Typ</span><span class="sxs-lookup"><span data-stu-id="244b0-132">Type</span></span>|<span data-ttu-id="244b0-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="244b0-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="244b0-134">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="244b0-134">period</span></span>|<span data-ttu-id="244b0-135">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="244b0-135">String</span></span>|<span data-ttu-id="244b0-136">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="244b0-136">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="244b0-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="244b0-137">Response</span></span>
<span data-ttu-id="244b0-138">Bei erfolgreicher Ausführung gibt die Funktion den Antwortcode `200 OK` und einen [Bericht](../resources/intune-shared-report.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="244b0-138">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="244b0-139">Beispiel</span><span class="sxs-lookup"><span data-stu-id="244b0-139">Example</span></span>
### <a name="request"></a><span data-ttu-id="244b0-140">Anforderung</span><span class="sxs-lookup"><span data-stu-id="244b0-140">Request</span></span>
<span data-ttu-id="244b0-141">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="244b0-141">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports/managedDeviceEnrollmentTopFailures(period='parameterValue')
```

### <a name="response"></a><span data-ttu-id="244b0-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="244b0-142">Response</span></span>
<span data-ttu-id="244b0-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="244b0-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



