---
title: CircularGeofenceManagementCondition erstellen
description: Erstellen eines neuen circularGeofenceManagementCondition-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b437d163de5ebe211d6fe73b6ac0064c7081d6a7
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30981559"
---
# <a name="create-circulargeofencemanagementcondition"></a><span data-ttu-id="8b40d-103">CircularGeofenceManagementCondition erstellen</span><span class="sxs-lookup"><span data-stu-id="8b40d-103">Create circularGeofenceManagementCondition</span></span>

> <span data-ttu-id="8b40d-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8b40d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8b40d-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="8b40d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8b40d-106">Erstellen eines neuen [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="8b40d-106">Create a new [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8b40d-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="8b40d-107">Prerequisites</span></span>
<span data-ttu-id="8b40d-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8b40d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8b40d-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8b40d-110">Permission type</span></span>|<span data-ttu-id="8b40d-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8b40d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8b40d-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8b40d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8b40d-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b40d-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8b40d-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8b40d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8b40d-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8b40d-115">Not supported.</span></span>|
|<span data-ttu-id="8b40d-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8b40d-116">Application</span></span>|<span data-ttu-id="8b40d-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8b40d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8b40d-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8b40d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managementConditions
POST /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions
```

## <a name="request-headers"></a><span data-ttu-id="8b40d-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8b40d-119">Request headers</span></span>
|<span data-ttu-id="8b40d-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="8b40d-120">Header</span></span>|<span data-ttu-id="8b40d-121">Wert</span><span class="sxs-lookup"><span data-stu-id="8b40d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8b40d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8b40d-122">Authorization</span></span>|<span data-ttu-id="8b40d-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="8b40d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8b40d-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="8b40d-124">Accept</span></span>|<span data-ttu-id="8b40d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8b40d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8b40d-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8b40d-126">Request body</span></span>
<span data-ttu-id="8b40d-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das circularGeofenceManagementCondition-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="8b40d-127">In the request body, supply a JSON representation for the circularGeofenceManagementCondition object.</span></span>

<span data-ttu-id="8b40d-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der circularGeofenceManagementCondition erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="8b40d-128">The following table shows the properties that are required when you create the circularGeofenceManagementCondition.</span></span>

|<span data-ttu-id="8b40d-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8b40d-129">Property</span></span>|<span data-ttu-id="8b40d-130">Typ</span><span class="sxs-lookup"><span data-stu-id="8b40d-130">Type</span></span>|<span data-ttu-id="8b40d-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8b40d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8b40d-132">id</span><span class="sxs-lookup"><span data-stu-id="8b40d-132">id</span></span>|<span data-ttu-id="8b40d-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8b40d-133">String</span></span>|<span data-ttu-id="8b40d-134">Eindeutiger Bezeichner für die Verwaltungsbedingung.</span><span class="sxs-lookup"><span data-stu-id="8b40d-134">Unique identifier for the management condition.</span></span> <span data-ttu-id="8b40d-135">Vom System generierter Wert, der bei der Erstellung zugewiesen wird.</span><span class="sxs-lookup"><span data-stu-id="8b40d-135">System generated value assigned when created.</span></span> <span data-ttu-id="8b40d-136">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="8b40d-136">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="8b40d-137">uniqueName</span><span class="sxs-lookup"><span data-stu-id="8b40d-137">uniqueName</span></span>|<span data-ttu-id="8b40d-138">String</span><span class="sxs-lookup"><span data-stu-id="8b40d-138">String</span></span>|<span data-ttu-id="8b40d-139">Eindeutiger Name für die Verwaltungsbedingung.</span><span class="sxs-lookup"><span data-stu-id="8b40d-139">Unique name for the management condition.</span></span> <span data-ttu-id="8b40d-140">Wird in Verwaltungs Bedingungsausdrücken verwendet.</span><span class="sxs-lookup"><span data-stu-id="8b40d-140">Used in management condition expressions.</span></span> <span data-ttu-id="8b40d-141">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="8b40d-141">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="8b40d-142">displayName</span><span class="sxs-lookup"><span data-stu-id="8b40d-142">displayName</span></span>|<span data-ttu-id="8b40d-143">String</span><span class="sxs-lookup"><span data-stu-id="8b40d-143">String</span></span>|<span data-ttu-id="8b40d-144">Der Administrator definierte Name der Verwaltungsbedingung.</span><span class="sxs-lookup"><span data-stu-id="8b40d-144">The admin defined name of the management condition.</span></span> <span data-ttu-id="8b40d-145">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="8b40d-145">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="8b40d-146">description</span><span class="sxs-lookup"><span data-stu-id="8b40d-146">description</span></span>|<span data-ttu-id="8b40d-147">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8b40d-147">String</span></span>|<span data-ttu-id="8b40d-148">Die vom Administrator definierte Beschreibung der Verwaltungsbedingung.</span><span class="sxs-lookup"><span data-stu-id="8b40d-148">The admin defined description of the management condition.</span></span> <span data-ttu-id="8b40d-149">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="8b40d-149">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="8b40d-150">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8b40d-150">createdDateTime</span></span>|<span data-ttu-id="8b40d-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8b40d-151">DateTimeOffset</span></span>|<span data-ttu-id="8b40d-152">Der Zeitpunkt, zu dem die Verwaltungsbedingung erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="8b40d-152">The time the management condition was created.</span></span> <span data-ttu-id="8b40d-153">Generierte Dienstseite.</span><span class="sxs-lookup"><span data-stu-id="8b40d-153">Generated service side.</span></span> <span data-ttu-id="8b40d-154">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="8b40d-154">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="8b40d-155">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8b40d-155">modifiedDateTime</span></span>|<span data-ttu-id="8b40d-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8b40d-156">DateTimeOffset</span></span>|<span data-ttu-id="8b40d-157">Der Zeitpunkt, zu dem die Verwaltungsbedingung zuletzt geändert wurde.</span><span class="sxs-lookup"><span data-stu-id="8b40d-157">The time the management condition was last modified.</span></span> <span data-ttu-id="8b40d-158">Aktualisierte Dienstseite.</span><span class="sxs-lookup"><span data-stu-id="8b40d-158">Updated service side.</span></span> <span data-ttu-id="8b40d-159">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="8b40d-159">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="8b40d-160">eTag</span><span class="sxs-lookup"><span data-stu-id="8b40d-160">eTag</span></span>|<span data-ttu-id="8b40d-161">String</span><span class="sxs-lookup"><span data-stu-id="8b40d-161">String</span></span>|<span data-ttu-id="8b40d-162">ETag der Verwaltungsbedingung.</span><span class="sxs-lookup"><span data-stu-id="8b40d-162">ETag of the management condition.</span></span> <span data-ttu-id="8b40d-163">Aktualisierte Dienstseite.</span><span class="sxs-lookup"><span data-stu-id="8b40d-163">Updated service side.</span></span> <span data-ttu-id="8b40d-164">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="8b40d-164">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="8b40d-165">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="8b40d-165">applicablePlatforms</span></span>|<span data-ttu-id="8b40d-166">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="8b40d-166">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="8b40d-167">Die entsprechenden Plattformen für diese Verwaltungsbedingung.</span><span class="sxs-lookup"><span data-stu-id="8b40d-167">The applicable platforms for this management condition.</span></span> <span data-ttu-id="8b40d-168">Von [ManagementCondition](../resources/intune-fencing-managementcondition.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="8b40d-168">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md).</span></span> <span data-ttu-id="8b40d-169">Mögliche Werte: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`.</span><span class="sxs-lookup"><span data-stu-id="8b40d-169">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`.</span></span>|
|<span data-ttu-id="8b40d-170">latitude</span><span class="sxs-lookup"><span data-stu-id="8b40d-170">latitude</span></span>|<span data-ttu-id="8b40d-171">Gleitkommawert mit doppelter Genauigkeit</span><span class="sxs-lookup"><span data-stu-id="8b40d-171">Double</span></span>|<span data-ttu-id="8b40d-172">Latitude in Grad, zwischen-90 und + 90 inklusive.</span><span class="sxs-lookup"><span data-stu-id="8b40d-172">Latitude in degrees, between -90 and +90 inclusive.</span></span>|
|<span data-ttu-id="8b40d-173">longitude</span><span class="sxs-lookup"><span data-stu-id="8b40d-173">longitude</span></span>|<span data-ttu-id="8b40d-174">Gleitkommawert mit doppelter Genauigkeit</span><span class="sxs-lookup"><span data-stu-id="8b40d-174">Double</span></span>|<span data-ttu-id="8b40d-175">Längengrad, zwischen-180 und + 180 inklusive.</span><span class="sxs-lookup"><span data-stu-id="8b40d-175">Longitude in degrees, between -180 and +180 inclusive.</span></span>|
|<span data-ttu-id="8b40d-176">radiusInMeters</span><span class="sxs-lookup"><span data-stu-id="8b40d-176">radiusInMeters</span></span>|<span data-ttu-id="8b40d-177">Einzel</span><span class="sxs-lookup"><span data-stu-id="8b40d-177">Single</span></span>|<span data-ttu-id="8b40d-178">Radius in Meter.</span><span class="sxs-lookup"><span data-stu-id="8b40d-178">Radius in meters.</span></span>|



## <a name="response"></a><span data-ttu-id="8b40d-179">Antwort</span><span class="sxs-lookup"><span data-stu-id="8b40d-179">Response</span></span>
<span data-ttu-id="8b40d-180">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="8b40d-180">If successful, this method returns a `201 Created` response code and a [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8b40d-181">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8b40d-181">Example</span></span>

### <a name="request"></a><span data-ttu-id="8b40d-182">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8b40d-182">Request</span></span>
<span data-ttu-id="8b40d-183">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8b40d-183">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managementConditions
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

### <a name="response"></a><span data-ttu-id="8b40d-184">Antwort</span><span class="sxs-lookup"><span data-stu-id="8b40d-184">Response</span></span>
<span data-ttu-id="8b40d-p110">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8b40d-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




