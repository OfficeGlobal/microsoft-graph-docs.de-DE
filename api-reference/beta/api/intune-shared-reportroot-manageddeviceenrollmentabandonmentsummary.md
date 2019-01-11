---
title: ManagedDeviceEnrollmentAbandonmentSummary-Funktion
description: Metadaten für die Registrierung Aufgabe Zusammenfassungsbericht
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: c96df67827857e763d67329ce83a81d3bfa39720
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27885400"
---
# <a name="manageddeviceenrollmentabandonmentsummary-function"></a><span data-ttu-id="1daed-103">ManagedDeviceEnrollmentAbandonmentSummary-Funktion</span><span class="sxs-lookup"><span data-stu-id="1daed-103">managedDeviceEnrollmentAbandonmentSummary function</span></span>

> <span data-ttu-id="1daed-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="1daed-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1daed-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1daed-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1daed-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="1daed-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1daed-107">Metadaten für die Registrierung Aufgabe Zusammenfassungsbericht</span><span class="sxs-lookup"><span data-stu-id="1daed-107">Metadata for Enrollment abandonment summary report</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1daed-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="1daed-108">Prerequisites</span></span>
<span data-ttu-id="1daed-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1daed-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1daed-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1daed-111">Permission type</span></span>|<span data-ttu-id="1daed-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1daed-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1daed-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1daed-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="1daed-114">&nbsp;&nbsp; **Behandelt Probleme mit**</span><span class="sxs-lookup"><span data-stu-id="1daed-114">&nbsp; &nbsp; **Troublshooting**</span></span> | <span data-ttu-id="1daed-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="1daed-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="1daed-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1daed-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1daed-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1daed-117">Not supported.</span></span>|
|<span data-ttu-id="1daed-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1daed-118">Application</span></span>|<span data-ttu-id="1daed-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1daed-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1daed-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1daed-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentAbandonmentSummary
```

## <a name="request-headers"></a><span data-ttu-id="1daed-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1daed-121">Request headers</span></span>
|<span data-ttu-id="1daed-122">Header</span><span class="sxs-lookup"><span data-stu-id="1daed-122">Header</span></span>|<span data-ttu-id="1daed-123">Wert</span><span class="sxs-lookup"><span data-stu-id="1daed-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1daed-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="1daed-124">Authorization</span></span>|<span data-ttu-id="1daed-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="1daed-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1daed-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="1daed-126">Accept</span></span>|<span data-ttu-id="1daed-127">application/json</span><span class="sxs-lookup"><span data-stu-id="1daed-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1daed-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1daed-128">Request body</span></span>
<span data-ttu-id="1daed-129">Geben Sie in der Anforderungs-URL die folgenden Abfrageparameter mit Werten an.</span><span class="sxs-lookup"><span data-stu-id="1daed-129">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="1daed-130">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Funktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="1daed-130">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="1daed-131">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1daed-131">Property</span></span>|<span data-ttu-id="1daed-132">Typ</span><span class="sxs-lookup"><span data-stu-id="1daed-132">Type</span></span>|<span data-ttu-id="1daed-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1daed-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1daed-134">skip</span><span class="sxs-lookup"><span data-stu-id="1daed-134">skip</span></span>|<span data-ttu-id="1daed-135">Int32</span><span class="sxs-lookup"><span data-stu-id="1daed-135">Int32</span></span>|<span data-ttu-id="1daed-136">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="1daed-136">Not yet documented</span></span>|
|<span data-ttu-id="1daed-137">Nach oben</span><span class="sxs-lookup"><span data-stu-id="1daed-137">top</span></span>|<span data-ttu-id="1daed-138">Int32</span><span class="sxs-lookup"><span data-stu-id="1daed-138">Int32</span></span>|<span data-ttu-id="1daed-139">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="1daed-139">Not yet documented</span></span>|
|<span data-ttu-id="1daed-140">filter</span><span class="sxs-lookup"><span data-stu-id="1daed-140">filter</span></span>|<span data-ttu-id="1daed-141">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1daed-141">String</span></span>|<span data-ttu-id="1daed-142">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="1daed-142">Not yet documented</span></span>|
|<span data-ttu-id="1daed-143">skipToken</span><span class="sxs-lookup"><span data-stu-id="1daed-143">skipToken</span></span>|<span data-ttu-id="1daed-144">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1daed-144">String</span></span>|<span data-ttu-id="1daed-145">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="1daed-145">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="1daed-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="1daed-146">Response</span></span>
<span data-ttu-id="1daed-147">Bei erfolgreicher Ausführung gibt die Funktion den Antwortcode `200 OK` und einen [Bericht](../resources/intune-shared-report.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="1daed-147">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1daed-148">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1daed-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="1daed-149">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1daed-149">Request</span></span>
<span data-ttu-id="1daed-150">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1daed-150">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports/managedDeviceEnrollmentAbandonmentSummary(skip=4,top=3,filter='parameterValue',skipToken='parameterValue')
```

### <a name="response"></a><span data-ttu-id="1daed-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="1daed-151">Response</span></span>
<span data-ttu-id="1daed-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1daed-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





