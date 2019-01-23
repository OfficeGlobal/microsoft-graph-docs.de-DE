---
title: IosVpnConfiguration aktualisieren
description: Aktualisieren Sie die Eigenschaften eines IosVpnConfiguration-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: ef6ce932f40de3f160b107786b1cc72cb21246a4
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29407921"
---
# <a name="update-iosvpnconfiguration"></a><span data-ttu-id="f4913-103">IosVpnConfiguration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="f4913-103">Update iosVpnConfiguration</span></span>

> <span data-ttu-id="f4913-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="f4913-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f4913-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f4913-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f4913-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f4913-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f4913-107">Aktualisieren Sie die Eigenschaften eines [IosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="f4913-107">Update the properties of a [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f4913-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f4913-108">Prerequisites</span></span>
<span data-ttu-id="f4913-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="f4913-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f4913-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f4913-111">Permission type</span></span>|<span data-ttu-id="f4913-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f4913-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f4913-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f4913-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f4913-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4913-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f4913-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f4913-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f4913-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f4913-116">Not supported.</span></span>|
|<span data-ttu-id="f4913-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f4913-117">Application</span></span>|<span data-ttu-id="f4913-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f4913-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f4913-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f4913-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="f4913-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f4913-120">Request headers</span></span>
|<span data-ttu-id="f4913-121">Header</span><span class="sxs-lookup"><span data-stu-id="f4913-121">Header</span></span>|<span data-ttu-id="f4913-122">Wert</span><span class="sxs-lookup"><span data-stu-id="f4913-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f4913-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="f4913-123">Authorization</span></span>|<span data-ttu-id="f4913-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="f4913-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f4913-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="f4913-125">Accept</span></span>|<span data-ttu-id="f4913-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f4913-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f4913-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f4913-127">Request body</span></span>
<span data-ttu-id="f4913-128">Geben Sie im Textkörper Anforderung für das Objekt [IosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="f4913-128">In the request body, supply a JSON representation for the [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) object.</span></span>

<span data-ttu-id="f4913-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [IosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="f4913-129">The following table shows the properties that are required when you create the [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md).</span></span>

|<span data-ttu-id="f4913-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f4913-130">Property</span></span>|<span data-ttu-id="f4913-131">Typ</span><span class="sxs-lookup"><span data-stu-id="f4913-131">Type</span></span>|<span data-ttu-id="f4913-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f4913-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f4913-133">id</span><span class="sxs-lookup"><span data-stu-id="f4913-133">id</span></span>|<span data-ttu-id="f4913-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f4913-134">String</span></span>|<span data-ttu-id="f4913-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="f4913-135">Key of the entity.</span></span> <span data-ttu-id="f4913-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f4913-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f4913-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f4913-137">lastModifiedDateTime</span></span>|<span data-ttu-id="f4913-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f4913-138">DateTimeOffset</span></span>|<span data-ttu-id="f4913-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="f4913-139">DateTime the object was last modified.</span></span> <span data-ttu-id="f4913-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f4913-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f4913-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f4913-141">roleScopeTagIds</span></span>|<span data-ttu-id="f4913-142">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="f4913-142">String collection</span></span>|<span data-ttu-id="f4913-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="f4913-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f4913-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f4913-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f4913-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="f4913-145">supportsScopeTags</span></span>|<span data-ttu-id="f4913-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="f4913-146">Boolean</span></span>|<span data-ttu-id="f4913-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f4913-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f4913-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="f4913-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f4913-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="f4913-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f4913-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="f4913-150">This property is read-only.</span></span> <span data-ttu-id="f4913-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f4913-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f4913-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f4913-152">createdDateTime</span></span>|<span data-ttu-id="f4913-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f4913-153">DateTimeOffset</span></span>|<span data-ttu-id="f4913-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="f4913-154">DateTime the object was created.</span></span> <span data-ttu-id="f4913-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f4913-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f4913-156">description</span><span class="sxs-lookup"><span data-stu-id="f4913-156">description</span></span>|<span data-ttu-id="f4913-157">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f4913-157">String</span></span>|<span data-ttu-id="f4913-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="f4913-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f4913-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f4913-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f4913-160">displayName</span><span class="sxs-lookup"><span data-stu-id="f4913-160">displayName</span></span>|<span data-ttu-id="f4913-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f4913-161">String</span></span>|<span data-ttu-id="f4913-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="f4913-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f4913-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f4913-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f4913-164">Version</span><span class="sxs-lookup"><span data-stu-id="f4913-164">version</span></span>|<span data-ttu-id="f4913-165">Int32</span><span class="sxs-lookup"><span data-stu-id="f4913-165">Int32</span></span>|<span data-ttu-id="f4913-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="f4913-166">Version of the device configuration.</span></span> <span data-ttu-id="f4913-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f4913-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f4913-168">connectionName</span><span class="sxs-lookup"><span data-stu-id="f4913-168">connectionName</span></span>|<span data-ttu-id="f4913-169">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f4913-169">String</span></span>|<span data-ttu-id="f4913-170">Name der Verbindung für den Benutzer angezeigt.</span><span class="sxs-lookup"><span data-stu-id="f4913-170">Connection name displayed to the user.</span></span> <span data-ttu-id="f4913-171">Geerbt von [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f4913-171">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="f4913-172">connectionType</span><span class="sxs-lookup"><span data-stu-id="f4913-172">connectionType</span></span>|[<span data-ttu-id="f4913-173">appleVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="f4913-173">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="f4913-174">Verbindungstyp.</span><span class="sxs-lookup"><span data-stu-id="f4913-174">Connection type.</span></span> <span data-ttu-id="f4913-175">Geerbt von [AppleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f4913-175">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="f4913-176">Mögliche Werte sind: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`.</span><span class="sxs-lookup"><span data-stu-id="f4913-176">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`.</span></span>|
|<span data-ttu-id="f4913-177">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="f4913-177">loginGroupOrDomain</span></span>|<span data-ttu-id="f4913-178">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f4913-178">String</span></span>|<span data-ttu-id="f4913-179">Anmeldegruppe oder Domäne Wenn Verbindungstyp auf Dell SonicWALL Mobile Verbindung festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="f4913-179">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="f4913-180">Geerbt von [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f4913-180">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="f4913-181">role</span><span class="sxs-lookup"><span data-stu-id="f4913-181">role</span></span>|<span data-ttu-id="f4913-182">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f4913-182">String</span></span>|<span data-ttu-id="f4913-183">Rolle, wenn Verbindungstyp auf Pulse Secure festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="f4913-183">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="f4913-184">Geerbt von [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f4913-184">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="f4913-185">Bereich</span><span class="sxs-lookup"><span data-stu-id="f4913-185">realm</span></span>|<span data-ttu-id="f4913-186">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f4913-186">String</span></span>|<span data-ttu-id="f4913-187">Realm Wenn Verbindungstyp auf Pulse Secure festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="f4913-187">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="f4913-188">Geerbt von [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f4913-188">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="f4913-189">Server</span><span class="sxs-lookup"><span data-stu-id="f4913-189">server</span></span>|[<span data-ttu-id="f4913-190">vpnServer</span><span class="sxs-lookup"><span data-stu-id="f4913-190">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="f4913-191">VPN-Server im Netzwerk.</span><span class="sxs-lookup"><span data-stu-id="f4913-191">VPN Server on the network.</span></span> <span data-ttu-id="f4913-192">Stellen Sie sicher, dass Endbenutzer dieser Speicherort im Netzwerk zugreifen können.</span><span class="sxs-lookup"><span data-stu-id="f4913-192">Make sure end users can access this network location.</span></span> <span data-ttu-id="f4913-193">Geerbt von [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f4913-193">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="f4913-194">Bezeichner</span><span class="sxs-lookup"><span data-stu-id="f4913-194">identifier</span></span>|<span data-ttu-id="f4913-195">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f4913-195">String</span></span>|<span data-ttu-id="f4913-196">Bezeichner von VPN-Anbieter bereitgestellt, wenn Verbindungstyp auf benutzerdefinierte VPN festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="f4913-196">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="f4913-197">Beispiel: Cisco AnyConnect verwendet eine Kennung des dem Formular com.cisco.anyconnect.applevpn.plugin Inherited aus [AppleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f4913-197">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="f4913-198">customData</span><span class="sxs-lookup"><span data-stu-id="f4913-198">customData</span></span>|<span data-ttu-id="f4913-199">[KeyValue](../resources/intune-deviceconfig-keyvalue.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="f4913-199">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="f4913-200">Benutzerdefinierte Daten beim Verbindungstyp auf benutzerdefinierte VPN festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="f4913-200">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="f4913-201">Verwenden Sie dieses Feld, um von Intune, nicht jedoch in Ihre VPN-Lösung verfügbar unterstützten Funktionen zu aktivieren.</span><span class="sxs-lookup"><span data-stu-id="f4913-201">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="f4913-202">Wenden Sie sich an Ihrer VPN-Hersteller, um Informationen zum Hinzufügen dieser Schlüssel/Wert-Paare.</span><span class="sxs-lookup"><span data-stu-id="f4913-202">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="f4913-203">Diese Sammlung kann maximal 25 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="f4913-203">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="f4913-204">Geerbt von [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f4913-204">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="f4913-205">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="f4913-205">customKeyValueData</span></span>|<span data-ttu-id="f4913-206">[keyValuePair](../resources/intune-shared-keyvaluepair.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="f4913-206">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="f4913-207">Benutzerdefinierte Daten beim Verbindungstyp auf benutzerdefinierte VPN festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="f4913-207">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="f4913-208">Verwenden Sie dieses Feld, um von Intune, nicht jedoch in Ihre VPN-Lösung verfügbar unterstützten Funktionen zu aktivieren.</span><span class="sxs-lookup"><span data-stu-id="f4913-208">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="f4913-209">Wenden Sie sich an Ihrer VPN-Hersteller, um Informationen zum Hinzufügen dieser Schlüssel/Wert-Paare.</span><span class="sxs-lookup"><span data-stu-id="f4913-209">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="f4913-210">Diese Sammlung kann maximal 25 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="f4913-210">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="f4913-211">Geerbt von [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f4913-211">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="f4913-212">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="f4913-212">enableSplitTunneling</span></span>|<span data-ttu-id="f4913-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="f4913-213">Boolean</span></span>|<span data-ttu-id="f4913-214">Senden Sie alle Netzwerkdatenverkehr über VPN.</span><span class="sxs-lookup"><span data-stu-id="f4913-214">Send all network traffic through VPN.</span></span> <span data-ttu-id="f4913-215">Geerbt von [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f4913-215">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="f4913-216">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="f4913-216">authenticationMethod</span></span>|[<span data-ttu-id="f4913-217">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="f4913-217">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="f4913-218">Authentifizierungsmethode für diese VPN-Verbindung.</span><span class="sxs-lookup"><span data-stu-id="f4913-218">Authentication method for this VPN connection.</span></span> <span data-ttu-id="f4913-219">Geerbt von [AppleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f4913-219">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="f4913-220">Mögliche Werte sind: `certificate` und `usernameAndPassword`.</span><span class="sxs-lookup"><span data-stu-id="f4913-220">Possible values are: `certificate`, `usernameAndPassword`.</span></span>|
|<span data-ttu-id="f4913-221">enablePerApp</span><span class="sxs-lookup"><span data-stu-id="f4913-221">enablePerApp</span></span>|<span data-ttu-id="f4913-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="f4913-222">Boolean</span></span>|<span data-ttu-id="f4913-223">Dies auf True festlegen, erstellt pro App VPN-Nutzlast, später Apps zugeordnet sein kann, die diese VPN-Verbindung auf iOS-Gerät des Endbenutzers auslösen kann.</span><span class="sxs-lookup"><span data-stu-id="f4913-223">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span> <span data-ttu-id="f4913-224">Geerbt von [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f4913-224">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="f4913-225">safariDomains</span><span class="sxs-lookup"><span data-stu-id="f4913-225">safariDomains</span></span>|<span data-ttu-id="f4913-226">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="f4913-226">String collection</span></span>|<span data-ttu-id="f4913-227">Safari Domänen, wenn diese VPN pro App-Einstellung aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="f4913-227">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="f4913-228">Zusätzlich zu den apps dieses VPN zugeordnet angegeben Safari Domänen Hier wird auch können Sie diese VPN-Verbindung zu lösen.</span><span class="sxs-lookup"><span data-stu-id="f4913-228">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span> <span data-ttu-id="f4913-229">Geerbt von [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f4913-229">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="f4913-230">onDemandRules</span><span class="sxs-lookup"><span data-stu-id="f4913-230">onDemandRules</span></span>|<span data-ttu-id="f4913-231">[VpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="f4913-231">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="f4913-232">Bei Bedarf Regeln.</span><span class="sxs-lookup"><span data-stu-id="f4913-232">On-Demand Rules.</span></span> <span data-ttu-id="f4913-233">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="f4913-233">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="f4913-234">Geerbt von [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f4913-234">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="f4913-235">proxyServer</span><span class="sxs-lookup"><span data-stu-id="f4913-235">proxyServer</span></span>|[<span data-ttu-id="f4913-236">vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="f4913-236">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="f4913-237">Proxy-Server.</span><span class="sxs-lookup"><span data-stu-id="f4913-237">Proxy Server.</span></span> <span data-ttu-id="f4913-238">Geerbt von [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f4913-238">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="f4913-239">optInToDeviceIdSharing</span><span class="sxs-lookup"><span data-stu-id="f4913-239">optInToDeviceIdSharing</span></span>|<span data-ttu-id="f4913-240">Boolean</span><span class="sxs-lookup"><span data-stu-id="f4913-240">Boolean</span></span>|<span data-ttu-id="f4913-241">Opt-In, das das Gerät Id Drittanbieter-VPN-Clients für die Verwendung während der Network Access Control Validierung Freigabe.</span><span class="sxs-lookup"><span data-stu-id="f4913-241">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span> <span data-ttu-id="f4913-242">Geerbt von [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f4913-242">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="f4913-243">providerType</span><span class="sxs-lookup"><span data-stu-id="f4913-243">providerType</span></span>|[<span data-ttu-id="f4913-244">vpnProviderType</span><span class="sxs-lookup"><span data-stu-id="f4913-244">vpnProviderType</span></span>](../resources/intune-deviceconfig-vpnprovidertype.md)|<span data-ttu-id="f4913-245">Providertyp für VPN-app.</span><span class="sxs-lookup"><span data-stu-id="f4913-245">Provider type for per-app VPN.</span></span> <span data-ttu-id="f4913-246">Mögliche Werte sind: `notConfigured`, `appProxy` und `packetTunnel`.</span><span class="sxs-lookup"><span data-stu-id="f4913-246">Possible values are: `notConfigured`, `appProxy`, `packetTunnel`.</span></span>|
|<span data-ttu-id="f4913-247">userDomain</span><span class="sxs-lookup"><span data-stu-id="f4913-247">userDomain</span></span>|<span data-ttu-id="f4913-248">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f4913-248">String</span></span>|<span data-ttu-id="f4913-249">Zscaler.</span><span class="sxs-lookup"><span data-stu-id="f4913-249">Zscaler only.</span></span> <span data-ttu-id="f4913-250">Geben Sie eine statische Domäne, um das Feld Anmeldename mit in der app Zscaler vorab auszufüllen.</span><span class="sxs-lookup"><span data-stu-id="f4913-250">Enter a static domain to pre-populate the login field with in the Zscaler app.</span></span> <span data-ttu-id="f4913-251">Wenn dies leer ist, wird stattdessen Azure Active Directory-Domäne des Benutzers verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="f4913-251">If this is left empty, the user's Azure Active Directory domain will be used instead.</span></span>|
|<span data-ttu-id="f4913-252">strictEnforcement</span><span class="sxs-lookup"><span data-stu-id="f4913-252">strictEnforcement</span></span>|<span data-ttu-id="f4913-253">Boolean</span><span class="sxs-lookup"><span data-stu-id="f4913-253">Boolean</span></span>|<span data-ttu-id="f4913-254">Zscaler.</span><span class="sxs-lookup"><span data-stu-id="f4913-254">Zscaler only.</span></span> <span data-ttu-id="f4913-255">Blöcke Netzwerkverkehr bis auf Anzeichen für die Benutzer in Zscaler app.</span><span class="sxs-lookup"><span data-stu-id="f4913-255">Blocks network traffic until the user signs into Zscaler app.</span></span> <span data-ttu-id="f4913-256">"True" bedeutet, dass Datenverkehr ausgeschlossen wird.</span><span class="sxs-lookup"><span data-stu-id="f4913-256">"True" means traffic is blocked.</span></span>|
|<span data-ttu-id="f4913-257">cloudName</span><span class="sxs-lookup"><span data-stu-id="f4913-257">cloudName</span></span>|<span data-ttu-id="f4913-258">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f4913-258">String</span></span>|<span data-ttu-id="f4913-259">Zscaler.</span><span class="sxs-lookup"><span data-stu-id="f4913-259">Zscaler only.</span></span> <span data-ttu-id="f4913-260">Zscaler Cloud, die der Benutzer zugewiesen ist.</span><span class="sxs-lookup"><span data-stu-id="f4913-260">Zscaler cloud which the user is assigned to.</span></span>|
|<span data-ttu-id="f4913-261">excludeList</span><span class="sxs-lookup"><span data-stu-id="f4913-261">excludeList</span></span>|<span data-ttu-id="f4913-262">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="f4913-262">String collection</span></span>|<span data-ttu-id="f4913-263">Zscaler.</span><span class="sxs-lookup"><span data-stu-id="f4913-263">Zscaler only.</span></span> <span data-ttu-id="f4913-264">Liste der Netzwerkadressen, die nicht über die Cloud Zscaler gesendet werden.</span><span class="sxs-lookup"><span data-stu-id="f4913-264">List of network addresses which are not sent through the Zscaler cloud.</span></span>|



## <a name="response"></a><span data-ttu-id="f4913-265">Antwort</span><span class="sxs-lookup"><span data-stu-id="f4913-265">Response</span></span>
<span data-ttu-id="f4913-266">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [IosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="f4913-266">If successful, this method returns a `200 OK` response code and an updated [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f4913-267">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f4913-267">Example</span></span>

### <a name="request"></a><span data-ttu-id="f4913-268">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f4913-268">Request</span></span>
<span data-ttu-id="f4913-269">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f4913-269">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f4913-270">Antwort</span><span class="sxs-lookup"><span data-stu-id="f4913-270">Response</span></span>
<span data-ttu-id="f4913-p132">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f4913-p132">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




