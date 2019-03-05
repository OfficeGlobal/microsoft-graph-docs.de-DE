---
title: windows10VpnConfiguration-Ressourcentyp
description: Durch die Bereitstellung der Konfigurationen in diesem Profil können Sie das Windows 10-Gerät (Desktop oder Mobil) anweisen, eine Verbindung mit dem gewünschten VPN-Endpunkt herzustellen. Durch Angeben der Authentifizierungsmethode und der vom VPN-Endpunkt erwarteten Sicherheitstypen können Sie die VPN-Verbindung für Endbenutzer nahtlos ausführen.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c4b1b906fc4a98895acc6e23a4b3e9a4d78ff28a
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30148713"
---
# <a name="windows10vpnconfiguration-resource-type"></a><span data-ttu-id="37579-104">windows10VpnConfiguration-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="37579-104">windows10VpnConfiguration resource type</span></span>

> <span data-ttu-id="37579-105">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="37579-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="37579-106">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="37579-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="37579-107">Durch die Bereitstellung der Konfigurationen in diesem Profil können Sie das Windows 10-Gerät (Desktop oder Mobil) anweisen, eine Verbindung mit dem gewünschten VPN-Endpunkt herzustellen.</span><span class="sxs-lookup"><span data-stu-id="37579-107">By providing the configurations in this profile you can instruct the Windows 10 device (desktop or mobile) to connect to desired VPN endpoint.</span></span> <span data-ttu-id="37579-108">Durch Angeben der Authentifizierungsmethode und der vom VPN-Endpunkt erwarteten Sicherheitstypen können Sie die VPN-Verbindung für Endbenutzer nahtlos ausführen.</span><span class="sxs-lookup"><span data-stu-id="37579-108">By specifying the authentication method and security types expected by VPN endpoint you can make the VPN connection seamless for end user.</span></span>


