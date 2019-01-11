---
title: AndroidWorkProfileVpnConfiguration aktualisieren
description: Aktualisieren Sie die Eigenschaften eines AndroidWorkProfileVpnConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 6c1ff2e73ce14568d1ce7c725db1ffc3ae206d64
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27868894"
---
# <a name="update-androidworkprofilevpnconfiguration"></a><span data-ttu-id="ea8e1-103">AndroidWorkProfileVpnConfiguration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="ea8e1-103">Update androidWorkProfileVpnConfiguration</span></span>

> <span data-ttu-id="ea8e1-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="ea8e1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ea8e1-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ea8e1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ea8e1-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="ea8e1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ea8e1-107">Aktualisieren Sie die Eigenschaften eines [AndroidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="ea8e1-107">Update the properties of a [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ea8e1-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="ea8e1-108">Prerequisites</span></span>
<span data-ttu-id="ea8e1-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ea8e1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ea8e1-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ea8e1-111">Permission type</span></span>|<span data-ttu-id="ea8e1-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ea8e1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ea8e1-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ea8e1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ea8e1-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea8e1-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ea8e1-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ea8e1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ea8e1-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ea8e1-116">Not supported.</span></span>|
|<span data-ttu-id="ea8e1-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ea8e1-117">Application</span></span>|<span data-ttu-id="ea8e1-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ea8e1-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ea8e1-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ea8e1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="ea8e1-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ea8e1-120">Request headers</span></span>
|<span data-ttu-id="ea8e1-121">Header</span><span class="sxs-lookup"><span data-stu-id="ea8e1-121">Header</span></span>|<span data-ttu-id="ea8e1-122">Wert</span><span class="sxs-lookup"><span data-stu-id="ea8e1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ea8e1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ea8e1-123">Authorization</span></span>|<span data-ttu-id="ea8e1-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="ea8e1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ea8e1-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="ea8e1-125">Accept</span></span>|<span data-ttu-id="ea8e1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ea8e1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ea8e1-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ea8e1-127">Request body</span></span>
<span data-ttu-id="ea8e1-128">Geben Sie im Textkörper Anforderung für das Objekt [AndroidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="ea8e1-128">In the request body, supply a JSON representation for the [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) object.</span></span>

<span data-ttu-id="ea8e1-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [AndroidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="ea8e1-129">The following table shows the properties that are required when you create the [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md).</span></span>

|<span data-ttu-id="ea8e1-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ea8e1-130">Property</span></span>|<span data-ttu-id="ea8e1-131">Typ</span><span class="sxs-lookup"><span data-stu-id="ea8e1-131">Type</span></span>|<span data-ttu-id="ea8e1-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ea8e1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ea8e1-133">id</span><span class="sxs-lookup"><span data-stu-id="ea8e1-133">id</span></span>|<span data-ttu-id="ea8e1-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ea8e1-134">String</span></span>|<span data-ttu-id="ea8e1-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="ea8e1-135">Key of the entity.</span></span> <span data-ttu-id="ea8e1-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ea8e1-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ea8e1-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ea8e1-137">lastModifiedDateTime</span></span>|<span data-ttu-id="ea8e1-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ea8e1-138">DateTimeOffset</span></span>|<span data-ttu-id="ea8e1-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="ea8e1-139">DateTime the object was last modified.</span></span> <span data-ttu-id="ea8e1-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ea8e1-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ea8e1-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ea8e1-141">roleScopeTagIds</span></span>|<span data-ttu-id="ea8e1-142">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="ea8e1-142">String collection</span></span>|<span data-ttu-id="ea8e1-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="ea8e1-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ea8e1-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ea8e1-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ea8e1-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="ea8e1-145">supportsScopeTags</span></span>|<span data-ttu-id="ea8e1-146">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="ea8e1-146">Boolean</span></span>|<span data-ttu-id="ea8e1-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ea8e1-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="ea8e1-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="ea8e1-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="ea8e1-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="ea8e1-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="ea8e1-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="ea8e1-150">This property is read-only.</span></span> <span data-ttu-id="ea8e1-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ea8e1-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ea8e1-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ea8e1-152">createdDateTime</span></span>|<span data-ttu-id="ea8e1-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ea8e1-153">DateTimeOffset</span></span>|<span data-ttu-id="ea8e1-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="ea8e1-154">DateTime the object was created.</span></span> <span data-ttu-id="ea8e1-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ea8e1-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ea8e1-156">description</span><span class="sxs-lookup"><span data-stu-id="ea8e1-156">description</span></span>|<span data-ttu-id="ea8e1-157">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ea8e1-157">String</span></span>|<span data-ttu-id="ea8e1-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="ea8e1-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ea8e1-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ea8e1-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ea8e1-160">displayName</span><span class="sxs-lookup"><span data-stu-id="ea8e1-160">displayName</span></span>|<span data-ttu-id="ea8e1-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ea8e1-161">String</span></span>|<span data-ttu-id="ea8e1-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="ea8e1-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ea8e1-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ea8e1-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ea8e1-164">Version</span><span class="sxs-lookup"><span data-stu-id="ea8e1-164">version</span></span>|<span data-ttu-id="ea8e1-165">Int32</span><span class="sxs-lookup"><span data-stu-id="ea8e1-165">Int32</span></span>|<span data-ttu-id="ea8e1-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="ea8e1-166">Version of the device configuration.</span></span> <span data-ttu-id="ea8e1-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ea8e1-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ea8e1-168">connectionName</span><span class="sxs-lookup"><span data-stu-id="ea8e1-168">connectionName</span></span>|<span data-ttu-id="ea8e1-169">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ea8e1-169">String</span></span>|<span data-ttu-id="ea8e1-170">Name der Verbindung für den Benutzer angezeigt.</span><span class="sxs-lookup"><span data-stu-id="ea8e1-170">Connection name displayed to the user.</span></span>|
|<span data-ttu-id="ea8e1-171">connectionType</span><span class="sxs-lookup"><span data-stu-id="ea8e1-171">connectionType</span></span>|[<span data-ttu-id="ea8e1-172">androidWorkProfileVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="ea8e1-172">androidWorkProfileVpnConnectionType</span></span>](../resources/intune-deviceconfig-androidworkprofilevpnconnectiontype.md)|<span data-ttu-id="ea8e1-173">Verbindungstyp.</span><span class="sxs-lookup"><span data-stu-id="ea8e1-173">Connection type.</span></span> <span data-ttu-id="ea8e1-174">Mögliche Werte sind: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix` und `paloAltoGlobalProtect`.</span><span class="sxs-lookup"><span data-stu-id="ea8e1-174">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`, `paloAltoGlobalProtect`.</span></span>|
|<span data-ttu-id="ea8e1-175">role</span><span class="sxs-lookup"><span data-stu-id="ea8e1-175">role</span></span>|<span data-ttu-id="ea8e1-176">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ea8e1-176">String</span></span>|<span data-ttu-id="ea8e1-177">Rolle, wenn Verbindungstyp auf Pulse Secure festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="ea8e1-177">Role when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="ea8e1-178">Bereich</span><span class="sxs-lookup"><span data-stu-id="ea8e1-178">realm</span></span>|<span data-ttu-id="ea8e1-179">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ea8e1-179">String</span></span>|<span data-ttu-id="ea8e1-180">Realm Wenn Verbindungstyp auf Pulse Secure festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="ea8e1-180">Realm when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="ea8e1-181">Server</span><span class="sxs-lookup"><span data-stu-id="ea8e1-181">servers</span></span>|<span data-ttu-id="ea8e1-182">[VpnServer](../resources/intune-deviceconfig-vpnserver.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="ea8e1-182">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="ea8e1-183">Liste der VPN-Server im Netzwerk.</span><span class="sxs-lookup"><span data-stu-id="ea8e1-183">List of VPN Servers on the network.</span></span> <span data-ttu-id="ea8e1-184">Stellen Sie sicher, dass Endbenutzer diese Netzwerkadressen zugreifen können.</span><span class="sxs-lookup"><span data-stu-id="ea8e1-184">Make sure end users can access these network locations.</span></span> <span data-ttu-id="ea8e1-185">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="ea8e1-185">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="ea8e1-186">Fingerabdruck</span><span class="sxs-lookup"><span data-stu-id="ea8e1-186">fingerprint</span></span>|<span data-ttu-id="ea8e1-187">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ea8e1-187">String</span></span>|<span data-ttu-id="ea8e1-188">Fingerabdruck ist, dass eine Zeichenfolge, die zum Überprüfen des VPN-Servers verwendet wird, als vertrauenswürdig eingestuft werden kann die gilt nur bei Verbindungstyp Check Point "Kapseln" VPN ist.</span><span class="sxs-lookup"><span data-stu-id="ea8e1-188">Fingerprint is a string that will be used to verify the VPN server can be trusted, which is only applicable when connection type is Check Point Capsule VPN.</span></span>|
|<span data-ttu-id="ea8e1-189">customData</span><span class="sxs-lookup"><span data-stu-id="ea8e1-189">customData</span></span>|<span data-ttu-id="ea8e1-190">[KeyValue](../resources/intune-deviceconfig-keyvalue.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="ea8e1-190">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="ea8e1-191">Benutzerdefinierte Daten beim Verbindungstyp auf Citrix festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="ea8e1-191">Custom data when connection type is set to Citrix.</span></span> <span data-ttu-id="ea8e1-192">Diese Sammlung kann maximal 25 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="ea8e1-192">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="ea8e1-193">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="ea8e1-193">customKeyValueData</span></span>|<span data-ttu-id="ea8e1-194">[keyValuePair](../resources/intune-shared-keyvaluepair.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="ea8e1-194">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="ea8e1-195">Benutzerdefinierte Daten beim Verbindungstyp auf Citrix festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="ea8e1-195">Custom data when connection type is set to Citrix.</span></span> <span data-ttu-id="ea8e1-196">Diese Sammlung kann maximal 25 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="ea8e1-196">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="ea8e1-197">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="ea8e1-197">authenticationMethod</span></span>|[<span data-ttu-id="ea8e1-198">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="ea8e1-198">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="ea8e1-199">Authentifizierungsmethode.</span><span class="sxs-lookup"><span data-stu-id="ea8e1-199">Authentication method.</span></span> <span data-ttu-id="ea8e1-200">Mögliche Werte sind: `certificate` und `usernameAndPassword`.</span><span class="sxs-lookup"><span data-stu-id="ea8e1-200">Possible values are: `certificate`, `usernameAndPassword`.</span></span>|



## <a name="response"></a><span data-ttu-id="ea8e1-201">Antwort</span><span class="sxs-lookup"><span data-stu-id="ea8e1-201">Response</span></span>
<span data-ttu-id="ea8e1-202">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [AndroidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="ea8e1-202">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ea8e1-203">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ea8e1-203">Example</span></span>
### <a name="request"></a><span data-ttu-id="ea8e1-204">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ea8e1-204">Request</span></span>
<span data-ttu-id="ea8e1-205">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ea8e1-205">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ea8e1-206">Antwort</span><span class="sxs-lookup"><span data-stu-id="ea8e1-206">Response</span></span>
<span data-ttu-id="ea8e1-p116">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ea8e1-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





