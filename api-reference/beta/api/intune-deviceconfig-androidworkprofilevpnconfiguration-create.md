---
title: AndroidWorkProfileVpnConfiguration erstellen
description: Erstellen eines neuen androidWorkProfileVpnConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: aabfed08848f0c3e68fadb557051afa48596e80f
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30140768"
---
# <a name="create-androidworkprofilevpnconfiguration"></a><span data-ttu-id="33d21-103">AndroidWorkProfileVpnConfiguration erstellen</span><span class="sxs-lookup"><span data-stu-id="33d21-103">Create androidWorkProfileVpnConfiguration</span></span>

> <span data-ttu-id="33d21-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="33d21-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="33d21-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="33d21-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="33d21-106">Erstellen eines neuen [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="33d21-106">Create a new [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="33d21-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="33d21-107">Prerequisites</span></span>
<span data-ttu-id="33d21-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="33d21-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="33d21-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="33d21-110">Permission type</span></span>|<span data-ttu-id="33d21-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="33d21-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="33d21-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="33d21-112">Delegated (work or school account)</span></span>|<span data-ttu-id="33d21-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="33d21-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="33d21-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="33d21-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="33d21-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="33d21-115">Not supported.</span></span>|
|<span data-ttu-id="33d21-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="33d21-116">Application</span></span>|<span data-ttu-id="33d21-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="33d21-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="33d21-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="33d21-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="33d21-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="33d21-119">Request headers</span></span>
|<span data-ttu-id="33d21-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="33d21-120">Header</span></span>|<span data-ttu-id="33d21-121">Wert</span><span class="sxs-lookup"><span data-stu-id="33d21-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="33d21-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="33d21-122">Authorization</span></span>|<span data-ttu-id="33d21-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="33d21-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="33d21-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="33d21-124">Accept</span></span>|<span data-ttu-id="33d21-125">application/json</span><span class="sxs-lookup"><span data-stu-id="33d21-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="33d21-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="33d21-126">Request body</span></span>
<span data-ttu-id="33d21-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das androidWorkProfileVpnConfiguration-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="33d21-127">In the request body, supply a JSON representation for the androidWorkProfileVpnConfiguration object.</span></span>

<span data-ttu-id="33d21-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der androidWorkProfileVpnConfiguration erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="33d21-128">The following table shows the properties that are required when you create the androidWorkProfileVpnConfiguration.</span></span>

|<span data-ttu-id="33d21-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="33d21-129">Property</span></span>|<span data-ttu-id="33d21-130">Typ</span><span class="sxs-lookup"><span data-stu-id="33d21-130">Type</span></span>|<span data-ttu-id="33d21-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="33d21-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="33d21-132">id</span><span class="sxs-lookup"><span data-stu-id="33d21-132">id</span></span>|<span data-ttu-id="33d21-133">string</span><span class="sxs-lookup"><span data-stu-id="33d21-133">String</span></span>|<span data-ttu-id="33d21-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="33d21-134">Key of the entity.</span></span> <span data-ttu-id="33d21-135">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="33d21-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="33d21-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="33d21-136">lastModifiedDateTime</span></span>|<span data-ttu-id="33d21-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="33d21-137">DateTimeOffset</span></span>|<span data-ttu-id="33d21-138">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="33d21-138">DateTime the object was last modified.</span></span> <span data-ttu-id="33d21-139">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="33d21-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="33d21-140">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="33d21-140">roleScopeTagIds</span></span>|<span data-ttu-id="33d21-141">String collection</span><span class="sxs-lookup"><span data-stu-id="33d21-141">String collection</span></span>|<span data-ttu-id="33d21-142">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="33d21-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="33d21-143">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="33d21-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="33d21-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="33d21-144">supportsScopeTags</span></span>|<span data-ttu-id="33d21-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="33d21-145">Boolean</span></span>|<span data-ttu-id="33d21-146">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereichs Tags unterstützt.</span><span class="sxs-lookup"><span data-stu-id="33d21-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="33d21-147">Das Zuweisen zur ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert auf false festgelegt ist und Entitäten für bereichsbezogene Benutzer nicht sichtbar sind.</span><span class="sxs-lookup"><span data-stu-id="33d21-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="33d21-148">Dies geschieht für in Silverlight erstellte Legacy Richtlinien und kann durch Löschen und erneutes Erstellen der Richtlinie im Azure-Portal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="33d21-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="33d21-149">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="33d21-149">This property is read-only.</span></span> <span data-ttu-id="33d21-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="33d21-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="33d21-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="33d21-151">createdDateTime</span></span>|<span data-ttu-id="33d21-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="33d21-152">DateTimeOffset</span></span>|<span data-ttu-id="33d21-153">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="33d21-153">DateTime the object was created.</span></span> <span data-ttu-id="33d21-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="33d21-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="33d21-155">description</span><span class="sxs-lookup"><span data-stu-id="33d21-155">description</span></span>|<span data-ttu-id="33d21-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="33d21-156">String</span></span>|<span data-ttu-id="33d21-157">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="33d21-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="33d21-158">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="33d21-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="33d21-159">displayName</span><span class="sxs-lookup"><span data-stu-id="33d21-159">displayName</span></span>|<span data-ttu-id="33d21-160">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="33d21-160">String</span></span>|<span data-ttu-id="33d21-161">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="33d21-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="33d21-162">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="33d21-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="33d21-163">Version</span><span class="sxs-lookup"><span data-stu-id="33d21-163">version</span></span>|<span data-ttu-id="33d21-164">Int32</span><span class="sxs-lookup"><span data-stu-id="33d21-164">Int32</span></span>|<span data-ttu-id="33d21-165">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="33d21-165">Version of the device configuration.</span></span> <span data-ttu-id="33d21-166">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="33d21-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="33d21-167">connectionName</span><span class="sxs-lookup"><span data-stu-id="33d21-167">connectionName</span></span>|<span data-ttu-id="33d21-168">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="33d21-168">String</span></span>|<span data-ttu-id="33d21-169">Dem Benutzer angezeigter Verbindungsname.</span><span class="sxs-lookup"><span data-stu-id="33d21-169">Connection name displayed to the user.</span></span>|
|<span data-ttu-id="33d21-170">connectionType</span><span class="sxs-lookup"><span data-stu-id="33d21-170">connectionType</span></span>|[<span data-ttu-id="33d21-171">androidWorkProfileVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="33d21-171">androidWorkProfileVpnConnectionType</span></span>](../resources/intune-deviceconfig-androidworkprofilevpnconnectiontype.md)|<span data-ttu-id="33d21-172">Verbindungstyp.</span><span class="sxs-lookup"><span data-stu-id="33d21-172">Connection type.</span></span> <span data-ttu-id="33d21-173">Mögliche Werte sind: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix` und `paloAltoGlobalProtect`.</span><span class="sxs-lookup"><span data-stu-id="33d21-173">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`, `paloAltoGlobalProtect`.</span></span>|
|<span data-ttu-id="33d21-174">role</span><span class="sxs-lookup"><span data-stu-id="33d21-174">role</span></span>|<span data-ttu-id="33d21-175">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="33d21-175">String</span></span>|<span data-ttu-id="33d21-176">Role, wenn der Verbindungstyp auf Pulse Secure festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="33d21-176">Role when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="33d21-177">Bereich</span><span class="sxs-lookup"><span data-stu-id="33d21-177">realm</span></span>|<span data-ttu-id="33d21-178">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="33d21-178">String</span></span>|<span data-ttu-id="33d21-179">Bereich, wenn der Verbindungstyp auf Pulse Secure festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="33d21-179">Realm when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="33d21-180">Server</span><span class="sxs-lookup"><span data-stu-id="33d21-180">servers</span></span>|<span data-ttu-id="33d21-181">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="33d21-181">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="33d21-182">Liste der VPN-Server im Netzwerk.</span><span class="sxs-lookup"><span data-stu-id="33d21-182">List of VPN Servers on the network.</span></span> <span data-ttu-id="33d21-183">Stellen Sie sicher, dass Endbenutzer auf diese Netzwerkspeicherorte zugreifen können.</span><span class="sxs-lookup"><span data-stu-id="33d21-183">Make sure end users can access these network locations.</span></span> <span data-ttu-id="33d21-184">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="33d21-184">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="33d21-185">Fingerabdruck</span><span class="sxs-lookup"><span data-stu-id="33d21-185">fingerprint</span></span>|<span data-ttu-id="33d21-186">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="33d21-186">String</span></span>|<span data-ttu-id="33d21-187">Fingerabdruck ist eine Zeichenfolge, die verwendet wird, um zu überprüfen, ob der VPN-Server vertrauenswürdig ist, was nur beim Verbindungstyp Check Point Capsule VPN gilt.</span><span class="sxs-lookup"><span data-stu-id="33d21-187">Fingerprint is a string that will be used to verify the VPN server can be trusted, which is only applicable when connection type is Check Point Capsule VPN.</span></span>|
|<span data-ttu-id="33d21-188">customData</span><span class="sxs-lookup"><span data-stu-id="33d21-188">customData</span></span>|<span data-ttu-id="33d21-189">[keyValue](../resources/intune-deviceconfig-keyvalue.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="33d21-189">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="33d21-190">Benutzerdefinierte Daten, wenn der Verbindungstyp auf Citrix festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="33d21-190">Custom data when connection type is set to Citrix.</span></span> <span data-ttu-id="33d21-191">Diese Auflistung kann maximal 25 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="33d21-191">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="33d21-192">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="33d21-192">customKeyValueData</span></span>|<span data-ttu-id="33d21-193">[keyValuePair](../resources/intune-shared-keyvaluepair.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="33d21-193">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="33d21-194">Benutzerdefinierte Daten, wenn der Verbindungstyp auf Citrix festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="33d21-194">Custom data when connection type is set to Citrix.</span></span> <span data-ttu-id="33d21-195">Diese Auflistung kann maximal 25 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="33d21-195">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="33d21-196">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="33d21-196">authenticationMethod</span></span>|[<span data-ttu-id="33d21-197">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="33d21-197">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="33d21-198">Authentifizierungsmethode.</span><span class="sxs-lookup"><span data-stu-id="33d21-198">Authentication method.</span></span> <span data-ttu-id="33d21-199">Mögliche Werte sind: `certificate` und `usernameAndPassword`.</span><span class="sxs-lookup"><span data-stu-id="33d21-199">Possible values are: `certificate`, `usernameAndPassword`.</span></span>|



## <a name="response"></a><span data-ttu-id="33d21-200">Antwort</span><span class="sxs-lookup"><span data-stu-id="33d21-200">Response</span></span>
<span data-ttu-id="33d21-201">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="33d21-201">If successful, this method returns a `201 Created` response code and a [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="33d21-202">Beispiel</span><span class="sxs-lookup"><span data-stu-id="33d21-202">Example</span></span>

### <a name="request"></a><span data-ttu-id="33d21-203">Anforderung</span><span class="sxs-lookup"><span data-stu-id="33d21-203">Request</span></span>
<span data-ttu-id="33d21-204">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="33d21-204">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="33d21-205">Antwort</span><span class="sxs-lookup"><span data-stu-id="33d21-205">Response</span></span>
<span data-ttu-id="33d21-p115">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="33d21-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




