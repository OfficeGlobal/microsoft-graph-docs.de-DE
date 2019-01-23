---
title: Erstellen von macOSVpnConfiguration
description: Erstellen eines neuen MacOSVpnConfiguration-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 2c8e2aefb0aa7bfc3a73ac83d32823d9c3c44a3b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29416013"
---
# <a name="create-macosvpnconfiguration"></a><span data-ttu-id="b4e2c-103">Erstellen von macOSVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="b4e2c-103">Create macOSVpnConfiguration</span></span>

> <span data-ttu-id="b4e2c-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="b4e2c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b4e2c-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b4e2c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b4e2c-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b4e2c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b4e2c-107">Erstellen eines neuen [MacOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="b4e2c-107">Create a new [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b4e2c-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b4e2c-108">Prerequisites</span></span>
<span data-ttu-id="b4e2c-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="b4e2c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b4e2c-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b4e2c-111">Permission type</span></span>|<span data-ttu-id="b4e2c-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b4e2c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b4e2c-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b4e2c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b4e2c-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4e2c-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b4e2c-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b4e2c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b4e2c-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b4e2c-116">Not supported.</span></span>|
|<span data-ttu-id="b4e2c-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b4e2c-117">Application</span></span>|<span data-ttu-id="b4e2c-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b4e2c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b4e2c-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b4e2c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="b4e2c-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b4e2c-120">Request headers</span></span>
|<span data-ttu-id="b4e2c-121">Header</span><span class="sxs-lookup"><span data-stu-id="b4e2c-121">Header</span></span>|<span data-ttu-id="b4e2c-122">Wert</span><span class="sxs-lookup"><span data-stu-id="b4e2c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b4e2c-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="b4e2c-123">Authorization</span></span>|<span data-ttu-id="b4e2c-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b4e2c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b4e2c-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="b4e2c-125">Accept</span></span>|<span data-ttu-id="b4e2c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b4e2c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b4e2c-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b4e2c-127">Request body</span></span>
<span data-ttu-id="b4e2c-128">Geben Sie im Textkörper Anforderung für das Objekt MacOSVpnConfiguration eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="b4e2c-128">In the request body, supply a JSON representation for the macOSVpnConfiguration object.</span></span>

<span data-ttu-id="b4e2c-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die MacOSVpnConfiguration erstellen.</span><span class="sxs-lookup"><span data-stu-id="b4e2c-129">The following table shows the properties that are required when you create the macOSVpnConfiguration.</span></span>

