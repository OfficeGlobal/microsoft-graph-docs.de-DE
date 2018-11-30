---
title: Aktualisieren von „deviceConfigurationDeviceOverview“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs deviceConfigurationDeviceOverview.
ms.openlocfilehash: 7eecc3e7871ae1ec8891c5f3f8c7dfde9d517c00
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018081"
---
# <a name="update-deviceconfigurationdeviceoverview"></a><span data-ttu-id="f3803-103">Aktualisieren von „deviceConfigurationDeviceOverview“</span><span class="sxs-lookup"><span data-stu-id="f3803-103">Update deviceConfigurationDeviceOverview</span></span>

> <span data-ttu-id="f3803-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="f3803-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f3803-105">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="f3803-105">Update the properties of a [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f3803-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f3803-106">Prerequisites</span></span>
<span data-ttu-id="f3803-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f3803-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f3803-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f3803-109">Permission type</span></span>|<span data-ttu-id="f3803-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f3803-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f3803-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f3803-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f3803-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3803-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f3803-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f3803-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f3803-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f3803-114">Not supported.</span></span>|
|<span data-ttu-id="f3803-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f3803-115">Application</span></span>|<span data-ttu-id="f3803-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f3803-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f3803-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f3803-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatusOverview
```

## <a name="request-headers"></a><span data-ttu-id="f3803-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f3803-118">Request headers</span></span>
|<span data-ttu-id="f3803-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="f3803-119">Header</span></span>|<span data-ttu-id="f3803-120">Wert</span><span class="sxs-lookup"><span data-stu-id="f3803-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f3803-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f3803-121">Authorization</span></span>|<span data-ttu-id="f3803-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="f3803-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f3803-123">Accept</span><span class="sxs-lookup"><span data-stu-id="f3803-123">Accept</span></span>|<span data-ttu-id="f3803-124">application/json</span><span class="sxs-lookup"><span data-stu-id="f3803-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f3803-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f3803-125">Request body</span></span>
<span data-ttu-id="f3803-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) an.</span><span class="sxs-lookup"><span data-stu-id="f3803-126">In the request body, supply a JSON representation for the [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object.</span></span>

<span data-ttu-id="f3803-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="f3803-127">The following table shows the properties that are required when you create the [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md).</span></span>

|<span data-ttu-id="f3803-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f3803-128">Property</span></span>|<span data-ttu-id="f3803-129">Typ</span><span class="sxs-lookup"><span data-stu-id="f3803-129">Type</span></span>|<span data-ttu-id="f3803-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f3803-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f3803-131">id</span><span class="sxs-lookup"><span data-stu-id="f3803-131">id</span></span>|<span data-ttu-id="f3803-132">String</span><span class="sxs-lookup"><span data-stu-id="f3803-132">String</span></span>|<span data-ttu-id="f3803-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="f3803-133">Key of the entity.</span></span>|
|<span data-ttu-id="f3803-134">pendingCount</span><span class="sxs-lookup"><span data-stu-id="f3803-134">pendingCount</span></span>|<span data-ttu-id="f3803-135">Int32</span><span class="sxs-lookup"><span data-stu-id="f3803-135">Int32</span></span>|<span data-ttu-id="f3803-136">Anzahl der ausstehenden Geräte</span><span class="sxs-lookup"><span data-stu-id="f3803-136">Number of pending devices</span></span>|
|<span data-ttu-id="f3803-137">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="f3803-137">notApplicableCount</span></span>|<span data-ttu-id="f3803-138">Int32</span><span class="sxs-lookup"><span data-stu-id="f3803-138">Int32</span></span>|<span data-ttu-id="f3803-139">Anzahl der ausgenommenen Geräte</span><span class="sxs-lookup"><span data-stu-id="f3803-139">Number of not applicable devices</span></span>|
|<span data-ttu-id="f3803-140">successCount</span><span class="sxs-lookup"><span data-stu-id="f3803-140">successCount</span></span>|<span data-ttu-id="f3803-141">Int32</span><span class="sxs-lookup"><span data-stu-id="f3803-141">Int32</span></span>|<span data-ttu-id="f3803-142">Anzahl der erfolgreichen Geräte</span><span class="sxs-lookup"><span data-stu-id="f3803-142">Number of succeeded devices</span></span>|
|<span data-ttu-id="f3803-143">errorCount</span><span class="sxs-lookup"><span data-stu-id="f3803-143">errorCount</span></span>|<span data-ttu-id="f3803-144">Int32</span><span class="sxs-lookup"><span data-stu-id="f3803-144">Int32</span></span>|<span data-ttu-id="f3803-145">Anzahl der fehlerhaften Geräte</span><span class="sxs-lookup"><span data-stu-id="f3803-145">Number of error devices</span></span>|
|<span data-ttu-id="f3803-146">failedCount</span><span class="sxs-lookup"><span data-stu-id="f3803-146">failedCount</span></span>|<span data-ttu-id="f3803-147">Int32</span><span class="sxs-lookup"><span data-stu-id="f3803-147">Int32</span></span>|<span data-ttu-id="f3803-148">Anzahl der fehlgeschlagenen Geräte</span><span class="sxs-lookup"><span data-stu-id="f3803-148">Number of failed devices</span></span>|
|<span data-ttu-id="f3803-149">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="f3803-149">lastUpdateDateTime</span></span>|<span data-ttu-id="f3803-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f3803-150">DateTimeOffset</span></span>|<span data-ttu-id="f3803-151">Datum und Uhrzeit der letzten Aktualisierung</span><span class="sxs-lookup"><span data-stu-id="f3803-151">Last update time</span></span>|
|<span data-ttu-id="f3803-152">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="f3803-152">configurationVersion</span></span>|<span data-ttu-id="f3803-153">Int32</span><span class="sxs-lookup"><span data-stu-id="f3803-153">Int32</span></span>|<span data-ttu-id="f3803-154">Version der Richtlinie für diese Übersicht</span><span class="sxs-lookup"><span data-stu-id="f3803-154">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="f3803-155">Antwort</span><span class="sxs-lookup"><span data-stu-id="f3803-155">Response</span></span>
<span data-ttu-id="f3803-156">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="f3803-156">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f3803-157">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f3803-157">Example</span></span>
### <a name="request"></a><span data-ttu-id="f3803-158">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f3803-158">Request</span></span>
<span data-ttu-id="f3803-159">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f3803-159">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f3803-160">Antwort</span><span class="sxs-lookup"><span data-stu-id="f3803-160">Response</span></span>
<span data-ttu-id="f3803-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f3803-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



