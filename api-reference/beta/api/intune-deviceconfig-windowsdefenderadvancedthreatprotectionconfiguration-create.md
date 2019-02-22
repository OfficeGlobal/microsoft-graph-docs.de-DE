---
title: Erstellen von „windowsDefenderAdvancedThreatProtectionConfiguration“
description: Diese Methode erstellt ein neues Objekt des Typs windowsDefenderAdvancedThreatProtectionConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 973d6a3cd6386815b89fe4b6d8767f9611de20a5
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30146228"
---
# <a name="create-windowsdefenderadvancedthreatprotectionconfiguration"></a><span data-ttu-id="08861-103">Erstellen von „windowsDefenderAdvancedThreatProtectionConfiguration“</span><span class="sxs-lookup"><span data-stu-id="08861-103">Create windowsDefenderAdvancedThreatProtectionConfiguration</span></span>

> <span data-ttu-id="08861-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="08861-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="08861-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="08861-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="08861-106">Diese Methode erstellt ein neues Objekt des Typs [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="08861-106">Create a new [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="08861-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="08861-107">Prerequisites</span></span>
<span data-ttu-id="08861-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="08861-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="08861-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="08861-110">Permission type</span></span>|<span data-ttu-id="08861-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="08861-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="08861-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="08861-112">Delegated (work or school account)</span></span>|<span data-ttu-id="08861-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08861-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="08861-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="08861-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="08861-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="08861-115">Not supported.</span></span>|
|<span data-ttu-id="08861-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="08861-116">Application</span></span>|<span data-ttu-id="08861-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="08861-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="08861-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="08861-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="08861-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="08861-119">Request headers</span></span>
|<span data-ttu-id="08861-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="08861-120">Header</span></span>|<span data-ttu-id="08861-121">Wert</span><span class="sxs-lookup"><span data-stu-id="08861-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="08861-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="08861-122">Authorization</span></span>|<span data-ttu-id="08861-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="08861-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="08861-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="08861-124">Accept</span></span>|<span data-ttu-id="08861-125">application/json</span><span class="sxs-lookup"><span data-stu-id="08861-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="08861-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="08861-126">Request body</span></span>
<span data-ttu-id="08861-127">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „windowsDefenderAdvancedThreatProtectionConfiguration“ an.</span><span class="sxs-lookup"><span data-stu-id="08861-127">In the request body, supply a JSON representation for the windowsDefenderAdvancedThreatProtectionConfiguration object.</span></span>

<span data-ttu-id="08861-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „windowsDefenderAdvancedThreatProtectionConfiguration“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="08861-128">The following table shows the properties that are required when you create the windowsDefenderAdvancedThreatProtectionConfiguration.</span></span>

|<span data-ttu-id="08861-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="08861-129">Property</span></span>|<span data-ttu-id="08861-130">Typ</span><span class="sxs-lookup"><span data-stu-id="08861-130">Type</span></span>|<span data-ttu-id="08861-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="08861-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="08861-132">id</span><span class="sxs-lookup"><span data-stu-id="08861-132">id</span></span>|<span data-ttu-id="08861-133">string</span><span class="sxs-lookup"><span data-stu-id="08861-133">String</span></span>|<span data-ttu-id="08861-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="08861-134">Key of the entity.</span></span> <span data-ttu-id="08861-135">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="08861-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="08861-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="08861-136">lastModifiedDateTime</span></span>|<span data-ttu-id="08861-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="08861-137">DateTimeOffset</span></span>|<span data-ttu-id="08861-138">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="08861-138">DateTime the object was last modified.</span></span> <span data-ttu-id="08861-139">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="08861-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="08861-140">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="08861-140">roleScopeTagIds</span></span>|<span data-ttu-id="08861-141">String collection</span><span class="sxs-lookup"><span data-stu-id="08861-141">String collection</span></span>|<span data-ttu-id="08861-142">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="08861-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="08861-143">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="08861-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="08861-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="08861-144">supportsScopeTags</span></span>|<span data-ttu-id="08861-145">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="08861-145">Boolean</span></span>|<span data-ttu-id="08861-146">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereichs Tags unterstützt.</span><span class="sxs-lookup"><span data-stu-id="08861-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="08861-147">Das Zuweisen zur ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert auf false festgelegt ist und Entitäten für bereichsbezogene Benutzer nicht sichtbar sind.</span><span class="sxs-lookup"><span data-stu-id="08861-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="08861-148">Dies geschieht für in Silverlight erstellte Legacy Richtlinien und kann durch Löschen und erneutes Erstellen der Richtlinie im Azure-Portal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="08861-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="08861-149">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="08861-149">This property is read-only.</span></span> <span data-ttu-id="08861-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="08861-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="08861-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="08861-151">createdDateTime</span></span>|<span data-ttu-id="08861-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="08861-152">DateTimeOffset</span></span>|<span data-ttu-id="08861-153">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="08861-153">DateTime the object was created.</span></span> <span data-ttu-id="08861-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="08861-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="08861-155">description</span><span class="sxs-lookup"><span data-stu-id="08861-155">description</span></span>|<span data-ttu-id="08861-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="08861-156">String</span></span>|<span data-ttu-id="08861-157">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="08861-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="08861-158">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="08861-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="08861-159">displayName</span><span class="sxs-lookup"><span data-stu-id="08861-159">displayName</span></span>|<span data-ttu-id="08861-160">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="08861-160">String</span></span>|<span data-ttu-id="08861-161">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="08861-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="08861-162">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="08861-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="08861-163">Version</span><span class="sxs-lookup"><span data-stu-id="08861-163">version</span></span>|<span data-ttu-id="08861-164">Int32</span><span class="sxs-lookup"><span data-stu-id="08861-164">Int32</span></span>|<span data-ttu-id="08861-165">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="08861-165">Version of the device configuration.</span></span> <span data-ttu-id="08861-166">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="08861-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="08861-167">advancedThreatProtectionOnboardingBlob</span><span class="sxs-lookup"><span data-stu-id="08861-167">advancedThreatProtectionOnboardingBlob</span></span>|<span data-ttu-id="08861-168">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="08861-168">String</span></span>|<span data-ttu-id="08861-169">Windows Defender Advanced Threat Protection Onboarding-BLOB.</span><span class="sxs-lookup"><span data-stu-id="08861-169">Windows Defender AdvancedThreatProtection Onboarding Blob.</span></span>|
|<span data-ttu-id="08861-170">advancedThreatProtectionOnboardingFilename</span><span class="sxs-lookup"><span data-stu-id="08861-170">advancedThreatProtectionOnboardingFilename</span></span>|<span data-ttu-id="08861-171">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="08861-171">String</span></span>|<span data-ttu-id="08861-172">Name der Datei, aus der AdvancedThreatProtectionOnboardingBlob abgerufen wurde.</span><span class="sxs-lookup"><span data-stu-id="08861-172">Name of the file from which AdvancedThreatProtectionOnboardingBlob was obtained.</span></span>|
|<span data-ttu-id="08861-173">advancedThreatProtectionAutoPopulateOnboardingBlob</span><span class="sxs-lookup"><span data-stu-id="08861-173">advancedThreatProtectionAutoPopulateOnboardingBlob</span></span>|<span data-ttu-id="08861-174">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="08861-174">Boolean</span></span>|<span data-ttu-id="08861-175">Automatisches Auffüllen des Onboarding-BLOBs programmgesteuert von Advanced Threat Protection Service</span><span class="sxs-lookup"><span data-stu-id="08861-175">Auto populate onboarding blob programmatically from Advanced Threat protection service</span></span>|
|<span data-ttu-id="08861-176">allowSampleSharing</span><span class="sxs-lookup"><span data-stu-id="08861-176">allowSampleSharing</span></span>|<span data-ttu-id="08861-177">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="08861-177">Boolean</span></span>|<span data-ttu-id="08861-178">Regel „Beispielfreigabe zulassen“ in Windows Defender Advanced Threat Protection</span><span class="sxs-lookup"><span data-stu-id="08861-178">Windows Defender AdvancedThreatProtection "Allow Sample Sharing" Rule</span></span>|
|<span data-ttu-id="08861-179">enableExpeditedTelemetryReporting</span><span class="sxs-lookup"><span data-stu-id="08861-179">enableExpeditedTelemetryReporting</span></span>|<span data-ttu-id="08861-180">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="08861-180">Boolean</span></span>|<span data-ttu-id="08861-181">Verkürzt das Meldungsintervall für Windows Defender Advanced Threat Protection-Telemetriedaten.</span><span class="sxs-lookup"><span data-stu-id="08861-181">Expedite Windows Defender Advanced Threat Protection telemetry reporting frequency.</span></span>|
|<span data-ttu-id="08861-182">advancedThreatProtectionOffboardingBlob</span><span class="sxs-lookup"><span data-stu-id="08861-182">advancedThreatProtectionOffboardingBlob</span></span>|<span data-ttu-id="08861-183">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="08861-183">String</span></span>|<span data-ttu-id="08861-184">Windows Defender Advanced Threat Protection Offboarding-BLOB.</span><span class="sxs-lookup"><span data-stu-id="08861-184">Windows Defender AdvancedThreatProtection Offboarding Blob.</span></span>|
|<span data-ttu-id="08861-185">advancedThreatProtectionOffboardingFilename</span><span class="sxs-lookup"><span data-stu-id="08861-185">advancedThreatProtectionOffboardingFilename</span></span>|<span data-ttu-id="08861-186">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="08861-186">String</span></span>|<span data-ttu-id="08861-187">Name der Datei, aus der AdvancedThreatProtectionOffboardingBlob abgerufen wurde.</span><span class="sxs-lookup"><span data-stu-id="08861-187">Name of the file from which AdvancedThreatProtectionOffboardingBlob was obtained.</span></span>|



## <a name="response"></a><span data-ttu-id="08861-188">Antwort</span><span class="sxs-lookup"><span data-stu-id="08861-188">Response</span></span>
<span data-ttu-id="08861-189">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="08861-189">If successful, this method returns a `201 Created` response code and a [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="08861-190">Beispiel</span><span class="sxs-lookup"><span data-stu-id="08861-190">Example</span></span>

### <a name="request"></a><span data-ttu-id="08861-191">Anforderung</span><span class="sxs-lookup"><span data-stu-id="08861-191">Request</span></span>
<span data-ttu-id="08861-192">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="08861-192">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 830

{
  "@odata.type": "#microsoft.graph.windowsDefenderAdvancedThreatProtectionConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "advancedThreatProtectionOnboardingBlob": "Advanced Threat Protection Onboarding Blob value",
  "advancedThreatProtectionOnboardingFilename": "Advanced Threat Protection Onboarding Filename value",
  "advancedThreatProtectionAutoPopulateOnboardingBlob": true,
  "allowSampleSharing": true,
  "enableExpeditedTelemetryReporting": true,
  "advancedThreatProtectionOffboardingBlob": "Advanced Threat Protection Offboarding Blob value",
  "advancedThreatProtectionOffboardingFilename": "Advanced Threat Protection Offboarding Filename value"
}
```

### <a name="response"></a><span data-ttu-id="08861-193">Antwort</span><span class="sxs-lookup"><span data-stu-id="08861-193">Response</span></span>
<span data-ttu-id="08861-p110">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="08861-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1002

{
  "@odata.type": "#microsoft.graph.windowsDefenderAdvancedThreatProtectionConfiguration",
  "id": "294373aa-73aa-2943-aa73-4329aa734329",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "advancedThreatProtectionOnboardingBlob": "Advanced Threat Protection Onboarding Blob value",
  "advancedThreatProtectionOnboardingFilename": "Advanced Threat Protection Onboarding Filename value",
  "advancedThreatProtectionAutoPopulateOnboardingBlob": true,
  "allowSampleSharing": true,
  "enableExpeditedTelemetryReporting": true,
  "advancedThreatProtectionOffboardingBlob": "Advanced Threat Protection Offboarding Blob value",
  "advancedThreatProtectionOffboardingFilename": "Advanced Threat Protection Offboarding Filename value"
}
```




