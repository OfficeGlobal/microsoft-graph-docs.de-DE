---
title: Aktualisieren von „windowsUpdateForBusinessConfiguration“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs windowsUpdateForBusinessConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f1babb06a3a1f897a8abe67a52cbbe46119483c8
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30989211"
---
# <a name="update-windowsupdateforbusinessconfiguration"></a><span data-ttu-id="ccb7a-103">Aktualisieren von „windowsUpdateForBusinessConfiguration“</span><span class="sxs-lookup"><span data-stu-id="ccb7a-103">Update windowsUpdateForBusinessConfiguration</span></span>

> <span data-ttu-id="ccb7a-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ccb7a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ccb7a-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="ccb7a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ccb7a-106">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ccb7a-106">Update the properties of a [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ccb7a-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="ccb7a-107">Prerequisites</span></span>
<span data-ttu-id="ccb7a-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ccb7a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ccb7a-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ccb7a-110">Permission type</span></span>|<span data-ttu-id="ccb7a-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ccb7a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ccb7a-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ccb7a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ccb7a-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ccb7a-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ccb7a-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ccb7a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ccb7a-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ccb7a-115">Not supported.</span></span>|
|<span data-ttu-id="ccb7a-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ccb7a-116">Application</span></span>|<span data-ttu-id="ccb7a-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ccb7a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ccb7a-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ccb7a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="ccb7a-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ccb7a-119">Request headers</span></span>
|<span data-ttu-id="ccb7a-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="ccb7a-120">Header</span></span>|<span data-ttu-id="ccb7a-121">Wert</span><span class="sxs-lookup"><span data-stu-id="ccb7a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ccb7a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ccb7a-122">Authorization</span></span>|<span data-ttu-id="ccb7a-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="ccb7a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ccb7a-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="ccb7a-124">Accept</span></span>|<span data-ttu-id="ccb7a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ccb7a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ccb7a-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ccb7a-126">Request body</span></span>
<span data-ttu-id="ccb7a-127">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) an.</span><span class="sxs-lookup"><span data-stu-id="ccb7a-127">In the request body, supply a JSON representation for the [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object.</span></span>

<span data-ttu-id="ccb7a-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="ccb7a-128">The following table shows the properties that are required when you create the [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md).</span></span>

|<span data-ttu-id="ccb7a-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ccb7a-129">Property</span></span>|<span data-ttu-id="ccb7a-130">Typ</span><span class="sxs-lookup"><span data-stu-id="ccb7a-130">Type</span></span>|<span data-ttu-id="ccb7a-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ccb7a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ccb7a-132">id</span><span class="sxs-lookup"><span data-stu-id="ccb7a-132">id</span></span>|<span data-ttu-id="ccb7a-133">String</span><span class="sxs-lookup"><span data-stu-id="ccb7a-133">String</span></span>|<span data-ttu-id="ccb7a-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="ccb7a-134">Key of the entity.</span></span> <span data-ttu-id="ccb7a-135">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ccb7a-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ccb7a-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ccb7a-136">lastModifiedDateTime</span></span>|<span data-ttu-id="ccb7a-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ccb7a-137">DateTimeOffset</span></span>|<span data-ttu-id="ccb7a-138">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="ccb7a-138">DateTime the object was last modified.</span></span> <span data-ttu-id="ccb7a-139">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ccb7a-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ccb7a-140">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="ccb7a-140">roleScopeTagIds</span></span>|<span data-ttu-id="ccb7a-141">String collection</span><span class="sxs-lookup"><span data-stu-id="ccb7a-141">String collection</span></span>|<span data-ttu-id="ccb7a-142">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="ccb7a-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ccb7a-143">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ccb7a-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ccb7a-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="ccb7a-144">supportsScopeTags</span></span>|<span data-ttu-id="ccb7a-145">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="ccb7a-145">Boolean</span></span>|<span data-ttu-id="ccb7a-146">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereichs Tags unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ccb7a-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="ccb7a-147">Das Zuweisen zur ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert auf false festgelegt ist und Entitäten für bereichsbezogene Benutzer nicht sichtbar sind.</span><span class="sxs-lookup"><span data-stu-id="ccb7a-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="ccb7a-148">Dies geschieht für in Silverlight erstellte Legacy Richtlinien und kann durch Löschen und erneutes Erstellen der Richtlinie im Azure-Portal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="ccb7a-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="ccb7a-149">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="ccb7a-149">This property is read-only.</span></span> <span data-ttu-id="ccb7a-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ccb7a-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ccb7a-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ccb7a-151">createdDateTime</span></span>|<span data-ttu-id="ccb7a-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ccb7a-152">DateTimeOffset</span></span>|<span data-ttu-id="ccb7a-153">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="ccb7a-153">DateTime the object was created.</span></span> <span data-ttu-id="ccb7a-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ccb7a-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ccb7a-155">description</span><span class="sxs-lookup"><span data-stu-id="ccb7a-155">description</span></span>|<span data-ttu-id="ccb7a-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ccb7a-156">String</span></span>|<span data-ttu-id="ccb7a-157">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="ccb7a-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ccb7a-158">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ccb7a-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ccb7a-159">displayName</span><span class="sxs-lookup"><span data-stu-id="ccb7a-159">displayName</span></span>|<span data-ttu-id="ccb7a-160">String</span><span class="sxs-lookup"><span data-stu-id="ccb7a-160">String</span></span>|<span data-ttu-id="ccb7a-161">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="ccb7a-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ccb7a-162">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ccb7a-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ccb7a-163">Version</span><span class="sxs-lookup"><span data-stu-id="ccb7a-163">version</span></span>|<span data-ttu-id="ccb7a-164">Int32</span><span class="sxs-lookup"><span data-stu-id="ccb7a-164">Int32</span></span>|<span data-ttu-id="ccb7a-165">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="ccb7a-165">Version of the device configuration.</span></span> <span data-ttu-id="ccb7a-166">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ccb7a-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ccb7a-167">deliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="ccb7a-167">deliveryOptimizationMode</span></span>|[<span data-ttu-id="ccb7a-168">windowsDeliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="ccb7a-168">windowsDeliveryOptimizationMode</span></span>](../resources/intune-deviceconfig-windowsdeliveryoptimizationmode.md)|<span data-ttu-id="ccb7a-169">Bereitstellungs OptimierungsModus.</span><span class="sxs-lookup"><span data-stu-id="ccb7a-169">Delivery Optimization Mode.</span></span> <span data-ttu-id="ccb7a-170">Mögliche Werte: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.</span><span class="sxs-lookup"><span data-stu-id="ccb7a-170">Possible values are: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.</span></span>|
|<span data-ttu-id="ccb7a-171">prereleaseFeatures</span><span class="sxs-lookup"><span data-stu-id="ccb7a-171">prereleaseFeatures</span></span>|[<span data-ttu-id="ccb7a-172">prereleaseFeatures</span><span class="sxs-lookup"><span data-stu-id="ccb7a-172">prereleaseFeatures</span></span>](../resources/intune-deviceconfig-prereleasefeatures.md)|<span data-ttu-id="ccb7a-173">Pre-Release-Funktionen.</span><span class="sxs-lookup"><span data-stu-id="ccb7a-173">The pre-release features.</span></span> <span data-ttu-id="ccb7a-174">Mögliche Werte sind: `userDefined`, `settingsOnly`, `settingsAndExperimentations` und `notAllowed`.</span><span class="sxs-lookup"><span data-stu-id="ccb7a-174">Possible values are: `userDefined`, `settingsOnly`, `settingsAndExperimentations`, `notAllowed`.</span></span>|
|<span data-ttu-id="ccb7a-175">automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="ccb7a-175">automaticUpdateMode</span></span>|[<span data-ttu-id="ccb7a-176">automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="ccb7a-176">automaticUpdateMode</span></span>](../resources/intune-deviceconfig-automaticupdatemode.md)|<span data-ttu-id="ccb7a-177">Modus für automatische Updates.</span><span class="sxs-lookup"><span data-stu-id="ccb7a-177">Automatic update mode.</span></span> <span data-ttu-id="ccb7a-178">Mögliche Werte: `userDefined`, `notifyDownload`, `autoInstallAtMaintenanceTime`, `autoInstallAndRebootAtMaintenanceTime`, `autoInstallAndRebootAtScheduledTime`, `autoInstallAndRebootWithoutEndUserControl`, `windowsDefault`.</span><span class="sxs-lookup"><span data-stu-id="ccb7a-178">Possible values are: `userDefined`, `notifyDownload`, `autoInstallAtMaintenanceTime`, `autoInstallAndRebootAtMaintenanceTime`, `autoInstallAndRebootAtScheduledTime`, `autoInstallAndRebootWithoutEndUserControl`, `windowsDefault`.</span></span>|
|<span data-ttu-id="ccb7a-179">microsoftUpdateServiceAllowed</span><span class="sxs-lookup"><span data-stu-id="ccb7a-179">microsoftUpdateServiceAllowed</span></span>|<span data-ttu-id="ccb7a-180">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="ccb7a-180">Boolean</span></span>|<span data-ttu-id="ccb7a-181">Legt fest, dass der Microsoft Update Service zugelassen wird.</span><span class="sxs-lookup"><span data-stu-id="ccb7a-181">Allow Microsoft Update Service</span></span>|
|<span data-ttu-id="ccb7a-182">driversExcluded</span><span class="sxs-lookup"><span data-stu-id="ccb7a-182">driversExcluded</span></span>|<span data-ttu-id="ccb7a-183">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="ccb7a-183">Boolean</span></span>|<span data-ttu-id="ccb7a-184">Legt fest, dass Treiber von Windows-Updates ausgenommen werden.</span><span class="sxs-lookup"><span data-stu-id="ccb7a-184">Exclude Windows update Drivers</span></span>|
|<span data-ttu-id="ccb7a-185">installationSchedule</span><span class="sxs-lookup"><span data-stu-id="ccb7a-185">installationSchedule</span></span>|[<span data-ttu-id="ccb7a-186">windowsUpdateInstallScheduleType</span><span class="sxs-lookup"><span data-stu-id="ccb7a-186">windowsUpdateInstallScheduleType</span></span>](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)|<span data-ttu-id="ccb7a-187">Installationszeitplan</span><span class="sxs-lookup"><span data-stu-id="ccb7a-187">Installation schedule</span></span>|
|<span data-ttu-id="ccb7a-188">qualityUpdatesDeferralPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="ccb7a-188">qualityUpdatesDeferralPeriodInDays</span></span>|<span data-ttu-id="ccb7a-189">Int32</span><span class="sxs-lookup"><span data-stu-id="ccb7a-189">Int32</span></span>|<span data-ttu-id="ccb7a-190">Legt fest, um wie viele Tage Qualitätsupdates zurückgestellt werden sollen.</span><span class="sxs-lookup"><span data-stu-id="ccb7a-190">Defer Quality Updates by these many days</span></span>|
|<span data-ttu-id="ccb7a-191">featureUpdatesDeferralPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="ccb7a-191">featureUpdatesDeferralPeriodInDays</span></span>|<span data-ttu-id="ccb7a-192">Int32</span><span class="sxs-lookup"><span data-stu-id="ccb7a-192">Int32</span></span>|<span data-ttu-id="ccb7a-193">Legt fest, um wie viele Tage Funktionsupdates zurückgestellt werden sollen.</span><span class="sxs-lookup"><span data-stu-id="ccb7a-193">Defer Feature Updates by these many days</span></span>|
|<span data-ttu-id="ccb7a-194">qualityUpdatesPaused</span><span class="sxs-lookup"><span data-stu-id="ccb7a-194">qualityUpdatesPaused</span></span>|<span data-ttu-id="ccb7a-195">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="ccb7a-195">Boolean</span></span>|<span data-ttu-id="ccb7a-196">Setzt Qualitätsupdates aus.</span><span class="sxs-lookup"><span data-stu-id="ccb7a-196">Pause Quality Updates</span></span>|
|<span data-ttu-id="ccb7a-197">featureUpdatesPaused</span><span class="sxs-lookup"><span data-stu-id="ccb7a-197">featureUpdatesPaused</span></span>|<span data-ttu-id="ccb7a-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="ccb7a-198">Boolean</span></span>|<span data-ttu-id="ccb7a-199">Setzt Funktionsupdates aus.</span><span class="sxs-lookup"><span data-stu-id="ccb7a-199">Pause Feature Updates</span></span>|
|<span data-ttu-id="ccb7a-200">qualityUpdatesPauseExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="ccb7a-200">qualityUpdatesPauseExpiryDateTime</span></span>|<span data-ttu-id="ccb7a-201">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ccb7a-201">DateTimeOffset</span></span>|<span data-ttu-id="ccb7a-202">Datum und Uhrzeit des Ablaufs der Aussetzung der Qualitätsupdates</span><span class="sxs-lookup"><span data-stu-id="ccb7a-202">Quality Updates Pause Expiry datetime</span></span>|
|<span data-ttu-id="ccb7a-203">featureUpdatesPauseExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="ccb7a-203">featureUpdatesPauseExpiryDateTime</span></span>|<span data-ttu-id="ccb7a-204">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ccb7a-204">DateTimeOffset</span></span>|<span data-ttu-id="ccb7a-205">Datum und Uhrzeit des Ablaufs der Aussetzung der Funktionsupdates</span><span class="sxs-lookup"><span data-stu-id="ccb7a-205">Feature Updates Pause Expiry datetime</span></span>|
|<span data-ttu-id="ccb7a-206">businessReadyUpdatesOnly</span><span class="sxs-lookup"><span data-stu-id="ccb7a-206">businessReadyUpdatesOnly</span></span>|[<span data-ttu-id="ccb7a-207">windowsUpdateType</span><span class="sxs-lookup"><span data-stu-id="ccb7a-207">windowsUpdateType</span></span>](../resources/intune-deviceconfig-windowsupdatetype.md)|<span data-ttu-id="ccb7a-208">Bestimmt, von welchen Zweigstellen die Aktualisierungen empfangen werden.</span><span class="sxs-lookup"><span data-stu-id="ccb7a-208">Determines which branch devices will receive their updates from.</span></span> <span data-ttu-id="ccb7a-209">Mögliche Werte sind: `userDefined`, `all`, `businessReadyOnly`, `windowsInsiderBuildFast`, `windowsInsiderBuildSlow` und `windowsInsiderBuildRelease`.</span><span class="sxs-lookup"><span data-stu-id="ccb7a-209">Possible values are: `userDefined`, `all`, `businessReadyOnly`, `windowsInsiderBuildFast`, `windowsInsiderBuildSlow`, `windowsInsiderBuildRelease`.</span></span>|
|<span data-ttu-id="ccb7a-210">skipChecksBeforeRestart</span><span class="sxs-lookup"><span data-stu-id="ccb7a-210">skipChecksBeforeRestart</span></span>|<span data-ttu-id="ccb7a-211">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="ccb7a-211">Boolean</span></span>|<span data-ttu-id="ccb7a-212">Alle Überprüfung vor Neustart überspringen: Akkustand = 40%, Benutzer Anwesenheit, Anzeige erforderlich, Präsentationsmodus, Vollbildmodus, Telefonanruf Status, Spielmodus usw.</span><span class="sxs-lookup"><span data-stu-id="ccb7a-212">Set to skip all check before restart: Battery level = 40%, User presence, Display Needed, Presentation mode, Full screen mode, phone call state, game mode etc.</span></span> |
|<span data-ttu-id="ccb7a-213">updateWeeks</span><span class="sxs-lookup"><span data-stu-id="ccb7a-213">updateWeeks</span></span>|[<span data-ttu-id="ccb7a-214">windowsUpdateForBusinessUpdateWeeks</span><span class="sxs-lookup"><span data-stu-id="ccb7a-214">windowsUpdateForBusinessUpdateWeeks</span></span>](../resources/intune-deviceconfig-windowsupdateforbusinessupdateweeks.md)|<span data-ttu-id="ccb7a-215">Updateinstallation für die Wochen des Monats geplant.</span><span class="sxs-lookup"><span data-stu-id="ccb7a-215">Scheduled the update installation on the weeks of the month.</span></span> <span data-ttu-id="ccb7a-216">Mögliche Werte sind: `userDefined`, `firstWeek`, `secondWeek`, `thirdWeek`, `fourthWeek` und `everyWeek`.</span><span class="sxs-lookup"><span data-stu-id="ccb7a-216">Possible values are: `userDefined`, `firstWeek`, `secondWeek`, `thirdWeek`, `fourthWeek`, `everyWeek`.</span></span>|
|<span data-ttu-id="ccb7a-217">qualityUpdatesPauseStartDate</span><span class="sxs-lookup"><span data-stu-id="ccb7a-217">qualityUpdatesPauseStartDate</span></span>|<span data-ttu-id="ccb7a-218">Datum</span><span class="sxs-lookup"><span data-stu-id="ccb7a-218">Date</span></span>|<span data-ttu-id="ccb7a-219">Qualitäts Updates unterBrechen das Startdatum.</span><span class="sxs-lookup"><span data-stu-id="ccb7a-219">Quality Updates Pause start date.</span></span> <span data-ttu-id="ccb7a-220">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="ccb7a-220">This property is read-only.</span></span>|
|<span data-ttu-id="ccb7a-221">featureUpdatesPauseStartDate</span><span class="sxs-lookup"><span data-stu-id="ccb7a-221">featureUpdatesPauseStartDate</span></span>|<span data-ttu-id="ccb7a-222">Datum</span><span class="sxs-lookup"><span data-stu-id="ccb7a-222">Date</span></span>|<span data-ttu-id="ccb7a-223">Feature-Updates unterBrechen Startdatum.</span><span class="sxs-lookup"><span data-stu-id="ccb7a-223">Feature Updates Pause start date.</span></span> <span data-ttu-id="ccb7a-224">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="ccb7a-224">This property is read-only.</span></span>|
|<span data-ttu-id="ccb7a-225">featureUpdatesRollbackWindowInDays</span><span class="sxs-lookup"><span data-stu-id="ccb7a-225">featureUpdatesRollbackWindowInDays</span></span>|<span data-ttu-id="ccb7a-226">Int32</span><span class="sxs-lookup"><span data-stu-id="ccb7a-226">Int32</span></span>|<span data-ttu-id="ccb7a-227">Die Anzahl der Tage nach einer Funktions Aktualisierung, für die ein Rollback gültig ist.</span><span class="sxs-lookup"><span data-stu-id="ccb7a-227">The number of days after a Feature Update for which a rollback is valid</span></span>|
|<span data-ttu-id="ccb7a-228">qualityUpdatesWillBeRolledBack</span><span class="sxs-lookup"><span data-stu-id="ccb7a-228">qualityUpdatesWillBeRolledBack</span></span>|<span data-ttu-id="ccb7a-229">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="ccb7a-229">Boolean</span></span>|<span data-ttu-id="ccb7a-230">Gibt an, ob bei der nächsten Geräteüberprüfung Rollback-Qualitäts Aktualisierungen vorgenommen werden.</span><span class="sxs-lookup"><span data-stu-id="ccb7a-230">Specifies whether to rollback Quality Updates on the next device check in</span></span>|
|<span data-ttu-id="ccb7a-231">featureUpdatesWillBeRolledBack</span><span class="sxs-lookup"><span data-stu-id="ccb7a-231">featureUpdatesWillBeRolledBack</span></span>|<span data-ttu-id="ccb7a-232">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="ccb7a-232">Boolean</span></span>|<span data-ttu-id="ccb7a-233">Gibt an, ob Feature-Updates bei der nächsten Geräteüberprüfung zurückgesetzt werden sollen.</span><span class="sxs-lookup"><span data-stu-id="ccb7a-233">Specifies whether to rollback Feature Updates on the next device check in</span></span>|
|<span data-ttu-id="ccb7a-234">qualityUpdatesRollbackStartDateTime</span><span class="sxs-lookup"><span data-stu-id="ccb7a-234">qualityUpdatesRollbackStartDateTime</span></span>|<span data-ttu-id="ccb7a-235">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ccb7a-235">DateTimeOffset</span></span>|<span data-ttu-id="ccb7a-236">Quality Updates Rollback Start DateTime</span><span class="sxs-lookup"><span data-stu-id="ccb7a-236">Quality Updates Rollback Start datetime</span></span>|
|<span data-ttu-id="ccb7a-237">featureUpdatesRollbackStartDateTime</span><span class="sxs-lookup"><span data-stu-id="ccb7a-237">featureUpdatesRollbackStartDateTime</span></span>|<span data-ttu-id="ccb7a-238">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ccb7a-238">DateTimeOffset</span></span>|<span data-ttu-id="ccb7a-239">Feature Updates Rollback Start DateTime</span><span class="sxs-lookup"><span data-stu-id="ccb7a-239">Feature Updates Rollback Start datetime</span></span>|
|<span data-ttu-id="ccb7a-240">engagedRestartDeadlineInDays</span><span class="sxs-lookup"><span data-stu-id="ccb7a-240">engagedRestartDeadlineInDays</span></span>|<span data-ttu-id="ccb7a-241">Int32</span><span class="sxs-lookup"><span data-stu-id="ccb7a-241">Int32</span></span>|<span data-ttu-id="ccb7a-242">Stichtag in Tagen vor automatischer Planung und Ausführung eines ausstehenden Neustarts außerhalb der aktiven Stunden, mit gültigem Bereich zwischen 2 und 30 Tagen</span><span class="sxs-lookup"><span data-stu-id="ccb7a-242">Deadline in days before automatically scheduling and executing a pending restart outside of active hours, with valid range from 2 to 30 days</span></span>|
|<span data-ttu-id="ccb7a-243">engagedRestartSnoozeScheduleInDays</span><span class="sxs-lookup"><span data-stu-id="ccb7a-243">engagedRestartSnoozeScheduleInDays</span></span>|<span data-ttu-id="ccb7a-244">Int32</span><span class="sxs-lookup"><span data-stu-id="ccb7a-244">Int32</span></span>|<span data-ttu-id="ccb7a-245">Anzahl der Tage, die ein Benutzer zum erneuten Verfassen von Benachrichtigungen mit einem gültigen Gültigkeitszeitraum von 1 bis 3 Tagen aufgefordert werden kann.</span><span class="sxs-lookup"><span data-stu-id="ccb7a-245">Number of days a user can snooze Engaged Restart reminder notifications with valid range from 1 to 3 days</span></span>|
|<span data-ttu-id="ccb7a-246">engagedRestartTransitionScheduleInDays</span><span class="sxs-lookup"><span data-stu-id="ccb7a-246">engagedRestartTransitionScheduleInDays</span></span>|<span data-ttu-id="ccb7a-247">Int32</span><span class="sxs-lookup"><span data-stu-id="ccb7a-247">Int32</span></span>|<span data-ttu-id="ccb7a-248">Anzahl der Tage vor dem Übergang von automatischen Neustarts außerhalb der aktiven Stunden zu einem erneuten Neustart, die der Benutzer mit einem gültigen Bereich zwischen 0 und 30 Tagen planen muss.</span><span class="sxs-lookup"><span data-stu-id="ccb7a-248">Number of days before transitioning from Auto Restarts scheduled outside of active hours to Engaged Restart, which requires the user to schedule, with valid range from 0 to 30 days</span></span>|
|<span data-ttu-id="ccb7a-249">autoRestartNotificationDismissal</span><span class="sxs-lookup"><span data-stu-id="ccb7a-249">autoRestartNotificationDismissal</span></span>|[<span data-ttu-id="ccb7a-250">autoRestartNotificationDismissalMethod</span><span class="sxs-lookup"><span data-stu-id="ccb7a-250">autoRestartNotificationDismissalMethod</span></span>](../resources/intune-deviceconfig-autorestartnotificationdismissalmethod.md)|<span data-ttu-id="ccb7a-251">Geben Sie die Methode an, mit der die erforderliche automatische Neustartbenachrichtigung geschlossen wird.</span><span class="sxs-lookup"><span data-stu-id="ccb7a-251">Specify the method by which the auto-restart required notification is dismissed.</span></span> <span data-ttu-id="ccb7a-252">Mögliche Werte sind: `notConfigured`, `automatic` und `user`.</span><span class="sxs-lookup"><span data-stu-id="ccb7a-252">Possible values are: `notConfigured`, `automatic`, `user`.</span></span>|
|<span data-ttu-id="ccb7a-253">scheduleRestartWarningInHours</span><span class="sxs-lookup"><span data-stu-id="ccb7a-253">scheduleRestartWarningInHours</span></span>|<span data-ttu-id="ccb7a-254">Int32</span><span class="sxs-lookup"><span data-stu-id="ccb7a-254">Int32</span></span>|<span data-ttu-id="ccb7a-255">Geben Sie den Zeitraum für Warnbenachrichtigungen für automatische Neustarts an.</span><span class="sxs-lookup"><span data-stu-id="ccb7a-255">Specify the period for auto-restart warning reminder notifications.</span></span> <span data-ttu-id="ccb7a-256">Unterstützte Werte: 2, 4, 8, 12 oder 24 (Stunden).</span><span class="sxs-lookup"><span data-stu-id="ccb7a-256">Supported values: 2, 4, 8, 12 or 24 (hours).</span></span>|
|<span data-ttu-id="ccb7a-257">scheduleImminentRestartWarningInMinutes</span><span class="sxs-lookup"><span data-stu-id="ccb7a-257">scheduleImminentRestartWarningInMinutes</span></span>|<span data-ttu-id="ccb7a-258">Int32</span><span class="sxs-lookup"><span data-stu-id="ccb7a-258">Int32</span></span>|<span data-ttu-id="ccb7a-259">Geben Sie den Zeitraum für den automatischen Neustart unmittelbar bevorstehender Warnbenachrichtigungen an.</span><span class="sxs-lookup"><span data-stu-id="ccb7a-259">Specify the period for auto-restart imminent warning notifications.</span></span> <span data-ttu-id="ccb7a-260">Unterstützte Werte: 15, 30 oder 60 (Minuten).</span><span class="sxs-lookup"><span data-stu-id="ccb7a-260">Supported values: 15, 30 or 60 (minutes).</span></span>|
|<span data-ttu-id="ccb7a-261">userPauseAccess</span><span class="sxs-lookup"><span data-stu-id="ccb7a-261">userPauseAccess</span></span>|[<span data-ttu-id="ccb7a-262">Aktivierung</span><span class="sxs-lookup"><span data-stu-id="ccb7a-262">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="ccb7a-263">Gibt an, ob der Zugriff von Endbenutzern auf Softwareupdates angehalten werden soll.</span><span class="sxs-lookup"><span data-stu-id="ccb7a-263">Specifies whether to enable end user’s access to pause software updates.</span></span> <span data-ttu-id="ccb7a-264">Mögliche Werte sind: `notConfigured`, `enabled` und `disabled`.</span><span class="sxs-lookup"><span data-stu-id="ccb7a-264">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="ccb7a-265">userWindowsUpdateScanAccess</span><span class="sxs-lookup"><span data-stu-id="ccb7a-265">userWindowsUpdateScanAccess</span></span>|[<span data-ttu-id="ccb7a-266">Aktivierung</span><span class="sxs-lookup"><span data-stu-id="ccb7a-266">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="ccb7a-267">Gibt an, ob der Benutzer Zugriff zum Überprüfen von Windows Update deaktiviert werden soll.</span><span class="sxs-lookup"><span data-stu-id="ccb7a-267">Specifies whether to disable user’s access to scan Windows Update.</span></span> <span data-ttu-id="ccb7a-268">Mögliche Werte sind: `notConfigured`, `enabled` und `disabled`.</span><span class="sxs-lookup"><span data-stu-id="ccb7a-268">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="ccb7a-269">updateNotificationLevel</span><span class="sxs-lookup"><span data-stu-id="ccb7a-269">updateNotificationLevel</span></span>|[<span data-ttu-id="ccb7a-270">windowsUpdateNotificationDisplayOption</span><span class="sxs-lookup"><span data-stu-id="ccb7a-270">windowsUpdateNotificationDisplayOption</span></span>](../resources/intune-deviceconfig-windowsupdatenotificationdisplayoption.md)|<span data-ttu-id="ccb7a-271">Gibt an, welche Windows Update-Benachrichtigungen angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="ccb7a-271">Specifies what Windows Update notifications users see.</span></span> <span data-ttu-id="ccb7a-272">Mögliche Werte sind: `notConfigured`, `defaultNotifications`, `restartWarningsOnly` und `disableAllNotifications`.</span><span class="sxs-lookup"><span data-stu-id="ccb7a-272">Possible values are: `notConfigured`, `defaultNotifications`, `restartWarningsOnly`, `disableAllNotifications`.</span></span>|



## <a name="response"></a><span data-ttu-id="ccb7a-273">Antwort</span><span class="sxs-lookup"><span data-stu-id="ccb7a-273">Response</span></span>
<span data-ttu-id="ccb7a-274">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="ccb7a-274">If successful, this method returns a `200 OK` response code and an updated [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ccb7a-275">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ccb7a-275">Example</span></span>

### <a name="request"></a><span data-ttu-id="ccb7a-276">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ccb7a-276">Request</span></span>
<span data-ttu-id="ccb7a-277">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ccb7a-277">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1903

{
  "@odata.type": "#microsoft.graph.windowsUpdateForBusinessConfiguration",
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
  "qualityUpdatesPauseStartDate": "<Unknown Primitive Type Edm.Date>",
  "featureUpdatesPauseStartDate": "<Unknown Primitive Type Edm.Date>",
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
  "scheduleImminentRestartWarningInMinutes": 7,
  "userPauseAccess": "enabled",
  "userWindowsUpdateScanAccess": "enabled",
  "updateNotificationLevel": "defaultNotifications"
}
```

### <a name="response"></a><span data-ttu-id="ccb7a-278">Antwort</span><span class="sxs-lookup"><span data-stu-id="ccb7a-278">Response</span></span>
<span data-ttu-id="ccb7a-p123">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ccb7a-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2075

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
  "qualityUpdatesPauseStartDate": "<Unknown Primitive Type Edm.Date>",
  "featureUpdatesPauseStartDate": "<Unknown Primitive Type Edm.Date>",
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
  "scheduleImminentRestartWarningInMinutes": 7,
  "userPauseAccess": "enabled",
  "userWindowsUpdateScanAccess": "enabled",
  "updateNotificationLevel": "defaultNotifications"
}
```




