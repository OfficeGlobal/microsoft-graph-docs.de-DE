---
title: Aktualisieren von „deviceConfigurationDeviceOverview“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs deviceConfigurationDeviceOverview.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5a3a8c916581e24397bb2f86d164f2a49dea3fa7
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30968311"
---
# <a name="update-deviceconfigurationdeviceoverview"></a><span data-ttu-id="eb4f4-103">Aktualisieren von „deviceConfigurationDeviceOverview“</span><span class="sxs-lookup"><span data-stu-id="eb4f4-103">Update deviceConfigurationDeviceOverview</span></span>

> <span data-ttu-id="eb4f4-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="eb4f4-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eb4f4-105">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="eb4f4-105">Update the properties of a [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="eb4f4-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="eb4f4-106">Prerequisites</span></span>
<span data-ttu-id="eb4f4-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eb4f4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eb4f4-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="eb4f4-109">Permission type</span></span>|<span data-ttu-id="eb4f4-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="eb4f4-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eb4f4-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="eb4f4-111">Delegated (work or school account)</span></span>|<span data-ttu-id="eb4f4-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eb4f4-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="eb4f4-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="eb4f4-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eb4f4-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="eb4f4-114">Not supported.</span></span>|
|<span data-ttu-id="eb4f4-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="eb4f4-115">Application</span></span>|<span data-ttu-id="eb4f4-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="eb4f4-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="eb4f4-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="eb4f4-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatusOverview
```

## <a name="request-headers"></a><span data-ttu-id="eb4f4-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="eb4f4-118">Request headers</span></span>
|<span data-ttu-id="eb4f4-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="eb4f4-119">Header</span></span>|<span data-ttu-id="eb4f4-120">Wert</span><span class="sxs-lookup"><span data-stu-id="eb4f4-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eb4f4-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="eb4f4-121">Authorization</span></span>|<span data-ttu-id="eb4f4-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="eb4f4-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eb4f4-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="eb4f4-123">Accept</span></span>|<span data-ttu-id="eb4f4-124">application/json</span><span class="sxs-lookup"><span data-stu-id="eb4f4-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eb4f4-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="eb4f4-125">Request body</span></span>
<span data-ttu-id="eb4f4-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) an.</span><span class="sxs-lookup"><span data-stu-id="eb4f4-126">In the request body, supply a JSON representation for the [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object.</span></span>

<span data-ttu-id="eb4f4-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="eb4f4-127">The following table shows the properties that are required when you create the [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md).</span></span>

|<span data-ttu-id="eb4f4-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="eb4f4-128">Property</span></span>|<span data-ttu-id="eb4f4-129">Typ</span><span class="sxs-lookup"><span data-stu-id="eb4f4-129">Type</span></span>|<span data-ttu-id="eb4f4-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="eb4f4-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eb4f4-131">id</span><span class="sxs-lookup"><span data-stu-id="eb4f4-131">id</span></span>|<span data-ttu-id="eb4f4-132">String</span><span class="sxs-lookup"><span data-stu-id="eb4f4-132">String</span></span>|<span data-ttu-id="eb4f4-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="eb4f4-133">Key of the entity.</span></span>|
|<span data-ttu-id="eb4f4-134">pendingCount</span><span class="sxs-lookup"><span data-stu-id="eb4f4-134">pendingCount</span></span>|<span data-ttu-id="eb4f4-135">Int32</span><span class="sxs-lookup"><span data-stu-id="eb4f4-135">Int32</span></span>|<span data-ttu-id="eb4f4-136">Anzahl der ausstehenden Geräte</span><span class="sxs-lookup"><span data-stu-id="eb4f4-136">Number of pending devices</span></span>|
|<span data-ttu-id="eb4f4-137">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="eb4f4-137">notApplicableCount</span></span>|<span data-ttu-id="eb4f4-138">Int32</span><span class="sxs-lookup"><span data-stu-id="eb4f4-138">Int32</span></span>|<span data-ttu-id="eb4f4-139">Anzahl der ausgenommenen Geräte</span><span class="sxs-lookup"><span data-stu-id="eb4f4-139">Number of not applicable devices</span></span>|
|<span data-ttu-id="eb4f4-140">successCount</span><span class="sxs-lookup"><span data-stu-id="eb4f4-140">successCount</span></span>|<span data-ttu-id="eb4f4-141">Int32</span><span class="sxs-lookup"><span data-stu-id="eb4f4-141">Int32</span></span>|<span data-ttu-id="eb4f4-142">Anzahl der erfolgreichen Geräte</span><span class="sxs-lookup"><span data-stu-id="eb4f4-142">Number of succeeded devices</span></span>|
|<span data-ttu-id="eb4f4-143">errorCount</span><span class="sxs-lookup"><span data-stu-id="eb4f4-143">errorCount</span></span>|<span data-ttu-id="eb4f4-144">Int32</span><span class="sxs-lookup"><span data-stu-id="eb4f4-144">Int32</span></span>|<span data-ttu-id="eb4f4-145">Anzahl der fehlerhaften Geräte</span><span class="sxs-lookup"><span data-stu-id="eb4f4-145">Number of error devices</span></span>|
|<span data-ttu-id="eb4f4-146">failedCount</span><span class="sxs-lookup"><span data-stu-id="eb4f4-146">failedCount</span></span>|<span data-ttu-id="eb4f4-147">Int32</span><span class="sxs-lookup"><span data-stu-id="eb4f4-147">Int32</span></span>|<span data-ttu-id="eb4f4-148">Anzahl der fehlgeschlagenen Geräte</span><span class="sxs-lookup"><span data-stu-id="eb4f4-148">Number of failed devices</span></span>|
|<span data-ttu-id="eb4f4-149">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="eb4f4-149">lastUpdateDateTime</span></span>|<span data-ttu-id="eb4f4-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eb4f4-150">DateTimeOffset</span></span>|<span data-ttu-id="eb4f4-151">Datum und Uhrzeit der letzten Aktualisierung</span><span class="sxs-lookup"><span data-stu-id="eb4f4-151">Last update time</span></span>|
|<span data-ttu-id="eb4f4-152">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="eb4f4-152">configurationVersion</span></span>|<span data-ttu-id="eb4f4-153">Int32</span><span class="sxs-lookup"><span data-stu-id="eb4f4-153">Int32</span></span>|<span data-ttu-id="eb4f4-154">Version der Richtlinie für diese Übersicht</span><span class="sxs-lookup"><span data-stu-id="eb4f4-154">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="eb4f4-155">Antwort</span><span class="sxs-lookup"><span data-stu-id="eb4f4-155">Response</span></span>
<span data-ttu-id="eb4f4-156">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="eb4f4-156">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eb4f4-157">Beispiel</span><span class="sxs-lookup"><span data-stu-id="eb4f4-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="eb4f4-158">Anforderung</span><span class="sxs-lookup"><span data-stu-id="eb4f4-158">Request</span></span>
<span data-ttu-id="eb4f4-159">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="eb4f4-159">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatusOverview
Content-type: application/json
Content-length: 284

{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceOverview",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```

### <a name="response"></a><span data-ttu-id="eb4f4-160">Antwort</span><span class="sxs-lookup"><span data-stu-id="eb4f4-160">Response</span></span>
<span data-ttu-id="eb4f4-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="eb4f4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 333

{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceOverview",
  "id": "62d48e3a-8e3a-62d4-3a8e-d4623a8ed462",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```



