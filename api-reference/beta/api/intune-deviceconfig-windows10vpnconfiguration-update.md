---
title: Windows10VpnConfiguration aktualisieren
description: Aktualisieren Sie die Eigenschaften eines windows10VpnConfiguration-Objekts.
author: tfitzmac
ms.openlocfilehash: 24112120dd414bc7929d9223094b528b32ad818a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27305068"
---
# <a name="update-windows10vpnconfiguration"></a><span data-ttu-id="40e92-103">Windows10VpnConfiguration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="40e92-103">Update windows10VpnConfiguration</span></span>

> <span data-ttu-id="40e92-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="40e92-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="40e92-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="40e92-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="40e92-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="40e92-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="40e92-107">Aktualisieren Sie die Eigenschaften eines [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="40e92-107">Update the properties of a [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="40e92-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="40e92-108">Prerequisites</span></span>
<span data-ttu-id="40e92-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="40e92-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="40e92-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="40e92-111">Permission type</span></span>|<span data-ttu-id="40e92-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="40e92-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="40e92-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="40e92-113">Delegated (work or school account)</span></span>|<span data-ttu-id="40e92-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40e92-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="40e92-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="40e92-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="40e92-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="40e92-116">Not supported.</span></span>|
|<span data-ttu-id="40e92-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="40e92-117">Application</span></span>|<span data-ttu-id="40e92-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="40e92-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="40e92-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="40e92-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="40e92-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="40e92-120">Request headers</span></span>
|<span data-ttu-id="40e92-121">Header</span><span class="sxs-lookup"><span data-stu-id="40e92-121">Header</span></span>|<span data-ttu-id="40e92-122">Wert</span><span class="sxs-lookup"><span data-stu-id="40e92-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="40e92-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="40e92-123">Authorization</span></span>|<span data-ttu-id="40e92-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="40e92-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="40e92-125">Accept</span><span class="sxs-lookup"><span data-stu-id="40e92-125">Accept</span></span>|<span data-ttu-id="40e92-126">application/json</span><span class="sxs-lookup"><span data-stu-id="40e92-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="40e92-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="40e92-127">Request body</span></span>
<span data-ttu-id="40e92-128">Geben Sie im Textkörper Anforderung für das Objekt [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="40e92-128">In the request body, supply a JSON representation for the [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>

<span data-ttu-id="40e92-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="40e92-129">The following table shows the properties that are required when you create the [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md).</span></span>

|<span data-ttu-id="40e92-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="40e92-130">Property</span></span>|<span data-ttu-id="40e92-131">Typ</span><span class="sxs-lookup"><span data-stu-id="40e92-131">Type</span></span>|<span data-ttu-id="40e92-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="40e92-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="40e92-133">id</span><span class="sxs-lookup"><span data-stu-id="40e92-133">id</span></span>|<span data-ttu-id="40e92-134">String</span><span class="sxs-lookup"><span data-stu-id="40e92-134">String</span></span>|<span data-ttu-id="40e92-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="40e92-135">Key of the entity.</span></span> <span data-ttu-id="40e92-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="40e92-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="40e92-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="40e92-137">lastModifiedDateTime</span></span>|<span data-ttu-id="40e92-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="40e92-138">DateTimeOffset</span></span>|<span data-ttu-id="40e92-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="40e92-139">DateTime the object was last modified.</span></span> <span data-ttu-id="40e92-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="40e92-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="40e92-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="40e92-141">roleScopeTagIds</span></span>|<span data-ttu-id="40e92-142">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="40e92-142">String collection</span></span>|<span data-ttu-id="40e92-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="40e92-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="40e92-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="40e92-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="40e92-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="40e92-145">supportsScopeTags</span></span>|<span data-ttu-id="40e92-146">Boolesch</span><span class="sxs-lookup"><span data-stu-id="40e92-146">Boolean</span></span>|<span data-ttu-id="40e92-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="40e92-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="40e92-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="40e92-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="40e92-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="40e92-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="40e92-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="40e92-150">This property is read-only.</span></span> <span data-ttu-id="40e92-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="40e92-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="40e92-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="40e92-152">createdDateTime</span></span>|<span data-ttu-id="40e92-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="40e92-153">DateTimeOffset</span></span>|<span data-ttu-id="40e92-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="40e92-154">DateTime the object was created.</span></span> <span data-ttu-id="40e92-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="40e92-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="40e92-156">description</span><span class="sxs-lookup"><span data-stu-id="40e92-156">description</span></span>|<span data-ttu-id="40e92-157">String</span><span class="sxs-lookup"><span data-stu-id="40e92-157">String</span></span>|<span data-ttu-id="40e92-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="40e92-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="40e92-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="40e92-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="40e92-160">displayName</span><span class="sxs-lookup"><span data-stu-id="40e92-160">displayName</span></span>|<span data-ttu-id="40e92-161">String</span><span class="sxs-lookup"><span data-stu-id="40e92-161">String</span></span>|<span data-ttu-id="40e92-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="40e92-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="40e92-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="40e92-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="40e92-164">Version</span><span class="sxs-lookup"><span data-stu-id="40e92-164">version</span></span>|<span data-ttu-id="40e92-165">Int32</span><span class="sxs-lookup"><span data-stu-id="40e92-165">Int32</span></span>|<span data-ttu-id="40e92-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="40e92-166">Version of the device configuration.</span></span> <span data-ttu-id="40e92-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="40e92-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="40e92-168">connectionName</span><span class="sxs-lookup"><span data-stu-id="40e92-168">connectionName</span></span>|<span data-ttu-id="40e92-169">String</span><span class="sxs-lookup"><span data-stu-id="40e92-169">String</span></span>|<span data-ttu-id="40e92-170">Name der Verbindung für den Benutzer angezeigt.</span><span class="sxs-lookup"><span data-stu-id="40e92-170">Connection name displayed to the user.</span></span> <span data-ttu-id="40e92-171">Geerbt von [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="40e92-171">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="40e92-172">Server</span><span class="sxs-lookup"><span data-stu-id="40e92-172">servers</span></span>|<span data-ttu-id="40e92-173">[VpnServer](../resources/intune-deviceconfig-vpnserver.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="40e92-173">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="40e92-174">Liste der VPN-Server im Netzwerk.</span><span class="sxs-lookup"><span data-stu-id="40e92-174">List of VPN Servers on the network.</span></span> <span data-ttu-id="40e92-175">Stellen Sie sicher, dass Endbenutzer diese Netzwerkadressen zugreifen können.</span><span class="sxs-lookup"><span data-stu-id="40e92-175">Make sure end users can access these network locations.</span></span> <span data-ttu-id="40e92-176">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="40e92-176">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="40e92-177">Geerbt von [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="40e92-177">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="40e92-178">customXml</span><span class="sxs-lookup"><span data-stu-id="40e92-178">customXml</span></span>|<span data-ttu-id="40e92-179">Binär</span><span class="sxs-lookup"><span data-stu-id="40e92-179">Binary</span></span>|<span data-ttu-id="40e92-180">Benutzerdefinierte XML-Befehle, die die VPN-Verbindung konfiguriert.</span><span class="sxs-lookup"><span data-stu-id="40e92-180">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="40e92-181">(UTF8 codiert Bytearray) Geerbt von [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="40e92-181">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="40e92-182">profileTarget</span><span class="sxs-lookup"><span data-stu-id="40e92-182">profileTarget</span></span>|[<span data-ttu-id="40e92-183">windows10VpnProfileTarget</span><span class="sxs-lookup"><span data-stu-id="40e92-183">windows10VpnProfileTarget</span></span>](../resources/intune-deviceconfig-windows10vpnprofiletarget.md)|<span data-ttu-id="40e92-184">Profil Zieltyp.</span><span class="sxs-lookup"><span data-stu-id="40e92-184">Profile target type.</span></span> <span data-ttu-id="40e92-185">Mögliche Werte sind: `user`, `device` und `autoPilotDevice`.</span><span class="sxs-lookup"><span data-stu-id="40e92-185">Possible values are: `user`, `device`, `autoPilotDevice`.</span></span>|
|<span data-ttu-id="40e92-186">connectionType</span><span class="sxs-lookup"><span data-stu-id="40e92-186">connectionType</span></span>|[<span data-ttu-id="40e92-187">windows10VpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="40e92-187">windows10VpnConnectionType</span></span>](../resources/intune-deviceconfig-windows10vpnconnectiontype.md)|<span data-ttu-id="40e92-188">Verbindungstyp.</span><span class="sxs-lookup"><span data-stu-id="40e92-188">Connection type.</span></span> <span data-ttu-id="40e92-189">Mögliche Werte: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `automatic`, `ikEv2`, `l2tp`, `pptp`, `citrix`, `paloAltoGlobalProtect`.</span><span class="sxs-lookup"><span data-stu-id="40e92-189">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `automatic`, `ikEv2`, `l2tp`, `pptp`, `citrix`, `paloAltoGlobalProtect`.</span></span>|
|<span data-ttu-id="40e92-190">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="40e92-190">enableSplitTunneling</span></span>|<span data-ttu-id="40e92-191">Boolesch</span><span class="sxs-lookup"><span data-stu-id="40e92-191">Boolean</span></span>|<span data-ttu-id="40e92-192">Split-tunneling zu aktivieren.</span><span class="sxs-lookup"><span data-stu-id="40e92-192">Enable split tunneling.</span></span>|
|<span data-ttu-id="40e92-193">enableAlwaysOn</span><span class="sxs-lookup"><span data-stu-id="40e92-193">enableAlwaysOn</span></span>|<span data-ttu-id="40e92-194">Boolesch</span><span class="sxs-lookup"><span data-stu-id="40e92-194">Boolean</span></span>|<span data-ttu-id="40e92-195">Aktivieren Sie Always On-Modus.</span><span class="sxs-lookup"><span data-stu-id="40e92-195">Enable Always On mode.</span></span>|
|<span data-ttu-id="40e92-196">enableDeviceTunnel</span><span class="sxs-lookup"><span data-stu-id="40e92-196">enableDeviceTunnel</span></span>|<span data-ttu-id="40e92-197">Boolesch</span><span class="sxs-lookup"><span data-stu-id="40e92-197">Boolean</span></span>|<span data-ttu-id="40e92-198">Aktivieren Sie Gerät Tunnel.</span><span class="sxs-lookup"><span data-stu-id="40e92-198">Enable device tunnel.</span></span>|
|<span data-ttu-id="40e92-199">enableDnsRegistration</span><span class="sxs-lookup"><span data-stu-id="40e92-199">enableDnsRegistration</span></span>|<span data-ttu-id="40e92-200">Boolesch</span><span class="sxs-lookup"><span data-stu-id="40e92-200">Boolean</span></span>|<span data-ttu-id="40e92-201">Aktivieren Sie die IP-Adressregistrierung mit internen DNS.</span><span class="sxs-lookup"><span data-stu-id="40e92-201">Enable IP address registration with internal DNS.</span></span>|
|<span data-ttu-id="40e92-202">dnsSuffixes</span><span class="sxs-lookup"><span data-stu-id="40e92-202">dnsSuffixes</span></span>|<span data-ttu-id="40e92-203">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="40e92-203">String collection</span></span>|<span data-ttu-id="40e92-204">Geben Sie die DNS-Suffixe hinzufügen zu DNS-Suchliste Kurznamen ordnungsgemäß weitergeleitet.</span><span class="sxs-lookup"><span data-stu-id="40e92-204">Specify DNS suffixes to add to the DNS search list to properly route short names.</span></span>|
|<span data-ttu-id="40e92-205">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="40e92-205">authenticationMethod</span></span>|[<span data-ttu-id="40e92-206">windows10VpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="40e92-206">windows10VpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-windows10vpnauthenticationmethod.md)|<span data-ttu-id="40e92-207">Authentifizierungsmethode.</span><span class="sxs-lookup"><span data-stu-id="40e92-207">Authentication method.</span></span> <span data-ttu-id="40e92-208">Mögliche Werte sind: `certificate`, `usernameAndPassword` und `customEapXml`.</span><span class="sxs-lookup"><span data-stu-id="40e92-208">Possible values are: `certificate`, `usernameAndPassword`, `customEapXml`.</span></span>|
|<span data-ttu-id="40e92-209">rememberUserCredentials</span><span class="sxs-lookup"><span data-stu-id="40e92-209">rememberUserCredentials</span></span>|<span data-ttu-id="40e92-210">Boolesch</span><span class="sxs-lookup"><span data-stu-id="40e92-210">Boolean</span></span>|<span data-ttu-id="40e92-211">Beachten Sie die Anmeldeinformationen des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="40e92-211">Remember user credentials.</span></span>|
|<span data-ttu-id="40e92-212">enableConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="40e92-212">enableConditionalAccess</span></span>|<span data-ttu-id="40e92-213">Boolesch</span><span class="sxs-lookup"><span data-stu-id="40e92-213">Boolean</span></span>|<span data-ttu-id="40e92-214">Aktivieren Sie bedingte Zugriff.</span><span class="sxs-lookup"><span data-stu-id="40e92-214">Enable conditional access.</span></span>|
|<span data-ttu-id="40e92-215">enableSingleSignOnWithAlternateCertificate</span><span class="sxs-lookup"><span data-stu-id="40e92-215">enableSingleSignOnWithAlternateCertificate</span></span>|<span data-ttu-id="40e92-216">Boolesch</span><span class="sxs-lookup"><span data-stu-id="40e92-216">Boolean</span></span>|<span data-ttu-id="40e92-217">Aktivieren Sie einmaliges Anmelden (SSO) mit anderen Zertifikats.</span><span class="sxs-lookup"><span data-stu-id="40e92-217">Enable single sign-on (SSO) with alternate certificate.</span></span>|
|<span data-ttu-id="40e92-218">singleSignOnEku</span><span class="sxs-lookup"><span data-stu-id="40e92-218">singleSignOnEku</span></span>|[<span data-ttu-id="40e92-219">extendedKeyUsage</span><span class="sxs-lookup"><span data-stu-id="40e92-219">extendedKeyUsage</span></span>](../resources/intune-deviceconfig-extendedkeyusage.md)|<span data-ttu-id="40e92-220">Einmaliges Anmelden erweiterte Schlüsselverwendung (EKU).</span><span class="sxs-lookup"><span data-stu-id="40e92-220">Single sign-on Extended Key Usage (EKU).</span></span>|
|<span data-ttu-id="40e92-221">singleSignOnIssuerHash</span><span class="sxs-lookup"><span data-stu-id="40e92-221">singleSignOnIssuerHash</span></span>|<span data-ttu-id="40e92-222">String</span><span class="sxs-lookup"><span data-stu-id="40e92-222">String</span></span>|<span data-ttu-id="40e92-223">Einmaliges Anmelden Aussteller Hash.</span><span class="sxs-lookup"><span data-stu-id="40e92-223">Single sign-on issuer hash.</span></span>|
|<span data-ttu-id="40e92-224">eapXml</span><span class="sxs-lookup"><span data-stu-id="40e92-224">eapXml</span></span>|<span data-ttu-id="40e92-225">Binär</span><span class="sxs-lookup"><span data-stu-id="40e92-225">Binary</span></span>|<span data-ttu-id="40e92-226">Extensible Authentication-Protokoll (EAP) XML.</span><span class="sxs-lookup"><span data-stu-id="40e92-226">Extensible Authentication Protocol (EAP) XML.</span></span> <span data-ttu-id="40e92-227">(UTF8-codiertes Bytearray)</span><span class="sxs-lookup"><span data-stu-id="40e92-227">(UTF8 encoded byte array)</span></span>|
|<span data-ttu-id="40e92-228">proxyServer</span><span class="sxs-lookup"><span data-stu-id="40e92-228">proxyServer</span></span>|[<span data-ttu-id="40e92-229">windows10VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="40e92-229">windows10VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows10vpnproxyserver.md)|<span data-ttu-id="40e92-230">Proxy-Server.</span><span class="sxs-lookup"><span data-stu-id="40e92-230">Proxy Server.</span></span>|
|<span data-ttu-id="40e92-231">associatedApps</span><span class="sxs-lookup"><span data-stu-id="40e92-231">associatedApps</span></span>|<span data-ttu-id="40e92-232">[windows10AssociatedApps](../resources/intune-deviceconfig-windows10associatedapps.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="40e92-232">[windows10AssociatedApps](../resources/intune-deviceconfig-windows10associatedapps.md) collection</span></span>|<span data-ttu-id="40e92-233">Zugehörige Apps.</span><span class="sxs-lookup"><span data-stu-id="40e92-233">Associated Apps.</span></span> <span data-ttu-id="40e92-234">Diese Collection darf maximal 10.000 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="40e92-234">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="40e92-235">onlyAssociatedAppsCanUseConnection</span><span class="sxs-lookup"><span data-stu-id="40e92-235">onlyAssociatedAppsCanUseConnection</span></span>|<span data-ttu-id="40e92-236">Boolesch</span><span class="sxs-lookup"><span data-stu-id="40e92-236">Boolean</span></span>|<span data-ttu-id="40e92-237">Nur zugeordnete Apps können Verbindung (pro app VPN) verwenden.</span><span class="sxs-lookup"><span data-stu-id="40e92-237">Only associated Apps can use connection (per-app VPN).</span></span>|
|<span data-ttu-id="40e92-238">windowsInformationProtectionDomain</span><span class="sxs-lookup"><span data-stu-id="40e92-238">windowsInformationProtectionDomain</span></span>|<span data-ttu-id="40e92-239">String</span><span class="sxs-lookup"><span data-stu-id="40e92-239">String</span></span>|<span data-ttu-id="40e92-240">Windows Informationen Schutz (WIP) Domäne, die diese Verbindung zugeordnet.</span><span class="sxs-lookup"><span data-stu-id="40e92-240">Windows Information Protection (WIP) domain to associate with this connection.</span></span>|
|<span data-ttu-id="40e92-241">trafficRules</span><span class="sxs-lookup"><span data-stu-id="40e92-241">trafficRules</span></span>|<span data-ttu-id="40e92-242">[VpnTrafficRule](../resources/intune-deviceconfig-vpntrafficrule.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="40e92-242">[vpnTrafficRule](../resources/intune-deviceconfig-vpntrafficrule.md) collection</span></span>|<span data-ttu-id="40e92-243">Datenverkehr Regeln.</span><span class="sxs-lookup"><span data-stu-id="40e92-243">Traffic rules.</span></span> <span data-ttu-id="40e92-244">Diese Sammlung kann bis zu 1000 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="40e92-244">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="40e92-245">Routen</span><span class="sxs-lookup"><span data-stu-id="40e92-245">routes</span></span>|<span data-ttu-id="40e92-246">[VpnRoute](../resources/intune-deviceconfig-vpnroute.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="40e92-246">[vpnRoute](../resources/intune-deviceconfig-vpnroute.md) collection</span></span>|<span data-ttu-id="40e92-247">Routen (optional für Drittanbieter-Anbieter).</span><span class="sxs-lookup"><span data-stu-id="40e92-247">Routes (optional for third-party providers).</span></span> <span data-ttu-id="40e92-248">Diese Sammlung kann bis zu 1000 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="40e92-248">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="40e92-249">dnsRules</span><span class="sxs-lookup"><span data-stu-id="40e92-249">dnsRules</span></span>|<span data-ttu-id="40e92-250">[VpnDnsRule](../resources/intune-deviceconfig-vpndnsrule.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="40e92-250">[vpnDnsRule](../resources/intune-deviceconfig-vpndnsrule.md) collection</span></span>|<span data-ttu-id="40e92-251">DNS-Regeln.</span><span class="sxs-lookup"><span data-stu-id="40e92-251">DNS rules.</span></span> <span data-ttu-id="40e92-252">Diese Sammlung kann bis zu 1000 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="40e92-252">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="40e92-253">Antwort</span><span class="sxs-lookup"><span data-stu-id="40e92-253">Response</span></span>
<span data-ttu-id="40e92-254">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="40e92-254">If successful, this method returns a `200 OK` response code and an updated [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="40e92-255">Beispiel</span><span class="sxs-lookup"><span data-stu-id="40e92-255">Example</span></span>
### <a name="request"></a><span data-ttu-id="40e92-256">Anforderung</span><span class="sxs-lookup"><span data-stu-id="40e92-256">Request</span></span>
<span data-ttu-id="40e92-257">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="40e92-257">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 3259

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
  "profileTarget": "device",
  "connectionType": "f5EdgeClient",
  "enableSplitTunneling": true,
  "enableAlwaysOn": true,
  "enableDeviceTunnel": true,
  "enableDnsRegistration": true,
  "dnsSuffixes": [
    "Dns Suffixes value"
  ],
  "authenticationMethod": "usernameAndPassword",
  "rememberUserCredentials": true,
  "enableConditionalAccess": true,
  "enableSingleSignOnWithAlternateCertificate": true,
  "singleSignOnEku": {
    "@odata.type": "microsoft.graph.extendedKeyUsage",
    "name": "Name value",
    "objectIdentifier": "Object Identifier value"
  },
  "singleSignOnIssuerHash": "Single Sign On Issuer Hash value",
  "eapXml": "ZWFwWG1s",
  "proxyServer": {
    "@odata.type": "microsoft.graph.windows10VpnProxyServer",
    "automaticConfigurationScriptUrl": "https://example.com/automaticConfigurationScriptUrl/",
    "address": "Address value",
    "port": 4,
    "bypassProxyServerForLocalAddress": true
  },
  "associatedApps": [
    {
      "@odata.type": "microsoft.graph.windows10AssociatedApps",
      "appType": "universal",
      "identifier": "Identifier value"
    }
  ],
  "onlyAssociatedAppsCanUseConnection": true,
  "windowsInformationProtectionDomain": "Windows Information Protection Domain value",
  "trafficRules": [
    {
      "@odata.type": "microsoft.graph.vpnTrafficRule",
      "name": "Name value",
      "protocols": 9,
      "localPortRanges": [
        {
          "@odata.type": "microsoft.graph.numberRange",
          "lowerNumber": 11,
          "upperNumber": 11
        }
      ],
      "remotePortRanges": [
        {
          "@odata.type": "microsoft.graph.numberRange",
          "lowerNumber": 11,
          "upperNumber": 11
        }
      ],
      "localAddressRanges": [
        {
          "@odata.type": "microsoft.graph.iPv4Range",
          "lowerAddress": "Lower Address value",
          "upperAddress": "Upper Address value"
        }
      ],
      "remoteAddressRanges": [
        {
          "@odata.type": "microsoft.graph.iPv4Range",
          "lowerAddress": "Lower Address value",
          "upperAddress": "Upper Address value"
        }
      ],
      "appId": "App Id value",
      "appType": "desktop",
      "routingPolicyType": "splitTunnel",
      "claims": "Claims value"
    }
  ],
  "routes": [
    {
      "@odata.type": "microsoft.graph.vpnRoute",
      "destinationPrefix": "Destination Prefix value",
      "prefixSize": 10
    }
  ],
  "dnsRules": [
    {
      "@odata.type": "microsoft.graph.vpnDnsRule",
      "name": "Name value",
      "servers": [
        "Servers value"
      ],
      "proxyServerUri": "Proxy Server Uri value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="40e92-258">Antwort</span><span class="sxs-lookup"><span data-stu-id="40e92-258">Response</span></span>
<span data-ttu-id="40e92-p122">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="40e92-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3431

{
  "@odata.type": "#microsoft.graph.windows10VpnConfiguration",
  "id": "c23c9727-9727-c23c-2797-3cc227973cc2",
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
  "profileTarget": "device",
  "connectionType": "f5EdgeClient",
  "enableSplitTunneling": true,
  "enableAlwaysOn": true,
  "enableDeviceTunnel": true,
  "enableDnsRegistration": true,
  "dnsSuffixes": [
    "Dns Suffixes value"
  ],
  "authenticationMethod": "usernameAndPassword",
  "rememberUserCredentials": true,
  "enableConditionalAccess": true,
  "enableSingleSignOnWithAlternateCertificate": true,
  "singleSignOnEku": {
    "@odata.type": "microsoft.graph.extendedKeyUsage",
    "name": "Name value",
    "objectIdentifier": "Object Identifier value"
  },
  "singleSignOnIssuerHash": "Single Sign On Issuer Hash value",
  "eapXml": "ZWFwWG1s",
  "proxyServer": {
    "@odata.type": "microsoft.graph.windows10VpnProxyServer",
    "automaticConfigurationScriptUrl": "https://example.com/automaticConfigurationScriptUrl/",
    "address": "Address value",
    "port": 4,
    "bypassProxyServerForLocalAddress": true
  },
  "associatedApps": [
    {
      "@odata.type": "microsoft.graph.windows10AssociatedApps",
      "appType": "universal",
      "identifier": "Identifier value"
    }
  ],
  "onlyAssociatedAppsCanUseConnection": true,
  "windowsInformationProtectionDomain": "Windows Information Protection Domain value",
  "trafficRules": [
    {
      "@odata.type": "microsoft.graph.vpnTrafficRule",
      "name": "Name value",
      "protocols": 9,
      "localPortRanges": [
        {
          "@odata.type": "microsoft.graph.numberRange",
          "lowerNumber": 11,
          "upperNumber": 11
        }
      ],
      "remotePortRanges": [
        {
          "@odata.type": "microsoft.graph.numberRange",
          "lowerNumber": 11,
          "upperNumber": 11
        }
      ],
      "localAddressRanges": [
        {
          "@odata.type": "microsoft.graph.iPv4Range",
          "lowerAddress": "Lower Address value",
          "upperAddress": "Upper Address value"
        }
      ],
      "remoteAddressRanges": [
        {
          "@odata.type": "microsoft.graph.iPv4Range",
          "lowerAddress": "Lower Address value",
          "upperAddress": "Upper Address value"
        }
      ],
      "appId": "App Id value",
      "appType": "desktop",
      "routingPolicyType": "splitTunnel",
      "claims": "Claims value"
    }
  ],
  "routes": [
    {
      "@odata.type": "microsoft.graph.vpnRoute",
      "destinationPrefix": "Destination Prefix value",
      "prefixSize": 10
    }
  ],
  "dnsRules": [
    {
      "@odata.type": "microsoft.graph.vpnDnsRule",
      "name": "Name value",
      "servers": [
        "Servers value"
      ],
      "proxyServerUri": "Proxy Server Uri value"
    }
  ]
}
```





