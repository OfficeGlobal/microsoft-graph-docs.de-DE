---
title: MacOSVpnConfiguration erstellen
description: Erstellen eines neuen macOSVpnConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2a9769bc59f69c5ed88679a7ead4e4bdd51840f6
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30970800"
---
# <a name="create-macosvpnconfiguration"></a><span data-ttu-id="d1edc-103">MacOSVpnConfiguration erstellen</span><span class="sxs-lookup"><span data-stu-id="d1edc-103">Create macOSVpnConfiguration</span></span>

> <span data-ttu-id="d1edc-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d1edc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d1edc-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="d1edc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d1edc-106">Erstellen eines neuen [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="d1edc-106">Create a new [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d1edc-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="d1edc-107">Prerequisites</span></span>
<span data-ttu-id="d1edc-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d1edc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d1edc-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d1edc-110">Permission type</span></span>|<span data-ttu-id="d1edc-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d1edc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d1edc-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d1edc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d1edc-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1edc-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d1edc-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d1edc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d1edc-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d1edc-115">Not supported.</span></span>|
|<span data-ttu-id="d1edc-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d1edc-116">Application</span></span>|<span data-ttu-id="d1edc-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d1edc-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d1edc-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d1edc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="d1edc-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d1edc-119">Request headers</span></span>
|<span data-ttu-id="d1edc-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="d1edc-120">Header</span></span>|<span data-ttu-id="d1edc-121">Wert</span><span class="sxs-lookup"><span data-stu-id="d1edc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d1edc-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d1edc-122">Authorization</span></span>|<span data-ttu-id="d1edc-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="d1edc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d1edc-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="d1edc-124">Accept</span></span>|<span data-ttu-id="d1edc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d1edc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d1edc-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d1edc-126">Request body</span></span>
<span data-ttu-id="d1edc-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das macOSVpnConfiguration-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="d1edc-127">In the request body, supply a JSON representation for the macOSVpnConfiguration object.</span></span>

<span data-ttu-id="d1edc-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der macOSVpnConfiguration erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="d1edc-128">The following table shows the properties that are required when you create the macOSVpnConfiguration.</span></span>

