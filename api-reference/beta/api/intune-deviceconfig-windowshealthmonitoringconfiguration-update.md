---
title: WindowsHealthMonitoringConfiguration aktualisieren
description: Aktualisieren der Eigenschaften eines windowsHealthMonitoringConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d19801400b75cfb712e5249d53938012bdb9b1d8
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/14/2019
ms.locfileid: "30631555"
---
# <a name="update-windowshealthmonitoringconfiguration"></a><span data-ttu-id="e2ce5-103">WindowsHealthMonitoringConfiguration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="e2ce5-103">Update windowsHealthMonitoringConfiguration</span></span>

> <span data-ttu-id="e2ce5-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e2ce5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e2ce5-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="e2ce5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e2ce5-106">Aktualisieren der Eigenschaften eines [windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="e2ce5-106">Update the properties of a [windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e2ce5-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="e2ce5-107">Prerequisites</span></span>
<span data-ttu-id="e2ce5-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="e2ce5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="e2ce5-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e2ce5-110">Permission type</span></span>|<span data-ttu-id="e2ce5-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e2ce5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e2ce5-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e2ce5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e2ce5-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2ce5-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e2ce5-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e2ce5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e2ce5-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e2ce5-115">Not supported.</span></span>|
|<span data-ttu-id="e2ce5-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e2ce5-116">Application</span></span>|<span data-ttu-id="e2ce5-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e2ce5-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e2ce5-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e2ce5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="e2ce5-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e2ce5-119">Request headers</span></span>
|<span data-ttu-id="e2ce5-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="e2ce5-120">Header</span></span>|<span data-ttu-id="e2ce5-121">Wert</span><span class="sxs-lookup"><span data-stu-id="e2ce5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e2ce5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e2ce5-122">Authorization</span></span>|<span data-ttu-id="e2ce5-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="e2ce5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e2ce5-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="e2ce5-124">Accept</span></span>|<span data-ttu-id="e2ce5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e2ce5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e2ce5-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e2ce5-126">Request body</span></span>
<span data-ttu-id="e2ce5-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="e2ce5-127">In the request body, supply a JSON representation for the [windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md) object.</span></span>

<span data-ttu-id="e2ce5-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="e2ce5-128">The following table shows the properties that are required when you create the [windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md).</span></span>

