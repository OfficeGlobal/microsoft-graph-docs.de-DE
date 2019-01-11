---
title: Ressourcentyp windows10VpnConfiguration
description: Durch die Konfigurationen in dieses Profil bereitstellen können Sie das Windows-10-Gerät (desktop oder mobilen) zur gewünschten Endpunkt für VPN-Verbindung anweisen. Durch Angeben von erwartet die Authentifizierungstypen-Methode und der Sicherheit durch VPN-Endpunkt, dass Sie die VPN-Verbindung nahtlos für Endbenutzer vornehmen können.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 72617e1d91a6a9ce180e63733a209bcee7e204bc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27816066"
---
# <a name="windows10vpnconfiguration-resource-type"></a><span data-ttu-id="70cb0-104">Ressourcentyp windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="70cb0-104">windows10VpnConfiguration resource type</span></span>

> <span data-ttu-id="70cb0-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="70cb0-105">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="70cb0-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="70cb0-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="70cb0-107">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="70cb0-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="70cb0-108">Durch die Konfigurationen in dieses Profil bereitstellen können Sie das Windows-10-Gerät (desktop oder mobilen) zur gewünschten Endpunkt für VPN-Verbindung anweisen.</span><span class="sxs-lookup"><span data-stu-id="70cb0-108">By providing the configurations in this profile you can instruct the Windows 10 device (desktop or mobile) to connect to desired VPN endpoint.</span></span> <span data-ttu-id="70cb0-109">Durch Angeben von erwartet die Authentifizierungstypen-Methode und der Sicherheit durch VPN-Endpunkt, dass Sie die VPN-Verbindung nahtlos für Endbenutzer vornehmen können.</span><span class="sxs-lookup"><span data-stu-id="70cb0-109">By specifying the authentication method and security types expected by VPN endpoint you can make the VPN connection seamless for end user.</span></span>

