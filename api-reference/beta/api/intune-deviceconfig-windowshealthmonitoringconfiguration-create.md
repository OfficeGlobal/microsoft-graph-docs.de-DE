---
title: WindowsHealthMonitoringConfiguration erstellen
description: Erstellen eines neuen windowsHealthMonitoringConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 75ace30116ddf2515f99f8bcdd6a2c9c19f45b58
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30972928"
---
# <a name="create-windowshealthmonitoringconfiguration"></a><span data-ttu-id="da3b2-103">WindowsHealthMonitoringConfiguration erstellen</span><span class="sxs-lookup"><span data-stu-id="da3b2-103">Create windowsHealthMonitoringConfiguration</span></span>

> <span data-ttu-id="da3b2-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="da3b2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="da3b2-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="da3b2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="da3b2-106">Erstellen eines neuen [windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="da3b2-106">Create a new [windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="da3b2-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="da3b2-107">Prerequisites</span></span>
<span data-ttu-id="da3b2-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="da3b2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="da3b2-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="da3b2-110">Permission type</span></span>|<span data-ttu-id="da3b2-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="da3b2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="da3b2-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="da3b2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="da3b2-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da3b2-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="da3b2-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="da3b2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="da3b2-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="da3b2-115">Not supported.</span></span>|
|<span data-ttu-id="da3b2-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="da3b2-116">Application</span></span>|<span data-ttu-id="da3b2-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="da3b2-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="da3b2-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="da3b2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="da3b2-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="da3b2-119">Request headers</span></span>
|<span data-ttu-id="da3b2-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="da3b2-120">Header</span></span>|<span data-ttu-id="da3b2-121">Wert</span><span class="sxs-lookup"><span data-stu-id="da3b2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="da3b2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="da3b2-122">Authorization</span></span>|<span data-ttu-id="da3b2-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="da3b2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="da3b2-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="da3b2-124">Accept</span></span>|<span data-ttu-id="da3b2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="da3b2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="da3b2-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="da3b2-126">Request body</span></span>
<span data-ttu-id="da3b2-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das windowsHealthMonitoringConfiguration-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="da3b2-127">In the request body, supply a JSON representation for the windowsHealthMonitoringConfiguration object.</span></span>

<span data-ttu-id="da3b2-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der windowsHealthMonitoringConfiguration erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="da3b2-128">The following table shows the properties that are required when you create the windowsHealthMonitoringConfiguration.</span></span>

|<span data-ttu-id="da3b2-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="da3b2-129">Property</span></span>|<span data-ttu-id="da3b2-130">Typ</span><span class="sxs-lookup"><span data-stu-id="da3b2-130">Type</span></span>|<span data-ttu-id="da3b2-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="da3b2-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="da3b2-132">id</span><span class="sxs-lookup"><span data-stu-id="da3b2-132">id</span></span>|<span data-ttu-id="da3b2-133">String</span><span class="sxs-lookup"><span data-stu-id="da3b2-133">String</span></span>|<span data-ttu-id="da3b2-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="da3b2-134">Key of the entity.</span></span> <span data-ttu-id="da3b2-135">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="da3b2-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="da3b2-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="da3b2-136">lastModifiedDateTime</span></span>|<span data-ttu-id="da3b2-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="da3b2-137">DateTimeOffset</span></span>|<span data-ttu-id="da3b2-138">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="da3b2-138">DateTime the object was last modified.</span></span> <span data-ttu-id="da3b2-139">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="da3b2-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="da3b2-140">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="da3b2-140">roleScopeTagIds</span></span>|<span data-ttu-id="da3b2-141">String collection</span><span class="sxs-lookup"><span data-stu-id="da3b2-141">String collection</span></span>|<span data-ttu-id="da3b2-142">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="da3b2-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="da3b2-143">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="da3b2-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="da3b2-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="da3b2-144">supportsScopeTags</span></span>|<span data-ttu-id="da3b2-145">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="da3b2-145">Boolean</span></span>|<span data-ttu-id="da3b2-146">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereichs Tags unterstützt.</span><span class="sxs-lookup"><span data-stu-id="da3b2-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="da3b2-147">Das Zuweisen zur ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert auf false festgelegt ist und Entitäten für bereichsbezogene Benutzer nicht sichtbar sind.</span><span class="sxs-lookup"><span data-stu-id="da3b2-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="da3b2-148">Dies geschieht für in Silverlight erstellte Legacy Richtlinien und kann durch Löschen und erneutes Erstellen der Richtlinie im Azure-Portal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="da3b2-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="da3b2-149">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="da3b2-149">This property is read-only.</span></span> <span data-ttu-id="da3b2-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="da3b2-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="da3b2-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="da3b2-151">createdDateTime</span></span>|<span data-ttu-id="da3b2-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="da3b2-152">DateTimeOffset</span></span>|<span data-ttu-id="da3b2-153">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="da3b2-153">DateTime the object was created.</span></span> <span data-ttu-id="da3b2-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="da3b2-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="da3b2-155">description</span><span class="sxs-lookup"><span data-stu-id="da3b2-155">description</span></span>|<span data-ttu-id="da3b2-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="da3b2-156">String</span></span>|<span data-ttu-id="da3b2-157">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="da3b2-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="da3b2-158">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="da3b2-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="da3b2-159">displayName</span><span class="sxs-lookup"><span data-stu-id="da3b2-159">displayName</span></span>|<span data-ttu-id="da3b2-160">String</span><span class="sxs-lookup"><span data-stu-id="da3b2-160">String</span></span>|<span data-ttu-id="da3b2-161">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="da3b2-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="da3b2-162">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="da3b2-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="da3b2-163">Version</span><span class="sxs-lookup"><span data-stu-id="da3b2-163">version</span></span>|<span data-ttu-id="da3b2-164">Int32</span><span class="sxs-lookup"><span data-stu-id="da3b2-164">Int32</span></span>|<span data-ttu-id="da3b2-165">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="da3b2-165">Version of the device configuration.</span></span> <span data-ttu-id="da3b2-166">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="da3b2-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="da3b2-167">allowDeviceHealthMonitoring</span><span class="sxs-lookup"><span data-stu-id="da3b2-167">allowDeviceHealthMonitoring</span></span>|[<span data-ttu-id="da3b2-168">Aktivierung</span><span class="sxs-lookup"><span data-stu-id="da3b2-168">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="da3b2-169">Aktiviert die Gerätestatus Überwachung auf dem Gerät.</span><span class="sxs-lookup"><span data-stu-id="da3b2-169">Enables device health monitoring on the device.</span></span> <span data-ttu-id="da3b2-170">Mögliche Werte sind: `notConfigured`, `enabled` und `disabled`.</span><span class="sxs-lookup"><span data-stu-id="da3b2-170">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="da3b2-171">configDeviceHealthMonitoringScope</span><span class="sxs-lookup"><span data-stu-id="da3b2-171">configDeviceHealthMonitoringScope</span></span>|[<span data-ttu-id="da3b2-172">windowsHealthMonitoringScope</span><span class="sxs-lookup"><span data-stu-id="da3b2-172">windowsHealthMonitoringScope</span></span>](../resources/intune-deviceconfig-windowshealthmonitoringscope.md)|<span data-ttu-id="da3b2-173">Gibt-Satz von Ereignissen, die von dem Gerät erfasst werden, auf dem die Integritätsüberwachung aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="da3b2-173">Sepcifies set of events collected from the device where health monitoring is enabled.</span></span> <span data-ttu-id="da3b2-174">Mögliche Werte sind: `undefined`, `healthMonitoring` und `bootPerformance`.</span><span class="sxs-lookup"><span data-stu-id="da3b2-174">Possible values are: `undefined`, `healthMonitoring`, `bootPerformance`.</span></span>|



## <a name="response"></a><span data-ttu-id="da3b2-175">Antwort</span><span class="sxs-lookup"><span data-stu-id="da3b2-175">Response</span></span>
<span data-ttu-id="da3b2-176">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="da3b2-176">If successful, this method returns a `201 Created` response code and a [windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="da3b2-177">Beispiel</span><span class="sxs-lookup"><span data-stu-id="da3b2-177">Example</span></span>

### <a name="request"></a><span data-ttu-id="da3b2-178">Anforderung</span><span class="sxs-lookup"><span data-stu-id="da3b2-178">Request</span></span>
<span data-ttu-id="da3b2-179">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="da3b2-179">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="da3b2-180">Antwort</span><span class="sxs-lookup"><span data-stu-id="da3b2-180">Response</span></span>
<span data-ttu-id="da3b2-p112">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="da3b2-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




