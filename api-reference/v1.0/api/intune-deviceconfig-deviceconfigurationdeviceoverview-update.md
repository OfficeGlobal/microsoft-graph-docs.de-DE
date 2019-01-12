---
title: Aktualisieren von „deviceConfigurationDeviceOverview“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs deviceConfigurationDeviceOverview.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f6aadd22c5762b2b8159a858014d6f374deabaf0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27914206"
---
# <a name="update-deviceconfigurationdeviceoverview"></a><span data-ttu-id="222d0-103">Aktualisieren von „deviceConfigurationDeviceOverview“</span><span class="sxs-lookup"><span data-stu-id="222d0-103">Update deviceConfigurationDeviceOverview</span></span>

> <span data-ttu-id="222d0-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="222d0-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="222d0-105">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="222d0-105">Update the properties of a [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="222d0-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="222d0-106">Prerequisites</span></span>
<span data-ttu-id="222d0-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="222d0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="222d0-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="222d0-109">Permission type</span></span>|<span data-ttu-id="222d0-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="222d0-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="222d0-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="222d0-111">Delegated (work or school account)</span></span>|<span data-ttu-id="222d0-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="222d0-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="222d0-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="222d0-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="222d0-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="222d0-114">Not supported.</span></span>|
|<span data-ttu-id="222d0-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="222d0-115">Application</span></span>|<span data-ttu-id="222d0-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="222d0-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="222d0-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="222d0-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatusOverview
```

## <a name="request-headers"></a><span data-ttu-id="222d0-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="222d0-118">Request headers</span></span>
|<span data-ttu-id="222d0-119">Header</span><span class="sxs-lookup"><span data-stu-id="222d0-119">Header</span></span>|<span data-ttu-id="222d0-120">Wert</span><span class="sxs-lookup"><span data-stu-id="222d0-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="222d0-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="222d0-121">Authorization</span></span>|<span data-ttu-id="222d0-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="222d0-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="222d0-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="222d0-123">Accept</span></span>|<span data-ttu-id="222d0-124">application/json</span><span class="sxs-lookup"><span data-stu-id="222d0-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="222d0-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="222d0-125">Request body</span></span>
<span data-ttu-id="222d0-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) an.</span><span class="sxs-lookup"><span data-stu-id="222d0-126">In the request body, supply a JSON representation for the [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object.</span></span>

<span data-ttu-id="222d0-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="222d0-127">The following table shows the properties that are required when you create the [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md).</span></span>

|<span data-ttu-id="222d0-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="222d0-128">Property</span></span>|<span data-ttu-id="222d0-129">Typ</span><span class="sxs-lookup"><span data-stu-id="222d0-129">Type</span></span>|<span data-ttu-id="222d0-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="222d0-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="222d0-131">id</span><span class="sxs-lookup"><span data-stu-id="222d0-131">id</span></span>|<span data-ttu-id="222d0-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="222d0-132">String</span></span>|<span data-ttu-id="222d0-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="222d0-133">Key of the entity.</span></span>|
|<span data-ttu-id="222d0-134">pendingCount</span><span class="sxs-lookup"><span data-stu-id="222d0-134">pendingCount</span></span>|<span data-ttu-id="222d0-135">Int32</span><span class="sxs-lookup"><span data-stu-id="222d0-135">Int32</span></span>|<span data-ttu-id="222d0-136">Anzahl der ausstehenden Geräte</span><span class="sxs-lookup"><span data-stu-id="222d0-136">Number of pending devices</span></span>|
|<span data-ttu-id="222d0-137">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="222d0-137">notApplicableCount</span></span>|<span data-ttu-id="222d0-138">Int32</span><span class="sxs-lookup"><span data-stu-id="222d0-138">Int32</span></span>|<span data-ttu-id="222d0-139">Anzahl der ausgenommenen Geräte</span><span class="sxs-lookup"><span data-stu-id="222d0-139">Number of not applicable devices</span></span>|
|<span data-ttu-id="222d0-140">successCount</span><span class="sxs-lookup"><span data-stu-id="222d0-140">successCount</span></span>|<span data-ttu-id="222d0-141">Int32</span><span class="sxs-lookup"><span data-stu-id="222d0-141">Int32</span></span>|<span data-ttu-id="222d0-142">Anzahl der erfolgreichen Geräte</span><span class="sxs-lookup"><span data-stu-id="222d0-142">Number of succeeded devices</span></span>|
|<span data-ttu-id="222d0-143">errorCount</span><span class="sxs-lookup"><span data-stu-id="222d0-143">errorCount</span></span>|<span data-ttu-id="222d0-144">Int32</span><span class="sxs-lookup"><span data-stu-id="222d0-144">Int32</span></span>|<span data-ttu-id="222d0-145">Anzahl der fehlerhaften Geräte</span><span class="sxs-lookup"><span data-stu-id="222d0-145">Number of error devices</span></span>|
|<span data-ttu-id="222d0-146">failedCount</span><span class="sxs-lookup"><span data-stu-id="222d0-146">failedCount</span></span>|<span data-ttu-id="222d0-147">Int32</span><span class="sxs-lookup"><span data-stu-id="222d0-147">Int32</span></span>|<span data-ttu-id="222d0-148">Anzahl der fehlgeschlagenen Geräte</span><span class="sxs-lookup"><span data-stu-id="222d0-148">Number of failed devices</span></span>|
|<span data-ttu-id="222d0-149">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="222d0-149">lastUpdateDateTime</span></span>|<span data-ttu-id="222d0-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="222d0-150">DateTimeOffset</span></span>|<span data-ttu-id="222d0-151">Datum und Uhrzeit der letzten Aktualisierung</span><span class="sxs-lookup"><span data-stu-id="222d0-151">Last update time</span></span>|
|<span data-ttu-id="222d0-152">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="222d0-152">configurationVersion</span></span>|<span data-ttu-id="222d0-153">Int32</span><span class="sxs-lookup"><span data-stu-id="222d0-153">Int32</span></span>|<span data-ttu-id="222d0-154">Version der Richtlinie für diese Übersicht</span><span class="sxs-lookup"><span data-stu-id="222d0-154">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="222d0-155">Antwort</span><span class="sxs-lookup"><span data-stu-id="222d0-155">Response</span></span>
<span data-ttu-id="222d0-156">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="222d0-156">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="222d0-157">Beispiel</span><span class="sxs-lookup"><span data-stu-id="222d0-157">Example</span></span>
### <a name="request"></a><span data-ttu-id="222d0-158">Anforderung</span><span class="sxs-lookup"><span data-stu-id="222d0-158">Request</span></span>
<span data-ttu-id="222d0-159">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="222d0-159">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="222d0-160">Antwort</span><span class="sxs-lookup"><span data-stu-id="222d0-160">Response</span></span>
<span data-ttu-id="222d0-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="222d0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



