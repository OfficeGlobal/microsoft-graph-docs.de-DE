---
title: Aktualisieren von „managedDeviceMobileAppConfigurationUserSummary“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs managedDeviceMobileAppConfigurationUserSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fc12a1322dadc4cfafd28b64ec35002ece2ee34e
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30977898"
---
# <a name="update-manageddevicemobileappconfigurationusersummary"></a><span data-ttu-id="8c6d7-103">Aktualisieren von „managedDeviceMobileAppConfigurationUserSummary“</span><span class="sxs-lookup"><span data-stu-id="8c6d7-103">Update managedDeviceMobileAppConfigurationUserSummary</span></span>

> <span data-ttu-id="8c6d7-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="8c6d7-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8c6d7-105">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md).</span><span class="sxs-lookup"><span data-stu-id="8c6d7-105">Update the properties of a [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8c6d7-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="8c6d7-106">Prerequisites</span></span>
<span data-ttu-id="8c6d7-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8c6d7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8c6d7-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8c6d7-109">Permission type</span></span>|<span data-ttu-id="8c6d7-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8c6d7-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8c6d7-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8c6d7-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8c6d7-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c6d7-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="8c6d7-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8c6d7-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8c6d7-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8c6d7-114">Not supported.</span></span>|
|<span data-ttu-id="8c6d7-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8c6d7-115">Application</span></span>|<span data-ttu-id="8c6d7-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8c6d7-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8c6d7-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8c6d7-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatusSummary
```

## <a name="request-headers"></a><span data-ttu-id="8c6d7-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8c6d7-118">Request headers</span></span>
|<span data-ttu-id="8c6d7-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="8c6d7-119">Header</span></span>|<span data-ttu-id="8c6d7-120">Wert</span><span class="sxs-lookup"><span data-stu-id="8c6d7-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8c6d7-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="8c6d7-121">Authorization</span></span>|<span data-ttu-id="8c6d7-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="8c6d7-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8c6d7-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="8c6d7-123">Accept</span></span>|<span data-ttu-id="8c6d7-124">application/json</span><span class="sxs-lookup"><span data-stu-id="8c6d7-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8c6d7-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8c6d7-125">Request body</span></span>
<span data-ttu-id="8c6d7-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) an.</span><span class="sxs-lookup"><span data-stu-id="8c6d7-126">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object.</span></span>

<span data-ttu-id="8c6d7-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="8c6d7-127">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md).</span></span>

|<span data-ttu-id="8c6d7-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8c6d7-128">Property</span></span>|<span data-ttu-id="8c6d7-129">Typ</span><span class="sxs-lookup"><span data-stu-id="8c6d7-129">Type</span></span>|<span data-ttu-id="8c6d7-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8c6d7-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8c6d7-131">id</span><span class="sxs-lookup"><span data-stu-id="8c6d7-131">id</span></span>|<span data-ttu-id="8c6d7-132">String</span><span class="sxs-lookup"><span data-stu-id="8c6d7-132">String</span></span>|<span data-ttu-id="8c6d7-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="8c6d7-133">Key of the entity.</span></span>|
|<span data-ttu-id="8c6d7-134">pendingCount</span><span class="sxs-lookup"><span data-stu-id="8c6d7-134">pendingCount</span></span>|<span data-ttu-id="8c6d7-135">Int32</span><span class="sxs-lookup"><span data-stu-id="8c6d7-135">Int32</span></span>|<span data-ttu-id="8c6d7-136">Anzahl der ausstehenden Benutzer</span><span class="sxs-lookup"><span data-stu-id="8c6d7-136">Number of pending Users</span></span>|
|<span data-ttu-id="8c6d7-137">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="8c6d7-137">notApplicableCount</span></span>|<span data-ttu-id="8c6d7-138">Int32</span><span class="sxs-lookup"><span data-stu-id="8c6d7-138">Int32</span></span>|<span data-ttu-id="8c6d7-139">Anzahl der nicht anwendbaren Benutzer</span><span class="sxs-lookup"><span data-stu-id="8c6d7-139">Number of not applicable users</span></span>|
|<span data-ttu-id="8c6d7-140">successCount</span><span class="sxs-lookup"><span data-stu-id="8c6d7-140">successCount</span></span>|<span data-ttu-id="8c6d7-141">Int32</span><span class="sxs-lookup"><span data-stu-id="8c6d7-141">Int32</span></span>|<span data-ttu-id="8c6d7-142">Anzahl der erfolgreichen Benutzer</span><span class="sxs-lookup"><span data-stu-id="8c6d7-142">Number of succeeded Users</span></span>|
|<span data-ttu-id="8c6d7-143">errorCount</span><span class="sxs-lookup"><span data-stu-id="8c6d7-143">errorCount</span></span>|<span data-ttu-id="8c6d7-144">Int32</span><span class="sxs-lookup"><span data-stu-id="8c6d7-144">Int32</span></span>|<span data-ttu-id="8c6d7-145">Anzahl der Benutzer mit Fehlern</span><span class="sxs-lookup"><span data-stu-id="8c6d7-145">Number of error Users</span></span>|
|<span data-ttu-id="8c6d7-146">failedCount</span><span class="sxs-lookup"><span data-stu-id="8c6d7-146">failedCount</span></span>|<span data-ttu-id="8c6d7-147">Int32</span><span class="sxs-lookup"><span data-stu-id="8c6d7-147">Int32</span></span>|<span data-ttu-id="8c6d7-148">Anzahl der fehlgeschlagenen Benutzer</span><span class="sxs-lookup"><span data-stu-id="8c6d7-148">Number of failed Users</span></span>|
|<span data-ttu-id="8c6d7-149">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="8c6d7-149">lastUpdateDateTime</span></span>|<span data-ttu-id="8c6d7-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8c6d7-150">DateTimeOffset</span></span>|<span data-ttu-id="8c6d7-151">Datum und Uhrzeit der letzten Aktualisierung</span><span class="sxs-lookup"><span data-stu-id="8c6d7-151">Last update time</span></span>|
|<span data-ttu-id="8c6d7-152">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="8c6d7-152">configurationVersion</span></span>|<span data-ttu-id="8c6d7-153">Int32</span><span class="sxs-lookup"><span data-stu-id="8c6d7-153">Int32</span></span>|<span data-ttu-id="8c6d7-154">Version der Richtlinie für diese Übersicht</span><span class="sxs-lookup"><span data-stu-id="8c6d7-154">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="8c6d7-155">Antwort</span><span class="sxs-lookup"><span data-stu-id="8c6d7-155">Response</span></span>
<span data-ttu-id="8c6d7-156">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) zurück.</span><span class="sxs-lookup"><span data-stu-id="8c6d7-156">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8c6d7-157">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8c6d7-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="8c6d7-158">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8c6d7-158">Request</span></span>
<span data-ttu-id="8c6d7-159">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8c6d7-159">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatusSummary
Content-type: application/json
Content-length: 297

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationUserSummary",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```

### <a name="response"></a><span data-ttu-id="8c6d7-160">Antwort</span><span class="sxs-lookup"><span data-stu-id="8c6d7-160">Response</span></span>
<span data-ttu-id="8c6d7-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8c6d7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 346

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationUserSummary",
  "id": "7b953742-3742-7b95-4237-957b4237957b",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```



