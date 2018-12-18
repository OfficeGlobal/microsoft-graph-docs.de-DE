---
title: WindowsWifiConfiguration aktualisieren
description: Aktualisieren Sie die Eigenschaften eines WindowsWifiConfiguration-Objekts.
author: tfitzmac
ms.openlocfilehash: 0cd1d8ba372daf63561bf94763994fedafb24f46
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27310283"
---
# <a name="update-windowswificonfiguration"></a><span data-ttu-id="b01b1-103">WindowsWifiConfiguration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="b01b1-103">Update windowsWifiConfiguration</span></span>

> <span data-ttu-id="b01b1-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b01b1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b01b1-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b01b1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b01b1-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="b01b1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b01b1-107">Aktualisieren Sie die Eigenschaften eines [WindowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="b01b1-107">Update the properties of a [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b01b1-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b01b1-108">Prerequisites</span></span>
<span data-ttu-id="b01b1-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b01b1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b01b1-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b01b1-111">Permission type</span></span>|<span data-ttu-id="b01b1-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b01b1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b01b1-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b01b1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b01b1-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b01b1-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b01b1-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b01b1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b01b1-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b01b1-116">Not supported.</span></span>|
|<span data-ttu-id="b01b1-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b01b1-117">Application</span></span>|<span data-ttu-id="b01b1-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b01b1-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b01b1-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b01b1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="b01b1-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b01b1-120">Request headers</span></span>
|<span data-ttu-id="b01b1-121">Header</span><span class="sxs-lookup"><span data-stu-id="b01b1-121">Header</span></span>|<span data-ttu-id="b01b1-122">Wert</span><span class="sxs-lookup"><span data-stu-id="b01b1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b01b1-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="b01b1-123">Authorization</span></span>|<span data-ttu-id="b01b1-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b01b1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b01b1-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b01b1-125">Accept</span></span>|<span data-ttu-id="b01b1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b01b1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b01b1-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b01b1-127">Request body</span></span>
<span data-ttu-id="b01b1-128">Geben Sie im Textkörper Anforderung für das Objekt [WindowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="b01b1-128">In the request body, supply a JSON representation for the [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) object.</span></span>

<span data-ttu-id="b01b1-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [WindowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="b01b1-129">The following table shows the properties that are required when you create the [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span></span>

|<span data-ttu-id="b01b1-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b01b1-130">Property</span></span>|<span data-ttu-id="b01b1-131">Typ</span><span class="sxs-lookup"><span data-stu-id="b01b1-131">Type</span></span>|<span data-ttu-id="b01b1-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b01b1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b01b1-133">id</span><span class="sxs-lookup"><span data-stu-id="b01b1-133">id</span></span>|<span data-ttu-id="b01b1-134">String</span><span class="sxs-lookup"><span data-stu-id="b01b1-134">String</span></span>|<span data-ttu-id="b01b1-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="b01b1-135">Key of the entity.</span></span> <span data-ttu-id="b01b1-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b01b1-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b01b1-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b01b1-137">lastModifiedDateTime</span></span>|<span data-ttu-id="b01b1-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b01b1-138">DateTimeOffset</span></span>|<span data-ttu-id="b01b1-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="b01b1-139">DateTime the object was last modified.</span></span> <span data-ttu-id="b01b1-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b01b1-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b01b1-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b01b1-141">roleScopeTagIds</span></span>|<span data-ttu-id="b01b1-142">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="b01b1-142">String collection</span></span>|<span data-ttu-id="b01b1-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="b01b1-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b01b1-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b01b1-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b01b1-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="b01b1-145">supportsScopeTags</span></span>|<span data-ttu-id="b01b1-146">Boolesch</span><span class="sxs-lookup"><span data-stu-id="b01b1-146">Boolean</span></span>|<span data-ttu-id="b01b1-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b01b1-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="b01b1-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="b01b1-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="b01b1-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="b01b1-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="b01b1-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="b01b1-150">This property is read-only.</span></span> <span data-ttu-id="b01b1-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b01b1-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b01b1-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b01b1-152">createdDateTime</span></span>|<span data-ttu-id="b01b1-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b01b1-153">DateTimeOffset</span></span>|<span data-ttu-id="b01b1-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="b01b1-154">DateTime the object was created.</span></span> <span data-ttu-id="b01b1-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b01b1-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b01b1-156">description</span><span class="sxs-lookup"><span data-stu-id="b01b1-156">description</span></span>|<span data-ttu-id="b01b1-157">String</span><span class="sxs-lookup"><span data-stu-id="b01b1-157">String</span></span>|<span data-ttu-id="b01b1-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="b01b1-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b01b1-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b01b1-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b01b1-160">displayName</span><span class="sxs-lookup"><span data-stu-id="b01b1-160">displayName</span></span>|<span data-ttu-id="b01b1-161">String</span><span class="sxs-lookup"><span data-stu-id="b01b1-161">String</span></span>|<span data-ttu-id="b01b1-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="b01b1-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b01b1-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b01b1-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b01b1-164">Version</span><span class="sxs-lookup"><span data-stu-id="b01b1-164">version</span></span>|<span data-ttu-id="b01b1-165">Int32</span><span class="sxs-lookup"><span data-stu-id="b01b1-165">Int32</span></span>|<span data-ttu-id="b01b1-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="b01b1-166">Version of the device configuration.</span></span> <span data-ttu-id="b01b1-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b01b1-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b01b1-168">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="b01b1-168">preSharedKey</span></span>|<span data-ttu-id="b01b1-169">String</span><span class="sxs-lookup"><span data-stu-id="b01b1-169">String</span></span>|<span data-ttu-id="b01b1-170">Dies ist die vorinstallierten Schlüssel für WPA persönliche Wi-Fi-Netzwerk.</span><span class="sxs-lookup"><span data-stu-id="b01b1-170">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span>|
|<span data-ttu-id="b01b1-171">wifiSecurityType</span><span class="sxs-lookup"><span data-stu-id="b01b1-171">wifiSecurityType</span></span>|[<span data-ttu-id="b01b1-172">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="b01b1-172">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="b01b1-173">Den Sicherheitstyp Wifi angeben.</span><span class="sxs-lookup"><span data-stu-id="b01b1-173">Specify the Wifi Security Type.</span></span> <span data-ttu-id="b01b1-174">Mögliche Werte sind: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal` und `wpa2Enterprise`.</span><span class="sxs-lookup"><span data-stu-id="b01b1-174">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="b01b1-175">meteredConnectionLimit</span><span class="sxs-lookup"><span data-stu-id="b01b1-175">meteredConnectionLimit</span></span>|[<span data-ttu-id="b01b1-176">meteredConnectionLimitType</span><span class="sxs-lookup"><span data-stu-id="b01b1-176">meteredConnectionLimitType</span></span>](../resources/intune-deviceconfig-meteredconnectionlimittype.md)|<span data-ttu-id="b01b1-177">Geben Sie den gemessenen Verbindungstyp des Grenzwert für die WLAN-Verbindung.</span><span class="sxs-lookup"><span data-stu-id="b01b1-177">Specify the metered connection limit type for the wifi connection.</span></span> <span data-ttu-id="b01b1-178">Mögliche Werte sind: `unrestricted`, `fixed` und `variable`.</span><span class="sxs-lookup"><span data-stu-id="b01b1-178">Possible values are: `unrestricted`, `fixed`, `variable`.</span></span>|
|<span data-ttu-id="b01b1-179">SSID</span><span class="sxs-lookup"><span data-stu-id="b01b1-179">ssid</span></span>|<span data-ttu-id="b01b1-180">String</span><span class="sxs-lookup"><span data-stu-id="b01b1-180">String</span></span>|<span data-ttu-id="b01b1-181">Geben Sie die SSID des WLAN-Verbindung.</span><span class="sxs-lookup"><span data-stu-id="b01b1-181">Specify the SSID of the wifi connection.</span></span>|
|<span data-ttu-id="b01b1-182">Netzwerkname</span><span class="sxs-lookup"><span data-stu-id="b01b1-182">networkName</span></span>|<span data-ttu-id="b01b1-183">String</span><span class="sxs-lookup"><span data-stu-id="b01b1-183">String</span></span>|<span data-ttu-id="b01b1-184">Geben Sie den Namen der Netzwerk-Konfiguration.</span><span class="sxs-lookup"><span data-stu-id="b01b1-184">Specify the network configuration name.</span></span>|
|<span data-ttu-id="b01b1-185">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="b01b1-185">connectAutomatically</span></span>|<span data-ttu-id="b01b1-186">Boolesch</span><span class="sxs-lookup"><span data-stu-id="b01b1-186">Boolean</span></span>|<span data-ttu-id="b01b1-187">Geben Sie an, ob die WLAN-Verbindung automatisch im Bereich eine Verbindung herstellen soll.</span><span class="sxs-lookup"><span data-stu-id="b01b1-187">Specify whether the wifi connection should connect automatically when in range.</span></span>|
|<span data-ttu-id="b01b1-188">connectToPreferredNetwork</span><span class="sxs-lookup"><span data-stu-id="b01b1-188">connectToPreferredNetwork</span></span>|<span data-ttu-id="b01b1-189">Boolesch</span><span class="sxs-lookup"><span data-stu-id="b01b1-189">Boolean</span></span>|<span data-ttu-id="b01b1-190">Geben Sie an, ob die WLAN-Verbindung zu bevorzugten Netzwerken, wenn bereits mit diesem verbunden eine Verbindung herstellen soll.</span><span class="sxs-lookup"><span data-stu-id="b01b1-190">Specify whether the wifi connection should connect to more preferred networks when already connected to this one.</span></span>  <span data-ttu-id="b01b1-191">Erfordert ConnectAutomatically auf true festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="b01b1-191">Requires ConnectAutomatically to be true.</span></span>|
|<span data-ttu-id="b01b1-192">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="b01b1-192">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="b01b1-193">Boolesch</span><span class="sxs-lookup"><span data-stu-id="b01b1-193">Boolean</span></span>|<span data-ttu-id="b01b1-194">Geben Sie an, ob die WLAN-Verbindung automatisch verbinden sollte, auch wenn die SSID nicht übertragen wird.</span><span class="sxs-lookup"><span data-stu-id="b01b1-194">Specify whether the wifi connection should connect automatically even when the SSID is not broadcasting.</span></span>|
|<span data-ttu-id="b01b1-195">proxySetting</span><span class="sxs-lookup"><span data-stu-id="b01b1-195">proxySetting</span></span>|[<span data-ttu-id="b01b1-196">wiFiProxySetting</span><span class="sxs-lookup"><span data-stu-id="b01b1-196">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="b01b1-197">Geben Sie die Proxyeinstellung für Wi-Fi-Konfiguration.</span><span class="sxs-lookup"><span data-stu-id="b01b1-197">Specify the proxy setting for Wi-Fi configuration.</span></span> <span data-ttu-id="b01b1-198">Mögliche Werte sind: `none`, `manual` und `automatic`.</span><span class="sxs-lookup"><span data-stu-id="b01b1-198">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="b01b1-199">proxyManualAddress</span><span class="sxs-lookup"><span data-stu-id="b01b1-199">proxyManualAddress</span></span>|<span data-ttu-id="b01b1-200">String</span><span class="sxs-lookup"><span data-stu-id="b01b1-200">String</span></span>|<span data-ttu-id="b01b1-201">Geben Sie die IP-Adresse des Proxyservers ein.</span><span class="sxs-lookup"><span data-stu-id="b01b1-201">Specify the IP address for the proxy server.</span></span>|
|<span data-ttu-id="b01b1-202">proxyManualPort</span><span class="sxs-lookup"><span data-stu-id="b01b1-202">proxyManualPort</span></span>|<span data-ttu-id="b01b1-203">Int32</span><span class="sxs-lookup"><span data-stu-id="b01b1-203">Int32</span></span>|<span data-ttu-id="b01b1-204">Geben Sie den Port für den Proxyserver ein.</span><span class="sxs-lookup"><span data-stu-id="b01b1-204">Specify the port for the proxy server.</span></span>|
|<span data-ttu-id="b01b1-205">proxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="b01b1-205">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="b01b1-206">String</span><span class="sxs-lookup"><span data-stu-id="b01b1-206">String</span></span>|<span data-ttu-id="b01b1-207">Geben Sie die URL für das Skript Server Proxykonfiguration.</span><span class="sxs-lookup"><span data-stu-id="b01b1-207">Specify the URL for the proxy server configuration script.</span></span>|
|<span data-ttu-id="b01b1-208">forceFIPSCompliance</span><span class="sxs-lookup"><span data-stu-id="b01b1-208">forceFIPSCompliance</span></span>|<span data-ttu-id="b01b1-209">Boolesch</span><span class="sxs-lookup"><span data-stu-id="b01b1-209">Boolean</span></span>|<span data-ttu-id="b01b1-210">Gibt an, ob FIPS-Konformität zu erzwingen.</span><span class="sxs-lookup"><span data-stu-id="b01b1-210">Specify whether to force FIPS compliance.</span></span>|



## <a name="response"></a><span data-ttu-id="b01b1-211">Antwort</span><span class="sxs-lookup"><span data-stu-id="b01b1-211">Response</span></span>
<span data-ttu-id="b01b1-212">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [WindowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="b01b1-212">If successful, this method returns a `200 OK` response code and an updated [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b01b1-213">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b01b1-213">Example</span></span>
### <a name="request"></a><span data-ttu-id="b01b1-214">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b01b1-214">Request</span></span>
<span data-ttu-id="b01b1-215">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b01b1-215">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 787

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "preSharedKey": "Pre Shared Key value",
  "wifiSecurityType": "wpaPersonal",
  "meteredConnectionLimit": "fixed",
  "ssid": "Ssid value",
  "networkName": "Network Name value",
  "connectAutomatically": true,
  "connectToPreferredNetwork": true,
  "connectWhenNetworkNameIsHidden": true,
  "proxySetting": "manual",
  "proxyManualAddress": "Proxy Manual Address value",
  "proxyManualPort": 15,
  "proxyAutomaticConfigurationUrl": "https://example.com/proxyAutomaticConfigurationUrl/",
  "forceFIPSCompliance": true
}
```

### <a name="response"></a><span data-ttu-id="b01b1-216">Antwort</span><span class="sxs-lookup"><span data-stu-id="b01b1-216">Response</span></span>
<span data-ttu-id="b01b1-p115">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b01b1-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 958

{
  "@odata.type": "#microsoft.graph.windowsWifiConfiguration",
  "id": "8a9e790f-790f-8a9e-0f79-9e8a0f799e8a",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "preSharedKey": "Pre Shared Key value",
  "wifiSecurityType": "wpaPersonal",
  "meteredConnectionLimit": "fixed",
  "ssid": "Ssid value",
  "networkName": "Network Name value",
  "connectAutomatically": true,
  "connectToPreferredNetwork": true,
  "connectWhenNetworkNameIsHidden": true,
  "proxySetting": "manual",
  "proxyManualAddress": "Proxy Manual Address value",
  "proxyManualPort": 15,
  "proxyAutomaticConfigurationUrl": "https://example.com/proxyAutomaticConfigurationUrl/",
  "forceFIPSCompliance": true
}
```





