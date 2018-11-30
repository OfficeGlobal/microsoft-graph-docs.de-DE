---
title: Erstellen von circularGeofenceManagementCondition
description: Erstellen eines neuen CircularGeofenceManagementCondition-Objekts.
ms.openlocfilehash: 1d25e2e8f712683462e7751b4ca874403b750da2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065095"
---
# <a name="create-circulargeofencemanagementcondition"></a><span data-ttu-id="382c7-103">Erstellen von circularGeofenceManagementCondition</span><span class="sxs-lookup"><span data-stu-id="382c7-103">Create circularGeofenceManagementCondition</span></span>

> <span data-ttu-id="382c7-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="382c7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="382c7-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="382c7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="382c7-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="382c7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="382c7-107">Erstellen eines neuen [CircularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="382c7-107">Create a new [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="382c7-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="382c7-108">Prerequisites</span></span>
<span data-ttu-id="382c7-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="382c7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="382c7-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="382c7-111">Permission type</span></span>|<span data-ttu-id="382c7-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="382c7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="382c7-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="382c7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="382c7-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="382c7-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="382c7-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="382c7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="382c7-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="382c7-116">Not supported.</span></span>|
|<span data-ttu-id="382c7-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="382c7-117">Application</span></span>|<span data-ttu-id="382c7-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="382c7-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="382c7-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="382c7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managementConditions
POST /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions
```

## <a name="request-headers"></a><span data-ttu-id="382c7-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="382c7-120">Request headers</span></span>
|<span data-ttu-id="382c7-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="382c7-121">Header</span></span>|<span data-ttu-id="382c7-122">Wert</span><span class="sxs-lookup"><span data-stu-id="382c7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="382c7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="382c7-123">Authorization</span></span>|<span data-ttu-id="382c7-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="382c7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="382c7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="382c7-125">Accept</span></span>|<span data-ttu-id="382c7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="382c7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="382c7-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="382c7-127">Request body</span></span>
<span data-ttu-id="382c7-128">Geben Sie im Textkörper Anforderung für das Objekt CircularGeofenceManagementCondition eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="382c7-128">In the request body, supply a JSON representation for the circularGeofenceManagementCondition object.</span></span>

<span data-ttu-id="382c7-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die CircularGeofenceManagementCondition erstellen.</span><span class="sxs-lookup"><span data-stu-id="382c7-129">The following table shows the properties that are required when you create the circularGeofenceManagementCondition.</span></span>

|<span data-ttu-id="382c7-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="382c7-130">Property</span></span>|<span data-ttu-id="382c7-131">Typ</span><span class="sxs-lookup"><span data-stu-id="382c7-131">Type</span></span>|<span data-ttu-id="382c7-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="382c7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="382c7-133">id</span><span class="sxs-lookup"><span data-stu-id="382c7-133">id</span></span>|<span data-ttu-id="382c7-134">String</span><span class="sxs-lookup"><span data-stu-id="382c7-134">String</span></span>|<span data-ttu-id="382c7-135">Eindeutiger Bezeichner für die Bedingung Management.</span><span class="sxs-lookup"><span data-stu-id="382c7-135">Unique identifier for the management condition.</span></span> <span data-ttu-id="382c7-136">System generierten Wert, die beim Erstellen zugewiesen.</span><span class="sxs-lookup"><span data-stu-id="382c7-136">System generated value assigned when created.</span></span> <span data-ttu-id="382c7-137">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="382c7-137">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="382c7-138">uniqueName</span><span class="sxs-lookup"><span data-stu-id="382c7-138">uniqueName</span></span>|<span data-ttu-id="382c7-139">String</span><span class="sxs-lookup"><span data-stu-id="382c7-139">String</span></span>|<span data-ttu-id="382c7-140">Eindeutiger Name für die Bedingung Management.</span><span class="sxs-lookup"><span data-stu-id="382c7-140">Unique name for the management condition.</span></span> <span data-ttu-id="382c7-141">In Management Bedingung Ausdrücken verwendet.</span><span class="sxs-lookup"><span data-stu-id="382c7-141">Used in management condition expressions.</span></span> <span data-ttu-id="382c7-142">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="382c7-142">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="382c7-143">displayName</span><span class="sxs-lookup"><span data-stu-id="382c7-143">displayName</span></span>|<span data-ttu-id="382c7-144">String</span><span class="sxs-lookup"><span data-stu-id="382c7-144">String</span></span>|<span data-ttu-id="382c7-145">Der Administrator definierter Name der Bedingung Management.</span><span class="sxs-lookup"><span data-stu-id="382c7-145">The admin defined name of the management condition.</span></span> <span data-ttu-id="382c7-146">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="382c7-146">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="382c7-147">description</span><span class="sxs-lookup"><span data-stu-id="382c7-147">description</span></span>|<span data-ttu-id="382c7-148">String</span><span class="sxs-lookup"><span data-stu-id="382c7-148">String</span></span>|<span data-ttu-id="382c7-149">Der Administrator definiert die Beschreibung der Bedingung Management.</span><span class="sxs-lookup"><span data-stu-id="382c7-149">The admin defined description of the management condition.</span></span> <span data-ttu-id="382c7-150">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="382c7-150">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="382c7-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="382c7-151">createdDateTime</span></span>|<span data-ttu-id="382c7-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="382c7-152">DateTimeOffset</span></span>|<span data-ttu-id="382c7-153">Der Zeitpunkt, an die Bedingung Management erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="382c7-153">The time the management condition was created.</span></span> <span data-ttu-id="382c7-154">Generierte Service-Seite.</span><span class="sxs-lookup"><span data-stu-id="382c7-154">Generated service side.</span></span> <span data-ttu-id="382c7-155">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="382c7-155">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="382c7-156">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="382c7-156">modifiedDateTime</span></span>|<span data-ttu-id="382c7-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="382c7-157">DateTimeOffset</span></span>|<span data-ttu-id="382c7-158">Die Zeit, die die Bedingung Management zuletzt geändert wurde.</span><span class="sxs-lookup"><span data-stu-id="382c7-158">The time the management condition was last modified.</span></span> <span data-ttu-id="382c7-159">Aktualisierte Service-Seite.</span><span class="sxs-lookup"><span data-stu-id="382c7-159">Updated service side.</span></span> <span data-ttu-id="382c7-160">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="382c7-160">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="382c7-161">eTag</span><span class="sxs-lookup"><span data-stu-id="382c7-161">eTag</span></span>|<span data-ttu-id="382c7-162">String</span><span class="sxs-lookup"><span data-stu-id="382c7-162">String</span></span>|<span data-ttu-id="382c7-163">ETag der Bedingung Management.</span><span class="sxs-lookup"><span data-stu-id="382c7-163">ETag of the management condition.</span></span> <span data-ttu-id="382c7-164">Aktualisierte Service-Seite.</span><span class="sxs-lookup"><span data-stu-id="382c7-164">Updated service side.</span></span> <span data-ttu-id="382c7-165">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="382c7-165">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="382c7-166">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="382c7-166">applicablePlatforms</span></span>|<span data-ttu-id="382c7-167">[DevicePlatformType](../resources/intune-shared-deviceplatformtype.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="382c7-167">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="382c7-168">Die entsprechenden Plattformen für diese Bedingung Management.</span><span class="sxs-lookup"><span data-stu-id="382c7-168">The applicable platforms for this management condition.</span></span> <span data-ttu-id="382c7-169">Geerbt von [ManagementCondition](../resources/intune-fencing-managementcondition.md).</span><span class="sxs-lookup"><span data-stu-id="382c7-169">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md).</span></span> <span data-ttu-id="382c7-170">Mögliche Werte sind: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater` und `androidWorkProfile`.</span><span class="sxs-lookup"><span data-stu-id="382c7-170">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`.</span></span>|
|<span data-ttu-id="382c7-171">latitude</span><span class="sxs-lookup"><span data-stu-id="382c7-171">latitude</span></span>|<span data-ttu-id="382c7-172">Gleitkommawert mit doppelter Genauigkeit</span><span class="sxs-lookup"><span data-stu-id="382c7-172">Double</span></span>|<span data-ttu-id="382c7-173">Breitengrad zwischen-90 und + 90 inklusive in Grad.</span><span class="sxs-lookup"><span data-stu-id="382c7-173">Latitude in degrees, between -90 and +90 inclusive.</span></span>|
|<span data-ttu-id="382c7-174">longitude</span><span class="sxs-lookup"><span data-stu-id="382c7-174">longitude</span></span>|<span data-ttu-id="382c7-175">Gleitkommawert mit doppelter Genauigkeit</span><span class="sxs-lookup"><span data-stu-id="382c7-175">Double</span></span>|<span data-ttu-id="382c7-176">Längengrad in zwischen-180 und inklusive und + 180 Grad.</span><span class="sxs-lookup"><span data-stu-id="382c7-176">Longitude in degrees, between -180 and +180 inclusive.</span></span>|
|<span data-ttu-id="382c7-177">radiusInMeters</span><span class="sxs-lookup"><span data-stu-id="382c7-177">radiusInMeters</span></span>|<span data-ttu-id="382c7-178">Single</span><span class="sxs-lookup"><span data-stu-id="382c7-178">Single</span></span>|<span data-ttu-id="382c7-179">RADIUS in Meter.</span><span class="sxs-lookup"><span data-stu-id="382c7-179">Radius in meters.</span></span>|



## <a name="response"></a><span data-ttu-id="382c7-180">Antwort</span><span class="sxs-lookup"><span data-stu-id="382c7-180">Response</span></span>
<span data-ttu-id="382c7-181">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [CircularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="382c7-181">If successful, this method returns a `201 Created` response code and a [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="382c7-182">Beispiel</span><span class="sxs-lookup"><span data-stu-id="382c7-182">Example</span></span>
### <a name="request"></a><span data-ttu-id="382c7-183">Anforderung</span><span class="sxs-lookup"><span data-stu-id="382c7-183">Request</span></span>
<span data-ttu-id="382c7-184">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="382c7-184">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="382c7-185">Antwort</span><span class="sxs-lookup"><span data-stu-id="382c7-185">Response</span></span>
<span data-ttu-id="382c7-p111">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="382c7-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





