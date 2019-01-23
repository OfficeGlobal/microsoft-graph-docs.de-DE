---
title: Erstellen von windows10VpnConfiguration
description: Erstellen eines neuen windows10VpnConfiguration-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 72264db454928358068f31dc5a439a5e74ce1da6
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29412044"
---
# <a name="create-windows10vpnconfiguration"></a><span data-ttu-id="6b196-103">Erstellen von windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="6b196-103">Create windows10VpnConfiguration</span></span>

> <span data-ttu-id="6b196-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="6b196-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="6b196-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6b196-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6b196-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6b196-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6b196-107">Erstellen eines neuen [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="6b196-107">Create a new [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6b196-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="6b196-108">Prerequisites</span></span>
<span data-ttu-id="6b196-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="6b196-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="6b196-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6b196-111">Permission type</span></span>|<span data-ttu-id="6b196-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6b196-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6b196-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6b196-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6b196-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b196-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6b196-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6b196-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6b196-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6b196-116">Not supported.</span></span>|
|<span data-ttu-id="6b196-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6b196-117">Application</span></span>|<span data-ttu-id="6b196-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6b196-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6b196-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6b196-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="6b196-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6b196-120">Request headers</span></span>
|<span data-ttu-id="6b196-121">Header</span><span class="sxs-lookup"><span data-stu-id="6b196-121">Header</span></span>|<span data-ttu-id="6b196-122">Wert</span><span class="sxs-lookup"><span data-stu-id="6b196-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6b196-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="6b196-123">Authorization</span></span>|<span data-ttu-id="6b196-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="6b196-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6b196-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="6b196-125">Accept</span></span>|<span data-ttu-id="6b196-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6b196-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6b196-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6b196-127">Request body</span></span>
<span data-ttu-id="6b196-128">Geben Sie im Textkörper Anforderung für das Objekt windows10VpnConfiguration eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="6b196-128">In the request body, supply a JSON representation for the windows10VpnConfiguration object.</span></span>

<span data-ttu-id="6b196-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die windows10VpnConfiguration erstellen.</span><span class="sxs-lookup"><span data-stu-id="6b196-129">The following table shows the properties that are required when you create the windows10VpnConfiguration.</span></span>

|<span data-ttu-id="6b196-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6b196-130">Property</span></span>|<span data-ttu-id="6b196-131">Typ</span><span class="sxs-lookup"><span data-stu-id="6b196-131">Type</span></span>|<span data-ttu-id="6b196-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6b196-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6b196-133">id</span><span class="sxs-lookup"><span data-stu-id="6b196-133">id</span></span>|<span data-ttu-id="6b196-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6b196-134">String</span></span>|<span data-ttu-id="6b196-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="6b196-135">Key of the entity.</span></span> <span data-ttu-id="6b196-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6b196-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6b196-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6b196-137">lastModifiedDateTime</span></span>|<span data-ttu-id="6b196-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6b196-138">DateTimeOffset</span></span>|<span data-ttu-id="6b196-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="6b196-139">DateTime the object was last modified.</span></span> <span data-ttu-id="6b196-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6b196-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6b196-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6b196-141">roleScopeTagIds</span></span>|<span data-ttu-id="6b196-142">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="6b196-142">String collection</span></span>|<span data-ttu-id="6b196-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="6b196-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="6b196-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6b196-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6b196-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="6b196-145">supportsScopeTags</span></span>|<span data-ttu-id="6b196-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b196-146">Boolean</span></span>|<span data-ttu-id="6b196-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6b196-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="6b196-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="6b196-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="6b196-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="6b196-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="6b196-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="6b196-150">This property is read-only.</span></span> <span data-ttu-id="6b196-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6b196-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6b196-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6b196-152">createdDateTime</span></span>|<span data-ttu-id="6b196-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6b196-153">DateTimeOffset</span></span>|<span data-ttu-id="6b196-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="6b196-154">DateTime the object was created.</span></span> <span data-ttu-id="6b196-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6b196-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6b196-156">description</span><span class="sxs-lookup"><span data-stu-id="6b196-156">description</span></span>|<span data-ttu-id="6b196-157">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6b196-157">String</span></span>|<span data-ttu-id="6b196-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="6b196-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6b196-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6b196-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6b196-160">displayName</span><span class="sxs-lookup"><span data-stu-id="6b196-160">displayName</span></span>|<span data-ttu-id="6b196-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6b196-161">String</span></span>|<span data-ttu-id="6b196-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="6b196-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6b196-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6b196-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6b196-164">Version</span><span class="sxs-lookup"><span data-stu-id="6b196-164">version</span></span>|<span data-ttu-id="6b196-165">Int32</span><span class="sxs-lookup"><span data-stu-id="6b196-165">Int32</span></span>|<span data-ttu-id="6b196-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="6b196-166">Version of the device configuration.</span></span> <span data-ttu-id="6b196-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6b196-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6b196-168">connectionName</span><span class="sxs-lookup"><span data-stu-id="6b196-168">connectionName</span></span>|<span data-ttu-id="6b196-169">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6b196-169">String</span></span>|<span data-ttu-id="6b196-170">Name der Verbindung für den Benutzer angezeigt.</span><span class="sxs-lookup"><span data-stu-id="6b196-170">Connection name displayed to the user.</span></span> <span data-ttu-id="6b196-171">Geerbt von [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6b196-171">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="6b196-172">Server</span><span class="sxs-lookup"><span data-stu-id="6b196-172">servers</span></span>|<span data-ttu-id="6b196-173">[VpnServer](../resources/intune-deviceconfig-vpnserver.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="6b196-173">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="6b196-174">Liste der VPN-Server im Netzwerk.</span><span class="sxs-lookup"><span data-stu-id="6b196-174">List of VPN Servers on the network.</span></span> <span data-ttu-id="6b196-175">Stellen Sie sicher, dass Endbenutzer diese Netzwerkadressen zugreifen können.</span><span class="sxs-lookup"><span data-stu-id="6b196-175">Make sure end users can access these network locations.</span></span> <span data-ttu-id="6b196-176">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="6b196-176">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="6b196-177">Geerbt von [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6b196-177">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="6b196-178">customXml</span><span class="sxs-lookup"><span data-stu-id="6b196-178">customXml</span></span>|<span data-ttu-id="6b196-179">Binär</span><span class="sxs-lookup"><span data-stu-id="6b196-179">Binary</span></span>|<span data-ttu-id="6b196-180">Benutzerdefinierte XML-Befehle, die die VPN-Verbindung konfiguriert.</span><span class="sxs-lookup"><span data-stu-id="6b196-180">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="6b196-181">(UTF8 codiert Bytearray) Geerbt von [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6b196-181">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="6b196-182">profileTarget</span><span class="sxs-lookup"><span data-stu-id="6b196-182">profileTarget</span></span>|[<span data-ttu-id="6b196-183">windows10VpnProfileTarget</span><span class="sxs-lookup"><span data-stu-id="6b196-183">windows10VpnProfileTarget</span></span>](../resources/intune-deviceconfig-windows10vpnprofiletarget.md)|<span data-ttu-id="6b196-184">Profil Zieltyp.</span><span class="sxs-lookup"><span data-stu-id="6b196-184">Profile target type.</span></span> <span data-ttu-id="6b196-185">Mögliche Werte sind: `user`, `device` und `autoPilotDevice`.</span><span class="sxs-lookup"><span data-stu-id="6b196-185">Possible values are: `user`, `device`, `autoPilotDevice`.</span></span>|
|<span data-ttu-id="6b196-186">connectionType</span><span class="sxs-lookup"><span data-stu-id="6b196-186">connectionType</span></span>|[<span data-ttu-id="6b196-187">windows10VpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="6b196-187">windows10VpnConnectionType</span></span>](../resources/intune-deviceconfig-windows10vpnconnectiontype.md)|<span data-ttu-id="6b196-188">Verbindungstyp.</span><span class="sxs-lookup"><span data-stu-id="6b196-188">Connection type.</span></span> <span data-ttu-id="6b196-189">Mögliche Werte: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `automatic`, `ikEv2`, `l2tp`, `pptp`, `citrix`, `paloAltoGlobalProtect`.</span><span class="sxs-lookup"><span data-stu-id="6b196-189">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `automatic`, `ikEv2`, `l2tp`, `pptp`, `citrix`, `paloAltoGlobalProtect`.</span></span>|
|<span data-ttu-id="6b196-190">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="6b196-190">enableSplitTunneling</span></span>|<span data-ttu-id="6b196-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b196-191">Boolean</span></span>|<span data-ttu-id="6b196-192">Split-tunneling zu aktivieren.</span><span class="sxs-lookup"><span data-stu-id="6b196-192">Enable split tunneling.</span></span>|
|<span data-ttu-id="6b196-193">enableAlwaysOn</span><span class="sxs-lookup"><span data-stu-id="6b196-193">enableAlwaysOn</span></span>|<span data-ttu-id="6b196-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b196-194">Boolean</span></span>|<span data-ttu-id="6b196-195">Aktivieren Sie Always On-Modus.</span><span class="sxs-lookup"><span data-stu-id="6b196-195">Enable Always On mode.</span></span>|
|<span data-ttu-id="6b196-196">enableDeviceTunnel</span><span class="sxs-lookup"><span data-stu-id="6b196-196">enableDeviceTunnel</span></span>|<span data-ttu-id="6b196-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b196-197">Boolean</span></span>|<span data-ttu-id="6b196-198">Aktivieren Sie Gerät Tunnel.</span><span class="sxs-lookup"><span data-stu-id="6b196-198">Enable device tunnel.</span></span>|
|<span data-ttu-id="6b196-199">enableDnsRegistration</span><span class="sxs-lookup"><span data-stu-id="6b196-199">enableDnsRegistration</span></span>|<span data-ttu-id="6b196-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b196-200">Boolean</span></span>|<span data-ttu-id="6b196-201">Aktivieren Sie die IP-Adressregistrierung mit internen DNS.</span><span class="sxs-lookup"><span data-stu-id="6b196-201">Enable IP address registration with internal DNS.</span></span>|
|<span data-ttu-id="6b196-202">dnsSuffixes</span><span class="sxs-lookup"><span data-stu-id="6b196-202">dnsSuffixes</span></span>|<span data-ttu-id="6b196-203">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="6b196-203">String collection</span></span>|<span data-ttu-id="6b196-204">Geben Sie die DNS-Suffixe hinzufügen zu DNS-Suchliste Kurznamen ordnungsgemäß weitergeleitet.</span><span class="sxs-lookup"><span data-stu-id="6b196-204">Specify DNS suffixes to add to the DNS search list to properly route short names.</span></span>|
|<span data-ttu-id="6b196-205">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="6b196-205">authenticationMethod</span></span>|[<span data-ttu-id="6b196-206">windows10VpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="6b196-206">windows10VpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-windows10vpnauthenticationmethod.md)|<span data-ttu-id="6b196-207">Authentifizierungsmethode.</span><span class="sxs-lookup"><span data-stu-id="6b196-207">Authentication method.</span></span> <span data-ttu-id="6b196-208">Mögliche Werte sind: `certificate`, `usernameAndPassword` und `customEapXml`.</span><span class="sxs-lookup"><span data-stu-id="6b196-208">Possible values are: `certificate`, `usernameAndPassword`, `customEapXml`.</span></span>|
|<span data-ttu-id="6b196-209">rememberUserCredentials</span><span class="sxs-lookup"><span data-stu-id="6b196-209">rememberUserCredentials</span></span>|<span data-ttu-id="6b196-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b196-210">Boolean</span></span>|<span data-ttu-id="6b196-211">Beachten Sie die Anmeldeinformationen des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="6b196-211">Remember user credentials.</span></span>|
|<span data-ttu-id="6b196-212">enableConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="6b196-212">enableConditionalAccess</span></span>|<span data-ttu-id="6b196-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b196-213">Boolean</span></span>|<span data-ttu-id="6b196-214">Aktivieren Sie bedingte Zugriff.</span><span class="sxs-lookup"><span data-stu-id="6b196-214">Enable conditional access.</span></span>|
|<span data-ttu-id="6b196-215">enableSingleSignOnWithAlternateCertificate</span><span class="sxs-lookup"><span data-stu-id="6b196-215">enableSingleSignOnWithAlternateCertificate</span></span>|<span data-ttu-id="6b196-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b196-216">Boolean</span></span>|<span data-ttu-id="6b196-217">Aktivieren Sie einmaliges Anmelden (SSO) mit anderen Zertifikats.</span><span class="sxs-lookup"><span data-stu-id="6b196-217">Enable single sign-on (SSO) with alternate certificate.</span></span>|
|<span data-ttu-id="6b196-218">singleSignOnEku</span><span class="sxs-lookup"><span data-stu-id="6b196-218">singleSignOnEku</span></span>|[<span data-ttu-id="6b196-219">extendedKeyUsage</span><span class="sxs-lookup"><span data-stu-id="6b196-219">extendedKeyUsage</span></span>](../resources/intune-deviceconfig-extendedkeyusage.md)|<span data-ttu-id="6b196-220">Einmaliges Anmelden erweiterte Schlüsselverwendung (EKU).</span><span class="sxs-lookup"><span data-stu-id="6b196-220">Single sign-on Extended Key Usage (EKU).</span></span>|
|<span data-ttu-id="6b196-221">singleSignOnIssuerHash</span><span class="sxs-lookup"><span data-stu-id="6b196-221">singleSignOnIssuerHash</span></span>|<span data-ttu-id="6b196-222">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6b196-222">String</span></span>|<span data-ttu-id="6b196-223">Einmaliges Anmelden Aussteller Hash.</span><span class="sxs-lookup"><span data-stu-id="6b196-223">Single sign-on issuer hash.</span></span>|
|<span data-ttu-id="6b196-224">eapXml</span><span class="sxs-lookup"><span data-stu-id="6b196-224">eapXml</span></span>|<span data-ttu-id="6b196-225">Binär</span><span class="sxs-lookup"><span data-stu-id="6b196-225">Binary</span></span>|<span data-ttu-id="6b196-226">Extensible Authentication-Protokoll (EAP) XML.</span><span class="sxs-lookup"><span data-stu-id="6b196-226">Extensible Authentication Protocol (EAP) XML.</span></span> <span data-ttu-id="6b196-227">(UTF8-codiertes Bytearray)</span><span class="sxs-lookup"><span data-stu-id="6b196-227">(UTF8 encoded byte array)</span></span>|
|<span data-ttu-id="6b196-228">proxyServer</span><span class="sxs-lookup"><span data-stu-id="6b196-228">proxyServer</span></span>|[<span data-ttu-id="6b196-229">windows10VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="6b196-229">windows10VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows10vpnproxyserver.md)|<span data-ttu-id="6b196-230">Proxy-Server.</span><span class="sxs-lookup"><span data-stu-id="6b196-230">Proxy Server.</span></span>|
|<span data-ttu-id="6b196-231">associatedApps</span><span class="sxs-lookup"><span data-stu-id="6b196-231">associatedApps</span></span>|<span data-ttu-id="6b196-232">[windows10AssociatedApps](../resources/intune-deviceconfig-windows10associatedapps.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="6b196-232">[windows10AssociatedApps](../resources/intune-deviceconfig-windows10associatedapps.md) collection</span></span>|<span data-ttu-id="6b196-233">Zugehörige Apps.</span><span class="sxs-lookup"><span data-stu-id="6b196-233">Associated Apps.</span></span> <span data-ttu-id="6b196-234">Diese Collection darf maximal 10.000 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="6b196-234">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="6b196-235">onlyAssociatedAppsCanUseConnection</span><span class="sxs-lookup"><span data-stu-id="6b196-235">onlyAssociatedAppsCanUseConnection</span></span>|<span data-ttu-id="6b196-236">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b196-236">Boolean</span></span>|<span data-ttu-id="6b196-237">Nur zugeordnete Apps können Verbindung (pro app VPN) verwenden.</span><span class="sxs-lookup"><span data-stu-id="6b196-237">Only associated Apps can use connection (per-app VPN).</span></span>|
|<span data-ttu-id="6b196-238">windowsInformationProtectionDomain</span><span class="sxs-lookup"><span data-stu-id="6b196-238">windowsInformationProtectionDomain</span></span>|<span data-ttu-id="6b196-239">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6b196-239">String</span></span>|<span data-ttu-id="6b196-240">Windows Informationen Schutz (WIP) Domäne, die diese Verbindung zugeordnet.</span><span class="sxs-lookup"><span data-stu-id="6b196-240">Windows Information Protection (WIP) domain to associate with this connection.</span></span>|
|<span data-ttu-id="6b196-241">trafficRules</span><span class="sxs-lookup"><span data-stu-id="6b196-241">trafficRules</span></span>|<span data-ttu-id="6b196-242">[VpnTrafficRule](../resources/intune-deviceconfig-vpntrafficrule.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="6b196-242">[vpnTrafficRule](../resources/intune-deviceconfig-vpntrafficrule.md) collection</span></span>|<span data-ttu-id="6b196-243">Datenverkehr Regeln.</span><span class="sxs-lookup"><span data-stu-id="6b196-243">Traffic rules.</span></span> <span data-ttu-id="6b196-244">Diese Sammlung kann bis zu 1000 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="6b196-244">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="6b196-245">Routen</span><span class="sxs-lookup"><span data-stu-id="6b196-245">routes</span></span>|<span data-ttu-id="6b196-246">[VpnRoute](../resources/intune-deviceconfig-vpnroute.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="6b196-246">[vpnRoute](../resources/intune-deviceconfig-vpnroute.md) collection</span></span>|<span data-ttu-id="6b196-247">Routen (optional für Drittanbieter-Anbieter).</span><span class="sxs-lookup"><span data-stu-id="6b196-247">Routes (optional for third-party providers).</span></span> <span data-ttu-id="6b196-248">Diese Sammlung kann bis zu 1000 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="6b196-248">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="6b196-249">dnsRules</span><span class="sxs-lookup"><span data-stu-id="6b196-249">dnsRules</span></span>|<span data-ttu-id="6b196-250">[VpnDnsRule](../resources/intune-deviceconfig-vpndnsrule.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="6b196-250">[vpnDnsRule](../resources/intune-deviceconfig-vpndnsrule.md) collection</span></span>|<span data-ttu-id="6b196-251">DNS-Regeln.</span><span class="sxs-lookup"><span data-stu-id="6b196-251">DNS rules.</span></span> <span data-ttu-id="6b196-252">Diese Sammlung kann bis zu 1000 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="6b196-252">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="6b196-253">trustedNetworkDomains</span><span class="sxs-lookup"><span data-stu-id="6b196-253">trustedNetworkDomains</span></span>|<span data-ttu-id="6b196-254">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="6b196-254">String collection</span></span>|<span data-ttu-id="6b196-255">Vertrauenswürdige Netzwerkdomänen</span><span class="sxs-lookup"><span data-stu-id="6b196-255">Trusted Network Domains</span></span>|



## <a name="response"></a><span data-ttu-id="6b196-256">Antwort</span><span class="sxs-lookup"><span data-stu-id="6b196-256">Response</span></span>
<span data-ttu-id="6b196-257">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="6b196-257">If successful, this method returns a `201 Created` response code and a [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6b196-258">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6b196-258">Example</span></span>

### <a name="request"></a><span data-ttu-id="6b196-259">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6b196-259">Request</span></span>
<span data-ttu-id="6b196-260">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6b196-260">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6b196-261">Antwort</span><span class="sxs-lookup"><span data-stu-id="6b196-261">Response</span></span>
<span data-ttu-id="6b196-p122">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6b196-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




