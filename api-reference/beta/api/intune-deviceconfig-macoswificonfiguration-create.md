---
title: MacOSWiFiConfiguration erstellen
description: Erstellen eines neuen macOSWiFiConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 28b72ed5e99bd6aa3779e433c7976a4ad4b0d142
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30967265"
---
# <a name="create-macoswificonfiguration"></a><span data-ttu-id="c4343-103">MacOSWiFiConfiguration erstellen</span><span class="sxs-lookup"><span data-stu-id="c4343-103">Create macOSWiFiConfiguration</span></span>

> <span data-ttu-id="c4343-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c4343-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c4343-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="c4343-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c4343-106">Erstellen eines neuen [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="c4343-106">Create a new [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c4343-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c4343-107">Prerequisites</span></span>
<span data-ttu-id="c4343-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c4343-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c4343-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c4343-110">Permission type</span></span>|<span data-ttu-id="c4343-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c4343-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c4343-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c4343-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c4343-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4343-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c4343-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c4343-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c4343-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c4343-115">Not supported.</span></span>|
|<span data-ttu-id="c4343-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c4343-116">Application</span></span>|<span data-ttu-id="c4343-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c4343-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c4343-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c4343-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="c4343-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c4343-119">Request headers</span></span>
|<span data-ttu-id="c4343-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="c4343-120">Header</span></span>|<span data-ttu-id="c4343-121">Wert</span><span class="sxs-lookup"><span data-stu-id="c4343-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c4343-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c4343-122">Authorization</span></span>|<span data-ttu-id="c4343-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c4343-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c4343-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="c4343-124">Accept</span></span>|<span data-ttu-id="c4343-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c4343-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c4343-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c4343-126">Request body</span></span>
<span data-ttu-id="c4343-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das macOSWiFiConfiguration-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="c4343-127">In the request body, supply a JSON representation for the macOSWiFiConfiguration object.</span></span>

<span data-ttu-id="c4343-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der macOSWiFiConfiguration erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="c4343-128">The following table shows the properties that are required when you create the macOSWiFiConfiguration.</span></span>

