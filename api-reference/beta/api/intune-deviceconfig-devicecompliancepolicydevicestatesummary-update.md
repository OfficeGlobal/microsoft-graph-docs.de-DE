---
title: Aktualisieren von „deviceCompliancePolicyDeviceStateSummary“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs deviceCompliancePolicyDeviceStateSummary.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 4874905a7ab1501cad6c72871111792cabf55c22
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399150"
---
# <a name="update-devicecompliancepolicydevicestatesummary"></a><span data-ttu-id="8fb24-103">Aktualisieren von „deviceCompliancePolicyDeviceStateSummary“</span><span class="sxs-lookup"><span data-stu-id="8fb24-103">Update deviceCompliancePolicyDeviceStateSummary</span></span>

> <span data-ttu-id="8fb24-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="8fb24-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="8fb24-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8fb24-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8fb24-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8fb24-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8fb24-107">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="8fb24-107">Update the properties of a [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8fb24-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="8fb24-108">Prerequisites</span></span>
<span data-ttu-id="8fb24-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="8fb24-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="8fb24-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8fb24-111">Permission type</span></span>|<span data-ttu-id="8fb24-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8fb24-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8fb24-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8fb24-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8fb24-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8fb24-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8fb24-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8fb24-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8fb24-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8fb24-116">Not supported.</span></span>|
|<span data-ttu-id="8fb24-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8fb24-117">Application</span></span>|<span data-ttu-id="8fb24-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8fb24-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8fb24-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8fb24-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicyDeviceStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="8fb24-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8fb24-120">Request headers</span></span>
|<span data-ttu-id="8fb24-121">Header</span><span class="sxs-lookup"><span data-stu-id="8fb24-121">Header</span></span>|<span data-ttu-id="8fb24-122">Wert</span><span class="sxs-lookup"><span data-stu-id="8fb24-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8fb24-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="8fb24-123">Authorization</span></span>|<span data-ttu-id="8fb24-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="8fb24-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8fb24-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="8fb24-125">Accept</span></span>|<span data-ttu-id="8fb24-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8fb24-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8fb24-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8fb24-127">Request body</span></span>
<span data-ttu-id="8fb24-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) an.</span><span class="sxs-lookup"><span data-stu-id="8fb24-128">In the request body, supply a JSON representation for the [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>

<span data-ttu-id="8fb24-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="8fb24-129">The following table shows the properties that are required when you create the [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md).</span></span>

|<span data-ttu-id="8fb24-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8fb24-130">Property</span></span>|<span data-ttu-id="8fb24-131">Typ</span><span class="sxs-lookup"><span data-stu-id="8fb24-131">Type</span></span>|<span data-ttu-id="8fb24-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8fb24-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8fb24-133">inGracePeriodCount</span><span class="sxs-lookup"><span data-stu-id="8fb24-133">inGracePeriodCount</span></span>|<span data-ttu-id="8fb24-134">Int32</span><span class="sxs-lookup"><span data-stu-id="8fb24-134">Int32</span></span>|<span data-ttu-id="8fb24-135">Anzahl von Geräten, die sich in der Toleranzperiode befinden</span><span class="sxs-lookup"><span data-stu-id="8fb24-135">Number of devices that are in grace period</span></span>|
|<span data-ttu-id="8fb24-136">configManagerCount</span><span class="sxs-lookup"><span data-stu-id="8fb24-136">configManagerCount</span></span>|<span data-ttu-id="8fb24-137">Int32</span><span class="sxs-lookup"><span data-stu-id="8fb24-137">Int32</span></span>|<span data-ttu-id="8fb24-138">Anzahl von Geräten, deren Konformität mit System Center Configuration Manager verwaltet wird</span><span class="sxs-lookup"><span data-stu-id="8fb24-138">Number of devices that have compliance managed by System Center Configuration Manager</span></span>|
|<span data-ttu-id="8fb24-139">id</span><span class="sxs-lookup"><span data-stu-id="8fb24-139">id</span></span>|<span data-ttu-id="8fb24-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8fb24-140">String</span></span>|<span data-ttu-id="8fb24-141">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="8fb24-141">Key of the entity.</span></span>|
|<span data-ttu-id="8fb24-142">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8fb24-142">unknownDeviceCount</span></span>|<span data-ttu-id="8fb24-143">Int32</span><span class="sxs-lookup"><span data-stu-id="8fb24-143">Int32</span></span>|<span data-ttu-id="8fb24-144">Anzahl von unbekannten Geräten</span><span class="sxs-lookup"><span data-stu-id="8fb24-144">Number of unknown devices</span></span>|
|<span data-ttu-id="8fb24-145">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8fb24-145">notApplicableDeviceCount</span></span>|<span data-ttu-id="8fb24-146">Int32</span><span class="sxs-lookup"><span data-stu-id="8fb24-146">Int32</span></span>|<span data-ttu-id="8fb24-147">Anzahl der ausgenommenen Geräte</span><span class="sxs-lookup"><span data-stu-id="8fb24-147">Number of not applicable devices</span></span>|
|<span data-ttu-id="8fb24-148">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8fb24-148">compliantDeviceCount</span></span>|<span data-ttu-id="8fb24-149">Int32</span><span class="sxs-lookup"><span data-stu-id="8fb24-149">Int32</span></span>|<span data-ttu-id="8fb24-150">Anzahl von konformen Geräten</span><span class="sxs-lookup"><span data-stu-id="8fb24-150">Number of compliant devices</span></span>|
|<span data-ttu-id="8fb24-151">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8fb24-151">remediatedDeviceCount</span></span>|<span data-ttu-id="8fb24-152">Int32</span><span class="sxs-lookup"><span data-stu-id="8fb24-152">Int32</span></span>|<span data-ttu-id="8fb24-153">Anzahl von korrigierten Geräten</span><span class="sxs-lookup"><span data-stu-id="8fb24-153">Number of remediated devices</span></span>|
|<span data-ttu-id="8fb24-154">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8fb24-154">nonCompliantDeviceCount</span></span>|<span data-ttu-id="8fb24-155">Int32</span><span class="sxs-lookup"><span data-stu-id="8fb24-155">Int32</span></span>|<span data-ttu-id="8fb24-156">Anzahl von nicht konformen Geräten</span><span class="sxs-lookup"><span data-stu-id="8fb24-156">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="8fb24-157">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8fb24-157">errorDeviceCount</span></span>|<span data-ttu-id="8fb24-158">Int32</span><span class="sxs-lookup"><span data-stu-id="8fb24-158">Int32</span></span>|<span data-ttu-id="8fb24-159">Anzahl von Geräten mit Fehlern</span><span class="sxs-lookup"><span data-stu-id="8fb24-159">Number of error devices</span></span>|
|<span data-ttu-id="8fb24-160">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8fb24-160">conflictDeviceCount</span></span>|<span data-ttu-id="8fb24-161">Int32</span><span class="sxs-lookup"><span data-stu-id="8fb24-161">Int32</span></span>|<span data-ttu-id="8fb24-162">Anzahl von Geräten mit Konflikt</span><span class="sxs-lookup"><span data-stu-id="8fb24-162">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="8fb24-163">Antwort</span><span class="sxs-lookup"><span data-stu-id="8fb24-163">Response</span></span>
<span data-ttu-id="8fb24-164">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="8fb24-164">If successful, this method returns a `200 OK` response code and an updated [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8fb24-165">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8fb24-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="8fb24-166">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8fb24-166">Request</span></span>
<span data-ttu-id="8fb24-167">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8fb24-167">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicyDeviceStateSummary
Content-type: application/json
Content-length: 349

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyDeviceStateSummary",
  "inGracePeriodCount": 2,
  "configManagerCount": 2,
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```

### <a name="response"></a><span data-ttu-id="8fb24-168">Antwort</span><span class="sxs-lookup"><span data-stu-id="8fb24-168">Response</span></span>
<span data-ttu-id="8fb24-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8fb24-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 398

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyDeviceStateSummary",
  "inGracePeriodCount": 2,
  "configManagerCount": 2,
  "id": "8c4de8a7-e8a7-8c4d-a7e8-4d8ca7e84d8c",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```




