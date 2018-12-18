---
title: MacOSVpnConfiguration aktualisieren
description: Aktualisieren Sie die Eigenschaften eines MacOSVpnConfiguration-Objekts.
author: tfitzmac
ms.openlocfilehash: fc28d344f29ba6a5dfe32ea67d2d3f45fb757bfa
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27330884"
---
# <a name="update-macosvpnconfiguration"></a><span data-ttu-id="b40cc-103">MacOSVpnConfiguration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="b40cc-103">Update macOSVpnConfiguration</span></span>

> <span data-ttu-id="b40cc-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b40cc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b40cc-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b40cc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b40cc-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="b40cc-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b40cc-107">Aktualisieren Sie die Eigenschaften eines [MacOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="b40cc-107">Update the properties of a [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b40cc-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b40cc-108">Prerequisites</span></span>
<span data-ttu-id="b40cc-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b40cc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b40cc-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b40cc-111">Permission type</span></span>|<span data-ttu-id="b40cc-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b40cc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b40cc-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b40cc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b40cc-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b40cc-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b40cc-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b40cc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b40cc-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b40cc-116">Not supported.</span></span>|
|<span data-ttu-id="b40cc-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b40cc-117">Application</span></span>|<span data-ttu-id="b40cc-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b40cc-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b40cc-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b40cc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="b40cc-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b40cc-120">Request headers</span></span>
|<span data-ttu-id="b40cc-121">Header</span><span class="sxs-lookup"><span data-stu-id="b40cc-121">Header</span></span>|<span data-ttu-id="b40cc-122">Wert</span><span class="sxs-lookup"><span data-stu-id="b40cc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b40cc-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="b40cc-123">Authorization</span></span>|<span data-ttu-id="b40cc-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b40cc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b40cc-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b40cc-125">Accept</span></span>|<span data-ttu-id="b40cc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b40cc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b40cc-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b40cc-127">Request body</span></span>
<span data-ttu-id="b40cc-128">Geben Sie im Textkörper Anforderung für das Objekt [MacOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="b40cc-128">In the request body, supply a JSON representation for the [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) object.</span></span>

<span data-ttu-id="b40cc-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [MacOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="b40cc-129">The following table shows the properties that are required when you create the [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md).</span></span>

|<span data-ttu-id="b40cc-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b40cc-130">Property</span></span>|<span data-ttu-id="b40cc-131">Typ</span><span class="sxs-lookup"><span data-stu-id="b40cc-131">Type</span></span>|<span data-ttu-id="b40cc-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b40cc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b40cc-133">id</span><span class="sxs-lookup"><span data-stu-id="b40cc-133">id</span></span>|<span data-ttu-id="b40cc-134">String</span><span class="sxs-lookup"><span data-stu-id="b40cc-134">String</span></span>|<span data-ttu-id="b40cc-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="b40cc-135">Key of the entity.</span></span> <span data-ttu-id="b40cc-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b40cc-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b40cc-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b40cc-137">lastModifiedDateTime</span></span>|<span data-ttu-id="b40cc-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b40cc-138">DateTimeOffset</span></span>|<span data-ttu-id="b40cc-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="b40cc-139">DateTime the object was last modified.</span></span> <span data-ttu-id="b40cc-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b40cc-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b40cc-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b40cc-141">roleScopeTagIds</span></span>|<span data-ttu-id="b40cc-142">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="b40cc-142">String collection</span></span>|<span data-ttu-id="b40cc-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="b40cc-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b40cc-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b40cc-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b40cc-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="b40cc-145">supportsScopeTags</span></span>|<span data-ttu-id="b40cc-146">Boolesch</span><span class="sxs-lookup"><span data-stu-id="b40cc-146">Boolean</span></span>|<span data-ttu-id="b40cc-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b40cc-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="b40cc-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="b40cc-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="b40cc-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="b40cc-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="b40cc-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="b40cc-150">This property is read-only.</span></span> <span data-ttu-id="b40cc-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b40cc-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b40cc-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b40cc-152">createdDateTime</span></span>|<span data-ttu-id="b40cc-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b40cc-153">DateTimeOffset</span></span>|<span data-ttu-id="b40cc-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="b40cc-154">DateTime the object was created.</span></span> <span data-ttu-id="b40cc-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b40cc-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b40cc-156">description</span><span class="sxs-lookup"><span data-stu-id="b40cc-156">description</span></span>|<span data-ttu-id="b40cc-157">String</span><span class="sxs-lookup"><span data-stu-id="b40cc-157">String</span></span>|<span data-ttu-id="b40cc-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="b40cc-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b40cc-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b40cc-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b40cc-160">displayName</span><span class="sxs-lookup"><span data-stu-id="b40cc-160">displayName</span></span>|<span data-ttu-id="b40cc-161">String</span><span class="sxs-lookup"><span data-stu-id="b40cc-161">String</span></span>|<span data-ttu-id="b40cc-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="b40cc-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b40cc-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b40cc-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b40cc-164">Version</span><span class="sxs-lookup"><span data-stu-id="b40cc-164">version</span></span>|<span data-ttu-id="b40cc-165">Int32</span><span class="sxs-lookup"><span data-stu-id="b40cc-165">Int32</span></span>|<span data-ttu-id="b40cc-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="b40cc-166">Version of the device configuration.</span></span> <span data-ttu-id="b40cc-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b40cc-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b40cc-168">connectionName</span><span class="sxs-lookup"><span data-stu-id="b40cc-168">connectionName</span></span>|<span data-ttu-id="b40cc-169">String</span><span class="sxs-lookup"><span data-stu-id="b40cc-169">String</span></span>|<span data-ttu-id="b40cc-170">Name der Verbindung für den Benutzer angezeigt.</span><span class="sxs-lookup"><span data-stu-id="b40cc-170">Connection name displayed to the user.</span></span> <span data-ttu-id="b40cc-171">Geerbt von [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b40cc-171">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="b40cc-172">connectionType</span><span class="sxs-lookup"><span data-stu-id="b40cc-172">connectionType</span></span>|[<span data-ttu-id="b40cc-173">appleVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="b40cc-173">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="b40cc-174">Verbindungstyp.</span><span class="sxs-lookup"><span data-stu-id="b40cc-174">Connection type.</span></span> <span data-ttu-id="b40cc-175">Geerbt von [AppleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b40cc-175">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="b40cc-176">Mögliche Werte sind: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`.</span><span class="sxs-lookup"><span data-stu-id="b40cc-176">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`.</span></span>|
|<span data-ttu-id="b40cc-177">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="b40cc-177">loginGroupOrDomain</span></span>|<span data-ttu-id="b40cc-178">String</span><span class="sxs-lookup"><span data-stu-id="b40cc-178">String</span></span>|<span data-ttu-id="b40cc-179">Anmeldegruppe oder Domäne Wenn Verbindungstyp auf Dell SonicWALL Mobile Verbindung festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="b40cc-179">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="b40cc-180">Geerbt von [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b40cc-180">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="b40cc-181">role</span><span class="sxs-lookup"><span data-stu-id="b40cc-181">role</span></span>|<span data-ttu-id="b40cc-182">String</span><span class="sxs-lookup"><span data-stu-id="b40cc-182">String</span></span>|<span data-ttu-id="b40cc-183">Rolle, wenn Verbindungstyp auf Pulse Secure festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="b40cc-183">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="b40cc-184">Geerbt von [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b40cc-184">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="b40cc-185">Bereich</span><span class="sxs-lookup"><span data-stu-id="b40cc-185">realm</span></span>|<span data-ttu-id="b40cc-186">String</span><span class="sxs-lookup"><span data-stu-id="b40cc-186">String</span></span>|<span data-ttu-id="b40cc-187">Realm Wenn Verbindungstyp auf Pulse Secure festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="b40cc-187">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="b40cc-188">Geerbt von [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b40cc-188">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="b40cc-189">Server</span><span class="sxs-lookup"><span data-stu-id="b40cc-189">server</span></span>|[<span data-ttu-id="b40cc-190">vpnServer</span><span class="sxs-lookup"><span data-stu-id="b40cc-190">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="b40cc-191">VPN-Server im Netzwerk.</span><span class="sxs-lookup"><span data-stu-id="b40cc-191">VPN Server on the network.</span></span> <span data-ttu-id="b40cc-192">Stellen Sie sicher, dass Endbenutzer dieser Speicherort im Netzwerk zugreifen können.</span><span class="sxs-lookup"><span data-stu-id="b40cc-192">Make sure end users can access this network location.</span></span> <span data-ttu-id="b40cc-193">Geerbt von [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b40cc-193">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="b40cc-194">Bezeichner</span><span class="sxs-lookup"><span data-stu-id="b40cc-194">identifier</span></span>|<span data-ttu-id="b40cc-195">String</span><span class="sxs-lookup"><span data-stu-id="b40cc-195">String</span></span>|<span data-ttu-id="b40cc-196">Bezeichner von VPN-Anbieter bereitgestellt, wenn Verbindungstyp auf benutzerdefinierte VPN festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="b40cc-196">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="b40cc-197">Beispiel: Cisco AnyConnect verwendet eine Kennung des dem Formular com.cisco.anyconnect.applevpn.plugin Inherited aus [AppleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b40cc-197">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="b40cc-198">customData</span><span class="sxs-lookup"><span data-stu-id="b40cc-198">customData</span></span>|<span data-ttu-id="b40cc-199">[KeyValue](../resources/intune-deviceconfig-keyvalue.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="b40cc-199">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="b40cc-200">Benutzerdefinierte Daten beim Verbindungstyp auf benutzerdefinierte VPN festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="b40cc-200">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="b40cc-201">Verwenden Sie dieses Feld, um von Intune, nicht jedoch in Ihre VPN-Lösung verfügbar unterstützten Funktionen zu aktivieren.</span><span class="sxs-lookup"><span data-stu-id="b40cc-201">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="b40cc-202">Wenden Sie sich an Ihrer VPN-Hersteller, um Informationen zum Hinzufügen dieser Schlüssel/Wert-Paare.</span><span class="sxs-lookup"><span data-stu-id="b40cc-202">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="b40cc-203">Diese Sammlung kann maximal 25 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="b40cc-203">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="b40cc-204">Geerbt von [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b40cc-204">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="b40cc-205">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="b40cc-205">customKeyValueData</span></span>|<span data-ttu-id="b40cc-206">[keyValuePair](../resources/intune-shared-keyvaluepair.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="b40cc-206">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="b40cc-207">Benutzerdefinierte Daten beim Verbindungstyp auf benutzerdefinierte VPN festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="b40cc-207">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="b40cc-208">Verwenden Sie dieses Feld, um von Intune, nicht jedoch in Ihre VPN-Lösung verfügbar unterstützten Funktionen zu aktivieren.</span><span class="sxs-lookup"><span data-stu-id="b40cc-208">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="b40cc-209">Wenden Sie sich an Ihrer VPN-Hersteller, um Informationen zum Hinzufügen dieser Schlüssel/Wert-Paare.</span><span class="sxs-lookup"><span data-stu-id="b40cc-209">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="b40cc-210">Diese Sammlung kann maximal 25 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="b40cc-210">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="b40cc-211">Geerbt von [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b40cc-211">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="b40cc-212">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="b40cc-212">enableSplitTunneling</span></span>|<span data-ttu-id="b40cc-213">Boolesch</span><span class="sxs-lookup"><span data-stu-id="b40cc-213">Boolean</span></span>|<span data-ttu-id="b40cc-214">Senden Sie alle Netzwerkdatenverkehr über VPN.</span><span class="sxs-lookup"><span data-stu-id="b40cc-214">Send all network traffic through VPN.</span></span> <span data-ttu-id="b40cc-215">Geerbt von [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b40cc-215">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="b40cc-216">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="b40cc-216">authenticationMethod</span></span>|[<span data-ttu-id="b40cc-217">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="b40cc-217">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="b40cc-218">Authentifizierungsmethode für diese VPN-Verbindung.</span><span class="sxs-lookup"><span data-stu-id="b40cc-218">Authentication method for this VPN connection.</span></span> <span data-ttu-id="b40cc-219">Geerbt von [AppleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b40cc-219">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="b40cc-220">Mögliche Werte sind: `certificate` und `usernameAndPassword`.</span><span class="sxs-lookup"><span data-stu-id="b40cc-220">Possible values are: `certificate`, `usernameAndPassword`.</span></span>|
|<span data-ttu-id="b40cc-221">enablePerApp</span><span class="sxs-lookup"><span data-stu-id="b40cc-221">enablePerApp</span></span>|<span data-ttu-id="b40cc-222">Boolesch</span><span class="sxs-lookup"><span data-stu-id="b40cc-222">Boolean</span></span>|<span data-ttu-id="b40cc-223">Dies auf True festlegen, erstellt pro App VPN-Nutzlast, später Apps zugeordnet sein kann, die diese VPN-Verbindung auf iOS-Gerät des Endbenutzers auslösen kann.</span><span class="sxs-lookup"><span data-stu-id="b40cc-223">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span> <span data-ttu-id="b40cc-224">Geerbt von [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b40cc-224">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="b40cc-225">safariDomains</span><span class="sxs-lookup"><span data-stu-id="b40cc-225">safariDomains</span></span>|<span data-ttu-id="b40cc-226">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="b40cc-226">String collection</span></span>|<span data-ttu-id="b40cc-227">Safari Domänen, wenn diese VPN pro App-Einstellung aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="b40cc-227">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="b40cc-228">Zusätzlich zu den apps dieses VPN zugeordnet angegeben Safari Domänen Hier wird auch können Sie diese VPN-Verbindung zu lösen.</span><span class="sxs-lookup"><span data-stu-id="b40cc-228">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span> <span data-ttu-id="b40cc-229">Geerbt von [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b40cc-229">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="b40cc-230">onDemandRules</span><span class="sxs-lookup"><span data-stu-id="b40cc-230">onDemandRules</span></span>|<span data-ttu-id="b40cc-231">[VpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="b40cc-231">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="b40cc-232">Bei Bedarf Regeln.</span><span class="sxs-lookup"><span data-stu-id="b40cc-232">On-Demand Rules.</span></span> <span data-ttu-id="b40cc-233">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="b40cc-233">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="b40cc-234">Geerbt von [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b40cc-234">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="b40cc-235">proxyServer</span><span class="sxs-lookup"><span data-stu-id="b40cc-235">proxyServer</span></span>|[<span data-ttu-id="b40cc-236">vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="b40cc-236">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="b40cc-237">Proxy-Server.</span><span class="sxs-lookup"><span data-stu-id="b40cc-237">Proxy Server.</span></span> <span data-ttu-id="b40cc-238">Geerbt von [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b40cc-238">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="b40cc-239">optInToDeviceIdSharing</span><span class="sxs-lookup"><span data-stu-id="b40cc-239">optInToDeviceIdSharing</span></span>|<span data-ttu-id="b40cc-240">Boolesch</span><span class="sxs-lookup"><span data-stu-id="b40cc-240">Boolean</span></span>|<span data-ttu-id="b40cc-241">Opt-In, das das Gerät Id Drittanbieter-VPN-Clients für die Verwendung während der Network Access Control Validierung Freigabe.</span><span class="sxs-lookup"><span data-stu-id="b40cc-241">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span> <span data-ttu-id="b40cc-242">Geerbt von [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b40cc-242">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="b40cc-243">Antwort</span><span class="sxs-lookup"><span data-stu-id="b40cc-243">Response</span></span>
<span data-ttu-id="b40cc-244">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [MacOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="b40cc-244">If successful, this method returns a `200 OK` response code and an updated [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b40cc-245">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b40cc-245">Example</span></span>
### <a name="request"></a><span data-ttu-id="b40cc-246">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b40cc-246">Request</span></span>
<span data-ttu-id="b40cc-247">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b40cc-247">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1861

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
  "connectionType": "pulseSecure",
  "loginGroupOrDomain": "Login Group Or Domain value",
  "role": "Role value",
  "realm": "Realm value",
  "server": {
    "@odata.type": "microsoft.graph.vpnServer",
    "description": "Description value",
    "address": "Address value",
    "isDefaultServer": true
  },
  "identifier": "Identifier value",
  "customData": [
    {
      "@odata.type": "microsoft.graph.keyValue",
      "key": "Key value",
      "value": "Value value"
    }
  ],
  "customKeyValueData": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "enableSplitTunneling": true,
  "authenticationMethod": "usernameAndPassword",
  "enablePerApp": true,
  "safariDomains": [
    "Safari Domains value"
  ],
  "onDemandRules": [
    {
      "@odata.type": "microsoft.graph.vpnOnDemandRule",
      "ssids": [
        "Ssids value"
      ],
      "dnsSearchDomains": [
        "Dns Search Domains value"
      ],
      "probeUrl": "https://example.com/probeUrl/",
      "action": "evaluateConnection",
      "domainAction": "neverConnect",
      "domains": [
        "Domains value"
      ],
      "probeRequiredUrl": "https://example.com/probeRequiredUrl/"
    }
  ],
  "proxyServer": {
    "@odata.type": "microsoft.graph.vpnProxyServer",
    "automaticConfigurationScriptUrl": "https://example.com/automaticConfigurationScriptUrl/",
    "address": "Address value",
    "port": 4
  },
  "optInToDeviceIdSharing": true
}
```

### <a name="response"></a><span data-ttu-id="b40cc-248">Antwort</span><span class="sxs-lookup"><span data-stu-id="b40cc-248">Response</span></span>
<span data-ttu-id="b40cc-p127">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b40cc-p127">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2029

{
  "@odata.type": "#microsoft.graph.macOSVpnConfiguration",
  "id": "8ce00178-0178-8ce0-7801-e08c7801e08c",
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
  "connectionType": "pulseSecure",
  "loginGroupOrDomain": "Login Group Or Domain value",
  "role": "Role value",
  "realm": "Realm value",
  "server": {
    "@odata.type": "microsoft.graph.vpnServer",
    "description": "Description value",
    "address": "Address value",
    "isDefaultServer": true
  },
  "identifier": "Identifier value",
  "customData": [
    {
      "@odata.type": "microsoft.graph.keyValue",
      "key": "Key value",
      "value": "Value value"
    }
  ],
  "customKeyValueData": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "enableSplitTunneling": true,
  "authenticationMethod": "usernameAndPassword",
  "enablePerApp": true,
  "safariDomains": [
    "Safari Domains value"
  ],
  "onDemandRules": [
    {
      "@odata.type": "microsoft.graph.vpnOnDemandRule",
      "ssids": [
        "Ssids value"
      ],
      "dnsSearchDomains": [
        "Dns Search Domains value"
      ],
      "probeUrl": "https://example.com/probeUrl/",
      "action": "evaluateConnection",
      "domainAction": "neverConnect",
      "domains": [
        "Domains value"
      ],
      "probeRequiredUrl": "https://example.com/probeRequiredUrl/"
    }
  ],
  "proxyServer": {
    "@odata.type": "microsoft.graph.vpnProxyServer",
    "automaticConfigurationScriptUrl": "https://example.com/automaticConfigurationScriptUrl/",
    "address": "Address value",
    "port": 4
  },
  "optInToDeviceIdSharing": true
}
```