|<span data-ttu-id="e2ce5-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e2ce5-129">Property</span></span>|<span data-ttu-id="e2ce5-130">Typ</span><span class="sxs-lookup"><span data-stu-id="e2ce5-130">Type</span></span>|<span data-ttu-id="e2ce5-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e2ce5-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e2ce5-132">id</span><span class="sxs-lookup"><span data-stu-id="e2ce5-132">id</span></span>|<span data-ttu-id="e2ce5-133">String</span><span class="sxs-lookup"><span data-stu-id="e2ce5-133">String</span></span>|<span data-ttu-id="e2ce5-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="e2ce5-134">Key of the entity.</span></span> <span data-ttu-id="e2ce5-135">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e2ce5-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e2ce5-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e2ce5-136">lastModifiedDateTime</span></span>|<span data-ttu-id="e2ce5-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e2ce5-137">DateTimeOffset</span></span>|<span data-ttu-id="e2ce5-138">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="e2ce5-138">DateTime the object was last modified.</span></span> <span data-ttu-id="e2ce5-139">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e2ce5-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e2ce5-140">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="e2ce5-140">roleScopeTagIds</span></span>|<span data-ttu-id="e2ce5-141">String collection</span><span class="sxs-lookup"><span data-stu-id="e2ce5-141">String collection</span></span>|<span data-ttu-id="e2ce5-142">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="e2ce5-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="e2ce5-143">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e2ce5-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e2ce5-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="e2ce5-144">supportsScopeTags</span></span>|<span data-ttu-id="e2ce5-145">Boolesch</span><span class="sxs-lookup"><span data-stu-id="e2ce5-145">Boolean</span></span>|<span data-ttu-id="e2ce5-146">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereichs Tags unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e2ce5-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="e2ce5-147">Das Zuweisen zur ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert auf false festgelegt ist und Entitäten für bereichsbezogene Benutzer nicht sichtbar sind.</span><span class="sxs-lookup"><span data-stu-id="e2ce5-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="e2ce5-148">Dies geschieht für in Silverlight erstellte Legacy Richtlinien und kann durch Löschen und erneutes Erstellen der Richtlinie im Azure-Portal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="e2ce5-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="e2ce5-149">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="e2ce5-149">This property is read-only.</span></span> <span data-ttu-id="e2ce5-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e2ce5-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e2ce5-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e2ce5-151">createdDateTime</span></span>|<span data-ttu-id="e2ce5-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e2ce5-152">DateTimeOffset</span></span>|<span data-ttu-id="e2ce5-153">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="e2ce5-153">DateTime the object was created.</span></span> <span data-ttu-id="e2ce5-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e2ce5-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e2ce5-155">description</span><span class="sxs-lookup"><span data-stu-id="e2ce5-155">description</span></span>|<span data-ttu-id="e2ce5-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e2ce5-156">String</span></span>|<span data-ttu-id="e2ce5-157">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="e2ce5-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e2ce5-158">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e2ce5-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e2ce5-159">displayName</span><span class="sxs-lookup"><span data-stu-id="e2ce5-159">displayName</span></span>|<span data-ttu-id="e2ce5-160">String</span><span class="sxs-lookup"><span data-stu-id="e2ce5-160">String</span></span>|<span data-ttu-id="e2ce5-161">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="e2ce5-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e2ce5-162">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e2ce5-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e2ce5-163">Version</span><span class="sxs-lookup"><span data-stu-id="e2ce5-163">version</span></span>|<span data-ttu-id="e2ce5-164">Int32</span><span class="sxs-lookup"><span data-stu-id="e2ce5-164">Int32</span></span>|<span data-ttu-id="e2ce5-165">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="e2ce5-165">Version of the device configuration.</span></span> <span data-ttu-id="e2ce5-166">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e2ce5-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e2ce5-167">allowDeviceHealthMonitoring</span><span class="sxs-lookup"><span data-stu-id="e2ce5-167">allowDeviceHealthMonitoring</span></span>|[<span data-ttu-id="e2ce5-168">Aktivierung</span><span class="sxs-lookup"><span data-stu-id="e2ce5-168">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="e2ce5-169">Aktiviert die Gerätestatus Überwachung auf dem Gerät.</span><span class="sxs-lookup"><span data-stu-id="e2ce5-169">Enables device health monitoring on the device.</span></span> <span data-ttu-id="e2ce5-170">Mögliche Werte sind: `notConfigured`, `enabled` und `disabled`.</span><span class="sxs-lookup"><span data-stu-id="e2ce5-170">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="e2ce5-171">configDeviceHealthMonitoringScope</span><span class="sxs-lookup"><span data-stu-id="e2ce5-171">configDeviceHealthMonitoringScope</span></span>|[<span data-ttu-id="e2ce5-172">windowsHealthMonitoringScope</span><span class="sxs-lookup"><span data-stu-id="e2ce5-172">windowsHealthMonitoringScope</span></span>](../resources/intune-deviceconfig-windowshealthmonitoringscope.md)|<span data-ttu-id="e2ce5-173">Gibt-Satz von Ereignissen, die von dem Gerät erfasst werden, auf dem die Integritätsüberwachung aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="e2ce5-173">Sepcifies set of events collected from the device where health monitoring is enabled.</span></span> <span data-ttu-id="e2ce5-174">Mögliche Werte sind: `undefined`, `healthMonitoring` und `bootPerformance`.</span><span class="sxs-lookup"><span data-stu-id="e2ce5-174">Possible values are: `undefined`, `healthMonitoring`, `bootPerformance`.</span></span>|



## <a name="response"></a><span data-ttu-id="e2ce5-175">Antwort</span><span class="sxs-lookup"><span data-stu-id="e2ce5-175">Response</span></span>
<span data-ttu-id="e2ce5-176">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="e2ce5-176">If successful, this method returns a `200 OK` response code and an updated [windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e2ce5-177">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e2ce5-177">Example</span></span>

### <a name="request"></a><span data-ttu-id="e2ce5-178">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e2ce5-178">Request</span></span>
<span data-ttu-id="e2ce5-179">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e2ce5-179">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 371

{
  "@odata.type": "#microsoft.graph.windowsHealthMonitoringConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "allowDeviceHealthMonitoring": "enabled",
  "configDeviceHealthMonitoringScope": "healthMonitoring"
}
```

### <a name="response"></a><span data-ttu-id="e2ce5-180">Antwort</span><span class="sxs-lookup"><span data-stu-id="e2ce5-180">Response</span></span>
<span data-ttu-id="e2ce5-p112">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e2ce5-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 543

{
  "@odata.type": "#microsoft.graph.windowsHealthMonitoringConfiguration",
  "id": "3439bcec-bcec-3439-ecbc-3934ecbc3934",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "allowDeviceHealthMonitoring": "enabled",
  "configDeviceHealthMonitoringScope": "healthMonitoring"
}
```




