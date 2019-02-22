---
title: Aktualisieren von „deviceConfigurationDeviceStateSummary“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs deviceConfigurationDeviceStateSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 816612ef041bf71dbd2e9f2ebf7b3b212892322b
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30156119"
---
# <a name="update-deviceconfigurationdevicestatesummary"></a><span data-ttu-id="fa926-103">Aktualisieren von „deviceConfigurationDeviceStateSummary“</span><span class="sxs-lookup"><span data-stu-id="fa926-103">Update deviceConfigurationDeviceStateSummary</span></span>

> <span data-ttu-id="fa926-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="fa926-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fa926-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="fa926-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fa926-106">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="fa926-106">Update the properties of a [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fa926-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="fa926-107">Prerequisites</span></span>
<span data-ttu-id="fa926-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="fa926-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="fa926-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="fa926-110">Permission type</span></span>|<span data-ttu-id="fa926-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="fa926-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fa926-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="fa926-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fa926-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fa926-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="fa926-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="fa926-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fa926-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fa926-115">Not supported.</span></span>|
|<span data-ttu-id="fa926-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="fa926-116">Application</span></span>|<span data-ttu-id="fa926-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fa926-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fa926-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="fa926-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationDeviceStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="fa926-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="fa926-119">Request headers</span></span>
|<span data-ttu-id="fa926-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="fa926-120">Header</span></span>|<span data-ttu-id="fa926-121">Wert</span><span class="sxs-lookup"><span data-stu-id="fa926-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fa926-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="fa926-122">Authorization</span></span>|<span data-ttu-id="fa926-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="fa926-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fa926-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="fa926-124">Accept</span></span>|<span data-ttu-id="fa926-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fa926-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fa926-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="fa926-126">Request body</span></span>
<span data-ttu-id="fa926-127">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) an.</span><span class="sxs-lookup"><span data-stu-id="fa926-127">In the request body, supply a JSON representation for the [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object.</span></span>

<span data-ttu-id="fa926-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="fa926-128">The following table shows the properties that are required when you create the [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md).</span></span>

|<span data-ttu-id="fa926-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="fa926-129">Property</span></span>|<span data-ttu-id="fa926-130">Typ</span><span class="sxs-lookup"><span data-stu-id="fa926-130">Type</span></span>|<span data-ttu-id="fa926-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fa926-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fa926-132">id</span><span class="sxs-lookup"><span data-stu-id="fa926-132">id</span></span>|<span data-ttu-id="fa926-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fa926-133">String</span></span>|<span data-ttu-id="fa926-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="fa926-134">Key of the entity.</span></span>|
|<span data-ttu-id="fa926-135">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="fa926-135">unknownDeviceCount</span></span>|<span data-ttu-id="fa926-136">Int32</span><span class="sxs-lookup"><span data-stu-id="fa926-136">Int32</span></span>|<span data-ttu-id="fa926-137">Anzahl von unbekannten Geräten</span><span class="sxs-lookup"><span data-stu-id="fa926-137">Number of unknown devices</span></span>|
|<span data-ttu-id="fa926-138">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="fa926-138">notApplicableDeviceCount</span></span>|<span data-ttu-id="fa926-139">Int32</span><span class="sxs-lookup"><span data-stu-id="fa926-139">Int32</span></span>|<span data-ttu-id="fa926-140">Anzahl der ausgenommenen Geräte</span><span class="sxs-lookup"><span data-stu-id="fa926-140">Number of not applicable devices</span></span>|
|<span data-ttu-id="fa926-141">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="fa926-141">compliantDeviceCount</span></span>|<span data-ttu-id="fa926-142">Int32</span><span class="sxs-lookup"><span data-stu-id="fa926-142">Int32</span></span>|<span data-ttu-id="fa926-143">Anzahl von konformen Geräten</span><span class="sxs-lookup"><span data-stu-id="fa926-143">Number of compliant devices</span></span>|
|<span data-ttu-id="fa926-144">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="fa926-144">remediatedDeviceCount</span></span>|<span data-ttu-id="fa926-145">Int32</span><span class="sxs-lookup"><span data-stu-id="fa926-145">Int32</span></span>|<span data-ttu-id="fa926-146">Anzahl von korrigierten Geräten</span><span class="sxs-lookup"><span data-stu-id="fa926-146">Number of remediated devices</span></span>|
|<span data-ttu-id="fa926-147">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="fa926-147">nonCompliantDeviceCount</span></span>|<span data-ttu-id="fa926-148">Int32</span><span class="sxs-lookup"><span data-stu-id="fa926-148">Int32</span></span>|<span data-ttu-id="fa926-149">Anzahl von nicht konformen Geräten</span><span class="sxs-lookup"><span data-stu-id="fa926-149">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="fa926-150">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="fa926-150">errorDeviceCount</span></span>|<span data-ttu-id="fa926-151">Int32</span><span class="sxs-lookup"><span data-stu-id="fa926-151">Int32</span></span>|<span data-ttu-id="fa926-152">Anzahl von Geräten mit Fehlern</span><span class="sxs-lookup"><span data-stu-id="fa926-152">Number of error devices</span></span>|
|<span data-ttu-id="fa926-153">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="fa926-153">conflictDeviceCount</span></span>|<span data-ttu-id="fa926-154">Int32</span><span class="sxs-lookup"><span data-stu-id="fa926-154">Int32</span></span>|<span data-ttu-id="fa926-155">Anzahl von Geräten mit Konflikt</span><span class="sxs-lookup"><span data-stu-id="fa926-155">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="fa926-156">Antwort</span><span class="sxs-lookup"><span data-stu-id="fa926-156">Response</span></span>
<span data-ttu-id="fa926-157">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="fa926-157">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fa926-158">Beispiel</span><span class="sxs-lookup"><span data-stu-id="fa926-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="fa926-159">Anforderung</span><span class="sxs-lookup"><span data-stu-id="fa926-159">Request</span></span>
<span data-ttu-id="fa926-160">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="fa926-160">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationDeviceStateSummaries
Content-type: application/json
Content-length: 290

{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceStateSummary",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```

### <a name="response"></a><span data-ttu-id="fa926-161">Antwort</span><span class="sxs-lookup"><span data-stu-id="fa926-161">Response</span></span>
<span data-ttu-id="fa926-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fa926-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 339

{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceStateSummary",
  "id": "5db26f5a-6f5a-5db2-5a6f-b25d5a6fb25d",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```




