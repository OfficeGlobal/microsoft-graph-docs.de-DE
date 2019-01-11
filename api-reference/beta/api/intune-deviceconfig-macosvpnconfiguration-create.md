---
title: Erstellen von macOSVpnConfiguration
description: Erstellen eines neuen MacOSVpnConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: d88b4fe6b0489168536acdad01dc4e32f26f68f7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27837660"
---
# <a name="create-macosvpnconfiguration"></a><span data-ttu-id="504de-103">Erstellen von macOSVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="504de-103">Create macOSVpnConfiguration</span></span>

> <span data-ttu-id="504de-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="504de-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="504de-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="504de-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="504de-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="504de-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="504de-107">Erstellen eines neuen [MacOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="504de-107">Create a new [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="504de-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="504de-108">Prerequisites</span></span>
<span data-ttu-id="504de-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="504de-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="504de-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="504de-111">Permission type</span></span>|<span data-ttu-id="504de-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="504de-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="504de-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="504de-113">Delegated (work or school account)</span></span>|<span data-ttu-id="504de-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="504de-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="504de-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="504de-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="504de-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="504de-116">Not supported.</span></span>|
|<span data-ttu-id="504de-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="504de-117">Application</span></span>|<span data-ttu-id="504de-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="504de-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="504de-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="504de-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="504de-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="504de-120">Request headers</span></span>
|<span data-ttu-id="504de-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="504de-121">Header</span></span>|<span data-ttu-id="504de-122">Wert</span><span class="sxs-lookup"><span data-stu-id="504de-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="504de-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="504de-123">Authorization</span></span>|<span data-ttu-id="504de-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="504de-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="504de-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="504de-125">Accept</span></span>|<span data-ttu-id="504de-126">application/json</span><span class="sxs-lookup"><span data-stu-id="504de-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="504de-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="504de-127">Request body</span></span>
<span data-ttu-id="504de-128">Geben Sie im Textkörper Anforderung für das Objekt MacOSVpnConfiguration eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="504de-128">In the request body, supply a JSON representation for the macOSVpnConfiguration object.</span></span>

<span data-ttu-id="504de-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die MacOSVpnConfiguration erstellen.</span><span class="sxs-lookup"><span data-stu-id="504de-129">The following table shows the properties that are required when you create the macOSVpnConfiguration.</span></span>

|<span data-ttu-id="504de-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="504de-130">Property</span></span>|<span data-ttu-id="504de-131">Typ</span><span class="sxs-lookup"><span data-stu-id="504de-131">Type</span></span>|<span data-ttu-id="504de-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="504de-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="504de-133">id</span><span class="sxs-lookup"><span data-stu-id="504de-133">id</span></span>|<span data-ttu-id="504de-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="504de-134">String</span></span>|<span data-ttu-id="504de-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="504de-135">Key of the entity.</span></span> <span data-ttu-id="504de-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="504de-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="504de-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="504de-137">lastModifiedDateTime</span></span>|<span data-ttu-id="504de-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="504de-138">DateTimeOffset</span></span>|<span data-ttu-id="504de-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="504de-139">DateTime the object was last modified.</span></span> <span data-ttu-id="504de-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="504de-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="504de-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="504de-141">roleScopeTagIds</span></span>|<span data-ttu-id="504de-142">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="504de-142">String collection</span></span>|<span data-ttu-id="504de-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="504de-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="504de-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="504de-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="504de-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="504de-145">supportsScopeTags</span></span>|<span data-ttu-id="504de-146">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="504de-146">Boolean</span></span>|<span data-ttu-id="504de-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="504de-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="504de-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="504de-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="504de-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="504de-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="504de-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="504de-150">This property is read-only.</span></span> <span data-ttu-id="504de-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="504de-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="504de-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="504de-152">createdDateTime</span></span>|<span data-ttu-id="504de-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="504de-153">DateTimeOffset</span></span>|<span data-ttu-id="504de-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="504de-154">DateTime the object was created.</span></span> <span data-ttu-id="504de-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="504de-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="504de-156">description</span><span class="sxs-lookup"><span data-stu-id="504de-156">description</span></span>|<span data-ttu-id="504de-157">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="504de-157">String</span></span>|<span data-ttu-id="504de-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="504de-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="504de-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="504de-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="504de-160">displayName</span><span class="sxs-lookup"><span data-stu-id="504de-160">displayName</span></span>|<span data-ttu-id="504de-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="504de-161">String</span></span>|<span data-ttu-id="504de-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="504de-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="504de-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="504de-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="504de-164">Version</span><span class="sxs-lookup"><span data-stu-id="504de-164">version</span></span>|<span data-ttu-id="504de-165">Int32</span><span class="sxs-lookup"><span data-stu-id="504de-165">Int32</span></span>|<span data-ttu-id="504de-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="504de-166">Version of the device configuration.</span></span> <span data-ttu-id="504de-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="504de-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="504de-168">connectionName</span><span class="sxs-lookup"><span data-stu-id="504de-168">connectionName</span></span>|<span data-ttu-id="504de-169">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="504de-169">String</span></span>|<span data-ttu-id="504de-170">Name der Verbindung für den Benutzer angezeigt.</span><span class="sxs-lookup"><span data-stu-id="504de-170">Connection name displayed to the user.</span></span> <span data-ttu-id="504de-171">Geerbt von [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="504de-171">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="504de-172">connectionType</span><span class="sxs-lookup"><span data-stu-id="504de-172">connectionType</span></span>|[<span data-ttu-id="504de-173">appleVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="504de-173">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="504de-174">Verbindungstyp.</span><span class="sxs-lookup"><span data-stu-id="504de-174">Connection type.</span></span> <span data-ttu-id="504de-175">Geerbt von [AppleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="504de-175">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="504de-176">Mögliche Werte sind: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`.</span><span class="sxs-lookup"><span data-stu-id="504de-176">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`.</span></span>|
|<span data-ttu-id="504de-177">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="504de-177">loginGroupOrDomain</span></span>|<span data-ttu-id="504de-178">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="504de-178">String</span></span>|<span data-ttu-id="504de-179">Anmeldegruppe oder Domäne Wenn Verbindungstyp auf Dell SonicWALL Mobile Verbindung festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="504de-179">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="504de-180">Geerbt von [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="504de-180">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="504de-181">role</span><span class="sxs-lookup"><span data-stu-id="504de-181">role</span></span>|<span data-ttu-id="504de-182">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="504de-182">String</span></span>|<span data-ttu-id="504de-183">Rolle, wenn Verbindungstyp auf Pulse Secure festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="504de-183">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="504de-184">Geerbt von [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="504de-184">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="504de-185">Bereich</span><span class="sxs-lookup"><span data-stu-id="504de-185">realm</span></span>|<span data-ttu-id="504de-186">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="504de-186">String</span></span>|<span data-ttu-id="504de-187">Realm Wenn Verbindungstyp auf Pulse Secure festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="504de-187">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="504de-188">Geerbt von [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="504de-188">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="504de-189">Server</span><span class="sxs-lookup"><span data-stu-id="504de-189">server</span></span>|[<span data-ttu-id="504de-190">vpnServer</span><span class="sxs-lookup"><span data-stu-id="504de-190">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="504de-191">VPN-Server im Netzwerk.</span><span class="sxs-lookup"><span data-stu-id="504de-191">VPN Server on the network.</span></span> <span data-ttu-id="504de-192">Stellen Sie sicher, dass Endbenutzer dieser Speicherort im Netzwerk zugreifen können.</span><span class="sxs-lookup"><span data-stu-id="504de-192">Make sure end users can access this network location.</span></span> <span data-ttu-id="504de-193">Geerbt von [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="504de-193">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="504de-194">Bezeichner</span><span class="sxs-lookup"><span data-stu-id="504de-194">identifier</span></span>|<span data-ttu-id="504de-195">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="504de-195">String</span></span>|<span data-ttu-id="504de-196">Bezeichner von VPN-Anbieter bereitgestellt, wenn Verbindungstyp auf benutzerdefinierte VPN festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="504de-196">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="504de-197">Beispiel: Cisco AnyConnect verwendet eine Kennung des dem Formular com.cisco.anyconnect.applevpn.plugin Inherited aus [AppleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="504de-197">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="504de-198">customData</span><span class="sxs-lookup"><span data-stu-id="504de-198">customData</span></span>|<span data-ttu-id="504de-199">[KeyValue](../resources/intune-deviceconfig-keyvalue.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="504de-199">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="504de-200">Benutzerdefinierte Daten beim Verbindungstyp auf benutzerdefinierte VPN festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="504de-200">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="504de-201">Verwenden Sie dieses Feld, um von Intune, nicht jedoch in Ihre VPN-Lösung verfügbar unterstützten Funktionen zu aktivieren.</span><span class="sxs-lookup"><span data-stu-id="504de-201">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="504de-202">Wenden Sie sich an Ihrer VPN-Hersteller, um Informationen zum Hinzufügen dieser Schlüssel/Wert-Paare.</span><span class="sxs-lookup"><span data-stu-id="504de-202">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="504de-203">Diese Sammlung kann maximal 25 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="504de-203">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="504de-204">Geerbt von [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="504de-204">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="504de-205">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="504de-205">customKeyValueData</span></span>|<span data-ttu-id="504de-206">[keyValuePair](../resources/intune-shared-keyvaluepair.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="504de-206">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="504de-207">Benutzerdefinierte Daten beim Verbindungstyp auf benutzerdefinierte VPN festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="504de-207">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="504de-208">Verwenden Sie dieses Feld, um von Intune, nicht jedoch in Ihre VPN-Lösung verfügbar unterstützten Funktionen zu aktivieren.</span><span class="sxs-lookup"><span data-stu-id="504de-208">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="504de-209">Wenden Sie sich an Ihrer VPN-Hersteller, um Informationen zum Hinzufügen dieser Schlüssel/Wert-Paare.</span><span class="sxs-lookup"><span data-stu-id="504de-209">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="504de-210">Diese Sammlung kann maximal 25 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="504de-210">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="504de-211">Geerbt von [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="504de-211">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="504de-212">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="504de-212">enableSplitTunneling</span></span>|<span data-ttu-id="504de-213">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="504de-213">Boolean</span></span>|<span data-ttu-id="504de-214">Senden Sie alle Netzwerkdatenverkehr über VPN.</span><span class="sxs-lookup"><span data-stu-id="504de-214">Send all network traffic through VPN.</span></span> <span data-ttu-id="504de-215">Geerbt von [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="504de-215">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="504de-216">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="504de-216">authenticationMethod</span></span>|[<span data-ttu-id="504de-217">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="504de-217">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="504de-218">Authentifizierungsmethode für diese VPN-Verbindung.</span><span class="sxs-lookup"><span data-stu-id="504de-218">Authentication method for this VPN connection.</span></span> <span data-ttu-id="504de-219">Geerbt von [AppleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="504de-219">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="504de-220">Mögliche Werte sind: `certificate` und `usernameAndPassword`.</span><span class="sxs-lookup"><span data-stu-id="504de-220">Possible values are: `certificate`, `usernameAndPassword`.</span></span>|
|<span data-ttu-id="504de-221">enablePerApp</span><span class="sxs-lookup"><span data-stu-id="504de-221">enablePerApp</span></span>|<span data-ttu-id="504de-222">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="504de-222">Boolean</span></span>|<span data-ttu-id="504de-223">Dies auf True festlegen, erstellt pro App VPN-Nutzlast, später Apps zugeordnet sein kann, die diese VPN-Verbindung auf iOS-Gerät des Endbenutzers auslösen kann.</span><span class="sxs-lookup"><span data-stu-id="504de-223">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span> <span data-ttu-id="504de-224">Geerbt von [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="504de-224">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="504de-225">safariDomains</span><span class="sxs-lookup"><span data-stu-id="504de-225">safariDomains</span></span>|<span data-ttu-id="504de-226">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="504de-226">String collection</span></span>|<span data-ttu-id="504de-227">Safari Domänen, wenn diese VPN pro App-Einstellung aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="504de-227">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="504de-228">Zusätzlich zu den apps dieses VPN zugeordnet angegeben Safari Domänen Hier wird auch können Sie diese VPN-Verbindung zu lösen.</span><span class="sxs-lookup"><span data-stu-id="504de-228">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span> <span data-ttu-id="504de-229">Geerbt von [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="504de-229">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="504de-230">onDemandRules</span><span class="sxs-lookup"><span data-stu-id="504de-230">onDemandRules</span></span>|<span data-ttu-id="504de-231">[VpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="504de-231">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="504de-232">Bei Bedarf Regeln.</span><span class="sxs-lookup"><span data-stu-id="504de-232">On-Demand Rules.</span></span> <span data-ttu-id="504de-233">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="504de-233">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="504de-234">Geerbt von [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="504de-234">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="504de-235">proxyServer</span><span class="sxs-lookup"><span data-stu-id="504de-235">proxyServer</span></span>|[<span data-ttu-id="504de-236">vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="504de-236">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="504de-237">Proxy-Server.</span><span class="sxs-lookup"><span data-stu-id="504de-237">Proxy Server.</span></span> <span data-ttu-id="504de-238">Geerbt von [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="504de-238">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="504de-239">optInToDeviceIdSharing</span><span class="sxs-lookup"><span data-stu-id="504de-239">optInToDeviceIdSharing</span></span>|<span data-ttu-id="504de-240">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="504de-240">Boolean</span></span>|<span data-ttu-id="504de-241">Opt-In, das das Gerät Id Drittanbieter-VPN-Clients für die Verwendung während der Network Access Control Validierung Freigabe.</span><span class="sxs-lookup"><span data-stu-id="504de-241">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span> <span data-ttu-id="504de-242">Geerbt von [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="504de-242">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="504de-243">Antwort</span><span class="sxs-lookup"><span data-stu-id="504de-243">Response</span></span>
<span data-ttu-id="504de-244">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [MacOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="504de-244">If successful, this method returns a `201 Created` response code and a [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="504de-245">Beispiel</span><span class="sxs-lookup"><span data-stu-id="504de-245">Example</span></span>
### <a name="request"></a><span data-ttu-id="504de-246">Anforderung</span><span class="sxs-lookup"><span data-stu-id="504de-246">Request</span></span>
<span data-ttu-id="504de-247">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="504de-247">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1921

{
  "@odata.type": "#microsoft.graph.macOSVpnConfiguration",
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

### <a name="response"></a><span data-ttu-id="504de-248">Antwort</span><span class="sxs-lookup"><span data-stu-id="504de-248">Response</span></span>
<span data-ttu-id="504de-p127">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="504de-p127">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





