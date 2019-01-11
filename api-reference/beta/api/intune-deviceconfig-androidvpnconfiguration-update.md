---
title: AndroidVpnConfiguration aktualisieren
description: Aktualisieren Sie die Eigenschaften eines AndroidVpnConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 6ad88fff142a6c4b3827135a31a80171687a3940
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27812628"
---
# <a name="update-androidvpnconfiguration"></a><span data-ttu-id="b9568-103">AndroidVpnConfiguration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="b9568-103">Update androidVpnConfiguration</span></span>

> <span data-ttu-id="b9568-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b9568-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b9568-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b9568-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b9568-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="b9568-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b9568-107">Aktualisieren Sie die Eigenschaften eines [AndroidVpnConfiguration](../resources/intune-deviceconfig-androidvpnconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="b9568-107">Update the properties of a [androidVpnConfiguration](../resources/intune-deviceconfig-androidvpnconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b9568-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b9568-108">Prerequisites</span></span>
<span data-ttu-id="b9568-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b9568-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b9568-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b9568-111">Permission type</span></span>|<span data-ttu-id="b9568-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b9568-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b9568-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b9568-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b9568-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9568-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b9568-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b9568-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b9568-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b9568-116">Not supported.</span></span>|
|<span data-ttu-id="b9568-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b9568-117">Application</span></span>|<span data-ttu-id="b9568-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b9568-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b9568-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b9568-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="b9568-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b9568-120">Request headers</span></span>
|<span data-ttu-id="b9568-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="b9568-121">Header</span></span>|<span data-ttu-id="b9568-122">Wert</span><span class="sxs-lookup"><span data-stu-id="b9568-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b9568-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b9568-123">Authorization</span></span>|<span data-ttu-id="b9568-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b9568-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b9568-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="b9568-125">Accept</span></span>|<span data-ttu-id="b9568-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b9568-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b9568-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b9568-127">Request body</span></span>
<span data-ttu-id="b9568-128">Geben Sie im Textkörper Anforderung für das Objekt [AndroidVpnConfiguration](../resources/intune-deviceconfig-androidvpnconfiguration.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="b9568-128">In the request body, supply a JSON representation for the [androidVpnConfiguration](../resources/intune-deviceconfig-androidvpnconfiguration.md) object.</span></span>

<span data-ttu-id="b9568-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [AndroidVpnConfiguration](../resources/intune-deviceconfig-androidvpnconfiguration.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="b9568-129">The following table shows the properties that are required when you create the [androidVpnConfiguration](../resources/intune-deviceconfig-androidvpnconfiguration.md).</span></span>

|<span data-ttu-id="b9568-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b9568-130">Property</span></span>|<span data-ttu-id="b9568-131">Typ</span><span class="sxs-lookup"><span data-stu-id="b9568-131">Type</span></span>|<span data-ttu-id="b9568-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b9568-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b9568-133">id</span><span class="sxs-lookup"><span data-stu-id="b9568-133">id</span></span>|<span data-ttu-id="b9568-134">String</span><span class="sxs-lookup"><span data-stu-id="b9568-134">String</span></span>|<span data-ttu-id="b9568-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="b9568-135">Key of the entity.</span></span> <span data-ttu-id="b9568-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b9568-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b9568-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b9568-137">lastModifiedDateTime</span></span>|<span data-ttu-id="b9568-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b9568-138">DateTimeOffset</span></span>|<span data-ttu-id="b9568-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="b9568-139">DateTime the object was last modified.</span></span> <span data-ttu-id="b9568-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b9568-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b9568-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b9568-141">roleScopeTagIds</span></span>|<span data-ttu-id="b9568-142">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="b9568-142">String collection</span></span>|<span data-ttu-id="b9568-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="b9568-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b9568-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b9568-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b9568-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="b9568-145">supportsScopeTags</span></span>|<span data-ttu-id="b9568-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9568-146">Boolean</span></span>|<span data-ttu-id="b9568-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b9568-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="b9568-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="b9568-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="b9568-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="b9568-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="b9568-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="b9568-150">This property is read-only.</span></span> <span data-ttu-id="b9568-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b9568-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b9568-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b9568-152">createdDateTime</span></span>|<span data-ttu-id="b9568-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b9568-153">DateTimeOffset</span></span>|<span data-ttu-id="b9568-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="b9568-154">DateTime the object was created.</span></span> <span data-ttu-id="b9568-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b9568-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b9568-156">description</span><span class="sxs-lookup"><span data-stu-id="b9568-156">description</span></span>|<span data-ttu-id="b9568-157">String</span><span class="sxs-lookup"><span data-stu-id="b9568-157">String</span></span>|<span data-ttu-id="b9568-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="b9568-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b9568-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b9568-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b9568-160">displayName</span><span class="sxs-lookup"><span data-stu-id="b9568-160">displayName</span></span>|<span data-ttu-id="b9568-161">String</span><span class="sxs-lookup"><span data-stu-id="b9568-161">String</span></span>|<span data-ttu-id="b9568-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="b9568-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b9568-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b9568-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b9568-164">Version</span><span class="sxs-lookup"><span data-stu-id="b9568-164">version</span></span>|<span data-ttu-id="b9568-165">Int32</span><span class="sxs-lookup"><span data-stu-id="b9568-165">Int32</span></span>|<span data-ttu-id="b9568-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="b9568-166">Version of the device configuration.</span></span> <span data-ttu-id="b9568-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b9568-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b9568-168">connectionName</span><span class="sxs-lookup"><span data-stu-id="b9568-168">connectionName</span></span>|<span data-ttu-id="b9568-169">String</span><span class="sxs-lookup"><span data-stu-id="b9568-169">String</span></span>|<span data-ttu-id="b9568-170">Name der Verbindung für den Benutzer angezeigt.</span><span class="sxs-lookup"><span data-stu-id="b9568-170">Connection name displayed to the user.</span></span>|
|<span data-ttu-id="b9568-171">connectionType</span><span class="sxs-lookup"><span data-stu-id="b9568-171">connectionType</span></span>|[<span data-ttu-id="b9568-172">androidVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="b9568-172">androidVpnConnectionType</span></span>](../resources/intune-deviceconfig-androidvpnconnectiontype.md)|<span data-ttu-id="b9568-173">Verbindungstyp.</span><span class="sxs-lookup"><span data-stu-id="b9568-173">Connection type.</span></span> <span data-ttu-id="b9568-174">Mögliche Werte sind: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn` und `citrix`.</span><span class="sxs-lookup"><span data-stu-id="b9568-174">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`.</span></span>|
|<span data-ttu-id="b9568-175">role</span><span class="sxs-lookup"><span data-stu-id="b9568-175">role</span></span>|<span data-ttu-id="b9568-176">String</span><span class="sxs-lookup"><span data-stu-id="b9568-176">String</span></span>|<span data-ttu-id="b9568-177">Rolle, wenn Verbindungstyp auf Pulse Secure festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="b9568-177">Role when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="b9568-178">Bereich</span><span class="sxs-lookup"><span data-stu-id="b9568-178">realm</span></span>|<span data-ttu-id="b9568-179">String</span><span class="sxs-lookup"><span data-stu-id="b9568-179">String</span></span>|<span data-ttu-id="b9568-180">Realm Wenn Verbindungstyp auf Pulse Secure festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="b9568-180">Realm when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="b9568-181">Server</span><span class="sxs-lookup"><span data-stu-id="b9568-181">servers</span></span>|<span data-ttu-id="b9568-182">[VpnServer](../resources/intune-deviceconfig-vpnserver.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="b9568-182">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="b9568-183">Liste der VPN-Server im Netzwerk.</span><span class="sxs-lookup"><span data-stu-id="b9568-183">List of VPN Servers on the network.</span></span> <span data-ttu-id="b9568-184">Stellen Sie sicher, dass Endbenutzer diese Netzwerkadressen zugreifen können.</span><span class="sxs-lookup"><span data-stu-id="b9568-184">Make sure end users can access these network locations.</span></span> <span data-ttu-id="b9568-185">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="b9568-185">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="b9568-186">Fingerabdruck</span><span class="sxs-lookup"><span data-stu-id="b9568-186">fingerprint</span></span>|<span data-ttu-id="b9568-187">String</span><span class="sxs-lookup"><span data-stu-id="b9568-187">String</span></span>|<span data-ttu-id="b9568-188">Fingerabdruck ist, dass eine Zeichenfolge, die zum Überprüfen des VPN-Servers verwendet wird, als vertrauenswürdig eingestuft werden kann die gilt nur bei Verbindungstyp Check Point "Kapseln" VPN ist.</span><span class="sxs-lookup"><span data-stu-id="b9568-188">Fingerprint is a string that will be used to verify the VPN server can be trusted, which is only applicable when connection type is Check Point Capsule VPN.</span></span>|
|<span data-ttu-id="b9568-189">customData</span><span class="sxs-lookup"><span data-stu-id="b9568-189">customData</span></span>|<span data-ttu-id="b9568-190">[KeyValue](../resources/intune-deviceconfig-keyvalue.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="b9568-190">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="b9568-191">Benutzerdefinierte Daten beim Verbindungstyp auf Citrix festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="b9568-191">Custom data when connection type is set to Citrix.</span></span> <span data-ttu-id="b9568-192">Diese Sammlung kann maximal 25 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="b9568-192">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="b9568-193">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="b9568-193">customKeyValueData</span></span>|<span data-ttu-id="b9568-194">[keyValuePair](../resources/intune-shared-keyvaluepair.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="b9568-194">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="b9568-195">Benutzerdefinierte Daten beim Verbindungstyp auf Citrix festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="b9568-195">Custom data when connection type is set to Citrix.</span></span> <span data-ttu-id="b9568-196">Diese Sammlung kann maximal 25 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="b9568-196">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="b9568-197">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="b9568-197">authenticationMethod</span></span>|[<span data-ttu-id="b9568-198">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="b9568-198">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="b9568-199">Authentifizierungsmethode.</span><span class="sxs-lookup"><span data-stu-id="b9568-199">Authentication method.</span></span> <span data-ttu-id="b9568-200">Mögliche Werte sind: `certificate` und `usernameAndPassword`.</span><span class="sxs-lookup"><span data-stu-id="b9568-200">Possible values are: `certificate`, `usernameAndPassword`.</span></span>|



## <a name="response"></a><span data-ttu-id="b9568-201">Antwort</span><span class="sxs-lookup"><span data-stu-id="b9568-201">Response</span></span>
<span data-ttu-id="b9568-202">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [AndroidVpnConfiguration](../resources/intune-deviceconfig-androidvpnconfiguration.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="b9568-202">If successful, this method returns a `200 OK` response code and an updated [androidVpnConfiguration](../resources/intune-deviceconfig-androidvpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b9568-203">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b9568-203">Example</span></span>
### <a name="request"></a><span data-ttu-id="b9568-204">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b9568-204">Request</span></span>
<span data-ttu-id="b9568-205">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b9568-205">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 980

{
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

### <a name="response"></a><span data-ttu-id="b9568-206">Antwort</span><span class="sxs-lookup"><span data-stu-id="b9568-206">Response</span></span>
<span data-ttu-id="b9568-p116">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b9568-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1150

{
  "@odata.type": "#microsoft.graph.androidVpnConfiguration",
  "id": "d4c48852-8852-d4c4-5288-c4d45288c4d4",
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





