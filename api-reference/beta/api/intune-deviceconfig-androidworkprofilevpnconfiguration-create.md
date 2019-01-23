---
title: Erstellen von androidWorkProfileVpnConfiguration
description: Erstellen eines neuen AndroidWorkProfileVpnConfiguration-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 6cdac06f045af7b5fc60f2debc0b17c7baf6bd2d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399178"
---
# <a name="create-androidworkprofilevpnconfiguration"></a><span data-ttu-id="c1e8f-103">Erstellen von androidWorkProfileVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="c1e8f-103">Create androidWorkProfileVpnConfiguration</span></span>

> <span data-ttu-id="c1e8f-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="c1e8f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c1e8f-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c1e8f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c1e8f-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c1e8f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c1e8f-107">Erstellen eines neuen [AndroidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="c1e8f-107">Create a new [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c1e8f-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c1e8f-108">Prerequisites</span></span>
<span data-ttu-id="c1e8f-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="c1e8f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="c1e8f-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c1e8f-111">Permission type</span></span>|<span data-ttu-id="c1e8f-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c1e8f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c1e8f-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c1e8f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c1e8f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1e8f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c1e8f-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c1e8f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c1e8f-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c1e8f-116">Not supported.</span></span>|
|<span data-ttu-id="c1e8f-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c1e8f-117">Application</span></span>|<span data-ttu-id="c1e8f-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c1e8f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c1e8f-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c1e8f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="c1e8f-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c1e8f-120">Request headers</span></span>
|<span data-ttu-id="c1e8f-121">Header</span><span class="sxs-lookup"><span data-stu-id="c1e8f-121">Header</span></span>|<span data-ttu-id="c1e8f-122">Wert</span><span class="sxs-lookup"><span data-stu-id="c1e8f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c1e8f-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="c1e8f-123">Authorization</span></span>|<span data-ttu-id="c1e8f-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c1e8f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c1e8f-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="c1e8f-125">Accept</span></span>|<span data-ttu-id="c1e8f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c1e8f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c1e8f-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c1e8f-127">Request body</span></span>
<span data-ttu-id="c1e8f-128">Geben Sie im Textkörper Anforderung für das Objekt AndroidWorkProfileVpnConfiguration eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="c1e8f-128">In the request body, supply a JSON representation for the androidWorkProfileVpnConfiguration object.</span></span>

<span data-ttu-id="c1e8f-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die AndroidWorkProfileVpnConfiguration erstellen.</span><span class="sxs-lookup"><span data-stu-id="c1e8f-129">The following table shows the properties that are required when you create the androidWorkProfileVpnConfiguration.</span></span>

