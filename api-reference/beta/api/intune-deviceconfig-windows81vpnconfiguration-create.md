---
title: Erstellen von windows81VpnConfiguration
description: Erstellen eines neuen windows81VpnConfiguration-Objekts.
ms.openlocfilehash: 7bf50bacf245a020ba72084ead62a545d59a93c6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063977"
---
# <a name="create-windows81vpnconfiguration"></a><span data-ttu-id="f90fa-103">Erstellen von windows81VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="f90fa-103">Create windows81VpnConfiguration</span></span>

> <span data-ttu-id="f90fa-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f90fa-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f90fa-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f90fa-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f90fa-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="f90fa-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f90fa-107">Erstellen eines neuen [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="f90fa-107">Create a new [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f90fa-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f90fa-108">Prerequisites</span></span>
<span data-ttu-id="f90fa-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f90fa-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f90fa-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f90fa-111">Permission type</span></span>|<span data-ttu-id="f90fa-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f90fa-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f90fa-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f90fa-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f90fa-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f90fa-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f90fa-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f90fa-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f90fa-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f90fa-116">Not supported.</span></span>|
|<span data-ttu-id="f90fa-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f90fa-117">Application</span></span>|<span data-ttu-id="f90fa-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f90fa-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f90fa-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f90fa-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="f90fa-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f90fa-120">Request headers</span></span>
|<span data-ttu-id="f90fa-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="f90fa-121">Header</span></span>|<span data-ttu-id="f90fa-122">Wert</span><span class="sxs-lookup"><span data-stu-id="f90fa-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f90fa-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f90fa-123">Authorization</span></span>|<span data-ttu-id="f90fa-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="f90fa-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f90fa-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f90fa-125">Accept</span></span>|<span data-ttu-id="f90fa-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f90fa-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f90fa-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f90fa-127">Request body</span></span>
<span data-ttu-id="f90fa-128">Geben Sie im Textkörper Anforderung für das Objekt windows81VpnConfiguration eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="f90fa-128">In the request body, supply a JSON representation for the windows81VpnConfiguration object.</span></span>

<span data-ttu-id="f90fa-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die windows81VpnConfiguration erstellen.</span><span class="sxs-lookup"><span data-stu-id="f90fa-129">The following table shows the properties that are required when you create the windows81VpnConfiguration.</span></span>

