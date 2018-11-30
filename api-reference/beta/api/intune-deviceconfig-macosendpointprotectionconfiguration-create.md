---
title: Erstellen von macOSEndpointProtectionConfiguration
description: Erstellen eines neuen MacOSEndpointProtectionConfiguration-Objekts.
ms.openlocfilehash: 9f34936359cb3bee08a3427669bc1bc0c2fb7ac2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062763"
---
# <a name="create-macosendpointprotectionconfiguration"></a><span data-ttu-id="19e60-103">Erstellen von macOSEndpointProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="19e60-103">Create macOSEndpointProtectionConfiguration</span></span>

> <span data-ttu-id="19e60-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="19e60-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="19e60-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="19e60-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="19e60-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="19e60-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="19e60-107">Erstellen eines neuen [MacOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="19e60-107">Create a new [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="19e60-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="19e60-108">Prerequisites</span></span>
<span data-ttu-id="19e60-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="19e60-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="19e60-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="19e60-111">Permission type</span></span>|<span data-ttu-id="19e60-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="19e60-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="19e60-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="19e60-113">Delegated (work or school account)</span></span>|<span data-ttu-id="19e60-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="19e60-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="19e60-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="19e60-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="19e60-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="19e60-116">Not supported.</span></span>|
|<span data-ttu-id="19e60-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="19e60-117">Application</span></span>|<span data-ttu-id="19e60-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="19e60-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="19e60-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="19e60-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="19e60-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="19e60-120">Request headers</span></span>
|<span data-ttu-id="19e60-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="19e60-121">Header</span></span>|<span data-ttu-id="19e60-122">Wert</span><span class="sxs-lookup"><span data-stu-id="19e60-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="19e60-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="19e60-123">Authorization</span></span>|<span data-ttu-id="19e60-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="19e60-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="19e60-125">Accept</span><span class="sxs-lookup"><span data-stu-id="19e60-125">Accept</span></span>|<span data-ttu-id="19e60-126">application/json</span><span class="sxs-lookup"><span data-stu-id="19e60-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="19e60-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="19e60-127">Request body</span></span>
<span data-ttu-id="19e60-128">Geben Sie im Textkörper Anforderung für das Objekt MacOSEndpointProtectionConfiguration eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="19e60-128">In the request body, supply a JSON representation for the macOSEndpointProtectionConfiguration object.</span></span>

<span data-ttu-id="19e60-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die MacOSEndpointProtectionConfiguration erstellen.</span><span class="sxs-lookup"><span data-stu-id="19e60-129">The following table shows the properties that are required when you create the macOSEndpointProtectionConfiguration.</span></span>

|<span data-ttu-id="19e60-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="19e60-130">Property</span></span>|<span data-ttu-id="19e60-131">Typ</span><span class="sxs-lookup"><span data-stu-id="19e60-131">Type</span></span>|<span data-ttu-id="19e60-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="19e60-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="19e60-133">id</span><span class="sxs-lookup"><span data-stu-id="19e60-133">id</span></span>|<span data-ttu-id="19e60-134">String</span><span class="sxs-lookup"><span data-stu-id="19e60-134">String</span></span>|<span data-ttu-id="19e60-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="19e60-135">Key of the entity.</span></span> <span data-ttu-id="19e60-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="19e60-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="19e60-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="19e60-137">lastModifiedDateTime</span></span>|<span data-ttu-id="19e60-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="19e60-138">DateTimeOffset</span></span>|<span data-ttu-id="19e60-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="19e60-139">DateTime the object was last modified.</span></span> <span data-ttu-id="19e60-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="19e60-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="19e60-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="19e60-141">roleScopeTagIds</span></span>|<span data-ttu-id="19e60-142">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="19e60-142">String collection</span></span>|<span data-ttu-id="19e60-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="19e60-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="19e60-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="19e60-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="19e60-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="19e60-145">supportsScopeTags</span></span>|<span data-ttu-id="19e60-146">Boolesch</span><span class="sxs-lookup"><span data-stu-id="19e60-146">Boolean</span></span>|<span data-ttu-id="19e60-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="19e60-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="19e60-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="19e60-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="19e60-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="19e60-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="19e60-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="19e60-150">This property is read-only.</span></span> <span data-ttu-id="19e60-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="19e60-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="19e60-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="19e60-152">createdDateTime</span></span>|<span data-ttu-id="19e60-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="19e60-153">DateTimeOffset</span></span>|<span data-ttu-id="19e60-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="19e60-154">DateTime the object was created.</span></span> <span data-ttu-id="19e60-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="19e60-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="19e60-156">description</span><span class="sxs-lookup"><span data-stu-id="19e60-156">description</span></span>|<span data-ttu-id="19e60-157">String</span><span class="sxs-lookup"><span data-stu-id="19e60-157">String</span></span>|<span data-ttu-id="19e60-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="19e60-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="19e60-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="19e60-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="19e60-160">displayName</span><span class="sxs-lookup"><span data-stu-id="19e60-160">displayName</span></span>|<span data-ttu-id="19e60-161">String</span><span class="sxs-lookup"><span data-stu-id="19e60-161">String</span></span>|<span data-ttu-id="19e60-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="19e60-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="19e60-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="19e60-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="19e60-164">Version</span><span class="sxs-lookup"><span data-stu-id="19e60-164">version</span></span>|<span data-ttu-id="19e60-165">Int32</span><span class="sxs-lookup"><span data-stu-id="19e60-165">Int32</span></span>|<span data-ttu-id="19e60-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="19e60-166">Version of the device configuration.</span></span> <span data-ttu-id="19e60-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="19e60-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="19e60-168">gatekeeperAllowedAppSource</span><span class="sxs-lookup"><span data-stu-id="19e60-168">gatekeeperAllowedAppSource</span></span>|[<span data-ttu-id="19e60-169">macOSGatekeeperAppSources</span><span class="sxs-lookup"><span data-stu-id="19e60-169">macOSGatekeeperAppSources</span></span>](../resources/intune-deviceconfig-macosgatekeeperappsources.md)|<span data-ttu-id="19e60-170">System und den Datenschutz, der bestimmt, welche Download Speicherorte apps auf einem Mac OS-Gerät aus ausgeführt werden können.</span><span class="sxs-lookup"><span data-stu-id="19e60-170">System and Privacy setting that determines which download locations apps can be run from on a macOS device.</span></span> <span data-ttu-id="19e60-171">Mögliche Werte: sind `notConfigured`, `macAppStore`, `macAppStoreAndIdentifiedDevelopers` und `anywhere`.</span><span class="sxs-lookup"><span data-stu-id="19e60-171">Possible values are: `notConfigured`, `macAppStore`, `macAppStoreAndIdentifiedDevelopers`, `anywhere`.</span></span>|
|<span data-ttu-id="19e60-172">gatekeeperBlockOverride</span><span class="sxs-lookup"><span data-stu-id="19e60-172">gatekeeperBlockOverride</span></span>|<span data-ttu-id="19e60-173">Boolesch</span><span class="sxs-lookup"><span data-stu-id="19e60-173">Boolean</span></span>|<span data-ttu-id="19e60-174">Wenn auf True festgelegt, der Benutzer außer Kraft setzen für Gatekeeper deaktiviert wird.</span><span class="sxs-lookup"><span data-stu-id="19e60-174">If set to true, the user override for Gatekeeper will be disabled.</span></span>|
|<span data-ttu-id="19e60-175">firewallEnabled</span><span class="sxs-lookup"><span data-stu-id="19e60-175">firewallEnabled</span></span>|<span data-ttu-id="19e60-176">Boolesch</span><span class="sxs-lookup"><span data-stu-id="19e60-176">Boolean</span></span>|<span data-ttu-id="19e60-177">Gibt an, ob die Firewall oder nicht aktiviert werden soll.</span><span class="sxs-lookup"><span data-stu-id="19e60-177">Whether the firewall should be enabled or not.</span></span>|
|<span data-ttu-id="19e60-178">firewallBlockAllIncoming</span><span class="sxs-lookup"><span data-stu-id="19e60-178">firewallBlockAllIncoming</span></span>|<span data-ttu-id="19e60-179">Boolesch</span><span class="sxs-lookup"><span data-stu-id="19e60-179">Boolean</span></span>|<span data-ttu-id="19e60-180">Entspricht der Option "Alle eingehende Verbindungen blockieren".</span><span class="sxs-lookup"><span data-stu-id="19e60-180">Corresponds to the “Block all incoming connections” option.</span></span>|
|<span data-ttu-id="19e60-181">firewallEnableStealthMode</span><span class="sxs-lookup"><span data-stu-id="19e60-181">firewallEnableStealthMode</span></span>|<span data-ttu-id="19e60-182">Boolesch</span><span class="sxs-lookup"><span data-stu-id="19e60-182">Boolean</span></span>|<span data-ttu-id="19e60-183">Entspricht "Enable Tarnmodus."</span><span class="sxs-lookup"><span data-stu-id="19e60-183">Corresponds to “Enable stealth mode.”</span></span>|
|<span data-ttu-id="19e60-184">firewallApplications</span><span class="sxs-lookup"><span data-stu-id="19e60-184">firewallApplications</span></span>|<span data-ttu-id="19e60-185">[MacOSFirewallApplication](../resources/intune-deviceconfig-macosfirewallapplication.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="19e60-185">[macOSFirewallApplication](../resources/intune-deviceconfig-macosfirewallapplication.md) collection</span></span>|<span data-ttu-id="19e60-186">Liste von Anwendungen mit Firewalleinstellungen.</span><span class="sxs-lookup"><span data-stu-id="19e60-186">List of applications with firewall settings.</span></span> <span data-ttu-id="19e60-187">Firewalleinstellungen für Applikationen nicht in dieser Liste werden vom Benutzer festgelegt.</span><span class="sxs-lookup"><span data-stu-id="19e60-187">Firewall settings for applications not on this list are determined by the user.</span></span> <span data-ttu-id="19e60-188">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="19e60-188">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="19e60-189">Antwort</span><span class="sxs-lookup"><span data-stu-id="19e60-189">Response</span></span>
<span data-ttu-id="19e60-190">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [MacOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="19e60-190">If successful, this method returns a `201 Created` response code and a [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="19e60-191">Beispiel</span><span class="sxs-lookup"><span data-stu-id="19e60-191">Example</span></span>
### <a name="request"></a><span data-ttu-id="19e60-192">Anforderung</span><span class="sxs-lookup"><span data-stu-id="19e60-192">Request</span></span>
<span data-ttu-id="19e60-193">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="19e60-193">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 711

{
  "@odata.type": "#microsoft.graph.macOSEndpointProtectionConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "gatekeeperAllowedAppSource": "macAppStore",
  "gatekeeperBlockOverride": true,
  "firewallEnabled": true,
  "firewallBlockAllIncoming": true,
  "firewallEnableStealthMode": true,
  "firewallApplications": [
    {
      "@odata.type": "microsoft.graph.macOSFirewallApplication",
      "bundleId": "Bundle Id value",
      "allowsIncomingConnections": true
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="19e60-194">Antwort</span><span class="sxs-lookup"><span data-stu-id="19e60-194">Response</span></span>
<span data-ttu-id="19e60-p113">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="19e60-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 819

{
  "@odata.type": "#microsoft.graph.macOSEndpointProtectionConfiguration",
  "id": "7bf7f3ca-f3ca-7bf7-caf3-f77bcaf3f77b",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "gatekeeperAllowedAppSource": "macAppStore",
  "gatekeeperBlockOverride": true,
  "firewallEnabled": true,
  "firewallBlockAllIncoming": true,
  "firewallEnableStealthMode": true,
  "firewallApplications": [
    {
      "@odata.type": "microsoft.graph.macOSFirewallApplication",
      "bundleId": "Bundle Id value",
      "allowsIncomingConnections": true
    }
  ]
}
```





