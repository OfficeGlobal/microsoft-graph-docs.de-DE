---
title: AndroidForWorkVpnConfiguration aktualisieren
description: Aktualisieren Sie die Eigenschaften eines AndroidForWorkVpnConfiguration-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b9bfa09a87d45b769d6d38d6ed633aa39c1d1364
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29394383"
---
# <a name="update-androidforworkvpnconfiguration"></a><span data-ttu-id="09f67-103">AndroidForWorkVpnConfiguration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="09f67-103">Update androidForWorkVpnConfiguration</span></span>

> <span data-ttu-id="09f67-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="09f67-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="09f67-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="09f67-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="09f67-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="09f67-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="09f67-107">Aktualisieren Sie die Eigenschaften eines [AndroidForWorkVpnConfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="09f67-107">Update the properties of a [androidForWorkVpnConfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="09f67-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="09f67-108">Prerequisites</span></span>
<span data-ttu-id="09f67-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="09f67-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="09f67-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="09f67-111">Permission type</span></span>|<span data-ttu-id="09f67-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="09f67-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="09f67-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="09f67-113">Delegated (work or school account)</span></span>|<span data-ttu-id="09f67-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09f67-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="09f67-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="09f67-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="09f67-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="09f67-116">Not supported.</span></span>|
|<span data-ttu-id="09f67-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="09f67-117">Application</span></span>|<span data-ttu-id="09f67-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="09f67-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="09f67-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="09f67-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="09f67-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="09f67-120">Request headers</span></span>
|<span data-ttu-id="09f67-121">Header</span><span class="sxs-lookup"><span data-stu-id="09f67-121">Header</span></span>|<span data-ttu-id="09f67-122">Wert</span><span class="sxs-lookup"><span data-stu-id="09f67-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="09f67-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="09f67-123">Authorization</span></span>|<span data-ttu-id="09f67-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="09f67-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="09f67-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="09f67-125">Accept</span></span>|<span data-ttu-id="09f67-126">application/json</span><span class="sxs-lookup"><span data-stu-id="09f67-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="09f67-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="09f67-127">Request body</span></span>
<span data-ttu-id="09f67-128">Geben Sie im Textkörper Anforderung für das Objekt [AndroidForWorkVpnConfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="09f67-128">In the request body, supply a JSON representation for the [androidForWorkVpnConfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md) object.</span></span>

<span data-ttu-id="09f67-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [AndroidForWorkVpnConfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="09f67-129">The following table shows the properties that are required when you create the [androidForWorkVpnConfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md).</span></span>

|<span data-ttu-id="09f67-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="09f67-130">Property</span></span>|<span data-ttu-id="09f67-131">Typ</span><span class="sxs-lookup"><span data-stu-id="09f67-131">Type</span></span>|<span data-ttu-id="09f67-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="09f67-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="09f67-133">id</span><span class="sxs-lookup"><span data-stu-id="09f67-133">id</span></span>|<span data-ttu-id="09f67-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="09f67-134">String</span></span>|<span data-ttu-id="09f67-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="09f67-135">Key of the entity.</span></span> <span data-ttu-id="09f67-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="09f67-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="09f67-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="09f67-137">lastModifiedDateTime</span></span>|<span data-ttu-id="09f67-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="09f67-138">DateTimeOffset</span></span>|<span data-ttu-id="09f67-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="09f67-139">DateTime the object was last modified.</span></span> <span data-ttu-id="09f67-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="09f67-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="09f67-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="09f67-141">roleScopeTagIds</span></span>|<span data-ttu-id="09f67-142">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="09f67-142">String collection</span></span>|<span data-ttu-id="09f67-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="09f67-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="09f67-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="09f67-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="09f67-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="09f67-145">supportsScopeTags</span></span>|<span data-ttu-id="09f67-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="09f67-146">Boolean</span></span>|<span data-ttu-id="09f67-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="09f67-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="09f67-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="09f67-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="09f67-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="09f67-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="09f67-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="09f67-150">This property is read-only.</span></span> <span data-ttu-id="09f67-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="09f67-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="09f67-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="09f67-152">createdDateTime</span></span>|<span data-ttu-id="09f67-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="09f67-153">DateTimeOffset</span></span>|<span data-ttu-id="09f67-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="09f67-154">DateTime the object was created.</span></span> <span data-ttu-id="09f67-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="09f67-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="09f67-156">description</span><span class="sxs-lookup"><span data-stu-id="09f67-156">description</span></span>|<span data-ttu-id="09f67-157">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="09f67-157">String</span></span>|<span data-ttu-id="09f67-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="09f67-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="09f67-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="09f67-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="09f67-160">displayName</span><span class="sxs-lookup"><span data-stu-id="09f67-160">displayName</span></span>|<span data-ttu-id="09f67-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="09f67-161">String</span></span>|<span data-ttu-id="09f67-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="09f67-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="09f67-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="09f67-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="09f67-164">Version</span><span class="sxs-lookup"><span data-stu-id="09f67-164">version</span></span>|<span data-ttu-id="09f67-165">Int32</span><span class="sxs-lookup"><span data-stu-id="09f67-165">Int32</span></span>|<span data-ttu-id="09f67-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="09f67-166">Version of the device configuration.</span></span> <span data-ttu-id="09f67-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="09f67-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="09f67-168">connectionName</span><span class="sxs-lookup"><span data-stu-id="09f67-168">connectionName</span></span>|<span data-ttu-id="09f67-169">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="09f67-169">String</span></span>|<span data-ttu-id="09f67-170">Name der Verbindung für den Benutzer angezeigt.</span><span class="sxs-lookup"><span data-stu-id="09f67-170">Connection name displayed to the user.</span></span>|
|<span data-ttu-id="09f67-171">connectionType</span><span class="sxs-lookup"><span data-stu-id="09f67-171">connectionType</span></span>|[<span data-ttu-id="09f67-172">androidForWorkVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="09f67-172">androidForWorkVpnConnectionType</span></span>](../resources/intune-deviceconfig-androidforworkvpnconnectiontype.md)|<span data-ttu-id="09f67-173">Verbindungstyp.</span><span class="sxs-lookup"><span data-stu-id="09f67-173">Connection type.</span></span> <span data-ttu-id="09f67-174">Mögliche Werte sind: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn` und `citrix`.</span><span class="sxs-lookup"><span data-stu-id="09f67-174">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`.</span></span>|
|<span data-ttu-id="09f67-175">role</span><span class="sxs-lookup"><span data-stu-id="09f67-175">role</span></span>|<span data-ttu-id="09f67-176">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="09f67-176">String</span></span>|<span data-ttu-id="09f67-177">Rolle, wenn Verbindungstyp auf Pulse Secure festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="09f67-177">Role when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="09f67-178">Bereich</span><span class="sxs-lookup"><span data-stu-id="09f67-178">realm</span></span>|<span data-ttu-id="09f67-179">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="09f67-179">String</span></span>|<span data-ttu-id="09f67-180">Realm Wenn Verbindungstyp auf Pulse Secure festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="09f67-180">Realm when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="09f67-181">Server</span><span class="sxs-lookup"><span data-stu-id="09f67-181">servers</span></span>|<span data-ttu-id="09f67-182">[VpnServer](../resources/intune-deviceconfig-vpnserver.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="09f67-182">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="09f67-183">Liste der VPN-Server im Netzwerk.</span><span class="sxs-lookup"><span data-stu-id="09f67-183">List of VPN Servers on the network.</span></span> <span data-ttu-id="09f67-184">Stellen Sie sicher, dass Endbenutzer diese Netzwerkadressen zugreifen können.</span><span class="sxs-lookup"><span data-stu-id="09f67-184">Make sure end users can access these network locations.</span></span> <span data-ttu-id="09f67-185">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="09f67-185">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="09f67-186">Fingerabdruck</span><span class="sxs-lookup"><span data-stu-id="09f67-186">fingerprint</span></span>|<span data-ttu-id="09f67-187">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="09f67-187">String</span></span>|<span data-ttu-id="09f67-188">Fingerabdruck ist, dass eine Zeichenfolge, die zum Überprüfen des VPN-Servers verwendet wird, als vertrauenswürdig eingestuft werden kann die gilt nur bei Verbindungstyp Check Point "Kapseln" VPN ist.</span><span class="sxs-lookup"><span data-stu-id="09f67-188">Fingerprint is a string that will be used to verify the VPN server can be trusted, which is only applicable when connection type is Check Point Capsule VPN.</span></span>|
|<span data-ttu-id="09f67-189">customData</span><span class="sxs-lookup"><span data-stu-id="09f67-189">customData</span></span>|<span data-ttu-id="09f67-190">[KeyValue](../resources/intune-deviceconfig-keyvalue.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="09f67-190">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="09f67-191">Benutzerdefinierte Daten beim Verbindungstyp auf Citrix festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="09f67-191">Custom data when connection type is set to Citrix.</span></span> <span data-ttu-id="09f67-192">Diese Sammlung kann maximal 25 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="09f67-192">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="09f67-193">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="09f67-193">customKeyValueData</span></span>|<span data-ttu-id="09f67-194">[keyValuePair](../resources/intune-shared-keyvaluepair.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="09f67-194">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="09f67-195">Benutzerdefinierte Daten beim Verbindungstyp auf Citrix festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="09f67-195">Custom data when connection type is set to Citrix.</span></span> <span data-ttu-id="09f67-196">Diese Sammlung kann maximal 25 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="09f67-196">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="09f67-197">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="09f67-197">authenticationMethod</span></span>|[<span data-ttu-id="09f67-198">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="09f67-198">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="09f67-199">Authentifizierungsmethode.</span><span class="sxs-lookup"><span data-stu-id="09f67-199">Authentication method.</span></span> <span data-ttu-id="09f67-200">Mögliche Werte sind: `certificate` und `usernameAndPassword`.</span><span class="sxs-lookup"><span data-stu-id="09f67-200">Possible values are: `certificate`, `usernameAndPassword`.</span></span>|



## <a name="response"></a><span data-ttu-id="09f67-201">Antwort</span><span class="sxs-lookup"><span data-stu-id="09f67-201">Response</span></span>
<span data-ttu-id="09f67-202">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [AndroidForWorkVpnConfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="09f67-202">If successful, this method returns a `200 OK` response code and an updated [androidForWorkVpnConfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="09f67-203">Beispiel</span><span class="sxs-lookup"><span data-stu-id="09f67-203">Example</span></span>

### <a name="request"></a><span data-ttu-id="09f67-204">Anforderung</span><span class="sxs-lookup"><span data-stu-id="09f67-204">Request</span></span>
<span data-ttu-id="09f67-205">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="09f67-205">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 985

{
  "@odata.type": "#microsoft.graph.androidForWorkVpnConfiguration",
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

### <a name="response"></a><span data-ttu-id="09f67-206">Antwort</span><span class="sxs-lookup"><span data-stu-id="09f67-206">Response</span></span>
<span data-ttu-id="09f67-p116">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="09f67-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1157

{
  "@odata.type": "#microsoft.graph.androidForWorkVpnConfiguration",
  "id": "2cf4c52c-c52c-2cf4-2cc5-f42c2cc5f42c",
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




