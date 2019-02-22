---
title: MacOSVpnConfiguration aktualisieren
description: Aktualisieren der Eigenschaften eines macOSVpnConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 73fecc7200c6172b8edd22922d9d4a573659b9a2
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30156112"
---
# <a name="update-macosvpnconfiguration"></a><span data-ttu-id="00caa-103">MacOSVpnConfiguration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="00caa-103">Update macOSVpnConfiguration</span></span>

> <span data-ttu-id="00caa-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="00caa-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="00caa-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="00caa-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="00caa-106">Aktualisieren der Eigenschaften eines [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="00caa-106">Update the properties of a [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="00caa-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="00caa-107">Prerequisites</span></span>
<span data-ttu-id="00caa-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="00caa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="00caa-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="00caa-110">Permission type</span></span>|<span data-ttu-id="00caa-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="00caa-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="00caa-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="00caa-112">Delegated (work or school account)</span></span>|<span data-ttu-id="00caa-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00caa-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="00caa-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="00caa-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="00caa-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="00caa-115">Not supported.</span></span>|
|<span data-ttu-id="00caa-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="00caa-116">Application</span></span>|<span data-ttu-id="00caa-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="00caa-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="00caa-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="00caa-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="00caa-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="00caa-119">Request headers</span></span>
|<span data-ttu-id="00caa-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="00caa-120">Header</span></span>|<span data-ttu-id="00caa-121">Wert</span><span class="sxs-lookup"><span data-stu-id="00caa-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="00caa-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="00caa-122">Authorization</span></span>|<span data-ttu-id="00caa-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="00caa-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="00caa-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="00caa-124">Accept</span></span>|<span data-ttu-id="00caa-125">application/json</span><span class="sxs-lookup"><span data-stu-id="00caa-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="00caa-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="00caa-126">Request body</span></span>
<span data-ttu-id="00caa-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="00caa-127">In the request body, supply a JSON representation for the [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) object.</span></span>

<span data-ttu-id="00caa-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="00caa-128">The following table shows the properties that are required when you create the [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md).</span></span>

|<span data-ttu-id="00caa-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="00caa-129">Property</span></span>|<span data-ttu-id="00caa-130">Typ</span><span class="sxs-lookup"><span data-stu-id="00caa-130">Type</span></span>|<span data-ttu-id="00caa-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="00caa-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="00caa-132">id</span><span class="sxs-lookup"><span data-stu-id="00caa-132">id</span></span>|<span data-ttu-id="00caa-133">string</span><span class="sxs-lookup"><span data-stu-id="00caa-133">String</span></span>|<span data-ttu-id="00caa-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="00caa-134">Key of the entity.</span></span> <span data-ttu-id="00caa-135">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="00caa-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="00caa-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="00caa-136">lastModifiedDateTime</span></span>|<span data-ttu-id="00caa-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="00caa-137">DateTimeOffset</span></span>|<span data-ttu-id="00caa-138">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="00caa-138">DateTime the object was last modified.</span></span> <span data-ttu-id="00caa-139">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="00caa-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="00caa-140">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="00caa-140">roleScopeTagIds</span></span>|<span data-ttu-id="00caa-141">String collection</span><span class="sxs-lookup"><span data-stu-id="00caa-141">String collection</span></span>|<span data-ttu-id="00caa-142">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="00caa-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="00caa-143">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="00caa-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="00caa-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="00caa-144">supportsScopeTags</span></span>|<span data-ttu-id="00caa-145">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="00caa-145">Boolean</span></span>|<span data-ttu-id="00caa-146">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereichs Tags unterstützt.</span><span class="sxs-lookup"><span data-stu-id="00caa-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="00caa-147">Das Zuweisen zur ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert auf false festgelegt ist und Entitäten für bereichsbezogene Benutzer nicht sichtbar sind.</span><span class="sxs-lookup"><span data-stu-id="00caa-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="00caa-148">Dies geschieht für in Silverlight erstellte Legacy Richtlinien und kann durch Löschen und erneutes Erstellen der Richtlinie im Azure-Portal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="00caa-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="00caa-149">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="00caa-149">This property is read-only.</span></span> <span data-ttu-id="00caa-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="00caa-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="00caa-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="00caa-151">createdDateTime</span></span>|<span data-ttu-id="00caa-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="00caa-152">DateTimeOffset</span></span>|<span data-ttu-id="00caa-153">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="00caa-153">DateTime the object was created.</span></span> <span data-ttu-id="00caa-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="00caa-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="00caa-155">description</span><span class="sxs-lookup"><span data-stu-id="00caa-155">description</span></span>|<span data-ttu-id="00caa-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="00caa-156">String</span></span>|<span data-ttu-id="00caa-157">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="00caa-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="00caa-158">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="00caa-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="00caa-159">displayName</span><span class="sxs-lookup"><span data-stu-id="00caa-159">displayName</span></span>|<span data-ttu-id="00caa-160">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="00caa-160">String</span></span>|<span data-ttu-id="00caa-161">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="00caa-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="00caa-162">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="00caa-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="00caa-163">Version</span><span class="sxs-lookup"><span data-stu-id="00caa-163">version</span></span>|<span data-ttu-id="00caa-164">Int32</span><span class="sxs-lookup"><span data-stu-id="00caa-164">Int32</span></span>|<span data-ttu-id="00caa-165">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="00caa-165">Version of the device configuration.</span></span> <span data-ttu-id="00caa-166">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="00caa-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="00caa-167">connectionName</span><span class="sxs-lookup"><span data-stu-id="00caa-167">connectionName</span></span>|<span data-ttu-id="00caa-168">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="00caa-168">String</span></span>|<span data-ttu-id="00caa-169">Dem Benutzer angezeigter Verbindungsname.</span><span class="sxs-lookup"><span data-stu-id="00caa-169">Connection name displayed to the user.</span></span> <span data-ttu-id="00caa-170">Geerbt von [der applevpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="00caa-170">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="00caa-171">connectionType</span><span class="sxs-lookup"><span data-stu-id="00caa-171">connectionType</span></span>|[<span data-ttu-id="00caa-172">appleVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="00caa-172">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="00caa-173">Verbindungstyp.</span><span class="sxs-lookup"><span data-stu-id="00caa-173">Connection type.</span></span> <span data-ttu-id="00caa-174">Von [der applevpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="00caa-174">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="00caa-175">Mögliche Werte sind: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient` `dellSonicWallMobileConnect` `checkPointCapsuleVpn`,,, `customVpn`, `ciscoIPSec` `citrix`,, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess` `f5Access2018` `citrixSso`,,, `paloAltoGlobalProtectV2`.</span><span class="sxs-lookup"><span data-stu-id="00caa-175">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`.</span></span>|
|<span data-ttu-id="00caa-176">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="00caa-176">loginGroupOrDomain</span></span>|<span data-ttu-id="00caa-177">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="00caa-177">String</span></span>|<span data-ttu-id="00caa-178">Anmeldegruppe oder Domäne, wenn der Verbindungstyp auf Dell SonicWALL Mobile Connection festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="00caa-178">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="00caa-179">Geerbt von [der applevpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="00caa-179">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="00caa-180">role</span><span class="sxs-lookup"><span data-stu-id="00caa-180">role</span></span>|<span data-ttu-id="00caa-181">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="00caa-181">String</span></span>|<span data-ttu-id="00caa-182">Role, wenn der Verbindungstyp auf Pulse Secure festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="00caa-182">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="00caa-183">Geerbt von [der applevpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="00caa-183">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="00caa-184">Bereich</span><span class="sxs-lookup"><span data-stu-id="00caa-184">realm</span></span>|<span data-ttu-id="00caa-185">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="00caa-185">String</span></span>|<span data-ttu-id="00caa-186">Bereich, wenn der Verbindungstyp auf Pulse Secure festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="00caa-186">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="00caa-187">Geerbt von [der applevpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="00caa-187">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="00caa-188">Server</span><span class="sxs-lookup"><span data-stu-id="00caa-188">server</span></span>|[<span data-ttu-id="00caa-189">vpnServer</span><span class="sxs-lookup"><span data-stu-id="00caa-189">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="00caa-190">VPN-Server im Netzwerk.</span><span class="sxs-lookup"><span data-stu-id="00caa-190">VPN Server on the network.</span></span> <span data-ttu-id="00caa-191">Stellen Sie sicher, dass Endbenutzer auf diesen Netzwerkspeicherort zugreifen können.</span><span class="sxs-lookup"><span data-stu-id="00caa-191">Make sure end users can access this network location.</span></span> <span data-ttu-id="00caa-192">Geerbt von [der applevpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="00caa-192">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="00caa-193">Bezeichner</span><span class="sxs-lookup"><span data-stu-id="00caa-193">identifier</span></span>|<span data-ttu-id="00caa-194">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="00caa-194">String</span></span>|<span data-ttu-id="00caa-195">Vom VPN-Anbieter bereitgestellter Bezeichner, wenn der Verbindungstyp auf benutzerdefiniertes VPN festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="00caa-195">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="00caa-196">Beispiel: Cisco AnyConnect verwendet einen Bezeichner des Formulars "com. Cisco. AnyConnect. applevpn. Plugin", geerbt von [der applevpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="00caa-196">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="00caa-197">customData</span><span class="sxs-lookup"><span data-stu-id="00caa-197">customData</span></span>|<span data-ttu-id="00caa-198">[keyValue](../resources/intune-deviceconfig-keyvalue.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="00caa-198">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="00caa-199">Benutzerdefinierte Daten, wenn der Verbindungstyp auf benutzerdefiniertes VPN festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="00caa-199">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="00caa-200">Verwenden Sie dieses Feld, um die Funktionalität zu aktivieren, die von InTune nicht unterstützt wird, aber in Ihrer VPN-Lösung verfügbar ist.</span><span class="sxs-lookup"><span data-stu-id="00caa-200">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="00caa-201">Wenden Sie sich an Ihren VPN-Anbieter, um zu erfahren, wie diese Schlüssel-Wert-Paare hinzugefügt werden.</span><span class="sxs-lookup"><span data-stu-id="00caa-201">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="00caa-202">Diese Auflistung kann maximal 25 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="00caa-202">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="00caa-203">Geerbt von [der applevpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="00caa-203">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="00caa-204">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="00caa-204">customKeyValueData</span></span>|<span data-ttu-id="00caa-205">[keyValuePair](../resources/intune-shared-keyvaluepair.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="00caa-205">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="00caa-206">Benutzerdefinierte Daten, wenn der Verbindungstyp auf benutzerdefiniertes VPN festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="00caa-206">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="00caa-207">Verwenden Sie dieses Feld, um die Funktionalität zu aktivieren, die von InTune nicht unterstützt wird, aber in Ihrer VPN-Lösung verfügbar ist.</span><span class="sxs-lookup"><span data-stu-id="00caa-207">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="00caa-208">Wenden Sie sich an Ihren VPN-Anbieter, um zu erfahren, wie diese Schlüssel-Wert-Paare hinzugefügt werden.</span><span class="sxs-lookup"><span data-stu-id="00caa-208">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="00caa-209">Diese Auflistung kann maximal 25 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="00caa-209">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="00caa-210">Geerbt von [der applevpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="00caa-210">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="00caa-211">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="00caa-211">enableSplitTunneling</span></span>|<span data-ttu-id="00caa-212">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="00caa-212">Boolean</span></span>|<span data-ttu-id="00caa-213">Senden Sie den gesamten Netzwerkdatenverkehr über VPN.</span><span class="sxs-lookup"><span data-stu-id="00caa-213">Send all network traffic through VPN.</span></span> <span data-ttu-id="00caa-214">Geerbt von [der applevpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="00caa-214">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="00caa-215">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="00caa-215">authenticationMethod</span></span>|[<span data-ttu-id="00caa-216">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="00caa-216">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="00caa-217">Authentifizierungsmethode für diese VPN-Verbindung.</span><span class="sxs-lookup"><span data-stu-id="00caa-217">Authentication method for this VPN connection.</span></span> <span data-ttu-id="00caa-218">Von [der applevpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="00caa-218">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="00caa-219">Mögliche Werte sind: `certificate` und `usernameAndPassword`.</span><span class="sxs-lookup"><span data-stu-id="00caa-219">Possible values are: `certificate`, `usernameAndPassword`.</span></span>|
|<span data-ttu-id="00caa-220">enablePerApp</span><span class="sxs-lookup"><span data-stu-id="00caa-220">enablePerApp</span></span>|<span data-ttu-id="00caa-221">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="00caa-221">Boolean</span></span>|<span data-ttu-id="00caa-222">Wenn Sie dies auf true festlegen, wird eine pro-App-VPN-Nutzlast erstellt, die später apps zugeordnet werden kann, die diese VPN-Anschluss auf dem iOS-Gerät des Endbenutzers auslösen können.</span><span class="sxs-lookup"><span data-stu-id="00caa-222">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span> <span data-ttu-id="00caa-223">Geerbt von [der applevpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="00caa-223">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="00caa-224">safariDomains</span><span class="sxs-lookup"><span data-stu-id="00caa-224">safariDomains</span></span>|<span data-ttu-id="00caa-225">String collection</span><span class="sxs-lookup"><span data-stu-id="00caa-225">String collection</span></span>|<span data-ttu-id="00caa-226">Safari-Domänen, wenn diese VPN-pro-app-Einstellung aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="00caa-226">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="00caa-227">Zusätzlich zu den apps, die mit diesem VPN verknüpft sind, können auch hier angegebene Safari-Domänen diese VPN-Verbindung auslösen.</span><span class="sxs-lookup"><span data-stu-id="00caa-227">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span> <span data-ttu-id="00caa-228">Geerbt von [der applevpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="00caa-228">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="00caa-229">onDemandRules</span><span class="sxs-lookup"><span data-stu-id="00caa-229">onDemandRules</span></span>|<span data-ttu-id="00caa-230">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="00caa-230">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="00caa-231">Regeln für on-Demand.</span><span class="sxs-lookup"><span data-stu-id="00caa-231">On-Demand Rules.</span></span> <span data-ttu-id="00caa-232">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="00caa-232">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="00caa-233">Geerbt von [der applevpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="00caa-233">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="00caa-234">Sie</span><span class="sxs-lookup"><span data-stu-id="00caa-234">proxyServer</span></span>|[<span data-ttu-id="00caa-235">vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="00caa-235">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="00caa-236">Proxy Server.</span><span class="sxs-lookup"><span data-stu-id="00caa-236">Proxy Server.</span></span> <span data-ttu-id="00caa-237">Geerbt von [der applevpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="00caa-237">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="00caa-238">optInToDeviceIdSharing</span><span class="sxs-lookup"><span data-stu-id="00caa-238">optInToDeviceIdSharing</span></span>|<span data-ttu-id="00caa-239">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="00caa-239">Boolean</span></span>|<span data-ttu-id="00caa-240">Opt-in für die Freigabe der Geräte-ID an Drittanbieter-VPN-Clients für die Verwendung während der Überprüfung der Netzwerkzugriffssteuerung.</span><span class="sxs-lookup"><span data-stu-id="00caa-240">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span> <span data-ttu-id="00caa-241">Geerbt von [der applevpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="00caa-241">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="00caa-242">Antwort</span><span class="sxs-lookup"><span data-stu-id="00caa-242">Response</span></span>
<span data-ttu-id="00caa-243">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="00caa-243">If successful, this method returns a `200 OK` response code and an updated [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="00caa-244">Beispiel</span><span class="sxs-lookup"><span data-stu-id="00caa-244">Example</span></span>

### <a name="request"></a><span data-ttu-id="00caa-245">Anforderung</span><span class="sxs-lookup"><span data-stu-id="00caa-245">Request</span></span>
<span data-ttu-id="00caa-246">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="00caa-246">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1857

{
  "@odata.type": "#microsoft.graph.macOSVpnConfiguration",
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

### <a name="response"></a><span data-ttu-id="00caa-247">Antwort</span><span class="sxs-lookup"><span data-stu-id="00caa-247">Response</span></span>
<span data-ttu-id="00caa-p126">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="00caa-p126">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