|<span data-ttu-id="c1e8f-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c1e8f-130">Property</span></span>|<span data-ttu-id="c1e8f-131">Typ</span><span class="sxs-lookup"><span data-stu-id="c1e8f-131">Type</span></span>|<span data-ttu-id="c1e8f-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c1e8f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c1e8f-133">id</span><span class="sxs-lookup"><span data-stu-id="c1e8f-133">id</span></span>|<span data-ttu-id="c1e8f-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c1e8f-134">String</span></span>|<span data-ttu-id="c1e8f-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="c1e8f-135">Key of the entity.</span></span> <span data-ttu-id="c1e8f-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c1e8f-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c1e8f-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c1e8f-137">lastModifiedDateTime</span></span>|<span data-ttu-id="c1e8f-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c1e8f-138">DateTimeOffset</span></span>|<span data-ttu-id="c1e8f-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="c1e8f-139">DateTime the object was last modified.</span></span> <span data-ttu-id="c1e8f-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c1e8f-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c1e8f-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c1e8f-141">roleScopeTagIds</span></span>|<span data-ttu-id="c1e8f-142">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="c1e8f-142">String collection</span></span>|<span data-ttu-id="c1e8f-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="c1e8f-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c1e8f-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c1e8f-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c1e8f-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="c1e8f-145">supportsScopeTags</span></span>|<span data-ttu-id="c1e8f-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1e8f-146">Boolean</span></span>|<span data-ttu-id="c1e8f-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c1e8f-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="c1e8f-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="c1e8f-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="c1e8f-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="c1e8f-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="c1e8f-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="c1e8f-150">This property is read-only.</span></span> <span data-ttu-id="c1e8f-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c1e8f-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c1e8f-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c1e8f-152">createdDateTime</span></span>|<span data-ttu-id="c1e8f-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c1e8f-153">DateTimeOffset</span></span>|<span data-ttu-id="c1e8f-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="c1e8f-154">DateTime the object was created.</span></span> <span data-ttu-id="c1e8f-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c1e8f-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c1e8f-156">description</span><span class="sxs-lookup"><span data-stu-id="c1e8f-156">description</span></span>|<span data-ttu-id="c1e8f-157">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c1e8f-157">String</span></span>|<span data-ttu-id="c1e8f-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="c1e8f-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c1e8f-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c1e8f-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c1e8f-160">displayName</span><span class="sxs-lookup"><span data-stu-id="c1e8f-160">displayName</span></span>|<span data-ttu-id="c1e8f-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c1e8f-161">String</span></span>|<span data-ttu-id="c1e8f-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="c1e8f-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c1e8f-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c1e8f-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c1e8f-164">Version</span><span class="sxs-lookup"><span data-stu-id="c1e8f-164">version</span></span>|<span data-ttu-id="c1e8f-165">Int32</span><span class="sxs-lookup"><span data-stu-id="c1e8f-165">Int32</span></span>|<span data-ttu-id="c1e8f-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="c1e8f-166">Version of the device configuration.</span></span> <span data-ttu-id="c1e8f-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c1e8f-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c1e8f-168">connectionName</span><span class="sxs-lookup"><span data-stu-id="c1e8f-168">connectionName</span></span>|<span data-ttu-id="c1e8f-169">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c1e8f-169">String</span></span>|<span data-ttu-id="c1e8f-170">Name der Verbindung für den Benutzer angezeigt.</span><span class="sxs-lookup"><span data-stu-id="c1e8f-170">Connection name displayed to the user.</span></span>|
|<span data-ttu-id="c1e8f-171">connectionType</span><span class="sxs-lookup"><span data-stu-id="c1e8f-171">connectionType</span></span>|[<span data-ttu-id="c1e8f-172">androidWorkProfileVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="c1e8f-172">androidWorkProfileVpnConnectionType</span></span>](../resources/intune-deviceconfig-androidworkprofilevpnconnectiontype.md)|<span data-ttu-id="c1e8f-173">Verbindungstyp.</span><span class="sxs-lookup"><span data-stu-id="c1e8f-173">Connection type.</span></span> <span data-ttu-id="c1e8f-174">Mögliche Werte sind: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix` und `paloAltoGlobalProtect`.</span><span class="sxs-lookup"><span data-stu-id="c1e8f-174">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`, `paloAltoGlobalProtect`.</span></span>|
|<span data-ttu-id="c1e8f-175">role</span><span class="sxs-lookup"><span data-stu-id="c1e8f-175">role</span></span>|<span data-ttu-id="c1e8f-176">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c1e8f-176">String</span></span>|<span data-ttu-id="c1e8f-177">Rolle, wenn Verbindungstyp auf Pulse Secure festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="c1e8f-177">Role when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="c1e8f-178">Bereich</span><span class="sxs-lookup"><span data-stu-id="c1e8f-178">realm</span></span>|<span data-ttu-id="c1e8f-179">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c1e8f-179">String</span></span>|<span data-ttu-id="c1e8f-180">Realm Wenn Verbindungstyp auf Pulse Secure festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="c1e8f-180">Realm when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="c1e8f-181">Server</span><span class="sxs-lookup"><span data-stu-id="c1e8f-181">servers</span></span>|<span data-ttu-id="c1e8f-182">[VpnServer](../resources/intune-deviceconfig-vpnserver.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="c1e8f-182">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="c1e8f-183">Liste der VPN-Server im Netzwerk.</span><span class="sxs-lookup"><span data-stu-id="c1e8f-183">List of VPN Servers on the network.</span></span> <span data-ttu-id="c1e8f-184">Stellen Sie sicher, dass Endbenutzer diese Netzwerkadressen zugreifen können.</span><span class="sxs-lookup"><span data-stu-id="c1e8f-184">Make sure end users can access these network locations.</span></span> <span data-ttu-id="c1e8f-185">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="c1e8f-185">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="c1e8f-186">Fingerabdruck</span><span class="sxs-lookup"><span data-stu-id="c1e8f-186">fingerprint</span></span>|<span data-ttu-id="c1e8f-187">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c1e8f-187">String</span></span>|<span data-ttu-id="c1e8f-188">Fingerabdruck ist, dass eine Zeichenfolge, die zum Überprüfen des VPN-Servers verwendet wird, als vertrauenswürdig eingestuft werden kann die gilt nur bei Verbindungstyp Check Point "Kapseln" VPN ist.</span><span class="sxs-lookup"><span data-stu-id="c1e8f-188">Fingerprint is a string that will be used to verify the VPN server can be trusted, which is only applicable when connection type is Check Point Capsule VPN.</span></span>|
|<span data-ttu-id="c1e8f-189">customData</span><span class="sxs-lookup"><span data-stu-id="c1e8f-189">customData</span></span>|<span data-ttu-id="c1e8f-190">[KeyValue](../resources/intune-deviceconfig-keyvalue.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="c1e8f-190">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="c1e8f-191">Benutzerdefinierte Daten beim Verbindungstyp auf Citrix festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="c1e8f-191">Custom data when connection type is set to Citrix.</span></span> <span data-ttu-id="c1e8f-192">Diese Sammlung kann maximal 25 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="c1e8f-192">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="c1e8f-193">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="c1e8f-193">customKeyValueData</span></span>|<span data-ttu-id="c1e8f-194">[keyValuePair](../resources/intune-shared-keyvaluepair.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="c1e8f-194">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="c1e8f-195">Benutzerdefinierte Daten beim Verbindungstyp auf Citrix festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="c1e8f-195">Custom data when connection type is set to Citrix.</span></span> <span data-ttu-id="c1e8f-196">Diese Sammlung kann maximal 25 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="c1e8f-196">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="c1e8f-197">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="c1e8f-197">authenticationMethod</span></span>|[<span data-ttu-id="c1e8f-198">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="c1e8f-198">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="c1e8f-199">Authentifizierungsmethode.</span><span class="sxs-lookup"><span data-stu-id="c1e8f-199">Authentication method.</span></span> <span data-ttu-id="c1e8f-200">Mögliche Werte sind: `certificate` und `usernameAndPassword`.</span><span class="sxs-lookup"><span data-stu-id="c1e8f-200">Possible values are: `certificate`, `usernameAndPassword`.</span></span>|



## <a name="response"></a><span data-ttu-id="c1e8f-201">Antwort</span><span class="sxs-lookup"><span data-stu-id="c1e8f-201">Response</span></span>
<span data-ttu-id="c1e8f-202">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [AndroidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="c1e8f-202">If successful, this method returns a `201 Created` response code and a [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c1e8f-203">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c1e8f-203">Example</span></span>

### <a name="request"></a><span data-ttu-id="c1e8f-204">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c1e8f-204">Request</span></span>
<span data-ttu-id="c1e8f-205">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c1e8f-205">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 989

{
  "@odata.type": "#microsoft.graph.androidWorkProfileVpnConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "connectionName": "Connection Name value",
  "connectionType": "pulseSecure",
  "role": "Role value",
  "realm": "Realm value",
  "servers": [
    {
      "@odata.type": "microsoft.graph.vpnServer",
      "description": "Description value",
      "address": "Address value",
      "isDefaultServer": true
    }
  ],
  "fingerprint": "Fingerprint value",
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
  "authenticationMethod": "usernameAndPassword"
}
```

### <a name="response"></a><span data-ttu-id="c1e8f-206">Antwort</span><span class="sxs-lookup"><span data-stu-id="c1e8f-206">Response</span></span>
<span data-ttu-id="c1e8f-p116">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c1e8f-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1161

{
  "@odata.type": "#microsoft.graph.androidWorkProfileVpnConfiguration",
  "id": "32910378-0378-3291-7803-913278039132",
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
  "role": "Role value",
  "realm": "Realm value",
  "servers": [
    {
      "@odata.type": "microsoft.graph.vpnServer",
      "description": "Description value",
      "address": "Address value",
      "isDefaultServer": true
    }
  ],
  "fingerprint": "Fingerprint value",
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
  "authenticationMethod": "usernameAndPassword"
}
```