|<span data-ttu-id="b4e2c-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b4e2c-130">Property</span></span>|<span data-ttu-id="b4e2c-131">Typ</span><span class="sxs-lookup"><span data-stu-id="b4e2c-131">Type</span></span>|<span data-ttu-id="b4e2c-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b4e2c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b4e2c-133">id</span><span class="sxs-lookup"><span data-stu-id="b4e2c-133">id</span></span>|<span data-ttu-id="b4e2c-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b4e2c-134">String</span></span>|<span data-ttu-id="b4e2c-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="b4e2c-135">Key of the entity.</span></span> <span data-ttu-id="b4e2c-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b4e2c-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b4e2c-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b4e2c-137">lastModifiedDateTime</span></span>|<span data-ttu-id="b4e2c-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b4e2c-138">DateTimeOffset</span></span>|<span data-ttu-id="b4e2c-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="b4e2c-139">DateTime the object was last modified.</span></span> <span data-ttu-id="b4e2c-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b4e2c-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b4e2c-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b4e2c-141">roleScopeTagIds</span></span>|<span data-ttu-id="b4e2c-142">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="b4e2c-142">String collection</span></span>|<span data-ttu-id="b4e2c-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="b4e2c-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b4e2c-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b4e2c-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b4e2c-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="b4e2c-145">supportsScopeTags</span></span>|<span data-ttu-id="b4e2c-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="b4e2c-146">Boolean</span></span>|<span data-ttu-id="b4e2c-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b4e2c-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="b4e2c-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="b4e2c-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="b4e2c-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="b4e2c-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="b4e2c-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="b4e2c-150">This property is read-only.</span></span> <span data-ttu-id="b4e2c-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b4e2c-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b4e2c-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b4e2c-152">createdDateTime</span></span>|<span data-ttu-id="b4e2c-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b4e2c-153">DateTimeOffset</span></span>|<span data-ttu-id="b4e2c-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="b4e2c-154">DateTime the object was created.</span></span> <span data-ttu-id="b4e2c-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b4e2c-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b4e2c-156">description</span><span class="sxs-lookup"><span data-stu-id="b4e2c-156">description</span></span>|<span data-ttu-id="b4e2c-157">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b4e2c-157">String</span></span>|<span data-ttu-id="b4e2c-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="b4e2c-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b4e2c-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b4e2c-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b4e2c-160">displayName</span><span class="sxs-lookup"><span data-stu-id="b4e2c-160">displayName</span></span>|<span data-ttu-id="b4e2c-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b4e2c-161">String</span></span>|<span data-ttu-id="b4e2c-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="b4e2c-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b4e2c-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b4e2c-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b4e2c-164">Version</span><span class="sxs-lookup"><span data-stu-id="b4e2c-164">version</span></span>|<span data-ttu-id="b4e2c-165">Int32</span><span class="sxs-lookup"><span data-stu-id="b4e2c-165">Int32</span></span>|<span data-ttu-id="b4e2c-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="b4e2c-166">Version of the device configuration.</span></span> <span data-ttu-id="b4e2c-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b4e2c-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b4e2c-168">connectionName</span><span class="sxs-lookup"><span data-stu-id="b4e2c-168">connectionName</span></span>|<span data-ttu-id="b4e2c-169">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b4e2c-169">String</span></span>|<span data-ttu-id="b4e2c-170">Name der Verbindung für den Benutzer angezeigt.</span><span class="sxs-lookup"><span data-stu-id="b4e2c-170">Connection name displayed to the user.</span></span> <span data-ttu-id="b4e2c-171">Geerbt von [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b4e2c-171">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="b4e2c-172">connectionType</span><span class="sxs-lookup"><span data-stu-id="b4e2c-172">connectionType</span></span>|[<span data-ttu-id="b4e2c-173">appleVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="b4e2c-173">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="b4e2c-174">Verbindungstyp.</span><span class="sxs-lookup"><span data-stu-id="b4e2c-174">Connection type.</span></span> <span data-ttu-id="b4e2c-175">Geerbt von [AppleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b4e2c-175">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="b4e2c-176">Mögliche Werte sind: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`.</span><span class="sxs-lookup"><span data-stu-id="b4e2c-176">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`.</span></span>|
|<span data-ttu-id="b4e2c-177">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="b4e2c-177">loginGroupOrDomain</span></span>|<span data-ttu-id="b4e2c-178">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b4e2c-178">String</span></span>|<span data-ttu-id="b4e2c-179">Anmeldegruppe oder Domäne Wenn Verbindungstyp auf Dell SonicWALL Mobile Verbindung festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="b4e2c-179">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="b4e2c-180">Geerbt von [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b4e2c-180">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="b4e2c-181">role</span><span class="sxs-lookup"><span data-stu-id="b4e2c-181">role</span></span>|<span data-ttu-id="b4e2c-182">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b4e2c-182">String</span></span>|<span data-ttu-id="b4e2c-183">Rolle, wenn Verbindungstyp auf Pulse Secure festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="b4e2c-183">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="b4e2c-184">Geerbt von [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b4e2c-184">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="b4e2c-185">Bereich</span><span class="sxs-lookup"><span data-stu-id="b4e2c-185">realm</span></span>|<span data-ttu-id="b4e2c-186">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b4e2c-186">String</span></span>|<span data-ttu-id="b4e2c-187">Realm Wenn Verbindungstyp auf Pulse Secure festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="b4e2c-187">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="b4e2c-188">Geerbt von [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b4e2c-188">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="b4e2c-189">Server</span><span class="sxs-lookup"><span data-stu-id="b4e2c-189">server</span></span>|[<span data-ttu-id="b4e2c-190">vpnServer</span><span class="sxs-lookup"><span data-stu-id="b4e2c-190">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="b4e2c-191">VPN-Server im Netzwerk.</span><span class="sxs-lookup"><span data-stu-id="b4e2c-191">VPN Server on the network.</span></span> <span data-ttu-id="b4e2c-192">Stellen Sie sicher, dass Endbenutzer dieser Speicherort im Netzwerk zugreifen können.</span><span class="sxs-lookup"><span data-stu-id="b4e2c-192">Make sure end users can access this network location.</span></span> <span data-ttu-id="b4e2c-193">Geerbt von [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b4e2c-193">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="b4e2c-194">Bezeichner</span><span class="sxs-lookup"><span data-stu-id="b4e2c-194">identifier</span></span>|<span data-ttu-id="b4e2c-195">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b4e2c-195">String</span></span>|<span data-ttu-id="b4e2c-196">Bezeichner von VPN-Anbieter bereitgestellt, wenn Verbindungstyp auf benutzerdefinierte VPN festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="b4e2c-196">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="b4e2c-197">Beispiel: Cisco AnyConnect verwendet eine Kennung des dem Formular com.cisco.anyconnect.applevpn.plugin Inherited aus [AppleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b4e2c-197">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="b4e2c-198">customData</span><span class="sxs-lookup"><span data-stu-id="b4e2c-198">customData</span></span>|<span data-ttu-id="b4e2c-199">[KeyValue](../resources/intune-deviceconfig-keyvalue.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="b4e2c-199">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="b4e2c-200">Benutzerdefinierte Daten beim Verbindungstyp auf benutzerdefinierte VPN festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="b4e2c-200">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="b4e2c-201">Verwenden Sie dieses Feld, um von Intune, nicht jedoch in Ihre VPN-Lösung verfügbar unterstützten Funktionen zu aktivieren.</span><span class="sxs-lookup"><span data-stu-id="b4e2c-201">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="b4e2c-202">Wenden Sie sich an Ihrer VPN-Hersteller, um Informationen zum Hinzufügen dieser Schlüssel/Wert-Paare.</span><span class="sxs-lookup"><span data-stu-id="b4e2c-202">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="b4e2c-203">Diese Sammlung kann maximal 25 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="b4e2c-203">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="b4e2c-204">Geerbt von [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b4e2c-204">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="b4e2c-205">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="b4e2c-205">customKeyValueData</span></span>|<span data-ttu-id="b4e2c-206">[keyValuePair](../resources/intune-shared-keyvaluepair.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="b4e2c-206">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="b4e2c-207">Benutzerdefinierte Daten beim Verbindungstyp auf benutzerdefinierte VPN festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="b4e2c-207">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="b4e2c-208">Verwenden Sie dieses Feld, um von Intune, nicht jedoch in Ihre VPN-Lösung verfügbar unterstützten Funktionen zu aktivieren.</span><span class="sxs-lookup"><span data-stu-id="b4e2c-208">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="b4e2c-209">Wenden Sie sich an Ihrer VPN-Hersteller, um Informationen zum Hinzufügen dieser Schlüssel/Wert-Paare.</span><span class="sxs-lookup"><span data-stu-id="b4e2c-209">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="b4e2c-210">Diese Sammlung kann maximal 25 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="b4e2c-210">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="b4e2c-211">Geerbt von [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b4e2c-211">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="b4e2c-212">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="b4e2c-212">enableSplitTunneling</span></span>|<span data-ttu-id="b4e2c-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="b4e2c-213">Boolean</span></span>|<span data-ttu-id="b4e2c-214">Senden Sie alle Netzwerkdatenverkehr über VPN.</span><span class="sxs-lookup"><span data-stu-id="b4e2c-214">Send all network traffic through VPN.</span></span> <span data-ttu-id="b4e2c-215">Geerbt von [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b4e2c-215">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="b4e2c-216">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="b4e2c-216">authenticationMethod</span></span>|[<span data-ttu-id="b4e2c-217">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="b4e2c-217">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="b4e2c-218">Authentifizierungsmethode für diese VPN-Verbindung.</span><span class="sxs-lookup"><span data-stu-id="b4e2c-218">Authentication method for this VPN connection.</span></span> <span data-ttu-id="b4e2c-219">Geerbt von [AppleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b4e2c-219">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="b4e2c-220">Mögliche Werte sind: `certificate` und `usernameAndPassword`.</span><span class="sxs-lookup"><span data-stu-id="b4e2c-220">Possible values are: `certificate`, `usernameAndPassword`.</span></span>|
|<span data-ttu-id="b4e2c-221">enablePerApp</span><span class="sxs-lookup"><span data-stu-id="b4e2c-221">enablePerApp</span></span>|<span data-ttu-id="b4e2c-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="b4e2c-222">Boolean</span></span>|<span data-ttu-id="b4e2c-223">Dies auf True festlegen, erstellt pro App VPN-Nutzlast, später Apps zugeordnet sein kann, die diese VPN-Verbindung auf iOS-Gerät des Endbenutzers auslösen kann.</span><span class="sxs-lookup"><span data-stu-id="b4e2c-223">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span> <span data-ttu-id="b4e2c-224">Geerbt von [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b4e2c-224">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="b4e2c-225">safariDomains</span><span class="sxs-lookup"><span data-stu-id="b4e2c-225">safariDomains</span></span>|<span data-ttu-id="b4e2c-226">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="b4e2c-226">String collection</span></span>|<span data-ttu-id="b4e2c-227">Safari Domänen, wenn diese VPN pro App-Einstellung aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="b4e2c-227">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="b4e2c-228">Zusätzlich zu den apps dieses VPN zugeordnet angegeben Safari Domänen Hier wird auch können Sie diese VPN-Verbindung zu lösen.</span><span class="sxs-lookup"><span data-stu-id="b4e2c-228">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span> <span data-ttu-id="b4e2c-229">Geerbt von [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b4e2c-229">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="b4e2c-230">onDemandRules</span><span class="sxs-lookup"><span data-stu-id="b4e2c-230">onDemandRules</span></span>|<span data-ttu-id="b4e2c-231">[VpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="b4e2c-231">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="b4e2c-232">Bei Bedarf Regeln.</span><span class="sxs-lookup"><span data-stu-id="b4e2c-232">On-Demand Rules.</span></span> <span data-ttu-id="b4e2c-233">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="b4e2c-233">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="b4e2c-234">Geerbt von [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b4e2c-234">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="b4e2c-235">proxyServer</span><span class="sxs-lookup"><span data-stu-id="b4e2c-235">proxyServer</span></span>|[<span data-ttu-id="b4e2c-236">vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="b4e2c-236">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="b4e2c-237">Proxy-Server.</span><span class="sxs-lookup"><span data-stu-id="b4e2c-237">Proxy Server.</span></span> <span data-ttu-id="b4e2c-238">Geerbt von [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b4e2c-238">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="b4e2c-239">optInToDeviceIdSharing</span><span class="sxs-lookup"><span data-stu-id="b4e2c-239">optInToDeviceIdSharing</span></span>|<span data-ttu-id="b4e2c-240">Boolean</span><span class="sxs-lookup"><span data-stu-id="b4e2c-240">Boolean</span></span>|<span data-ttu-id="b4e2c-241">Opt-In, das das Gerät Id Drittanbieter-VPN-Clients für die Verwendung während der Network Access Control Validierung Freigabe.</span><span class="sxs-lookup"><span data-stu-id="b4e2c-241">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span> <span data-ttu-id="b4e2c-242">Geerbt von [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b4e2c-242">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="b4e2c-243">Antwort</span><span class="sxs-lookup"><span data-stu-id="b4e2c-243">Response</span></span>
<span data-ttu-id="b4e2c-244">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [MacOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="b4e2c-244">If successful, this method returns a `201 Created` response code and a [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b4e2c-245">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b4e2c-245">Example</span></span>

### <a name="request"></a><span data-ttu-id="b4e2c-246">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b4e2c-246">Request</span></span>
<span data-ttu-id="b4e2c-247">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b4e2c-247">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b4e2c-248">Antwort</span><span class="sxs-lookup"><span data-stu-id="b4e2c-248">Response</span></span>
<span data-ttu-id="b4e2c-p127">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b4e2c-p127">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