|<span data-ttu-id="f90fa-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f90fa-130">Property</span></span>|<span data-ttu-id="f90fa-131">Typ</span><span class="sxs-lookup"><span data-stu-id="f90fa-131">Type</span></span>|<span data-ttu-id="f90fa-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f90fa-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f90fa-133">id</span><span class="sxs-lookup"><span data-stu-id="f90fa-133">id</span></span>|<span data-ttu-id="f90fa-134">String</span><span class="sxs-lookup"><span data-stu-id="f90fa-134">String</span></span>|<span data-ttu-id="f90fa-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="f90fa-135">Key of the entity.</span></span> <span data-ttu-id="f90fa-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f90fa-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f90fa-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f90fa-137">lastModifiedDateTime</span></span>|<span data-ttu-id="f90fa-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f90fa-138">DateTimeOffset</span></span>|<span data-ttu-id="f90fa-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="f90fa-139">DateTime the object was last modified.</span></span> <span data-ttu-id="f90fa-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f90fa-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f90fa-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f90fa-141">roleScopeTagIds</span></span>|<span data-ttu-id="f90fa-142">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="f90fa-142">String collection</span></span>|<span data-ttu-id="f90fa-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="f90fa-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f90fa-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f90fa-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f90fa-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="f90fa-145">supportsScopeTags</span></span>|<span data-ttu-id="f90fa-146">Boolesch</span><span class="sxs-lookup"><span data-stu-id="f90fa-146">Boolean</span></span>|<span data-ttu-id="f90fa-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f90fa-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f90fa-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="f90fa-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f90fa-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="f90fa-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f90fa-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="f90fa-150">This property is read-only.</span></span> <span data-ttu-id="f90fa-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f90fa-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f90fa-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f90fa-152">createdDateTime</span></span>|<span data-ttu-id="f90fa-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f90fa-153">DateTimeOffset</span></span>|<span data-ttu-id="f90fa-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="f90fa-154">DateTime the object was created.</span></span> <span data-ttu-id="f90fa-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f90fa-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f90fa-156">description</span><span class="sxs-lookup"><span data-stu-id="f90fa-156">description</span></span>|<span data-ttu-id="f90fa-157">String</span><span class="sxs-lookup"><span data-stu-id="f90fa-157">String</span></span>|<span data-ttu-id="f90fa-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="f90fa-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f90fa-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f90fa-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f90fa-160">displayName</span><span class="sxs-lookup"><span data-stu-id="f90fa-160">displayName</span></span>|<span data-ttu-id="f90fa-161">String</span><span class="sxs-lookup"><span data-stu-id="f90fa-161">String</span></span>|<span data-ttu-id="f90fa-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="f90fa-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f90fa-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f90fa-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f90fa-164">Version</span><span class="sxs-lookup"><span data-stu-id="f90fa-164">version</span></span>|<span data-ttu-id="f90fa-165">Int32</span><span class="sxs-lookup"><span data-stu-id="f90fa-165">Int32</span></span>|<span data-ttu-id="f90fa-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="f90fa-166">Version of the device configuration.</span></span> <span data-ttu-id="f90fa-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f90fa-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f90fa-168">connectionName</span><span class="sxs-lookup"><span data-stu-id="f90fa-168">connectionName</span></span>|<span data-ttu-id="f90fa-169">String</span><span class="sxs-lookup"><span data-stu-id="f90fa-169">String</span></span>|<span data-ttu-id="f90fa-170">Name der Verbindung für den Benutzer angezeigt.</span><span class="sxs-lookup"><span data-stu-id="f90fa-170">Connection name displayed to the user.</span></span> <span data-ttu-id="f90fa-171">Geerbt von [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f90fa-171">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="f90fa-172">Server</span><span class="sxs-lookup"><span data-stu-id="f90fa-172">servers</span></span>|<span data-ttu-id="f90fa-173">[VpnServer](../resources/intune-deviceconfig-vpnserver.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="f90fa-173">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="f90fa-174">Liste der VPN-Server im Netzwerk.</span><span class="sxs-lookup"><span data-stu-id="f90fa-174">List of VPN Servers on the network.</span></span> <span data-ttu-id="f90fa-175">Stellen Sie sicher, dass Endbenutzer diese Netzwerkadressen zugreifen können.</span><span class="sxs-lookup"><span data-stu-id="f90fa-175">Make sure end users can access these network locations.</span></span> <span data-ttu-id="f90fa-176">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="f90fa-176">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="f90fa-177">Geerbt von [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f90fa-177">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="f90fa-178">customXml</span><span class="sxs-lookup"><span data-stu-id="f90fa-178">customXml</span></span>|<span data-ttu-id="f90fa-179">Binär</span><span class="sxs-lookup"><span data-stu-id="f90fa-179">Binary</span></span>|<span data-ttu-id="f90fa-180">Benutzerdefinierte XML-Befehle, die die VPN-Verbindung konfiguriert.</span><span class="sxs-lookup"><span data-stu-id="f90fa-180">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="f90fa-181">(UTF8 codiert Bytearray) Geerbt von [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f90fa-181">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="f90fa-182">applyOnlyToWindows81</span><span class="sxs-lookup"><span data-stu-id="f90fa-182">applyOnlyToWindows81</span></span>|<span data-ttu-id="f90fa-183">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f90fa-183">Boolean</span></span>|<span data-ttu-id="f90fa-184">Wert, der angibt, ob die Richtlinie nur für Windows 8.1 gilt.</span><span class="sxs-lookup"><span data-stu-id="f90fa-184">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="f90fa-185">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="f90fa-185">This property is read-only.</span></span>|
|<span data-ttu-id="f90fa-186">connectionType</span><span class="sxs-lookup"><span data-stu-id="f90fa-186">connectionType</span></span>|[<span data-ttu-id="f90fa-187">windowsVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="f90fa-187">windowsVpnConnectionType</span></span>](../resources/intune-deviceconfig-windowsvpnconnectiontype.md)|<span data-ttu-id="f90fa-188">Verbindungstyp.</span><span class="sxs-lookup"><span data-stu-id="f90fa-188">Connection type.</span></span> <span data-ttu-id="f90fa-189">Mögliche Werte: sind `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect` und `checkPointCapsuleVpn`.</span><span class="sxs-lookup"><span data-stu-id="f90fa-189">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`.</span></span>|
|<span data-ttu-id="f90fa-190">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="f90fa-190">loginGroupOrDomain</span></span>|<span data-ttu-id="f90fa-191">String</span><span class="sxs-lookup"><span data-stu-id="f90fa-191">String</span></span>|<span data-ttu-id="f90fa-192">Anmeldegruppe oder Domäne Wenn Verbindungstyp auf Dell SonicWALL Mobile Verbindung festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="f90fa-192">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span>|
|<span data-ttu-id="f90fa-193">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="f90fa-193">enableSplitTunneling</span></span>|<span data-ttu-id="f90fa-194">Boolesch</span><span class="sxs-lookup"><span data-stu-id="f90fa-194">Boolean</span></span>|<span data-ttu-id="f90fa-195">Aktivieren Sie die Split-tunneling für das VPN.</span><span class="sxs-lookup"><span data-stu-id="f90fa-195">Enable split tunneling for the VPN.</span></span>|
|<span data-ttu-id="f90fa-196">proxyServer</span><span class="sxs-lookup"><span data-stu-id="f90fa-196">proxyServer</span></span>|[<span data-ttu-id="f90fa-197">windows81VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="f90fa-197">windows81VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows81vpnproxyserver.md)|<span data-ttu-id="f90fa-198">Proxy-Server.</span><span class="sxs-lookup"><span data-stu-id="f90fa-198">Proxy Server.</span></span>|



## <a name="response"></a><span data-ttu-id="f90fa-199">Antwort</span><span class="sxs-lookup"><span data-stu-id="f90fa-199">Response</span></span>
<span data-ttu-id="f90fa-200">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="f90fa-200">If successful, this method returns a `201 Created` response code and a [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f90fa-201">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f90fa-201">Example</span></span>
### <a name="request"></a><span data-ttu-id="f90fa-202">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f90fa-202">Request</span></span>
<span data-ttu-id="f90fa-203">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f90fa-203">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1079

{
  "@odata.type": "#microsoft.graph.windows81VpnConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "connectionName": "Connection Name value",
  "servers": [
    {
      "@odata.type": "microsoft.graph.vpnServer",
      "description": "Description value",
      "address": "Address value",
      "isDefaultServer": true
    }
  ],
  "customXml": "Y3VzdG9tWG1s",
  "applyOnlyToWindows81": true,
  "connectionType": "f5EdgeClient",
  "loginGroupOrDomain": "Login Group Or Domain value",
  "enableSplitTunneling": true,
  "proxyServer": {
    "@odata.type": "microsoft.graph.windows81VpnProxyServer",
    "automaticConfigurationScriptUrl": "https://example.com/automaticConfigurationScriptUrl/",
    "address": "Address value",
    "port": 4,
    "automaticallyDetectProxySettings": true,
    "bypassProxyServerForLocalAddress": true
  }
}
```

### <a name="response"></a><span data-ttu-id="f90fa-204">Antwort</span><span class="sxs-lookup"><span data-stu-id="f90fa-204">Response</span></span>
<span data-ttu-id="f90fa-p116">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f90fa-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1187

{
  "@odata.type": "#microsoft.graph.windows81VpnConfiguration",
  "id": "6aa07da3-7da3-6aa0-a37d-a06aa37da06a",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "connectionName": "Connection Name value",
  "servers": [
    {
      "@odata.type": "microsoft.graph.vpnServer",
      "description": "Description value",
      "address": "Address value",
      "isDefaultServer": true
    }
  ],
  "customXml": "Y3VzdG9tWG1s",
  "applyOnlyToWindows81": true,
  "connectionType": "f5EdgeClient",
  "loginGroupOrDomain": "Login Group Or Domain value",
  "enableSplitTunneling": true,
  "proxyServer": {
    "@odata.type": "microsoft.graph.windows81VpnProxyServer",
    "automaticConfigurationScriptUrl": "https://example.com/automaticConfigurationScriptUrl/",
    "address": "Address value",
    "port": 4,
    "automaticallyDetectProxySettings": true,
    "bypassProxyServerForLocalAddress": true
  }
}
```





