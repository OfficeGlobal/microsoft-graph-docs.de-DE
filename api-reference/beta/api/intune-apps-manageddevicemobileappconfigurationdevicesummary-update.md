---
title: Aktualisieren von „managedDeviceMobileAppConfigurationDeviceSummary“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs managedDeviceMobileAppConfigurationDeviceSummary.
ms.openlocfilehash: bc5c7642daa408186e05dd06c7630a8c8431df1f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059894"
---
# <a name="update-manageddevicemobileappconfigurationdevicesummary"></a><span data-ttu-id="130f0-103">Aktualisieren von „managedDeviceMobileAppConfigurationDeviceSummary“</span><span class="sxs-lookup"><span data-stu-id="130f0-103">Update managedDeviceMobileAppConfigurationDeviceSummary</span></span>

> <span data-ttu-id="130f0-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="130f0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="130f0-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="130f0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="130f0-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="130f0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="130f0-107">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="130f0-107">Update the properties of a [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="130f0-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="130f0-108">Prerequisites</span></span>
<span data-ttu-id="130f0-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="130f0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="130f0-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="130f0-111">Permission type</span></span>|<span data-ttu-id="130f0-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="130f0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="130f0-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="130f0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="130f0-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="130f0-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="130f0-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="130f0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="130f0-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="130f0-116">Not supported.</span></span>|
|<span data-ttu-id="130f0-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="130f0-117">Application</span></span>|<span data-ttu-id="130f0-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="130f0-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="130f0-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="130f0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatusSummary
```

## <a name="request-headers"></a><span data-ttu-id="130f0-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="130f0-120">Request headers</span></span>
|<span data-ttu-id="130f0-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="130f0-121">Header</span></span>|<span data-ttu-id="130f0-122">Wert</span><span class="sxs-lookup"><span data-stu-id="130f0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="130f0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="130f0-123">Authorization</span></span>|<span data-ttu-id="130f0-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="130f0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="130f0-125">Accept</span><span class="sxs-lookup"><span data-stu-id="130f0-125">Accept</span></span>|<span data-ttu-id="130f0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="130f0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="130f0-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="130f0-127">Request body</span></span>
<span data-ttu-id="130f0-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) an.</span><span class="sxs-lookup"><span data-stu-id="130f0-128">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object.</span></span>

<span data-ttu-id="130f0-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="130f0-129">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md).</span></span>

|<span data-ttu-id="130f0-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="130f0-130">Property</span></span>|<span data-ttu-id="130f0-131">Typ</span><span class="sxs-lookup"><span data-stu-id="130f0-131">Type</span></span>|<span data-ttu-id="130f0-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="130f0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="130f0-133">id</span><span class="sxs-lookup"><span data-stu-id="130f0-133">id</span></span>|<span data-ttu-id="130f0-134">String</span><span class="sxs-lookup"><span data-stu-id="130f0-134">String</span></span>|<span data-ttu-id="130f0-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="130f0-135">Key of the entity.</span></span>|
|<span data-ttu-id="130f0-136">pendingCount</span><span class="sxs-lookup"><span data-stu-id="130f0-136">pendingCount</span></span>|<span data-ttu-id="130f0-137">Int32</span><span class="sxs-lookup"><span data-stu-id="130f0-137">Int32</span></span>|<span data-ttu-id="130f0-138">Anzahl der ausstehenden Geräte</span><span class="sxs-lookup"><span data-stu-id="130f0-138">Number of pending devices</span></span>|
|<span data-ttu-id="130f0-139">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="130f0-139">notApplicableCount</span></span>|<span data-ttu-id="130f0-140">Int32</span><span class="sxs-lookup"><span data-stu-id="130f0-140">Int32</span></span>|<span data-ttu-id="130f0-141">Anzahl der ausgenommenen Geräte</span><span class="sxs-lookup"><span data-stu-id="130f0-141">Number of not applicable devices</span></span>|
|<span data-ttu-id="130f0-142">notApplicablePlatformCount</span><span class="sxs-lookup"><span data-stu-id="130f0-142">notApplicablePlatformCount</span></span>|<span data-ttu-id="130f0-143">Int32</span><span class="sxs-lookup"><span data-stu-id="130f0-143">Int32</span></span>|<span data-ttu-id="130f0-144">Anzahl der Geräte, die aufgrund von Konflikt Plattform und Richtlinie nicht zutreffend</span><span class="sxs-lookup"><span data-stu-id="130f0-144">Number of not applicable devices due to mismatch platform and policy</span></span>|
|<span data-ttu-id="130f0-145">successCount</span><span class="sxs-lookup"><span data-stu-id="130f0-145">successCount</span></span>|<span data-ttu-id="130f0-146">Int32</span><span class="sxs-lookup"><span data-stu-id="130f0-146">Int32</span></span>|<span data-ttu-id="130f0-147">Anzahl der erfolgreichen Geräte</span><span class="sxs-lookup"><span data-stu-id="130f0-147">Number of succeeded devices</span></span>|
|<span data-ttu-id="130f0-148">errorCount</span><span class="sxs-lookup"><span data-stu-id="130f0-148">errorCount</span></span>|<span data-ttu-id="130f0-149">Int32</span><span class="sxs-lookup"><span data-stu-id="130f0-149">Int32</span></span>|<span data-ttu-id="130f0-150">Anzahl der fehlerhaften Geräte</span><span class="sxs-lookup"><span data-stu-id="130f0-150">Number of error devices</span></span>|
|<span data-ttu-id="130f0-151">failedCount</span><span class="sxs-lookup"><span data-stu-id="130f0-151">failedCount</span></span>|<span data-ttu-id="130f0-152">Int32</span><span class="sxs-lookup"><span data-stu-id="130f0-152">Int32</span></span>|<span data-ttu-id="130f0-153">Anzahl der fehlgeschlagenen Geräte</span><span class="sxs-lookup"><span data-stu-id="130f0-153">Number of failed devices</span></span>|
|<span data-ttu-id="130f0-154">conflictCount</span><span class="sxs-lookup"><span data-stu-id="130f0-154">conflictCount</span></span>|<span data-ttu-id="130f0-155">Int32</span><span class="sxs-lookup"><span data-stu-id="130f0-155">Int32</span></span>|<span data-ttu-id="130f0-156">Anzahl der Geräte in Konflikt</span><span class="sxs-lookup"><span data-stu-id="130f0-156">Number of devices in conflict</span></span>|
|<span data-ttu-id="130f0-157">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="130f0-157">lastUpdateDateTime</span></span>|<span data-ttu-id="130f0-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="130f0-158">DateTimeOffset</span></span>|<span data-ttu-id="130f0-159">Datum und Uhrzeit der letzten Aktualisierung</span><span class="sxs-lookup"><span data-stu-id="130f0-159">Last update time</span></span>|
|<span data-ttu-id="130f0-160">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="130f0-160">configurationVersion</span></span>|<span data-ttu-id="130f0-161">Int32</span><span class="sxs-lookup"><span data-stu-id="130f0-161">Int32</span></span>|<span data-ttu-id="130f0-162">Version der Richtlinie für diese Übersicht</span><span class="sxs-lookup"><span data-stu-id="130f0-162">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="130f0-163">Antwort</span><span class="sxs-lookup"><span data-stu-id="130f0-163">Response</span></span>
<span data-ttu-id="130f0-164">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="130f0-164">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="130f0-165">Beispiel</span><span class="sxs-lookup"><span data-stu-id="130f0-165">Example</span></span>
### <a name="request"></a><span data-ttu-id="130f0-166">Anforderung</span><span class="sxs-lookup"><span data-stu-id="130f0-166">Request</span></span>
<span data-ttu-id="130f0-167">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="130f0-167">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatusSummary
Content-type: application/json
Content-length: 273

{
  "pendingCount": 12,
  "notApplicableCount": 2,
  "notApplicablePlatformCount": 10,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "conflictCount": 13,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```

### <a name="response"></a><span data-ttu-id="130f0-168">Antwort</span><span class="sxs-lookup"><span data-stu-id="130f0-168">Response</span></span>
<span data-ttu-id="130f0-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="130f0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 409

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceSummary",
  "id": "9997c455-c455-9997-55c4-979955c49799",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "notApplicablePlatformCount": 10,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "conflictCount": 13,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```





