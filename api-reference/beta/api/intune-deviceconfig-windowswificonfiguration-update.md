---
title: WindowsWifiConfiguration aktualisieren
description: Aktualisieren Sie die Eigenschaften eines WindowsWifiConfiguration-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 982942a679a10b4a33a22bb69a9b55a5b6a9a814
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29405023"
---
# <a name="update-windowswificonfiguration"></a><span data-ttu-id="84562-103">WindowsWifiConfiguration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="84562-103">Update windowsWifiConfiguration</span></span>

> <span data-ttu-id="84562-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="84562-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="84562-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="84562-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="84562-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="84562-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="84562-107">Aktualisieren Sie die Eigenschaften eines [WindowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="84562-107">Update the properties of a [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="84562-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="84562-108">Prerequisites</span></span>
<span data-ttu-id="84562-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="84562-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="84562-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="84562-111">Permission type</span></span>|<span data-ttu-id="84562-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="84562-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="84562-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="84562-113">Delegated (work or school account)</span></span>|<span data-ttu-id="84562-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84562-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="84562-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="84562-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="84562-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="84562-116">Not supported.</span></span>|
|<span data-ttu-id="84562-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="84562-117">Application</span></span>|<span data-ttu-id="84562-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="84562-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="84562-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="84562-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="84562-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="84562-120">Request headers</span></span>
|<span data-ttu-id="84562-121">Header</span><span class="sxs-lookup"><span data-stu-id="84562-121">Header</span></span>|<span data-ttu-id="84562-122">Wert</span><span class="sxs-lookup"><span data-stu-id="84562-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="84562-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="84562-123">Authorization</span></span>|<span data-ttu-id="84562-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="84562-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="84562-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="84562-125">Accept</span></span>|<span data-ttu-id="84562-126">application/json</span><span class="sxs-lookup"><span data-stu-id="84562-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="84562-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="84562-127">Request body</span></span>
<span data-ttu-id="84562-128">Geben Sie im Textkörper Anforderung für das Objekt [WindowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="84562-128">In the request body, supply a JSON representation for the [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) object.</span></span>

<span data-ttu-id="84562-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [WindowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="84562-129">The following table shows the properties that are required when you create the [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span></span>

|<span data-ttu-id="84562-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="84562-130">Property</span></span>|<span data-ttu-id="84562-131">Typ</span><span class="sxs-lookup"><span data-stu-id="84562-131">Type</span></span>|<span data-ttu-id="84562-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="84562-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="84562-133">id</span><span class="sxs-lookup"><span data-stu-id="84562-133">id</span></span>|<span data-ttu-id="84562-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="84562-134">String</span></span>|<span data-ttu-id="84562-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="84562-135">Key of the entity.</span></span> <span data-ttu-id="84562-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="84562-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="84562-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="84562-137">lastModifiedDateTime</span></span>|<span data-ttu-id="84562-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="84562-138">DateTimeOffset</span></span>|<span data-ttu-id="84562-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="84562-139">DateTime the object was last modified.</span></span> <span data-ttu-id="84562-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="84562-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="84562-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="84562-141">roleScopeTagIds</span></span>|<span data-ttu-id="84562-142">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="84562-142">String collection</span></span>|<span data-ttu-id="84562-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="84562-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="84562-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="84562-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="84562-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="84562-145">supportsScopeTags</span></span>|<span data-ttu-id="84562-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="84562-146">Boolean</span></span>|<span data-ttu-id="84562-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="84562-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="84562-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="84562-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="84562-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="84562-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="84562-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="84562-150">This property is read-only.</span></span> <span data-ttu-id="84562-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="84562-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="84562-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="84562-152">createdDateTime</span></span>|<span data-ttu-id="84562-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="84562-153">DateTimeOffset</span></span>|<span data-ttu-id="84562-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="84562-154">DateTime the object was created.</span></span> <span data-ttu-id="84562-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="84562-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="84562-156">description</span><span class="sxs-lookup"><span data-stu-id="84562-156">description</span></span>|<span data-ttu-id="84562-157">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="84562-157">String</span></span>|<span data-ttu-id="84562-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="84562-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="84562-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="84562-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="84562-160">displayName</span><span class="sxs-lookup"><span data-stu-id="84562-160">displayName</span></span>|<span data-ttu-id="84562-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="84562-161">String</span></span>|<span data-ttu-id="84562-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="84562-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="84562-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="84562-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="84562-164">Version</span><span class="sxs-lookup"><span data-stu-id="84562-164">version</span></span>|<span data-ttu-id="84562-165">Int32</span><span class="sxs-lookup"><span data-stu-id="84562-165">Int32</span></span>|<span data-ttu-id="84562-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="84562-166">Version of the device configuration.</span></span> <span data-ttu-id="84562-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="84562-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="84562-168">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="84562-168">preSharedKey</span></span>|<span data-ttu-id="84562-169">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="84562-169">String</span></span>|<span data-ttu-id="84562-170">Dies ist die vorinstallierten Schlüssel für WPA persönliche Wi-Fi-Netzwerk.</span><span class="sxs-lookup"><span data-stu-id="84562-170">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span>|
|<span data-ttu-id="84562-171">wifiSecurityType</span><span class="sxs-lookup"><span data-stu-id="84562-171">wifiSecurityType</span></span>|[<span data-ttu-id="84562-172">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="84562-172">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="84562-173">Den Sicherheitstyp Wifi angeben.</span><span class="sxs-lookup"><span data-stu-id="84562-173">Specify the Wifi Security Type.</span></span> <span data-ttu-id="84562-174">Mögliche Werte sind: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal` und `wpa2Enterprise`.</span><span class="sxs-lookup"><span data-stu-id="84562-174">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="84562-175">meteredConnectionLimit</span><span class="sxs-lookup"><span data-stu-id="84562-175">meteredConnectionLimit</span></span>|[<span data-ttu-id="84562-176">meteredConnectionLimitType</span><span class="sxs-lookup"><span data-stu-id="84562-176">meteredConnectionLimitType</span></span>](../resources/intune-deviceconfig-meteredconnectionlimittype.md)|<span data-ttu-id="84562-177">Geben Sie den gemessenen Verbindungstyp des Grenzwert für die WLAN-Verbindung.</span><span class="sxs-lookup"><span data-stu-id="84562-177">Specify the metered connection limit type for the wifi connection.</span></span> <span data-ttu-id="84562-178">Mögliche Werte sind: `unrestricted`, `fixed` und `variable`.</span><span class="sxs-lookup"><span data-stu-id="84562-178">Possible values are: `unrestricted`, `fixed`, `variable`.</span></span>|
|<span data-ttu-id="84562-179">SSID</span><span class="sxs-lookup"><span data-stu-id="84562-179">ssid</span></span>|<span data-ttu-id="84562-180">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="84562-180">String</span></span>|<span data-ttu-id="84562-181">Geben Sie die SSID des WLAN-Verbindung.</span><span class="sxs-lookup"><span data-stu-id="84562-181">Specify the SSID of the wifi connection.</span></span>|
|<span data-ttu-id="84562-182">Netzwerkname</span><span class="sxs-lookup"><span data-stu-id="84562-182">networkName</span></span>|<span data-ttu-id="84562-183">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="84562-183">String</span></span>|<span data-ttu-id="84562-184">Geben Sie den Namen der Netzwerk-Konfiguration.</span><span class="sxs-lookup"><span data-stu-id="84562-184">Specify the network configuration name.</span></span>|
|<span data-ttu-id="84562-185">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="84562-185">connectAutomatically</span></span>|<span data-ttu-id="84562-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="84562-186">Boolean</span></span>|<span data-ttu-id="84562-187">Geben Sie an, ob die WLAN-Verbindung automatisch im Bereich eine Verbindung herstellen soll.</span><span class="sxs-lookup"><span data-stu-id="84562-187">Specify whether the wifi connection should connect automatically when in range.</span></span>|
|<span data-ttu-id="84562-188">connectToPreferredNetwork</span><span class="sxs-lookup"><span data-stu-id="84562-188">connectToPreferredNetwork</span></span>|<span data-ttu-id="84562-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="84562-189">Boolean</span></span>|<span data-ttu-id="84562-190">Geben Sie an, ob die WLAN-Verbindung zu bevorzugten Netzwerken, wenn bereits mit diesem verbunden eine Verbindung herstellen soll.</span><span class="sxs-lookup"><span data-stu-id="84562-190">Specify whether the wifi connection should connect to more preferred networks when already connected to this one.</span></span>  <span data-ttu-id="84562-191">Erfordert ConnectAutomatically auf true festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="84562-191">Requires ConnectAutomatically to be true.</span></span>|
|<span data-ttu-id="84562-192">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="84562-192">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="84562-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="84562-193">Boolean</span></span>|<span data-ttu-id="84562-194">Geben Sie an, ob die WLAN-Verbindung automatisch verbinden sollte, auch wenn die SSID nicht übertragen wird.</span><span class="sxs-lookup"><span data-stu-id="84562-194">Specify whether the wifi connection should connect automatically even when the SSID is not broadcasting.</span></span>|
|<span data-ttu-id="84562-195">proxySetting</span><span class="sxs-lookup"><span data-stu-id="84562-195">proxySetting</span></span>|[<span data-ttu-id="84562-196">wiFiProxySetting</span><span class="sxs-lookup"><span data-stu-id="84562-196">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="84562-197">Geben Sie die Proxyeinstellung für Wi-Fi-Konfiguration.</span><span class="sxs-lookup"><span data-stu-id="84562-197">Specify the proxy setting for Wi-Fi configuration.</span></span> <span data-ttu-id="84562-198">Mögliche Werte sind: `none`, `manual` und `automatic`.</span><span class="sxs-lookup"><span data-stu-id="84562-198">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="84562-199">proxyManualAddress</span><span class="sxs-lookup"><span data-stu-id="84562-199">proxyManualAddress</span></span>|<span data-ttu-id="84562-200">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="84562-200">String</span></span>|<span data-ttu-id="84562-201">Geben Sie die IP-Adresse des Proxyservers ein.</span><span class="sxs-lookup"><span data-stu-id="84562-201">Specify the IP address for the proxy server.</span></span>|
|<span data-ttu-id="84562-202">proxyManualPort</span><span class="sxs-lookup"><span data-stu-id="84562-202">proxyManualPort</span></span>|<span data-ttu-id="84562-203">Int32</span><span class="sxs-lookup"><span data-stu-id="84562-203">Int32</span></span>|<span data-ttu-id="84562-204">Geben Sie den Port für den Proxyserver ein.</span><span class="sxs-lookup"><span data-stu-id="84562-204">Specify the port for the proxy server.</span></span>|
|<span data-ttu-id="84562-205">proxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="84562-205">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="84562-206">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="84562-206">String</span></span>|<span data-ttu-id="84562-207">Geben Sie die URL für das Skript Server Proxykonfiguration.</span><span class="sxs-lookup"><span data-stu-id="84562-207">Specify the URL for the proxy server configuration script.</span></span>|
|<span data-ttu-id="84562-208">forceFIPSCompliance</span><span class="sxs-lookup"><span data-stu-id="84562-208">forceFIPSCompliance</span></span>|<span data-ttu-id="84562-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="84562-209">Boolean</span></span>|<span data-ttu-id="84562-210">Gibt an, ob FIPS-Konformität zu erzwingen.</span><span class="sxs-lookup"><span data-stu-id="84562-210">Specify whether to force FIPS compliance.</span></span>|



## <a name="response"></a><span data-ttu-id="84562-211">Antwort</span><span class="sxs-lookup"><span data-stu-id="84562-211">Response</span></span>
<span data-ttu-id="84562-212">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [WindowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="84562-212">If successful, this method returns a `200 OK` response code and an updated [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="84562-213">Beispiel</span><span class="sxs-lookup"><span data-stu-id="84562-213">Example</span></span>

### <a name="request"></a><span data-ttu-id="84562-214">Anforderung</span><span class="sxs-lookup"><span data-stu-id="84562-214">Request</span></span>
<span data-ttu-id="84562-215">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="84562-215">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="84562-216">Antwort</span><span class="sxs-lookup"><span data-stu-id="84562-216">Response</span></span>
<span data-ttu-id="84562-p115">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="84562-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




