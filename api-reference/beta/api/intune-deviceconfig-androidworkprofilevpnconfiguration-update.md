---
title: AndroidWorkProfileVpnConfiguration aktualisieren
description: Aktualisieren der Eigenschaften eines androidWorkProfileVpnConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 61ea061f5e6a1d1e9f9900ceb5de5ec8cabfd6da
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30164106"
---
# <a name="update-androidworkprofilevpnconfiguration"></a><span data-ttu-id="9bb4e-103">AndroidWorkProfileVpnConfiguration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="9bb4e-103">Update androidWorkProfileVpnConfiguration</span></span>

> <span data-ttu-id="9bb4e-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9bb4e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9bb4e-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="9bb4e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9bb4e-106">Aktualisieren der Eigenschaften eines [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="9bb4e-106">Update the properties of a [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9bb4e-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="9bb4e-107">Prerequisites</span></span>
<span data-ttu-id="9bb4e-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="9bb4e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="9bb4e-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9bb4e-110">Permission type</span></span>|<span data-ttu-id="9bb4e-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9bb4e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9bb4e-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9bb4e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9bb4e-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9bb4e-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9bb4e-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9bb4e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9bb4e-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9bb4e-115">Not supported.</span></span>|
|<span data-ttu-id="9bb4e-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9bb4e-116">Application</span></span>|<span data-ttu-id="9bb4e-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9bb4e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9bb4e-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9bb4e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="9bb4e-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9bb4e-119">Request headers</span></span>
|<span data-ttu-id="9bb4e-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="9bb4e-120">Header</span></span>|<span data-ttu-id="9bb4e-121">Wert</span><span class="sxs-lookup"><span data-stu-id="9bb4e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9bb4e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9bb4e-122">Authorization</span></span>|<span data-ttu-id="9bb4e-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="9bb4e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9bb4e-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="9bb4e-124">Accept</span></span>|<span data-ttu-id="9bb4e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9bb4e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9bb4e-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9bb4e-126">Request body</span></span>
<span data-ttu-id="9bb4e-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="9bb4e-127">In the request body, supply a JSON representation for the [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) object.</span></span>

<span data-ttu-id="9bb4e-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="9bb4e-128">The following table shows the properties that are required when you create the [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md).</span></span>

