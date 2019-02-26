---
title: WindowsDeliveryOptimizationConfiguration erstellen
description: Erstellen eines neuen windowsDeliveryOptimizationConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ca26c05cb9d24563534b0abf48bf663cecebfcdd
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30139809"
---
# <a name="create-windowsdeliveryoptimizationconfiguration"></a><span data-ttu-id="1ce98-103">WindowsDeliveryOptimizationConfiguration erstellen</span><span class="sxs-lookup"><span data-stu-id="1ce98-103">Create windowsDeliveryOptimizationConfiguration</span></span>

> <span data-ttu-id="1ce98-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1ce98-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1ce98-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="1ce98-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1ce98-106">Erstellen eines neuen [windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="1ce98-106">Create a new [windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1ce98-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="1ce98-107">Prerequisites</span></span>
<span data-ttu-id="1ce98-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="1ce98-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="1ce98-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1ce98-110">Permission type</span></span>|<span data-ttu-id="1ce98-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1ce98-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1ce98-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1ce98-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1ce98-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1ce98-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1ce98-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1ce98-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1ce98-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1ce98-115">Not supported.</span></span>|
|<span data-ttu-id="1ce98-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1ce98-116">Application</span></span>|<span data-ttu-id="1ce98-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1ce98-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1ce98-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1ce98-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="1ce98-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1ce98-119">Request headers</span></span>
|<span data-ttu-id="1ce98-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="1ce98-120">Header</span></span>|<span data-ttu-id="1ce98-121">Wert</span><span class="sxs-lookup"><span data-stu-id="1ce98-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1ce98-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1ce98-122">Authorization</span></span>|<span data-ttu-id="1ce98-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="1ce98-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1ce98-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="1ce98-124">Accept</span></span>|<span data-ttu-id="1ce98-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1ce98-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1ce98-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1ce98-126">Request body</span></span>
<span data-ttu-id="1ce98-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das windowsDeliveryOptimizationConfiguration-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="1ce98-127">In the request body, supply a JSON representation for the windowsDeliveryOptimizationConfiguration object.</span></span>

<span data-ttu-id="1ce98-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der windowsDeliveryOptimizationConfiguration erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="1ce98-128">The following table shows the properties that are required when you create the windowsDeliveryOptimizationConfiguration.</span></span>

