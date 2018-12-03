---
title: Erstellen von iosVpnConfiguration
description: Erstellen eines neuen IosVpnConfiguration-Objekts.
ms.openlocfilehash: 3cb5640a77f44025d7f3582a90c4681c7e97f3e2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061650"
---
# <a name="create-iosvpnconfiguration"></a><span data-ttu-id="6c4db-103">Erstellen von iosVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="6c4db-103">Create iosVpnConfiguration</span></span>

> <span data-ttu-id="6c4db-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="6c4db-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6c4db-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6c4db-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6c4db-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="6c4db-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6c4db-107">Erstellen eines neuen [IosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="6c4db-107">Create a new [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6c4db-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="6c4db-108">Prerequisites</span></span>
<span data-ttu-id="6c4db-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6c4db-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6c4db-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6c4db-111">Permission type</span></span>|<span data-ttu-id="6c4db-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6c4db-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6c4db-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6c4db-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6c4db-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c4db-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6c4db-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6c4db-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6c4db-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6c4db-116">Not supported.</span></span>|
|<span data-ttu-id="6c4db-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6c4db-117">Application</span></span>|<span data-ttu-id="6c4db-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6c4db-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6c4db-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6c4db-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="6c4db-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6c4db-120">Request headers</span></span>
|<span data-ttu-id="6c4db-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="6c4db-121">Header</span></span>|<span data-ttu-id="6c4db-122">Wert</span><span class="sxs-lookup"><span data-stu-id="6c4db-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6c4db-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6c4db-123">Authorization</span></span>|<span data-ttu-id="6c4db-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="6c4db-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6c4db-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6c4db-125">Accept</span></span>|<span data-ttu-id="6c4db-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6c4db-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6c4db-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6c4db-127">Request body</span></span>
<span data-ttu-id="6c4db-128">Geben Sie im Textkörper Anforderung für das Objekt IosVpnConfiguration eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="6c4db-128">In the request body, supply a JSON representation for the iosVpnConfiguration object.</span></span>

<span data-ttu-id="6c4db-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die IosVpnConfiguration erstellen.</span><span class="sxs-lookup"><span data-stu-id="6c4db-129">The following table shows the properties that are required when you create the iosVpnConfiguration.</span></span>

|<span data-ttu-id="6c4db-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6c4db-130">Property</span></span>|<span data-ttu-id="6c4db-131">Typ</span><span class="sxs-lookup"><span data-stu-id="6c4db-131">Type</span></span>|<span data-ttu-id="6c4db-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6c4db-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6c4db-133">id</span><span class="sxs-lookup"><span data-stu-id="6c4db-133">id</span></span>|<span data-ttu-id="6c4db-134">String</span><span class="sxs-lookup"><span data-stu-id="6c4db-134">String</span></span>|<span data-ttu-id="6c4db-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="6c4db-135">Key of the entity.</span></span> <span data-ttu-id="6c4db-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6c4db-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6c4db-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6c4db-137">lastModifiedDateTime</span></span>|<span data-ttu-id="6c4db-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6c4db-138">DateTimeOffset</span></span>|<span data-ttu-id="6c4db-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="6c4db-139">DateTime the object was last modified.</span></span> <span data-ttu-id="6c4db-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6c4db-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6c4db-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6c4db-141">roleScopeTagIds</span></span>|<span data-ttu-id="6c4db-142">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="6c4db-142">String collection</span></span>|<span data-ttu-id="6c4db-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="6c4db-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="6c4db-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6c4db-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6c4db-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="6c4db-145">supportsScopeTags</span></span>|<span data-ttu-id="6c4db-146">Boolesch</span><span class="sxs-lookup"><span data-stu-id="6c4db-146">Boolean</span></span>|<span data-ttu-id="6c4db-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6c4db-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="6c4db-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="6c4db-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="6c4db-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="6c4db-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="6c4db-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="6c4db-150">This property is read-only.</span></span> <span data-ttu-id="6c4db-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6c4db-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6c4db-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6c4db-152">createdDateTime</span></span>|<span data-ttu-id="6c4db-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6c4db-153">DateTimeOffset</span></span>|<span data-ttu-id="6c4db-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="6c4db-154">DateTime the object was created.</span></span> <span data-ttu-id="6c4db-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6c4db-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6c4db-156">description</span><span class="sxs-lookup"><span data-stu-id="6c4db-156">description</span></span>|<span data-ttu-id="6c4db-157">String</span><span class="sxs-lookup"><span data-stu-id="6c4db-157">String</span></span>|<span data-ttu-id="6c4db-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="6c4db-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6c4db-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6c4db-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6c4db-160">displayName</span><span class="sxs-lookup"><span data-stu-id="6c4db-160">displayName</span></span>|<span data-ttu-id="6c4db-161">String</span><span class="sxs-lookup"><span data-stu-id="6c4db-161">String</span></span>|<span data-ttu-id="6c4db-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="6c4db-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6c4db-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6c4db-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6c4db-164">Version</span><span class="sxs-lookup"><span data-stu-id="6c4db-164">version</span></span>|<span data-ttu-id="6c4db-165">Int32</span><span class="sxs-lookup"><span data-stu-id="6c4db-165">Int32</span></span>|<span data-ttu-id="6c4db-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="6c4db-166">Version of the device configuration.</span></span> <span data-ttu-id="6c4db-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6c4db-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6c4db-168">connectionName</span><span class="sxs-lookup"><span data-stu-id="6c4db-168">connectionName</span></span>|<span data-ttu-id="6c4db-169">String</span><span class="sxs-lookup"><span data-stu-id="6c4db-169">String</span></span>|<span data-ttu-id="6c4db-170">Name der Verbindung für den Benutzer angezeigt.</span><span class="sxs-lookup"><span data-stu-id="6c4db-170">Connection name displayed to the user.</span></span> <span data-ttu-id="6c4db-171">Geerbt von [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6c4db-171">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="6c4db-172">connectionType</span><span class="sxs-lookup"><span data-stu-id="6c4db-172">connectionType</span></span>|[<span data-ttu-id="6c4db-173">appleVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="6c4db-173">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="6c4db-174">Verbindungstyp.</span><span class="sxs-lookup"><span data-stu-id="6c4db-174">Connection type.</span></span> <span data-ttu-id="6c4db-175">Geerbt von [AppleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6c4db-175">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="6c4db-176">Mögliche Werte sind: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`.</span><span class="sxs-lookup"><span data-stu-id="6c4db-176">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`.</span></span>|
|<span data-ttu-id="6c4db-177">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="6c4db-177">loginGroupOrDomain</span></span>|<span data-ttu-id="6c4db-178">String</span><span class="sxs-lookup"><span data-stu-id="6c4db-178">String</span></span>|<span data-ttu-id="6c4db-179">Anmeldegruppe oder Domäne Wenn Verbindungstyp auf Dell SonicWALL Mobile Verbindung festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="6c4db-179">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="6c4db-180">Geerbt von [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6c4db-180">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="6c4db-181">role</span><span class="sxs-lookup"><span data-stu-id="6c4db-181">role</span></span>|<span data-ttu-id="6c4db-182">String</span><span class="sxs-lookup"><span data-stu-id="6c4db-182">String</span></span>|<span data-ttu-id="6c4db-183">Rolle, wenn Verbindungstyp auf Pulse Secure festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="6c4db-183">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="6c4db-184">Geerbt von [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6c4db-184">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="6c4db-185">Bereich</span><span class="sxs-lookup"><span data-stu-id="6c4db-185">realm</span></span>|<span data-ttu-id="6c4db-186">String</span><span class="sxs-lookup"><span data-stu-id="6c4db-186">String</span></span>|<span data-ttu-id="6c4db-187">Realm Wenn Verbindungstyp auf Pulse Secure festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="6c4db-187">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="6c4db-188">Geerbt von [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6c4db-188">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="6c4db-189">Server</span><span class="sxs-lookup"><span data-stu-id="6c4db-189">server</span></span>|[<span data-ttu-id="6c4db-190">vpnServer</span><span class="sxs-lookup"><span data-stu-id="6c4db-190">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="6c4db-191">VPN-Server im Netzwerk.</span><span class="sxs-lookup"><span data-stu-id="6c4db-191">VPN Server on the network.</span></span> <span data-ttu-id="6c4db-192">Stellen Sie sicher, dass Endbenutzer dieser Speicherort im Netzwerk zugreifen können.</span><span class="sxs-lookup"><span data-stu-id="6c4db-192">Make sure end users can access this network location.</span></span> <span data-ttu-id="6c4db-193">Geerbt von [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6c4db-193">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="6c4db-194">Bezeichner</span><span class="sxs-lookup"><span data-stu-id="6c4db-194">identifier</span></span>|<span data-ttu-id="6c4db-195">String</span><span class="sxs-lookup"><span data-stu-id="6c4db-195">String</span></span>|<span data-ttu-id="6c4db-196">Bezeichner von VPN-Anbieter bereitgestellt, wenn Verbindungstyp auf benutzerdefinierte VPN festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="6c4db-196">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="6c4db-197">Beispiel: Cisco AnyConnect verwendet eine Kennung des dem Formular com.cisco.anyconnect.applevpn.plugin Inherited aus [AppleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6c4db-197">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="6c4db-198">customData</span><span class="sxs-lookup"><span data-stu-id="6c4db-198">customData</span></span>|<span data-ttu-id="6c4db-199">[KeyValue](../resources/intune-deviceconfig-keyvalue.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="6c4db-199">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="6c4db-200">Benutzerdefinierte Daten beim Verbindungstyp auf benutzerdefinierte VPN festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="6c4db-200">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="6c4db-201">Verwenden Sie dieses Feld, um von Intune, nicht jedoch in Ihre VPN-Lösung verfügbar unterstützten Funktionen zu aktivieren.</span><span class="sxs-lookup"><span data-stu-id="6c4db-201">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="6c4db-202">Wenden Sie sich an Ihrer VPN-Hersteller, um Informationen zum Hinzufügen dieser Schlüssel/Wert-Paare.</span><span class="sxs-lookup"><span data-stu-id="6c4db-202">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="6c4db-203">Diese Sammlung kann maximal 25 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="6c4db-203">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="6c4db-204">Geerbt von [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6c4db-204">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="6c4db-205">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="6c4db-205">customKeyValueData</span></span>|<span data-ttu-id="6c4db-206">[keyValuePair](../resources/intune-shared-keyvaluepair.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="6c4db-206">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="6c4db-207">Benutzerdefinierte Daten beim Verbindungstyp auf benutzerdefinierte VPN festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="6c4db-207">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="6c4db-208">Verwenden Sie dieses Feld, um von Intune, nicht jedoch in Ihre VPN-Lösung verfügbar unterstützten Funktionen zu aktivieren.</span><span class="sxs-lookup"><span data-stu-id="6c4db-208">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="6c4db-209">Wenden Sie sich an Ihrer VPN-Hersteller, um Informationen zum Hinzufügen dieser Schlüssel/Wert-Paare.</span><span class="sxs-lookup"><span data-stu-id="6c4db-209">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="6c4db-210">Diese Sammlung kann maximal 25 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="6c4db-210">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="6c4db-211">Geerbt von [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6c4db-211">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="6c4db-212">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="6c4db-212">enableSplitTunneling</span></span>|<span data-ttu-id="6c4db-213">Boolesch</span><span class="sxs-lookup"><span data-stu-id="6c4db-213">Boolean</span></span>|<span data-ttu-id="6c4db-214">Senden Sie alle Netzwerkdatenverkehr über VPN.</span><span class="sxs-lookup"><span data-stu-id="6c4db-214">Send all network traffic through VPN.</span></span> <span data-ttu-id="6c4db-215">Geerbt von [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6c4db-215">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="6c4db-216">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="6c4db-216">authenticationMethod</span></span>|[<span data-ttu-id="6c4db-217">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="6c4db-217">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="6c4db-218">Authentifizierungsmethode für diese VPN-Verbindung.</span><span class="sxs-lookup"><span data-stu-id="6c4db-218">Authentication method for this VPN connection.</span></span> <span data-ttu-id="6c4db-219">Geerbt von [AppleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6c4db-219">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="6c4db-220">Mögliche Werte sind: `certificate` und `usernameAndPassword`.</span><span class="sxs-lookup"><span data-stu-id="6c4db-220">Possible values are: `certificate`, `usernameAndPassword`.</span></span>|
|<span data-ttu-id="6c4db-221">enablePerApp</span><span class="sxs-lookup"><span data-stu-id="6c4db-221">enablePerApp</span></span>|<span data-ttu-id="6c4db-222">Boolesch</span><span class="sxs-lookup"><span data-stu-id="6c4db-222">Boolean</span></span>|<span data-ttu-id="6c4db-223">Dies auf True festlegen, erstellt pro App VPN-Nutzlast, später Apps zugeordnet sein kann, die diese VPN-Verbindung auf iOS-Gerät des Endbenutzers auslösen kann.</span><span class="sxs-lookup"><span data-stu-id="6c4db-223">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span> <span data-ttu-id="6c4db-224">Geerbt von [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6c4db-224">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="6c4db-225">safariDomains</span><span class="sxs-lookup"><span data-stu-id="6c4db-225">safariDomains</span></span>|<span data-ttu-id="6c4db-226">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="6c4db-226">String collection</span></span>|<span data-ttu-id="6c4db-227">Safari Domänen, wenn diese VPN pro App-Einstellung aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="6c4db-227">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="6c4db-228">Zusätzlich zu den apps dieses VPN zugeordnet angegeben Safari Domänen Hier wird auch können Sie diese VPN-Verbindung zu lösen.</span><span class="sxs-lookup"><span data-stu-id="6c4db-228">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span> <span data-ttu-id="6c4db-229">Geerbt von [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6c4db-229">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="6c4db-230">onDemandRules</span><span class="sxs-lookup"><span data-stu-id="6c4db-230">onDemandRules</span></span>|<span data-ttu-id="6c4db-231">[VpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="6c4db-231">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="6c4db-232">Bei Bedarf Regeln.</span><span class="sxs-lookup"><span data-stu-id="6c4db-232">On-Demand Rules.</span></span> <span data-ttu-id="6c4db-233">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="6c4db-233">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="6c4db-234">Geerbt von [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6c4db-234">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="6c4db-235">proxyServer</span><span class="sxs-lookup"><span data-stu-id="6c4db-235">proxyServer</span></span>|[<span data-ttu-id="6c4db-236">vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="6c4db-236">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="6c4db-237">Proxy-Server.</span><span class="sxs-lookup"><span data-stu-id="6c4db-237">Proxy Server.</span></span> <span data-ttu-id="6c4db-238">Geerbt von [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6c4db-238">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="6c4db-239">optInToDeviceIdSharing</span><span class="sxs-lookup"><span data-stu-id="6c4db-239">optInToDeviceIdSharing</span></span>|<span data-ttu-id="6c4db-240">Boolesch</span><span class="sxs-lookup"><span data-stu-id="6c4db-240">Boolean</span></span>|<span data-ttu-id="6c4db-241">Opt-In, das das Gerät Id Drittanbieter-VPN-Clients für die Verwendung während der Network Access Control Validierung Freigabe.</span><span class="sxs-lookup"><span data-stu-id="6c4db-241">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span> <span data-ttu-id="6c4db-242">Geerbt von [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6c4db-242">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="6c4db-243">providerType</span><span class="sxs-lookup"><span data-stu-id="6c4db-243">providerType</span></span>|[<span data-ttu-id="6c4db-244">vpnProviderType</span><span class="sxs-lookup"><span data-stu-id="6c4db-244">vpnProviderType</span></span>](../resources/intune-deviceconfig-vpnprovidertype.md)|<span data-ttu-id="6c4db-245">Providertyp für VPN-app.</span><span class="sxs-lookup"><span data-stu-id="6c4db-245">Provider type for per-app VPN.</span></span> <span data-ttu-id="6c4db-246">Mögliche Werte sind: `notConfigured`, `appProxy` und `packetTunnel`.</span><span class="sxs-lookup"><span data-stu-id="6c4db-246">Possible values are: `notConfigured`, `appProxy`, `packetTunnel`.</span></span>|
|<span data-ttu-id="6c4db-247">userDomain</span><span class="sxs-lookup"><span data-stu-id="6c4db-247">userDomain</span></span>|<span data-ttu-id="6c4db-248">String</span><span class="sxs-lookup"><span data-stu-id="6c4db-248">String</span></span>|<span data-ttu-id="6c4db-249">Zscaler.</span><span class="sxs-lookup"><span data-stu-id="6c4db-249">Zscaler only.</span></span> <span data-ttu-id="6c4db-250">Geben Sie eine statische Domäne, um das Feld Anmeldename mit in der app Zscaler vorab auszufüllen.</span><span class="sxs-lookup"><span data-stu-id="6c4db-250">Enter a static domain to pre-populate the login field with in the Zscaler app.</span></span> <span data-ttu-id="6c4db-251">Wenn dies leer ist, wird stattdessen Azure Active Directory-Domäne des Benutzers verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="6c4db-251">If this is left empty, the user's Azure Active Directory domain will be used instead.</span></span>|
|<span data-ttu-id="6c4db-252">strictEnforcement</span><span class="sxs-lookup"><span data-stu-id="6c4db-252">strictEnforcement</span></span>|<span data-ttu-id="6c4db-253">Boolesch</span><span class="sxs-lookup"><span data-stu-id="6c4db-253">Boolean</span></span>|<span data-ttu-id="6c4db-254">Zscaler.</span><span class="sxs-lookup"><span data-stu-id="6c4db-254">Zscaler only.</span></span> <span data-ttu-id="6c4db-255">Blöcke Netzwerkverkehr bis auf Anzeichen für die Benutzer in Zscaler app.</span><span class="sxs-lookup"><span data-stu-id="6c4db-255">Blocks network traffic until the user signs into Zscaler app.</span></span> <span data-ttu-id="6c4db-256">"True" bedeutet, dass Datenverkehr ausgeschlossen wird.</span><span class="sxs-lookup"><span data-stu-id="6c4db-256">"True" means traffic is blocked.</span></span>|
|<span data-ttu-id="6c4db-257">cloudName</span><span class="sxs-lookup"><span data-stu-id="6c4db-257">cloudName</span></span>|<span data-ttu-id="6c4db-258">String</span><span class="sxs-lookup"><span data-stu-id="6c4db-258">String</span></span>|<span data-ttu-id="6c4db-259">Zscaler.</span><span class="sxs-lookup"><span data-stu-id="6c4db-259">Zscaler only.</span></span> <span data-ttu-id="6c4db-260">Zscaler Cloud, die der Benutzer zugewiesen ist.</span><span class="sxs-lookup"><span data-stu-id="6c4db-260">Zscaler cloud which the user is assigned to.</span></span>|
|<span data-ttu-id="6c4db-261">excludeList</span><span class="sxs-lookup"><span data-stu-id="6c4db-261">excludeList</span></span>|<span data-ttu-id="6c4db-262">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="6c4db-262">String collection</span></span>|<span data-ttu-id="6c4db-263">Zscaler.</span><span class="sxs-lookup"><span data-stu-id="6c4db-263">Zscaler only.</span></span> <span data-ttu-id="6c4db-264">Liste der Netzwerkadressen, die nicht über die Cloud Zscaler gesendet werden.</span><span class="sxs-lookup"><span data-stu-id="6c4db-264">List of network addresses which are not sent through the Zscaler cloud.</span></span>|



## <a name="response"></a><span data-ttu-id="6c4db-265">Antwort</span><span class="sxs-lookup"><span data-stu-id="6c4db-265">Response</span></span>
<span data-ttu-id="6c4db-266">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [IosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="6c4db-266">If successful, this method returns a `201 Created` response code and a [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6c4db-267">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6c4db-267">Example</span></span>
### <a name="request"></a><span data-ttu-id="6c4db-268">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6c4db-268">Request</span></span>
<span data-ttu-id="6c4db-269">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6c4db-269">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 2106

{
  "@odata.type": "#microsoft.graph.iosVpnConfiguration",
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
  "optInToDeviceIdSharing": true,
  "providerType": "appProxy",
  "userDomain": "User Domain value",
  "strictEnforcement": true,
  "cloudName": "Cloud Name value",
  "excludeList": [
    "Exclude List value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="6c4db-270">Antwort</span><span class="sxs-lookup"><span data-stu-id="6c4db-270">Response</span></span>
<span data-ttu-id="6c4db-p132">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6c4db-p132">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2214

{
  "@odata.type": "#microsoft.graph.iosVpnConfiguration",
  "id": "bd12424c-424c-bd12-4c42-12bd4c4212bd",
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
  "optInToDeviceIdSharing": true,
  "providerType": "appProxy",
  "userDomain": "User Domain value",
  "strictEnforcement": true,
  "cloudName": "Cloud Name value",
  "excludeList": [
    "Exclude List value"
  ]
}
```