|<span data-ttu-id="d1edc-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d1edc-129">Property</span></span>|<span data-ttu-id="d1edc-130">Typ</span><span class="sxs-lookup"><span data-stu-id="d1edc-130">Type</span></span>|<span data-ttu-id="d1edc-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d1edc-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d1edc-132">id</span><span class="sxs-lookup"><span data-stu-id="d1edc-132">id</span></span>|<span data-ttu-id="d1edc-133">String</span><span class="sxs-lookup"><span data-stu-id="d1edc-133">String</span></span>|<span data-ttu-id="d1edc-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="d1edc-134">Key of the entity.</span></span> <span data-ttu-id="d1edc-135">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d1edc-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d1edc-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d1edc-136">lastModifiedDateTime</span></span>|<span data-ttu-id="d1edc-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d1edc-137">DateTimeOffset</span></span>|<span data-ttu-id="d1edc-138">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="d1edc-138">DateTime the object was last modified.</span></span> <span data-ttu-id="d1edc-139">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d1edc-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d1edc-140">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="d1edc-140">roleScopeTagIds</span></span>|<span data-ttu-id="d1edc-141">String collection</span><span class="sxs-lookup"><span data-stu-id="d1edc-141">String collection</span></span>|<span data-ttu-id="d1edc-142">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="d1edc-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d1edc-143">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d1edc-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d1edc-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="d1edc-144">supportsScopeTags</span></span>|<span data-ttu-id="d1edc-145">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d1edc-145">Boolean</span></span>|<span data-ttu-id="d1edc-146">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereichs Tags unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d1edc-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="d1edc-147">Das Zuweisen zur ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert auf false festgelegt ist und Entitäten für bereichsbezogene Benutzer nicht sichtbar sind.</span><span class="sxs-lookup"><span data-stu-id="d1edc-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="d1edc-148">Dies geschieht für in Silverlight erstellte Legacy Richtlinien und kann durch Löschen und erneutes Erstellen der Richtlinie im Azure-Portal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="d1edc-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="d1edc-149">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d1edc-149">This property is read-only.</span></span> <span data-ttu-id="d1edc-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d1edc-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d1edc-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d1edc-151">createdDateTime</span></span>|<span data-ttu-id="d1edc-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d1edc-152">DateTimeOffset</span></span>|<span data-ttu-id="d1edc-153">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="d1edc-153">DateTime the object was created.</span></span> <span data-ttu-id="d1edc-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d1edc-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d1edc-155">description</span><span class="sxs-lookup"><span data-stu-id="d1edc-155">description</span></span>|<span data-ttu-id="d1edc-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d1edc-156">String</span></span>|<span data-ttu-id="d1edc-157">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="d1edc-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d1edc-158">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d1edc-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d1edc-159">displayName</span><span class="sxs-lookup"><span data-stu-id="d1edc-159">displayName</span></span>|<span data-ttu-id="d1edc-160">String</span><span class="sxs-lookup"><span data-stu-id="d1edc-160">String</span></span>|<span data-ttu-id="d1edc-161">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="d1edc-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d1edc-162">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d1edc-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d1edc-163">Version</span><span class="sxs-lookup"><span data-stu-id="d1edc-163">version</span></span>|<span data-ttu-id="d1edc-164">Int32</span><span class="sxs-lookup"><span data-stu-id="d1edc-164">Int32</span></span>|<span data-ttu-id="d1edc-165">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="d1edc-165">Version of the device configuration.</span></span> <span data-ttu-id="d1edc-166">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d1edc-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d1edc-167">connectionName</span><span class="sxs-lookup"><span data-stu-id="d1edc-167">connectionName</span></span>|<span data-ttu-id="d1edc-168">String</span><span class="sxs-lookup"><span data-stu-id="d1edc-168">String</span></span>|<span data-ttu-id="d1edc-169">Dem Benutzer angezeigter Verbindungsname.</span><span class="sxs-lookup"><span data-stu-id="d1edc-169">Connection name displayed to the user.</span></span> <span data-ttu-id="d1edc-170">Geerbt von [der applevpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1edc-170">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="d1edc-171">connectionType</span><span class="sxs-lookup"><span data-stu-id="d1edc-171">connectionType</span></span>|[<span data-ttu-id="d1edc-172">appleVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="d1edc-172">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="d1edc-173">Verbindungstyp.</span><span class="sxs-lookup"><span data-stu-id="d1edc-173">Connection type.</span></span> <span data-ttu-id="d1edc-174">Von [der applevpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="d1edc-174">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="d1edc-175">Mögliche Werte sind: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient` `dellSonicWallMobileConnect` `checkPointCapsuleVpn`,,, `customVpn`, `ciscoIPSec` `citrix`,, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess` `f5Access2018` `citrixSso`,,, `paloAltoGlobalProtectV2`.</span><span class="sxs-lookup"><span data-stu-id="d1edc-175">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`.</span></span>|
|<span data-ttu-id="d1edc-176">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="d1edc-176">loginGroupOrDomain</span></span>|<span data-ttu-id="d1edc-177">String</span><span class="sxs-lookup"><span data-stu-id="d1edc-177">String</span></span>|<span data-ttu-id="d1edc-178">Anmeldegruppe oder Domäne, wenn der Verbindungstyp auf Dell SonicWALL Mobile Connection festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="d1edc-178">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="d1edc-179">Geerbt von [der applevpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1edc-179">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="d1edc-180">role</span><span class="sxs-lookup"><span data-stu-id="d1edc-180">role</span></span>|<span data-ttu-id="d1edc-181">String</span><span class="sxs-lookup"><span data-stu-id="d1edc-181">String</span></span>|<span data-ttu-id="d1edc-182">Role, wenn der Verbindungstyp auf Pulse Secure festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="d1edc-182">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="d1edc-183">Geerbt von [der applevpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1edc-183">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="d1edc-184">Reich</span><span class="sxs-lookup"><span data-stu-id="d1edc-184">realm</span></span>|<span data-ttu-id="d1edc-185">String</span><span class="sxs-lookup"><span data-stu-id="d1edc-185">String</span></span>|<span data-ttu-id="d1edc-186">Bereich, wenn der Verbindungstyp auf Pulse Secure festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="d1edc-186">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="d1edc-187">Geerbt von [der applevpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1edc-187">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="d1edc-188">Server</span><span class="sxs-lookup"><span data-stu-id="d1edc-188">server</span></span>|[<span data-ttu-id="d1edc-189">vpnServer</span><span class="sxs-lookup"><span data-stu-id="d1edc-189">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="d1edc-190">VPN-Server im Netzwerk.</span><span class="sxs-lookup"><span data-stu-id="d1edc-190">VPN Server on the network.</span></span> <span data-ttu-id="d1edc-191">Stellen Sie sicher, dass Endbenutzer auf diesen Netzwerkspeicherort zugreifen können.</span><span class="sxs-lookup"><span data-stu-id="d1edc-191">Make sure end users can access this network location.</span></span> <span data-ttu-id="d1edc-192">Geerbt von [der applevpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1edc-192">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="d1edc-193">Bezeichner</span><span class="sxs-lookup"><span data-stu-id="d1edc-193">identifier</span></span>|<span data-ttu-id="d1edc-194">String</span><span class="sxs-lookup"><span data-stu-id="d1edc-194">String</span></span>|<span data-ttu-id="d1edc-195">Vom VPN-Anbieter bereitgestellter Bezeichner, wenn der Verbindungstyp auf benutzerdefiniertes VPN festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="d1edc-195">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="d1edc-196">Beispiel: Cisco AnyConnect verwendet einen Bezeichner des Formulars "com. Cisco. AnyConnect. applevpn. Plugin", geerbt von [der applevpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1edc-196">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="d1edc-197">customData</span><span class="sxs-lookup"><span data-stu-id="d1edc-197">customData</span></span>|<span data-ttu-id="d1edc-198">[keyValue](../resources/intune-deviceconfig-keyvalue.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="d1edc-198">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="d1edc-199">Benutzerdefinierte Daten, wenn der Verbindungstyp auf benutzerdefiniertes VPN festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="d1edc-199">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="d1edc-200">Verwenden Sie dieses Feld, um die Funktionalität zu aktivieren, die von InTune nicht unterstützt wird, aber in Ihrer VPN-Lösung verfügbar ist.</span><span class="sxs-lookup"><span data-stu-id="d1edc-200">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="d1edc-201">Wenden Sie sich an Ihren VPN-Anbieter, um zu erfahren, wie diese Schlüssel-Wert-Paare hinzugefügt werden.</span><span class="sxs-lookup"><span data-stu-id="d1edc-201">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="d1edc-202">Diese Auflistung kann maximal 25 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="d1edc-202">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="d1edc-203">Geerbt von [der applevpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1edc-203">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="d1edc-204">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="d1edc-204">customKeyValueData</span></span>|<span data-ttu-id="d1edc-205">[keyValuePair](../resources/intune-shared-keyvaluepair.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="d1edc-205">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="d1edc-206">Benutzerdefinierte Daten, wenn der Verbindungstyp auf benutzerdefiniertes VPN festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="d1edc-206">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="d1edc-207">Verwenden Sie dieses Feld, um die Funktionalität zu aktivieren, die von InTune nicht unterstützt wird, aber in Ihrer VPN-Lösung verfügbar ist.</span><span class="sxs-lookup"><span data-stu-id="d1edc-207">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="d1edc-208">Wenden Sie sich an Ihren VPN-Anbieter, um zu erfahren, wie diese Schlüssel-Wert-Paare hinzugefügt werden.</span><span class="sxs-lookup"><span data-stu-id="d1edc-208">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="d1edc-209">Diese Auflistung kann maximal 25 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="d1edc-209">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="d1edc-210">Geerbt von [der applevpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1edc-210">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="d1edc-211">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="d1edc-211">enableSplitTunneling</span></span>|<span data-ttu-id="d1edc-212">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d1edc-212">Boolean</span></span>|<span data-ttu-id="d1edc-213">Senden Sie den gesamten Netzwerkdatenverkehr über VPN.</span><span class="sxs-lookup"><span data-stu-id="d1edc-213">Send all network traffic through VPN.</span></span> <span data-ttu-id="d1edc-214">Geerbt von [der applevpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1edc-214">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="d1edc-215">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="d1edc-215">authenticationMethod</span></span>|[<span data-ttu-id="d1edc-216">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="d1edc-216">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="d1edc-217">Authentifizierungsmethode für diese VPN-Verbindung.</span><span class="sxs-lookup"><span data-stu-id="d1edc-217">Authentication method for this VPN connection.</span></span> <span data-ttu-id="d1edc-218">Von [der applevpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="d1edc-218">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="d1edc-219">Mögliche Werte sind: `certificate` und `usernameAndPassword`.</span><span class="sxs-lookup"><span data-stu-id="d1edc-219">Possible values are: `certificate`, `usernameAndPassword`.</span></span>|
|<span data-ttu-id="d1edc-220">enablePerApp</span><span class="sxs-lookup"><span data-stu-id="d1edc-220">enablePerApp</span></span>|<span data-ttu-id="d1edc-221">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d1edc-221">Boolean</span></span>|<span data-ttu-id="d1edc-222">Wenn Sie dies auf true festlegen, wird eine pro-App-VPN-Nutzlast erstellt, die später apps zugeordnet werden kann, die diese VPN-Anschluss auf dem iOS-Gerät des Endbenutzers auslösen können.</span><span class="sxs-lookup"><span data-stu-id="d1edc-222">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span> <span data-ttu-id="d1edc-223">Geerbt von [der applevpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1edc-223">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="d1edc-224">safariDomains</span><span class="sxs-lookup"><span data-stu-id="d1edc-224">safariDomains</span></span>|<span data-ttu-id="d1edc-225">String collection</span><span class="sxs-lookup"><span data-stu-id="d1edc-225">String collection</span></span>|<span data-ttu-id="d1edc-226">Safari-Domänen, wenn diese VPN-pro-app-Einstellung aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="d1edc-226">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="d1edc-227">Zusätzlich zu den apps, die mit diesem VPN verknüpft sind, können auch hier angegebene Safari-Domänen diese VPN-Verbindung auslösen.</span><span class="sxs-lookup"><span data-stu-id="d1edc-227">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span> <span data-ttu-id="d1edc-228">Geerbt von [der applevpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1edc-228">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="d1edc-229">onDemandRules</span><span class="sxs-lookup"><span data-stu-id="d1edc-229">onDemandRules</span></span>|<span data-ttu-id="d1edc-230">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="d1edc-230">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="d1edc-231">Regeln für on-Demand.</span><span class="sxs-lookup"><span data-stu-id="d1edc-231">On-Demand Rules.</span></span> <span data-ttu-id="d1edc-232">Diese Sammlung darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="d1edc-232">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="d1edc-233">Geerbt von [der applevpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1edc-233">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="d1edc-234">Sie</span><span class="sxs-lookup"><span data-stu-id="d1edc-234">proxyServer</span></span>|[<span data-ttu-id="d1edc-235">vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="d1edc-235">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="d1edc-236">Proxy Server.</span><span class="sxs-lookup"><span data-stu-id="d1edc-236">Proxy Server.</span></span> <span data-ttu-id="d1edc-237">Geerbt von [der applevpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1edc-237">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="d1edc-238">optInToDeviceIdSharing</span><span class="sxs-lookup"><span data-stu-id="d1edc-238">optInToDeviceIdSharing</span></span>|<span data-ttu-id="d1edc-239">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d1edc-239">Boolean</span></span>|<span data-ttu-id="d1edc-240">Opt-in für die Freigabe der Geräte-ID an Drittanbieter-VPN-Clients für die Verwendung während der Überprüfung der Netzwerkzugriffssteuerung.</span><span class="sxs-lookup"><span data-stu-id="d1edc-240">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span> <span data-ttu-id="d1edc-241">Geerbt von [der applevpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1edc-241">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="d1edc-242">Antwort</span><span class="sxs-lookup"><span data-stu-id="d1edc-242">Response</span></span>
<span data-ttu-id="d1edc-243">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="d1edc-243">If successful, this method returns a `201 Created` response code and a [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d1edc-244">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d1edc-244">Example</span></span>

### <a name="request"></a><span data-ttu-id="d1edc-245">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d1edc-245">Request</span></span>
<span data-ttu-id="d1edc-246">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d1edc-246">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="d1edc-247">Antwort</span><span class="sxs-lookup"><span data-stu-id="d1edc-247">Response</span></span>
<span data-ttu-id="d1edc-p126">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d1edc-p126">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




