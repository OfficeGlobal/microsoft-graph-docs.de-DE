---
title: Aktualisieren von „windowsDefenderAdvancedThreatProtectionConfiguration“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs windowsDefenderAdvancedThreatProtectionConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: fea7f12f3ea6e90aaeea38d828dbe072b2995430
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396371"
---
# <a name="update-windowsdefenderadvancedthreatprotectionconfiguration"></a><span data-ttu-id="9ac6b-103">Aktualisieren von „windowsDefenderAdvancedThreatProtectionConfiguration“</span><span class="sxs-lookup"><span data-stu-id="9ac6b-103">Update windowsDefenderAdvancedThreatProtectionConfiguration</span></span>

> <span data-ttu-id="9ac6b-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="9ac6b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="9ac6b-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9ac6b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9ac6b-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9ac6b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9ac6b-107">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9ac6b-107">Update the properties of a [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9ac6b-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="9ac6b-108">Prerequisites</span></span>
<span data-ttu-id="9ac6b-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="9ac6b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="9ac6b-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9ac6b-111">Permission type</span></span>|<span data-ttu-id="9ac6b-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9ac6b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9ac6b-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9ac6b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9ac6b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ac6b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9ac6b-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9ac6b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9ac6b-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9ac6b-116">Not supported.</span></span>|
|<span data-ttu-id="9ac6b-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9ac6b-117">Application</span></span>|<span data-ttu-id="9ac6b-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9ac6b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9ac6b-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9ac6b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="9ac6b-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9ac6b-120">Request headers</span></span>
|<span data-ttu-id="9ac6b-121">Header</span><span class="sxs-lookup"><span data-stu-id="9ac6b-121">Header</span></span>|<span data-ttu-id="9ac6b-122">Wert</span><span class="sxs-lookup"><span data-stu-id="9ac6b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9ac6b-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="9ac6b-123">Authorization</span></span>|<span data-ttu-id="9ac6b-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="9ac6b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9ac6b-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="9ac6b-125">Accept</span></span>|<span data-ttu-id="9ac6b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9ac6b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9ac6b-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9ac6b-127">Request body</span></span>
<span data-ttu-id="9ac6b-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) an.</span><span class="sxs-lookup"><span data-stu-id="9ac6b-128">In the request body, supply a JSON representation for the [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object.</span></span>

<span data-ttu-id="9ac6b-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="9ac6b-129">The following table shows the properties that are required when you create the [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md).</span></span>

