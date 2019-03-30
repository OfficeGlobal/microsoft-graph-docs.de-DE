---
title: IosVpnConfiguration erstellen
description: Erstellen eines neuen iosVpnConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e220b2a41ce61ae71343b2754993c6b5082f352e
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30985872"
---
# <a name="create-iosvpnconfiguration"></a><span data-ttu-id="cda0b-103">IosVpnConfiguration erstellen</span><span class="sxs-lookup"><span data-stu-id="cda0b-103">Create iosVpnConfiguration</span></span>

> <span data-ttu-id="cda0b-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="cda0b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cda0b-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="cda0b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cda0b-106">Erstellen eines neuen [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="cda0b-106">Create a new [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cda0b-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="cda0b-107">Prerequisites</span></span>
<span data-ttu-id="cda0b-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cda0b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cda0b-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="cda0b-110">Permission type</span></span>|<span data-ttu-id="cda0b-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="cda0b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cda0b-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="cda0b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cda0b-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cda0b-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="cda0b-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="cda0b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cda0b-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cda0b-115">Not supported.</span></span>|
|<span data-ttu-id="cda0b-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="cda0b-116">Application</span></span>|<span data-ttu-id="cda0b-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cda0b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cda0b-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="cda0b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="cda0b-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="cda0b-119">Request headers</span></span>
|<span data-ttu-id="cda0b-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="cda0b-120">Header</span></span>|<span data-ttu-id="cda0b-121">Wert</span><span class="sxs-lookup"><span data-stu-id="cda0b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cda0b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="cda0b-122">Authorization</span></span>|<span data-ttu-id="cda0b-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="cda0b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cda0b-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="cda0b-124">Accept</span></span>|<span data-ttu-id="cda0b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="cda0b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cda0b-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="cda0b-126">Request body</span></span>
<span data-ttu-id="cda0b-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das iosVpnConfiguration-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="cda0b-127">In the request body, supply a JSON representation for the iosVpnConfiguration object.</span></span>

<span data-ttu-id="cda0b-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der iosVpnConfiguration erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="cda0b-128">The following table shows the properties that are required when you create the iosVpnConfiguration.</span></span>

|<span data-ttu-id="cda0b-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="cda0b-129">Property</span></span>|<span data-ttu-id="cda0b-130">Typ</span><span class="sxs-lookup"><span data-stu-id="cda0b-130">Type</span></span>|<span data-ttu-id="cda0b-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cda0b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cda0b-132">id</span><span class="sxs-lookup"><span data-stu-id="cda0b-132">id</span></span>|<span data-ttu-id="cda0b-133">String</span><span class="sxs-lookup"><span data-stu-id="cda0b-133">String</span></span>|<span data-ttu-id="cda0b-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="cda0b-134">Key of the entity.</span></span> <span data-ttu-id="cda0b-135">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cda0b-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cda0b-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cda0b-136">lastModifiedDateTime</span></span>|<span data-ttu-id="cda0b-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cda0b-137">DateTimeOffset</span></span>|<span data-ttu-id="cda0b-138">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="cda0b-138">DateTime the object was last modified.</span></span> <span data-ttu-id="cda0b-139">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cda0b-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cda0b-140">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="cda0b-140">roleScopeTagIds</span></span>|<span data-ttu-id="cda0b-141">String collection</span><span class="sxs-lookup"><span data-stu-id="cda0b-141">String collection</span></span>|<span data-ttu-id="cda0b-142">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="cda0b-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="cda0b-143">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cda0b-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cda0b-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="cda0b-144">supportsScopeTags</span></span>|<span data-ttu-id="cda0b-145">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="cda0b-145">Boolean</span></span>|<span data-ttu-id="cda0b-146">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereichs Tags unterstützt.</span><span class="sxs-lookup"><span data-stu-id="cda0b-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="cda0b-147">Das Zuweisen zur ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert auf false festgelegt ist und Entitäten für bereichsbezogene Benutzer nicht sichtbar sind.</span><span class="sxs-lookup"><span data-stu-id="cda0b-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="cda0b-148">Dies geschieht für in Silverlight erstellte Legacy Richtlinien und kann durch Löschen und erneutes Erstellen der Richtlinie im Azure-Portal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="cda0b-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="cda0b-149">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="cda0b-149">This property is read-only.</span></span> <span data-ttu-id="cda0b-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cda0b-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cda0b-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cda0b-151">createdDateTime</span></span>|<span data-ttu-id="cda0b-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cda0b-152">DateTimeOffset</span></span>|<span data-ttu-id="cda0b-153">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="cda0b-153">DateTime the object was created.</span></span> <span data-ttu-id="cda0b-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cda0b-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cda0b-155">description</span><span class="sxs-lookup"><span data-stu-id="cda0b-155">description</span></span>|<span data-ttu-id="cda0b-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="cda0b-156">String</span></span>|<span data-ttu-id="cda0b-157">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="cda0b-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="cda0b-158">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cda0b-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cda0b-159">displayName</span><span class="sxs-lookup"><span data-stu-id="cda0b-159">displayName</span></span>|<span data-ttu-id="cda0b-160">String</span><span class="sxs-lookup"><span data-stu-id="cda0b-160">String</span></span>|<span data-ttu-id="cda0b-161">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="cda0b-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="cda0b-162">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cda0b-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cda0b-163">Version</span><span class="sxs-lookup"><span data-stu-id="cda0b-163">version</span></span>|<span data-ttu-id="cda0b-164">Int32</span><span class="sxs-lookup"><span data-stu-id="cda0b-164">Int32</span></span>|<span data-ttu-id="cda0b-165">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="cda0b-165">Version of the device configuration.</span></span> <span data-ttu-id="cda0b-166">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cda0b-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cda0b-167">connectionName</span><span class="sxs-lookup"><span data-stu-id="cda0b-167">connectionName</span></span>|<span data-ttu-id="cda0b-168">String</span><span class="sxs-lookup"><span data-stu-id="cda0b-168">String</span></span>|<span data-ttu-id="cda0b-169">Dem Benutzer angezeigter Verbindungsname.</span><span class="sxs-lookup"><span data-stu-id="cda0b-169">Connection name displayed to the user.</span></span> <span data-ttu-id="cda0b-170">Geerbt von [der applevpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cda0b-170">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="cda0b-171">connectionType</span><span class="sxs-lookup"><span data-stu-id="cda0b-171">connectionType</span></span>|[<span data-ttu-id="cda0b-172">appleVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="cda0b-172">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="cda0b-173">Verbindungstyp.</span><span class="sxs-lookup"><span data-stu-id="cda0b-173">Connection type.</span></span> <span data-ttu-id="cda0b-174">Von [der applevpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="cda0b-174">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="cda0b-175">Mögliche Werte sind: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient` `dellSonicWallMobileConnect` `checkPointCapsuleVpn`,,, `customVpn`, `ciscoIPSec` `citrix`,, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess` `f5Access2018` `citrixSso`,,, `paloAltoGlobalProtectV2`.</span><span class="sxs-lookup"><span data-stu-id="cda0b-175">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`.</span></span>|
|<span data-ttu-id="cda0b-176">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="cda0b-176">loginGroupOrDomain</span></span>|<span data-ttu-id="cda0b-177">String</span><span class="sxs-lookup"><span data-stu-id="cda0b-177">String</span></span>|<span data-ttu-id="cda0b-178">Anmeldegruppe oder Domäne, wenn der Verbindungstyp auf Dell SonicWALL Mobile Connection festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="cda0b-178">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="cda0b-179">Geerbt von [der applevpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cda0b-179">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="cda0b-180">role</span><span class="sxs-lookup"><span data-stu-id="cda0b-180">role</span></span>|<span data-ttu-id="cda0b-181">String</span><span class="sxs-lookup"><span data-stu-id="cda0b-181">String</span></span>|<span data-ttu-id="cda0b-182">Role, wenn der Verbindungstyp auf Pulse Secure festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="cda0b-182">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="cda0b-183">Geerbt von [der applevpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cda0b-183">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="cda0b-184">Reich</span><span class="sxs-lookup"><span data-stu-id="cda0b-184">realm</span></span>|<span data-ttu-id="cda0b-185">String</span><span class="sxs-lookup"><span data-stu-id="cda0b-185">String</span></span>|<span data-ttu-id="cda0b-186">Bereich, wenn der Verbindungstyp auf Pulse Secure festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="cda0b-186">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="cda0b-187">Geerbt von [der applevpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cda0b-187">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="cda0b-188">Server</span><span class="sxs-lookup"><span data-stu-id="cda0b-188">server</span></span>|[<span data-ttu-id="cda0b-189">vpnServer</span><span class="sxs-lookup"><span data-stu-id="cda0b-189">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="cda0b-190">VPN-Server im Netzwerk.</span><span class="sxs-lookup"><span data-stu-id="cda0b-190">VPN Server on the network.</span></span> <span data-ttu-id="cda0b-191">Stellen Sie sicher, dass Endbenutzer auf diesen Netzwerkspeicherort zugreifen können.</span><span class="sxs-lookup"><span data-stu-id="cda0b-191">Make sure end users can access this network location.</span></span> <span data-ttu-id="cda0b-192">Geerbt von [der applevpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cda0b-192">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="cda0b-193">Bezeichner</span><span class="sxs-lookup"><span data-stu-id="cda0b-193">identifier</span></span>|<span data-ttu-id="cda0b-194">String</span><span class="sxs-lookup"><span data-stu-id="cda0b-194">String</span></span>|<span data-ttu-id="cda0b-195">Vom VPN-Anbieter bereitgestellter Bezeichner, wenn der Verbindungstyp auf benutzerdefiniertes VPN festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="cda0b-195">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="cda0b-196">Beispiel: Cisco AnyConnect verwendet einen Bezeichner des Formulars "com. Cisco. AnyConnect. applevpn. Plugin", geerbt von [der applevpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cda0b-196">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="cda0b-197">customData</span><span class="sxs-lookup"><span data-stu-id="cda0b-197">customData</span></span>|<span data-ttu-id="cda0b-198">[keyValue](../resources/intune-deviceconfig-keyvalue.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="cda0b-198">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="cda0b-199">Benutzerdefinierte Daten, wenn der Verbindungstyp auf benutzerdefiniertes VPN festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="cda0b-199">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="cda0b-200">Verwenden Sie dieses Feld, um die Funktionalität zu aktivieren, die von InTune nicht unterstützt wird, aber in Ihrer VPN-Lösung verfügbar ist.</span><span class="sxs-lookup"><span data-stu-id="cda0b-200">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="cda0b-201">Wenden Sie sich an Ihren VPN-Anbieter, um zu erfahren, wie diese Schlüssel-Wert-Paare hinzugefügt werden.</span><span class="sxs-lookup"><span data-stu-id="cda0b-201">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="cda0b-202">Diese Auflistung kann maximal 25 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="cda0b-202">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="cda0b-203">Geerbt von [der applevpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cda0b-203">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="cda0b-204">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="cda0b-204">customKeyValueData</span></span>|<span data-ttu-id="cda0b-205">[keyValuePair](../resources/intune-shared-keyvaluepair.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="cda0b-205">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="cda0b-206">Benutzerdefinierte Daten, wenn der Verbindungstyp auf benutzerdefiniertes VPN festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="cda0b-206">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="cda0b-207">Verwenden Sie dieses Feld, um die Funktionalität zu aktivieren, die von InTune nicht unterstützt wird, aber in Ihrer VPN-Lösung verfügbar ist.</span><span class="sxs-lookup"><span data-stu-id="cda0b-207">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="cda0b-208">Wenden Sie sich an Ihren VPN-Anbieter, um zu erfahren, wie diese Schlüssel-Wert-Paare hinzugefügt werden.</span><span class="sxs-lookup"><span data-stu-id="cda0b-208">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="cda0b-209">Diese Auflistung kann maximal 25 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="cda0b-209">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="cda0b-210">Geerbt von [der applevpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cda0b-210">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="cda0b-211">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="cda0b-211">enableSplitTunneling</span></span>|<span data-ttu-id="cda0b-212">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="cda0b-212">Boolean</span></span>|<span data-ttu-id="cda0b-213">Senden Sie den gesamten Netzwerkdatenverkehr über VPN.</span><span class="sxs-lookup"><span data-stu-id="cda0b-213">Send all network traffic through VPN.</span></span> <span data-ttu-id="cda0b-214">Geerbt von [der applevpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cda0b-214">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="cda0b-215">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="cda0b-215">authenticationMethod</span></span>|[<span data-ttu-id="cda0b-216">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="cda0b-216">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="cda0b-217">Authentifizierungsmethode für diese VPN-Verbindung.</span><span class="sxs-lookup"><span data-stu-id="cda0b-217">Authentication method for this VPN connection.</span></span> <span data-ttu-id="cda0b-218">Von [der applevpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="cda0b-218">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="cda0b-219">Mögliche Werte sind: `certificate` und `usernameAndPassword`.</span><span class="sxs-lookup"><span data-stu-id="cda0b-219">Possible values are: `certificate`, `usernameAndPassword`.</span></span>|
|<span data-ttu-id="cda0b-220">enablePerApp</span><span class="sxs-lookup"><span data-stu-id="cda0b-220">enablePerApp</span></span>|<span data-ttu-id="cda0b-221">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="cda0b-221">Boolean</span></span>|<span data-ttu-id="cda0b-222">Wenn Sie dies auf true festlegen, wird eine pro-App-VPN-Nutzlast erstellt, die später apps zugeordnet werden kann, die diese VPN-Anschluss auf dem iOS-Gerät des Endbenutzers auslösen können.</span><span class="sxs-lookup"><span data-stu-id="cda0b-222">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span> <span data-ttu-id="cda0b-223">Geerbt von [der applevpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cda0b-223">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="cda0b-224">safariDomains</span><span class="sxs-lookup"><span data-stu-id="cda0b-224">safariDomains</span></span>|<span data-ttu-id="cda0b-225">String collection</span><span class="sxs-lookup"><span data-stu-id="cda0b-225">String collection</span></span>|<span data-ttu-id="cda0b-226">Safari-Domänen, wenn diese VPN-pro-app-Einstellung aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="cda0b-226">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="cda0b-227">Zusätzlich zu den apps, die mit diesem VPN verknüpft sind, können auch hier angegebene Safari-Domänen diese VPN-Verbindung auslösen.</span><span class="sxs-lookup"><span data-stu-id="cda0b-227">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span> <span data-ttu-id="cda0b-228">Geerbt von [der applevpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cda0b-228">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="cda0b-229">onDemandRules</span><span class="sxs-lookup"><span data-stu-id="cda0b-229">onDemandRules</span></span>|<span data-ttu-id="cda0b-230">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="cda0b-230">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="cda0b-231">Regeln für on-Demand.</span><span class="sxs-lookup"><span data-stu-id="cda0b-231">On-Demand Rules.</span></span> <span data-ttu-id="cda0b-232">Diese Sammlung darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="cda0b-232">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="cda0b-233">Geerbt von [der applevpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cda0b-233">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="cda0b-234">Sie</span><span class="sxs-lookup"><span data-stu-id="cda0b-234">proxyServer</span></span>|[<span data-ttu-id="cda0b-235">vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="cda0b-235">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="cda0b-236">Proxy Server.</span><span class="sxs-lookup"><span data-stu-id="cda0b-236">Proxy Server.</span></span> <span data-ttu-id="cda0b-237">Geerbt von [der applevpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cda0b-237">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="cda0b-238">optInToDeviceIdSharing</span><span class="sxs-lookup"><span data-stu-id="cda0b-238">optInToDeviceIdSharing</span></span>|<span data-ttu-id="cda0b-239">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="cda0b-239">Boolean</span></span>|<span data-ttu-id="cda0b-240">Opt-in für die Freigabe der Geräte-ID an Drittanbieter-VPN-Clients für die Verwendung während der Überprüfung der Netzwerkzugriffssteuerung.</span><span class="sxs-lookup"><span data-stu-id="cda0b-240">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span> <span data-ttu-id="cda0b-241">Geerbt von [der applevpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cda0b-241">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="cda0b-242">providerType</span><span class="sxs-lookup"><span data-stu-id="cda0b-242">providerType</span></span>|[<span data-ttu-id="cda0b-243">vpnProviderType</span><span class="sxs-lookup"><span data-stu-id="cda0b-243">vpnProviderType</span></span>](../resources/intune-deviceconfig-vpnprovidertype.md)|<span data-ttu-id="cda0b-244">Anbietertyp für pro-App-VPN.</span><span class="sxs-lookup"><span data-stu-id="cda0b-244">Provider type for per-app VPN.</span></span> <span data-ttu-id="cda0b-245">Mögliche Werte sind: `notConfigured`, `appProxy` und `packetTunnel`.</span><span class="sxs-lookup"><span data-stu-id="cda0b-245">Possible values are: `notConfigured`, `appProxy`, `packetTunnel`.</span></span>|
|<span data-ttu-id="cda0b-246">User Domain</span><span class="sxs-lookup"><span data-stu-id="cda0b-246">userDomain</span></span>|<span data-ttu-id="cda0b-247">String</span><span class="sxs-lookup"><span data-stu-id="cda0b-247">String</span></span>|<span data-ttu-id="cda0b-248">Nur Zscaler.</span><span class="sxs-lookup"><span data-stu-id="cda0b-248">Zscaler only.</span></span> <span data-ttu-id="cda0b-249">Geben Sie in der Zscaler-App eine statische Domäne ein, in der das Anmeldefeld vorab aufgefüllt werden soll.</span><span class="sxs-lookup"><span data-stu-id="cda0b-249">Enter a static domain to pre-populate the login field with in the Zscaler app.</span></span> <span data-ttu-id="cda0b-250">Wenn dieser Wert leer bleibt, wird stattdessen die Azure Active Directory-Domäne des Benutzers verwendet.</span><span class="sxs-lookup"><span data-stu-id="cda0b-250">If this is left empty, the user's Azure Active Directory domain will be used instead.</span></span>|
|<span data-ttu-id="cda0b-251">strictEnforcement</span><span class="sxs-lookup"><span data-stu-id="cda0b-251">strictEnforcement</span></span>|<span data-ttu-id="cda0b-252">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="cda0b-252">Boolean</span></span>|<span data-ttu-id="cda0b-253">Nur Zscaler.</span><span class="sxs-lookup"><span data-stu-id="cda0b-253">Zscaler only.</span></span> <span data-ttu-id="cda0b-254">Blockiert den Netzwerkdatenverkehr, bis sich der Benutzer bei der Zscaler-App anmeldet.</span><span class="sxs-lookup"><span data-stu-id="cda0b-254">Blocks network traffic until the user signs into Zscaler app.</span></span> <span data-ttu-id="cda0b-255">"True" bedeutet, dass der Datenverkehr blockiert ist.</span><span class="sxs-lookup"><span data-stu-id="cda0b-255">"True" means traffic is blocked.</span></span>|
|<span data-ttu-id="cda0b-256">cloudName</span><span class="sxs-lookup"><span data-stu-id="cda0b-256">cloudName</span></span>|<span data-ttu-id="cda0b-257">String</span><span class="sxs-lookup"><span data-stu-id="cda0b-257">String</span></span>|<span data-ttu-id="cda0b-258">Nur Zscaler.</span><span class="sxs-lookup"><span data-stu-id="cda0b-258">Zscaler only.</span></span> <span data-ttu-id="cda0b-259">Zscaler-Wolke, der der Benutzer zugewiesen ist.</span><span class="sxs-lookup"><span data-stu-id="cda0b-259">Zscaler cloud which the user is assigned to.</span></span>|
|<span data-ttu-id="cda0b-260">excludeList</span><span class="sxs-lookup"><span data-stu-id="cda0b-260">excludeList</span></span>|<span data-ttu-id="cda0b-261">String collection</span><span class="sxs-lookup"><span data-stu-id="cda0b-261">String collection</span></span>|<span data-ttu-id="cda0b-262">Nur Zscaler.</span><span class="sxs-lookup"><span data-stu-id="cda0b-262">Zscaler only.</span></span> <span data-ttu-id="cda0b-263">Liste der Netzwerkadressen, die nicht über die Zscaler-Cloud gesendet werden.</span><span class="sxs-lookup"><span data-stu-id="cda0b-263">List of network addresses which are not sent through the Zscaler cloud.</span></span>|



## <a name="response"></a><span data-ttu-id="cda0b-264">Antwort</span><span class="sxs-lookup"><span data-stu-id="cda0b-264">Response</span></span>
<span data-ttu-id="cda0b-265">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="cda0b-265">If successful, this method returns a `201 Created` response code and a [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cda0b-266">Beispiel</span><span class="sxs-lookup"><span data-stu-id="cda0b-266">Example</span></span>

### <a name="request"></a><span data-ttu-id="cda0b-267">Anforderung</span><span class="sxs-lookup"><span data-stu-id="cda0b-267">Request</span></span>
<span data-ttu-id="cda0b-268">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="cda0b-268">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="cda0b-269">Antwort</span><span class="sxs-lookup"><span data-stu-id="cda0b-269">Response</span></span>
<span data-ttu-id="cda0b-p131">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cda0b-p131">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




