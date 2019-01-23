---
title: Erstellen von windowsPhone81VpnConfiguration
description: Erstellen eines neuen windowsPhone81VpnConfiguration-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 0079291ca4c22b0ee4cd04f42f63b8bd0287d87c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29414571"
---
# <a name="create-windowsphone81vpnconfiguration"></a><span data-ttu-id="b54c1-103">Erstellen von windowsPhone81VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="b54c1-103">Create windowsPhone81VpnConfiguration</span></span>

> <span data-ttu-id="b54c1-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="b54c1-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b54c1-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b54c1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b54c1-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b54c1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b54c1-107">Erstellen eines neuen [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="b54c1-107">Create a new [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b54c1-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b54c1-108">Prerequisites</span></span>
<span data-ttu-id="b54c1-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="b54c1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b54c1-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b54c1-111">Permission type</span></span>|<span data-ttu-id="b54c1-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b54c1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b54c1-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b54c1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b54c1-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b54c1-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b54c1-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b54c1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b54c1-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b54c1-116">Not supported.</span></span>|
|<span data-ttu-id="b54c1-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b54c1-117">Application</span></span>|<span data-ttu-id="b54c1-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b54c1-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b54c1-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b54c1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="b54c1-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b54c1-120">Request headers</span></span>
|<span data-ttu-id="b54c1-121">Header</span><span class="sxs-lookup"><span data-stu-id="b54c1-121">Header</span></span>|<span data-ttu-id="b54c1-122">Wert</span><span class="sxs-lookup"><span data-stu-id="b54c1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b54c1-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="b54c1-123">Authorization</span></span>|<span data-ttu-id="b54c1-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b54c1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b54c1-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="b54c1-125">Accept</span></span>|<span data-ttu-id="b54c1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b54c1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b54c1-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b54c1-127">Request body</span></span>
<span data-ttu-id="b54c1-128">Geben Sie im Textkörper Anforderung für das Objekt windowsPhone81VpnConfiguration eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="b54c1-128">In the request body, supply a JSON representation for the windowsPhone81VpnConfiguration object.</span></span>

<span data-ttu-id="b54c1-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die windowsPhone81VpnConfiguration erstellen.</span><span class="sxs-lookup"><span data-stu-id="b54c1-129">The following table shows the properties that are required when you create the windowsPhone81VpnConfiguration.</span></span>