<span data-ttu-id="70cb0-110">Erbt vom [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="70cb0-110">Inherits from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="70cb0-111">Methoden</span><span class="sxs-lookup"><span data-stu-id="70cb0-111">Methods</span></span>
|<span data-ttu-id="70cb0-112">Methode</span><span class="sxs-lookup"><span data-stu-id="70cb0-112">Method</span></span>|<span data-ttu-id="70cb0-113">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="70cb0-113">Return Type</span></span>|<span data-ttu-id="70cb0-114">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="70cb0-114">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="70cb0-115">Liste windows10VpnConfigurations</span><span class="sxs-lookup"><span data-stu-id="70cb0-115">List windows10VpnConfigurations</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-list.md)|<span data-ttu-id="70cb0-116">[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="70cb0-116">[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) collection</span></span>|<span data-ttu-id="70cb0-117">Listeneigenschaften und Beziehungen der [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="70cb0-117">List properties and relationships of the [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="70cb0-118">Abrufen von windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="70cb0-118">Get windows10VpnConfiguration</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-get.md)|[<span data-ttu-id="70cb0-119">windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="70cb0-119">windows10VpnConfiguration</span></span>](../resources/intune-deviceconfig-windows10vpnconfiguration.md)|<span data-ttu-id="70cb0-120">Lesen Sie Eigenschaften und Beziehungen des [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="70cb0-120">Read properties and relationships of the [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>|
|[<span data-ttu-id="70cb0-121">Erstellen von windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="70cb0-121">Create windows10VpnConfiguration</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-create.md)|[<span data-ttu-id="70cb0-122">windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="70cb0-122">windows10VpnConfiguration</span></span>](../resources/intune-deviceconfig-windows10vpnconfiguration.md)|<span data-ttu-id="70cb0-123">Erstellen eines neuen [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="70cb0-123">Create a new [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>|
|[<span data-ttu-id="70cb0-124">Windows10VpnConfiguration löschen</span><span class="sxs-lookup"><span data-stu-id="70cb0-124">Delete windows10VpnConfiguration</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-delete.md)|<span data-ttu-id="70cb0-125">Keine</span><span class="sxs-lookup"><span data-stu-id="70cb0-125">None</span></span>|<span data-ttu-id="70cb0-126">Löscht eine [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="70cb0-126">Deletes a [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md).</span></span>|
|[<span data-ttu-id="70cb0-127">Windows10VpnConfiguration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="70cb0-127">Update windows10VpnConfiguration</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-update.md)|[<span data-ttu-id="70cb0-128">windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="70cb0-128">windows10VpnConfiguration</span></span>](../resources/intune-deviceconfig-windows10vpnconfiguration.md)|<span data-ttu-id="70cb0-129">Aktualisieren Sie die Eigenschaften eines [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="70cb0-129">Update the properties of a [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="70cb0-130">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="70cb0-130">Properties</span></span>
|<span data-ttu-id="70cb0-131">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="70cb0-131">Property</span></span>|<span data-ttu-id="70cb0-132">Typ</span><span class="sxs-lookup"><span data-stu-id="70cb0-132">Type</span></span>|<span data-ttu-id="70cb0-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="70cb0-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="70cb0-134">id</span><span class="sxs-lookup"><span data-stu-id="70cb0-134">id</span></span>|<span data-ttu-id="70cb0-135">String</span><span class="sxs-lookup"><span data-stu-id="70cb0-135">String</span></span>|<span data-ttu-id="70cb0-136">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="70cb0-136">Key of the entity.</span></span> <span data-ttu-id="70cb0-137">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="70cb0-137">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="70cb0-138">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="70cb0-138">lastModifiedDateTime</span></span>|<span data-ttu-id="70cb0-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="70cb0-139">DateTimeOffset</span></span>|<span data-ttu-id="70cb0-140">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="70cb0-140">DateTime the object was last modified.</span></span> <span data-ttu-id="70cb0-141">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="70cb0-141">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="70cb0-142">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="70cb0-142">roleScopeTagIds</span></span>|<span data-ttu-id="70cb0-143">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="70cb0-143">String collection</span></span>|<span data-ttu-id="70cb0-144">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="70cb0-144">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="70cb0-145">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="70cb0-145">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="70cb0-146">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="70cb0-146">supportsScopeTags</span></span>|<span data-ttu-id="70cb0-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="70cb0-147">Boolean</span></span>|<span data-ttu-id="70cb0-148">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="70cb0-148">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="70cb0-149">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="70cb0-149">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="70cb0-150">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="70cb0-150">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="70cb0-151">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="70cb0-151">This property is read-only.</span></span> <span data-ttu-id="70cb0-152">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="70cb0-152">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="70cb0-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="70cb0-153">createdDateTime</span></span>|<span data-ttu-id="70cb0-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="70cb0-154">DateTimeOffset</span></span>|<span data-ttu-id="70cb0-155">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="70cb0-155">DateTime the object was created.</span></span> <span data-ttu-id="70cb0-156">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="70cb0-156">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="70cb0-157">description</span><span class="sxs-lookup"><span data-stu-id="70cb0-157">description</span></span>|<span data-ttu-id="70cb0-158">String</span><span class="sxs-lookup"><span data-stu-id="70cb0-158">String</span></span>|<span data-ttu-id="70cb0-159">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="70cb0-159">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="70cb0-160">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="70cb0-160">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="70cb0-161">displayName</span><span class="sxs-lookup"><span data-stu-id="70cb0-161">displayName</span></span>|<span data-ttu-id="70cb0-162">String</span><span class="sxs-lookup"><span data-stu-id="70cb0-162">String</span></span>|<span data-ttu-id="70cb0-163">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="70cb0-163">Admin provided name of the device configuration.</span></span> <span data-ttu-id="70cb0-164">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="70cb0-164">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="70cb0-165">Version</span><span class="sxs-lookup"><span data-stu-id="70cb0-165">version</span></span>|<span data-ttu-id="70cb0-166">Int32</span><span class="sxs-lookup"><span data-stu-id="70cb0-166">Int32</span></span>|<span data-ttu-id="70cb0-167">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="70cb0-167">Version of the device configuration.</span></span> <span data-ttu-id="70cb0-168">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="70cb0-168">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="70cb0-169">connectionName</span><span class="sxs-lookup"><span data-stu-id="70cb0-169">connectionName</span></span>|<span data-ttu-id="70cb0-170">String</span><span class="sxs-lookup"><span data-stu-id="70cb0-170">String</span></span>|<span data-ttu-id="70cb0-171">Name der Verbindung für den Benutzer angezeigt.</span><span class="sxs-lookup"><span data-stu-id="70cb0-171">Connection name displayed to the user.</span></span> <span data-ttu-id="70cb0-172">Geerbt von [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="70cb0-172">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="70cb0-173">Server</span><span class="sxs-lookup"><span data-stu-id="70cb0-173">servers</span></span>|<span data-ttu-id="70cb0-174">[VpnServer](../resources/intune-deviceconfig-vpnserver.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="70cb0-174">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="70cb0-175">Liste der VPN-Server im Netzwerk.</span><span class="sxs-lookup"><span data-stu-id="70cb0-175">List of VPN Servers on the network.</span></span> <span data-ttu-id="70cb0-176">Stellen Sie sicher, dass Endbenutzer diese Netzwerkadressen zugreifen können.</span><span class="sxs-lookup"><span data-stu-id="70cb0-176">Make sure end users can access these network locations.</span></span> <span data-ttu-id="70cb0-177">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="70cb0-177">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="70cb0-178">Geerbt von [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="70cb0-178">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="70cb0-179">customXml</span><span class="sxs-lookup"><span data-stu-id="70cb0-179">customXml</span></span>|<span data-ttu-id="70cb0-180">Binär</span><span class="sxs-lookup"><span data-stu-id="70cb0-180">Binary</span></span>|<span data-ttu-id="70cb0-181">Benutzerdefinierte XML-Befehle, die die VPN-Verbindung konfiguriert.</span><span class="sxs-lookup"><span data-stu-id="70cb0-181">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="70cb0-182">(UTF8 codiert Bytearray) Geerbt von [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="70cb0-182">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="70cb0-183">profileTarget</span><span class="sxs-lookup"><span data-stu-id="70cb0-183">profileTarget</span></span>|[<span data-ttu-id="70cb0-184">windows10VpnProfileTarget</span><span class="sxs-lookup"><span data-stu-id="70cb0-184">windows10VpnProfileTarget</span></span>](../resources/intune-deviceconfig-windows10vpnprofiletarget.md)|<span data-ttu-id="70cb0-185">Profil Zieltyp.</span><span class="sxs-lookup"><span data-stu-id="70cb0-185">Profile target type.</span></span> <span data-ttu-id="70cb0-186">Mögliche Werte sind: `user`, `device` und `autoPilotDevice`.</span><span class="sxs-lookup"><span data-stu-id="70cb0-186">Possible values are: `user`, `device`, `autoPilotDevice`.</span></span>|
|<span data-ttu-id="70cb0-187">connectionType</span><span class="sxs-lookup"><span data-stu-id="70cb0-187">connectionType</span></span>|[<span data-ttu-id="70cb0-188">windows10VpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="70cb0-188">windows10VpnConnectionType</span></span>](../resources/intune-deviceconfig-windows10vpnconnectiontype.md)|<span data-ttu-id="70cb0-189">Verbindungstyp.</span><span class="sxs-lookup"><span data-stu-id="70cb0-189">Connection type.</span></span> <span data-ttu-id="70cb0-190">Mögliche Werte: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `automatic`, `ikEv2`, `l2tp`, `pptp`, `citrix`, `paloAltoGlobalProtect`.</span><span class="sxs-lookup"><span data-stu-id="70cb0-190">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `automatic`, `ikEv2`, `l2tp`, `pptp`, `citrix`, `paloAltoGlobalProtect`.</span></span>|
|<span data-ttu-id="70cb0-191">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="70cb0-191">enableSplitTunneling</span></span>|<span data-ttu-id="70cb0-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="70cb0-192">Boolean</span></span>|<span data-ttu-id="70cb0-193">Split-tunneling zu aktivieren.</span><span class="sxs-lookup"><span data-stu-id="70cb0-193">Enable split tunneling.</span></span>|
|<span data-ttu-id="70cb0-194">enableAlwaysOn</span><span class="sxs-lookup"><span data-stu-id="70cb0-194">enableAlwaysOn</span></span>|<span data-ttu-id="70cb0-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="70cb0-195">Boolean</span></span>|<span data-ttu-id="70cb0-196">Aktivieren Sie Always On-Modus.</span><span class="sxs-lookup"><span data-stu-id="70cb0-196">Enable Always On mode.</span></span>|
|<span data-ttu-id="70cb0-197">enableDeviceTunnel</span><span class="sxs-lookup"><span data-stu-id="70cb0-197">enableDeviceTunnel</span></span>|<span data-ttu-id="70cb0-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="70cb0-198">Boolean</span></span>|<span data-ttu-id="70cb0-199">Aktivieren Sie Gerät Tunnel.</span><span class="sxs-lookup"><span data-stu-id="70cb0-199">Enable device tunnel.</span></span>|
|<span data-ttu-id="70cb0-200">enableDnsRegistration</span><span class="sxs-lookup"><span data-stu-id="70cb0-200">enableDnsRegistration</span></span>|<span data-ttu-id="70cb0-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="70cb0-201">Boolean</span></span>|<span data-ttu-id="70cb0-202">Aktivieren Sie die IP-Adressregistrierung mit internen DNS.</span><span class="sxs-lookup"><span data-stu-id="70cb0-202">Enable IP address registration with internal DNS.</span></span>|
|<span data-ttu-id="70cb0-203">dnsSuffixes</span><span class="sxs-lookup"><span data-stu-id="70cb0-203">dnsSuffixes</span></span>|<span data-ttu-id="70cb0-204">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="70cb0-204">String collection</span></span>|<span data-ttu-id="70cb0-205">Geben Sie die DNS-Suffixe hinzufügen zu DNS-Suchliste Kurznamen ordnungsgemäß weitergeleitet.</span><span class="sxs-lookup"><span data-stu-id="70cb0-205">Specify DNS suffixes to add to the DNS search list to properly route short names.</span></span>|
|<span data-ttu-id="70cb0-206">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="70cb0-206">authenticationMethod</span></span>|[<span data-ttu-id="70cb0-207">windows10VpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="70cb0-207">windows10VpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-windows10vpnauthenticationmethod.md)|<span data-ttu-id="70cb0-208">Authentifizierungsmethode.</span><span class="sxs-lookup"><span data-stu-id="70cb0-208">Authentication method.</span></span> <span data-ttu-id="70cb0-209">Mögliche Werte sind: `certificate`, `usernameAndPassword` und `customEapXml`.</span><span class="sxs-lookup"><span data-stu-id="70cb0-209">Possible values are: `certificate`, `usernameAndPassword`, `customEapXml`.</span></span>|
|<span data-ttu-id="70cb0-210">rememberUserCredentials</span><span class="sxs-lookup"><span data-stu-id="70cb0-210">rememberUserCredentials</span></span>|<span data-ttu-id="70cb0-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="70cb0-211">Boolean</span></span>|<span data-ttu-id="70cb0-212">Beachten Sie die Anmeldeinformationen des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="70cb0-212">Remember user credentials.</span></span>|
|<span data-ttu-id="70cb0-213">enableConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="70cb0-213">enableConditionalAccess</span></span>|<span data-ttu-id="70cb0-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="70cb0-214">Boolean</span></span>|<span data-ttu-id="70cb0-215">Aktivieren Sie bedingte Zugriff.</span><span class="sxs-lookup"><span data-stu-id="70cb0-215">Enable conditional access.</span></span>|
|<span data-ttu-id="70cb0-216">enableSingleSignOnWithAlternateCertificate</span><span class="sxs-lookup"><span data-stu-id="70cb0-216">enableSingleSignOnWithAlternateCertificate</span></span>|<span data-ttu-id="70cb0-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="70cb0-217">Boolean</span></span>|<span data-ttu-id="70cb0-218">Aktivieren Sie einmaliges Anmelden (SSO) mit anderen Zertifikats.</span><span class="sxs-lookup"><span data-stu-id="70cb0-218">Enable single sign-on (SSO) with alternate certificate.</span></span>|
|<span data-ttu-id="70cb0-219">singleSignOnEku</span><span class="sxs-lookup"><span data-stu-id="70cb0-219">singleSignOnEku</span></span>|[<span data-ttu-id="70cb0-220">extendedKeyUsage</span><span class="sxs-lookup"><span data-stu-id="70cb0-220">extendedKeyUsage</span></span>](../resources/intune-deviceconfig-extendedkeyusage.md)|<span data-ttu-id="70cb0-221">Einmaliges Anmelden erweiterte Schlüsselverwendung (EKU).</span><span class="sxs-lookup"><span data-stu-id="70cb0-221">Single sign-on Extended Key Usage (EKU).</span></span>|
|<span data-ttu-id="70cb0-222">singleSignOnIssuerHash</span><span class="sxs-lookup"><span data-stu-id="70cb0-222">singleSignOnIssuerHash</span></span>|<span data-ttu-id="70cb0-223">String</span><span class="sxs-lookup"><span data-stu-id="70cb0-223">String</span></span>|<span data-ttu-id="70cb0-224">Einmaliges Anmelden Aussteller Hash.</span><span class="sxs-lookup"><span data-stu-id="70cb0-224">Single sign-on issuer hash.</span></span>|
|<span data-ttu-id="70cb0-225">eapXml</span><span class="sxs-lookup"><span data-stu-id="70cb0-225">eapXml</span></span>|<span data-ttu-id="70cb0-226">Binär</span><span class="sxs-lookup"><span data-stu-id="70cb0-226">Binary</span></span>|<span data-ttu-id="70cb0-227">Extensible Authentication-Protokoll (EAP) XML.</span><span class="sxs-lookup"><span data-stu-id="70cb0-227">Extensible Authentication Protocol (EAP) XML.</span></span> <span data-ttu-id="70cb0-228">(UTF8-codiertes Bytearray)</span><span class="sxs-lookup"><span data-stu-id="70cb0-228">(UTF8 encoded byte array)</span></span>|
|<span data-ttu-id="70cb0-229">proxyServer</span><span class="sxs-lookup"><span data-stu-id="70cb0-229">proxyServer</span></span>|[<span data-ttu-id="70cb0-230">windows10VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="70cb0-230">windows10VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows10vpnproxyserver.md)|<span data-ttu-id="70cb0-231">Proxy-Server.</span><span class="sxs-lookup"><span data-stu-id="70cb0-231">Proxy Server.</span></span>|
|<span data-ttu-id="70cb0-232">associatedApps</span><span class="sxs-lookup"><span data-stu-id="70cb0-232">associatedApps</span></span>|<span data-ttu-id="70cb0-233">[windows10AssociatedApps](../resources/intune-deviceconfig-windows10associatedapps.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="70cb0-233">[windows10AssociatedApps](../resources/intune-deviceconfig-windows10associatedapps.md) collection</span></span>|<span data-ttu-id="70cb0-234">Zugehörige Apps.</span><span class="sxs-lookup"><span data-stu-id="70cb0-234">Associated Apps.</span></span> <span data-ttu-id="70cb0-235">Diese Collection darf maximal 10.000 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="70cb0-235">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="70cb0-236">onlyAssociatedAppsCanUseConnection</span><span class="sxs-lookup"><span data-stu-id="70cb0-236">onlyAssociatedAppsCanUseConnection</span></span>|<span data-ttu-id="70cb0-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="70cb0-237">Boolean</span></span>|<span data-ttu-id="70cb0-238">Nur zugeordnete Apps können Verbindung (pro app VPN) verwenden.</span><span class="sxs-lookup"><span data-stu-id="70cb0-238">Only associated Apps can use connection (per-app VPN).</span></span>|
|<span data-ttu-id="70cb0-239">windowsInformationProtectionDomain</span><span class="sxs-lookup"><span data-stu-id="70cb0-239">windowsInformationProtectionDomain</span></span>|<span data-ttu-id="70cb0-240">String</span><span class="sxs-lookup"><span data-stu-id="70cb0-240">String</span></span>|<span data-ttu-id="70cb0-241">Windows Informationen Schutz (WIP) Domäne, die diese Verbindung zugeordnet.</span><span class="sxs-lookup"><span data-stu-id="70cb0-241">Windows Information Protection (WIP) domain to associate with this connection.</span></span>|
|<span data-ttu-id="70cb0-242">trafficRules</span><span class="sxs-lookup"><span data-stu-id="70cb0-242">trafficRules</span></span>|<span data-ttu-id="70cb0-243">[VpnTrafficRule](../resources/intune-deviceconfig-vpntrafficrule.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="70cb0-243">[vpnTrafficRule](../resources/intune-deviceconfig-vpntrafficrule.md) collection</span></span>|<span data-ttu-id="70cb0-244">Datenverkehr Regeln.</span><span class="sxs-lookup"><span data-stu-id="70cb0-244">Traffic rules.</span></span> <span data-ttu-id="70cb0-245">Diese Sammlung kann bis zu 1000 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="70cb0-245">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="70cb0-246">Routen</span><span class="sxs-lookup"><span data-stu-id="70cb0-246">routes</span></span>|<span data-ttu-id="70cb0-247">[VpnRoute](../resources/intune-deviceconfig-vpnroute.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="70cb0-247">[vpnRoute](../resources/intune-deviceconfig-vpnroute.md) collection</span></span>|<span data-ttu-id="70cb0-248">Routen (optional für Drittanbieter-Anbieter).</span><span class="sxs-lookup"><span data-stu-id="70cb0-248">Routes (optional for third-party providers).</span></span> <span data-ttu-id="70cb0-249">Diese Sammlung kann bis zu 1000 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="70cb0-249">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="70cb0-250">dnsRules</span><span class="sxs-lookup"><span data-stu-id="70cb0-250">dnsRules</span></span>|<span data-ttu-id="70cb0-251">[VpnDnsRule](../resources/intune-deviceconfig-vpndnsrule.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="70cb0-251">[vpnDnsRule](../resources/intune-deviceconfig-vpndnsrule.md) collection</span></span>|<span data-ttu-id="70cb0-252">DNS-Regeln.</span><span class="sxs-lookup"><span data-stu-id="70cb0-252">DNS rules.</span></span> <span data-ttu-id="70cb0-253">Diese Sammlung kann bis zu 1000 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="70cb0-253">This collection can contain a maximum of 1000 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="70cb0-254">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="70cb0-254">Relationships</span></span>
|<span data-ttu-id="70cb0-255">Beziehung</span><span class="sxs-lookup"><span data-stu-id="70cb0-255">Relationship</span></span>|<span data-ttu-id="70cb0-256">Typ</span><span class="sxs-lookup"><span data-stu-id="70cb0-256">Type</span></span>|<span data-ttu-id="70cb0-257">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="70cb0-257">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="70cb0-258">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="70cb0-258">groupAssignments</span></span>|<span data-ttu-id="70cb0-259">[DeviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="70cb0-259">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="70cb0-260">Die Liste derGruppenzuweisungen für das Gerätekonfigurationsprofil.</span><span class="sxs-lookup"><span data-stu-id="70cb0-260">The list of group assignments for the device configuration profile.</span></span> <span data-ttu-id="70cb0-261">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="70cb0-261">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="70cb0-262">assignments</span><span class="sxs-lookup"><span data-stu-id="70cb0-262">assignments</span></span>|<span data-ttu-id="70cb0-263">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="70cb0-263">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="70cb0-264">Liste der Zuweisungen für das Gerätekonfigurationsprofil.</span><span class="sxs-lookup"><span data-stu-id="70cb0-264">The list of assignments for the device configuration profile.</span></span> <span data-ttu-id="70cb0-265">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="70cb0-265">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="70cb0-266">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="70cb0-266">deviceStatuses</span></span>|<span data-ttu-id="70cb0-267">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="70cb0-267">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="70cb0-268">Installationsstatus der Gerätekonfiguration nach Gerät.</span><span class="sxs-lookup"><span data-stu-id="70cb0-268">Device configuration installation status by device.</span></span> <span data-ttu-id="70cb0-269">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="70cb0-269">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="70cb0-270">userStatuses</span><span class="sxs-lookup"><span data-stu-id="70cb0-270">userStatuses</span></span>|<span data-ttu-id="70cb0-271">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="70cb0-271">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="70cb0-272">Gerät Konfiguration Installationsstatus durch Benutzer.</span><span class="sxs-lookup"><span data-stu-id="70cb0-272">Device configuration installation status by user.</span></span> <span data-ttu-id="70cb0-273">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="70cb0-273">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="70cb0-274">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="70cb0-274">deviceStatusOverview</span></span>|[<span data-ttu-id="70cb0-275">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="70cb0-275">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="70cb0-276">Übersicht über den Status der Gerätekonfiguration nach Gerät. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="70cb0-276">Device Configuration devices status overview Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="70cb0-277">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="70cb0-277">userStatusOverview</span></span>|[<span data-ttu-id="70cb0-278">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="70cb0-278">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="70cb0-279">Übersicht über den Status der Gerätekonfiguration nach Benutzer. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="70cb0-279">Device Configuration users status overview Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="70cb0-280">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="70cb0-280">deviceSettingStateSummaries</span></span>|<span data-ttu-id="70cb0-281"> [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="70cb0-281">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="70cb0-282">Übersicht über den Einstellungsstatus für die Gerätekonfiguration nach Gerät. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="70cb0-282">Device Configuration Setting State Device Summary Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="70cb0-283">identityCertificate</span><span class="sxs-lookup"><span data-stu-id="70cb0-283">identityCertificate</span></span>|[<span data-ttu-id="70cb0-284">windowsCertificateProfileBase</span><span class="sxs-lookup"><span data-stu-id="70cb0-284">windowsCertificateProfileBase</span></span>](../resources/intune-deviceconfig-windowscertificateprofilebase.md)|<span data-ttu-id="70cb0-285">Identity-Zertifikat für die Clientauthentifizierung beim Authentifizierungsmethode Zertifikat ist.</span><span class="sxs-lookup"><span data-stu-id="70cb0-285">Identity certificate for client authentication when authentication method is certificate.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="70cb0-286">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="70cb0-286">JSON Representation</span></span>
<span data-ttu-id="70cb0-287">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="70cb0-287">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windows10VpnConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10VpnConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "connectionName": "String",
  "servers": [
    {
      "@odata.type": "microsoft.graph.vpnServer",
      "description": "String",
      "address": "String",
      "isDefaultServer": true
    }
  ],
  "customXml": "binary",
  "profileTarget": "String",
  "connectionType": "String",
  "enableSplitTunneling": true,
  "enableAlwaysOn": true,
  "enableDeviceTunnel": true,
  "enableDnsRegistration": true,
  "dnsSuffixes": [
    "String"
  ],
  "authenticationMethod": "String",
  "rememberUserCredentials": true,
  "enableConditionalAccess": true,
  "enableSingleSignOnWithAlternateCertificate": true,
  "singleSignOnEku": {
    "@odata.type": "microsoft.graph.extendedKeyUsage",
    "name": "String",
    "objectIdentifier": "String"
  },
  "singleSignOnIssuerHash": "String",
  "eapXml": "binary",
  "proxyServer": {
    "@odata.type": "microsoft.graph.windows10VpnProxyServer",
    "automaticConfigurationScriptUrl": "String",
    "address": "String",
    "port": 1024,
    "bypassProxyServerForLocalAddress": true
  },
  "associatedApps": [
    {
      "@odata.type": "microsoft.graph.windows10AssociatedApps",
      "appType": "String",
      "identifier": "String"
    }
  ],
  "onlyAssociatedAppsCanUseConnection": true,
  "windowsInformationProtectionDomain": "String",
  "trafficRules": [
    {
      "@odata.type": "microsoft.graph.vpnTrafficRule",
      "name": "String",
      "protocols": 1024,
      "localPortRanges": [
        {
          "@odata.type": "microsoft.graph.numberRange",
          "lowerNumber": 1024,
          "upperNumber": 1024
        }
      ],
      "remotePortRanges": [
        {
          "@odata.type": "microsoft.graph.numberRange",
          "lowerNumber": 1024,
          "upperNumber": 1024
        }
      ],
      "localAddressRanges": [
        {
          "@odata.type": "microsoft.graph.iPv4Range",
          "lowerAddress": "String",
          "upperAddress": "String"
        }
      ],
      "remoteAddressRanges": [
        {
          "@odata.type": "microsoft.graph.iPv4Range",
          "lowerAddress": "String",
          "upperAddress": "String"
        }
      ],
      "appId": "String",
      "appType": "String",
      "routingPolicyType": "String",
      "claims": "String"
    }
  ],
  "routes": [
    {
      "@odata.type": "microsoft.graph.vpnRoute",
      "destinationPrefix": "String",
      "prefixSize": 1024
    }
  ],
  "dnsRules": [
    {
      "@odata.type": "microsoft.graph.vpnDnsRule",
      "name": "String",
      "servers": [
        "String"
      ],
      "proxyServerUri": "String"
    }
  ]
}
```