|<span data-ttu-id="9ac6b-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9ac6b-130">Property</span></span>|<span data-ttu-id="9ac6b-131">Typ</span><span class="sxs-lookup"><span data-stu-id="9ac6b-131">Type</span></span>|<span data-ttu-id="9ac6b-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9ac6b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ac6b-133">id</span><span class="sxs-lookup"><span data-stu-id="9ac6b-133">id</span></span>|<span data-ttu-id="9ac6b-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9ac6b-134">String</span></span>|<span data-ttu-id="9ac6b-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="9ac6b-135">Key of the entity.</span></span> <span data-ttu-id="9ac6b-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9ac6b-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ac6b-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9ac6b-137">lastModifiedDateTime</span></span>|<span data-ttu-id="9ac6b-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9ac6b-138">DateTimeOffset</span></span>|<span data-ttu-id="9ac6b-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="9ac6b-139">DateTime the object was last modified.</span></span> <span data-ttu-id="9ac6b-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9ac6b-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ac6b-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9ac6b-141">roleScopeTagIds</span></span>|<span data-ttu-id="9ac6b-142">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="9ac6b-142">String collection</span></span>|<span data-ttu-id="9ac6b-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="9ac6b-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="9ac6b-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9ac6b-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ac6b-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="9ac6b-145">supportsScopeTags</span></span>|<span data-ttu-id="9ac6b-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ac6b-146">Boolean</span></span>|<span data-ttu-id="9ac6b-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9ac6b-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="9ac6b-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="9ac6b-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="9ac6b-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="9ac6b-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="9ac6b-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="9ac6b-150">This property is read-only.</span></span> <span data-ttu-id="9ac6b-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9ac6b-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ac6b-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9ac6b-152">createdDateTime</span></span>|<span data-ttu-id="9ac6b-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9ac6b-153">DateTimeOffset</span></span>|<span data-ttu-id="9ac6b-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="9ac6b-154">DateTime the object was created.</span></span> <span data-ttu-id="9ac6b-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9ac6b-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ac6b-156">description</span><span class="sxs-lookup"><span data-stu-id="9ac6b-156">description</span></span>|<span data-ttu-id="9ac6b-157">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9ac6b-157">String</span></span>|<span data-ttu-id="9ac6b-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="9ac6b-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="9ac6b-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9ac6b-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ac6b-160">displayName</span><span class="sxs-lookup"><span data-stu-id="9ac6b-160">displayName</span></span>|<span data-ttu-id="9ac6b-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9ac6b-161">String</span></span>|<span data-ttu-id="9ac6b-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="9ac6b-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="9ac6b-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9ac6b-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ac6b-164">Version</span><span class="sxs-lookup"><span data-stu-id="9ac6b-164">version</span></span>|<span data-ttu-id="9ac6b-165">Int32</span><span class="sxs-lookup"><span data-stu-id="9ac6b-165">Int32</span></span>|<span data-ttu-id="9ac6b-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="9ac6b-166">Version of the device configuration.</span></span> <span data-ttu-id="9ac6b-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9ac6b-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ac6b-168">advancedThreatProtectionOnboardingBlob</span><span class="sxs-lookup"><span data-stu-id="9ac6b-168">advancedThreatProtectionOnboardingBlob</span></span>|<span data-ttu-id="9ac6b-169">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9ac6b-169">String</span></span>|<span data-ttu-id="9ac6b-170">Windows Defender AdvancedThreatProtection Onboarding Blob.</span><span class="sxs-lookup"><span data-stu-id="9ac6b-170">Windows Defender AdvancedThreatProtection Onboarding Blob.</span></span>|
|<span data-ttu-id="9ac6b-171">advancedThreatProtectionOnboardingFilename</span><span class="sxs-lookup"><span data-stu-id="9ac6b-171">advancedThreatProtectionOnboardingFilename</span></span>|<span data-ttu-id="9ac6b-172">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9ac6b-172">String</span></span>|<span data-ttu-id="9ac6b-173">Der Name der Datei aus der AdvancedThreatProtectionOnboardingBlob abgerufen wurde.</span><span class="sxs-lookup"><span data-stu-id="9ac6b-173">Name of the file from which AdvancedThreatProtectionOnboardingBlob was obtained.</span></span>|
|<span data-ttu-id="9ac6b-174">advancedThreatProtectionAutoPopulateOnboardingBlob</span><span class="sxs-lookup"><span data-stu-id="9ac6b-174">advancedThreatProtectionAutoPopulateOnboardingBlob</span></span>|<span data-ttu-id="9ac6b-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ac6b-175">Boolean</span></span>|<span data-ttu-id="9ac6b-176">Füllen Sie automatisch auf Onboarding Blob programmgesteuert aus erweiterte Threat Protection-Diensts</span><span class="sxs-lookup"><span data-stu-id="9ac6b-176">Auto populate onboarding blob programmatically from Advanced Threat protection service</span></span>|
|<span data-ttu-id="9ac6b-177">allowSampleSharing</span><span class="sxs-lookup"><span data-stu-id="9ac6b-177">allowSampleSharing</span></span>|<span data-ttu-id="9ac6b-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ac6b-178">Boolean</span></span>|<span data-ttu-id="9ac6b-179">Regel „Beispielfreigabe zulassen“ in Windows Defender Advanced Threat Protection</span><span class="sxs-lookup"><span data-stu-id="9ac6b-179">Windows Defender AdvancedThreatProtection "Allow Sample Sharing" Rule</span></span>|
|<span data-ttu-id="9ac6b-180">enableExpeditedTelemetryReporting</span><span class="sxs-lookup"><span data-stu-id="9ac6b-180">enableExpeditedTelemetryReporting</span></span>|<span data-ttu-id="9ac6b-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ac6b-181">Boolean</span></span>|<span data-ttu-id="9ac6b-182">Verkürzt das Meldungsintervall für Windows Defender Advanced Threat Protection-Telemetriedaten.</span><span class="sxs-lookup"><span data-stu-id="9ac6b-182">Expedite Windows Defender Advanced Threat Protection telemetry reporting frequency.</span></span>|
|<span data-ttu-id="9ac6b-183">advancedThreatProtectionOffboardingBlob</span><span class="sxs-lookup"><span data-stu-id="9ac6b-183">advancedThreatProtectionOffboardingBlob</span></span>|<span data-ttu-id="9ac6b-184">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9ac6b-184">String</span></span>|<span data-ttu-id="9ac6b-185">Windows Defender AdvancedThreatProtection Offboarding Blob.</span><span class="sxs-lookup"><span data-stu-id="9ac6b-185">Windows Defender AdvancedThreatProtection Offboarding Blob.</span></span>|
|<span data-ttu-id="9ac6b-186">advancedThreatProtectionOffboardingFilename</span><span class="sxs-lookup"><span data-stu-id="9ac6b-186">advancedThreatProtectionOffboardingFilename</span></span>|<span data-ttu-id="9ac6b-187">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9ac6b-187">String</span></span>|<span data-ttu-id="9ac6b-188">Der Name der Datei aus der AdvancedThreatProtectionOffboardingBlob abgerufen wurde.</span><span class="sxs-lookup"><span data-stu-id="9ac6b-188">Name of the file from which AdvancedThreatProtectionOffboardingBlob was obtained.</span></span>|



## <a name="response"></a><span data-ttu-id="9ac6b-189">Antwort</span><span class="sxs-lookup"><span data-stu-id="9ac6b-189">Response</span></span>
<span data-ttu-id="9ac6b-190">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="9ac6b-190">If successful, this method returns a `200 OK` response code and an updated [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9ac6b-191">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9ac6b-191">Example</span></span>

### <a name="request"></a><span data-ttu-id="9ac6b-192">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9ac6b-192">Request</span></span>
<span data-ttu-id="9ac6b-193">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9ac6b-193">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="9ac6b-194">Antwort</span><span class="sxs-lookup"><span data-stu-id="9ac6b-194">Response</span></span>
<span data-ttu-id="9ac6b-p111">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9ac6b-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




