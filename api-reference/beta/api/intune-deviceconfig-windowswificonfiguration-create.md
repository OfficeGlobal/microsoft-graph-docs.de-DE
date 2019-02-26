---
title: WindowsWifiConfiguration erstellen
description: Erstellen eines neuen windowsWifiConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 39b5cf192fbb294818d2fb9fb23b49ed0c866739
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30163777"
---
# <a name="create-windowswificonfiguration"></a><span data-ttu-id="cd54b-103">WindowsWifiConfiguration erstellen</span><span class="sxs-lookup"><span data-stu-id="cd54b-103">Create windowsWifiConfiguration</span></span>

> <span data-ttu-id="cd54b-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="cd54b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cd54b-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="cd54b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cd54b-106">Erstellen eines neuen [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="cd54b-106">Create a new [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cd54b-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="cd54b-107">Prerequisites</span></span>
<span data-ttu-id="cd54b-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="cd54b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="cd54b-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="cd54b-110">Permission type</span></span>|<span data-ttu-id="cd54b-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="cd54b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cd54b-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="cd54b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cd54b-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd54b-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="cd54b-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="cd54b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cd54b-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cd54b-115">Not supported.</span></span>|
|<span data-ttu-id="cd54b-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="cd54b-116">Application</span></span>|<span data-ttu-id="cd54b-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cd54b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cd54b-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="cd54b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="cd54b-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="cd54b-119">Request headers</span></span>
|<span data-ttu-id="cd54b-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="cd54b-120">Header</span></span>|<span data-ttu-id="cd54b-121">Wert</span><span class="sxs-lookup"><span data-stu-id="cd54b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cd54b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="cd54b-122">Authorization</span></span>|<span data-ttu-id="cd54b-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="cd54b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cd54b-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="cd54b-124">Accept</span></span>|<span data-ttu-id="cd54b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="cd54b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cd54b-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="cd54b-126">Request body</span></span>
<span data-ttu-id="cd54b-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das windowsWifiConfiguration-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="cd54b-127">In the request body, supply a JSON representation for the windowsWifiConfiguration object.</span></span>

<span data-ttu-id="cd54b-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der windowsWifiConfiguration erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="cd54b-128">The following table shows the properties that are required when you create the windowsWifiConfiguration.</span></span>

|<span data-ttu-id="cd54b-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="cd54b-129">Property</span></span>|<span data-ttu-id="cd54b-130">Typ</span><span class="sxs-lookup"><span data-stu-id="cd54b-130">Type</span></span>|<span data-ttu-id="cd54b-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cd54b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cd54b-132">id</span><span class="sxs-lookup"><span data-stu-id="cd54b-132">id</span></span>|<span data-ttu-id="cd54b-133">string</span><span class="sxs-lookup"><span data-stu-id="cd54b-133">String</span></span>|<span data-ttu-id="cd54b-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="cd54b-134">Key of the entity.</span></span> <span data-ttu-id="cd54b-135">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cd54b-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cd54b-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cd54b-136">lastModifiedDateTime</span></span>|<span data-ttu-id="cd54b-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cd54b-137">DateTimeOffset</span></span>|<span data-ttu-id="cd54b-138">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="cd54b-138">DateTime the object was last modified.</span></span> <span data-ttu-id="cd54b-139">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cd54b-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cd54b-140">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="cd54b-140">roleScopeTagIds</span></span>|<span data-ttu-id="cd54b-141">String collection</span><span class="sxs-lookup"><span data-stu-id="cd54b-141">String collection</span></span>|<span data-ttu-id="cd54b-142">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="cd54b-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="cd54b-143">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cd54b-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cd54b-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="cd54b-144">supportsScopeTags</span></span>|<span data-ttu-id="cd54b-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd54b-145">Boolean</span></span>|<span data-ttu-id="cd54b-146">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereichs Tags unterstützt.</span><span class="sxs-lookup"><span data-stu-id="cd54b-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="cd54b-147">Das Zuweisen zur ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert auf false festgelegt ist und Entitäten für bereichsbezogene Benutzer nicht sichtbar sind.</span><span class="sxs-lookup"><span data-stu-id="cd54b-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="cd54b-148">Dies geschieht für in Silverlight erstellte Legacy Richtlinien und kann durch Löschen und erneutes Erstellen der Richtlinie im Azure-Portal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="cd54b-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="cd54b-149">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="cd54b-149">This property is read-only.</span></span> <span data-ttu-id="cd54b-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cd54b-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cd54b-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cd54b-151">createdDateTime</span></span>|<span data-ttu-id="cd54b-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cd54b-152">DateTimeOffset</span></span>|<span data-ttu-id="cd54b-153">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="cd54b-153">DateTime the object was created.</span></span> <span data-ttu-id="cd54b-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cd54b-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cd54b-155">description</span><span class="sxs-lookup"><span data-stu-id="cd54b-155">description</span></span>|<span data-ttu-id="cd54b-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="cd54b-156">String</span></span>|<span data-ttu-id="cd54b-157">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="cd54b-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="cd54b-158">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cd54b-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cd54b-159">displayName</span><span class="sxs-lookup"><span data-stu-id="cd54b-159">displayName</span></span>|<span data-ttu-id="cd54b-160">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="cd54b-160">String</span></span>|<span data-ttu-id="cd54b-161">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="cd54b-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="cd54b-162">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cd54b-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cd54b-163">Version</span><span class="sxs-lookup"><span data-stu-id="cd54b-163">version</span></span>|<span data-ttu-id="cd54b-164">Int32</span><span class="sxs-lookup"><span data-stu-id="cd54b-164">Int32</span></span>|<span data-ttu-id="cd54b-165">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="cd54b-165">Version of the device configuration.</span></span> <span data-ttu-id="cd54b-166">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cd54b-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cd54b-167">PresharedKey wurde</span><span class="sxs-lookup"><span data-stu-id="cd54b-167">preSharedKey</span></span>|<span data-ttu-id="cd54b-168">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="cd54b-168">String</span></span>|<span data-ttu-id="cd54b-169">Dies ist der vorinstallierte Schlüssel für ein persönliches WPA-Wi-Fi-Netzwerk.</span><span class="sxs-lookup"><span data-stu-id="cd54b-169">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span>|
|<span data-ttu-id="cd54b-170">wifiSecurityType</span><span class="sxs-lookup"><span data-stu-id="cd54b-170">wifiSecurityType</span></span>|[<span data-ttu-id="cd54b-171">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="cd54b-171">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="cd54b-172">Geben Sie den WiFi-Sicherheitstyp an.</span><span class="sxs-lookup"><span data-stu-id="cd54b-172">Specify the Wifi Security Type.</span></span> <span data-ttu-id="cd54b-173">Mögliche Werte sind: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal` und `wpa2Enterprise`.</span><span class="sxs-lookup"><span data-stu-id="cd54b-173">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="cd54b-174">meteredConnectionLimit</span><span class="sxs-lookup"><span data-stu-id="cd54b-174">meteredConnectionLimit</span></span>|[<span data-ttu-id="cd54b-175">meteredConnectionLimitType</span><span class="sxs-lookup"><span data-stu-id="cd54b-175">meteredConnectionLimitType</span></span>](../resources/intune-deviceconfig-meteredconnectionlimittype.md)|<span data-ttu-id="cd54b-176">Geben Sie den Grenzwert für die gemessene Verbindung für die WLAN-Verbindung an.</span><span class="sxs-lookup"><span data-stu-id="cd54b-176">Specify the metered connection limit type for the wifi connection.</span></span> <span data-ttu-id="cd54b-177">Mögliche Werte sind: `unrestricted`, `fixed` und `variable`.</span><span class="sxs-lookup"><span data-stu-id="cd54b-177">Possible values are: `unrestricted`, `fixed`, `variable`.</span></span>|
|<span data-ttu-id="cd54b-178">SSID</span><span class="sxs-lookup"><span data-stu-id="cd54b-178">ssid</span></span>|<span data-ttu-id="cd54b-179">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="cd54b-179">String</span></span>|<span data-ttu-id="cd54b-180">Geben Sie die SSID der WiFi-Verbindung an.</span><span class="sxs-lookup"><span data-stu-id="cd54b-180">Specify the SSID of the wifi connection.</span></span>|
|<span data-ttu-id="cd54b-181">networkName</span><span class="sxs-lookup"><span data-stu-id="cd54b-181">networkName</span></span>|<span data-ttu-id="cd54b-182">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="cd54b-182">String</span></span>|<span data-ttu-id="cd54b-183">Geben Sie den Namen der Netzwerkkonfiguration an.</span><span class="sxs-lookup"><span data-stu-id="cd54b-183">Specify the network configuration name.</span></span>|
|<span data-ttu-id="cd54b-184">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="cd54b-184">connectAutomatically</span></span>|<span data-ttu-id="cd54b-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd54b-185">Boolean</span></span>|<span data-ttu-id="cd54b-186">Geben Sie an, ob die WiFi-Verbindung automatisch eine Verbindung herstellen soll, wenn in Reichweite.</span><span class="sxs-lookup"><span data-stu-id="cd54b-186">Specify whether the wifi connection should connect automatically when in range.</span></span>|
|<span data-ttu-id="cd54b-187">connectToPreferredNetwork</span><span class="sxs-lookup"><span data-stu-id="cd54b-187">connectToPreferredNetwork</span></span>|<span data-ttu-id="cd54b-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd54b-188">Boolean</span></span>|<span data-ttu-id="cd54b-189">Geben Sie an, ob die WLAN-Verbindung mit den bevorzugten Netzwerken verbunden werden soll, wenn Sie bereits mit diesem verknüpft ist.</span><span class="sxs-lookup"><span data-stu-id="cd54b-189">Specify whether the wifi connection should connect to more preferred networks when already connected to this one.</span></span>  <span data-ttu-id="cd54b-190">Erfordert, dass ConnectAutomatically auf true festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="cd54b-190">Requires ConnectAutomatically to be true.</span></span>|
|<span data-ttu-id="cd54b-191">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="cd54b-191">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="cd54b-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd54b-192">Boolean</span></span>|<span data-ttu-id="cd54b-193">Geben Sie an, ob die WLAN-Verbindung automatisch eine Verbindung herstellen soll, selbst wenn die SSID nicht übertragen wird.</span><span class="sxs-lookup"><span data-stu-id="cd54b-193">Specify whether the wifi connection should connect automatically even when the SSID is not broadcasting.</span></span>|
|<span data-ttu-id="cd54b-194">proxySetting</span><span class="sxs-lookup"><span data-stu-id="cd54b-194">proxySetting</span></span>|[<span data-ttu-id="cd54b-195">wiFiProxySetting</span><span class="sxs-lookup"><span data-stu-id="cd54b-195">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="cd54b-196">Geben Sie die Proxyeinstellung für die WLAN-Konfiguration an.</span><span class="sxs-lookup"><span data-stu-id="cd54b-196">Specify the proxy setting for Wi-Fi configuration.</span></span> <span data-ttu-id="cd54b-197">Mögliche Werte sind: `none`, `manual` und `automatic`.</span><span class="sxs-lookup"><span data-stu-id="cd54b-197">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="cd54b-198">proxyManualAddress</span><span class="sxs-lookup"><span data-stu-id="cd54b-198">proxyManualAddress</span></span>|<span data-ttu-id="cd54b-199">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="cd54b-199">String</span></span>|<span data-ttu-id="cd54b-200">Geben Sie die IP-Adresse für den Proxy Server an.</span><span class="sxs-lookup"><span data-stu-id="cd54b-200">Specify the IP address for the proxy server.</span></span>|
|<span data-ttu-id="cd54b-201">proxyManualPort</span><span class="sxs-lookup"><span data-stu-id="cd54b-201">proxyManualPort</span></span>|<span data-ttu-id="cd54b-202">Int32</span><span class="sxs-lookup"><span data-stu-id="cd54b-202">Int32</span></span>|<span data-ttu-id="cd54b-203">Geben Sie den Anschluß für den Proxy Server an.</span><span class="sxs-lookup"><span data-stu-id="cd54b-203">Specify the port for the proxy server.</span></span>|
|<span data-ttu-id="cd54b-204">proxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="cd54b-204">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="cd54b-205">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="cd54b-205">String</span></span>|<span data-ttu-id="cd54b-206">Geben Sie die URL für das Proxy Server-Konfigurationsskript an.</span><span class="sxs-lookup"><span data-stu-id="cd54b-206">Specify the URL for the proxy server configuration script.</span></span>|
|<span data-ttu-id="cd54b-207">forceFIPSCompliance</span><span class="sxs-lookup"><span data-stu-id="cd54b-207">forceFIPSCompliance</span></span>|<span data-ttu-id="cd54b-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd54b-208">Boolean</span></span>|<span data-ttu-id="cd54b-209">Geben Sie an, ob die FIPS-Konformität erzwungen werden soll.</span><span class="sxs-lookup"><span data-stu-id="cd54b-209">Specify whether to force FIPS compliance.</span></span>|



## <a name="response"></a><span data-ttu-id="cd54b-210">Antwort</span><span class="sxs-lookup"><span data-stu-id="cd54b-210">Response</span></span>
<span data-ttu-id="cd54b-211">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="cd54b-211">If successful, this method returns a `201 Created` response code and a [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cd54b-212">Beispiel</span><span class="sxs-lookup"><span data-stu-id="cd54b-212">Example</span></span>

### <a name="request"></a><span data-ttu-id="cd54b-213">Anforderung</span><span class="sxs-lookup"><span data-stu-id="cd54b-213">Request</span></span>
<span data-ttu-id="cd54b-214">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="cd54b-214">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 786

{
  "@odata.type": "#microsoft.graph.windowsWifiConfiguration",
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

### <a name="response"></a><span data-ttu-id="cd54b-215">Antwort</span><span class="sxs-lookup"><span data-stu-id="cd54b-215">Response</span></span>
<span data-ttu-id="cd54b-p114">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cd54b-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




