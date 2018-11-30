---
title: Aktualisieren von „iosUpdateConfiguration“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs iosUpdateConfiguration.
ms.openlocfilehash: f1ea4fec09eb2b81656dd5838136be679747ca95
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058505"
---
# <a name="update-iosupdateconfiguration"></a><span data-ttu-id="7a6b5-103">Aktualisieren von „iosUpdateConfiguration“</span><span class="sxs-lookup"><span data-stu-id="7a6b5-103">Update iosUpdateConfiguration</span></span>

> <span data-ttu-id="7a6b5-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="7a6b5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7a6b5-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7a6b5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7a6b5-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="7a6b5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7a6b5-107">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7a6b5-107">Update the properties of a [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7a6b5-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="7a6b5-108">Prerequisites</span></span>
<span data-ttu-id="7a6b5-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7a6b5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7a6b5-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7a6b5-111">Permission type</span></span>|<span data-ttu-id="7a6b5-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7a6b5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7a6b5-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7a6b5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7a6b5-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7a6b5-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7a6b5-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7a6b5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7a6b5-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7a6b5-116">Not supported.</span></span>|
|<span data-ttu-id="7a6b5-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7a6b5-117">Application</span></span>|<span data-ttu-id="7a6b5-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7a6b5-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7a6b5-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7a6b5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="7a6b5-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7a6b5-120">Request headers</span></span>
|<span data-ttu-id="7a6b5-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="7a6b5-121">Header</span></span>|<span data-ttu-id="7a6b5-122">Wert</span><span class="sxs-lookup"><span data-stu-id="7a6b5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7a6b5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7a6b5-123">Authorization</span></span>|<span data-ttu-id="7a6b5-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="7a6b5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7a6b5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7a6b5-125">Accept</span></span>|<span data-ttu-id="7a6b5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7a6b5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7a6b5-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7a6b5-127">Request body</span></span>
<span data-ttu-id="7a6b5-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) an.</span><span class="sxs-lookup"><span data-stu-id="7a6b5-128">In the request body, supply a JSON representation for the [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object.</span></span>

<span data-ttu-id="7a6b5-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="7a6b5-129">The following table shows the properties that are required when you create the [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md).</span></span>

