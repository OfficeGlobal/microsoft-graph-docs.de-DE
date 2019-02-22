---
title: Windows10VpnConfiguration erstellen
description: Erstellen eines neuen windows10VpnConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0d6fc1972f04d4699294f0635c87411f72744ac6
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30148195"
---
# <a name="create-windows10vpnconfiguration"></a><span data-ttu-id="536c4-103">Windows10VpnConfiguration erstellen</span><span class="sxs-lookup"><span data-stu-id="536c4-103">Create windows10VpnConfiguration</span></span>

> <span data-ttu-id="536c4-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="536c4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="536c4-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="536c4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="536c4-106">Erstellen eines neuen [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="536c4-106">Create a new [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="536c4-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="536c4-107">Prerequisites</span></span>
<span data-ttu-id="536c4-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="536c4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="536c4-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="536c4-110">Permission type</span></span>|<span data-ttu-id="536c4-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="536c4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="536c4-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="536c4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="536c4-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="536c4-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="536c4-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="536c4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="536c4-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="536c4-115">Not supported.</span></span>|
|<span data-ttu-id="536c4-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="536c4-116">Application</span></span>|<span data-ttu-id="536c4-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="536c4-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="536c4-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="536c4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="536c4-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="536c4-119">Request headers</span></span>
|<span data-ttu-id="536c4-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="536c4-120">Header</span></span>|<span data-ttu-id="536c4-121">Wert</span><span class="sxs-lookup"><span data-stu-id="536c4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="536c4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="536c4-122">Authorization</span></span>|<span data-ttu-id="536c4-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="536c4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="536c4-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="536c4-124">Accept</span></span>|<span data-ttu-id="536c4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="536c4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="536c4-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="536c4-126">Request body</span></span>
<span data-ttu-id="536c4-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das windows10VpnConfiguration-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="536c4-127">In the request body, supply a JSON representation for the windows10VpnConfiguration object.</span></span>

<span data-ttu-id="536c4-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der windows10VpnConfiguration erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="536c4-128">The following table shows the properties that are required when you create the windows10VpnConfiguration.</span></span>

|<span data-ttu-id="536c4-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="536c4-129">Property</span></span>|<span data-ttu-id="536c4-130">Typ</span><span class="sxs-lookup"><span data-stu-id="536c4-130">Type</span></span>|<span data-ttu-id="536c4-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="536c4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="536c4-132">id</span><span class="sxs-lookup"><span data-stu-id="536c4-132">id</span></span>|<span data-ttu-id="536c4-133">string</span><span class="sxs-lookup"><span data-stu-id="536c4-133">String</span></span>|<span data-ttu-id="536c4-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="536c4-134">Key of the entity.</span></span> <span data-ttu-id="536c4-135">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="536c4-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="536c4-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="536c4-136">lastModifiedDateTime</span></span>|<span data-ttu-id="536c4-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="536c4-137">DateTimeOffset</span></span>|<span data-ttu-id="536c4-138">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="536c4-138">DateTime the object was last modified.</span></span> <span data-ttu-id="536c4-139">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="536c4-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="536c4-140">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="536c4-140">roleScopeTagIds</span></span>|<span data-ttu-id="536c4-141">String collection</span><span class="sxs-lookup"><span data-stu-id="536c4-141">String collection</span></span>|<span data-ttu-id="536c4-142">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="536c4-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="536c4-143">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="536c4-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="536c4-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="536c4-144">supportsScopeTags</span></span>|<span data-ttu-id="536c4-145">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="536c4-145">Boolean</span></span>|<span data-ttu-id="536c4-146">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereichs Tags unterstützt.</span><span class="sxs-lookup"><span data-stu-id="536c4-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="536c4-147">Das Zuweisen zur ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert auf false festgelegt ist und Entitäten für bereichsbezogene Benutzer nicht sichtbar sind.</span><span class="sxs-lookup"><span data-stu-id="536c4-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="536c4-148">Dies geschieht für in Silverlight erstellte Legacy Richtlinien und kann durch Löschen und erneutes Erstellen der Richtlinie im Azure-Portal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="536c4-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="536c4-149">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="536c4-149">This property is read-only.</span></span> <span data-ttu-id="536c4-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="536c4-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="536c4-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="536c4-151">createdDateTime</span></span>|<span data-ttu-id="536c4-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="536c4-152">DateTimeOffset</span></span>|<span data-ttu-id="536c4-153">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="536c4-153">DateTime the object was created.</span></span> <span data-ttu-id="536c4-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="536c4-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="536c4-155">description</span><span class="sxs-lookup"><span data-stu-id="536c4-155">description</span></span>|<span data-ttu-id="536c4-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="536c4-156">String</span></span>|<span data-ttu-id="536c4-157">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="536c4-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="536c4-158">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="536c4-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="536c4-159">displayName</span><span class="sxs-lookup"><span data-stu-id="536c4-159">displayName</span></span>|<span data-ttu-id="536c4-160">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="536c4-160">String</span></span>|<span data-ttu-id="536c4-161">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="536c4-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="536c4-162">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="536c4-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="536c4-163">Version</span><span class="sxs-lookup"><span data-stu-id="536c4-163">version</span></span>|<span data-ttu-id="536c4-164">Int32</span><span class="sxs-lookup"><span data-stu-id="536c4-164">Int32</span></span>|<span data-ttu-id="536c4-165">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="536c4-165">Version of the device configuration.</span></span> <span data-ttu-id="536c4-166">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="536c4-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="536c4-167">connectionName</span><span class="sxs-lookup"><span data-stu-id="536c4-167">connectionName</span></span>|<span data-ttu-id="536c4-168">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="536c4-168">String</span></span>|<span data-ttu-id="536c4-169">Dem Benutzer angezeigter Verbindungsname.</span><span class="sxs-lookup"><span data-stu-id="536c4-169">Connection name displayed to the user.</span></span> <span data-ttu-id="536c4-170">Geerbt von [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="536c4-170">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="536c4-171">Server</span><span class="sxs-lookup"><span data-stu-id="536c4-171">servers</span></span>|<span data-ttu-id="536c4-172">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="536c4-172">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="536c4-173">Liste der VPN-Server im Netzwerk.</span><span class="sxs-lookup"><span data-stu-id="536c4-173">List of VPN Servers on the network.</span></span> <span data-ttu-id="536c4-174">Stellen Sie sicher, dass Endbenutzer auf diese Netzwerkspeicherorte zugreifen können.</span><span class="sxs-lookup"><span data-stu-id="536c4-174">Make sure end users can access these network locations.</span></span> <span data-ttu-id="536c4-175">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="536c4-175">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="536c4-176">Geerbt von [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="536c4-176">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="536c4-177">customXml</span><span class="sxs-lookup"><span data-stu-id="536c4-177">customXml</span></span>|<span data-ttu-id="536c4-178">Binär</span><span class="sxs-lookup"><span data-stu-id="536c4-178">Binary</span></span>|<span data-ttu-id="536c4-179">Benutzerdefinierte XML-Befehle, mit denen die VPN-Verbindung konfiguriert wird.</span><span class="sxs-lookup"><span data-stu-id="536c4-179">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="536c4-180">(UTF8-codiertes Bytearray) Geerbt von [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="536c4-180">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="536c4-181">profileTarget</span><span class="sxs-lookup"><span data-stu-id="536c4-181">profileTarget</span></span>|[<span data-ttu-id="536c4-182">windows10VpnProfileTarget</span><span class="sxs-lookup"><span data-stu-id="536c4-182">windows10VpnProfileTarget</span></span>](../resources/intune-deviceconfig-windows10vpnprofiletarget.md)|<span data-ttu-id="536c4-183">Profil Zieltyp.</span><span class="sxs-lookup"><span data-stu-id="536c4-183">Profile target type.</span></span> <span data-ttu-id="536c4-184">Mögliche Werte sind: `user`, `device` und `autoPilotDevice`.</span><span class="sxs-lookup"><span data-stu-id="536c4-184">Possible values are: `user`, `device`, `autoPilotDevice`.</span></span>|
|<span data-ttu-id="536c4-185">connectionType</span><span class="sxs-lookup"><span data-stu-id="536c4-185">connectionType</span></span>|[<span data-ttu-id="536c4-186">windows10VpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="536c4-186">windows10VpnConnectionType</span></span>](../resources/intune-deviceconfig-windows10vpnconnectiontype.md)|<span data-ttu-id="536c4-187">Verbindungstyp.</span><span class="sxs-lookup"><span data-stu-id="536c4-187">Connection type.</span></span> <span data-ttu-id="536c4-188">Mögliche Werte: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `automatic`, `ikEv2`, `l2tp`, `pptp`, `citrix`, `paloAltoGlobalProtect`.</span><span class="sxs-lookup"><span data-stu-id="536c4-188">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `automatic`, `ikEv2`, `l2tp`, `pptp`, `citrix`, `paloAltoGlobalProtect`.</span></span>|
|<span data-ttu-id="536c4-189">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="536c4-189">enableSplitTunneling</span></span>|<span data-ttu-id="536c4-190">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="536c4-190">Boolean</span></span>|<span data-ttu-id="536c4-191">Aktivieren Sie geteilten Tunneln.</span><span class="sxs-lookup"><span data-stu-id="536c4-191">Enable split tunneling.</span></span>|
|<span data-ttu-id="536c4-192">enableAlwaysOn</span><span class="sxs-lookup"><span data-stu-id="536c4-192">enableAlwaysOn</span></span>|<span data-ttu-id="536c4-193">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="536c4-193">Boolean</span></span>|<span data-ttu-id="536c4-194">Aktivieren Sie Always on Mode.</span><span class="sxs-lookup"><span data-stu-id="536c4-194">Enable Always On mode.</span></span>|
|<span data-ttu-id="536c4-195">enableDeviceTunnel</span><span class="sxs-lookup"><span data-stu-id="536c4-195">enableDeviceTunnel</span></span>|<span data-ttu-id="536c4-196">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="536c4-196">Boolean</span></span>|<span data-ttu-id="536c4-197">Aktivieren Sie den Gerätetunnel.</span><span class="sxs-lookup"><span data-stu-id="536c4-197">Enable device tunnel.</span></span>|
|<span data-ttu-id="536c4-198">enableDnsRegistration</span><span class="sxs-lookup"><span data-stu-id="536c4-198">enableDnsRegistration</span></span>|<span data-ttu-id="536c4-199">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="536c4-199">Boolean</span></span>|<span data-ttu-id="536c4-200">Aktivieren Sie die IP-Adressregistrierung mit internem DNS.</span><span class="sxs-lookup"><span data-stu-id="536c4-200">Enable IP address registration with internal DNS.</span></span>|
|<span data-ttu-id="536c4-201">dnsSuffixes</span><span class="sxs-lookup"><span data-stu-id="536c4-201">dnsSuffixes</span></span>|<span data-ttu-id="536c4-202">String collection</span><span class="sxs-lookup"><span data-stu-id="536c4-202">String collection</span></span>|<span data-ttu-id="536c4-203">Geben Sie DNS-Suffixe an, die der DNS-Suchliste hinzugefügt werden sollen, um kurze Namen ordnungsgemäß weiterzuleiten</span><span class="sxs-lookup"><span data-stu-id="536c4-203">Specify DNS suffixes to add to the DNS search list to properly route short names.</span></span>|
|<span data-ttu-id="536c4-204">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="536c4-204">authenticationMethod</span></span>|[<span data-ttu-id="536c4-205">windows10VpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="536c4-205">windows10VpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-windows10vpnauthenticationmethod.md)|<span data-ttu-id="536c4-206">Authentifizierungsmethode.</span><span class="sxs-lookup"><span data-stu-id="536c4-206">Authentication method.</span></span> <span data-ttu-id="536c4-207">Mögliche Werte sind: `certificate`, `usernameAndPassword` und `customEapXml`.</span><span class="sxs-lookup"><span data-stu-id="536c4-207">Possible values are: `certificate`, `usernameAndPassword`, `customEapXml`.</span></span>|
|<span data-ttu-id="536c4-208">rememberUserCredentials</span><span class="sxs-lookup"><span data-stu-id="536c4-208">rememberUserCredentials</span></span>|<span data-ttu-id="536c4-209">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="536c4-209">Boolean</span></span>|<span data-ttu-id="536c4-210">Denken Sie an Benutzeranmeldeinformationen.</span><span class="sxs-lookup"><span data-stu-id="536c4-210">Remember user credentials.</span></span>|
|<span data-ttu-id="536c4-211">enableConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="536c4-211">enableConditionalAccess</span></span>|<span data-ttu-id="536c4-212">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="536c4-212">Boolean</span></span>|<span data-ttu-id="536c4-213">Aktivieren Sie den bedingten Zugriff.</span><span class="sxs-lookup"><span data-stu-id="536c4-213">Enable conditional access.</span></span>|
|<span data-ttu-id="536c4-214">enableSingleSignOnWithAlternateCertificate</span><span class="sxs-lookup"><span data-stu-id="536c4-214">enableSingleSignOnWithAlternateCertificate</span></span>|<span data-ttu-id="536c4-215">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="536c4-215">Boolean</span></span>|<span data-ttu-id="536c4-216">Aktivieren Sie einmaliges Anmelden (Single Sign-on, SSO) mit alternativem Zertifikat.</span><span class="sxs-lookup"><span data-stu-id="536c4-216">Enable single sign-on (SSO) with alternate certificate.</span></span>|
|<span data-ttu-id="536c4-217">singleSignOnEku</span><span class="sxs-lookup"><span data-stu-id="536c4-217">singleSignOnEku</span></span>|[<span data-ttu-id="536c4-218">extendedKeyUsage</span><span class="sxs-lookup"><span data-stu-id="536c4-218">extendedKeyUsage</span></span>](../resources/intune-deviceconfig-extendedkeyusage.md)|<span data-ttu-id="536c4-219">Erweiterte Schlüsselverwendung mit einmaligem Anmelden (EKU).</span><span class="sxs-lookup"><span data-stu-id="536c4-219">Single sign-on Extended Key Usage (EKU).</span></span>|
|<span data-ttu-id="536c4-220">singleSignOnIssuerHash</span><span class="sxs-lookup"><span data-stu-id="536c4-220">singleSignOnIssuerHash</span></span>|<span data-ttu-id="536c4-221">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="536c4-221">String</span></span>|<span data-ttu-id="536c4-222">Single Sign-on-Aussteller-Hash.</span><span class="sxs-lookup"><span data-stu-id="536c4-222">Single sign-on issuer hash.</span></span>|
|<span data-ttu-id="536c4-223">eapXml</span><span class="sxs-lookup"><span data-stu-id="536c4-223">eapXml</span></span>|<span data-ttu-id="536c4-224">Binär</span><span class="sxs-lookup"><span data-stu-id="536c4-224">Binary</span></span>|<span data-ttu-id="536c4-225">EAP-XML (Extensible Authentication Protocol).</span><span class="sxs-lookup"><span data-stu-id="536c4-225">Extensible Authentication Protocol (EAP) XML.</span></span> <span data-ttu-id="536c4-226">(UTF8-codiertes Bytearray)</span><span class="sxs-lookup"><span data-stu-id="536c4-226">(UTF8 encoded byte array)</span></span>|
|<span data-ttu-id="536c4-227">Sie</span><span class="sxs-lookup"><span data-stu-id="536c4-227">proxyServer</span></span>|[<span data-ttu-id="536c4-228">windows10VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="536c4-228">windows10VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows10vpnproxyserver.md)|<span data-ttu-id="536c4-229">Proxy Server.</span><span class="sxs-lookup"><span data-stu-id="536c4-229">Proxy Server.</span></span>|
|<span data-ttu-id="536c4-230">associatedApps</span><span class="sxs-lookup"><span data-stu-id="536c4-230">associatedApps</span></span>|<span data-ttu-id="536c4-231">[windows10AssociatedApps](../resources/intune-deviceconfig-windows10associatedapps.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="536c4-231">[windows10AssociatedApps](../resources/intune-deviceconfig-windows10associatedapps.md) collection</span></span>|<span data-ttu-id="536c4-232">Zugehörige apps.</span><span class="sxs-lookup"><span data-stu-id="536c4-232">Associated Apps.</span></span> <span data-ttu-id="536c4-233">Diese Collection darf maximal 10.000 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="536c4-233">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="536c4-234">onlyAssociatedAppsCanUseConnection</span><span class="sxs-lookup"><span data-stu-id="536c4-234">onlyAssociatedAppsCanUseConnection</span></span>|<span data-ttu-id="536c4-235">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="536c4-235">Boolean</span></span>|<span data-ttu-id="536c4-236">Nur zugehörige Apps können eine Verbindung (pro-App-VPN) verwenden.</span><span class="sxs-lookup"><span data-stu-id="536c4-236">Only associated Apps can use connection (per-app VPN).</span></span>|
|<span data-ttu-id="536c4-237">windowsInformationProtectionDomain</span><span class="sxs-lookup"><span data-stu-id="536c4-237">windowsInformationProtectionDomain</span></span>|<span data-ttu-id="536c4-238">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="536c4-238">String</span></span>|<span data-ttu-id="536c4-239">Windows Information Protection (WIP)-Domäne, die dieser Verbindung zugeordnet werden soll.</span><span class="sxs-lookup"><span data-stu-id="536c4-239">Windows Information Protection (WIP) domain to associate with this connection.</span></span>|
|<span data-ttu-id="536c4-240">trafficRules</span><span class="sxs-lookup"><span data-stu-id="536c4-240">trafficRules</span></span>|<span data-ttu-id="536c4-241">[vpnTrafficRule](../resources/intune-deviceconfig-vpntrafficrule.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="536c4-241">[vpnTrafficRule](../resources/intune-deviceconfig-vpntrafficrule.md) collection</span></span>|<span data-ttu-id="536c4-242">Datenverkehrs Regeln.</span><span class="sxs-lookup"><span data-stu-id="536c4-242">Traffic rules.</span></span> <span data-ttu-id="536c4-243">Diese Sammlung kann bis zu 1000 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="536c4-243">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="536c4-244">Routen</span><span class="sxs-lookup"><span data-stu-id="536c4-244">routes</span></span>|<span data-ttu-id="536c4-245">[vpnRoute](../resources/intune-deviceconfig-vpnroute.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="536c4-245">[vpnRoute](../resources/intune-deviceconfig-vpnroute.md) collection</span></span>|<span data-ttu-id="536c4-246">Routen (optional für Drittanbieter).</span><span class="sxs-lookup"><span data-stu-id="536c4-246">Routes (optional for third-party providers).</span></span> <span data-ttu-id="536c4-247">Diese Sammlung kann bis zu 1000 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="536c4-247">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="536c4-248">dnsRules</span><span class="sxs-lookup"><span data-stu-id="536c4-248">dnsRules</span></span>|<span data-ttu-id="536c4-249">[vpnDnsRule](../resources/intune-deviceconfig-vpndnsrule.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="536c4-249">[vpnDnsRule](../resources/intune-deviceconfig-vpndnsrule.md) collection</span></span>|<span data-ttu-id="536c4-250">DNS-Regeln.</span><span class="sxs-lookup"><span data-stu-id="536c4-250">DNS rules.</span></span> <span data-ttu-id="536c4-251">Diese Sammlung kann bis zu 1000 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="536c4-251">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="536c4-252">trustedNetworkDomains</span><span class="sxs-lookup"><span data-stu-id="536c4-252">trustedNetworkDomains</span></span>|<span data-ttu-id="536c4-253">String collection</span><span class="sxs-lookup"><span data-stu-id="536c4-253">String collection</span></span>|<span data-ttu-id="536c4-254">Vertrauenswürdige Netzwerkdomänen</span><span class="sxs-lookup"><span data-stu-id="536c4-254">Trusted Network Domains</span></span>|



## <a name="response"></a><span data-ttu-id="536c4-255">Antwort</span><span class="sxs-lookup"><span data-stu-id="536c4-255">Response</span></span>
<span data-ttu-id="536c4-256">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="536c4-256">If successful, this method returns a `201 Created` response code and a [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="536c4-257">Beispiel</span><span class="sxs-lookup"><span data-stu-id="536c4-257">Example</span></span>

### <a name="request"></a><span data-ttu-id="536c4-258">Anforderung</span><span class="sxs-lookup"><span data-stu-id="536c4-258">Request</span></span>
<span data-ttu-id="536c4-259">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="536c4-259">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 3387

{
  "@odata.type": "#microsoft.graph.windows10VpnConfiguration",
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
      "proxyServerUri": "Proxy Server Uri value",
      "autoTrigger": true,
      "persistent": true
    }
  ],
  "trustedNetworkDomains": [
    "Trusted Network Domains value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="536c4-260">Antwort</span><span class="sxs-lookup"><span data-stu-id="536c4-260">Response</span></span>
<span data-ttu-id="536c4-p121">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="536c4-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 3559

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
      "proxyServerUri": "Proxy Server Uri value",
      "autoTrigger": true,
      "persistent": true
    }
  ],
  "trustedNetworkDomains": [
    "Trusted Network Domains value"
  ]
}
```




