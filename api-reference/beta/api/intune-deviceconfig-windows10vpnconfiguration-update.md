---
title: Windows10VpnConfiguration aktualisieren
description: Aktualisieren Sie die Eigenschaften eines windows10VpnConfiguration-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d2d6a7fda3dc357d91fbb56b7bd3e01e76152cd8
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421606"
---
# <a name="update-windows10vpnconfiguration"></a><span data-ttu-id="4a6bf-103">Windows10VpnConfiguration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="4a6bf-103">Update windows10VpnConfiguration</span></span>

> <span data-ttu-id="4a6bf-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="4a6bf-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="4a6bf-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4a6bf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4a6bf-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="4a6bf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4a6bf-107">Aktualisieren Sie die Eigenschaften eines [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="4a6bf-107">Update the properties of a [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4a6bf-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="4a6bf-108">Prerequisites</span></span>
<span data-ttu-id="4a6bf-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="4a6bf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="4a6bf-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4a6bf-111">Permission type</span></span>|<span data-ttu-id="4a6bf-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4a6bf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4a6bf-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4a6bf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4a6bf-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a6bf-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4a6bf-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4a6bf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4a6bf-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4a6bf-116">Not supported.</span></span>|
|<span data-ttu-id="4a6bf-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4a6bf-117">Application</span></span>|<span data-ttu-id="4a6bf-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4a6bf-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4a6bf-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4a6bf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="4a6bf-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4a6bf-120">Request headers</span></span>
|<span data-ttu-id="4a6bf-121">Header</span><span class="sxs-lookup"><span data-stu-id="4a6bf-121">Header</span></span>|<span data-ttu-id="4a6bf-122">Wert</span><span class="sxs-lookup"><span data-stu-id="4a6bf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4a6bf-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="4a6bf-123">Authorization</span></span>|<span data-ttu-id="4a6bf-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="4a6bf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4a6bf-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="4a6bf-125">Accept</span></span>|<span data-ttu-id="4a6bf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4a6bf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4a6bf-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4a6bf-127">Request body</span></span>
<span data-ttu-id="4a6bf-128">Geben Sie im Textkörper Anforderung für das Objekt [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="4a6bf-128">In the request body, supply a JSON representation for the [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>

<span data-ttu-id="4a6bf-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="4a6bf-129">The following table shows the properties that are required when you create the [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md).</span></span>

|<span data-ttu-id="4a6bf-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4a6bf-130">Property</span></span>|<span data-ttu-id="4a6bf-131">Typ</span><span class="sxs-lookup"><span data-stu-id="4a6bf-131">Type</span></span>|<span data-ttu-id="4a6bf-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4a6bf-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4a6bf-133">id</span><span class="sxs-lookup"><span data-stu-id="4a6bf-133">id</span></span>|<span data-ttu-id="4a6bf-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4a6bf-134">String</span></span>|<span data-ttu-id="4a6bf-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="4a6bf-135">Key of the entity.</span></span> <span data-ttu-id="4a6bf-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4a6bf-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4a6bf-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4a6bf-137">lastModifiedDateTime</span></span>|<span data-ttu-id="4a6bf-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4a6bf-138">DateTimeOffset</span></span>|<span data-ttu-id="4a6bf-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="4a6bf-139">DateTime the object was last modified.</span></span> <span data-ttu-id="4a6bf-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4a6bf-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4a6bf-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4a6bf-141">roleScopeTagIds</span></span>|<span data-ttu-id="4a6bf-142">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="4a6bf-142">String collection</span></span>|<span data-ttu-id="4a6bf-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="4a6bf-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="4a6bf-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4a6bf-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4a6bf-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="4a6bf-145">supportsScopeTags</span></span>|<span data-ttu-id="4a6bf-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a6bf-146">Boolean</span></span>|<span data-ttu-id="4a6bf-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4a6bf-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="4a6bf-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="4a6bf-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="4a6bf-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="4a6bf-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="4a6bf-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="4a6bf-150">This property is read-only.</span></span> <span data-ttu-id="4a6bf-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4a6bf-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4a6bf-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4a6bf-152">createdDateTime</span></span>|<span data-ttu-id="4a6bf-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4a6bf-153">DateTimeOffset</span></span>|<span data-ttu-id="4a6bf-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="4a6bf-154">DateTime the object was created.</span></span> <span data-ttu-id="4a6bf-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4a6bf-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4a6bf-156">description</span><span class="sxs-lookup"><span data-stu-id="4a6bf-156">description</span></span>|<span data-ttu-id="4a6bf-157">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4a6bf-157">String</span></span>|<span data-ttu-id="4a6bf-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="4a6bf-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="4a6bf-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4a6bf-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4a6bf-160">displayName</span><span class="sxs-lookup"><span data-stu-id="4a6bf-160">displayName</span></span>|<span data-ttu-id="4a6bf-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4a6bf-161">String</span></span>|<span data-ttu-id="4a6bf-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="4a6bf-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="4a6bf-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4a6bf-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4a6bf-164">Version</span><span class="sxs-lookup"><span data-stu-id="4a6bf-164">version</span></span>|<span data-ttu-id="4a6bf-165">Int32</span><span class="sxs-lookup"><span data-stu-id="4a6bf-165">Int32</span></span>|<span data-ttu-id="4a6bf-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="4a6bf-166">Version of the device configuration.</span></span> <span data-ttu-id="4a6bf-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4a6bf-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4a6bf-168">connectionName</span><span class="sxs-lookup"><span data-stu-id="4a6bf-168">connectionName</span></span>|<span data-ttu-id="4a6bf-169">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4a6bf-169">String</span></span>|<span data-ttu-id="4a6bf-170">Name der Verbindung für den Benutzer angezeigt.</span><span class="sxs-lookup"><span data-stu-id="4a6bf-170">Connection name displayed to the user.</span></span> <span data-ttu-id="4a6bf-171">Geerbt von [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4a6bf-171">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="4a6bf-172">Server</span><span class="sxs-lookup"><span data-stu-id="4a6bf-172">servers</span></span>|<span data-ttu-id="4a6bf-173">[VpnServer](../resources/intune-deviceconfig-vpnserver.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="4a6bf-173">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="4a6bf-174">Liste der VPN-Server im Netzwerk.</span><span class="sxs-lookup"><span data-stu-id="4a6bf-174">List of VPN Servers on the network.</span></span> <span data-ttu-id="4a6bf-175">Stellen Sie sicher, dass Endbenutzer diese Netzwerkadressen zugreifen können.</span><span class="sxs-lookup"><span data-stu-id="4a6bf-175">Make sure end users can access these network locations.</span></span> <span data-ttu-id="4a6bf-176">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="4a6bf-176">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="4a6bf-177">Geerbt von [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4a6bf-177">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="4a6bf-178">customXml</span><span class="sxs-lookup"><span data-stu-id="4a6bf-178">customXml</span></span>|<span data-ttu-id="4a6bf-179">Binär</span><span class="sxs-lookup"><span data-stu-id="4a6bf-179">Binary</span></span>|<span data-ttu-id="4a6bf-180">Benutzerdefinierte XML-Befehle, die die VPN-Verbindung konfiguriert.</span><span class="sxs-lookup"><span data-stu-id="4a6bf-180">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="4a6bf-181">(UTF8 codiert Bytearray) Geerbt von [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4a6bf-181">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="4a6bf-182">profileTarget</span><span class="sxs-lookup"><span data-stu-id="4a6bf-182">profileTarget</span></span>|[<span data-ttu-id="4a6bf-183">windows10VpnProfileTarget</span><span class="sxs-lookup"><span data-stu-id="4a6bf-183">windows10VpnProfileTarget</span></span>](../resources/intune-deviceconfig-windows10vpnprofiletarget.md)|<span data-ttu-id="4a6bf-184">Profil Zieltyp.</span><span class="sxs-lookup"><span data-stu-id="4a6bf-184">Profile target type.</span></span> <span data-ttu-id="4a6bf-185">Mögliche Werte sind: `user`, `device` und `autoPilotDevice`.</span><span class="sxs-lookup"><span data-stu-id="4a6bf-185">Possible values are: `user`, `device`, `autoPilotDevice`.</span></span>|
|<span data-ttu-id="4a6bf-186">connectionType</span><span class="sxs-lookup"><span data-stu-id="4a6bf-186">connectionType</span></span>|[<span data-ttu-id="4a6bf-187">windows10VpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="4a6bf-187">windows10VpnConnectionType</span></span>](../resources/intune-deviceconfig-windows10vpnconnectiontype.md)|<span data-ttu-id="4a6bf-188">Verbindungstyp.</span><span class="sxs-lookup"><span data-stu-id="4a6bf-188">Connection type.</span></span> <span data-ttu-id="4a6bf-189">Mögliche Werte: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `automatic`, `ikEv2`, `l2tp`, `pptp`, `citrix`, `paloAltoGlobalProtect`.</span><span class="sxs-lookup"><span data-stu-id="4a6bf-189">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `automatic`, `ikEv2`, `l2tp`, `pptp`, `citrix`, `paloAltoGlobalProtect`.</span></span>|
|<span data-ttu-id="4a6bf-190">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="4a6bf-190">enableSplitTunneling</span></span>|<span data-ttu-id="4a6bf-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a6bf-191">Boolean</span></span>|<span data-ttu-id="4a6bf-192">Split-tunneling zu aktivieren.</span><span class="sxs-lookup"><span data-stu-id="4a6bf-192">Enable split tunneling.</span></span>|
|<span data-ttu-id="4a6bf-193">enableAlwaysOn</span><span class="sxs-lookup"><span data-stu-id="4a6bf-193">enableAlwaysOn</span></span>|<span data-ttu-id="4a6bf-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a6bf-194">Boolean</span></span>|<span data-ttu-id="4a6bf-195">Aktivieren Sie Always On-Modus.</span><span class="sxs-lookup"><span data-stu-id="4a6bf-195">Enable Always On mode.</span></span>|
|<span data-ttu-id="4a6bf-196">enableDeviceTunnel</span><span class="sxs-lookup"><span data-stu-id="4a6bf-196">enableDeviceTunnel</span></span>|<span data-ttu-id="4a6bf-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a6bf-197">Boolean</span></span>|<span data-ttu-id="4a6bf-198">Aktivieren Sie Gerät Tunnel.</span><span class="sxs-lookup"><span data-stu-id="4a6bf-198">Enable device tunnel.</span></span>|
|<span data-ttu-id="4a6bf-199">enableDnsRegistration</span><span class="sxs-lookup"><span data-stu-id="4a6bf-199">enableDnsRegistration</span></span>|<span data-ttu-id="4a6bf-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a6bf-200">Boolean</span></span>|<span data-ttu-id="4a6bf-201">Aktivieren Sie die IP-Adressregistrierung mit internen DNS.</span><span class="sxs-lookup"><span data-stu-id="4a6bf-201">Enable IP address registration with internal DNS.</span></span>|
|<span data-ttu-id="4a6bf-202">dnsSuffixes</span><span class="sxs-lookup"><span data-stu-id="4a6bf-202">dnsSuffixes</span></span>|<span data-ttu-id="4a6bf-203">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="4a6bf-203">String collection</span></span>|<span data-ttu-id="4a6bf-204">Geben Sie die DNS-Suffixe hinzufügen zu DNS-Suchliste Kurznamen ordnungsgemäß weitergeleitet.</span><span class="sxs-lookup"><span data-stu-id="4a6bf-204">Specify DNS suffixes to add to the DNS search list to properly route short names.</span></span>|
|<span data-ttu-id="4a6bf-205">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="4a6bf-205">authenticationMethod</span></span>|[<span data-ttu-id="4a6bf-206">windows10VpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="4a6bf-206">windows10VpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-windows10vpnauthenticationmethod.md)|<span data-ttu-id="4a6bf-207">Authentifizierungsmethode.</span><span class="sxs-lookup"><span data-stu-id="4a6bf-207">Authentication method.</span></span> <span data-ttu-id="4a6bf-208">Mögliche Werte sind: `certificate`, `usernameAndPassword` und `customEapXml`.</span><span class="sxs-lookup"><span data-stu-id="4a6bf-208">Possible values are: `certificate`, `usernameAndPassword`, `customEapXml`.</span></span>|
|<span data-ttu-id="4a6bf-209">rememberUserCredentials</span><span class="sxs-lookup"><span data-stu-id="4a6bf-209">rememberUserCredentials</span></span>|<span data-ttu-id="4a6bf-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a6bf-210">Boolean</span></span>|<span data-ttu-id="4a6bf-211">Beachten Sie die Anmeldeinformationen des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="4a6bf-211">Remember user credentials.</span></span>|
|<span data-ttu-id="4a6bf-212">enableConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="4a6bf-212">enableConditionalAccess</span></span>|<span data-ttu-id="4a6bf-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a6bf-213">Boolean</span></span>|<span data-ttu-id="4a6bf-214">Aktivieren Sie bedingte Zugriff.</span><span class="sxs-lookup"><span data-stu-id="4a6bf-214">Enable conditional access.</span></span>|
|<span data-ttu-id="4a6bf-215">enableSingleSignOnWithAlternateCertificate</span><span class="sxs-lookup"><span data-stu-id="4a6bf-215">enableSingleSignOnWithAlternateCertificate</span></span>|<span data-ttu-id="4a6bf-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a6bf-216">Boolean</span></span>|<span data-ttu-id="4a6bf-217">Aktivieren Sie einmaliges Anmelden (SSO) mit anderen Zertifikats.</span><span class="sxs-lookup"><span data-stu-id="4a6bf-217">Enable single sign-on (SSO) with alternate certificate.</span></span>|
|<span data-ttu-id="4a6bf-218">singleSignOnEku</span><span class="sxs-lookup"><span data-stu-id="4a6bf-218">singleSignOnEku</span></span>|[<span data-ttu-id="4a6bf-219">extendedKeyUsage</span><span class="sxs-lookup"><span data-stu-id="4a6bf-219">extendedKeyUsage</span></span>](../resources/intune-deviceconfig-extendedkeyusage.md)|<span data-ttu-id="4a6bf-220">Einmaliges Anmelden erweiterte Schlüsselverwendung (EKU).</span><span class="sxs-lookup"><span data-stu-id="4a6bf-220">Single sign-on Extended Key Usage (EKU).</span></span>|
|<span data-ttu-id="4a6bf-221">singleSignOnIssuerHash</span><span class="sxs-lookup"><span data-stu-id="4a6bf-221">singleSignOnIssuerHash</span></span>|<span data-ttu-id="4a6bf-222">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4a6bf-222">String</span></span>|<span data-ttu-id="4a6bf-223">Einmaliges Anmelden Aussteller Hash.</span><span class="sxs-lookup"><span data-stu-id="4a6bf-223">Single sign-on issuer hash.</span></span>|
|<span data-ttu-id="4a6bf-224">eapXml</span><span class="sxs-lookup"><span data-stu-id="4a6bf-224">eapXml</span></span>|<span data-ttu-id="4a6bf-225">Binär</span><span class="sxs-lookup"><span data-stu-id="4a6bf-225">Binary</span></span>|<span data-ttu-id="4a6bf-226">Extensible Authentication-Protokoll (EAP) XML.</span><span class="sxs-lookup"><span data-stu-id="4a6bf-226">Extensible Authentication Protocol (EAP) XML.</span></span> <span data-ttu-id="4a6bf-227">(UTF8-codiertes Bytearray)</span><span class="sxs-lookup"><span data-stu-id="4a6bf-227">(UTF8 encoded byte array)</span></span>|
|<span data-ttu-id="4a6bf-228">proxyServer</span><span class="sxs-lookup"><span data-stu-id="4a6bf-228">proxyServer</span></span>|[<span data-ttu-id="4a6bf-229">windows10VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="4a6bf-229">windows10VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows10vpnproxyserver.md)|<span data-ttu-id="4a6bf-230">Proxy-Server.</span><span class="sxs-lookup"><span data-stu-id="4a6bf-230">Proxy Server.</span></span>|
|<span data-ttu-id="4a6bf-231">associatedApps</span><span class="sxs-lookup"><span data-stu-id="4a6bf-231">associatedApps</span></span>|<span data-ttu-id="4a6bf-232">[windows10AssociatedApps](../resources/intune-deviceconfig-windows10associatedapps.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="4a6bf-232">[windows10AssociatedApps](../resources/intune-deviceconfig-windows10associatedapps.md) collection</span></span>|<span data-ttu-id="4a6bf-233">Zugehörige Apps.</span><span class="sxs-lookup"><span data-stu-id="4a6bf-233">Associated Apps.</span></span> <span data-ttu-id="4a6bf-234">Diese Collection darf maximal 10.000 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="4a6bf-234">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="4a6bf-235">onlyAssociatedAppsCanUseConnection</span><span class="sxs-lookup"><span data-stu-id="4a6bf-235">onlyAssociatedAppsCanUseConnection</span></span>|<span data-ttu-id="4a6bf-236">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a6bf-236">Boolean</span></span>|<span data-ttu-id="4a6bf-237">Nur zugeordnete Apps können Verbindung (pro app VPN) verwenden.</span><span class="sxs-lookup"><span data-stu-id="4a6bf-237">Only associated Apps can use connection (per-app VPN).</span></span>|
|<span data-ttu-id="4a6bf-238">windowsInformationProtectionDomain</span><span class="sxs-lookup"><span data-stu-id="4a6bf-238">windowsInformationProtectionDomain</span></span>|<span data-ttu-id="4a6bf-239">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4a6bf-239">String</span></span>|<span data-ttu-id="4a6bf-240">Windows Informationen Schutz (WIP) Domäne, die diese Verbindung zugeordnet.</span><span class="sxs-lookup"><span data-stu-id="4a6bf-240">Windows Information Protection (WIP) domain to associate with this connection.</span></span>|
|<span data-ttu-id="4a6bf-241">trafficRules</span><span class="sxs-lookup"><span data-stu-id="4a6bf-241">trafficRules</span></span>|<span data-ttu-id="4a6bf-242">[VpnTrafficRule](../resources/intune-deviceconfig-vpntrafficrule.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="4a6bf-242">[vpnTrafficRule](../resources/intune-deviceconfig-vpntrafficrule.md) collection</span></span>|<span data-ttu-id="4a6bf-243">Datenverkehr Regeln.</span><span class="sxs-lookup"><span data-stu-id="4a6bf-243">Traffic rules.</span></span> <span data-ttu-id="4a6bf-244">Diese Sammlung kann bis zu 1000 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="4a6bf-244">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="4a6bf-245">Routen</span><span class="sxs-lookup"><span data-stu-id="4a6bf-245">routes</span></span>|<span data-ttu-id="4a6bf-246">[VpnRoute](../resources/intune-deviceconfig-vpnroute.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="4a6bf-246">[vpnRoute](../resources/intune-deviceconfig-vpnroute.md) collection</span></span>|<span data-ttu-id="4a6bf-247">Routen (optional für Drittanbieter-Anbieter).</span><span class="sxs-lookup"><span data-stu-id="4a6bf-247">Routes (optional for third-party providers).</span></span> <span data-ttu-id="4a6bf-248">Diese Sammlung kann bis zu 1000 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="4a6bf-248">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="4a6bf-249">dnsRules</span><span class="sxs-lookup"><span data-stu-id="4a6bf-249">dnsRules</span></span>|<span data-ttu-id="4a6bf-250">[VpnDnsRule](../resources/intune-deviceconfig-vpndnsrule.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="4a6bf-250">[vpnDnsRule](../resources/intune-deviceconfig-vpndnsrule.md) collection</span></span>|<span data-ttu-id="4a6bf-251">DNS-Regeln.</span><span class="sxs-lookup"><span data-stu-id="4a6bf-251">DNS rules.</span></span> <span data-ttu-id="4a6bf-252">Diese Sammlung kann bis zu 1000 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="4a6bf-252">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="4a6bf-253">trustedNetworkDomains</span><span class="sxs-lookup"><span data-stu-id="4a6bf-253">trustedNetworkDomains</span></span>|<span data-ttu-id="4a6bf-254">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="4a6bf-254">String collection</span></span>|<span data-ttu-id="4a6bf-255">Vertrauenswürdige Netzwerkdomänen</span><span class="sxs-lookup"><span data-stu-id="4a6bf-255">Trusted Network Domains</span></span>|



## <a name="response"></a><span data-ttu-id="4a6bf-256">Antwort</span><span class="sxs-lookup"><span data-stu-id="4a6bf-256">Response</span></span>
<span data-ttu-id="4a6bf-257">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="4a6bf-257">If successful, this method returns a `200 OK` response code and an updated [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4a6bf-258">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4a6bf-258">Example</span></span>

### <a name="request"></a><span data-ttu-id="4a6bf-259">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4a6bf-259">Request</span></span>
<span data-ttu-id="4a6bf-260">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4a6bf-260">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="4a6bf-261">Antwort</span><span class="sxs-lookup"><span data-stu-id="4a6bf-261">Response</span></span>
<span data-ttu-id="4a6bf-p122">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4a6bf-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




