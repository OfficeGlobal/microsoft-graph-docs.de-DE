---
title: Aktualisieren von „managedDeviceMobileAppConfigurationDeviceSummary“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs managedDeviceMobileAppConfigurationDeviceSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a3ee88da271621c1233d7f494e1f9be683729675
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30256728"
---
# <a name="update-manageddevicemobileappconfigurationdevicesummary"></a><span data-ttu-id="48b97-103">Aktualisieren von „managedDeviceMobileAppConfigurationDeviceSummary“</span><span class="sxs-lookup"><span data-stu-id="48b97-103">Update managedDeviceMobileAppConfigurationDeviceSummary</span></span>

> <span data-ttu-id="48b97-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="48b97-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="48b97-105">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="48b97-105">Update the properties of a [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="48b97-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="48b97-106">Prerequisites</span></span>
<span data-ttu-id="48b97-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="48b97-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="48b97-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="48b97-109">Permission type</span></span>|<span data-ttu-id="48b97-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="48b97-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="48b97-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="48b97-111">Delegated (work or school account)</span></span>|<span data-ttu-id="48b97-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48b97-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="48b97-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="48b97-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="48b97-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="48b97-114">Not supported.</span></span>|
|<span data-ttu-id="48b97-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="48b97-115">Application</span></span>|<span data-ttu-id="48b97-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="48b97-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="48b97-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="48b97-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatusSummary
```

## <a name="request-headers"></a><span data-ttu-id="48b97-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="48b97-118">Request headers</span></span>
|<span data-ttu-id="48b97-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="48b97-119">Header</span></span>|<span data-ttu-id="48b97-120">Wert</span><span class="sxs-lookup"><span data-stu-id="48b97-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="48b97-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="48b97-121">Authorization</span></span>|<span data-ttu-id="48b97-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="48b97-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="48b97-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="48b97-123">Accept</span></span>|<span data-ttu-id="48b97-124">application/json</span><span class="sxs-lookup"><span data-stu-id="48b97-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="48b97-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="48b97-125">Request body</span></span>
<span data-ttu-id="48b97-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) an.</span><span class="sxs-lookup"><span data-stu-id="48b97-126">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object.</span></span>

<span data-ttu-id="48b97-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="48b97-127">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md).</span></span>

|<span data-ttu-id="48b97-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="48b97-128">Property</span></span>|<span data-ttu-id="48b97-129">Typ</span><span class="sxs-lookup"><span data-stu-id="48b97-129">Type</span></span>|<span data-ttu-id="48b97-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="48b97-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="48b97-131">id</span><span class="sxs-lookup"><span data-stu-id="48b97-131">id</span></span>|<span data-ttu-id="48b97-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="48b97-132">String</span></span>|<span data-ttu-id="48b97-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="48b97-133">Key of the entity.</span></span>|
|<span data-ttu-id="48b97-134">pendingCount</span><span class="sxs-lookup"><span data-stu-id="48b97-134">pendingCount</span></span>|<span data-ttu-id="48b97-135">Int32</span><span class="sxs-lookup"><span data-stu-id="48b97-135">Int32</span></span>|<span data-ttu-id="48b97-136">Anzahl der ausstehenden Geräte</span><span class="sxs-lookup"><span data-stu-id="48b97-136">Number of pending devices</span></span>|
|<span data-ttu-id="48b97-137">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="48b97-137">notApplicableCount</span></span>|<span data-ttu-id="48b97-138">Int32</span><span class="sxs-lookup"><span data-stu-id="48b97-138">Int32</span></span>|<span data-ttu-id="48b97-139">Anzahl der ausgenommenen Geräte</span><span class="sxs-lookup"><span data-stu-id="48b97-139">Number of not applicable devices</span></span>|
|<span data-ttu-id="48b97-140">successCount</span><span class="sxs-lookup"><span data-stu-id="48b97-140">successCount</span></span>|<span data-ttu-id="48b97-141">Int32</span><span class="sxs-lookup"><span data-stu-id="48b97-141">Int32</span></span>|<span data-ttu-id="48b97-142">Anzahl der erfolgreichen Geräte</span><span class="sxs-lookup"><span data-stu-id="48b97-142">Number of succeeded devices</span></span>|
|<span data-ttu-id="48b97-143">errorCount</span><span class="sxs-lookup"><span data-stu-id="48b97-143">errorCount</span></span>|<span data-ttu-id="48b97-144">Int32</span><span class="sxs-lookup"><span data-stu-id="48b97-144">Int32</span></span>|<span data-ttu-id="48b97-145">Anzahl der fehlerhaften Geräte</span><span class="sxs-lookup"><span data-stu-id="48b97-145">Number of error devices</span></span>|
|<span data-ttu-id="48b97-146">failedCount</span><span class="sxs-lookup"><span data-stu-id="48b97-146">failedCount</span></span>|<span data-ttu-id="48b97-147">Int32</span><span class="sxs-lookup"><span data-stu-id="48b97-147">Int32</span></span>|<span data-ttu-id="48b97-148">Anzahl der fehlgeschlagenen Geräte</span><span class="sxs-lookup"><span data-stu-id="48b97-148">Number of failed devices</span></span>|
|<span data-ttu-id="48b97-149">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="48b97-149">lastUpdateDateTime</span></span>|<span data-ttu-id="48b97-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="48b97-150">DateTimeOffset</span></span>|<span data-ttu-id="48b97-151">Datum und Uhrzeit der letzten Aktualisierung</span><span class="sxs-lookup"><span data-stu-id="48b97-151">Last update time</span></span>|
|<span data-ttu-id="48b97-152">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="48b97-152">configurationVersion</span></span>|<span data-ttu-id="48b97-153">Int32</span><span class="sxs-lookup"><span data-stu-id="48b97-153">Int32</span></span>|<span data-ttu-id="48b97-154">Version der Richtlinie für diese Übersicht</span><span class="sxs-lookup"><span data-stu-id="48b97-154">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="48b97-155">Antwort</span><span class="sxs-lookup"><span data-stu-id="48b97-155">Response</span></span>
<span data-ttu-id="48b97-156">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="48b97-156">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="48b97-157">Beispiel</span><span class="sxs-lookup"><span data-stu-id="48b97-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="48b97-158">Anforderung</span><span class="sxs-lookup"><span data-stu-id="48b97-158">Request</span></span>
<span data-ttu-id="48b97-159">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="48b97-159">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatusSummary
Content-type: application/json
Content-length: 299

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceSummary",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```

### <a name="response"></a><span data-ttu-id="48b97-160">Antwort</span><span class="sxs-lookup"><span data-stu-id="48b97-160">Response</span></span>
<span data-ttu-id="48b97-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="48b97-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 348

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceSummary",
  "id": "9997c455-c455-9997-55c4-979955c49799",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```



