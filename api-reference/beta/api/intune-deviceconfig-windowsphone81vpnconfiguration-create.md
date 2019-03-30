---
title: WindowsPhone81VpnConfiguration erstellen
description: Erstellen eines neuen windowsPhone81VpnConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 794c16ecf9ffd92e60536dc261b7114e166742ea
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30985410"
---
# <a name="create-windowsphone81vpnconfiguration"></a><span data-ttu-id="c5853-103">WindowsPhone81VpnConfiguration erstellen</span><span class="sxs-lookup"><span data-stu-id="c5853-103">Create windowsPhone81VpnConfiguration</span></span>

> <span data-ttu-id="c5853-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c5853-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c5853-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="c5853-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c5853-106">Erstellen eines neuen [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="c5853-106">Create a new [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c5853-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c5853-107">Prerequisites</span></span>
<span data-ttu-id="c5853-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c5853-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c5853-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c5853-110">Permission type</span></span>|<span data-ttu-id="c5853-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c5853-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c5853-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c5853-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c5853-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5853-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c5853-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c5853-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c5853-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c5853-115">Not supported.</span></span>|
|<span data-ttu-id="c5853-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c5853-116">Application</span></span>|<span data-ttu-id="c5853-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c5853-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c5853-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c5853-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="c5853-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c5853-119">Request headers</span></span>
|<span data-ttu-id="c5853-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="c5853-120">Header</span></span>|<span data-ttu-id="c5853-121">Wert</span><span class="sxs-lookup"><span data-stu-id="c5853-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c5853-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c5853-122">Authorization</span></span>|<span data-ttu-id="c5853-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c5853-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c5853-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="c5853-124">Accept</span></span>|<span data-ttu-id="c5853-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c5853-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c5853-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c5853-126">Request body</span></span>
<span data-ttu-id="c5853-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das windowsPhone81VpnConfiguration-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="c5853-127">In the request body, supply a JSON representation for the windowsPhone81VpnConfiguration object.</span></span>

<span data-ttu-id="c5853-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der windowsPhone81VpnConfiguration erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="c5853-128">The following table shows the properties that are required when you create the windowsPhone81VpnConfiguration.</span></span>

