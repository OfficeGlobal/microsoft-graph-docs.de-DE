---
title: Erstellen von windows81VpnConfiguration
description: Erstellen eines neuen windows81VpnConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e036ac960cf90d11987f88a19137b443dd4e178c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27975911"
---
# <a name="create-windows81vpnconfiguration"></a><span data-ttu-id="a654f-103">Erstellen von windows81VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="a654f-103">Create windows81VpnConfiguration</span></span>

> <span data-ttu-id="a654f-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="a654f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a654f-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a654f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a654f-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="a654f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a654f-107">Erstellen eines neuen [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="a654f-107">Create a new [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a654f-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="a654f-108">Prerequisites</span></span>
<span data-ttu-id="a654f-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a654f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a654f-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a654f-111">Permission type</span></span>|<span data-ttu-id="a654f-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a654f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a654f-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a654f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a654f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a654f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a654f-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a654f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a654f-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a654f-116">Not supported.</span></span>|
|<span data-ttu-id="a654f-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a654f-117">Application</span></span>|<span data-ttu-id="a654f-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a654f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a654f-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a654f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a654f-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a654f-120">Request headers</span></span>
|<span data-ttu-id="a654f-121">Header</span><span class="sxs-lookup"><span data-stu-id="a654f-121">Header</span></span>|<span data-ttu-id="a654f-122">Wert</span><span class="sxs-lookup"><span data-stu-id="a654f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a654f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a654f-123">Authorization</span></span>|<span data-ttu-id="a654f-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="a654f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a654f-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="a654f-125">Accept</span></span>|<span data-ttu-id="a654f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a654f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a654f-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a654f-127">Request body</span></span>
<span data-ttu-id="a654f-128">Geben Sie im Textkörper Anforderung für das Objekt windows81VpnConfiguration eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="a654f-128">In the request body, supply a JSON representation for the windows81VpnConfiguration object.</span></span>

<span data-ttu-id="a654f-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die windows81VpnConfiguration erstellen.</span><span class="sxs-lookup"><span data-stu-id="a654f-129">The following table shows the properties that are required when you create the windows81VpnConfiguration.</span></span>

|<span data-ttu-id="a654f-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a654f-130">Property</span></span>|<span data-ttu-id="a654f-131">Typ</span><span class="sxs-lookup"><span data-stu-id="a654f-131">Type</span></span>|<span data-ttu-id="a654f-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a654f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a654f-133">id</span><span class="sxs-lookup"><span data-stu-id="a654f-133">id</span></span>|<span data-ttu-id="a654f-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a654f-134">String</span></span>|<span data-ttu-id="a654f-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="a654f-135">Key of the entity.</span></span> <span data-ttu-id="a654f-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a654f-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a654f-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a654f-137">lastModifiedDateTime</span></span>|<span data-ttu-id="a654f-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a654f-138">DateTimeOffset</span></span>|<span data-ttu-id="a654f-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="a654f-139">DateTime the object was last modified.</span></span> <span data-ttu-id="a654f-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a654f-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a654f-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a654f-141">roleScopeTagIds</span></span>|<span data-ttu-id="a654f-142">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="a654f-142">String collection</span></span>|<span data-ttu-id="a654f-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="a654f-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a654f-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a654f-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a654f-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="a654f-145">supportsScopeTags</span></span>|<span data-ttu-id="a654f-146">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="a654f-146">Boolean</span></span>|<span data-ttu-id="a654f-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a654f-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="a654f-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="a654f-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="a654f-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="a654f-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="a654f-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="a654f-150">This property is read-only.</span></span> <span data-ttu-id="a654f-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a654f-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a654f-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a654f-152">createdDateTime</span></span>|<span data-ttu-id="a654f-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a654f-153">DateTimeOffset</span></span>|<span data-ttu-id="a654f-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="a654f-154">DateTime the object was created.</span></span> <span data-ttu-id="a654f-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a654f-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a654f-156">description</span><span class="sxs-lookup"><span data-stu-id="a654f-156">description</span></span>|<span data-ttu-id="a654f-157">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a654f-157">String</span></span>|<span data-ttu-id="a654f-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="a654f-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a654f-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a654f-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a654f-160">displayName</span><span class="sxs-lookup"><span data-stu-id="a654f-160">displayName</span></span>|<span data-ttu-id="a654f-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a654f-161">String</span></span>|<span data-ttu-id="a654f-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="a654f-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a654f-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a654f-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a654f-164">Version</span><span class="sxs-lookup"><span data-stu-id="a654f-164">version</span></span>|<span data-ttu-id="a654f-165">Int32</span><span class="sxs-lookup"><span data-stu-id="a654f-165">Int32</span></span>|<span data-ttu-id="a654f-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="a654f-166">Version of the device configuration.</span></span> <span data-ttu-id="a654f-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a654f-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a654f-168">connectionName</span><span class="sxs-lookup"><span data-stu-id="a654f-168">connectionName</span></span>|<span data-ttu-id="a654f-169">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a654f-169">String</span></span>|<span data-ttu-id="a654f-170">Name der Verbindung für den Benutzer angezeigt.</span><span class="sxs-lookup"><span data-stu-id="a654f-170">Connection name displayed to the user.</span></span> <span data-ttu-id="a654f-171">Geerbt von [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a654f-171">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="a654f-172">Server</span><span class="sxs-lookup"><span data-stu-id="a654f-172">servers</span></span>|<span data-ttu-id="a654f-173">[VpnServer](../resources/intune-deviceconfig-vpnserver.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="a654f-173">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="a654f-174">Liste der VPN-Server im Netzwerk.</span><span class="sxs-lookup"><span data-stu-id="a654f-174">List of VPN Servers on the network.</span></span> <span data-ttu-id="a654f-175">Stellen Sie sicher, dass Endbenutzer diese Netzwerkadressen zugreifen können.</span><span class="sxs-lookup"><span data-stu-id="a654f-175">Make sure end users can access these network locations.</span></span> <span data-ttu-id="a654f-176">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="a654f-176">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="a654f-177">Geerbt von [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a654f-177">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="a654f-178">customXml</span><span class="sxs-lookup"><span data-stu-id="a654f-178">customXml</span></span>|<span data-ttu-id="a654f-179">Binär</span><span class="sxs-lookup"><span data-stu-id="a654f-179">Binary</span></span>|<span data-ttu-id="a654f-180">Benutzerdefinierte XML-Befehle, die die VPN-Verbindung konfiguriert.</span><span class="sxs-lookup"><span data-stu-id="a654f-180">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="a654f-181">(UTF8 codiert Bytearray) Geerbt von [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a654f-181">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="a654f-182">applyOnlyToWindows81</span><span class="sxs-lookup"><span data-stu-id="a654f-182">applyOnlyToWindows81</span></span>|<span data-ttu-id="a654f-183">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="a654f-183">Boolean</span></span>|<span data-ttu-id="a654f-184">Wert, der angibt, ob die Richtlinie nur für Windows 8.1 gilt.</span><span class="sxs-lookup"><span data-stu-id="a654f-184">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="a654f-185">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="a654f-185">This property is read-only.</span></span>|
|<span data-ttu-id="a654f-186">connectionType</span><span class="sxs-lookup"><span data-stu-id="a654f-186">connectionType</span></span>|[<span data-ttu-id="a654f-187">windowsVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="a654f-187">windowsVpnConnectionType</span></span>](../resources/intune-deviceconfig-windowsvpnconnectiontype.md)|<span data-ttu-id="a654f-188">Verbindungstyp.</span><span class="sxs-lookup"><span data-stu-id="a654f-188">Connection type.</span></span> <span data-ttu-id="a654f-189">Mögliche Werte: sind `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect` und `checkPointCapsuleVpn`.</span><span class="sxs-lookup"><span data-stu-id="a654f-189">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`.</span></span>|
|<span data-ttu-id="a654f-190">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="a654f-190">loginGroupOrDomain</span></span>|<span data-ttu-id="a654f-191">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a654f-191">String</span></span>|<span data-ttu-id="a654f-192">Anmeldegruppe oder Domäne Wenn Verbindungstyp auf Dell SonicWALL Mobile Verbindung festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="a654f-192">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span>|
|<span data-ttu-id="a654f-193">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="a654f-193">enableSplitTunneling</span></span>|<span data-ttu-id="a654f-194">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="a654f-194">Boolean</span></span>|<span data-ttu-id="a654f-195">Aktivieren Sie die Split-tunneling für das VPN.</span><span class="sxs-lookup"><span data-stu-id="a654f-195">Enable split tunneling for the VPN.</span></span>|
|<span data-ttu-id="a654f-196">proxyServer</span><span class="sxs-lookup"><span data-stu-id="a654f-196">proxyServer</span></span>|[<span data-ttu-id="a654f-197">windows81VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="a654f-197">windows81VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows81vpnproxyserver.md)|<span data-ttu-id="a654f-198">Proxy-Server.</span><span class="sxs-lookup"><span data-stu-id="a654f-198">Proxy Server.</span></span>|



## <a name="response"></a><span data-ttu-id="a654f-199">Antwort</span><span class="sxs-lookup"><span data-stu-id="a654f-199">Response</span></span>
<span data-ttu-id="a654f-200">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="a654f-200">If successful, this method returns a `201 Created` response code and a [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a654f-201">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a654f-201">Example</span></span>
### <a name="request"></a><span data-ttu-id="a654f-202">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a654f-202">Request</span></span>
<span data-ttu-id="a654f-203">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a654f-203">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a654f-204">Antwort</span><span class="sxs-lookup"><span data-stu-id="a654f-204">Response</span></span>
<span data-ttu-id="a654f-p116">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a654f-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