|<span data-ttu-id="1ce98-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1ce98-129">Property</span></span>|<span data-ttu-id="1ce98-130">Typ</span><span class="sxs-lookup"><span data-stu-id="1ce98-130">Type</span></span>|<span data-ttu-id="1ce98-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1ce98-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1ce98-132">id</span><span class="sxs-lookup"><span data-stu-id="1ce98-132">id</span></span>|<span data-ttu-id="1ce98-133">string</span><span class="sxs-lookup"><span data-stu-id="1ce98-133">String</span></span>|<span data-ttu-id="1ce98-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="1ce98-134">Key of the entity.</span></span> <span data-ttu-id="1ce98-135">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1ce98-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1ce98-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1ce98-136">lastModifiedDateTime</span></span>|<span data-ttu-id="1ce98-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1ce98-137">DateTimeOffset</span></span>|<span data-ttu-id="1ce98-138">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="1ce98-138">DateTime the object was last modified.</span></span> <span data-ttu-id="1ce98-139">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1ce98-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1ce98-140">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="1ce98-140">roleScopeTagIds</span></span>|<span data-ttu-id="1ce98-141">String collection</span><span class="sxs-lookup"><span data-stu-id="1ce98-141">String collection</span></span>|<span data-ttu-id="1ce98-142">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="1ce98-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="1ce98-143">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1ce98-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1ce98-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="1ce98-144">supportsScopeTags</span></span>|<span data-ttu-id="1ce98-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="1ce98-145">Boolean</span></span>|<span data-ttu-id="1ce98-146">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereichs Tags unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1ce98-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="1ce98-147">Das Zuweisen zur ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert auf false festgelegt ist und Entitäten für bereichsbezogene Benutzer nicht sichtbar sind.</span><span class="sxs-lookup"><span data-stu-id="1ce98-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="1ce98-148">Dies geschieht für in Silverlight erstellte Legacy Richtlinien und kann durch Löschen und erneutes Erstellen der Richtlinie im Azure-Portal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="1ce98-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="1ce98-149">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="1ce98-149">This property is read-only.</span></span> <span data-ttu-id="1ce98-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1ce98-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1ce98-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1ce98-151">createdDateTime</span></span>|<span data-ttu-id="1ce98-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1ce98-152">DateTimeOffset</span></span>|<span data-ttu-id="1ce98-153">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="1ce98-153">DateTime the object was created.</span></span> <span data-ttu-id="1ce98-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1ce98-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1ce98-155">description</span><span class="sxs-lookup"><span data-stu-id="1ce98-155">description</span></span>|<span data-ttu-id="1ce98-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1ce98-156">String</span></span>|<span data-ttu-id="1ce98-157">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="1ce98-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="1ce98-158">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1ce98-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1ce98-159">displayName</span><span class="sxs-lookup"><span data-stu-id="1ce98-159">displayName</span></span>|<span data-ttu-id="1ce98-160">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1ce98-160">String</span></span>|<span data-ttu-id="1ce98-161">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="1ce98-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="1ce98-162">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1ce98-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1ce98-163">Version</span><span class="sxs-lookup"><span data-stu-id="1ce98-163">version</span></span>|<span data-ttu-id="1ce98-164">Int32</span><span class="sxs-lookup"><span data-stu-id="1ce98-164">Int32</span></span>|<span data-ttu-id="1ce98-165">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="1ce98-165">Version of the device configuration.</span></span> <span data-ttu-id="1ce98-166">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1ce98-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1ce98-167">deliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="1ce98-167">deliveryOptimizationMode</span></span>|[<span data-ttu-id="1ce98-168">windowsDeliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="1ce98-168">windowsDeliveryOptimizationMode</span></span>](../resources/intune-deviceconfig-windowsdeliveryoptimizationmode.md)|<span data-ttu-id="1ce98-169">Gibt die Downloadmethode an, die von der Zustellungsoptimierung zur Verwaltung der Netzwerkbandbreite bei umfangreichen Inhalts Verteilungsszenarien verwendet werden kann.</span><span class="sxs-lookup"><span data-stu-id="1ce98-169">Specifies the download method that delivery optimization can use to manage network bandwidth consumption for large content distribution scenarios.</span></span> <span data-ttu-id="1ce98-170">Mögliche Werte sind: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload` und `bypassMode`.</span><span class="sxs-lookup"><span data-stu-id="1ce98-170">Possible values are: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.</span></span>|
|<span data-ttu-id="1ce98-171">restrictPeerSelectionBy</span><span class="sxs-lookup"><span data-stu-id="1ce98-171">restrictPeerSelectionBy</span></span>|[<span data-ttu-id="1ce98-172">deliveryOptimizationRestrictPeerSelectionByOptions</span><span class="sxs-lookup"><span data-stu-id="1ce98-172">deliveryOptimizationRestrictPeerSelectionByOptions</span></span>](../resources/intune-deviceconfig-deliveryoptimizationrestrictpeerselectionbyoptions.md)|<span data-ttu-id="1ce98-173">Gibt an, dass die Peer Auswahl über die ausgewählte Option eingeschränkt werden soll.</span><span class="sxs-lookup"><span data-stu-id="1ce98-173">Specifies to restrict peer selection via selected option.</span></span>
<span data-ttu-id="1ce98-174">Option 1 (subNetzmaske) gilt nur für die Bereitstellungs Optimierungs Modi Download Modus LAN (1) und Gruppe (2).</span><span class="sxs-lookup"><span data-stu-id="1ce98-174">Option 1 (Subnet mask) only applies to Delivery Optimization modes Download Mode LAN (1) and Group (2).</span></span> <span data-ttu-id="1ce98-175">Mögliche Werte sind: `notConfigured` und `subnetMask`.</span><span class="sxs-lookup"><span data-stu-id="1ce98-175">Possible values are: `notConfigured`, `subnetMask`.</span></span>|
|<span data-ttu-id="1ce98-176">groupIdSource</span><span class="sxs-lookup"><span data-stu-id="1ce98-176">groupIdSource</span></span>|[<span data-ttu-id="1ce98-177">deliveryOptimizationGroupIdSource</span><span class="sxs-lookup"><span data-stu-id="1ce98-177">deliveryOptimizationGroupIdSource</span></span>](../resources/intune-deviceconfig-deliveryoptimizationgroupidsource.md)|<span data-ttu-id="1ce98-178">Gibt an, dass die Peer Auswahl auf eine Specfic-Quelle beschränkt werden soll.</span><span class="sxs-lookup"><span data-stu-id="1ce98-178">Specifies to restrict peer selection to a specfic source.</span></span>
<span data-ttu-id="1ce98-179">Die in dieser Richtlinie festgelegten Optionen gelten nur für den Downloadmodus für den Bereitstellungs Optimierungsmodus (2).</span><span class="sxs-lookup"><span data-stu-id="1ce98-179">The options set in this policy only apply to Delivery Optimization mode Group (2) download mode.</span></span> <span data-ttu-id="1ce98-180">Wenn die Gruppe (2) nicht als Download Modus festgelegt ist, wird diese Richtlinie ignoriert.</span><span class="sxs-lookup"><span data-stu-id="1ce98-180">If Group (2) isn't set as Download mode, this policy will be ignored.</span></span> <span data-ttu-id="1ce98-181">Bei Option 3-DHCP-Options-ID fragt der Client die DHCP-Optionskennung 234 ab und verwendet den zurückgegebenen GUID-Wert als Gruppen-ID.</span><span class="sxs-lookup"><span data-stu-id="1ce98-181">For option 3 - DHCP Option ID, the client will query DHCP Option ID 234 and use the returned GUID value as the Group ID.</span></span>|
|<span data-ttu-id="1ce98-182">bandwidthMode</span><span class="sxs-lookup"><span data-stu-id="1ce98-182">bandwidthMode</span></span>|[<span data-ttu-id="1ce98-183">deliveryOptimizationBandwidth</span><span class="sxs-lookup"><span data-stu-id="1ce98-183">deliveryOptimizationBandwidth</span></span>](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)|<span data-ttu-id="1ce98-184">Gibt die Nutzung von Vordergrund-und Hintergrund Bandbreite unter Verwendung von Prozentsätzen, absoluten Werten oder Stunden an.</span><span class="sxs-lookup"><span data-stu-id="1ce98-184">Specifies foreground and background bandwidth usage using percentages, absolutes, or hours.</span></span>|
|<span data-ttu-id="1ce98-185">backgroundDownloadFromHttpDelayInSeconds</span><span class="sxs-lookup"><span data-stu-id="1ce98-185">backgroundDownloadFromHttpDelayInSeconds</span></span>|<span data-ttu-id="1ce98-186">Int64</span><span class="sxs-lookup"><span data-stu-id="1ce98-186">Int64</span></span>|<span data-ttu-id="1ce98-187">Gibt die Anzahl der Sekunden an, die eine HTTP-Quelle in einem Hintergrund Download verzögert werden soll, der die Verwendung von Peer-to-Peer ermöglicht.</span><span class="sxs-lookup"><span data-stu-id="1ce98-187">Specifies number of seconds to delay an HTTP source in a background download that is allowed to use peer-to-peer.</span></span> <span data-ttu-id="1ce98-188">Gültige Werte 0 bis 4294967295</span><span class="sxs-lookup"><span data-stu-id="1ce98-188">Valid values 0 to 4294967295</span></span>|
|<span data-ttu-id="1ce98-189">foregroundDownloadFromHttpDelayInSeconds</span><span class="sxs-lookup"><span data-stu-id="1ce98-189">foregroundDownloadFromHttpDelayInSeconds</span></span>|<span data-ttu-id="1ce98-190">Int64</span><span class="sxs-lookup"><span data-stu-id="1ce98-190">Int64</span></span>|<span data-ttu-id="1ce98-191">Gibt die Anzahl von Sekunden an, die eine HTTP-Quelle in einem Vordergrund heruntergeladen wird, für die Peer-to-Peer (0-86400) verwendet werden darf.</span><span class="sxs-lookup"><span data-stu-id="1ce98-191">Specifies number of seconds to delay an HTTP source in a foreground download that is allowed to use peer-to-peer (0-86400).</span></span> <span data-ttu-id="1ce98-192">Gültige Werte 0 bis 86400</span><span class="sxs-lookup"><span data-stu-id="1ce98-192">Valid values 0 to 86400</span></span>
<span data-ttu-id="1ce98-193">Durch Angeben von 0 wird die zuStellungsOptimierung zum Verwalten dieser Einstellung mithilfe des Cloud-Diensts festgelegt.</span><span class="sxs-lookup"><span data-stu-id="1ce98-193">Specifying 0 sets Delivery Optimization to manage this setting using the cloud service.</span></span> <span data-ttu-id="1ce98-194">Gültige Werte 0 bis 86400</span><span class="sxs-lookup"><span data-stu-id="1ce98-194">Valid values 0 to 86400</span></span>|
|<span data-ttu-id="1ce98-195">minimumRamAllowedToPeerInGigabytes</span><span class="sxs-lookup"><span data-stu-id="1ce98-195">minimumRamAllowedToPeerInGigabytes</span></span>|<span data-ttu-id="1ce98-196">Int32</span><span class="sxs-lookup"><span data-stu-id="1ce98-196">Int32</span></span>|<span data-ttu-id="1ce98-197">Gibt die minimale RAM-Größe in GB an, um die Peer Zwischenspeicherung zu verwenden (1-100000).</span><span class="sxs-lookup"><span data-stu-id="1ce98-197">Specifies the minimum RAM size in GB to use Peer Caching (1-100000).</span></span> <span data-ttu-id="1ce98-198">Gültige Werte 1 bis 100000</span><span class="sxs-lookup"><span data-stu-id="1ce98-198">Valid values 1 to 100000</span></span>|
|<span data-ttu-id="1ce98-199">minimumDiskSizeAllowedToPeerInGigabytes</span><span class="sxs-lookup"><span data-stu-id="1ce98-199">minimumDiskSizeAllowedToPeerInGigabytes</span></span>|<span data-ttu-id="1ce98-200">Int32</span><span class="sxs-lookup"><span data-stu-id="1ce98-200">Int32</span></span>|<span data-ttu-id="1ce98-201">Gibt die minimale Datenträgergröße in GB für die Verwendung der Peer Zwischenspeicherung an (1-100000).</span><span class="sxs-lookup"><span data-stu-id="1ce98-201">Specifies the minimum disk size in GB to use Peer Caching (1-100000).</span></span> <span data-ttu-id="1ce98-202">Gültige Werte 1 bis 100000</span><span class="sxs-lookup"><span data-stu-id="1ce98-202">Valid values 1 to 100000</span></span>
<span data-ttu-id="1ce98-203">Empfohlene Werte: 64 GB bis 256 GB.</span><span class="sxs-lookup"><span data-stu-id="1ce98-203">Recommended values: 64 GB to 256 GB.</span></span> <span data-ttu-id="1ce98-204">Gültige Werte 1 bis 100000</span><span class="sxs-lookup"><span data-stu-id="1ce98-204">Valid values 1 to 100000</span></span>|
|<span data-ttu-id="1ce98-205">minimumFileSizeToCacheInMegabytes</span><span class="sxs-lookup"><span data-stu-id="1ce98-205">minimumFileSizeToCacheInMegabytes</span></span>|<span data-ttu-id="1ce98-206">Int32</span><span class="sxs-lookup"><span data-stu-id="1ce98-206">Int32</span></span>|<span data-ttu-id="1ce98-207">Gibt die minimale Größe der Inhaltsdatei in MB an, die für die Verwendung der Peer Zwischenspeicherung aktiviert ist (1-100000).</span><span class="sxs-lookup"><span data-stu-id="1ce98-207">Specifies the minimum content file size in MB enabled to use Peer Caching (1-100000).</span></span> <span data-ttu-id="1ce98-208">Gültige Werte 1 bis 100000</span><span class="sxs-lookup"><span data-stu-id="1ce98-208">Valid values 1 to 100000</span></span>
<span data-ttu-id="1ce98-209">Empfohlene Werte: 1 MB bis 100.000 MB.</span><span class="sxs-lookup"><span data-stu-id="1ce98-209">Recommended values: 1 MB to 100,000 MB.</span></span> <span data-ttu-id="1ce98-210">Gültige Werte 1 bis 100000</span><span class="sxs-lookup"><span data-stu-id="1ce98-210">Valid values 1 to 100000</span></span>|
|<span data-ttu-id="1ce98-211">minimumBatteryPercentageAllowedToUpload</span><span class="sxs-lookup"><span data-stu-id="1ce98-211">minimumBatteryPercentageAllowedToUpload</span></span>|<span data-ttu-id="1ce98-212">Int32</span><span class="sxs-lookup"><span data-stu-id="1ce98-212">Int32</span></span>|<span data-ttu-id="1ce98-213">Gibt den Mindestprozentsatz für die Batterie an, damit das Gerät Daten hochladen kann (0-100).</span><span class="sxs-lookup"><span data-stu-id="1ce98-213">Specifies the minimum battery percentage to allow the device to upload data (0-100).</span></span> <span data-ttu-id="1ce98-214">Gültige Werte: 0 bis 100.</span><span class="sxs-lookup"><span data-stu-id="1ce98-214">Valid values 0 to 100</span></span>
<span data-ttu-id="1ce98-215">Der Standardwert ist 0.</span><span class="sxs-lookup"><span data-stu-id="1ce98-215">The default value is 0.</span></span> <span data-ttu-id="1ce98-216">Der Wert 0 (null) ist "unbegrenzt" und der Standardwert des Cloud-Diensts wird verwendet.</span><span class="sxs-lookup"><span data-stu-id="1ce98-216">The value 0 (zero) means "not limited" and the cloud service default value will be used.</span></span> <span data-ttu-id="1ce98-217">Gültige Werte: 0 bis 100.</span><span class="sxs-lookup"><span data-stu-id="1ce98-217">Valid values 0 to 100</span></span>|
|<span data-ttu-id="1ce98-218">modifyCacheLocation</span><span class="sxs-lookup"><span data-stu-id="1ce98-218">modifyCacheLocation</span></span>|<span data-ttu-id="1ce98-219">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1ce98-219">String</span></span>|<span data-ttu-id="1ce98-220">Gibt das Laufwerk an, das von der BereitstellungsOptimierung für den Cache verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="1ce98-220">Specifies the drive that Delivery Optimization should use for its cache.</span></span>|
|<span data-ttu-id="1ce98-221">maximumCacheAgeInDays</span><span class="sxs-lookup"><span data-stu-id="1ce98-221">maximumCacheAgeInDays</span></span>|<span data-ttu-id="1ce98-222">Int32</span><span class="sxs-lookup"><span data-stu-id="1ce98-222">Int32</span></span>|<span data-ttu-id="1ce98-223">Gibt die maximale Zeitdauer in Tagen an, die jede Datei im Bereitstellungs Optimierungs Cache aufbewahrt wird, nachdem Sie erfolgreich heruntergeladen wurde (0-49710).</span><span class="sxs-lookup"><span data-stu-id="1ce98-223">Specifies the maximum time in days that each file is held in the Delivery Optimization cache after downloading successfully (0-49710).</span></span> <span data-ttu-id="1ce98-224">Gültige Werte 0 bis 49710</span><span class="sxs-lookup"><span data-stu-id="1ce98-224">Valid values 0 to 49710</span></span>|
|<span data-ttu-id="1ce98-225">maximumCacheSize</span><span class="sxs-lookup"><span data-stu-id="1ce98-225">maximumCacheSize</span></span>|[<span data-ttu-id="1ce98-226">deliveryOptimizationMaxCacheSize</span><span class="sxs-lookup"><span data-stu-id="1ce98-226">deliveryOptimizationMaxCacheSize</span></span>](../resources/intune-deviceconfig-deliveryoptimizationmaxcachesize.md)|<span data-ttu-id="1ce98-227">Gibt die maximale Cachegröße an, die von der zugestellten Optimierung als Prozentsatz oder in GB angegeben wird.</span><span class="sxs-lookup"><span data-stu-id="1ce98-227">Specifies the maximum cache size that Delivery Optimization either as a percentage or in GB.</span></span>|
|<span data-ttu-id="1ce98-228">vpnPeerCaching</span><span class="sxs-lookup"><span data-stu-id="1ce98-228">vpnPeerCaching</span></span>|[<span data-ttu-id="1ce98-229">Aktivierung</span><span class="sxs-lookup"><span data-stu-id="1ce98-229">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="1ce98-230">Gibt an, ob das Gerät an Peer-Zwischenspeicherung während der Verbindung über VPN mit dem Domänennetzwerk teilnehmen darf.</span><span class="sxs-lookup"><span data-stu-id="1ce98-230">Specifies whether the device is allowed to participate in Peer Caching while connected via VPN to the domain network.</span></span> <span data-ttu-id="1ce98-231">Mögliche Werte sind: `notConfigured`, `enabled` und `disabled`.</span><span class="sxs-lookup"><span data-stu-id="1ce98-231">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|



## <a name="response"></a><span data-ttu-id="1ce98-232">Antwort</span><span class="sxs-lookup"><span data-stu-id="1ce98-232">Response</span></span>
<span data-ttu-id="1ce98-233">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="1ce98-233">If successful, this method returns a `201 Created` response code and a [windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1ce98-234">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1ce98-234">Example</span></span>

### <a name="request"></a><span data-ttu-id="1ce98-235">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1ce98-235">Request</span></span>
<span data-ttu-id="1ce98-236">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1ce98-236">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1060

{
  "@odata.type": "#microsoft.graph.windowsDeliveryOptimizationConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "deliveryOptimizationMode": "httpOnly",
  "restrictPeerSelectionBy": "subnetMask",
  "groupIdSource": {
    "@odata.type": "microsoft.graph.deliveryOptimizationGroupIdSource"
  },
  "bandwidthMode": {
    "@odata.type": "microsoft.graph.deliveryOptimizationBandwidth"
  },
  "backgroundDownloadFromHttpDelayInSeconds": 8,
  "foregroundDownloadFromHttpDelayInSeconds": 8,
  "minimumRamAllowedToPeerInGigabytes": 2,
  "minimumDiskSizeAllowedToPeerInGigabytes": 7,
  "minimumFileSizeToCacheInMegabytes": 1,
  "minimumBatteryPercentageAllowedToUpload": 7,
  "modifyCacheLocation": "Modify Cache Location value",
  "maximumCacheAgeInDays": 5,
  "maximumCacheSize": {
    "@odata.type": "microsoft.graph.deliveryOptimizationMaxCacheSize"
  },
  "vpnPeerCaching": "enabled"
}
```

### <a name="response"></a><span data-ttu-id="1ce98-237">Antwort</span><span class="sxs-lookup"><span data-stu-id="1ce98-237">Response</span></span>
<span data-ttu-id="1ce98-p125">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1ce98-p125">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1232

{
  "@odata.type": "#microsoft.graph.windowsDeliveryOptimizationConfiguration",
  "id": "5954ee9b-ee9b-5954-9bee-54599bee5459",
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
  "restrictPeerSelectionBy": "subnetMask",
  "groupIdSource": {
    "@odata.type": "microsoft.graph.deliveryOptimizationGroupIdSource"
  },
  "bandwidthMode": {
    "@odata.type": "microsoft.graph.deliveryOptimizationBandwidth"
  },
  "backgroundDownloadFromHttpDelayInSeconds": 8,
  "foregroundDownloadFromHttpDelayInSeconds": 8,
  "minimumRamAllowedToPeerInGigabytes": 2,
  "minimumDiskSizeAllowedToPeerInGigabytes": 7,
  "minimumFileSizeToCacheInMegabytes": 1,
  "minimumBatteryPercentageAllowedToUpload": 7,
  "modifyCacheLocation": "Modify Cache Location value",
  "maximumCacheAgeInDays": 5,
  "maximumCacheSize": {
    "@odata.type": "microsoft.graph.deliveryOptimizationMaxCacheSize"
  },
  "vpnPeerCaching": "enabled"
}
```




