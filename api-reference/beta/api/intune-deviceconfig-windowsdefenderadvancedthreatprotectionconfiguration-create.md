---
title: Erstellen von „windowsDefenderAdvancedThreatProtectionConfiguration“
description: Diese Methode erstellt ein neues Objekt des Typs windowsDefenderAdvancedThreatProtectionConfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 704365da447e3e6ccf702479ddceb06a3c14c4cd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27836239"
---
# <a name="create-windowsdefenderadvancedthreatprotectionconfiguration"></a><span data-ttu-id="dd9e1-103">Erstellen von „windowsDefenderAdvancedThreatProtectionConfiguration“</span><span class="sxs-lookup"><span data-stu-id="dd9e1-103">Create windowsDefenderAdvancedThreatProtectionConfiguration</span></span>

> <span data-ttu-id="dd9e1-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="dd9e1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dd9e1-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="dd9e1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="dd9e1-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="dd9e1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dd9e1-107">Diese Methode erstellt ein neues Objekt des Typs [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="dd9e1-107">Create a new [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="dd9e1-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="dd9e1-108">Prerequisites</span></span>
<span data-ttu-id="dd9e1-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dd9e1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dd9e1-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="dd9e1-111">Permission type</span></span>|<span data-ttu-id="dd9e1-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="dd9e1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dd9e1-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="dd9e1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="dd9e1-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd9e1-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="dd9e1-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="dd9e1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dd9e1-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="dd9e1-116">Not supported.</span></span>|
|<span data-ttu-id="dd9e1-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="dd9e1-117">Application</span></span>|<span data-ttu-id="dd9e1-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="dd9e1-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dd9e1-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="dd9e1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="dd9e1-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="dd9e1-120">Request headers</span></span>
|<span data-ttu-id="dd9e1-121">Header</span><span class="sxs-lookup"><span data-stu-id="dd9e1-121">Header</span></span>|<span data-ttu-id="dd9e1-122">Wert</span><span class="sxs-lookup"><span data-stu-id="dd9e1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dd9e1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="dd9e1-123">Authorization</span></span>|<span data-ttu-id="dd9e1-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="dd9e1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dd9e1-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="dd9e1-125">Accept</span></span>|<span data-ttu-id="dd9e1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="dd9e1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dd9e1-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="dd9e1-127">Request body</span></span>
<span data-ttu-id="dd9e1-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „windowsDefenderAdvancedThreatProtectionConfiguration“ an.</span><span class="sxs-lookup"><span data-stu-id="dd9e1-128">In the request body, supply a JSON representation for the windowsDefenderAdvancedThreatProtectionConfiguration object.</span></span>

<span data-ttu-id="dd9e1-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „windowsDefenderAdvancedThreatProtectionConfiguration“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="dd9e1-129">The following table shows the properties that are required when you create the windowsDefenderAdvancedThreatProtectionConfiguration.</span></span>

|<span data-ttu-id="dd9e1-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="dd9e1-130">Property</span></span>|<span data-ttu-id="dd9e1-131">Typ</span><span class="sxs-lookup"><span data-stu-id="dd9e1-131">Type</span></span>|<span data-ttu-id="dd9e1-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="dd9e1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dd9e1-133">id</span><span class="sxs-lookup"><span data-stu-id="dd9e1-133">id</span></span>|<span data-ttu-id="dd9e1-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="dd9e1-134">String</span></span>|<span data-ttu-id="dd9e1-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="dd9e1-135">Key of the entity.</span></span> <span data-ttu-id="dd9e1-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="dd9e1-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dd9e1-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="dd9e1-137">lastModifiedDateTime</span></span>|<span data-ttu-id="dd9e1-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dd9e1-138">DateTimeOffset</span></span>|<span data-ttu-id="dd9e1-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="dd9e1-139">DateTime the object was last modified.</span></span> <span data-ttu-id="dd9e1-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="dd9e1-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dd9e1-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="dd9e1-141">roleScopeTagIds</span></span>|<span data-ttu-id="dd9e1-142">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="dd9e1-142">String collection</span></span>|<span data-ttu-id="dd9e1-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="dd9e1-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="dd9e1-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="dd9e1-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dd9e1-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="dd9e1-145">supportsScopeTags</span></span>|<span data-ttu-id="dd9e1-146">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="dd9e1-146">Boolean</span></span>|<span data-ttu-id="dd9e1-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="dd9e1-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="dd9e1-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="dd9e1-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="dd9e1-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="dd9e1-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="dd9e1-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="dd9e1-150">This property is read-only.</span></span> <span data-ttu-id="dd9e1-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="dd9e1-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dd9e1-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="dd9e1-152">createdDateTime</span></span>|<span data-ttu-id="dd9e1-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dd9e1-153">DateTimeOffset</span></span>|<span data-ttu-id="dd9e1-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="dd9e1-154">DateTime the object was created.</span></span> <span data-ttu-id="dd9e1-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="dd9e1-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dd9e1-156">description</span><span class="sxs-lookup"><span data-stu-id="dd9e1-156">description</span></span>|<span data-ttu-id="dd9e1-157">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="dd9e1-157">String</span></span>|<span data-ttu-id="dd9e1-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="dd9e1-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="dd9e1-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="dd9e1-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dd9e1-160">displayName</span><span class="sxs-lookup"><span data-stu-id="dd9e1-160">displayName</span></span>|<span data-ttu-id="dd9e1-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="dd9e1-161">String</span></span>|<span data-ttu-id="dd9e1-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="dd9e1-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="dd9e1-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="dd9e1-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dd9e1-164">Version</span><span class="sxs-lookup"><span data-stu-id="dd9e1-164">version</span></span>|<span data-ttu-id="dd9e1-165">Int32</span><span class="sxs-lookup"><span data-stu-id="dd9e1-165">Int32</span></span>|<span data-ttu-id="dd9e1-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="dd9e1-166">Version of the device configuration.</span></span> <span data-ttu-id="dd9e1-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="dd9e1-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dd9e1-168">advancedThreatProtectionOnboardingBlob</span><span class="sxs-lookup"><span data-stu-id="dd9e1-168">advancedThreatProtectionOnboardingBlob</span></span>|<span data-ttu-id="dd9e1-169">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="dd9e1-169">String</span></span>|<span data-ttu-id="dd9e1-170">Windows Defender AdvancedThreatProtection Onboarding Blob.</span><span class="sxs-lookup"><span data-stu-id="dd9e1-170">Windows Defender AdvancedThreatProtection Onboarding Blob.</span></span>|
|<span data-ttu-id="dd9e1-171">advancedThreatProtectionOnboardingFilename</span><span class="sxs-lookup"><span data-stu-id="dd9e1-171">advancedThreatProtectionOnboardingFilename</span></span>|<span data-ttu-id="dd9e1-172">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="dd9e1-172">String</span></span>|<span data-ttu-id="dd9e1-173">Der Name der Datei aus der AdvancedThreatProtectionOnboardingBlob abgerufen wurde.</span><span class="sxs-lookup"><span data-stu-id="dd9e1-173">Name of the file from which AdvancedThreatProtectionOnboardingBlob was obtained.</span></span>|
|<span data-ttu-id="dd9e1-174">advancedThreatProtectionAutoPopulateOnboardingBlob</span><span class="sxs-lookup"><span data-stu-id="dd9e1-174">advancedThreatProtectionAutoPopulateOnboardingBlob</span></span>|<span data-ttu-id="dd9e1-175">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="dd9e1-175">Boolean</span></span>|<span data-ttu-id="dd9e1-176">Füllen Sie automatisch auf Onboarding Blob programmgesteuert aus erweiterte Threat Protection-Diensts</span><span class="sxs-lookup"><span data-stu-id="dd9e1-176">Auto populate onboarding blob programmatically from Advanced Threat protection service</span></span>|
|<span data-ttu-id="dd9e1-177">allowSampleSharing</span><span class="sxs-lookup"><span data-stu-id="dd9e1-177">allowSampleSharing</span></span>|<span data-ttu-id="dd9e1-178">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="dd9e1-178">Boolean</span></span>|<span data-ttu-id="dd9e1-179">Regel „Beispielfreigabe zulassen“ in Windows Defender Advanced Threat Protection</span><span class="sxs-lookup"><span data-stu-id="dd9e1-179">Windows Defender AdvancedThreatProtection "Allow Sample Sharing" Rule</span></span>|
|<span data-ttu-id="dd9e1-180">enableExpeditedTelemetryReporting</span><span class="sxs-lookup"><span data-stu-id="dd9e1-180">enableExpeditedTelemetryReporting</span></span>|<span data-ttu-id="dd9e1-181">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="dd9e1-181">Boolean</span></span>|<span data-ttu-id="dd9e1-182">Verkürzt das Meldungsintervall für Windows Defender Advanced Threat Protection-Telemetriedaten.</span><span class="sxs-lookup"><span data-stu-id="dd9e1-182">Expedite Windows Defender Advanced Threat Protection telemetry reporting frequency.</span></span>|
|<span data-ttu-id="dd9e1-183">advancedThreatProtectionOffboardingBlob</span><span class="sxs-lookup"><span data-stu-id="dd9e1-183">advancedThreatProtectionOffboardingBlob</span></span>|<span data-ttu-id="dd9e1-184">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="dd9e1-184">String</span></span>|<span data-ttu-id="dd9e1-185">Windows Defender AdvancedThreatProtection Offboarding Blob.</span><span class="sxs-lookup"><span data-stu-id="dd9e1-185">Windows Defender AdvancedThreatProtection Offboarding Blob.</span></span>|
|<span data-ttu-id="dd9e1-186">advancedThreatProtectionOffboardingFilename</span><span class="sxs-lookup"><span data-stu-id="dd9e1-186">advancedThreatProtectionOffboardingFilename</span></span>|<span data-ttu-id="dd9e1-187">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="dd9e1-187">String</span></span>|<span data-ttu-id="dd9e1-188">Der Name der Datei aus der AdvancedThreatProtectionOffboardingBlob abgerufen wurde.</span><span class="sxs-lookup"><span data-stu-id="dd9e1-188">Name of the file from which AdvancedThreatProtectionOffboardingBlob was obtained.</span></span>|



## <a name="response"></a><span data-ttu-id="dd9e1-189">Antwort</span><span class="sxs-lookup"><span data-stu-id="dd9e1-189">Response</span></span>
<span data-ttu-id="dd9e1-190">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="dd9e1-190">If successful, this method returns a `201 Created` response code and a [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dd9e1-191">Beispiel</span><span class="sxs-lookup"><span data-stu-id="dd9e1-191">Example</span></span>
### <a name="request"></a><span data-ttu-id="dd9e1-192">Anforderung</span><span class="sxs-lookup"><span data-stu-id="dd9e1-192">Request</span></span>
<span data-ttu-id="dd9e1-193">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="dd9e1-193">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 894

{
  "@odata.type": "#microsoft.graph.windowsDefenderAdvancedThreatProtectionConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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

### <a name="response"></a><span data-ttu-id="dd9e1-194">Antwort</span><span class="sxs-lookup"><span data-stu-id="dd9e1-194">Response</span></span>
<span data-ttu-id="dd9e1-p111">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="dd9e1-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