|<span data-ttu-id="c5853-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c5853-129">Property</span></span>|<span data-ttu-id="c5853-130">Typ</span><span class="sxs-lookup"><span data-stu-id="c5853-130">Type</span></span>|<span data-ttu-id="c5853-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c5853-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c5853-132">id</span><span class="sxs-lookup"><span data-stu-id="c5853-132">id</span></span>|<span data-ttu-id="c5853-133">String</span><span class="sxs-lookup"><span data-stu-id="c5853-133">String</span></span>|<span data-ttu-id="c5853-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="c5853-134">Key of the entity.</span></span> <span data-ttu-id="c5853-135">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c5853-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c5853-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c5853-136">lastModifiedDateTime</span></span>|<span data-ttu-id="c5853-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c5853-137">DateTimeOffset</span></span>|<span data-ttu-id="c5853-138">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="c5853-138">DateTime the object was last modified.</span></span> <span data-ttu-id="c5853-139">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c5853-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c5853-140">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="c5853-140">roleScopeTagIds</span></span>|<span data-ttu-id="c5853-141">String collection</span><span class="sxs-lookup"><span data-stu-id="c5853-141">String collection</span></span>|<span data-ttu-id="c5853-142">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="c5853-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c5853-143">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c5853-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c5853-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="c5853-144">supportsScopeTags</span></span>|<span data-ttu-id="c5853-145">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c5853-145">Boolean</span></span>|<span data-ttu-id="c5853-146">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereichs Tags unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c5853-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="c5853-147">Das Zuweisen zur ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert auf false festgelegt ist und Entitäten für bereichsbezogene Benutzer nicht sichtbar sind.</span><span class="sxs-lookup"><span data-stu-id="c5853-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="c5853-148">Dies geschieht für in Silverlight erstellte Legacy Richtlinien und kann durch Löschen und erneutes Erstellen der Richtlinie im Azure-Portal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="c5853-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="c5853-149">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="c5853-149">This property is read-only.</span></span> <span data-ttu-id="c5853-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c5853-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c5853-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c5853-151">createdDateTime</span></span>|<span data-ttu-id="c5853-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c5853-152">DateTimeOffset</span></span>|<span data-ttu-id="c5853-153">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="c5853-153">DateTime the object was created.</span></span> <span data-ttu-id="c5853-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c5853-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c5853-155">description</span><span class="sxs-lookup"><span data-stu-id="c5853-155">description</span></span>|<span data-ttu-id="c5853-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c5853-156">String</span></span>|<span data-ttu-id="c5853-157">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="c5853-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c5853-158">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c5853-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c5853-159">displayName</span><span class="sxs-lookup"><span data-stu-id="c5853-159">displayName</span></span>|<span data-ttu-id="c5853-160">String</span><span class="sxs-lookup"><span data-stu-id="c5853-160">String</span></span>|<span data-ttu-id="c5853-161">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="c5853-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c5853-162">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c5853-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c5853-163">Version</span><span class="sxs-lookup"><span data-stu-id="c5853-163">version</span></span>|<span data-ttu-id="c5853-164">Int32</span><span class="sxs-lookup"><span data-stu-id="c5853-164">Int32</span></span>|<span data-ttu-id="c5853-165">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="c5853-165">Version of the device configuration.</span></span> <span data-ttu-id="c5853-166">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c5853-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c5853-167">connectionName</span><span class="sxs-lookup"><span data-stu-id="c5853-167">connectionName</span></span>|<span data-ttu-id="c5853-168">String</span><span class="sxs-lookup"><span data-stu-id="c5853-168">String</span></span>|<span data-ttu-id="c5853-169">Dem Benutzer angezeigter Verbindungsname.</span><span class="sxs-lookup"><span data-stu-id="c5853-169">Connection name displayed to the user.</span></span> <span data-ttu-id="c5853-170">Geerbt von [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c5853-170">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="c5853-171">Server</span><span class="sxs-lookup"><span data-stu-id="c5853-171">servers</span></span>|<span data-ttu-id="c5853-172">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="c5853-172">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="c5853-173">Liste der VPN-Server im Netzwerk.</span><span class="sxs-lookup"><span data-stu-id="c5853-173">List of VPN Servers on the network.</span></span> <span data-ttu-id="c5853-174">Stellen Sie sicher, dass Endbenutzer auf diese Netzwerkspeicherorte zugreifen können.</span><span class="sxs-lookup"><span data-stu-id="c5853-174">Make sure end users can access these network locations.</span></span> <span data-ttu-id="c5853-175">Diese Sammlung darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="c5853-175">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="c5853-176">Geerbt von [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c5853-176">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="c5853-177">customXml</span><span class="sxs-lookup"><span data-stu-id="c5853-177">customXml</span></span>|<span data-ttu-id="c5853-178">Binär</span><span class="sxs-lookup"><span data-stu-id="c5853-178">Binary</span></span>|<span data-ttu-id="c5853-179">Benutzerdefinierte XML-Befehle, mit denen die VPN-Verbindung konfiguriert wird.</span><span class="sxs-lookup"><span data-stu-id="c5853-179">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="c5853-180">(UTF8-codiertes Bytearray) Geerbt von [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c5853-180">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="c5853-181">applyOnlyToWindows81</span><span class="sxs-lookup"><span data-stu-id="c5853-181">applyOnlyToWindows81</span></span>|<span data-ttu-id="c5853-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5853-182">Boolean</span></span>|<span data-ttu-id="c5853-183">Wert, der angibt, ob die Richtlinie nur für Windows 8.1 gilt.</span><span class="sxs-lookup"><span data-stu-id="c5853-183">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="c5853-184">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="c5853-184">This property is read-only.</span></span> <span data-ttu-id="c5853-185">Geerbt von [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c5853-185">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="c5853-186">connectionType</span><span class="sxs-lookup"><span data-stu-id="c5853-186">connectionType</span></span>|[<span data-ttu-id="c5853-187">windowsVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="c5853-187">windowsVpnConnectionType</span></span>](../resources/intune-deviceconfig-windowsvpnconnectiontype.md)|<span data-ttu-id="c5853-188">Verbindungstyp.</span><span class="sxs-lookup"><span data-stu-id="c5853-188">Connection type.</span></span> <span data-ttu-id="c5853-189">Von [Windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="c5853-189">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md).</span></span> <span data-ttu-id="c5853-190">Mögliche Werte sind: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect` und `checkPointCapsuleVpn`.</span><span class="sxs-lookup"><span data-stu-id="c5853-190">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`.</span></span>|
|<span data-ttu-id="c5853-191">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="c5853-191">loginGroupOrDomain</span></span>|<span data-ttu-id="c5853-192">String</span><span class="sxs-lookup"><span data-stu-id="c5853-192">String</span></span>|<span data-ttu-id="c5853-193">Anmeldegruppe oder Domäne, wenn der Verbindungstyp auf Dell SonicWALL Mobile Connection festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="c5853-193">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="c5853-194">Geerbt von [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c5853-194">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="c5853-195">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="c5853-195">enableSplitTunneling</span></span>|<span data-ttu-id="c5853-196">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c5853-196">Boolean</span></span>|<span data-ttu-id="c5853-197">Aktivieren Sie den geteilten Tunnel für das VPN.</span><span class="sxs-lookup"><span data-stu-id="c5853-197">Enable split tunneling for the VPN.</span></span> <span data-ttu-id="c5853-198">Geerbt von [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c5853-198">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="c5853-199">Sie</span><span class="sxs-lookup"><span data-stu-id="c5853-199">proxyServer</span></span>|[<span data-ttu-id="c5853-200">windows81VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="c5853-200">windows81VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows81vpnproxyserver.md)|<span data-ttu-id="c5853-201">Proxy Server.</span><span class="sxs-lookup"><span data-stu-id="c5853-201">Proxy Server.</span></span> <span data-ttu-id="c5853-202">Geerbt von [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c5853-202">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="c5853-203">bypassVpnOnCompanyWifi</span><span class="sxs-lookup"><span data-stu-id="c5853-203">bypassVpnOnCompanyWifi</span></span>|<span data-ttu-id="c5853-204">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c5853-204">Boolean</span></span>|<span data-ttu-id="c5853-205">Bypass VPN on Company Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="c5853-205">Bypass VPN on company Wi-Fi.</span></span>|
|<span data-ttu-id="c5853-206">bypassVpnOnHomeWifi</span><span class="sxs-lookup"><span data-stu-id="c5853-206">bypassVpnOnHomeWifi</span></span>|<span data-ttu-id="c5853-207">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c5853-207">Boolean</span></span>|<span data-ttu-id="c5853-208">Bypass VPN on Home Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="c5853-208">Bypass VPN on home Wi-Fi.</span></span>|
|<span data-ttu-id="c5853-209">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="c5853-209">authenticationMethod</span></span>|[<span data-ttu-id="c5853-210">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="c5853-210">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="c5853-211">Authentifizierungsmethode.</span><span class="sxs-lookup"><span data-stu-id="c5853-211">Authentication method.</span></span> <span data-ttu-id="c5853-212">Mögliche Werte sind: `certificate` und `usernameAndPassword`.</span><span class="sxs-lookup"><span data-stu-id="c5853-212">Possible values are: `certificate`, `usernameAndPassword`.</span></span>|
|<span data-ttu-id="c5853-213">rememberUserCredentials</span><span class="sxs-lookup"><span data-stu-id="c5853-213">rememberUserCredentials</span></span>|<span data-ttu-id="c5853-214">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c5853-214">Boolean</span></span>|<span data-ttu-id="c5853-215">Denken Sie an Benutzeranmeldeinformationen.</span><span class="sxs-lookup"><span data-stu-id="c5853-215">Remember user credentials.</span></span>|
|<span data-ttu-id="c5853-216">dnsSuffixSearchList</span><span class="sxs-lookup"><span data-stu-id="c5853-216">dnsSuffixSearchList</span></span>|<span data-ttu-id="c5853-217">String collection</span><span class="sxs-lookup"><span data-stu-id="c5853-217">String collection</span></span>|<span data-ttu-id="c5853-218">DNS-Suffix-Suchliste.</span><span class="sxs-lookup"><span data-stu-id="c5853-218">DNS suffix search list.</span></span>|



## <a name="response"></a><span data-ttu-id="c5853-219">Antwort</span><span class="sxs-lookup"><span data-stu-id="c5853-219">Response</span></span>
<span data-ttu-id="c5853-220">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="c5853-220">If successful, this method returns a `201 Created` response code and a [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c5853-221">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c5853-221">Example</span></span>

### <a name="request"></a><span data-ttu-id="c5853-222">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c5853-222">Request</span></span>
<span data-ttu-id="c5853-223">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c5853-223">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1243

{
  "@odata.type": "#microsoft.graph.windowsPhone81VpnConfiguration",
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
  },
  "bypassVpnOnCompanyWifi": true,
  "bypassVpnOnHomeWifi": true,
  "authenticationMethod": "usernameAndPassword",
  "rememberUserCredentials": true,
  "dnsSuffixSearchList": [
    "Dns Suffix Search List value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="c5853-224">Antwort</span><span class="sxs-lookup"><span data-stu-id="c5853-224">Response</span></span>
<span data-ttu-id="c5853-p119">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c5853-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1415

{
  "@odata.type": "#microsoft.graph.windowsPhone81VpnConfiguration",
  "id": "7cecc0db-c0db-7cec-dbc0-ec7cdbc0ec7c",
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
  },
  "bypassVpnOnCompanyWifi": true,
  "bypassVpnOnHomeWifi": true,
  "authenticationMethod": "usernameAndPassword",
  "rememberUserCredentials": true,
  "dnsSuffixSearchList": [
    "Dns Suffix Search List value"
  ]
}
```




