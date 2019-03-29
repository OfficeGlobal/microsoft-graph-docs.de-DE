---
title: IosVpnConfiguration aktualisieren
description: Aktualisieren der Eigenschaften eines iosVpnConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5ac4b2fed7aae387854f1ca2b04587d847dc1d8b
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30981601"
---
# <a name="update-iosvpnconfiguration"></a><span data-ttu-id="c1827-103">IosVpnConfiguration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="c1827-103">Update iosVpnConfiguration</span></span>

> <span data-ttu-id="c1827-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c1827-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c1827-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="c1827-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c1827-106">Aktualisieren der Eigenschaften eines [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="c1827-106">Update the properties of a [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c1827-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c1827-107">Prerequisites</span></span>
<span data-ttu-id="c1827-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c1827-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c1827-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c1827-110">Permission type</span></span>|<span data-ttu-id="c1827-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c1827-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c1827-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c1827-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c1827-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1827-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c1827-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c1827-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c1827-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c1827-115">Not supported.</span></span>|
|<span data-ttu-id="c1827-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c1827-116">Application</span></span>|<span data-ttu-id="c1827-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c1827-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c1827-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c1827-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="c1827-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c1827-119">Request headers</span></span>
|<span data-ttu-id="c1827-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="c1827-120">Header</span></span>|<span data-ttu-id="c1827-121">Wert</span><span class="sxs-lookup"><span data-stu-id="c1827-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c1827-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c1827-122">Authorization</span></span>|<span data-ttu-id="c1827-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c1827-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c1827-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="c1827-124">Accept</span></span>|<span data-ttu-id="c1827-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c1827-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c1827-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c1827-126">Request body</span></span>
<span data-ttu-id="c1827-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="c1827-127">In the request body, supply a JSON representation for the [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) object.</span></span>

<span data-ttu-id="c1827-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="c1827-128">The following table shows the properties that are required when you create the [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md).</span></span>

