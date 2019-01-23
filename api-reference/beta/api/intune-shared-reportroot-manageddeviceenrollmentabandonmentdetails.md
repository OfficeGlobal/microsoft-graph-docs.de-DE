---
title: ManagedDeviceEnrollmentAbandonmentDetails-Funktion
description: Metadaten für die Registrierung Aufgabe Detailbericht
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 30312706926293e24226801a7e0193b28d3d6f9c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29393214"
---
# <a name="manageddeviceenrollmentabandonmentdetails-function"></a><span data-ttu-id="8afd9-103">ManagedDeviceEnrollmentAbandonmentDetails-Funktion</span><span class="sxs-lookup"><span data-stu-id="8afd9-103">managedDeviceEnrollmentAbandonmentDetails function</span></span>

> <span data-ttu-id="8afd9-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="8afd9-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="8afd9-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8afd9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8afd9-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8afd9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8afd9-107">Metadaten für die Registrierung Aufgabe Detailbericht</span><span class="sxs-lookup"><span data-stu-id="8afd9-107">Metadata for Enrollment abandonment details report</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8afd9-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="8afd9-108">Prerequisites</span></span>
<span data-ttu-id="8afd9-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8afd9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8afd9-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8afd9-111">Permission type</span></span>|<span data-ttu-id="8afd9-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8afd9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8afd9-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8afd9-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="8afd9-114">&nbsp;&nbsp; **Behandelt Probleme mit**</span><span class="sxs-lookup"><span data-stu-id="8afd9-114">&nbsp; &nbsp; **Troublshooting**</span></span> | <span data-ttu-id="8afd9-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="8afd9-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="8afd9-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8afd9-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8afd9-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8afd9-117">Not supported.</span></span>|
|<span data-ttu-id="8afd9-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8afd9-118">Application</span></span>|<span data-ttu-id="8afd9-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8afd9-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8afd9-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8afd9-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentAbandonmentDetails
```

## <a name="request-headers"></a><span data-ttu-id="8afd9-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8afd9-121">Request headers</span></span>
|<span data-ttu-id="8afd9-122">Header</span><span class="sxs-lookup"><span data-stu-id="8afd9-122">Header</span></span>|<span data-ttu-id="8afd9-123">Wert</span><span class="sxs-lookup"><span data-stu-id="8afd9-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8afd9-124">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="8afd9-124">Authorization</span></span>|<span data-ttu-id="8afd9-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="8afd9-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8afd9-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="8afd9-126">Accept</span></span>|<span data-ttu-id="8afd9-127">application/json</span><span class="sxs-lookup"><span data-stu-id="8afd9-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8afd9-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8afd9-128">Request body</span></span>
<span data-ttu-id="8afd9-129">Geben Sie in der Anforderungs-URL die folgenden Abfrageparameter mit Werten an.</span><span class="sxs-lookup"><span data-stu-id="8afd9-129">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="8afd9-130">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Funktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="8afd9-130">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="8afd9-131">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8afd9-131">Property</span></span>|<span data-ttu-id="8afd9-132">Typ</span><span class="sxs-lookup"><span data-stu-id="8afd9-132">Type</span></span>|<span data-ttu-id="8afd9-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8afd9-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8afd9-134">skip</span><span class="sxs-lookup"><span data-stu-id="8afd9-134">skip</span></span>|<span data-ttu-id="8afd9-135">Int32</span><span class="sxs-lookup"><span data-stu-id="8afd9-135">Int32</span></span>|<span data-ttu-id="8afd9-136">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="8afd9-136">Not yet documented</span></span>|
|<span data-ttu-id="8afd9-137">top</span><span class="sxs-lookup"><span data-stu-id="8afd9-137">top</span></span>|<span data-ttu-id="8afd9-138">Int32</span><span class="sxs-lookup"><span data-stu-id="8afd9-138">Int32</span></span>|<span data-ttu-id="8afd9-139">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="8afd9-139">Not yet documented</span></span>|
|<span data-ttu-id="8afd9-140">filter</span><span class="sxs-lookup"><span data-stu-id="8afd9-140">filter</span></span>|<span data-ttu-id="8afd9-141">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8afd9-141">String</span></span>|<span data-ttu-id="8afd9-142">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="8afd9-142">Not yet documented</span></span>|
|<span data-ttu-id="8afd9-143">skipToken</span><span class="sxs-lookup"><span data-stu-id="8afd9-143">skipToken</span></span>|<span data-ttu-id="8afd9-144">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8afd9-144">String</span></span>|<span data-ttu-id="8afd9-145">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="8afd9-145">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="8afd9-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="8afd9-146">Response</span></span>
<span data-ttu-id="8afd9-147">Bei erfolgreicher Ausführung gibt die Funktion den Antwortcode `200 OK` und einen [Bericht](../resources/intune-shared-report.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="8afd9-147">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8afd9-148">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8afd9-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="8afd9-149">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8afd9-149">Request</span></span>
<span data-ttu-id="8afd9-150">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8afd9-150">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports/managedDeviceEnrollmentAbandonmentDetails(skip=4,top=3,filter='parameterValue',skipToken='parameterValue')
```

### <a name="response"></a><span data-ttu-id="8afd9-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="8afd9-151">Response</span></span>
<span data-ttu-id="8afd9-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8afd9-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





