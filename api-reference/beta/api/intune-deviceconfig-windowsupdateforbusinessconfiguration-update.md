---
title: Aktualisieren von „windowsUpdateForBusinessConfiguration“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs windowsUpdateForBusinessConfiguration.
author: tfitzmac
ms.openlocfilehash: b887fe448a574f774cb45cd946cb1bf535c9f3b9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27307357"
---
# <a name="update-windowsupdateforbusinessconfiguration"></a><span data-ttu-id="f8038-103">Aktualisieren von „windowsUpdateForBusinessConfiguration“</span><span class="sxs-lookup"><span data-stu-id="f8038-103">Update windowsUpdateForBusinessConfiguration</span></span>

> <span data-ttu-id="f8038-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f8038-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f8038-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f8038-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f8038-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="f8038-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f8038-107">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f8038-107">Update the properties of a [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f8038-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f8038-108">Prerequisites</span></span>
<span data-ttu-id="f8038-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f8038-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f8038-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f8038-111">Permission type</span></span>|<span data-ttu-id="f8038-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f8038-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f8038-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f8038-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f8038-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f8038-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f8038-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f8038-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f8038-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f8038-116">Not supported.</span></span>|
|<span data-ttu-id="f8038-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f8038-117">Application</span></span>|<span data-ttu-id="f8038-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f8038-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f8038-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f8038-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="f8038-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f8038-120">Request headers</span></span>
|<span data-ttu-id="f8038-121">Header</span><span class="sxs-lookup"><span data-stu-id="f8038-121">Header</span></span>|<span data-ttu-id="f8038-122">Wert</span><span class="sxs-lookup"><span data-stu-id="f8038-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f8038-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="f8038-123">Authorization</span></span>|<span data-ttu-id="f8038-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="f8038-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f8038-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f8038-125">Accept</span></span>|<span data-ttu-id="f8038-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f8038-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f8038-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f8038-127">Request body</span></span>
<span data-ttu-id="f8038-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) an.</span><span class="sxs-lookup"><span data-stu-id="f8038-128">In the request body, supply a JSON representation for the [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object.</span></span>

<span data-ttu-id="f8038-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="f8038-129">The following table shows the properties that are required when you create the [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md).</span></span>

|<span data-ttu-id="f8038-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f8038-130">Property</span></span>|<span data-ttu-id="f8038-131">Typ</span><span class="sxs-lookup"><span data-stu-id="f8038-131">Type</span></span>|<span data-ttu-id="f8038-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f8038-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f8038-133">id</span><span class="sxs-lookup"><span data-stu-id="f8038-133">id</span></span>|<span data-ttu-id="f8038-134">String</span><span class="sxs-lookup"><span data-stu-id="f8038-134">String</span></span>|<span data-ttu-id="f8038-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="f8038-135">Key of the entity.</span></span> <span data-ttu-id="f8038-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f8038-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f8038-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f8038-137">lastModifiedDateTime</span></span>|<span data-ttu-id="f8038-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f8038-138">DateTimeOffset</span></span>|<span data-ttu-id="f8038-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="f8038-139">DateTime the object was last modified.</span></span> <span data-ttu-id="f8038-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f8038-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f8038-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f8038-141">roleScopeTagIds</span></span>|<span data-ttu-id="f8038-142">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="f8038-142">String collection</span></span>|<span data-ttu-id="f8038-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="f8038-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f8038-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f8038-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f8038-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="f8038-145">supportsScopeTags</span></span>|<span data-ttu-id="f8038-146">Boolesch</span><span class="sxs-lookup"><span data-stu-id="f8038-146">Boolean</span></span>|<span data-ttu-id="f8038-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f8038-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f8038-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="f8038-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f8038-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="f8038-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f8038-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="f8038-150">This property is read-only.</span></span> <span data-ttu-id="f8038-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f8038-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f8038-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f8038-152">createdDateTime</span></span>|<span data-ttu-id="f8038-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f8038-153">DateTimeOffset</span></span>|<span data-ttu-id="f8038-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="f8038-154">DateTime the object was created.</span></span> <span data-ttu-id="f8038-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f8038-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f8038-156">description</span><span class="sxs-lookup"><span data-stu-id="f8038-156">description</span></span>|<span data-ttu-id="f8038-157">String</span><span class="sxs-lookup"><span data-stu-id="f8038-157">String</span></span>|<span data-ttu-id="f8038-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="f8038-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f8038-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f8038-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f8038-160">displayName</span><span class="sxs-lookup"><span data-stu-id="f8038-160">displayName</span></span>|<span data-ttu-id="f8038-161">String</span><span class="sxs-lookup"><span data-stu-id="f8038-161">String</span></span>|<span data-ttu-id="f8038-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="f8038-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f8038-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f8038-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f8038-164">Version</span><span class="sxs-lookup"><span data-stu-id="f8038-164">version</span></span>|<span data-ttu-id="f8038-165">Int32</span><span class="sxs-lookup"><span data-stu-id="f8038-165">Int32</span></span>|<span data-ttu-id="f8038-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="f8038-166">Version of the device configuration.</span></span> <span data-ttu-id="f8038-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f8038-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f8038-168">deliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="f8038-168">deliveryOptimizationMode</span></span>|[<span data-ttu-id="f8038-169">windowsDeliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="f8038-169">windowsDeliveryOptimizationMode</span></span>](../resources/intune-deviceconfig-windowsdeliveryoptimizationmode.md)|<span data-ttu-id="f8038-170">Übermittlung Optimierung Modus.</span><span class="sxs-lookup"><span data-stu-id="f8038-170">Delivery Optimization Mode.</span></span> <span data-ttu-id="f8038-171">Mögliche Werte sind: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload` und `bypassMode`.</span><span class="sxs-lookup"><span data-stu-id="f8038-171">Possible values are: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.</span></span>|
|<span data-ttu-id="f8038-172">prereleaseFeatures</span><span class="sxs-lookup"><span data-stu-id="f8038-172">prereleaseFeatures</span></span>|[<span data-ttu-id="f8038-173">prereleaseFeatures</span><span class="sxs-lookup"><span data-stu-id="f8038-173">prereleaseFeatures</span></span>](../resources/intune-deviceconfig-prereleasefeatures.md)|<span data-ttu-id="f8038-174">Pre-Release-Funktionen.</span><span class="sxs-lookup"><span data-stu-id="f8038-174">The pre-release features.</span></span> <span data-ttu-id="f8038-175">Mögliche Werte sind: `userDefined`, `settingsOnly`, `settingsAndExperimentations` und `notAllowed`.</span><span class="sxs-lookup"><span data-stu-id="f8038-175">Possible values are: `userDefined`, `settingsOnly`, `settingsAndExperimentations`, `notAllowed`.</span></span>|
|<span data-ttu-id="f8038-176">automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="f8038-176">automaticUpdateMode</span></span>|[<span data-ttu-id="f8038-177">automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="f8038-177">automaticUpdateMode</span></span>](../resources/intune-deviceconfig-automaticupdatemode.md)|<span data-ttu-id="f8038-178">Modus für automatische Updates.</span><span class="sxs-lookup"><span data-stu-id="f8038-178">Automatic update mode.</span></span> <span data-ttu-id="f8038-179">Mögliche Werte sind: `userDefined`, `notifyDownload`, `autoInstallAtMaintenanceTime`, `autoInstallAndRebootAtMaintenanceTime`, `autoInstallAndRebootAtScheduledTime` und `autoInstallAndRebootWithoutEndUserControl`.</span><span class="sxs-lookup"><span data-stu-id="f8038-179">Possible values are: `userDefined`, `notifyDownload`, `autoInstallAtMaintenanceTime`, `autoInstallAndRebootAtMaintenanceTime`, `autoInstallAndRebootAtScheduledTime`, `autoInstallAndRebootWithoutEndUserControl`.</span></span>|
|<span data-ttu-id="f8038-180">microsoftUpdateServiceAllowed</span><span class="sxs-lookup"><span data-stu-id="f8038-180">microsoftUpdateServiceAllowed</span></span>|<span data-ttu-id="f8038-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="f8038-181">Boolean</span></span>|<span data-ttu-id="f8038-182">Legt fest, dass der Microsoft Update Service zugelassen wird.</span><span class="sxs-lookup"><span data-stu-id="f8038-182">Allow Microsoft Update Service</span></span>|
|<span data-ttu-id="f8038-183">driversExcluded</span><span class="sxs-lookup"><span data-stu-id="f8038-183">driversExcluded</span></span>|<span data-ttu-id="f8038-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="f8038-184">Boolean</span></span>|<span data-ttu-id="f8038-185">Legt fest, dass Treiber von Windows-Updates ausgenommen werden.</span><span class="sxs-lookup"><span data-stu-id="f8038-185">Exclude Windows update Drivers</span></span>|
|<span data-ttu-id="f8038-186">installationSchedule</span><span class="sxs-lookup"><span data-stu-id="f8038-186">installationSchedule</span></span>|[<span data-ttu-id="f8038-187">windowsUpdateInstallScheduleType</span><span class="sxs-lookup"><span data-stu-id="f8038-187">windowsUpdateInstallScheduleType</span></span>](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)|<span data-ttu-id="f8038-188">Installationszeitplan</span><span class="sxs-lookup"><span data-stu-id="f8038-188">Installation schedule</span></span>|
|<span data-ttu-id="f8038-189">qualityUpdatesDeferralPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="f8038-189">qualityUpdatesDeferralPeriodInDays</span></span>|<span data-ttu-id="f8038-190">Int32</span><span class="sxs-lookup"><span data-stu-id="f8038-190">Int32</span></span>|<span data-ttu-id="f8038-191">Legt fest, um wie viele Tage Qualitätsupdates zurückgestellt werden sollen.</span><span class="sxs-lookup"><span data-stu-id="f8038-191">Defer Quality Updates by these many days</span></span>|
|<span data-ttu-id="f8038-192">featureUpdatesDeferralPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="f8038-192">featureUpdatesDeferralPeriodInDays</span></span>|<span data-ttu-id="f8038-193">Int32</span><span class="sxs-lookup"><span data-stu-id="f8038-193">Int32</span></span>|<span data-ttu-id="f8038-194">Legt fest, um wie viele Tage Funktionsupdates zurückgestellt werden sollen.</span><span class="sxs-lookup"><span data-stu-id="f8038-194">Defer Feature Updates by these many days</span></span>|
|<span data-ttu-id="f8038-195">qualityUpdatesPaused</span><span class="sxs-lookup"><span data-stu-id="f8038-195">qualityUpdatesPaused</span></span>|<span data-ttu-id="f8038-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="f8038-196">Boolean</span></span>|<span data-ttu-id="f8038-197">Setzt Qualitätsupdates aus.</span><span class="sxs-lookup"><span data-stu-id="f8038-197">Pause Quality Updates</span></span>|
|<span data-ttu-id="f8038-198">featureUpdatesPaused</span><span class="sxs-lookup"><span data-stu-id="f8038-198">featureUpdatesPaused</span></span>|<span data-ttu-id="f8038-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="f8038-199">Boolean</span></span>|<span data-ttu-id="f8038-200">Setzt Funktionsupdates aus.</span><span class="sxs-lookup"><span data-stu-id="f8038-200">Pause Feature Updates</span></span>|
|<span data-ttu-id="f8038-201">qualityUpdatesPauseExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="f8038-201">qualityUpdatesPauseExpiryDateTime</span></span>|<span data-ttu-id="f8038-202">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f8038-202">DateTimeOffset</span></span>|<span data-ttu-id="f8038-203">Datum und Uhrzeit des Ablaufs der Aussetzung der Qualitätsupdates</span><span class="sxs-lookup"><span data-stu-id="f8038-203">Quality Updates Pause Expiry datetime</span></span>|
|<span data-ttu-id="f8038-204">featureUpdatesPauseExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="f8038-204">featureUpdatesPauseExpiryDateTime</span></span>|<span data-ttu-id="f8038-205">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f8038-205">DateTimeOffset</span></span>|<span data-ttu-id="f8038-206">Datum und Uhrzeit des Ablaufs der Aussetzung der Funktionsupdates</span><span class="sxs-lookup"><span data-stu-id="f8038-206">Feature Updates Pause Expiry datetime</span></span>|
|<span data-ttu-id="f8038-207">businessReadyUpdatesOnly</span><span class="sxs-lookup"><span data-stu-id="f8038-207">businessReadyUpdatesOnly</span></span>|[<span data-ttu-id="f8038-208">windowsUpdateType</span><span class="sxs-lookup"><span data-stu-id="f8038-208">windowsUpdateType</span></span>](../resources/intune-deviceconfig-windowsupdatetype.md)|<span data-ttu-id="f8038-209">Bestimmt, welche Geräte Branch ihre Updates von erhält.</span><span class="sxs-lookup"><span data-stu-id="f8038-209">Determines which branch devices will receive their updates from.</span></span> <span data-ttu-id="f8038-210">Mögliche Werte sind: `userDefined`, `all`, `businessReadyOnly`, `windowsInsiderBuildFast`, `windowsInsiderBuildSlow` und `windowsInsiderBuildRelease`.</span><span class="sxs-lookup"><span data-stu-id="f8038-210">Possible values are: `userDefined`, `all`, `businessReadyOnly`, `windowsInsiderBuildFast`, `windowsInsiderBuildSlow`, `windowsInsiderBuildRelease`.</span></span>|
|<span data-ttu-id="f8038-211">skipChecksBeforeRestart</span><span class="sxs-lookup"><span data-stu-id="f8038-211">skipChecksBeforeRestart</span></span>|<span data-ttu-id="f8038-212">Boolesch</span><span class="sxs-lookup"><span data-stu-id="f8038-212">Boolean</span></span>|<span data-ttu-id="f8038-213">Legen Sie vor dem Neustart alle Kontrollkästchen überspringen: Batterie Level = 40 %, Anwesenheitsinformationen des Benutzers, Anzeige benötigt, Präsentationsmodus, Vollbildmodus, Telefonanruf Zustand, Spiel Modus usw..</span><span class="sxs-lookup"><span data-stu-id="f8038-213">Set to skip all check before restart: Battery level = 40%, User presence, Display Needed, Presentation mode, Full screen mode, phone call state, game mode etc.</span></span> |
|<span data-ttu-id="f8038-214">updateWeeks</span><span class="sxs-lookup"><span data-stu-id="f8038-214">updateWeeks</span></span>|[<span data-ttu-id="f8038-215">windowsUpdateForBusinessUpdateWeeks</span><span class="sxs-lookup"><span data-stu-id="f8038-215">windowsUpdateForBusinessUpdateWeeks</span></span>](../resources/intune-deviceconfig-windowsupdateforbusinessupdateweeks.md)|<span data-ttu-id="f8038-216">Die Installation des Updates auf den Wochen des Monats geplant.</span><span class="sxs-lookup"><span data-stu-id="f8038-216">Scheduled the update installation on the weeks of the month.</span></span> <span data-ttu-id="f8038-217">Mögliche Werte sind: `userDefined`, `firstWeek`, `secondWeek`, `thirdWeek`, `fourthWeek` und `everyWeek`.</span><span class="sxs-lookup"><span data-stu-id="f8038-217">Possible values are: `userDefined`, `firstWeek`, `secondWeek`, `thirdWeek`, `fourthWeek`, `everyWeek`.</span></span>|
|<span data-ttu-id="f8038-218">qualityUpdatesPauseStartDateTime</span><span class="sxs-lookup"><span data-stu-id="f8038-218">qualityUpdatesPauseStartDateTime</span></span>|<span data-ttu-id="f8038-219">String</span><span class="sxs-lookup"><span data-stu-id="f8038-219">String</span></span>|<span data-ttu-id="f8038-220">Qualität Updates anhalten starten datetime</span><span class="sxs-lookup"><span data-stu-id="f8038-220">Quality Updates Pause Start datetime</span></span>|
|<span data-ttu-id="f8038-221">featureUpdatesPauseStartDateTime</span><span class="sxs-lookup"><span data-stu-id="f8038-221">featureUpdatesPauseStartDateTime</span></span>|<span data-ttu-id="f8038-222">String</span><span class="sxs-lookup"><span data-stu-id="f8038-222">String</span></span>|<span data-ttu-id="f8038-223">Feature Updates anhalten starten datetime</span><span class="sxs-lookup"><span data-stu-id="f8038-223">Feature Updates Pause Start datetime</span></span>|
|<span data-ttu-id="f8038-224">featureUpdatesRollbackWindowInDays</span><span class="sxs-lookup"><span data-stu-id="f8038-224">featureUpdatesRollbackWindowInDays</span></span>|<span data-ttu-id="f8038-225">Int32</span><span class="sxs-lookup"><span data-stu-id="f8038-225">Int32</span></span>|<span data-ttu-id="f8038-226">Die Anzahl der Tage nach einer Aktualisierung der Features für die ein Rollback gültig ist.</span><span class="sxs-lookup"><span data-stu-id="f8038-226">The number of days after a Feature Update for which a rollback is valid</span></span>|
|<span data-ttu-id="f8038-227">qualityUpdatesWillBeRolledBack</span><span class="sxs-lookup"><span data-stu-id="f8038-227">qualityUpdatesWillBeRolledBack</span></span>|<span data-ttu-id="f8038-228">Boolesch</span><span class="sxs-lookup"><span data-stu-id="f8038-228">Boolean</span></span>|<span data-ttu-id="f8038-229">Gibt an, ob Rollback Qualität Updates auf dem nächsten Gerät</span><span class="sxs-lookup"><span data-stu-id="f8038-229">Specifies whether to rollback Quality Updates on the next device check in</span></span>|
|<span data-ttu-id="f8038-230">featureUpdatesWillBeRolledBack</span><span class="sxs-lookup"><span data-stu-id="f8038-230">featureUpdatesWillBeRolledBack</span></span>|<span data-ttu-id="f8038-231">Boolesch</span><span class="sxs-lookup"><span data-stu-id="f8038-231">Boolean</span></span>|<span data-ttu-id="f8038-232">Gibt an, ob Rollback-Feature-Updates auf das nächste Gerät</span><span class="sxs-lookup"><span data-stu-id="f8038-232">Specifies whether to rollback Feature Updates on the next device check in</span></span>|
|<span data-ttu-id="f8038-233">qualityUpdatesRollbackStartDateTime</span><span class="sxs-lookup"><span data-stu-id="f8038-233">qualityUpdatesRollbackStartDateTime</span></span>|<span data-ttu-id="f8038-234">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f8038-234">DateTimeOffset</span></span>|<span data-ttu-id="f8038-235">Qualität Updates Rollback starten datetime</span><span class="sxs-lookup"><span data-stu-id="f8038-235">Quality Updates Rollback Start datetime</span></span>|
|<span data-ttu-id="f8038-236">featureUpdatesRollbackStartDateTime</span><span class="sxs-lookup"><span data-stu-id="f8038-236">featureUpdatesRollbackStartDateTime</span></span>|<span data-ttu-id="f8038-237">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f8038-237">DateTimeOffset</span></span>|<span data-ttu-id="f8038-238">Feature Updates Rollback starten datetime</span><span class="sxs-lookup"><span data-stu-id="f8038-238">Feature Updates Rollback Start datetime</span></span>|
|<span data-ttu-id="f8038-239">engagedRestartDeadlineInDays</span><span class="sxs-lookup"><span data-stu-id="f8038-239">engagedRestartDeadlineInDays</span></span>|<span data-ttu-id="f8038-240">Int32</span><span class="sxs-lookup"><span data-stu-id="f8038-240">Int32</span></span>|<span data-ttu-id="f8038-241">Stichtag in Tagen, bevor Sie automatisch planen und Ausführen von ein ausstehender Neustart außerhalb von aktiven Stunden mit gültigen Bereich von 2 bis 30 Tage</span><span class="sxs-lookup"><span data-stu-id="f8038-241">Deadline in days before automatically scheduling and executing a pending restart outside of active hours, with valid range from 2 to 30 days</span></span>|
|<span data-ttu-id="f8038-242">engagedRestartSnoozeScheduleInDays</span><span class="sxs-lookup"><span data-stu-id="f8038-242">engagedRestartSnoozeScheduleInDays</span></span>|<span data-ttu-id="f8038-243">Int32</span><span class="sxs-lookup"><span data-stu-id="f8038-243">Int32</span></span>|<span data-ttu-id="f8038-244">Anzahl der Tage, die ein Benutzer Erinnerungen mit gültigen Bereich von 1 bis 3 Tage engagiertes neu starten erneut erinnern können</span><span class="sxs-lookup"><span data-stu-id="f8038-244">Number of days a user can snooze Engaged Restart reminder notifications with valid range from 1 to 3 days</span></span>|
|<span data-ttu-id="f8038-245">engagedRestartTransitionScheduleInDays</span><span class="sxs-lookup"><span data-stu-id="f8038-245">engagedRestartTransitionScheduleInDays</span></span>|<span data-ttu-id="f8038-246">Int32</span><span class="sxs-lookup"><span data-stu-id="f8038-246">Int32</span></span>|<span data-ttu-id="f8038-247">Anzahl von Tagen vor dem Übergang von automatischen Neustart geplant außerhalb der aktiven engagiertes neu starten, die den Benutzer mit gültigen Bereich von 0 bis 30 Tage planen erforderlich sind</span><span class="sxs-lookup"><span data-stu-id="f8038-247">Number of days before transitioning from Auto Restarts scheduled outside of active hours to Engaged Restart, which requires the user to schedule, with valid range from 0 to 30 days</span></span>|
|<span data-ttu-id="f8038-248">autoRestartNotificationDismissal</span><span class="sxs-lookup"><span data-stu-id="f8038-248">autoRestartNotificationDismissal</span></span>|[<span data-ttu-id="f8038-249">autoRestartNotificationDismissalMethod</span><span class="sxs-lookup"><span data-stu-id="f8038-249">autoRestartNotificationDismissalMethod</span></span>](../resources/intune-deviceconfig-autorestartnotificationdismissalmethod.md)|<span data-ttu-id="f8038-250">Geben Sie die Methode mit der der automatische Neustart erforderlich, dass die Benachrichtigung geschlossen wird.</span><span class="sxs-lookup"><span data-stu-id="f8038-250">Specify the method by which the auto-restart required notification is dismissed.</span></span> <span data-ttu-id="f8038-251">Mögliche Werte sind: `notConfigured`, `automatic` und `user`.</span><span class="sxs-lookup"><span data-stu-id="f8038-251">Possible values are: `notConfigured`, `automatic`, `user`.</span></span>|
|<span data-ttu-id="f8038-252">scheduleRestartWarningInHours</span><span class="sxs-lookup"><span data-stu-id="f8038-252">scheduleRestartWarningInHours</span></span>|<span data-ttu-id="f8038-253">Int32</span><span class="sxs-lookup"><span data-stu-id="f8038-253">Int32</span></span>|<span data-ttu-id="f8038-254">Geben Sie den Zeitraum an, für die automatische Neustart Warnung Erinnerungen.</span><span class="sxs-lookup"><span data-stu-id="f8038-254">Specify the period for auto-restart warning reminder notifications.</span></span> <span data-ttu-id="f8038-255">Unterstützte Werte: 2, 4, 8, 12 oder 24 (Stunden).</span><span class="sxs-lookup"><span data-stu-id="f8038-255">Supported values: 2, 4, 8, 12 or 24 (hours).</span></span>|
|<span data-ttu-id="f8038-256">scheduleImminentRestartWarningInMinutes</span><span class="sxs-lookup"><span data-stu-id="f8038-256">scheduleImminentRestartWarningInMinutes</span></span>|<span data-ttu-id="f8038-257">Int32</span><span class="sxs-lookup"><span data-stu-id="f8038-257">Int32</span></span>|<span data-ttu-id="f8038-258">Geben Sie den Zeitraum an, für die automatische Neustart anstehender warnbenachrichtigungen.</span><span class="sxs-lookup"><span data-stu-id="f8038-258">Specify the period for auto-restart imminent warning notifications.</span></span> <span data-ttu-id="f8038-259">Unterstützte Werte: 15, 30 oder 60 (Minuten).</span><span class="sxs-lookup"><span data-stu-id="f8038-259">Supported values: 15, 30 or 60 (minutes).</span></span>|



## <a name="response"></a><span data-ttu-id="f8038-260">Antwort</span><span class="sxs-lookup"><span data-stu-id="f8038-260">Response</span></span>
<span data-ttu-id="f8038-261">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="f8038-261">If successful, this method returns a `200 OK` response code and an updated [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f8038-262">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f8038-262">Example</span></span>
### <a name="request"></a><span data-ttu-id="f8038-263">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f8038-263">Request</span></span>
<span data-ttu-id="f8038-264">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f8038-264">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1787

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "deliveryOptimizationMode": "httpOnly",
  "prereleaseFeatures": "settingsOnly",
  "automaticUpdateMode": "notifyDownload",
  "microsoftUpdateServiceAllowed": true,
  "driversExcluded": true,
  "installationSchedule": {
    "@odata.type": "microsoft.graph.windowsUpdateScheduledInstall",
    "scheduledInstallDay": "everyday",
    "scheduledInstallTime": "11:59:31.3170000"
  },
  "qualityUpdatesDeferralPeriodInDays": 2,
  "featureUpdatesDeferralPeriodInDays": 2,
  "qualityUpdatesPaused": true,
  "featureUpdatesPaused": true,
  "qualityUpdatesPauseExpiryDateTime": "2017-01-01T00:00:22.9594683-08:00",
  "featureUpdatesPauseExpiryDateTime": "2016-12-31T23:58:08.068669-08:00",
  "businessReadyUpdatesOnly": "all",
  "skipChecksBeforeRestart": true,
  "updateWeeks": "firstWeek",
  "qualityUpdatesPauseStartDateTime": "Quality Updates Pause Start Date Time value",
  "featureUpdatesPauseStartDateTime": "Feature Updates Pause Start Date Time value",
  "featureUpdatesRollbackWindowInDays": 2,
  "qualityUpdatesWillBeRolledBack": true,
  "featureUpdatesWillBeRolledBack": true,
  "qualityUpdatesRollbackStartDateTime": "2016-12-31T23:57:01.05526-08:00",
  "featureUpdatesRollbackStartDateTime": "2017-01-01T00:03:21.6080517-08:00",
  "engagedRestartDeadlineInDays": 12,
  "engagedRestartSnoozeScheduleInDays": 2,
  "engagedRestartTransitionScheduleInDays": 6,
  "autoRestartNotificationDismissal": "automatic",
  "scheduleRestartWarningInHours": 13,
  "scheduleImminentRestartWarningInMinutes": 7
}
```

### <a name="response"></a><span data-ttu-id="f8038-265">Antwort</span><span class="sxs-lookup"><span data-stu-id="f8038-265">Response</span></span>
<span data-ttu-id="f8038-p119">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f8038-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1971

{
  "@odata.type": "#microsoft.graph.windowsUpdateForBusinessConfiguration",
  "id": "4928dd6a-dd6a-4928-6add-28496add2849",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "deliveryOptimizationMode": "httpOnly",
  "prereleaseFeatures": "settingsOnly",
  "automaticUpdateMode": "notifyDownload",
  "microsoftUpdateServiceAllowed": true,
  "driversExcluded": true,
  "installationSchedule": {
    "@odata.type": "microsoft.graph.windowsUpdateScheduledInstall",
    "scheduledInstallDay": "everyday",
    "scheduledInstallTime": "11:59:31.3170000"
  },
  "qualityUpdatesDeferralPeriodInDays": 2,
  "featureUpdatesDeferralPeriodInDays": 2,
  "qualityUpdatesPaused": true,
  "featureUpdatesPaused": true,
  "qualityUpdatesPauseExpiryDateTime": "2017-01-01T00:00:22.9594683-08:00",
  "featureUpdatesPauseExpiryDateTime": "2016-12-31T23:58:08.068669-08:00",
  "businessReadyUpdatesOnly": "all",
  "skipChecksBeforeRestart": true,
  "updateWeeks": "firstWeek",
  "qualityUpdatesPauseStartDateTime": "Quality Updates Pause Start Date Time value",
  "featureUpdatesPauseStartDateTime": "Feature Updates Pause Start Date Time value",
  "featureUpdatesRollbackWindowInDays": 2,
  "qualityUpdatesWillBeRolledBack": true,
  "featureUpdatesWillBeRolledBack": true,
  "qualityUpdatesRollbackStartDateTime": "2016-12-31T23:57:01.05526-08:00",
  "featureUpdatesRollbackStartDateTime": "2017-01-01T00:03:21.6080517-08:00",
  "engagedRestartDeadlineInDays": 12,
  "engagedRestartSnoozeScheduleInDays": 2,
  "engagedRestartTransitionScheduleInDays": 6,
  "autoRestartNotificationDismissal": "automatic",
  "scheduleRestartWarningInHours": 13,
  "scheduleImminentRestartWarningInMinutes": 7
}
```