<span data-ttu-id="37579-109">Erbt von [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="37579-109">Inherits from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="37579-110">Methoden</span><span class="sxs-lookup"><span data-stu-id="37579-110">Methods</span></span>
|<span data-ttu-id="37579-111">Methode</span><span class="sxs-lookup"><span data-stu-id="37579-111">Method</span></span>|<span data-ttu-id="37579-112">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="37579-112">Return Type</span></span>|<span data-ttu-id="37579-113">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="37579-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="37579-114">Windows10VpnConfigurations aufListen</span><span class="sxs-lookup"><span data-stu-id="37579-114">List windows10VpnConfigurations</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-list.md)|<span data-ttu-id="37579-115">[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="37579-115">[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) collection</span></span>|<span data-ttu-id="37579-116">AufListen von Eigenschaften und Beziehungen der [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="37579-116">List properties and relationships of the [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="37579-117">Windows10VpnConfiguration abrufen</span><span class="sxs-lookup"><span data-stu-id="37579-117">Get windows10VpnConfiguration</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-get.md)|[<span data-ttu-id="37579-118">windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="37579-118">windows10VpnConfiguration</span></span>](../resources/intune-deviceconfig-windows10vpnconfiguration.md)|<span data-ttu-id="37579-119">Lesen von Eigenschaften und Beziehungen des [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="37579-119">Read properties and relationships of the [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>|
|[<span data-ttu-id="37579-120">Windows10VpnConfiguration erstellen</span><span class="sxs-lookup"><span data-stu-id="37579-120">Create windows10VpnConfiguration</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-create.md)|[<span data-ttu-id="37579-121">windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="37579-121">windows10VpnConfiguration</span></span>](../resources/intune-deviceconfig-windows10vpnconfiguration.md)|<span data-ttu-id="37579-122">Erstellen eines neuen [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="37579-122">Create a new [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>|
|[<span data-ttu-id="37579-123">Windows10VpnConfiguration löschen</span><span class="sxs-lookup"><span data-stu-id="37579-123">Delete windows10VpnConfiguration</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-delete.md)|<span data-ttu-id="37579-124">Keine</span><span class="sxs-lookup"><span data-stu-id="37579-124">None</span></span>|<span data-ttu-id="37579-125">Löscht eine [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="37579-125">Deletes a [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md).</span></span>|
|[<span data-ttu-id="37579-126">Windows10VpnConfiguration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="37579-126">Update windows10VpnConfiguration</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-update.md)|[<span data-ttu-id="37579-127">windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="37579-127">windows10VpnConfiguration</span></span>](../resources/intune-deviceconfig-windows10vpnconfiguration.md)|<span data-ttu-id="37579-128">Aktualisieren der Eigenschaften eines [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="37579-128">Update the properties of a [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="37579-129">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="37579-129">Properties</span></span>
|<span data-ttu-id="37579-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="37579-130">Property</span></span>|<span data-ttu-id="37579-131">Typ</span><span class="sxs-lookup"><span data-stu-id="37579-131">Type</span></span>|<span data-ttu-id="37579-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="37579-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="37579-133">id</span><span class="sxs-lookup"><span data-stu-id="37579-133">id</span></span>|<span data-ttu-id="37579-134">string</span><span class="sxs-lookup"><span data-stu-id="37579-134">String</span></span>|<span data-ttu-id="37579-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="37579-135">Key of the entity.</span></span> <span data-ttu-id="37579-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="37579-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="37579-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="37579-137">lastModifiedDateTime</span></span>|<span data-ttu-id="37579-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="37579-138">DateTimeOffset</span></span>|<span data-ttu-id="37579-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="37579-139">DateTime the object was last modified.</span></span> <span data-ttu-id="37579-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="37579-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="37579-141">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="37579-141">roleScopeTagIds</span></span>|<span data-ttu-id="37579-142">String collection</span><span class="sxs-lookup"><span data-stu-id="37579-142">String collection</span></span>|<span data-ttu-id="37579-143">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="37579-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="37579-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="37579-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="37579-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="37579-145">supportsScopeTags</span></span>|<span data-ttu-id="37579-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="37579-146">Boolean</span></span>|<span data-ttu-id="37579-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereichs Tags unterstützt.</span><span class="sxs-lookup"><span data-stu-id="37579-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="37579-148">Das Zuweisen zur ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert auf false festgelegt ist und Entitäten für bereichsbezogene Benutzer nicht sichtbar sind.</span><span class="sxs-lookup"><span data-stu-id="37579-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="37579-149">Dies geschieht für in Silverlight erstellte Legacy Richtlinien und kann durch Löschen und erneutes Erstellen der Richtlinie im Azure-Portal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="37579-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="37579-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="37579-150">This property is read-only.</span></span> <span data-ttu-id="37579-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="37579-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="37579-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="37579-152">createdDateTime</span></span>|<span data-ttu-id="37579-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="37579-153">DateTimeOffset</span></span>|<span data-ttu-id="37579-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="37579-154">DateTime the object was created.</span></span> <span data-ttu-id="37579-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="37579-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="37579-156">description</span><span class="sxs-lookup"><span data-stu-id="37579-156">description</span></span>|<span data-ttu-id="37579-157">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="37579-157">String</span></span>|<span data-ttu-id="37579-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="37579-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="37579-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="37579-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="37579-160">displayName</span><span class="sxs-lookup"><span data-stu-id="37579-160">displayName</span></span>|<span data-ttu-id="37579-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="37579-161">String</span></span>|<span data-ttu-id="37579-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="37579-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="37579-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="37579-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="37579-164">Version</span><span class="sxs-lookup"><span data-stu-id="37579-164">version</span></span>|<span data-ttu-id="37579-165">Int32</span><span class="sxs-lookup"><span data-stu-id="37579-165">Int32</span></span>|<span data-ttu-id="37579-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="37579-166">Version of the device configuration.</span></span> <span data-ttu-id="37579-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="37579-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="37579-168">connectionName</span><span class="sxs-lookup"><span data-stu-id="37579-168">connectionName</span></span>|<span data-ttu-id="37579-169">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="37579-169">String</span></span>|<span data-ttu-id="37579-170">Dem Benutzer angezeigter Verbindungsname.</span><span class="sxs-lookup"><span data-stu-id="37579-170">Connection name displayed to the user.</span></span> <span data-ttu-id="37579-171">Geerbt von [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="37579-171">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="37579-172">Server</span><span class="sxs-lookup"><span data-stu-id="37579-172">servers</span></span>|<span data-ttu-id="37579-173">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="37579-173">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="37579-174">Liste der VPN-Server im Netzwerk.</span><span class="sxs-lookup"><span data-stu-id="37579-174">List of VPN Servers on the network.</span></span> <span data-ttu-id="37579-175">Stellen Sie sicher, dass Endbenutzer auf diese Netzwerkspeicherorte zugreifen können.</span><span class="sxs-lookup"><span data-stu-id="37579-175">Make sure end users can access these network locations.</span></span> <span data-ttu-id="37579-176">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="37579-176">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="37579-177">Geerbt von [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="37579-177">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="37579-178">customXml</span><span class="sxs-lookup"><span data-stu-id="37579-178">customXml</span></span>|<span data-ttu-id="37579-179">Binär</span><span class="sxs-lookup"><span data-stu-id="37579-179">Binary</span></span>|<span data-ttu-id="37579-180">Benutzerdefinierte XML-Befehle, mit denen die VPN-Verbindung konfiguriert wird.</span><span class="sxs-lookup"><span data-stu-id="37579-180">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="37579-181">(UTF8-codiertes Bytearray) Geerbt von [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="37579-181">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="37579-182">profileTarget</span><span class="sxs-lookup"><span data-stu-id="37579-182">profileTarget</span></span>|[<span data-ttu-id="37579-183">windows10VpnProfileTarget</span><span class="sxs-lookup"><span data-stu-id="37579-183">windows10VpnProfileTarget</span></span>](../resources/intune-deviceconfig-windows10vpnprofiletarget.md)|<span data-ttu-id="37579-184">Profil Zieltyp.</span><span class="sxs-lookup"><span data-stu-id="37579-184">Profile target type.</span></span> <span data-ttu-id="37579-185">Mögliche Werte sind: `user`, `device` und `autoPilotDevice`.</span><span class="sxs-lookup"><span data-stu-id="37579-185">Possible values are: `user`, `device`, `autoPilotDevice`.</span></span>|
|<span data-ttu-id="37579-186">connectionType</span><span class="sxs-lookup"><span data-stu-id="37579-186">connectionType</span></span>|[<span data-ttu-id="37579-187">windows10VpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="37579-187">windows10VpnConnectionType</span></span>](../resources/intune-deviceconfig-windows10vpnconnectiontype.md)|<span data-ttu-id="37579-188">Verbindungstyp.</span><span class="sxs-lookup"><span data-stu-id="37579-188">Connection type.</span></span> <span data-ttu-id="37579-189">Mögliche Werte: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `automatic`, `ikEv2`, `l2tp`, `pptp`, `citrix`, `paloAltoGlobalProtect`.</span><span class="sxs-lookup"><span data-stu-id="37579-189">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `automatic`, `ikEv2`, `l2tp`, `pptp`, `citrix`, `paloAltoGlobalProtect`.</span></span>|
|<span data-ttu-id="37579-190">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="37579-190">enableSplitTunneling</span></span>|<span data-ttu-id="37579-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="37579-191">Boolean</span></span>|<span data-ttu-id="37579-192">Aktivieren Sie geteilten Tunneln.</span><span class="sxs-lookup"><span data-stu-id="37579-192">Enable split tunneling.</span></span>|
|<span data-ttu-id="37579-193">enableAlwaysOn</span><span class="sxs-lookup"><span data-stu-id="37579-193">enableAlwaysOn</span></span>|<span data-ttu-id="37579-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="37579-194">Boolean</span></span>|<span data-ttu-id="37579-195">Aktivieren Sie Always on Mode.</span><span class="sxs-lookup"><span data-stu-id="37579-195">Enable Always On mode.</span></span>|
|<span data-ttu-id="37579-196">enableDeviceTunnel</span><span class="sxs-lookup"><span data-stu-id="37579-196">enableDeviceTunnel</span></span>|<span data-ttu-id="37579-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="37579-197">Boolean</span></span>|<span data-ttu-id="37579-198">Aktivieren Sie den Gerätetunnel.</span><span class="sxs-lookup"><span data-stu-id="37579-198">Enable device tunnel.</span></span>|
|<span data-ttu-id="37579-199">enableDnsRegistration</span><span class="sxs-lookup"><span data-stu-id="37579-199">enableDnsRegistration</span></span>|<span data-ttu-id="37579-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="37579-200">Boolean</span></span>|<span data-ttu-id="37579-201">Aktivieren Sie die IP-Adressregistrierung mit internem DNS.</span><span class="sxs-lookup"><span data-stu-id="37579-201">Enable IP address registration with internal DNS.</span></span>|
|<span data-ttu-id="37579-202">dnsSuffixes</span><span class="sxs-lookup"><span data-stu-id="37579-202">dnsSuffixes</span></span>|<span data-ttu-id="37579-203">String collection</span><span class="sxs-lookup"><span data-stu-id="37579-203">String collection</span></span>|<span data-ttu-id="37579-204">Geben Sie DNS-Suffixe an, die der DNS-Suchliste hinzugefügt werden sollen, um kurze Namen ordnungsgemäß weiterzuleiten</span><span class="sxs-lookup"><span data-stu-id="37579-204">Specify DNS suffixes to add to the DNS search list to properly route short names.</span></span>|
|<span data-ttu-id="37579-205">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="37579-205">authenticationMethod</span></span>|[<span data-ttu-id="37579-206">windows10VpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="37579-206">windows10VpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-windows10vpnauthenticationmethod.md)|<span data-ttu-id="37579-207">Authentifizierungsmethode.</span><span class="sxs-lookup"><span data-stu-id="37579-207">Authentication method.</span></span> <span data-ttu-id="37579-208">Mögliche Werte sind: `certificate`, `usernameAndPassword` und `customEapXml`.</span><span class="sxs-lookup"><span data-stu-id="37579-208">Possible values are: `certificate`, `usernameAndPassword`, `customEapXml`.</span></span>|
|<span data-ttu-id="37579-209">rememberUserCredentials</span><span class="sxs-lookup"><span data-stu-id="37579-209">rememberUserCredentials</span></span>|<span data-ttu-id="37579-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="37579-210">Boolean</span></span>|<span data-ttu-id="37579-211">Denken Sie an Benutzeranmeldeinformationen.</span><span class="sxs-lookup"><span data-stu-id="37579-211">Remember user credentials.</span></span>|
|<span data-ttu-id="37579-212">enableConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="37579-212">enableConditionalAccess</span></span>|<span data-ttu-id="37579-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="37579-213">Boolean</span></span>|<span data-ttu-id="37579-214">Aktivieren Sie den bedingten Zugriff.</span><span class="sxs-lookup"><span data-stu-id="37579-214">Enable conditional access.</span></span>|
|<span data-ttu-id="37579-215">enableSingleSignOnWithAlternateCertificate</span><span class="sxs-lookup"><span data-stu-id="37579-215">enableSingleSignOnWithAlternateCertificate</span></span>|<span data-ttu-id="37579-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="37579-216">Boolean</span></span>|<span data-ttu-id="37579-217">Aktivieren Sie einmaliges Anmelden (Single Sign-on, SSO) mit alternativem Zertifikat.</span><span class="sxs-lookup"><span data-stu-id="37579-217">Enable single sign-on (SSO) with alternate certificate.</span></span>|
|<span data-ttu-id="37579-218">singleSignOnEku</span><span class="sxs-lookup"><span data-stu-id="37579-218">singleSignOnEku</span></span>|[<span data-ttu-id="37579-219">extendedKeyUsage</span><span class="sxs-lookup"><span data-stu-id="37579-219">extendedKeyUsage</span></span>](../resources/intune-deviceconfig-extendedkeyusage.md)|<span data-ttu-id="37579-220">Erweiterte Schlüsselverwendung mit einmaligem Anmelden (EKU).</span><span class="sxs-lookup"><span data-stu-id="37579-220">Single sign-on Extended Key Usage (EKU).</span></span>|
|<span data-ttu-id="37579-221">singleSignOnIssuerHash</span><span class="sxs-lookup"><span data-stu-id="37579-221">singleSignOnIssuerHash</span></span>|<span data-ttu-id="37579-222">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="37579-222">String</span></span>|<span data-ttu-id="37579-223">Single Sign-on-Aussteller-Hash.</span><span class="sxs-lookup"><span data-stu-id="37579-223">Single sign-on issuer hash.</span></span>|
|<span data-ttu-id="37579-224">eapXml</span><span class="sxs-lookup"><span data-stu-id="37579-224">eapXml</span></span>|<span data-ttu-id="37579-225">Binär</span><span class="sxs-lookup"><span data-stu-id="37579-225">Binary</span></span>|<span data-ttu-id="37579-226">EAP-XML (Extensible Authentication Protocol).</span><span class="sxs-lookup"><span data-stu-id="37579-226">Extensible Authentication Protocol (EAP) XML.</span></span> <span data-ttu-id="37579-227">(UTF8-codiertes Bytearray)</span><span class="sxs-lookup"><span data-stu-id="37579-227">(UTF8 encoded byte array)</span></span>|
|<span data-ttu-id="37579-228">Sie</span><span class="sxs-lookup"><span data-stu-id="37579-228">proxyServer</span></span>|[<span data-ttu-id="37579-229">windows10VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="37579-229">windows10VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows10vpnproxyserver.md)|<span data-ttu-id="37579-230">Proxy Server.</span><span class="sxs-lookup"><span data-stu-id="37579-230">Proxy Server.</span></span>|
|<span data-ttu-id="37579-231">associatedApps</span><span class="sxs-lookup"><span data-stu-id="37579-231">associatedApps</span></span>|<span data-ttu-id="37579-232">[windows10AssociatedApps](../resources/intune-deviceconfig-windows10associatedapps.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="37579-232">[windows10AssociatedApps](../resources/intune-deviceconfig-windows10associatedapps.md) collection</span></span>|<span data-ttu-id="37579-233">Zugehörige apps.</span><span class="sxs-lookup"><span data-stu-id="37579-233">Associated Apps.</span></span> <span data-ttu-id="37579-234">Diese Collection darf maximal 10.000 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="37579-234">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="37579-235">onlyAssociatedAppsCanUseConnection</span><span class="sxs-lookup"><span data-stu-id="37579-235">onlyAssociatedAppsCanUseConnection</span></span>|<span data-ttu-id="37579-236">Boolean</span><span class="sxs-lookup"><span data-stu-id="37579-236">Boolean</span></span>|<span data-ttu-id="37579-237">Nur zugehörige Apps können eine Verbindung (pro-App-VPN) verwenden.</span><span class="sxs-lookup"><span data-stu-id="37579-237">Only associated Apps can use connection (per-app VPN).</span></span>|
|<span data-ttu-id="37579-238">windowsInformationProtectionDomain</span><span class="sxs-lookup"><span data-stu-id="37579-238">windowsInformationProtectionDomain</span></span>|<span data-ttu-id="37579-239">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="37579-239">String</span></span>|<span data-ttu-id="37579-240">Windows Information Protection (WIP)-Domäne, die dieser Verbindung zugeordnet werden soll.</span><span class="sxs-lookup"><span data-stu-id="37579-240">Windows Information Protection (WIP) domain to associate with this connection.</span></span>|
|<span data-ttu-id="37579-241">trafficRules</span><span class="sxs-lookup"><span data-stu-id="37579-241">trafficRules</span></span>|<span data-ttu-id="37579-242">[vpnTrafficRule](../resources/intune-deviceconfig-vpntrafficrule.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="37579-242">[vpnTrafficRule](../resources/intune-deviceconfig-vpntrafficrule.md) collection</span></span>|<span data-ttu-id="37579-243">Datenverkehrs Regeln.</span><span class="sxs-lookup"><span data-stu-id="37579-243">Traffic rules.</span></span> <span data-ttu-id="37579-244">Diese Sammlung kann bis zu 1000 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="37579-244">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="37579-245">Routen</span><span class="sxs-lookup"><span data-stu-id="37579-245">routes</span></span>|<span data-ttu-id="37579-246">[vpnRoute](../resources/intune-deviceconfig-vpnroute.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="37579-246">[vpnRoute](../resources/intune-deviceconfig-vpnroute.md) collection</span></span>|<span data-ttu-id="37579-247">Routen (optional für Drittanbieter).</span><span class="sxs-lookup"><span data-stu-id="37579-247">Routes (optional for third-party providers).</span></span> <span data-ttu-id="37579-248">Diese Sammlung kann bis zu 1000 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="37579-248">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="37579-249">dnsRules</span><span class="sxs-lookup"><span data-stu-id="37579-249">dnsRules</span></span>|<span data-ttu-id="37579-250">[vpnDnsRule](../resources/intune-deviceconfig-vpndnsrule.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="37579-250">[vpnDnsRule](../resources/intune-deviceconfig-vpndnsrule.md) collection</span></span>|<span data-ttu-id="37579-251">DNS-Regeln.</span><span class="sxs-lookup"><span data-stu-id="37579-251">DNS rules.</span></span> <span data-ttu-id="37579-252">Diese Sammlung kann bis zu 1000 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="37579-252">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="37579-253">trustedNetworkDomains</span><span class="sxs-lookup"><span data-stu-id="37579-253">trustedNetworkDomains</span></span>|<span data-ttu-id="37579-254">String collection</span><span class="sxs-lookup"><span data-stu-id="37579-254">String collection</span></span>|<span data-ttu-id="37579-255">Vertrauenswürdige Netzwerkdomänen</span><span class="sxs-lookup"><span data-stu-id="37579-255">Trusted Network Domains</span></span>|

## <a name="relationships"></a><span data-ttu-id="37579-256">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="37579-256">Relationships</span></span>
|<span data-ttu-id="37579-257">Beziehung</span><span class="sxs-lookup"><span data-stu-id="37579-257">Relationship</span></span>|<span data-ttu-id="37579-258">Typ</span><span class="sxs-lookup"><span data-stu-id="37579-258">Type</span></span>|<span data-ttu-id="37579-259">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="37579-259">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="37579-260">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="37579-260">groupAssignments</span></span>|<span data-ttu-id="37579-261">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="37579-261">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="37579-262">Die Liste derGruppenzuweisungen für das Gerätekonfigurationsprofil.</span><span class="sxs-lookup"><span data-stu-id="37579-262">The list of group assignments for the device configuration profile.</span></span> <span data-ttu-id="37579-263">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="37579-263">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="37579-264">assignments</span><span class="sxs-lookup"><span data-stu-id="37579-264">assignments</span></span>|<span data-ttu-id="37579-265">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="37579-265">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="37579-266">Liste der Zuweisungen für das Gerätekonfigurationsprofil.</span><span class="sxs-lookup"><span data-stu-id="37579-266">The list of assignments for the device configuration profile.</span></span> <span data-ttu-id="37579-267">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="37579-267">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="37579-268">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="37579-268">deviceStatuses</span></span>|<span data-ttu-id="37579-269">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="37579-269">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="37579-270">Installationsstatus der Gerätekonfiguration nach Gerät.</span><span class="sxs-lookup"><span data-stu-id="37579-270">Device configuration installation status by device.</span></span> <span data-ttu-id="37579-271">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="37579-271">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="37579-272">userStatuses</span><span class="sxs-lookup"><span data-stu-id="37579-272">userStatuses</span></span>|<span data-ttu-id="37579-273">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="37579-273">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="37579-274">Installationsstatus der Gerätekonfiguration nach Benutzer.</span><span class="sxs-lookup"><span data-stu-id="37579-274">Device configuration installation status by user.</span></span> <span data-ttu-id="37579-275">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="37579-275">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="37579-276">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="37579-276">deviceStatusOverview</span></span>|[<span data-ttu-id="37579-277">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="37579-277">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="37579-278">Übersicht über den Status der Gerätekonfiguration nach Gerät. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="37579-278">Device Configuration devices status overview Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="37579-279">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="37579-279">userStatusOverview</span></span>|[<span data-ttu-id="37579-280">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="37579-280">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="37579-281">Übersicht über den Status der Gerätekonfiguration nach Benutzer. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="37579-281">Device Configuration users status overview Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="37579-282">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="37579-282">deviceSettingStateSummaries</span></span>|<span data-ttu-id="37579-283"> [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="37579-283">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="37579-284">Übersicht über den Einstellungsstatus für die Gerätekonfiguration nach Gerät. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="37579-284">Device Configuration Setting State Device Summary Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="37579-285">identityCertificate</span><span class="sxs-lookup"><span data-stu-id="37579-285">identityCertificate</span></span>|[<span data-ttu-id="37579-286">windowsCertificateProfileBase</span><span class="sxs-lookup"><span data-stu-id="37579-286">windowsCertificateProfileBase</span></span>](../resources/intune-deviceconfig-windowscertificateprofilebase.md)|<span data-ttu-id="37579-287">Identitätszertifikat für die Clientauthentifizierung, wenn die Authentifizierungsmethode das Zertifikat ist.</span><span class="sxs-lookup"><span data-stu-id="37579-287">Identity certificate for client authentication when authentication method is certificate.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="37579-288">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="37579-288">JSON Representation</span></span>
<span data-ttu-id="37579-289">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="37579-289">Here is a JSON representation of the resource.</span></span>
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
      "proxyServerUri": "String",
      "autoTrigger": true,
      "persistent": true
    }
  ],
  "trustedNetworkDomains": [
    "String"
  ]
}
```




