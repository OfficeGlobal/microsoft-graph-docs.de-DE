---
title: Erstellen von windowsWifiConfiguration
description: Erstellen eines neuen WindowsWifiConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f0e2a12b502ef5aea92ebcc011f2006efbe210fe
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27914465"
---
# <a name="create-windowswificonfiguration"></a><span data-ttu-id="a404d-103">Erstellen von windowsWifiConfiguration</span><span class="sxs-lookup"><span data-stu-id="a404d-103">Create windowsWifiConfiguration</span></span>

> <span data-ttu-id="a404d-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="a404d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a404d-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a404d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a404d-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="a404d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a404d-107">Erstellen eines neuen [WindowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="a404d-107">Create a new [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a404d-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="a404d-108">Prerequisites</span></span>
<span data-ttu-id="a404d-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a404d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a404d-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a404d-111">Permission type</span></span>|<span data-ttu-id="a404d-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a404d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a404d-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a404d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a404d-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a404d-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a404d-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a404d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a404d-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a404d-116">Not supported.</span></span>|
|<span data-ttu-id="a404d-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a404d-117">Application</span></span>|<span data-ttu-id="a404d-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a404d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a404d-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a404d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a404d-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a404d-120">Request headers</span></span>
|<span data-ttu-id="a404d-121">Header</span><span class="sxs-lookup"><span data-stu-id="a404d-121">Header</span></span>|<span data-ttu-id="a404d-122">Wert</span><span class="sxs-lookup"><span data-stu-id="a404d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a404d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a404d-123">Authorization</span></span>|<span data-ttu-id="a404d-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="a404d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a404d-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="a404d-125">Accept</span></span>|<span data-ttu-id="a404d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a404d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a404d-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a404d-127">Request body</span></span>
<span data-ttu-id="a404d-128">Geben Sie im Textkörper Anforderung für das Objekt WindowsWifiConfiguration eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="a404d-128">In the request body, supply a JSON representation for the windowsWifiConfiguration object.</span></span>

<span data-ttu-id="a404d-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die WindowsWifiConfiguration erstellen.</span><span class="sxs-lookup"><span data-stu-id="a404d-129">The following table shows the properties that are required when you create the windowsWifiConfiguration.</span></span>

|<span data-ttu-id="a404d-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a404d-130">Property</span></span>|<span data-ttu-id="a404d-131">Typ</span><span class="sxs-lookup"><span data-stu-id="a404d-131">Type</span></span>|<span data-ttu-id="a404d-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a404d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a404d-133">id</span><span class="sxs-lookup"><span data-stu-id="a404d-133">id</span></span>|<span data-ttu-id="a404d-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a404d-134">String</span></span>|<span data-ttu-id="a404d-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="a404d-135">Key of the entity.</span></span> <span data-ttu-id="a404d-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a404d-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a404d-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a404d-137">lastModifiedDateTime</span></span>|<span data-ttu-id="a404d-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a404d-138">DateTimeOffset</span></span>|<span data-ttu-id="a404d-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="a404d-139">DateTime the object was last modified.</span></span> <span data-ttu-id="a404d-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a404d-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a404d-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a404d-141">roleScopeTagIds</span></span>|<span data-ttu-id="a404d-142">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="a404d-142">String collection</span></span>|<span data-ttu-id="a404d-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="a404d-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a404d-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a404d-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a404d-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="a404d-145">supportsScopeTags</span></span>|<span data-ttu-id="a404d-146">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="a404d-146">Boolean</span></span>|<span data-ttu-id="a404d-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a404d-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="a404d-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="a404d-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="a404d-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="a404d-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="a404d-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="a404d-150">This property is read-only.</span></span> <span data-ttu-id="a404d-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a404d-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a404d-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a404d-152">createdDateTime</span></span>|<span data-ttu-id="a404d-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a404d-153">DateTimeOffset</span></span>|<span data-ttu-id="a404d-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="a404d-154">DateTime the object was created.</span></span> <span data-ttu-id="a404d-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a404d-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a404d-156">description</span><span class="sxs-lookup"><span data-stu-id="a404d-156">description</span></span>|<span data-ttu-id="a404d-157">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a404d-157">String</span></span>|<span data-ttu-id="a404d-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="a404d-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a404d-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a404d-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a404d-160">displayName</span><span class="sxs-lookup"><span data-stu-id="a404d-160">displayName</span></span>|<span data-ttu-id="a404d-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a404d-161">String</span></span>|<span data-ttu-id="a404d-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="a404d-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a404d-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a404d-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a404d-164">Version</span><span class="sxs-lookup"><span data-stu-id="a404d-164">version</span></span>|<span data-ttu-id="a404d-165">Int32</span><span class="sxs-lookup"><span data-stu-id="a404d-165">Int32</span></span>|<span data-ttu-id="a404d-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="a404d-166">Version of the device configuration.</span></span> <span data-ttu-id="a404d-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a404d-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a404d-168">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="a404d-168">preSharedKey</span></span>|<span data-ttu-id="a404d-169">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a404d-169">String</span></span>|<span data-ttu-id="a404d-170">Dies ist die vorinstallierten Schlüssel für WPA persönliche Wi-Fi-Netzwerk.</span><span class="sxs-lookup"><span data-stu-id="a404d-170">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span>|
|<span data-ttu-id="a404d-171">wifiSecurityType</span><span class="sxs-lookup"><span data-stu-id="a404d-171">wifiSecurityType</span></span>|[<span data-ttu-id="a404d-172">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="a404d-172">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="a404d-173">Den Sicherheitstyp Wifi angeben.</span><span class="sxs-lookup"><span data-stu-id="a404d-173">Specify the Wifi Security Type.</span></span> <span data-ttu-id="a404d-174">Mögliche Werte sind: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal` und `wpa2Enterprise`.</span><span class="sxs-lookup"><span data-stu-id="a404d-174">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="a404d-175">meteredConnectionLimit</span><span class="sxs-lookup"><span data-stu-id="a404d-175">meteredConnectionLimit</span></span>|[<span data-ttu-id="a404d-176">meteredConnectionLimitType</span><span class="sxs-lookup"><span data-stu-id="a404d-176">meteredConnectionLimitType</span></span>](../resources/intune-deviceconfig-meteredconnectionlimittype.md)|<span data-ttu-id="a404d-177">Geben Sie den gemessenen Verbindungstyp des Grenzwert für die WLAN-Verbindung.</span><span class="sxs-lookup"><span data-stu-id="a404d-177">Specify the metered connection limit type for the wifi connection.</span></span> <span data-ttu-id="a404d-178">Mögliche Werte sind: `unrestricted`, `fixed` und `variable`.</span><span class="sxs-lookup"><span data-stu-id="a404d-178">Possible values are: `unrestricted`, `fixed`, `variable`.</span></span>|
|<span data-ttu-id="a404d-179">SSID</span><span class="sxs-lookup"><span data-stu-id="a404d-179">ssid</span></span>|<span data-ttu-id="a404d-180">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a404d-180">String</span></span>|<span data-ttu-id="a404d-181">Geben Sie die SSID des WLAN-Verbindung.</span><span class="sxs-lookup"><span data-stu-id="a404d-181">Specify the SSID of the wifi connection.</span></span>|
|<span data-ttu-id="a404d-182">Netzwerkname</span><span class="sxs-lookup"><span data-stu-id="a404d-182">networkName</span></span>|<span data-ttu-id="a404d-183">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a404d-183">String</span></span>|<span data-ttu-id="a404d-184">Geben Sie den Namen der Netzwerk-Konfiguration.</span><span class="sxs-lookup"><span data-stu-id="a404d-184">Specify the network configuration name.</span></span>|
|<span data-ttu-id="a404d-185">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="a404d-185">connectAutomatically</span></span>|<span data-ttu-id="a404d-186">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="a404d-186">Boolean</span></span>|<span data-ttu-id="a404d-187">Geben Sie an, ob die WLAN-Verbindung automatisch im Bereich eine Verbindung herstellen soll.</span><span class="sxs-lookup"><span data-stu-id="a404d-187">Specify whether the wifi connection should connect automatically when in range.</span></span>|
|<span data-ttu-id="a404d-188">connectToPreferredNetwork</span><span class="sxs-lookup"><span data-stu-id="a404d-188">connectToPreferredNetwork</span></span>|<span data-ttu-id="a404d-189">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="a404d-189">Boolean</span></span>|<span data-ttu-id="a404d-190">Geben Sie an, ob die WLAN-Verbindung zu bevorzugten Netzwerken, wenn bereits mit diesem verbunden eine Verbindung herstellen soll.</span><span class="sxs-lookup"><span data-stu-id="a404d-190">Specify whether the wifi connection should connect to more preferred networks when already connected to this one.</span></span>  <span data-ttu-id="a404d-191">Erfordert ConnectAutomatically auf true festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="a404d-191">Requires ConnectAutomatically to be true.</span></span>|
|<span data-ttu-id="a404d-192">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="a404d-192">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="a404d-193">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="a404d-193">Boolean</span></span>|<span data-ttu-id="a404d-194">Geben Sie an, ob die WLAN-Verbindung automatisch verbinden sollte, auch wenn die SSID nicht übertragen wird.</span><span class="sxs-lookup"><span data-stu-id="a404d-194">Specify whether the wifi connection should connect automatically even when the SSID is not broadcasting.</span></span>|
|<span data-ttu-id="a404d-195">proxySetting</span><span class="sxs-lookup"><span data-stu-id="a404d-195">proxySetting</span></span>|[<span data-ttu-id="a404d-196">wiFiProxySetting</span><span class="sxs-lookup"><span data-stu-id="a404d-196">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="a404d-197">Geben Sie die Proxyeinstellung für Wi-Fi-Konfiguration.</span><span class="sxs-lookup"><span data-stu-id="a404d-197">Specify the proxy setting for Wi-Fi configuration.</span></span> <span data-ttu-id="a404d-198">Mögliche Werte sind: `none`, `manual` und `automatic`.</span><span class="sxs-lookup"><span data-stu-id="a404d-198">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="a404d-199">proxyManualAddress</span><span class="sxs-lookup"><span data-stu-id="a404d-199">proxyManualAddress</span></span>|<span data-ttu-id="a404d-200">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a404d-200">String</span></span>|<span data-ttu-id="a404d-201">Geben Sie die IP-Adresse des Proxyservers ein.</span><span class="sxs-lookup"><span data-stu-id="a404d-201">Specify the IP address for the proxy server.</span></span>|
|<span data-ttu-id="a404d-202">proxyManualPort</span><span class="sxs-lookup"><span data-stu-id="a404d-202">proxyManualPort</span></span>|<span data-ttu-id="a404d-203">Int32</span><span class="sxs-lookup"><span data-stu-id="a404d-203">Int32</span></span>|<span data-ttu-id="a404d-204">Geben Sie den Port für den Proxyserver ein.</span><span class="sxs-lookup"><span data-stu-id="a404d-204">Specify the port for the proxy server.</span></span>|
|<span data-ttu-id="a404d-205">proxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="a404d-205">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="a404d-206">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a404d-206">String</span></span>|<span data-ttu-id="a404d-207">Geben Sie die URL für das Skript Server Proxykonfiguration.</span><span class="sxs-lookup"><span data-stu-id="a404d-207">Specify the URL for the proxy server configuration script.</span></span>|
|<span data-ttu-id="a404d-208">forceFIPSCompliance</span><span class="sxs-lookup"><span data-stu-id="a404d-208">forceFIPSCompliance</span></span>|<span data-ttu-id="a404d-209">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="a404d-209">Boolean</span></span>|<span data-ttu-id="a404d-210">Gibt an, ob FIPS-Konformität zu erzwingen.</span><span class="sxs-lookup"><span data-stu-id="a404d-210">Specify whether to force FIPS compliance.</span></span>|



## <a name="response"></a><span data-ttu-id="a404d-211">Antwort</span><span class="sxs-lookup"><span data-stu-id="a404d-211">Response</span></span>
<span data-ttu-id="a404d-212">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [WindowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="a404d-212">If successful, this method returns a `201 Created` response code and a [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a404d-213">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a404d-213">Example</span></span>
### <a name="request"></a><span data-ttu-id="a404d-214">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a404d-214">Request</span></span>
<span data-ttu-id="a404d-215">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a404d-215">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 850

{
  "@odata.type": "#microsoft.graph.windowsWifiConfiguration",
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

### <a name="response"></a><span data-ttu-id="a404d-216">Antwort</span><span class="sxs-lookup"><span data-stu-id="a404d-216">Response</span></span>
<span data-ttu-id="a404d-p115">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a404d-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