|<span data-ttu-id="c1827-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c1827-129">Property</span></span>|<span data-ttu-id="c1827-130">Typ</span><span class="sxs-lookup"><span data-stu-id="c1827-130">Type</span></span>|<span data-ttu-id="c1827-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c1827-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c1827-132">id</span><span class="sxs-lookup"><span data-stu-id="c1827-132">id</span></span>|<span data-ttu-id="c1827-133">String</span><span class="sxs-lookup"><span data-stu-id="c1827-133">String</span></span>|<span data-ttu-id="c1827-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="c1827-134">Key of the entity.</span></span> <span data-ttu-id="c1827-135">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c1827-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c1827-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c1827-136">lastModifiedDateTime</span></span>|<span data-ttu-id="c1827-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c1827-137">DateTimeOffset</span></span>|<span data-ttu-id="c1827-138">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="c1827-138">DateTime the object was last modified.</span></span> <span data-ttu-id="c1827-139">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c1827-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c1827-140">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="c1827-140">roleScopeTagIds</span></span>|<span data-ttu-id="c1827-141">String collection</span><span class="sxs-lookup"><span data-stu-id="c1827-141">String collection</span></span>|<span data-ttu-id="c1827-142">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="c1827-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c1827-143">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c1827-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c1827-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="c1827-144">supportsScopeTags</span></span>|<span data-ttu-id="c1827-145">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c1827-145">Boolean</span></span>|<span data-ttu-id="c1827-146">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereichs Tags unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c1827-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="c1827-147">Das Zuweisen zur ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert auf false festgelegt ist und Entitäten für bereichsbezogene Benutzer nicht sichtbar sind.</span><span class="sxs-lookup"><span data-stu-id="c1827-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="c1827-148">Dies geschieht für in Silverlight erstellte Legacy Richtlinien und kann durch Löschen und erneutes Erstellen der Richtlinie im Azure-Portal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="c1827-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="c1827-149">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="c1827-149">This property is read-only.</span></span> <span data-ttu-id="c1827-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c1827-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c1827-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c1827-151">createdDateTime</span></span>|<span data-ttu-id="c1827-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c1827-152">DateTimeOffset</span></span>|<span data-ttu-id="c1827-153">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="c1827-153">DateTime the object was created.</span></span> <span data-ttu-id="c1827-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c1827-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c1827-155">description</span><span class="sxs-lookup"><span data-stu-id="c1827-155">description</span></span>|<span data-ttu-id="c1827-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c1827-156">String</span></span>|<span data-ttu-id="c1827-157">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="c1827-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c1827-158">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c1827-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c1827-159">displayName</span><span class="sxs-lookup"><span data-stu-id="c1827-159">displayName</span></span>|<span data-ttu-id="c1827-160">String</span><span class="sxs-lookup"><span data-stu-id="c1827-160">String</span></span>|<span data-ttu-id="c1827-161">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="c1827-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c1827-162">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c1827-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c1827-163">Version</span><span class="sxs-lookup"><span data-stu-id="c1827-163">version</span></span>|<span data-ttu-id="c1827-164">Int32</span><span class="sxs-lookup"><span data-stu-id="c1827-164">Int32</span></span>|<span data-ttu-id="c1827-165">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="c1827-165">Version of the device configuration.</span></span> <span data-ttu-id="c1827-166">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c1827-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c1827-167">connectionName</span><span class="sxs-lookup"><span data-stu-id="c1827-167">connectionName</span></span>|<span data-ttu-id="c1827-168">String</span><span class="sxs-lookup"><span data-stu-id="c1827-168">String</span></span>|<span data-ttu-id="c1827-169">Dem Benutzer angezeigter Verbindungsname.</span><span class="sxs-lookup"><span data-stu-id="c1827-169">Connection name displayed to the user.</span></span> <span data-ttu-id="c1827-170">Geerbt von [der applevpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c1827-170">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="c1827-171">connectionType</span><span class="sxs-lookup"><span data-stu-id="c1827-171">connectionType</span></span>|[<span data-ttu-id="c1827-172">appleVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="c1827-172">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="c1827-173">Verbindungstyp.</span><span class="sxs-lookup"><span data-stu-id="c1827-173">Connection type.</span></span> <span data-ttu-id="c1827-174">Von [der applevpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="c1827-174">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="c1827-175">Mögliche Werte sind: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient` `dellSonicWallMobileConnect` `checkPointCapsuleVpn`,,, `customVpn`, `ciscoIPSec` `citrix`,, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess` `f5Access2018` `citrixSso`,,, `paloAltoGlobalProtectV2`.</span><span class="sxs-lookup"><span data-stu-id="c1827-175">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`.</span></span>|
|<span data-ttu-id="c1827-176">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="c1827-176">loginGroupOrDomain</span></span>|<span data-ttu-id="c1827-177">String</span><span class="sxs-lookup"><span data-stu-id="c1827-177">String</span></span>|<span data-ttu-id="c1827-178">Anmeldegruppe oder Domäne, wenn der Verbindungstyp auf Dell SonicWALL Mobile Connection festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="c1827-178">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="c1827-179">Geerbt von [der applevpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c1827-179">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="c1827-180">role</span><span class="sxs-lookup"><span data-stu-id="c1827-180">role</span></span>|<span data-ttu-id="c1827-181">String</span><span class="sxs-lookup"><span data-stu-id="c1827-181">String</span></span>|<span data-ttu-id="c1827-182">Role, wenn der Verbindungstyp auf Pulse Secure festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="c1827-182">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="c1827-183">Geerbt von [der applevpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c1827-183">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="c1827-184">Reich</span><span class="sxs-lookup"><span data-stu-id="c1827-184">realm</span></span>|<span data-ttu-id="c1827-185">String</span><span class="sxs-lookup"><span data-stu-id="c1827-185">String</span></span>|<span data-ttu-id="c1827-186">Bereich, wenn der Verbindungstyp auf Pulse Secure festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="c1827-186">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="c1827-187">Geerbt von [der applevpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c1827-187">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="c1827-188">Server</span><span class="sxs-lookup"><span data-stu-id="c1827-188">server</span></span>|[<span data-ttu-id="c1827-189">vpnServer</span><span class="sxs-lookup"><span data-stu-id="c1827-189">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="c1827-190">VPN-Server im Netzwerk.</span><span class="sxs-lookup"><span data-stu-id="c1827-190">VPN Server on the network.</span></span> <span data-ttu-id="c1827-191">Stellen Sie sicher, dass Endbenutzer auf diesen Netzwerkspeicherort zugreifen können.</span><span class="sxs-lookup"><span data-stu-id="c1827-191">Make sure end users can access this network location.</span></span> <span data-ttu-id="c1827-192">Geerbt von [der applevpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c1827-192">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="c1827-193">Bezeichner</span><span class="sxs-lookup"><span data-stu-id="c1827-193">identifier</span></span>|<span data-ttu-id="c1827-194">String</span><span class="sxs-lookup"><span data-stu-id="c1827-194">String</span></span>|<span data-ttu-id="c1827-195">Vom VPN-Anbieter bereitgestellter Bezeichner, wenn der Verbindungstyp auf benutzerdefiniertes VPN festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="c1827-195">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="c1827-196">Beispiel: Cisco AnyConnect verwendet einen Bezeichner des Formulars "com. Cisco. AnyConnect. applevpn. Plugin", geerbt von [der applevpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c1827-196">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="c1827-197">customData</span><span class="sxs-lookup"><span data-stu-id="c1827-197">customData</span></span>|<span data-ttu-id="c1827-198">[keyValue](../resources/intune-deviceconfig-keyvalue.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="c1827-198">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="c1827-199">Benutzerdefinierte Daten, wenn der Verbindungstyp auf benutzerdefiniertes VPN festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="c1827-199">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="c1827-200">Verwenden Sie dieses Feld, um die Funktionalität zu aktivieren, die von InTune nicht unterstützt wird, aber in Ihrer VPN-Lösung verfügbar ist.</span><span class="sxs-lookup"><span data-stu-id="c1827-200">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="c1827-201">Wenden Sie sich an Ihren VPN-Anbieter, um zu erfahren, wie diese Schlüssel-Wert-Paare hinzugefügt werden.</span><span class="sxs-lookup"><span data-stu-id="c1827-201">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="c1827-202">Diese Auflistung kann maximal 25 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="c1827-202">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="c1827-203">Geerbt von [der applevpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c1827-203">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="c1827-204">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="c1827-204">customKeyValueData</span></span>|<span data-ttu-id="c1827-205">[keyValuePair](../resources/intune-shared-keyvaluepair.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="c1827-205">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="c1827-206">Benutzerdefinierte Daten, wenn der Verbindungstyp auf benutzerdefiniertes VPN festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="c1827-206">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="c1827-207">Verwenden Sie dieses Feld, um die Funktionalität zu aktivieren, die von InTune nicht unterstützt wird, aber in Ihrer VPN-Lösung verfügbar ist.</span><span class="sxs-lookup"><span data-stu-id="c1827-207">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="c1827-208">Wenden Sie sich an Ihren VPN-Anbieter, um zu erfahren, wie diese Schlüssel-Wert-Paare hinzugefügt werden.</span><span class="sxs-lookup"><span data-stu-id="c1827-208">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="c1827-209">Diese Auflistung kann maximal 25 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="c1827-209">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="c1827-210">Geerbt von [der applevpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c1827-210">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="c1827-211">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="c1827-211">enableSplitTunneling</span></span>|<span data-ttu-id="c1827-212">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c1827-212">Boolean</span></span>|<span data-ttu-id="c1827-213">Senden Sie den gesamten Netzwerkdatenverkehr über VPN.</span><span class="sxs-lookup"><span data-stu-id="c1827-213">Send all network traffic through VPN.</span></span> <span data-ttu-id="c1827-214">Geerbt von [der applevpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c1827-214">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="c1827-215">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="c1827-215">authenticationMethod</span></span>|[<span data-ttu-id="c1827-216">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="c1827-216">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="c1827-217">Authentifizierungsmethode für diese VPN-Verbindung.</span><span class="sxs-lookup"><span data-stu-id="c1827-217">Authentication method for this VPN connection.</span></span> <span data-ttu-id="c1827-218">Von [der applevpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="c1827-218">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="c1827-219">Mögliche Werte sind: `certificate` und `usernameAndPassword`.</span><span class="sxs-lookup"><span data-stu-id="c1827-219">Possible values are: `certificate`, `usernameAndPassword`.</span></span>|
|<span data-ttu-id="c1827-220">enablePerApp</span><span class="sxs-lookup"><span data-stu-id="c1827-220">enablePerApp</span></span>|<span data-ttu-id="c1827-221">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c1827-221">Boolean</span></span>|<span data-ttu-id="c1827-222">Wenn Sie dies auf true festlegen, wird eine pro-App-VPN-Nutzlast erstellt, die später apps zugeordnet werden kann, die diese VPN-Anschluss auf dem iOS-Gerät des Endbenutzers auslösen können.</span><span class="sxs-lookup"><span data-stu-id="c1827-222">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span> <span data-ttu-id="c1827-223">Geerbt von [der applevpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c1827-223">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="c1827-224">safariDomains</span><span class="sxs-lookup"><span data-stu-id="c1827-224">safariDomains</span></span>|<span data-ttu-id="c1827-225">String collection</span><span class="sxs-lookup"><span data-stu-id="c1827-225">String collection</span></span>|<span data-ttu-id="c1827-226">Safari-Domänen, wenn diese VPN-pro-app-Einstellung aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="c1827-226">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="c1827-227">Zusätzlich zu den apps, die mit diesem VPN verknüpft sind, können auch hier angegebene Safari-Domänen diese VPN-Verbindung auslösen.</span><span class="sxs-lookup"><span data-stu-id="c1827-227">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span> <span data-ttu-id="c1827-228">Geerbt von [der applevpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c1827-228">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="c1827-229">onDemandRules</span><span class="sxs-lookup"><span data-stu-id="c1827-229">onDemandRules</span></span>|<span data-ttu-id="c1827-230">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="c1827-230">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="c1827-231">Regeln für on-Demand.</span><span class="sxs-lookup"><span data-stu-id="c1827-231">On-Demand Rules.</span></span> <span data-ttu-id="c1827-232">Diese Sammlung darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="c1827-232">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="c1827-233">Geerbt von [der applevpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c1827-233">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="c1827-234">Sie</span><span class="sxs-lookup"><span data-stu-id="c1827-234">proxyServer</span></span>|[<span data-ttu-id="c1827-235">vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="c1827-235">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="c1827-236">Proxy Server.</span><span class="sxs-lookup"><span data-stu-id="c1827-236">Proxy Server.</span></span> <span data-ttu-id="c1827-237">Geerbt von [der applevpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c1827-237">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="c1827-238">optInToDeviceIdSharing</span><span class="sxs-lookup"><span data-stu-id="c1827-238">optInToDeviceIdSharing</span></span>|<span data-ttu-id="c1827-239">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c1827-239">Boolean</span></span>|<span data-ttu-id="c1827-240">Opt-in für die Freigabe der Geräte-ID an Drittanbieter-VPN-Clients für die Verwendung während der Überprüfung der Netzwerkzugriffssteuerung.</span><span class="sxs-lookup"><span data-stu-id="c1827-240">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span> <span data-ttu-id="c1827-241">Geerbt von [der applevpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c1827-241">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="c1827-242">providerType</span><span class="sxs-lookup"><span data-stu-id="c1827-242">providerType</span></span>|[<span data-ttu-id="c1827-243">vpnProviderType</span><span class="sxs-lookup"><span data-stu-id="c1827-243">vpnProviderType</span></span>](../resources/intune-deviceconfig-vpnprovidertype.md)|<span data-ttu-id="c1827-244">Anbietertyp für pro-App-VPN.</span><span class="sxs-lookup"><span data-stu-id="c1827-244">Provider type for per-app VPN.</span></span> <span data-ttu-id="c1827-245">Mögliche Werte sind: `notConfigured`, `appProxy` und `packetTunnel`.</span><span class="sxs-lookup"><span data-stu-id="c1827-245">Possible values are: `notConfigured`, `appProxy`, `packetTunnel`.</span></span>|
|<span data-ttu-id="c1827-246">User Domain</span><span class="sxs-lookup"><span data-stu-id="c1827-246">userDomain</span></span>|<span data-ttu-id="c1827-247">String</span><span class="sxs-lookup"><span data-stu-id="c1827-247">String</span></span>|<span data-ttu-id="c1827-248">Nur Zscaler.</span><span class="sxs-lookup"><span data-stu-id="c1827-248">Zscaler only.</span></span> <span data-ttu-id="c1827-249">Geben Sie in der Zscaler-App eine statische Domäne ein, in der das Anmeldefeld vorab aufgefüllt werden soll.</span><span class="sxs-lookup"><span data-stu-id="c1827-249">Enter a static domain to pre-populate the login field with in the Zscaler app.</span></span> <span data-ttu-id="c1827-250">Wenn dieser Wert leer bleibt, wird stattdessen die Azure Active Directory-Domäne des Benutzers verwendet.</span><span class="sxs-lookup"><span data-stu-id="c1827-250">If this is left empty, the user's Azure Active Directory domain will be used instead.</span></span>|
|<span data-ttu-id="c1827-251">strictEnforcement</span><span class="sxs-lookup"><span data-stu-id="c1827-251">strictEnforcement</span></span>|<span data-ttu-id="c1827-252">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c1827-252">Boolean</span></span>|<span data-ttu-id="c1827-253">Nur Zscaler.</span><span class="sxs-lookup"><span data-stu-id="c1827-253">Zscaler only.</span></span> <span data-ttu-id="c1827-254">Blockiert den Netzwerkdatenverkehr, bis sich der Benutzer bei der Zscaler-App anmeldet.</span><span class="sxs-lookup"><span data-stu-id="c1827-254">Blocks network traffic until the user signs into Zscaler app.</span></span> <span data-ttu-id="c1827-255">"True" bedeutet, dass der Datenverkehr blockiert ist.</span><span class="sxs-lookup"><span data-stu-id="c1827-255">"True" means traffic is blocked.</span></span>|
|<span data-ttu-id="c1827-256">cloudName</span><span class="sxs-lookup"><span data-stu-id="c1827-256">cloudName</span></span>|<span data-ttu-id="c1827-257">String</span><span class="sxs-lookup"><span data-stu-id="c1827-257">String</span></span>|<span data-ttu-id="c1827-258">Nur Zscaler.</span><span class="sxs-lookup"><span data-stu-id="c1827-258">Zscaler only.</span></span> <span data-ttu-id="c1827-259">Zscaler-Wolke, der der Benutzer zugewiesen ist.</span><span class="sxs-lookup"><span data-stu-id="c1827-259">Zscaler cloud which the user is assigned to.</span></span>|
|<span data-ttu-id="c1827-260">excludeList</span><span class="sxs-lookup"><span data-stu-id="c1827-260">excludeList</span></span>|<span data-ttu-id="c1827-261">String collection</span><span class="sxs-lookup"><span data-stu-id="c1827-261">String collection</span></span>|<span data-ttu-id="c1827-262">Nur Zscaler.</span><span class="sxs-lookup"><span data-stu-id="c1827-262">Zscaler only.</span></span> <span data-ttu-id="c1827-263">Liste der Netzwerkadressen, die nicht über die Zscaler-Cloud gesendet werden.</span><span class="sxs-lookup"><span data-stu-id="c1827-263">List of network addresses which are not sent through the Zscaler cloud.</span></span>|



## <a name="response"></a><span data-ttu-id="c1827-264">Antwort</span><span class="sxs-lookup"><span data-stu-id="c1827-264">Response</span></span>
<span data-ttu-id="c1827-265">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="c1827-265">If successful, this method returns a `200 OK` response code and an updated [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c1827-266">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c1827-266">Example</span></span>

### <a name="request"></a><span data-ttu-id="c1827-267">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c1827-267">Request</span></span>
<span data-ttu-id="c1827-268">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c1827-268">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 2042

{
  "@odata.type": "#microsoft.graph.iosVpnConfiguration",
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

### <a name="response"></a><span data-ttu-id="c1827-269">Antwort</span><span class="sxs-lookup"><span data-stu-id="c1827-269">Response</span></span>
<span data-ttu-id="c1827-p131">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c1827-p131">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