|<span data-ttu-id="b54c1-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b54c1-130">Property</span></span>|<span data-ttu-id="b54c1-131">Typ</span><span class="sxs-lookup"><span data-stu-id="b54c1-131">Type</span></span>|<span data-ttu-id="b54c1-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b54c1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b54c1-133">id</span><span class="sxs-lookup"><span data-stu-id="b54c1-133">id</span></span>|<span data-ttu-id="b54c1-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b54c1-134">String</span></span>|<span data-ttu-id="b54c1-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="b54c1-135">Key of the entity.</span></span> <span data-ttu-id="b54c1-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b54c1-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b54c1-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b54c1-137">lastModifiedDateTime</span></span>|<span data-ttu-id="b54c1-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b54c1-138">DateTimeOffset</span></span>|<span data-ttu-id="b54c1-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="b54c1-139">DateTime the object was last modified.</span></span> <span data-ttu-id="b54c1-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b54c1-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b54c1-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b54c1-141">roleScopeTagIds</span></span>|<span data-ttu-id="b54c1-142">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="b54c1-142">String collection</span></span>|<span data-ttu-id="b54c1-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="b54c1-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b54c1-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b54c1-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b54c1-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="b54c1-145">supportsScopeTags</span></span>|<span data-ttu-id="b54c1-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="b54c1-146">Boolean</span></span>|<span data-ttu-id="b54c1-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b54c1-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="b54c1-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="b54c1-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="b54c1-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="b54c1-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="b54c1-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="b54c1-150">This property is read-only.</span></span> <span data-ttu-id="b54c1-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b54c1-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b54c1-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b54c1-152">createdDateTime</span></span>|<span data-ttu-id="b54c1-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b54c1-153">DateTimeOffset</span></span>|<span data-ttu-id="b54c1-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="b54c1-154">DateTime the object was created.</span></span> <span data-ttu-id="b54c1-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b54c1-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b54c1-156">description</span><span class="sxs-lookup"><span data-stu-id="b54c1-156">description</span></span>|<span data-ttu-id="b54c1-157">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b54c1-157">String</span></span>|<span data-ttu-id="b54c1-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="b54c1-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b54c1-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b54c1-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b54c1-160">displayName</span><span class="sxs-lookup"><span data-stu-id="b54c1-160">displayName</span></span>|<span data-ttu-id="b54c1-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b54c1-161">String</span></span>|<span data-ttu-id="b54c1-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="b54c1-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b54c1-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b54c1-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b54c1-164">Version</span><span class="sxs-lookup"><span data-stu-id="b54c1-164">version</span></span>|<span data-ttu-id="b54c1-165">Int32</span><span class="sxs-lookup"><span data-stu-id="b54c1-165">Int32</span></span>|<span data-ttu-id="b54c1-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="b54c1-166">Version of the device configuration.</span></span> <span data-ttu-id="b54c1-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b54c1-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b54c1-168">connectionName</span><span class="sxs-lookup"><span data-stu-id="b54c1-168">connectionName</span></span>|<span data-ttu-id="b54c1-169">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b54c1-169">String</span></span>|<span data-ttu-id="b54c1-170">Name der Verbindung für den Benutzer angezeigt.</span><span class="sxs-lookup"><span data-stu-id="b54c1-170">Connection name displayed to the user.</span></span> <span data-ttu-id="b54c1-171">Geerbt von [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b54c1-171">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="b54c1-172">Server</span><span class="sxs-lookup"><span data-stu-id="b54c1-172">servers</span></span>|<span data-ttu-id="b54c1-173">[VpnServer](../resources/intune-deviceconfig-vpnserver.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="b54c1-173">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="b54c1-174">Liste der VPN-Server im Netzwerk.</span><span class="sxs-lookup"><span data-stu-id="b54c1-174">List of VPN Servers on the network.</span></span> <span data-ttu-id="b54c1-175">Stellen Sie sicher, dass Endbenutzer diese Netzwerkadressen zugreifen können.</span><span class="sxs-lookup"><span data-stu-id="b54c1-175">Make sure end users can access these network locations.</span></span> <span data-ttu-id="b54c1-176">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="b54c1-176">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="b54c1-177">Geerbt von [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b54c1-177">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="b54c1-178">customXml</span><span class="sxs-lookup"><span data-stu-id="b54c1-178">customXml</span></span>|<span data-ttu-id="b54c1-179">Binär</span><span class="sxs-lookup"><span data-stu-id="b54c1-179">Binary</span></span>|<span data-ttu-id="b54c1-180">Benutzerdefinierte XML-Befehle, die die VPN-Verbindung konfiguriert.</span><span class="sxs-lookup"><span data-stu-id="b54c1-180">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="b54c1-181">(UTF8 codiert Bytearray) Geerbt von [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b54c1-181">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="b54c1-182">applyOnlyToWindows81</span><span class="sxs-lookup"><span data-stu-id="b54c1-182">applyOnlyToWindows81</span></span>|<span data-ttu-id="b54c1-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="b54c1-183">Boolean</span></span>|<span data-ttu-id="b54c1-184">Wert, der angibt, ob die Richtlinie nur für Windows 8.1 gilt.</span><span class="sxs-lookup"><span data-stu-id="b54c1-184">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="b54c1-185">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="b54c1-185">This property is read-only.</span></span> <span data-ttu-id="b54c1-186">Geerbt von [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b54c1-186">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="b54c1-187">connectionType</span><span class="sxs-lookup"><span data-stu-id="b54c1-187">connectionType</span></span>|[<span data-ttu-id="b54c1-188">windowsVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="b54c1-188">windowsVpnConnectionType</span></span>](../resources/intune-deviceconfig-windowsvpnconnectiontype.md)|<span data-ttu-id="b54c1-189">Verbindungstyp.</span><span class="sxs-lookup"><span data-stu-id="b54c1-189">Connection type.</span></span> <span data-ttu-id="b54c1-190">Geerbt von [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b54c1-190">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md).</span></span> <span data-ttu-id="b54c1-191">Mögliche Werte: sind `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect` und `checkPointCapsuleVpn`.</span><span class="sxs-lookup"><span data-stu-id="b54c1-191">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`.</span></span>|
|<span data-ttu-id="b54c1-192">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="b54c1-192">loginGroupOrDomain</span></span>|<span data-ttu-id="b54c1-193">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b54c1-193">String</span></span>|<span data-ttu-id="b54c1-194">Anmeldegruppe oder Domäne Wenn Verbindungstyp auf Dell SonicWALL Mobile Verbindung festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="b54c1-194">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="b54c1-195">Geerbt von [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b54c1-195">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="b54c1-196">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="b54c1-196">enableSplitTunneling</span></span>|<span data-ttu-id="b54c1-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="b54c1-197">Boolean</span></span>|<span data-ttu-id="b54c1-198">Aktivieren Sie die Split-tunneling für das VPN.</span><span class="sxs-lookup"><span data-stu-id="b54c1-198">Enable split tunneling for the VPN.</span></span> <span data-ttu-id="b54c1-199">Geerbt von [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b54c1-199">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="b54c1-200">proxyServer</span><span class="sxs-lookup"><span data-stu-id="b54c1-200">proxyServer</span></span>|[<span data-ttu-id="b54c1-201">windows81VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="b54c1-201">windows81VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows81vpnproxyserver.md)|<span data-ttu-id="b54c1-202">Proxy-Server.</span><span class="sxs-lookup"><span data-stu-id="b54c1-202">Proxy Server.</span></span> <span data-ttu-id="b54c1-203">Geerbt von [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b54c1-203">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="b54c1-204">bypassVpnOnCompanyWifi</span><span class="sxs-lookup"><span data-stu-id="b54c1-204">bypassVpnOnCompanyWifi</span></span>|<span data-ttu-id="b54c1-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="b54c1-205">Boolean</span></span>|<span data-ttu-id="b54c1-206">Umgehung VPN auf Unternehmen Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="b54c1-206">Bypass VPN on company Wi-Fi.</span></span>|
|<span data-ttu-id="b54c1-207">bypassVpnOnHomeWifi</span><span class="sxs-lookup"><span data-stu-id="b54c1-207">bypassVpnOnHomeWifi</span></span>|<span data-ttu-id="b54c1-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="b54c1-208">Boolean</span></span>|<span data-ttu-id="b54c1-209">Umgehung VPN auf private Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="b54c1-209">Bypass VPN on home Wi-Fi.</span></span>|
|<span data-ttu-id="b54c1-210">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="b54c1-210">authenticationMethod</span></span>|[<span data-ttu-id="b54c1-211">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="b54c1-211">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="b54c1-212">Authentifizierungsmethode.</span><span class="sxs-lookup"><span data-stu-id="b54c1-212">Authentication method.</span></span> <span data-ttu-id="b54c1-213">Mögliche Werte sind: `certificate` und `usernameAndPassword`.</span><span class="sxs-lookup"><span data-stu-id="b54c1-213">Possible values are: `certificate`, `usernameAndPassword`.</span></span>|
|<span data-ttu-id="b54c1-214">rememberUserCredentials</span><span class="sxs-lookup"><span data-stu-id="b54c1-214">rememberUserCredentials</span></span>|<span data-ttu-id="b54c1-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="b54c1-215">Boolean</span></span>|<span data-ttu-id="b54c1-216">Beachten Sie die Anmeldeinformationen des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="b54c1-216">Remember user credentials.</span></span>|
|<span data-ttu-id="b54c1-217">dnsSuffixSearchList</span><span class="sxs-lookup"><span data-stu-id="b54c1-217">dnsSuffixSearchList</span></span>|<span data-ttu-id="b54c1-218">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="b54c1-218">String collection</span></span>|<span data-ttu-id="b54c1-219">DNS-Suffixsuchliste.</span><span class="sxs-lookup"><span data-stu-id="b54c1-219">DNS suffix search list.</span></span>|



## <a name="response"></a><span data-ttu-id="b54c1-220">Antwort</span><span class="sxs-lookup"><span data-stu-id="b54c1-220">Response</span></span>
<span data-ttu-id="b54c1-221">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="b54c1-221">If successful, this method returns a `201 Created` response code and a [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b54c1-222">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b54c1-222">Example</span></span>

### <a name="request"></a><span data-ttu-id="b54c1-223">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b54c1-223">Request</span></span>
<span data-ttu-id="b54c1-224">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b54c1-224">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b54c1-225">Antwort</span><span class="sxs-lookup"><span data-stu-id="b54c1-225">Response</span></span>
<span data-ttu-id="b54c1-p120">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b54c1-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