|<span data-ttu-id="7a6b5-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7a6b5-130">Property</span></span>|<span data-ttu-id="7a6b5-131">Typ</span><span class="sxs-lookup"><span data-stu-id="7a6b5-131">Type</span></span>|<span data-ttu-id="7a6b5-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7a6b5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7a6b5-133">id</span><span class="sxs-lookup"><span data-stu-id="7a6b5-133">id</span></span>|<span data-ttu-id="7a6b5-134">String</span><span class="sxs-lookup"><span data-stu-id="7a6b5-134">String</span></span>|<span data-ttu-id="7a6b5-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="7a6b5-135">Key of the entity.</span></span> <span data-ttu-id="7a6b5-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7a6b5-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7a6b5-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7a6b5-137">lastModifiedDateTime</span></span>|<span data-ttu-id="7a6b5-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7a6b5-138">DateTimeOffset</span></span>|<span data-ttu-id="7a6b5-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="7a6b5-139">DateTime the object was last modified.</span></span> <span data-ttu-id="7a6b5-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7a6b5-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7a6b5-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="7a6b5-141">roleScopeTagIds</span></span>|<span data-ttu-id="7a6b5-142">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="7a6b5-142">String collection</span></span>|<span data-ttu-id="7a6b5-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="7a6b5-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="7a6b5-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7a6b5-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7a6b5-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="7a6b5-145">supportsScopeTags</span></span>|<span data-ttu-id="7a6b5-146">Boolesch</span><span class="sxs-lookup"><span data-stu-id="7a6b5-146">Boolean</span></span>|<span data-ttu-id="7a6b5-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7a6b5-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="7a6b5-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="7a6b5-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="7a6b5-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="7a6b5-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="7a6b5-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="7a6b5-150">This property is read-only.</span></span> <span data-ttu-id="7a6b5-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7a6b5-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7a6b5-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7a6b5-152">createdDateTime</span></span>|<span data-ttu-id="7a6b5-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7a6b5-153">DateTimeOffset</span></span>|<span data-ttu-id="7a6b5-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="7a6b5-154">DateTime the object was created.</span></span> <span data-ttu-id="7a6b5-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7a6b5-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7a6b5-156">description</span><span class="sxs-lookup"><span data-stu-id="7a6b5-156">description</span></span>|<span data-ttu-id="7a6b5-157">String</span><span class="sxs-lookup"><span data-stu-id="7a6b5-157">String</span></span>|<span data-ttu-id="7a6b5-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="7a6b5-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="7a6b5-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7a6b5-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7a6b5-160">displayName</span><span class="sxs-lookup"><span data-stu-id="7a6b5-160">displayName</span></span>|<span data-ttu-id="7a6b5-161">String</span><span class="sxs-lookup"><span data-stu-id="7a6b5-161">String</span></span>|<span data-ttu-id="7a6b5-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="7a6b5-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="7a6b5-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7a6b5-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7a6b5-164">Version</span><span class="sxs-lookup"><span data-stu-id="7a6b5-164">version</span></span>|<span data-ttu-id="7a6b5-165">Int32</span><span class="sxs-lookup"><span data-stu-id="7a6b5-165">Int32</span></span>|<span data-ttu-id="7a6b5-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="7a6b5-166">Version of the device configuration.</span></span> <span data-ttu-id="7a6b5-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7a6b5-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7a6b5-168">isEnabled</span><span class="sxs-lookup"><span data-stu-id="7a6b5-168">isEnabled</span></span>|<span data-ttu-id="7a6b5-169">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="7a6b5-169">Boolean</span></span>|<span data-ttu-id="7a6b5-170">Die Einstellung wird in der Benutzeroberfläche aktiviert werden</span><span class="sxs-lookup"><span data-stu-id="7a6b5-170">Is setting enabled in UI</span></span>|
|<span data-ttu-id="7a6b5-171">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="7a6b5-171">activeHoursStart</span></span>|<span data-ttu-id="7a6b5-172">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="7a6b5-172">TimeOfDay</span></span>|<span data-ttu-id="7a6b5-173">Beginn der aktiven Stunden (Als aktive Stunden wird das Zeitfenster bezeichnet, in dem keine Updates installiert werden sollen.)</span><span class="sxs-lookup"><span data-stu-id="7a6b5-173">Active Hours Start (active hours mean the time window when updates install should not happen)</span></span>|
|<span data-ttu-id="7a6b5-174">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="7a6b5-174">activeHoursEnd</span></span>|<span data-ttu-id="7a6b5-175">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="7a6b5-175">TimeOfDay</span></span>|<span data-ttu-id="7a6b5-176">Ende der aktiven Stunden (Als aktive Stunden wird das Zeitfenster bezeichnet, in dem keine Updates installiert werden sollen.)</span><span class="sxs-lookup"><span data-stu-id="7a6b5-176">Active Hours End (active hours mean the time window when updates install should not happen)</span></span>|
|<span data-ttu-id="7a6b5-177">scheduledInstallDays</span><span class="sxs-lookup"><span data-stu-id="7a6b5-177">scheduledInstallDays</span></span>|<span data-ttu-id="7a6b5-178">[DayOfWeek](../resources/intune-deviceconfig-dayofweek.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="7a6b5-178">[dayOfWeek](../resources/intune-deviceconfig-dayofweek.md) collection</span></span>|<span data-ttu-id="7a6b5-179">Tage in der Woche, für die aktive Stunden konfiguriert sind.</span><span class="sxs-lookup"><span data-stu-id="7a6b5-179">Days in week for which active hours are configured.</span></span> <span data-ttu-id="7a6b5-180">Diese Sammlung darf maximal 7 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="7a6b5-180">This collection can contain a maximum of 7 elements.</span></span> <span data-ttu-id="7a6b5-181">Mögliche Werte sind: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday` und `saturday`.</span><span class="sxs-lookup"><span data-stu-id="7a6b5-181">Possible values are: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="7a6b5-182">utcTimeOffsetInMinutes</span><span class="sxs-lookup"><span data-stu-id="7a6b5-182">utcTimeOffsetInMinutes</span></span>|<span data-ttu-id="7a6b5-183">Int32</span><span class="sxs-lookup"><span data-stu-id="7a6b5-183">Int32</span></span>|<span data-ttu-id="7a6b5-184">UTC-Zeitversatz in Minuten</span><span class="sxs-lookup"><span data-stu-id="7a6b5-184">UTC Time Offset indicated in minutes</span></span>|
|<span data-ttu-id="7a6b5-185">enforcedSoftwareUpdateDelayInDays</span><span class="sxs-lookup"><span data-stu-id="7a6b5-185">enforcedSoftwareUpdateDelayInDays</span></span>|<span data-ttu-id="7a6b5-186">Int32</span><span class="sxs-lookup"><span data-stu-id="7a6b5-186">Int32</span></span>|<span data-ttu-id="7a6b5-187">Tage vor Softwareupdates für iOS-Geräte, die im Bereich von 0 bis 90 inklusive sichtbar sind</span><span class="sxs-lookup"><span data-stu-id="7a6b5-187">Days before software updates are visible to iOS devices ranging from 0 to 90 inclusive</span></span>|



## <a name="response"></a><span data-ttu-id="7a6b5-188">Antwort</span><span class="sxs-lookup"><span data-stu-id="7a6b5-188">Response</span></span>
<span data-ttu-id="7a6b5-189">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="7a6b5-189">If successful, this method returns a `200 OK` response code and an updated [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7a6b5-190">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7a6b5-190">Example</span></span>
### <a name="request"></a><span data-ttu-id="7a6b5-191">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7a6b5-191">Request</span></span>
<span data-ttu-id="7a6b5-192">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7a6b5-192">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 485

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "isEnabled": true,
  "activeHoursStart": "12:00:05.5020000",
  "activeHoursEnd": "11:59:00.8990000",
  "scheduledInstallDays": [
    "monday"
  ],
  "utcTimeOffsetInMinutes": 6,
  "enforcedSoftwareUpdateDelayInDays": 1
}
```

### <a name="response"></a><span data-ttu-id="7a6b5-193">Antwort</span><span class="sxs-lookup"><span data-stu-id="7a6b5-193">Response</span></span>
<span data-ttu-id="7a6b5-p112">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7a6b5-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 654

{
  "@odata.type": "#microsoft.graph.iosUpdateConfiguration",
  "id": "321aef09-ef09-321a-09ef-1a3209ef1a32",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "isEnabled": true,
  "activeHoursStart": "12:00:05.5020000",
  "activeHoursEnd": "11:59:00.8990000",
  "scheduledInstallDays": [
    "monday"
  ],
  "utcTimeOffsetInMinutes": 6,
  "enforcedSoftwareUpdateDelayInDays": 1
}
```





