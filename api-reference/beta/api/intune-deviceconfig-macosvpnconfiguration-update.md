---
title: MacOSVpnConfiguration aktualisieren
description: Aktualisieren Sie die Eigenschaften eines MacOSVpnConfiguration-Objekts.
ms.openlocfilehash: a8be01c1d61622581476d413417bb93b6140d12b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062242"
---
# <a name="update-macosvpnconfiguration"></a><span data-ttu-id="f4af5-103">MacOSVpnConfiguration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="f4af5-103">Update macOSVpnConfiguration</span></span>

> <span data-ttu-id="f4af5-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f4af5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f4af5-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f4af5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f4af5-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="f4af5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f4af5-107">Aktualisieren Sie die Eigenschaften eines [MacOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="f4af5-107">Update the properties of a [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f4af5-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f4af5-108">Prerequisites</span></span>
<span data-ttu-id="f4af5-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f4af5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f4af5-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f4af5-111">Permission type</span></span>|<span data-ttu-id="f4af5-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f4af5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f4af5-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f4af5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f4af5-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4af5-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f4af5-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f4af5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f4af5-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f4af5-116">Not supported.</span></span>|
|<span data-ttu-id="f4af5-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f4af5-117">Application</span></span>|<span data-ttu-id="f4af5-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f4af5-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f4af5-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f4af5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="f4af5-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f4af5-120">Request headers</span></span>
|<span data-ttu-id="f4af5-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="f4af5-121">Header</span></span>|<span data-ttu-id="f4af5-122">Wert</span><span class="sxs-lookup"><span data-stu-id="f4af5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f4af5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f4af5-123">Authorization</span></span>|<span data-ttu-id="f4af5-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="f4af5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f4af5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f4af5-125">Accept</span></span>|<span data-ttu-id="f4af5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f4af5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f4af5-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f4af5-127">Request body</span></span>
<span data-ttu-id="f4af5-128">Geben Sie im Textkörper Anforderung für das Objekt [MacOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="f4af5-128">In the request body, supply a JSON representation for the [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) object.</span></span>

<span data-ttu-id="f4af5-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [MacOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="f4af5-129">The following table shows the properties that are required when you create the [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md).</span></span>

|<span data-ttu-id="f4af5-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f4af5-130">Property</span></span>|<span data-ttu-id="f4af5-131">Typ</span><span class="sxs-lookup"><span data-stu-id="f4af5-131">Type</span></span>|<span data-ttu-id="f4af5-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f4af5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f4af5-133">id</span><span class="sxs-lookup"><span data-stu-id="f4af5-133">id</span></span>|<span data-ttu-id="f4af5-134">String</span><span class="sxs-lookup"><span data-stu-id="f4af5-134">String</span></span>|<span data-ttu-id="f4af5-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="f4af5-135">Key of the entity.</span></span> <span data-ttu-id="f4af5-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f4af5-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f4af5-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f4af5-137">lastModifiedDateTime</span></span>|<span data-ttu-id="f4af5-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f4af5-138">DateTimeOffset</span></span>|<span data-ttu-id="f4af5-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="f4af5-139">DateTime the object was last modified.</span></span> <span data-ttu-id="f4af5-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f4af5-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f4af5-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f4af5-141">roleScopeTagIds</span></span>|<span data-ttu-id="f4af5-142">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="f4af5-142">String collection</span></span>|<span data-ttu-id="f4af5-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="f4af5-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f4af5-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f4af5-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f4af5-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="f4af5-145">supportsScopeTags</span></span>|<span data-ttu-id="f4af5-146">Boolesch</span><span class="sxs-lookup"><span data-stu-id="f4af5-146">Boolean</span></span>|<span data-ttu-id="f4af5-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f4af5-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f4af5-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="f4af5-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f4af5-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="f4af5-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f4af5-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="f4af5-150">This property is read-only.</span></span> <span data-ttu-id="f4af5-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f4af5-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f4af5-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f4af5-152">createdDateTime</span></span>|<span data-ttu-id="f4af5-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f4af5-153">DateTimeOffset</span></span>|<span data-ttu-id="f4af5-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="f4af5-154">DateTime the object was created.</span></span> <span data-ttu-id="f4af5-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f4af5-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f4af5-156">description</span><span class="sxs-lookup"><span data-stu-id="f4af5-156">description</span></span>|<span data-ttu-id="f4af5-157">String</span><span class="sxs-lookup"><span data-stu-id="f4af5-157">String</span></span>|<span data-ttu-id="f4af5-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="f4af5-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f4af5-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f4af5-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f4af5-160">displayName</span><span class="sxs-lookup"><span data-stu-id="f4af5-160">displayName</span></span>|<span data-ttu-id="f4af5-161">String</span><span class="sxs-lookup"><span data-stu-id="f4af5-161">String</span></span>|<span data-ttu-id="f4af5-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="f4af5-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f4af5-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f4af5-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f4af5-164">Version</span><span class="sxs-lookup"><span data-stu-id="f4af5-164">version</span></span>|<span data-ttu-id="f4af5-165">Int32</span><span class="sxs-lookup"><span data-stu-id="f4af5-165">Int32</span></span>|<span data-ttu-id="f4af5-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="f4af5-166">Version of the device configuration.</span></span> <span data-ttu-id="f4af5-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f4af5-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f4af5-168">connectionName</span><span class="sxs-lookup"><span data-stu-id="f4af5-168">connectionName</span></span>|<span data-ttu-id="f4af5-169">String</span><span class="sxs-lookup"><span data-stu-id="f4af5-169">String</span></span>|<span data-ttu-id="f4af5-170">Name der Verbindung für den Benutzer angezeigt.</span><span class="sxs-lookup"><span data-stu-id="f4af5-170">Connection name displayed to the user.</span></span> <span data-ttu-id="f4af5-171">Geerbt von [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f4af5-171">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="f4af5-172">connectionType</span><span class="sxs-lookup"><span data-stu-id="f4af5-172">connectionType</span></span>|[<span data-ttu-id="f4af5-173">appleVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="f4af5-173">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="f4af5-174">Verbindungstyp.</span><span class="sxs-lookup"><span data-stu-id="f4af5-174">Connection type.</span></span> <span data-ttu-id="f4af5-175">Geerbt von [AppleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f4af5-175">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="f4af5-176">Mögliche Werte sind: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`.</span><span class="sxs-lookup"><span data-stu-id="f4af5-176">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`.</span></span>|
|<span data-ttu-id="f4af5-177">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="f4af5-177">loginGroupOrDomain</span></span>|<span data-ttu-id="f4af5-178">String</span><span class="sxs-lookup"><span data-stu-id="f4af5-178">String</span></span>|<span data-ttu-id="f4af5-179">Anmeldegruppe oder Domäne Wenn Verbindungstyp auf Dell SonicWALL Mobile Verbindung festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="f4af5-179">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="f4af5-180">Geerbt von [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f4af5-180">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="f4af5-181">role</span><span class="sxs-lookup"><span data-stu-id="f4af5-181">role</span></span>|<span data-ttu-id="f4af5-182">String</span><span class="sxs-lookup"><span data-stu-id="f4af5-182">String</span></span>|<span data-ttu-id="f4af5-183">Rolle, wenn Verbindungstyp auf Pulse Secure festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="f4af5-183">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="f4af5-184">Geerbt von [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f4af5-184">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="f4af5-185">Bereich</span><span class="sxs-lookup"><span data-stu-id="f4af5-185">realm</span></span>|<span data-ttu-id="f4af5-186">String</span><span class="sxs-lookup"><span data-stu-id="f4af5-186">String</span></span>|<span data-ttu-id="f4af5-187">Realm Wenn Verbindungstyp auf Pulse Secure festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="f4af5-187">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="f4af5-188">Geerbt von [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f4af5-188">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="f4af5-189">Server</span><span class="sxs-lookup"><span data-stu-id="f4af5-189">server</span></span>|[<span data-ttu-id="f4af5-190">vpnServer</span><span class="sxs-lookup"><span data-stu-id="f4af5-190">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="f4af5-191">VPN-Server im Netzwerk.</span><span class="sxs-lookup"><span data-stu-id="f4af5-191">VPN Server on the network.</span></span> <span data-ttu-id="f4af5-192">Stellen Sie sicher, dass Endbenutzer dieser Speicherort im Netzwerk zugreifen können.</span><span class="sxs-lookup"><span data-stu-id="f4af5-192">Make sure end users can access this network location.</span></span> <span data-ttu-id="f4af5-193">Geerbt von [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f4af5-193">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="f4af5-194">Bezeichner</span><span class="sxs-lookup"><span data-stu-id="f4af5-194">identifier</span></span>|<span data-ttu-id="f4af5-195">String</span><span class="sxs-lookup"><span data-stu-id="f4af5-195">String</span></span>|<span data-ttu-id="f4af5-196">Bezeichner von VPN-Anbieter bereitgestellt, wenn Verbindungstyp auf benutzerdefinierte VPN festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="f4af5-196">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="f4af5-197">Beispiel: Cisco AnyConnect verwendet eine Kennung des dem Formular com.cisco.anyconnect.applevpn.plugin Inherited aus [AppleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f4af5-197">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="f4af5-198">customData</span><span class="sxs-lookup"><span data-stu-id="f4af5-198">customData</span></span>|<span data-ttu-id="f4af5-199">[KeyValue](../resources/intune-deviceconfig-keyvalue.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="f4af5-199">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="f4af5-200">Benutzerdefinierte Daten beim Verbindungstyp auf benutzerdefinierte VPN festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="f4af5-200">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="f4af5-201">Verwenden Sie dieses Feld, um von Intune, nicht jedoch in Ihre VPN-Lösung verfügbar unterstützten Funktionen zu aktivieren.</span><span class="sxs-lookup"><span data-stu-id="f4af5-201">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="f4af5-202">Wenden Sie sich an Ihrer VPN-Hersteller, um Informationen zum Hinzufügen dieser Schlüssel/Wert-Paare.</span><span class="sxs-lookup"><span data-stu-id="f4af5-202">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="f4af5-203">Diese Sammlung kann maximal 25 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="f4af5-203">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="f4af5-204">Geerbt von [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f4af5-204">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="f4af5-205">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="f4af5-205">customKeyValueData</span></span>|<span data-ttu-id="f4af5-206">[keyValuePair](../resources/intune-shared-keyvaluepair.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="f4af5-206">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="f4af5-207">Benutzerdefinierte Daten beim Verbindungstyp auf benutzerdefinierte VPN festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="f4af5-207">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="f4af5-208">Verwenden Sie dieses Feld, um von Intune, nicht jedoch in Ihre VPN-Lösung verfügbar unterstützten Funktionen zu aktivieren.</span><span class="sxs-lookup"><span data-stu-id="f4af5-208">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="f4af5-209">Wenden Sie sich an Ihrer VPN-Hersteller, um Informationen zum Hinzufügen dieser Schlüssel/Wert-Paare.</span><span class="sxs-lookup"><span data-stu-id="f4af5-209">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="f4af5-210">Diese Sammlung kann maximal 25 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="f4af5-210">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="f4af5-211">Geerbt von [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f4af5-211">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="f4af5-212">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="f4af5-212">enableSplitTunneling</span></span>|<span data-ttu-id="f4af5-213">Boolesch</span><span class="sxs-lookup"><span data-stu-id="f4af5-213">Boolean</span></span>|<span data-ttu-id="f4af5-214">Senden Sie alle Netzwerkdatenverkehr über VPN.</span><span class="sxs-lookup"><span data-stu-id="f4af5-214">Send all network traffic through VPN.</span></span> <span data-ttu-id="f4af5-215">Geerbt von [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f4af5-215">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="f4af5-216">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="f4af5-216">authenticationMethod</span></span>|[<span data-ttu-id="f4af5-217">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="f4af5-217">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="f4af5-218">Authentifizierungsmethode für diese VPN-Verbindung.</span><span class="sxs-lookup"><span data-stu-id="f4af5-218">Authentication method for this VPN connection.</span></span> <span data-ttu-id="f4af5-219">Geerbt von [AppleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f4af5-219">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="f4af5-220">Mögliche Werte sind: `certificate` und `usernameAndPassword`.</span><span class="sxs-lookup"><span data-stu-id="f4af5-220">Possible values are: `certificate`, `usernameAndPassword`.</span></span>|
|<span data-ttu-id="f4af5-221">enablePerApp</span><span class="sxs-lookup"><span data-stu-id="f4af5-221">enablePerApp</span></span>|<span data-ttu-id="f4af5-222">Boolesch</span><span class="sxs-lookup"><span data-stu-id="f4af5-222">Boolean</span></span>|<span data-ttu-id="f4af5-223">Dies auf True festlegen, erstellt pro App VPN-Nutzlast, später Apps zugeordnet sein kann, die diese VPN-Verbindung auf iOS-Gerät des Endbenutzers auslösen kann.</span><span class="sxs-lookup"><span data-stu-id="f4af5-223">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span> <span data-ttu-id="f4af5-224">Geerbt von [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f4af5-224">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="f4af5-225">safariDomains</span><span class="sxs-lookup"><span data-stu-id="f4af5-225">safariDomains</span></span>|<span data-ttu-id="f4af5-226">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="f4af5-226">String collection</span></span>|<span data-ttu-id="f4af5-227">Safari Domänen, wenn diese VPN pro App-Einstellung aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="f4af5-227">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="f4af5-228">Zusätzlich zu den apps dieses VPN zugeordnet angegeben Safari Domänen Hier wird auch können Sie diese VPN-Verbindung zu lösen.</span><span class="sxs-lookup"><span data-stu-id="f4af5-228">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span> <span data-ttu-id="f4af5-229">Geerbt von [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f4af5-229">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="f4af5-230">onDemandRules</span><span class="sxs-lookup"><span data-stu-id="f4af5-230">onDemandRules</span></span>|<span data-ttu-id="f4af5-231">[VpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="f4af5-231">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="f4af5-232">Bei Bedarf Regeln.</span><span class="sxs-lookup"><span data-stu-id="f4af5-232">On-Demand Rules.</span></span> <span data-ttu-id="f4af5-233">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="f4af5-233">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="f4af5-234">Geerbt von [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f4af5-234">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="f4af5-235">proxyServer</span><span class="sxs-lookup"><span data-stu-id="f4af5-235">proxyServer</span></span>|[<span data-ttu-id="f4af5-236">vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="f4af5-236">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="f4af5-237">Proxy-Server.</span><span class="sxs-lookup"><span data-stu-id="f4af5-237">Proxy Server.</span></span> <span data-ttu-id="f4af5-238">Geerbt von [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f4af5-238">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="f4af5-239">optInToDeviceIdSharing</span><span class="sxs-lookup"><span data-stu-id="f4af5-239">optInToDeviceIdSharing</span></span>|<span data-ttu-id="f4af5-240">Boolesch</span><span class="sxs-lookup"><span data-stu-id="f4af5-240">Boolean</span></span>|<span data-ttu-id="f4af5-241">Opt-In, das das Gerät Id Drittanbieter-VPN-Clients für die Verwendung während der Network Access Control Validierung Freigabe.</span><span class="sxs-lookup"><span data-stu-id="f4af5-241">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span> <span data-ttu-id="f4af5-242">Geerbt von [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f4af5-242">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="f4af5-243">Antwort</span><span class="sxs-lookup"><span data-stu-id="f4af5-243">Response</span></span>
<span data-ttu-id="f4af5-244">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [MacOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="f4af5-244">If successful, this method returns a `200 OK` response code and an updated [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f4af5-245">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f4af5-245">Example</span></span>
### <a name="request"></a><span data-ttu-id="f4af5-246">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f4af5-246">Request</span></span>
<span data-ttu-id="f4af5-247">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f4af5-247">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f4af5-248">Antwort</span><span class="sxs-lookup"><span data-stu-id="f4af5-248">Response</span></span>
<span data-ttu-id="f4af5-p127">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f4af5-p127">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





