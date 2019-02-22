---
title: Aktualisieren von „iosUpdateConfiguration“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs iosUpdateConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 03c47cbe85b58d15701ab92eb6a7b4e555350fa2
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30143057"
---
# <a name="update-iosupdateconfiguration"></a><span data-ttu-id="3efcd-103">Aktualisieren von „iosUpdateConfiguration“</span><span class="sxs-lookup"><span data-stu-id="3efcd-103">Update iosUpdateConfiguration</span></span>

> <span data-ttu-id="3efcd-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3efcd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3efcd-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="3efcd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3efcd-106">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3efcd-106">Update the properties of a [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3efcd-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="3efcd-107">Prerequisites</span></span>
<span data-ttu-id="3efcd-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="3efcd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="3efcd-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3efcd-110">Permission type</span></span>|<span data-ttu-id="3efcd-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3efcd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3efcd-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3efcd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3efcd-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3efcd-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3efcd-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3efcd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3efcd-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3efcd-115">Not supported.</span></span>|
|<span data-ttu-id="3efcd-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3efcd-116">Application</span></span>|<span data-ttu-id="3efcd-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3efcd-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3efcd-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3efcd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="3efcd-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3efcd-119">Request headers</span></span>
|<span data-ttu-id="3efcd-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="3efcd-120">Header</span></span>|<span data-ttu-id="3efcd-121">Wert</span><span class="sxs-lookup"><span data-stu-id="3efcd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3efcd-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3efcd-122">Authorization</span></span>|<span data-ttu-id="3efcd-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="3efcd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3efcd-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="3efcd-124">Accept</span></span>|<span data-ttu-id="3efcd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3efcd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3efcd-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3efcd-126">Request body</span></span>
<span data-ttu-id="3efcd-127">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) an.</span><span class="sxs-lookup"><span data-stu-id="3efcd-127">In the request body, supply a JSON representation for the [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object.</span></span>

<span data-ttu-id="3efcd-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="3efcd-128">The following table shows the properties that are required when you create the [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md).</span></span>

|<span data-ttu-id="3efcd-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3efcd-129">Property</span></span>|<span data-ttu-id="3efcd-130">Typ</span><span class="sxs-lookup"><span data-stu-id="3efcd-130">Type</span></span>|<span data-ttu-id="3efcd-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3efcd-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3efcd-132">id</span><span class="sxs-lookup"><span data-stu-id="3efcd-132">id</span></span>|<span data-ttu-id="3efcd-133">string</span><span class="sxs-lookup"><span data-stu-id="3efcd-133">String</span></span>|<span data-ttu-id="3efcd-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="3efcd-134">Key of the entity.</span></span> <span data-ttu-id="3efcd-135">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3efcd-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3efcd-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3efcd-136">lastModifiedDateTime</span></span>|<span data-ttu-id="3efcd-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3efcd-137">DateTimeOffset</span></span>|<span data-ttu-id="3efcd-138">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="3efcd-138">DateTime the object was last modified.</span></span> <span data-ttu-id="3efcd-139">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3efcd-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3efcd-140">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="3efcd-140">roleScopeTagIds</span></span>|<span data-ttu-id="3efcd-141">String collection</span><span class="sxs-lookup"><span data-stu-id="3efcd-141">String collection</span></span>|<span data-ttu-id="3efcd-142">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="3efcd-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="3efcd-143">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3efcd-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3efcd-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="3efcd-144">supportsScopeTags</span></span>|<span data-ttu-id="3efcd-145">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="3efcd-145">Boolean</span></span>|<span data-ttu-id="3efcd-146">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereichs Tags unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3efcd-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="3efcd-147">Das Zuweisen zur ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert auf false festgelegt ist und Entitäten für bereichsbezogene Benutzer nicht sichtbar sind.</span><span class="sxs-lookup"><span data-stu-id="3efcd-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="3efcd-148">Dies geschieht für in Silverlight erstellte Legacy Richtlinien und kann durch Löschen und erneutes Erstellen der Richtlinie im Azure-Portal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="3efcd-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="3efcd-149">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="3efcd-149">This property is read-only.</span></span> <span data-ttu-id="3efcd-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3efcd-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3efcd-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3efcd-151">createdDateTime</span></span>|<span data-ttu-id="3efcd-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3efcd-152">DateTimeOffset</span></span>|<span data-ttu-id="3efcd-153">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="3efcd-153">DateTime the object was created.</span></span> <span data-ttu-id="3efcd-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3efcd-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3efcd-155">description</span><span class="sxs-lookup"><span data-stu-id="3efcd-155">description</span></span>|<span data-ttu-id="3efcd-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3efcd-156">String</span></span>|<span data-ttu-id="3efcd-157">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="3efcd-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="3efcd-158">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3efcd-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3efcd-159">displayName</span><span class="sxs-lookup"><span data-stu-id="3efcd-159">displayName</span></span>|<span data-ttu-id="3efcd-160">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3efcd-160">String</span></span>|<span data-ttu-id="3efcd-161">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="3efcd-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="3efcd-162">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3efcd-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3efcd-163">Version</span><span class="sxs-lookup"><span data-stu-id="3efcd-163">version</span></span>|<span data-ttu-id="3efcd-164">Int32</span><span class="sxs-lookup"><span data-stu-id="3efcd-164">Int32</span></span>|<span data-ttu-id="3efcd-165">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="3efcd-165">Version of the device configuration.</span></span> <span data-ttu-id="3efcd-166">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3efcd-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3efcd-167">isEnabled</span><span class="sxs-lookup"><span data-stu-id="3efcd-167">isEnabled</span></span>|<span data-ttu-id="3efcd-168">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="3efcd-168">Boolean</span></span>|<span data-ttu-id="3efcd-169">Einstellung ist in der Benutzeroberfläche aktiviert</span><span class="sxs-lookup"><span data-stu-id="3efcd-169">Is setting enabled in UI</span></span>|
|<span data-ttu-id="3efcd-170">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="3efcd-170">activeHoursStart</span></span>|<span data-ttu-id="3efcd-171">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="3efcd-171">TimeOfDay</span></span>|<span data-ttu-id="3efcd-172">Beginn der aktiven Stunden (Als aktive Stunden wird das Zeitfenster bezeichnet, in dem keine Updates installiert werden sollen.)</span><span class="sxs-lookup"><span data-stu-id="3efcd-172">Active Hours Start (active hours mean the time window when updates install should not happen)</span></span>|
|<span data-ttu-id="3efcd-173">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="3efcd-173">activeHoursEnd</span></span>|<span data-ttu-id="3efcd-174">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="3efcd-174">TimeOfDay</span></span>|<span data-ttu-id="3efcd-175">Ende der aktiven Stunden (Als aktive Stunden wird das Zeitfenster bezeichnet, in dem keine Updates installiert werden sollen.)</span><span class="sxs-lookup"><span data-stu-id="3efcd-175">Active Hours End (active hours mean the time window when updates install should not happen)</span></span>|
|<span data-ttu-id="3efcd-176">scheduledInstallDays</span><span class="sxs-lookup"><span data-stu-id="3efcd-176">scheduledInstallDays</span></span>|<span data-ttu-id="3efcd-177">[DayOfWeek](../resources/intune-deviceconfig-dayofweek.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="3efcd-177">[dayOfWeek](../resources/intune-deviceconfig-dayofweek.md) collection</span></span>|<span data-ttu-id="3efcd-178">Tage in der Woche, für die aktive Stunden konfiguriert sind.</span><span class="sxs-lookup"><span data-stu-id="3efcd-178">Days in week for which active hours are configured.</span></span> <span data-ttu-id="3efcd-179">Diese Sammlung darf maximal 7 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="3efcd-179">This collection can contain a maximum of 7 elements.</span></span> <span data-ttu-id="3efcd-180">Mögliche Werte sind: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday` und `saturday`.</span><span class="sxs-lookup"><span data-stu-id="3efcd-180">Possible values are: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="3efcd-181">utcTimeOffsetInMinutes</span><span class="sxs-lookup"><span data-stu-id="3efcd-181">utcTimeOffsetInMinutes</span></span>|<span data-ttu-id="3efcd-182">Int32</span><span class="sxs-lookup"><span data-stu-id="3efcd-182">Int32</span></span>|<span data-ttu-id="3efcd-183">UTC-Zeitversatz in Minuten</span><span class="sxs-lookup"><span data-stu-id="3efcd-183">UTC Time Offset indicated in minutes</span></span>|
|<span data-ttu-id="3efcd-184">enforcedSoftwareUpdateDelayInDays</span><span class="sxs-lookup"><span data-stu-id="3efcd-184">enforcedSoftwareUpdateDelayInDays</span></span>|<span data-ttu-id="3efcd-185">Int32</span><span class="sxs-lookup"><span data-stu-id="3efcd-185">Int32</span></span>|<span data-ttu-id="3efcd-186">Tage vor dem Anzeigen von Softwareupdates für iOS-Geräte von 0 bis einschließlich 90</span><span class="sxs-lookup"><span data-stu-id="3efcd-186">Days before software updates are visible to iOS devices ranging from 0 to 90 inclusive</span></span>|



## <a name="response"></a><span data-ttu-id="3efcd-187">Antwort</span><span class="sxs-lookup"><span data-stu-id="3efcd-187">Response</span></span>
<span data-ttu-id="3efcd-188">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="3efcd-188">If successful, this method returns a `200 OK` response code and an updated [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3efcd-189">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3efcd-189">Example</span></span>

### <a name="request"></a><span data-ttu-id="3efcd-190">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3efcd-190">Request</span></span>
<span data-ttu-id="3efcd-191">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3efcd-191">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 482

{
  "@odata.type": "#microsoft.graph.iosUpdateConfiguration",
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

### <a name="response"></a><span data-ttu-id="3efcd-192">Antwort</span><span class="sxs-lookup"><span data-stu-id="3efcd-192">Response</span></span>
<span data-ttu-id="3efcd-p111">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3efcd-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




