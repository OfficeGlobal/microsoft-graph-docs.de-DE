---
title: Windows81VpnConfiguration erstellen
description: Erstellen eines neuen windows81VpnConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7f3b9dd9d61f6078e4e14e20d1167967f832c421
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30156476"
---
# <a name="create-windows81vpnconfiguration"></a><span data-ttu-id="ae462-103">Windows81VpnConfiguration erstellen</span><span class="sxs-lookup"><span data-stu-id="ae462-103">Create windows81VpnConfiguration</span></span>

> <span data-ttu-id="ae462-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ae462-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ae462-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="ae462-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ae462-106">Erstellen eines neuen [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="ae462-106">Create a new [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ae462-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="ae462-107">Prerequisites</span></span>
<span data-ttu-id="ae462-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="ae462-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="ae462-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ae462-110">Permission type</span></span>|<span data-ttu-id="ae462-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ae462-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ae462-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ae462-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ae462-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae462-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ae462-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ae462-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ae462-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ae462-115">Not supported.</span></span>|
|<span data-ttu-id="ae462-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ae462-116">Application</span></span>|<span data-ttu-id="ae462-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ae462-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ae462-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ae462-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="ae462-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ae462-119">Request headers</span></span>
|<span data-ttu-id="ae462-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="ae462-120">Header</span></span>|<span data-ttu-id="ae462-121">Wert</span><span class="sxs-lookup"><span data-stu-id="ae462-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ae462-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ae462-122">Authorization</span></span>|<span data-ttu-id="ae462-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="ae462-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ae462-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="ae462-124">Accept</span></span>|<span data-ttu-id="ae462-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ae462-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ae462-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ae462-126">Request body</span></span>
<span data-ttu-id="ae462-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das windows81VpnConfiguration-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="ae462-127">In the request body, supply a JSON representation for the windows81VpnConfiguration object.</span></span>

<span data-ttu-id="ae462-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der windows81VpnConfiguration erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="ae462-128">The following table shows the properties that are required when you create the windows81VpnConfiguration.</span></span>

