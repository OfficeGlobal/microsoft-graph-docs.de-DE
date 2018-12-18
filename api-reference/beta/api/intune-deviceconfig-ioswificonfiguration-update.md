---
title: IosWiFiConfiguration aktualisieren
description: Aktualisieren Sie die Eigenschaften eines IosWiFiConfiguration-Objekts.
author: tfitzmac
ms.openlocfilehash: a413d608ee08f02380f387f8361e7103ff8364b0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27329981"
---
# <a name="update-ioswificonfiguration"></a><span data-ttu-id="8c838-103">IosWiFiConfiguration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="8c838-103">Update iosWiFiConfiguration</span></span>

> <span data-ttu-id="8c838-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="8c838-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8c838-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8c838-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8c838-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="8c838-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8c838-107">Aktualisieren Sie die Eigenschaften eines [IosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="8c838-107">Update the properties of a [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8c838-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="8c838-108">Prerequisites</span></span>
<span data-ttu-id="8c838-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8c838-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8c838-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8c838-111">Permission type</span></span>|<span data-ttu-id="8c838-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8c838-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8c838-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8c838-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8c838-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c838-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8c838-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8c838-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8c838-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8c838-116">Not supported.</span></span>|
|<span data-ttu-id="8c838-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8c838-117">Application</span></span>|<span data-ttu-id="8c838-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8c838-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8c838-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8c838-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="8c838-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8c838-120">Request headers</span></span>
|<span data-ttu-id="8c838-121">Header</span><span class="sxs-lookup"><span data-stu-id="8c838-121">Header</span></span>|<span data-ttu-id="8c838-122">Wert</span><span class="sxs-lookup"><span data-stu-id="8c838-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8c838-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="8c838-123">Authorization</span></span>|<span data-ttu-id="8c838-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="8c838-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8c838-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8c838-125">Accept</span></span>|<span data-ttu-id="8c838-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8c838-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8c838-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8c838-127">Request body</span></span>
<span data-ttu-id="8c838-128">Geben Sie im Textkörper Anforderung für das Objekt [IosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="8c838-128">In the request body, supply a JSON representation for the [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md) object.</span></span>

<span data-ttu-id="8c838-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [IosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="8c838-129">The following table shows the properties that are required when you create the [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md).</span></span>

|<span data-ttu-id="8c838-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8c838-130">Property</span></span>|<span data-ttu-id="8c838-131">Typ</span><span class="sxs-lookup"><span data-stu-id="8c838-131">Type</span></span>|<span data-ttu-id="8c838-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8c838-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8c838-133">id</span><span class="sxs-lookup"><span data-stu-id="8c838-133">id</span></span>|<span data-ttu-id="8c838-134">String</span><span class="sxs-lookup"><span data-stu-id="8c838-134">String</span></span>|<span data-ttu-id="8c838-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="8c838-135">Key of the entity.</span></span> <span data-ttu-id="8c838-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8c838-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8c838-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8c838-137">lastModifiedDateTime</span></span>|<span data-ttu-id="8c838-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8c838-138">DateTimeOffset</span></span>|<span data-ttu-id="8c838-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="8c838-139">DateTime the object was last modified.</span></span> <span data-ttu-id="8c838-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8c838-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8c838-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8c838-141">roleScopeTagIds</span></span>|<span data-ttu-id="8c838-142">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="8c838-142">String collection</span></span>|<span data-ttu-id="8c838-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="8c838-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="8c838-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8c838-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8c838-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="8c838-145">supportsScopeTags</span></span>|<span data-ttu-id="8c838-146">Boolesch</span><span class="sxs-lookup"><span data-stu-id="8c838-146">Boolean</span></span>|<span data-ttu-id="8c838-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8c838-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="8c838-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="8c838-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="8c838-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="8c838-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="8c838-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="8c838-150">This property is read-only.</span></span> <span data-ttu-id="8c838-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8c838-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8c838-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8c838-152">createdDateTime</span></span>|<span data-ttu-id="8c838-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8c838-153">DateTimeOffset</span></span>|<span data-ttu-id="8c838-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="8c838-154">DateTime the object was created.</span></span> <span data-ttu-id="8c838-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8c838-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8c838-156">description</span><span class="sxs-lookup"><span data-stu-id="8c838-156">description</span></span>|<span data-ttu-id="8c838-157">String</span><span class="sxs-lookup"><span data-stu-id="8c838-157">String</span></span>|<span data-ttu-id="8c838-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="8c838-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="8c838-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8c838-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8c838-160">displayName</span><span class="sxs-lookup"><span data-stu-id="8c838-160">displayName</span></span>|<span data-ttu-id="8c838-161">String</span><span class="sxs-lookup"><span data-stu-id="8c838-161">String</span></span>|<span data-ttu-id="8c838-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="8c838-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="8c838-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8c838-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8c838-164">Version</span><span class="sxs-lookup"><span data-stu-id="8c838-164">version</span></span>|<span data-ttu-id="8c838-165">Int32</span><span class="sxs-lookup"><span data-stu-id="8c838-165">Int32</span></span>|<span data-ttu-id="8c838-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="8c838-166">Version of the device configuration.</span></span> <span data-ttu-id="8c838-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8c838-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8c838-168">Netzwerkname</span><span class="sxs-lookup"><span data-stu-id="8c838-168">networkName</span></span>|<span data-ttu-id="8c838-169">String</span><span class="sxs-lookup"><span data-stu-id="8c838-169">String</span></span>|<span data-ttu-id="8c838-170">Netzwerkname</span><span class="sxs-lookup"><span data-stu-id="8c838-170">Network Name</span></span>|
|<span data-ttu-id="8c838-171">SSID</span><span class="sxs-lookup"><span data-stu-id="8c838-171">ssid</span></span>|<span data-ttu-id="8c838-172">String</span><span class="sxs-lookup"><span data-stu-id="8c838-172">String</span></span>|<span data-ttu-id="8c838-173">Dies ist der Name des Netzwerks Wi-Fi, die an alle Geräte gesendet wird.</span><span class="sxs-lookup"><span data-stu-id="8c838-173">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span>|
|<span data-ttu-id="8c838-174">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="8c838-174">connectAutomatically</span></span>|<span data-ttu-id="8c838-175">Boolesch</span><span class="sxs-lookup"><span data-stu-id="8c838-175">Boolean</span></span>|<span data-ttu-id="8c838-176">Verbinden Sie automatisch, wenn dieses Netzwerk im Bereich befindet.</span><span class="sxs-lookup"><span data-stu-id="8c838-176">Connect automatically when this network is in range.</span></span> <span data-ttu-id="8c838-177">Eine Einstellung auf "true" überspringt die Aufforderung der Benutzer und automatisch mit Wi-Fi-Netzwerk verbinden.</span><span class="sxs-lookup"><span data-stu-id="8c838-177">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span>|
|<span data-ttu-id="8c838-178">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="8c838-178">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="8c838-179">Boolesch</span><span class="sxs-lookup"><span data-stu-id="8c838-179">Boolean</span></span>|<span data-ttu-id="8c838-180">Verbinden Sie, wenn das Netzwerk seinen Namen (SSID) nicht übertragen wird.</span><span class="sxs-lookup"><span data-stu-id="8c838-180">Connect when the network is not broadcasting its name (SSID).</span></span> <span data-ttu-id="8c838-181">Bei Festlegung auf true festgelegt ist, dieses Profil erzwingt, dass das Gerät für die Verbindung mit einem Netzwerk SSID nicht, die an alle Geräte seine.</span><span class="sxs-lookup"><span data-stu-id="8c838-181">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span>|
|<span data-ttu-id="8c838-182">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="8c838-182">wiFiSecurityType</span></span>|[<span data-ttu-id="8c838-183">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="8c838-183">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="8c838-184">Gibt an, ob Wi-Fi-Endpunkt einen EAP-basierte Sicherheitstyp verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="8c838-184">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="8c838-185">Mögliche Werte sind: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal` und `wpa2Enterprise`.</span><span class="sxs-lookup"><span data-stu-id="8c838-185">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="8c838-186">proxySettings</span><span class="sxs-lookup"><span data-stu-id="8c838-186">proxySettings</span></span>|[<span data-ttu-id="8c838-187">wiFiProxySetting</span><span class="sxs-lookup"><span data-stu-id="8c838-187">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="8c838-188">Proxytyp für diese Wi-Fi-Verbindung.</span><span class="sxs-lookup"><span data-stu-id="8c838-188">Proxy Type for this Wi-Fi connection.</span></span> <span data-ttu-id="8c838-189">Mögliche Werte sind: `none`, `manual` und `automatic`.</span><span class="sxs-lookup"><span data-stu-id="8c838-189">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="8c838-190">proxyManualAddress</span><span class="sxs-lookup"><span data-stu-id="8c838-190">proxyManualAddress</span></span>|<span data-ttu-id="8c838-191">String</span><span class="sxs-lookup"><span data-stu-id="8c838-191">String</span></span>|<span data-ttu-id="8c838-192">IP-Adresse oder den DNS-Hostnamen des Proxyservers bei der manueller Konfiguration ausgewählt ist.</span><span class="sxs-lookup"><span data-stu-id="8c838-192">IP Address or DNS hostname of the proxy server when manual configuration is selected.</span></span>|
|<span data-ttu-id="8c838-193">proxyManualPort</span><span class="sxs-lookup"><span data-stu-id="8c838-193">proxyManualPort</span></span>|<span data-ttu-id="8c838-194">Int32</span><span class="sxs-lookup"><span data-stu-id="8c838-194">Int32</span></span>|<span data-ttu-id="8c838-195">Die Portnummer des Proxyservers bei der manueller Konfiguration ausgewählt ist.</span><span class="sxs-lookup"><span data-stu-id="8c838-195">Port of the proxy server when manual configuration is selected.</span></span>|
|<span data-ttu-id="8c838-196">proxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="8c838-196">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="8c838-197">String</span><span class="sxs-lookup"><span data-stu-id="8c838-197">String</span></span>|<span data-ttu-id="8c838-198">URL des eigentlichen Skripts Proxy Server automatische Konfiguration automatische Konfiguration aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="8c838-198">URL of the proxy server automatic configuration script when automatic configuration is selected.</span></span> <span data-ttu-id="8c838-199">Diese URL hat normalerweise den Speicherort der Datei PAC (Proxy Automatische Konfiguration).</span><span class="sxs-lookup"><span data-stu-id="8c838-199">This URL is typically the location of PAC (Proxy Auto Configuration) file.</span></span>|
|<span data-ttu-id="8c838-200">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="8c838-200">preSharedKey</span></span>|<span data-ttu-id="8c838-201">String</span><span class="sxs-lookup"><span data-stu-id="8c838-201">String</span></span>|<span data-ttu-id="8c838-202">Dies ist die vorinstallierten Schlüssel für WPA persönliche Wi-Fi-Netzwerk.</span><span class="sxs-lookup"><span data-stu-id="8c838-202">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span>|



## <a name="response"></a><span data-ttu-id="8c838-203">Antwort</span><span class="sxs-lookup"><span data-stu-id="8c838-203">Response</span></span>
<span data-ttu-id="8c838-204">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [IosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="8c838-204">If successful, this method returns a `200 OK` response code and an updated [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8c838-205">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8c838-205">Example</span></span>
### <a name="request"></a><span data-ttu-id="8c838-206">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8c838-206">Request</span></span>
<span data-ttu-id="8c838-207">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8c838-207">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 680

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "networkName": "Network Name value",
  "ssid": "Ssid value",
  "connectAutomatically": true,
  "connectWhenNetworkNameIsHidden": true,
  "wiFiSecurityType": "wpaPersonal",
  "proxySettings": "manual",
  "proxyManualAddress": "Proxy Manual Address value",
  "proxyManualPort": 15,
  "proxyAutomaticConfigurationUrl": "https://example.com/proxyAutomaticConfigurationUrl/",
  "preSharedKey": "Pre Shared Key value"
}
```

### <a name="response"></a><span data-ttu-id="8c838-208">Antwort</span><span class="sxs-lookup"><span data-stu-id="8c838-208">Response</span></span>
<span data-ttu-id="8c838-p116">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8c838-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 847

{
  "@odata.type": "#microsoft.graph.iosWiFiConfiguration",
  "id": "516f9ef9-9ef9-516f-f99e-6f51f99e6f51",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "networkName": "Network Name value",
  "ssid": "Ssid value",
  "connectAutomatically": true,
  "connectWhenNetworkNameIsHidden": true,
  "wiFiSecurityType": "wpaPersonal",
  "proxySettings": "manual",
  "proxyManualAddress": "Proxy Manual Address value",
  "proxyManualPort": 15,
  "proxyAutomaticConfigurationUrl": "https://example.com/proxyAutomaticConfigurationUrl/",
  "preSharedKey": "Pre Shared Key value"
}
```