|<span data-ttu-id="c4343-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c4343-129">Property</span></span>|<span data-ttu-id="c4343-130">Typ</span><span class="sxs-lookup"><span data-stu-id="c4343-130">Type</span></span>|<span data-ttu-id="c4343-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c4343-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c4343-132">id</span><span class="sxs-lookup"><span data-stu-id="c4343-132">id</span></span>|<span data-ttu-id="c4343-133">String</span><span class="sxs-lookup"><span data-stu-id="c4343-133">String</span></span>|<span data-ttu-id="c4343-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="c4343-134">Key of the entity.</span></span> <span data-ttu-id="c4343-135">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c4343-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c4343-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c4343-136">lastModifiedDateTime</span></span>|<span data-ttu-id="c4343-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c4343-137">DateTimeOffset</span></span>|<span data-ttu-id="c4343-138">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="c4343-138">DateTime the object was last modified.</span></span> <span data-ttu-id="c4343-139">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c4343-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c4343-140">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="c4343-140">roleScopeTagIds</span></span>|<span data-ttu-id="c4343-141">String collection</span><span class="sxs-lookup"><span data-stu-id="c4343-141">String collection</span></span>|<span data-ttu-id="c4343-142">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="c4343-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c4343-143">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c4343-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c4343-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="c4343-144">supportsScopeTags</span></span>|<span data-ttu-id="c4343-145">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c4343-145">Boolean</span></span>|<span data-ttu-id="c4343-146">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereichs Tags unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c4343-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="c4343-147">Das Zuweisen zur ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert auf false festgelegt ist und Entitäten für bereichsbezogene Benutzer nicht sichtbar sind.</span><span class="sxs-lookup"><span data-stu-id="c4343-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="c4343-148">Dies geschieht für in Silverlight erstellte Legacy Richtlinien und kann durch Löschen und erneutes Erstellen der Richtlinie im Azure-Portal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="c4343-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="c4343-149">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="c4343-149">This property is read-only.</span></span> <span data-ttu-id="c4343-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c4343-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c4343-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c4343-151">createdDateTime</span></span>|<span data-ttu-id="c4343-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c4343-152">DateTimeOffset</span></span>|<span data-ttu-id="c4343-153">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="c4343-153">DateTime the object was created.</span></span> <span data-ttu-id="c4343-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c4343-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c4343-155">description</span><span class="sxs-lookup"><span data-stu-id="c4343-155">description</span></span>|<span data-ttu-id="c4343-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c4343-156">String</span></span>|<span data-ttu-id="c4343-157">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="c4343-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c4343-158">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c4343-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c4343-159">displayName</span><span class="sxs-lookup"><span data-stu-id="c4343-159">displayName</span></span>|<span data-ttu-id="c4343-160">String</span><span class="sxs-lookup"><span data-stu-id="c4343-160">String</span></span>|<span data-ttu-id="c4343-161">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="c4343-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c4343-162">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c4343-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c4343-163">Version</span><span class="sxs-lookup"><span data-stu-id="c4343-163">version</span></span>|<span data-ttu-id="c4343-164">Int32</span><span class="sxs-lookup"><span data-stu-id="c4343-164">Int32</span></span>|<span data-ttu-id="c4343-165">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="c4343-165">Version of the device configuration.</span></span> <span data-ttu-id="c4343-166">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c4343-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c4343-167">networkName</span><span class="sxs-lookup"><span data-stu-id="c4343-167">networkName</span></span>|<span data-ttu-id="c4343-168">String</span><span class="sxs-lookup"><span data-stu-id="c4343-168">String</span></span>|<span data-ttu-id="c4343-169">Netzwerk Name</span><span class="sxs-lookup"><span data-stu-id="c4343-169">Network Name</span></span>|
|<span data-ttu-id="c4343-170">SSID</span><span class="sxs-lookup"><span data-stu-id="c4343-170">ssid</span></span>|<span data-ttu-id="c4343-171">String</span><span class="sxs-lookup"><span data-stu-id="c4343-171">String</span></span>|<span data-ttu-id="c4343-172">Dies ist der Name des WLAN-Netzwerks, das auf alle Geräte übertragen wird.</span><span class="sxs-lookup"><span data-stu-id="c4343-172">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span>|
|<span data-ttu-id="c4343-173">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="c4343-173">connectAutomatically</span></span>|<span data-ttu-id="c4343-174">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c4343-174">Boolean</span></span>|<span data-ttu-id="c4343-175">Verbinden Sie sich automatisch, wenn sich dieses Netzwerk in Reichweite befindet.</span><span class="sxs-lookup"><span data-stu-id="c4343-175">Connect automatically when this network is in range.</span></span> <span data-ttu-id="c4343-176">Wenn Sie diesen Wert auf true festlegen, wird die Benutzereingabe übersprungen, und das Gerät wird automatisch mit dem WLAN verbunden.</span><span class="sxs-lookup"><span data-stu-id="c4343-176">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span>|
|<span data-ttu-id="c4343-177">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="c4343-177">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="c4343-178">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c4343-178">Boolean</span></span>|<span data-ttu-id="c4343-179">Verbinden, wenn das Netzwerk seinen Namen (SSID) nicht sendet.</span><span class="sxs-lookup"><span data-stu-id="c4343-179">Connect when the network is not broadcasting its name (SSID).</span></span> <span data-ttu-id="c4343-180">Wenn dieser Wert auf "true" festgelegt ist, wird das Gerät gezwungen, eine Verbindung mit einem Netzwerk herzustellen, das seine SSID nicht auf alle Geräte übermittelt.</span><span class="sxs-lookup"><span data-stu-id="c4343-180">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span>|
|<span data-ttu-id="c4343-181">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="c4343-181">wiFiSecurityType</span></span>|[<span data-ttu-id="c4343-182">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="c4343-182">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="c4343-183">Gibt an, ob der WLAN-Endpunkt einen EAP-basierten Sicherheitstyp verwendet.</span><span class="sxs-lookup"><span data-stu-id="c4343-183">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="c4343-184">Mögliche Werte sind: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal` und `wpa2Enterprise`.</span><span class="sxs-lookup"><span data-stu-id="c4343-184">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="c4343-185">Proxy Settings</span><span class="sxs-lookup"><span data-stu-id="c4343-185">proxySettings</span></span>|[<span data-ttu-id="c4343-186">wiFiProxySetting</span><span class="sxs-lookup"><span data-stu-id="c4343-186">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="c4343-187">Proxytyp für diese WLAN-Verbindung.</span><span class="sxs-lookup"><span data-stu-id="c4343-187">Proxy Type for this Wi-Fi connection.</span></span> <span data-ttu-id="c4343-188">Mögliche Werte sind: `none`, `manual` und `automatic`.</span><span class="sxs-lookup"><span data-stu-id="c4343-188">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="c4343-189">proxyManualAddress</span><span class="sxs-lookup"><span data-stu-id="c4343-189">proxyManualAddress</span></span>|<span data-ttu-id="c4343-190">String</span><span class="sxs-lookup"><span data-stu-id="c4343-190">String</span></span>|<span data-ttu-id="c4343-191">Die IP-Adresse oder der DNS-Hostname des Proxyservers, wenn die manuelle Konfiguration ausgewählt ist.</span><span class="sxs-lookup"><span data-stu-id="c4343-191">IP Address or DNS hostname of the proxy server when manual configuration is selected.</span></span>|
|<span data-ttu-id="c4343-192">proxyManualPort</span><span class="sxs-lookup"><span data-stu-id="c4343-192">proxyManualPort</span></span>|<span data-ttu-id="c4343-193">Int32</span><span class="sxs-lookup"><span data-stu-id="c4343-193">Int32</span></span>|<span data-ttu-id="c4343-194">Der Proxy Server, wenn die manuelle Konfiguration ausgewählt ist.</span><span class="sxs-lookup"><span data-stu-id="c4343-194">Port of the proxy server when manual configuration is selected.</span></span>|
|<span data-ttu-id="c4343-195">proxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="c4343-195">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="c4343-196">String</span><span class="sxs-lookup"><span data-stu-id="c4343-196">String</span></span>|<span data-ttu-id="c4343-197">URL des automatischen Konfigurationsskripts des Proxyservers, wenn die automatische Konfiguration ausgewählt ist.</span><span class="sxs-lookup"><span data-stu-id="c4343-197">URL of the proxy server automatic configuration script when automatic configuration is selected.</span></span> <span data-ttu-id="c4343-198">Diese URL ist in der Regel der Speicherort der PAC (Proxy Auto Configuration)-Datei.</span><span class="sxs-lookup"><span data-stu-id="c4343-198">This URL is typically the location of PAC (Proxy Auto Configuration) file.</span></span>|
|<span data-ttu-id="c4343-199">PresharedKey wurde</span><span class="sxs-lookup"><span data-stu-id="c4343-199">preSharedKey</span></span>|<span data-ttu-id="c4343-200">String</span><span class="sxs-lookup"><span data-stu-id="c4343-200">String</span></span>|<span data-ttu-id="c4343-201">Dies ist der vorinstallierte Schlüssel für ein persönliches WPA-Wi-Fi-Netzwerk.</span><span class="sxs-lookup"><span data-stu-id="c4343-201">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span>|



## <a name="response"></a><span data-ttu-id="c4343-202">Antwort</span><span class="sxs-lookup"><span data-stu-id="c4343-202">Response</span></span>
<span data-ttu-id="c4343-203">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="c4343-203">If successful, this method returns a `201 Created` response code and a [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c4343-204">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c4343-204">Example</span></span>

### <a name="request"></a><span data-ttu-id="c4343-205">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c4343-205">Request</span></span>
<span data-ttu-id="c4343-206">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c4343-206">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 677

{
  "@odata.type": "#microsoft.graph.macOSWiFiConfiguration",
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

### <a name="response"></a><span data-ttu-id="c4343-207">Antwort</span><span class="sxs-lookup"><span data-stu-id="c4343-207">Response</span></span>
<span data-ttu-id="c4343-p115">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c4343-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 849

{
  "@odata.type": "#microsoft.graph.macOSWiFiConfiguration",
  "id": "471203fb-03fb-4712-fb03-1247fb031247",
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