|<span data-ttu-id="9bb4e-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9bb4e-129">Property</span></span>|<span data-ttu-id="9bb4e-130">Typ</span><span class="sxs-lookup"><span data-stu-id="9bb4e-130">Type</span></span>|<span data-ttu-id="9bb4e-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9bb4e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9bb4e-132">id</span><span class="sxs-lookup"><span data-stu-id="9bb4e-132">id</span></span>|<span data-ttu-id="9bb4e-133">string</span><span class="sxs-lookup"><span data-stu-id="9bb4e-133">String</span></span>|<span data-ttu-id="9bb4e-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="9bb4e-134">Key of the entity.</span></span> <span data-ttu-id="9bb4e-135">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9bb4e-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9bb4e-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9bb4e-136">lastModifiedDateTime</span></span>|<span data-ttu-id="9bb4e-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9bb4e-137">DateTimeOffset</span></span>|<span data-ttu-id="9bb4e-138">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="9bb4e-138">DateTime the object was last modified.</span></span> <span data-ttu-id="9bb4e-139">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9bb4e-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9bb4e-140">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="9bb4e-140">roleScopeTagIds</span></span>|<span data-ttu-id="9bb4e-141">String collection</span><span class="sxs-lookup"><span data-stu-id="9bb4e-141">String collection</span></span>|<span data-ttu-id="9bb4e-142">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="9bb4e-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="9bb4e-143">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9bb4e-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9bb4e-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="9bb4e-144">supportsScopeTags</span></span>|<span data-ttu-id="9bb4e-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="9bb4e-145">Boolean</span></span>|<span data-ttu-id="9bb4e-146">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereichs Tags unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9bb4e-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="9bb4e-147">Das Zuweisen zur ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert auf false festgelegt ist und Entitäten für bereichsbezogene Benutzer nicht sichtbar sind.</span><span class="sxs-lookup"><span data-stu-id="9bb4e-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="9bb4e-148">Dies geschieht für in Silverlight erstellte Legacy Richtlinien und kann durch Löschen und erneutes Erstellen der Richtlinie im Azure-Portal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="9bb4e-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="9bb4e-149">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="9bb4e-149">This property is read-only.</span></span> <span data-ttu-id="9bb4e-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9bb4e-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9bb4e-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9bb4e-151">createdDateTime</span></span>|<span data-ttu-id="9bb4e-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9bb4e-152">DateTimeOffset</span></span>|<span data-ttu-id="9bb4e-153">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="9bb4e-153">DateTime the object was created.</span></span> <span data-ttu-id="9bb4e-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9bb4e-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9bb4e-155">description</span><span class="sxs-lookup"><span data-stu-id="9bb4e-155">description</span></span>|<span data-ttu-id="9bb4e-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9bb4e-156">String</span></span>|<span data-ttu-id="9bb4e-157">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="9bb4e-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="9bb4e-158">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9bb4e-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9bb4e-159">displayName</span><span class="sxs-lookup"><span data-stu-id="9bb4e-159">displayName</span></span>|<span data-ttu-id="9bb4e-160">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9bb4e-160">String</span></span>|<span data-ttu-id="9bb4e-161">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="9bb4e-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="9bb4e-162">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9bb4e-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9bb4e-163">Version</span><span class="sxs-lookup"><span data-stu-id="9bb4e-163">version</span></span>|<span data-ttu-id="9bb4e-164">Int32</span><span class="sxs-lookup"><span data-stu-id="9bb4e-164">Int32</span></span>|<span data-ttu-id="9bb4e-165">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="9bb4e-165">Version of the device configuration.</span></span> <span data-ttu-id="9bb4e-166">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9bb4e-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9bb4e-167">connectionName</span><span class="sxs-lookup"><span data-stu-id="9bb4e-167">connectionName</span></span>|<span data-ttu-id="9bb4e-168">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9bb4e-168">String</span></span>|<span data-ttu-id="9bb4e-169">Dem Benutzer angezeigter Verbindungsname.</span><span class="sxs-lookup"><span data-stu-id="9bb4e-169">Connection name displayed to the user.</span></span>|
|<span data-ttu-id="9bb4e-170">connectionType</span><span class="sxs-lookup"><span data-stu-id="9bb4e-170">connectionType</span></span>|[<span data-ttu-id="9bb4e-171">androidWorkProfileVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="9bb4e-171">androidWorkProfileVpnConnectionType</span></span>](../resources/intune-deviceconfig-androidworkprofilevpnconnectiontype.md)|<span data-ttu-id="9bb4e-172">Verbindungstyp.</span><span class="sxs-lookup"><span data-stu-id="9bb4e-172">Connection type.</span></span> <span data-ttu-id="9bb4e-173">Mögliche Werte sind: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix` und `paloAltoGlobalProtect`.</span><span class="sxs-lookup"><span data-stu-id="9bb4e-173">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`, `paloAltoGlobalProtect`.</span></span>|
|<span data-ttu-id="9bb4e-174">role</span><span class="sxs-lookup"><span data-stu-id="9bb4e-174">role</span></span>|<span data-ttu-id="9bb4e-175">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9bb4e-175">String</span></span>|<span data-ttu-id="9bb4e-176">Role, wenn der Verbindungstyp auf Pulse Secure festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="9bb4e-176">Role when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="9bb4e-177">Bereich</span><span class="sxs-lookup"><span data-stu-id="9bb4e-177">realm</span></span>|<span data-ttu-id="9bb4e-178">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9bb4e-178">String</span></span>|<span data-ttu-id="9bb4e-179">Bereich, wenn der Verbindungstyp auf Pulse Secure festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="9bb4e-179">Realm when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="9bb4e-180">Server</span><span class="sxs-lookup"><span data-stu-id="9bb4e-180">servers</span></span>|<span data-ttu-id="9bb4e-181">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="9bb4e-181">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="9bb4e-182">Liste der VPN-Server im Netzwerk.</span><span class="sxs-lookup"><span data-stu-id="9bb4e-182">List of VPN Servers on the network.</span></span> <span data-ttu-id="9bb4e-183">Stellen Sie sicher, dass Endbenutzer auf diese Netzwerkspeicherorte zugreifen können.</span><span class="sxs-lookup"><span data-stu-id="9bb4e-183">Make sure end users can access these network locations.</span></span> <span data-ttu-id="9bb4e-184">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="9bb4e-184">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="9bb4e-185">Fingerabdruck</span><span class="sxs-lookup"><span data-stu-id="9bb4e-185">fingerprint</span></span>|<span data-ttu-id="9bb4e-186">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9bb4e-186">String</span></span>|<span data-ttu-id="9bb4e-187">Fingerabdruck ist eine Zeichenfolge, die verwendet wird, um zu überprüfen, ob der VPN-Server vertrauenswürdig ist, was nur beim Verbindungstyp Check Point Capsule VPN gilt.</span><span class="sxs-lookup"><span data-stu-id="9bb4e-187">Fingerprint is a string that will be used to verify the VPN server can be trusted, which is only applicable when connection type is Check Point Capsule VPN.</span></span>|
|<span data-ttu-id="9bb4e-188">customData</span><span class="sxs-lookup"><span data-stu-id="9bb4e-188">customData</span></span>|<span data-ttu-id="9bb4e-189">[keyValue](../resources/intune-deviceconfig-keyvalue.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="9bb4e-189">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="9bb4e-190">Benutzerdefinierte Daten, wenn der Verbindungstyp auf Citrix festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="9bb4e-190">Custom data when connection type is set to Citrix.</span></span> <span data-ttu-id="9bb4e-191">Diese Auflistung kann maximal 25 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="9bb4e-191">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="9bb4e-192">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="9bb4e-192">customKeyValueData</span></span>|<span data-ttu-id="9bb4e-193">[keyValuePair](../resources/intune-shared-keyvaluepair.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="9bb4e-193">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="9bb4e-194">Benutzerdefinierte Daten, wenn der Verbindungstyp auf Citrix festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="9bb4e-194">Custom data when connection type is set to Citrix.</span></span> <span data-ttu-id="9bb4e-195">Diese Auflistung kann maximal 25 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="9bb4e-195">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="9bb4e-196">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="9bb4e-196">authenticationMethod</span></span>|[<span data-ttu-id="9bb4e-197">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="9bb4e-197">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="9bb4e-198">Authentifizierungsmethode.</span><span class="sxs-lookup"><span data-stu-id="9bb4e-198">Authentication method.</span></span> <span data-ttu-id="9bb4e-199">Mögliche Werte sind: `certificate` und `usernameAndPassword`.</span><span class="sxs-lookup"><span data-stu-id="9bb4e-199">Possible values are: `certificate`, `usernameAndPassword`.</span></span>|



## <a name="response"></a><span data-ttu-id="9bb4e-200">Antwort</span><span class="sxs-lookup"><span data-stu-id="9bb4e-200">Response</span></span>
<span data-ttu-id="9bb4e-201">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="9bb4e-201">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9bb4e-202">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9bb4e-202">Example</span></span>

### <a name="request"></a><span data-ttu-id="9bb4e-203">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9bb4e-203">Request</span></span>
<span data-ttu-id="9bb4e-204">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9bb4e-204">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="9bb4e-205">Antwort</span><span class="sxs-lookup"><span data-stu-id="9bb4e-205">Response</span></span>
<span data-ttu-id="9bb4e-p115">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9bb4e-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




