---
title: WindowsHealthMonitoringConfiguration aktualisieren
description: Aktualisieren der Eigenschaften eines windowsHealthMonitoringConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0337ebb95f0ba17aab6a7a3171765c0b5b85a1b2
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30978766"
---
# <a name="update-windowshealthmonitoringconfiguration"></a><span data-ttu-id="58129-103">WindowsHealthMonitoringConfiguration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="58129-103">Update windowsHealthMonitoringConfiguration</span></span>

> <span data-ttu-id="58129-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="58129-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="58129-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="58129-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="58129-106">Aktualisieren der Eigenschaften eines [windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="58129-106">Update the properties of a [windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="58129-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="58129-107">Prerequisites</span></span>
<span data-ttu-id="58129-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="58129-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="58129-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="58129-110">Permission type</span></span>|<span data-ttu-id="58129-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="58129-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="58129-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="58129-112">Delegated (work or school account)</span></span>|<span data-ttu-id="58129-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58129-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="58129-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="58129-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="58129-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="58129-115">Not supported.</span></span>|
|<span data-ttu-id="58129-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="58129-116">Application</span></span>|<span data-ttu-id="58129-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="58129-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="58129-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="58129-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="58129-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="58129-119">Request headers</span></span>
|<span data-ttu-id="58129-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="58129-120">Header</span></span>|<span data-ttu-id="58129-121">Wert</span><span class="sxs-lookup"><span data-stu-id="58129-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="58129-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="58129-122">Authorization</span></span>|<span data-ttu-id="58129-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="58129-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="58129-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="58129-124">Accept</span></span>|<span data-ttu-id="58129-125">application/json</span><span class="sxs-lookup"><span data-stu-id="58129-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="58129-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="58129-126">Request body</span></span>
<span data-ttu-id="58129-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="58129-127">In the request body, supply a JSON representation for the [windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md) object.</span></span>

<span data-ttu-id="58129-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="58129-128">The following table shows the properties that are required when you create the [windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md).</span></span>

|<span data-ttu-id="58129-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="58129-129">Property</span></span>|<span data-ttu-id="58129-130">Typ</span><span class="sxs-lookup"><span data-stu-id="58129-130">Type</span></span>|<span data-ttu-id="58129-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="58129-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="58129-132">id</span><span class="sxs-lookup"><span data-stu-id="58129-132">id</span></span>|<span data-ttu-id="58129-133">String</span><span class="sxs-lookup"><span data-stu-id="58129-133">String</span></span>|<span data-ttu-id="58129-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="58129-134">Key of the entity.</span></span> <span data-ttu-id="58129-135">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="58129-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="58129-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="58129-136">lastModifiedDateTime</span></span>|<span data-ttu-id="58129-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="58129-137">DateTimeOffset</span></span>|<span data-ttu-id="58129-138">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="58129-138">DateTime the object was last modified.</span></span> <span data-ttu-id="58129-139">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="58129-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="58129-140">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="58129-140">roleScopeTagIds</span></span>|<span data-ttu-id="58129-141">String collection</span><span class="sxs-lookup"><span data-stu-id="58129-141">String collection</span></span>|<span data-ttu-id="58129-142">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="58129-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="58129-143">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="58129-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="58129-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="58129-144">supportsScopeTags</span></span>|<span data-ttu-id="58129-145">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="58129-145">Boolean</span></span>|<span data-ttu-id="58129-146">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereichs Tags unterstützt.</span><span class="sxs-lookup"><span data-stu-id="58129-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="58129-147">Das Zuweisen zur ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert auf false festgelegt ist und Entitäten für bereichsbezogene Benutzer nicht sichtbar sind.</span><span class="sxs-lookup"><span data-stu-id="58129-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="58129-148">Dies geschieht für in Silverlight erstellte Legacy Richtlinien und kann durch Löschen und erneutes Erstellen der Richtlinie im Azure-Portal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="58129-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="58129-149">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="58129-149">This property is read-only.</span></span> <span data-ttu-id="58129-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="58129-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="58129-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="58129-151">createdDateTime</span></span>|<span data-ttu-id="58129-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="58129-152">DateTimeOffset</span></span>|<span data-ttu-id="58129-153">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="58129-153">DateTime the object was created.</span></span> <span data-ttu-id="58129-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="58129-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="58129-155">description</span><span class="sxs-lookup"><span data-stu-id="58129-155">description</span></span>|<span data-ttu-id="58129-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="58129-156">String</span></span>|<span data-ttu-id="58129-157">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="58129-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="58129-158">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="58129-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="58129-159">displayName</span><span class="sxs-lookup"><span data-stu-id="58129-159">displayName</span></span>|<span data-ttu-id="58129-160">String</span><span class="sxs-lookup"><span data-stu-id="58129-160">String</span></span>|<span data-ttu-id="58129-161">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="58129-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="58129-162">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="58129-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="58129-163">Version</span><span class="sxs-lookup"><span data-stu-id="58129-163">version</span></span>|<span data-ttu-id="58129-164">Int32</span><span class="sxs-lookup"><span data-stu-id="58129-164">Int32</span></span>|<span data-ttu-id="58129-165">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="58129-165">Version of the device configuration.</span></span> <span data-ttu-id="58129-166">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="58129-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="58129-167">allowDeviceHealthMonitoring</span><span class="sxs-lookup"><span data-stu-id="58129-167">allowDeviceHealthMonitoring</span></span>|[<span data-ttu-id="58129-168">Aktivierung</span><span class="sxs-lookup"><span data-stu-id="58129-168">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="58129-169">Aktiviert die Gerätestatus Überwachung auf dem Gerät.</span><span class="sxs-lookup"><span data-stu-id="58129-169">Enables device health monitoring on the device.</span></span> <span data-ttu-id="58129-170">Mögliche Werte sind: `notConfigured`, `enabled` und `disabled`.</span><span class="sxs-lookup"><span data-stu-id="58129-170">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="58129-171">configDeviceHealthMonitoringScope</span><span class="sxs-lookup"><span data-stu-id="58129-171">configDeviceHealthMonitoringScope</span></span>|[<span data-ttu-id="58129-172">windowsHealthMonitoringScope</span><span class="sxs-lookup"><span data-stu-id="58129-172">windowsHealthMonitoringScope</span></span>](../resources/intune-deviceconfig-windowshealthmonitoringscope.md)|<span data-ttu-id="58129-173">Gibt-Satz von Ereignissen, die von dem Gerät erfasst werden, auf dem die Integritätsüberwachung aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="58129-173">Sepcifies set of events collected from the device where health monitoring is enabled.</span></span> <span data-ttu-id="58129-174">Mögliche Werte sind: `undefined`, `healthMonitoring` und `bootPerformance`.</span><span class="sxs-lookup"><span data-stu-id="58129-174">Possible values are: `undefined`, `healthMonitoring`, `bootPerformance`.</span></span>|



## <a name="response"></a><span data-ttu-id="58129-175">Antwort</span><span class="sxs-lookup"><span data-stu-id="58129-175">Response</span></span>
<span data-ttu-id="58129-176">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="58129-176">If successful, this method returns a `200 OK` response code and an updated [windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="58129-177">Beispiel</span><span class="sxs-lookup"><span data-stu-id="58129-177">Example</span></span>

### <a name="request"></a><span data-ttu-id="58129-178">Anforderung</span><span class="sxs-lookup"><span data-stu-id="58129-178">Request</span></span>
<span data-ttu-id="58129-179">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="58129-179">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="58129-180">Antwort</span><span class="sxs-lookup"><span data-stu-id="58129-180">Response</span></span>
<span data-ttu-id="58129-p112">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="58129-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




