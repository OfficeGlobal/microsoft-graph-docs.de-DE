---
title: Windows81VpnConfiguration aktualisieren
description: Aktualisieren Sie die Eigenschaften eines windows81VpnConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: cae55e29bf6dd56e86b5771660a720bfb862cc2c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27838724"
---
# <a name="update-windows81vpnconfiguration"></a><span data-ttu-id="6f803-103">Windows81VpnConfiguration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="6f803-103">Update windows81VpnConfiguration</span></span>

> <span data-ttu-id="6f803-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="6f803-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6f803-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6f803-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6f803-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="6f803-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6f803-107">Aktualisieren Sie die Eigenschaften eines [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="6f803-107">Update the properties of a [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6f803-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="6f803-108">Prerequisites</span></span>
<span data-ttu-id="6f803-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6f803-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6f803-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6f803-111">Permission type</span></span>|<span data-ttu-id="6f803-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6f803-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6f803-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6f803-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6f803-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f803-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6f803-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6f803-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6f803-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6f803-116">Not supported.</span></span>|
|<span data-ttu-id="6f803-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6f803-117">Application</span></span>|<span data-ttu-id="6f803-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6f803-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6f803-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6f803-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="6f803-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6f803-120">Request headers</span></span>
|<span data-ttu-id="6f803-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="6f803-121">Header</span></span>|<span data-ttu-id="6f803-122">Wert</span><span class="sxs-lookup"><span data-stu-id="6f803-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6f803-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6f803-123">Authorization</span></span>|<span data-ttu-id="6f803-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="6f803-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6f803-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="6f803-125">Accept</span></span>|<span data-ttu-id="6f803-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6f803-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6f803-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6f803-127">Request body</span></span>
<span data-ttu-id="6f803-128">Geben Sie im Textkörper Anforderung für das Objekt [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="6f803-128">In the request body, supply a JSON representation for the [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) object.</span></span>

<span data-ttu-id="6f803-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="6f803-129">The following table shows the properties that are required when you create the [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md).</span></span>

|<span data-ttu-id="6f803-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6f803-130">Property</span></span>|<span data-ttu-id="6f803-131">Typ</span><span class="sxs-lookup"><span data-stu-id="6f803-131">Type</span></span>|<span data-ttu-id="6f803-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6f803-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6f803-133">id</span><span class="sxs-lookup"><span data-stu-id="6f803-133">id</span></span>|<span data-ttu-id="6f803-134">String</span><span class="sxs-lookup"><span data-stu-id="6f803-134">String</span></span>|<span data-ttu-id="6f803-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="6f803-135">Key of the entity.</span></span> <span data-ttu-id="6f803-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6f803-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f803-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6f803-137">lastModifiedDateTime</span></span>|<span data-ttu-id="6f803-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6f803-138">DateTimeOffset</span></span>|<span data-ttu-id="6f803-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="6f803-139">DateTime the object was last modified.</span></span> <span data-ttu-id="6f803-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6f803-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f803-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6f803-141">roleScopeTagIds</span></span>|<span data-ttu-id="6f803-142">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="6f803-142">String collection</span></span>|<span data-ttu-id="6f803-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="6f803-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="6f803-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6f803-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f803-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="6f803-145">supportsScopeTags</span></span>|<span data-ttu-id="6f803-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f803-146">Boolean</span></span>|<span data-ttu-id="6f803-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6f803-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="6f803-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="6f803-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="6f803-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="6f803-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="6f803-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="6f803-150">This property is read-only.</span></span> <span data-ttu-id="6f803-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6f803-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f803-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6f803-152">createdDateTime</span></span>|<span data-ttu-id="6f803-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6f803-153">DateTimeOffset</span></span>|<span data-ttu-id="6f803-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="6f803-154">DateTime the object was created.</span></span> <span data-ttu-id="6f803-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6f803-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f803-156">description</span><span class="sxs-lookup"><span data-stu-id="6f803-156">description</span></span>|<span data-ttu-id="6f803-157">String</span><span class="sxs-lookup"><span data-stu-id="6f803-157">String</span></span>|<span data-ttu-id="6f803-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="6f803-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6f803-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6f803-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f803-160">displayName</span><span class="sxs-lookup"><span data-stu-id="6f803-160">displayName</span></span>|<span data-ttu-id="6f803-161">String</span><span class="sxs-lookup"><span data-stu-id="6f803-161">String</span></span>|<span data-ttu-id="6f803-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="6f803-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6f803-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6f803-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f803-164">Version</span><span class="sxs-lookup"><span data-stu-id="6f803-164">version</span></span>|<span data-ttu-id="6f803-165">Int32</span><span class="sxs-lookup"><span data-stu-id="6f803-165">Int32</span></span>|<span data-ttu-id="6f803-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="6f803-166">Version of the device configuration.</span></span> <span data-ttu-id="6f803-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6f803-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f803-168">connectionName</span><span class="sxs-lookup"><span data-stu-id="6f803-168">connectionName</span></span>|<span data-ttu-id="6f803-169">String</span><span class="sxs-lookup"><span data-stu-id="6f803-169">String</span></span>|<span data-ttu-id="6f803-170">Name der Verbindung für den Benutzer angezeigt.</span><span class="sxs-lookup"><span data-stu-id="6f803-170">Connection name displayed to the user.</span></span> <span data-ttu-id="6f803-171">Geerbt von [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6f803-171">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="6f803-172">Server</span><span class="sxs-lookup"><span data-stu-id="6f803-172">servers</span></span>|<span data-ttu-id="6f803-173">[VpnServer](../resources/intune-deviceconfig-vpnserver.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="6f803-173">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="6f803-174">Liste der VPN-Server im Netzwerk.</span><span class="sxs-lookup"><span data-stu-id="6f803-174">List of VPN Servers on the network.</span></span> <span data-ttu-id="6f803-175">Stellen Sie sicher, dass Endbenutzer diese Netzwerkadressen zugreifen können.</span><span class="sxs-lookup"><span data-stu-id="6f803-175">Make sure end users can access these network locations.</span></span> <span data-ttu-id="6f803-176">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="6f803-176">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="6f803-177">Geerbt von [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6f803-177">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="6f803-178">customXml</span><span class="sxs-lookup"><span data-stu-id="6f803-178">customXml</span></span>|<span data-ttu-id="6f803-179">Binär</span><span class="sxs-lookup"><span data-stu-id="6f803-179">Binary</span></span>|<span data-ttu-id="6f803-180">Benutzerdefinierte XML-Befehle, die die VPN-Verbindung konfiguriert.</span><span class="sxs-lookup"><span data-stu-id="6f803-180">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="6f803-181">(UTF8 codiert Bytearray) Geerbt von [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6f803-181">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="6f803-182">applyOnlyToWindows81</span><span class="sxs-lookup"><span data-stu-id="6f803-182">applyOnlyToWindows81</span></span>|<span data-ttu-id="6f803-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f803-183">Boolean</span></span>|<span data-ttu-id="6f803-184">Wert, der angibt, ob die Richtlinie nur für Windows 8.1 gilt.</span><span class="sxs-lookup"><span data-stu-id="6f803-184">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="6f803-185">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="6f803-185">This property is read-only.</span></span>|
|<span data-ttu-id="6f803-186">connectionType</span><span class="sxs-lookup"><span data-stu-id="6f803-186">connectionType</span></span>|[<span data-ttu-id="6f803-187">windowsVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="6f803-187">windowsVpnConnectionType</span></span>](../resources/intune-deviceconfig-windowsvpnconnectiontype.md)|<span data-ttu-id="6f803-188">Verbindungstyp.</span><span class="sxs-lookup"><span data-stu-id="6f803-188">Connection type.</span></span> <span data-ttu-id="6f803-189">Mögliche Werte: sind `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect` und `checkPointCapsuleVpn`.</span><span class="sxs-lookup"><span data-stu-id="6f803-189">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`.</span></span>|
|<span data-ttu-id="6f803-190">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="6f803-190">loginGroupOrDomain</span></span>|<span data-ttu-id="6f803-191">String</span><span class="sxs-lookup"><span data-stu-id="6f803-191">String</span></span>|<span data-ttu-id="6f803-192">Anmeldegruppe oder Domäne Wenn Verbindungstyp auf Dell SonicWALL Mobile Verbindung festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="6f803-192">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span>|
|<span data-ttu-id="6f803-193">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="6f803-193">enableSplitTunneling</span></span>|<span data-ttu-id="6f803-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f803-194">Boolean</span></span>|<span data-ttu-id="6f803-195">Aktivieren Sie die Split-tunneling für das VPN.</span><span class="sxs-lookup"><span data-stu-id="6f803-195">Enable split tunneling for the VPN.</span></span>|
|<span data-ttu-id="6f803-196">proxyServer</span><span class="sxs-lookup"><span data-stu-id="6f803-196">proxyServer</span></span>|[<span data-ttu-id="6f803-197">windows81VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="6f803-197">windows81VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows81vpnproxyserver.md)|<span data-ttu-id="6f803-198">Proxy-Server.</span><span class="sxs-lookup"><span data-stu-id="6f803-198">Proxy Server.</span></span>|



## <a name="response"></a><span data-ttu-id="6f803-199">Antwort</span><span class="sxs-lookup"><span data-stu-id="6f803-199">Response</span></span>
<span data-ttu-id="6f803-200">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="6f803-200">If successful, this method returns a `200 OK` response code and an updated [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6f803-201">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6f803-201">Example</span></span>
### <a name="request"></a><span data-ttu-id="6f803-202">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6f803-202">Request</span></span>
<span data-ttu-id="6f803-203">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6f803-203">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1015

{
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

### <a name="response"></a><span data-ttu-id="6f803-204">Antwort</span><span class="sxs-lookup"><span data-stu-id="6f803-204">Response</span></span>
<span data-ttu-id="6f803-p116">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6f803-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





