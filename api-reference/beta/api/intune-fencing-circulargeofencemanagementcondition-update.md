---
title: CircularGeofenceManagementCondition aktualisieren
description: Aktualisieren der Eigenschaften eines circularGeofenceManagementCondition-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: adb7c23b092bb163a668cd3906f93a8ac8fd609e
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30175213"
---
# <a name="update-circulargeofencemanagementcondition"></a><span data-ttu-id="f4f0e-103">CircularGeofenceManagementCondition aktualisieren</span><span class="sxs-lookup"><span data-stu-id="f4f0e-103">Update circularGeofenceManagementCondition</span></span>

> <span data-ttu-id="f4f0e-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f4f0e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f4f0e-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="f4f0e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f4f0e-106">Aktualisieren der Eigenschaften eines [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="f4f0e-106">Update the properties of a [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f4f0e-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f4f0e-107">Prerequisites</span></span>
<span data-ttu-id="f4f0e-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="f4f0e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f4f0e-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f4f0e-110">Permission type</span></span>|<span data-ttu-id="f4f0e-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f4f0e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f4f0e-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f4f0e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f4f0e-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4f0e-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f4f0e-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f4f0e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f4f0e-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f4f0e-115">Not supported.</span></span>|
|<span data-ttu-id="f4f0e-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f4f0e-116">Application</span></span>|<span data-ttu-id="f4f0e-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f4f0e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f4f0e-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f4f0e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managementConditions/{managementConditionId}
PATCH /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions/{managementConditionId}
```

## <a name="request-headers"></a><span data-ttu-id="f4f0e-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f4f0e-119">Request headers</span></span>
|<span data-ttu-id="f4f0e-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="f4f0e-120">Header</span></span>|<span data-ttu-id="f4f0e-121">Wert</span><span class="sxs-lookup"><span data-stu-id="f4f0e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f4f0e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f4f0e-122">Authorization</span></span>|<span data-ttu-id="f4f0e-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="f4f0e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f4f0e-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="f4f0e-124">Accept</span></span>|<span data-ttu-id="f4f0e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f4f0e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f4f0e-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f4f0e-126">Request body</span></span>
<span data-ttu-id="f4f0e-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="f4f0e-127">In the request body, supply a JSON representation for the [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) object.</span></span>

<span data-ttu-id="f4f0e-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="f4f0e-128">The following table shows the properties that are required when you create the [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md).</span></span>

|<span data-ttu-id="f4f0e-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f4f0e-129">Property</span></span>|<span data-ttu-id="f4f0e-130">Typ</span><span class="sxs-lookup"><span data-stu-id="f4f0e-130">Type</span></span>|<span data-ttu-id="f4f0e-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f4f0e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f4f0e-132">id</span><span class="sxs-lookup"><span data-stu-id="f4f0e-132">id</span></span>|<span data-ttu-id="f4f0e-133">string</span><span class="sxs-lookup"><span data-stu-id="f4f0e-133">String</span></span>|<span data-ttu-id="f4f0e-134">Eindeutiger Bezeichner für die Verwaltungsbedingung.</span><span class="sxs-lookup"><span data-stu-id="f4f0e-134">Unique identifier for the management condition.</span></span> <span data-ttu-id="f4f0e-135">Vom System generierter Wert, der bei der Erstellung zugewiesen wird.</span><span class="sxs-lookup"><span data-stu-id="f4f0e-135">System generated value assigned when created.</span></span> <span data-ttu-id="f4f0e-136">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="f4f0e-136">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="f4f0e-137">uniqueName</span><span class="sxs-lookup"><span data-stu-id="f4f0e-137">uniqueName</span></span>|<span data-ttu-id="f4f0e-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f4f0e-138">String</span></span>|<span data-ttu-id="f4f0e-139">Eindeutiger Name für die Verwaltungsbedingung.</span><span class="sxs-lookup"><span data-stu-id="f4f0e-139">Unique name for the management condition.</span></span> <span data-ttu-id="f4f0e-140">Wird in Verwaltungs Bedingungsausdrücken verwendet.</span><span class="sxs-lookup"><span data-stu-id="f4f0e-140">Used in management condition expressions.</span></span> <span data-ttu-id="f4f0e-141">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="f4f0e-141">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="f4f0e-142">displayName</span><span class="sxs-lookup"><span data-stu-id="f4f0e-142">displayName</span></span>|<span data-ttu-id="f4f0e-143">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f4f0e-143">String</span></span>|<span data-ttu-id="f4f0e-144">Der Administrator definierte Name der Verwaltungsbedingung.</span><span class="sxs-lookup"><span data-stu-id="f4f0e-144">The admin defined name of the management condition.</span></span> <span data-ttu-id="f4f0e-145">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="f4f0e-145">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="f4f0e-146">description</span><span class="sxs-lookup"><span data-stu-id="f4f0e-146">description</span></span>|<span data-ttu-id="f4f0e-147">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f4f0e-147">String</span></span>|<span data-ttu-id="f4f0e-148">Die vom Administrator definierte Beschreibung der Verwaltungsbedingung.</span><span class="sxs-lookup"><span data-stu-id="f4f0e-148">The admin defined description of the management condition.</span></span> <span data-ttu-id="f4f0e-149">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="f4f0e-149">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="f4f0e-150">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f4f0e-150">createdDateTime</span></span>|<span data-ttu-id="f4f0e-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f4f0e-151">DateTimeOffset</span></span>|<span data-ttu-id="f4f0e-152">Der Zeitpunkt, zu dem die Verwaltungsbedingung erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="f4f0e-152">The time the management condition was created.</span></span> <span data-ttu-id="f4f0e-153">Generierte Dienstseite.</span><span class="sxs-lookup"><span data-stu-id="f4f0e-153">Generated service side.</span></span> <span data-ttu-id="f4f0e-154">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="f4f0e-154">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="f4f0e-155">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f4f0e-155">modifiedDateTime</span></span>|<span data-ttu-id="f4f0e-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f4f0e-156">DateTimeOffset</span></span>|<span data-ttu-id="f4f0e-157">Der Zeitpunkt, zu dem die Verwaltungsbedingung zuletzt geändert wurde.</span><span class="sxs-lookup"><span data-stu-id="f4f0e-157">The time the management condition was last modified.</span></span> <span data-ttu-id="f4f0e-158">Aktualisierte Dienstseite.</span><span class="sxs-lookup"><span data-stu-id="f4f0e-158">Updated service side.</span></span> <span data-ttu-id="f4f0e-159">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="f4f0e-159">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="f4f0e-160">eTag</span><span class="sxs-lookup"><span data-stu-id="f4f0e-160">eTag</span></span>|<span data-ttu-id="f4f0e-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f4f0e-161">String</span></span>|<span data-ttu-id="f4f0e-162">ETag der Verwaltungsbedingung.</span><span class="sxs-lookup"><span data-stu-id="f4f0e-162">ETag of the management condition.</span></span> <span data-ttu-id="f4f0e-163">Aktualisierte Dienstseite.</span><span class="sxs-lookup"><span data-stu-id="f4f0e-163">Updated service side.</span></span> <span data-ttu-id="f4f0e-164">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="f4f0e-164">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="f4f0e-165">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="f4f0e-165">applicablePlatforms</span></span>|<span data-ttu-id="f4f0e-166">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="f4f0e-166">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="f4f0e-167">Die entsprechenden Plattformen für diese Verwaltungsbedingung.</span><span class="sxs-lookup"><span data-stu-id="f4f0e-167">The applicable platforms for this management condition.</span></span> <span data-ttu-id="f4f0e-168">Von [ManagementCondition](../resources/intune-fencing-managementcondition.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="f4f0e-168">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md).</span></span> <span data-ttu-id="f4f0e-169">Mögliche Werte sind: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater` und `androidWorkProfile`.</span><span class="sxs-lookup"><span data-stu-id="f4f0e-169">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`.</span></span>|
|<span data-ttu-id="f4f0e-170">latitude</span><span class="sxs-lookup"><span data-stu-id="f4f0e-170">latitude</span></span>|<span data-ttu-id="f4f0e-171">Double</span><span class="sxs-lookup"><span data-stu-id="f4f0e-171">Double</span></span>|<span data-ttu-id="f4f0e-172">Latitude in Grad, zwischen-90 und + 90 inklusive.</span><span class="sxs-lookup"><span data-stu-id="f4f0e-172">Latitude in degrees, between -90 and +90 inclusive.</span></span>|
|<span data-ttu-id="f4f0e-173">longitude</span><span class="sxs-lookup"><span data-stu-id="f4f0e-173">longitude</span></span>|<span data-ttu-id="f4f0e-174">Gleitkommawert mit doppelter Genauigkeit</span><span class="sxs-lookup"><span data-stu-id="f4f0e-174">Double</span></span>|<span data-ttu-id="f4f0e-175">Längengrad, zwischen-180 und + 180 inklusive.</span><span class="sxs-lookup"><span data-stu-id="f4f0e-175">Longitude in degrees, between -180 and +180 inclusive.</span></span>|
|<span data-ttu-id="f4f0e-176">radiusInMeters</span><span class="sxs-lookup"><span data-stu-id="f4f0e-176">radiusInMeters</span></span>|<span data-ttu-id="f4f0e-177">Einzel</span><span class="sxs-lookup"><span data-stu-id="f4f0e-177">Single</span></span>|<span data-ttu-id="f4f0e-178">Radius in Meter.</span><span class="sxs-lookup"><span data-stu-id="f4f0e-178">Radius in meters.</span></span>|



## <a name="response"></a><span data-ttu-id="f4f0e-179">Antwort</span><span class="sxs-lookup"><span data-stu-id="f4f0e-179">Response</span></span>
<span data-ttu-id="f4f0e-180">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="f4f0e-180">If successful, this method returns a `200 OK` response code and an updated [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f4f0e-181">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f4f0e-181">Example</span></span>

### <a name="request"></a><span data-ttu-id="f4f0e-182">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f4f0e-182">Request</span></span>
<span data-ttu-id="f4f0e-183">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f4f0e-183">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/managementConditions/{managementConditionId}
Content-type: application/json
Content-length: 444

{
  "@odata.type": "#microsoft.graph.circularGeofenceManagementCondition",
  "uniqueName": "Unique Name value",
  "displayName": "Display Name value",
  "description": "Description value",
  "eTag": "ETag value",
  "applicablePlatforms": [
    "androidForWork"
  ],
  "latitude": "<Unknown Primitive Type Edm.Double>",
  "longitude": "<Unknown Primitive Type Edm.Double>",
  "radiusInMeters": "<Unknown Primitive Type Edm.Single>"
}
```

### <a name="response"></a><span data-ttu-id="f4f0e-184">Antwort</span><span class="sxs-lookup"><span data-stu-id="f4f0e-184">Response</span></span>
<span data-ttu-id="f4f0e-p110">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f4f0e-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 612

{
  "@odata.type": "#microsoft.graph.circularGeofenceManagementCondition",
  "id": "30ee27b6-27b6-30ee-b627-ee30b627ee30",
  "uniqueName": "Unique Name value",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
  "eTag": "ETag value",
  "applicablePlatforms": [
    "androidForWork"
  ],
  "latitude": "<Unknown Primitive Type Edm.Double>",
  "longitude": "<Unknown Primitive Type Edm.Double>",
  "radiusInMeters": "<Unknown Primitive Type Edm.Single>"
}
```