|<span data-ttu-id="ae462-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ae462-129">Property</span></span>|<span data-ttu-id="ae462-130">Typ</span><span class="sxs-lookup"><span data-stu-id="ae462-130">Type</span></span>|<span data-ttu-id="ae462-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ae462-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ae462-132">id</span><span class="sxs-lookup"><span data-stu-id="ae462-132">id</span></span>|<span data-ttu-id="ae462-133">string</span><span class="sxs-lookup"><span data-stu-id="ae462-133">String</span></span>|<span data-ttu-id="ae462-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="ae462-134">Key of the entity.</span></span> <span data-ttu-id="ae462-135">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ae462-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ae462-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ae462-136">lastModifiedDateTime</span></span>|<span data-ttu-id="ae462-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ae462-137">DateTimeOffset</span></span>|<span data-ttu-id="ae462-138">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="ae462-138">DateTime the object was last modified.</span></span> <span data-ttu-id="ae462-139">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ae462-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ae462-140">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="ae462-140">roleScopeTagIds</span></span>|<span data-ttu-id="ae462-141">String collection</span><span class="sxs-lookup"><span data-stu-id="ae462-141">String collection</span></span>|<span data-ttu-id="ae462-142">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="ae462-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ae462-143">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ae462-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ae462-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="ae462-144">supportsScopeTags</span></span>|<span data-ttu-id="ae462-145">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="ae462-145">Boolean</span></span>|<span data-ttu-id="ae462-146">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereichs Tags unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ae462-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="ae462-147">Das Zuweisen zur ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert auf false festgelegt ist und Entitäten für bereichsbezogene Benutzer nicht sichtbar sind.</span><span class="sxs-lookup"><span data-stu-id="ae462-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="ae462-148">Dies geschieht für in Silverlight erstellte Legacy Richtlinien und kann durch Löschen und erneutes Erstellen der Richtlinie im Azure-Portal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="ae462-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="ae462-149">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="ae462-149">This property is read-only.</span></span> <span data-ttu-id="ae462-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ae462-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ae462-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ae462-151">createdDateTime</span></span>|<span data-ttu-id="ae462-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ae462-152">DateTimeOffset</span></span>|<span data-ttu-id="ae462-153">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="ae462-153">DateTime the object was created.</span></span> <span data-ttu-id="ae462-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ae462-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ae462-155">description</span><span class="sxs-lookup"><span data-stu-id="ae462-155">description</span></span>|<span data-ttu-id="ae462-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ae462-156">String</span></span>|<span data-ttu-id="ae462-157">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="ae462-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ae462-158">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ae462-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ae462-159">displayName</span><span class="sxs-lookup"><span data-stu-id="ae462-159">displayName</span></span>|<span data-ttu-id="ae462-160">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ae462-160">String</span></span>|<span data-ttu-id="ae462-161">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="ae462-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ae462-162">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ae462-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ae462-163">Version</span><span class="sxs-lookup"><span data-stu-id="ae462-163">version</span></span>|<span data-ttu-id="ae462-164">Int32</span><span class="sxs-lookup"><span data-stu-id="ae462-164">Int32</span></span>|<span data-ttu-id="ae462-165">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="ae462-165">Version of the device configuration.</span></span> <span data-ttu-id="ae462-166">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ae462-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ae462-167">connectionName</span><span class="sxs-lookup"><span data-stu-id="ae462-167">connectionName</span></span>|<span data-ttu-id="ae462-168">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ae462-168">String</span></span>|<span data-ttu-id="ae462-169">Dem Benutzer angezeigter Verbindungsname.</span><span class="sxs-lookup"><span data-stu-id="ae462-169">Connection name displayed to the user.</span></span> <span data-ttu-id="ae462-170">Geerbt von [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ae462-170">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="ae462-171">Server</span><span class="sxs-lookup"><span data-stu-id="ae462-171">servers</span></span>|<span data-ttu-id="ae462-172">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="ae462-172">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="ae462-173">Liste der VPN-Server im Netzwerk.</span><span class="sxs-lookup"><span data-stu-id="ae462-173">List of VPN Servers on the network.</span></span> <span data-ttu-id="ae462-174">Stellen Sie sicher, dass Endbenutzer auf diese Netzwerkspeicherorte zugreifen können.</span><span class="sxs-lookup"><span data-stu-id="ae462-174">Make sure end users can access these network locations.</span></span> <span data-ttu-id="ae462-175">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="ae462-175">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="ae462-176">Geerbt von [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ae462-176">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="ae462-177">customXml</span><span class="sxs-lookup"><span data-stu-id="ae462-177">customXml</span></span>|<span data-ttu-id="ae462-178">Binär</span><span class="sxs-lookup"><span data-stu-id="ae462-178">Binary</span></span>|<span data-ttu-id="ae462-179">Benutzerdefinierte XML-Befehle, mit denen die VPN-Verbindung konfiguriert wird.</span><span class="sxs-lookup"><span data-stu-id="ae462-179">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="ae462-180">(UTF8-codiertes Bytearray) Geerbt von [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ae462-180">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="ae462-181">applyOnlyToWindows81</span><span class="sxs-lookup"><span data-stu-id="ae462-181">applyOnlyToWindows81</span></span>|<span data-ttu-id="ae462-182">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="ae462-182">Boolean</span></span>|<span data-ttu-id="ae462-183">Wert, der angibt, ob die Richtlinie nur für Windows 8.1 gilt.</span><span class="sxs-lookup"><span data-stu-id="ae462-183">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="ae462-184">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="ae462-184">This property is read-only.</span></span>|
|<span data-ttu-id="ae462-185">connectionType</span><span class="sxs-lookup"><span data-stu-id="ae462-185">connectionType</span></span>|[<span data-ttu-id="ae462-186">windowsVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="ae462-186">windowsVpnConnectionType</span></span>](../resources/intune-deviceconfig-windowsvpnconnectiontype.md)|<span data-ttu-id="ae462-187">Verbindungstyp.</span><span class="sxs-lookup"><span data-stu-id="ae462-187">Connection type.</span></span> <span data-ttu-id="ae462-188">Mögliche Werte: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`.</span><span class="sxs-lookup"><span data-stu-id="ae462-188">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`.</span></span>|
|<span data-ttu-id="ae462-189">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="ae462-189">loginGroupOrDomain</span></span>|<span data-ttu-id="ae462-190">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ae462-190">String</span></span>|<span data-ttu-id="ae462-191">Anmeldegruppe oder Domäne, wenn der Verbindungstyp auf Dell SonicWALL Mobile Connection festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="ae462-191">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span>|
|<span data-ttu-id="ae462-192">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="ae462-192">enableSplitTunneling</span></span>|<span data-ttu-id="ae462-193">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="ae462-193">Boolean</span></span>|<span data-ttu-id="ae462-194">Aktivieren Sie den geteilten Tunnel für das VPN.</span><span class="sxs-lookup"><span data-stu-id="ae462-194">Enable split tunneling for the VPN.</span></span>|
|<span data-ttu-id="ae462-195">Sie</span><span class="sxs-lookup"><span data-stu-id="ae462-195">proxyServer</span></span>|[<span data-ttu-id="ae462-196">windows81VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="ae462-196">windows81VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows81vpnproxyserver.md)|<span data-ttu-id="ae462-197">Proxy Server.</span><span class="sxs-lookup"><span data-stu-id="ae462-197">Proxy Server.</span></span>|



## <a name="response"></a><span data-ttu-id="ae462-198">Antwort</span><span class="sxs-lookup"><span data-stu-id="ae462-198">Response</span></span>
<span data-ttu-id="ae462-199">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="ae462-199">If successful, this method returns a `201 Created` response code and a [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ae462-200">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ae462-200">Example</span></span>

### <a name="request"></a><span data-ttu-id="ae462-201">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ae462-201">Request</span></span>
<span data-ttu-id="ae462-202">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ae462-202">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1015

{
  "@odata.type": "#microsoft.graph.windows81VpnConfiguration",
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

### <a name="response"></a><span data-ttu-id="ae462-203">Antwort</span><span class="sxs-lookup"><span data-stu-id="ae462-203">Response</span></span>
<span data-ttu-id="ae462-p115">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ae462-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




