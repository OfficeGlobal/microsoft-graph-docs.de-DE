---
title: MacOSEndpointProtectionConfiguration erstellen
description: Erstellen eines neuen macOSEndpointProtectionConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c0ced93721538f745a05165175090397128e796a
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30171589"
---
# <a name="create-macosendpointprotectionconfiguration"></a><span data-ttu-id="6a407-103">MacOSEndpointProtectionConfiguration erstellen</span><span class="sxs-lookup"><span data-stu-id="6a407-103">Create macOSEndpointProtectionConfiguration</span></span>

> <span data-ttu-id="6a407-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6a407-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6a407-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="6a407-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6a407-106">Erstellen eines neuen [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="6a407-106">Create a new [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6a407-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="6a407-107">Prerequisites</span></span>
<span data-ttu-id="6a407-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="6a407-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="6a407-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6a407-110">Permission type</span></span>|<span data-ttu-id="6a407-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6a407-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6a407-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6a407-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6a407-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a407-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6a407-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6a407-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6a407-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6a407-115">Not supported.</span></span>|
|<span data-ttu-id="6a407-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6a407-116">Application</span></span>|<span data-ttu-id="6a407-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6a407-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6a407-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6a407-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="6a407-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6a407-119">Request headers</span></span>
|<span data-ttu-id="6a407-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="6a407-120">Header</span></span>|<span data-ttu-id="6a407-121">Wert</span><span class="sxs-lookup"><span data-stu-id="6a407-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6a407-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6a407-122">Authorization</span></span>|<span data-ttu-id="6a407-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="6a407-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6a407-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="6a407-124">Accept</span></span>|<span data-ttu-id="6a407-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6a407-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6a407-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6a407-126">Request body</span></span>
<span data-ttu-id="6a407-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das macOSEndpointProtectionConfiguration-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="6a407-127">In the request body, supply a JSON representation for the macOSEndpointProtectionConfiguration object.</span></span>

<span data-ttu-id="6a407-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der macOSEndpointProtectionConfiguration erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="6a407-128">The following table shows the properties that are required when you create the macOSEndpointProtectionConfiguration.</span></span>

|<span data-ttu-id="6a407-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6a407-129">Property</span></span>|<span data-ttu-id="6a407-130">Typ</span><span class="sxs-lookup"><span data-stu-id="6a407-130">Type</span></span>|<span data-ttu-id="6a407-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6a407-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6a407-132">id</span><span class="sxs-lookup"><span data-stu-id="6a407-132">id</span></span>|<span data-ttu-id="6a407-133">string</span><span class="sxs-lookup"><span data-stu-id="6a407-133">String</span></span>|<span data-ttu-id="6a407-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="6a407-134">Key of the entity.</span></span> <span data-ttu-id="6a407-135">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6a407-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6a407-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6a407-136">lastModifiedDateTime</span></span>|<span data-ttu-id="6a407-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6a407-137">DateTimeOffset</span></span>|<span data-ttu-id="6a407-138">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="6a407-138">DateTime the object was last modified.</span></span> <span data-ttu-id="6a407-139">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6a407-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6a407-140">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="6a407-140">roleScopeTagIds</span></span>|<span data-ttu-id="6a407-141">String collection</span><span class="sxs-lookup"><span data-stu-id="6a407-141">String collection</span></span>|<span data-ttu-id="6a407-142">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="6a407-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="6a407-143">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6a407-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6a407-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="6a407-144">supportsScopeTags</span></span>|<span data-ttu-id="6a407-145">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="6a407-145">Boolean</span></span>|<span data-ttu-id="6a407-146">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereichs Tags unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6a407-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="6a407-147">Das Zuweisen zur ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert auf false festgelegt ist und Entitäten für bereichsbezogene Benutzer nicht sichtbar sind.</span><span class="sxs-lookup"><span data-stu-id="6a407-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="6a407-148">Dies geschieht für in Silverlight erstellte Legacy Richtlinien und kann durch Löschen und erneutes Erstellen der Richtlinie im Azure-Portal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="6a407-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="6a407-149">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="6a407-149">This property is read-only.</span></span> <span data-ttu-id="6a407-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6a407-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6a407-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6a407-151">createdDateTime</span></span>|<span data-ttu-id="6a407-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6a407-152">DateTimeOffset</span></span>|<span data-ttu-id="6a407-153">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="6a407-153">DateTime the object was created.</span></span> <span data-ttu-id="6a407-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6a407-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6a407-155">description</span><span class="sxs-lookup"><span data-stu-id="6a407-155">description</span></span>|<span data-ttu-id="6a407-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6a407-156">String</span></span>|<span data-ttu-id="6a407-157">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="6a407-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6a407-158">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6a407-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6a407-159">displayName</span><span class="sxs-lookup"><span data-stu-id="6a407-159">displayName</span></span>|<span data-ttu-id="6a407-160">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6a407-160">String</span></span>|<span data-ttu-id="6a407-161">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="6a407-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6a407-162">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6a407-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6a407-163">Version</span><span class="sxs-lookup"><span data-stu-id="6a407-163">version</span></span>|<span data-ttu-id="6a407-164">Int32</span><span class="sxs-lookup"><span data-stu-id="6a407-164">Int32</span></span>|<span data-ttu-id="6a407-165">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="6a407-165">Version of the device configuration.</span></span> <span data-ttu-id="6a407-166">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6a407-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6a407-167">gatekeeperAllowedAppSource</span><span class="sxs-lookup"><span data-stu-id="6a407-167">gatekeeperAllowedAppSource</span></span>|[<span data-ttu-id="6a407-168">macOSGatekeeperAppSources</span><span class="sxs-lookup"><span data-stu-id="6a407-168">macOSGatekeeperAppSources</span></span>](../resources/intune-deviceconfig-macosgatekeeperappsources.md)|<span data-ttu-id="6a407-169">System-und Datenschutzeinstellung, die bestimmt, welche Downloadspeicherorte apps auf einem macOS-Gerät ausgeführt werden können.</span><span class="sxs-lookup"><span data-stu-id="6a407-169">System and Privacy setting that determines which download locations apps can be run from on a macOS device.</span></span> <span data-ttu-id="6a407-170">Mögliche Werte: `notConfigured`, `macAppStore`, `macAppStoreAndIdentifiedDevelopers`, `anywhere`.</span><span class="sxs-lookup"><span data-stu-id="6a407-170">Possible values are: `notConfigured`, `macAppStore`, `macAppStoreAndIdentifiedDevelopers`, `anywhere`.</span></span>|
|<span data-ttu-id="6a407-171">gatekeeperBlockOverride</span><span class="sxs-lookup"><span data-stu-id="6a407-171">gatekeeperBlockOverride</span></span>|<span data-ttu-id="6a407-172">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="6a407-172">Boolean</span></span>|<span data-ttu-id="6a407-173">Bei Festlegung auf "true" wird die Benutzer Außerkraftsetzung für Gatekeeper deaktiviert.</span><span class="sxs-lookup"><span data-stu-id="6a407-173">If set to true, the user override for Gatekeeper will be disabled.</span></span>|
|<span data-ttu-id="6a407-174">firewallEnabled</span><span class="sxs-lookup"><span data-stu-id="6a407-174">firewallEnabled</span></span>|<span data-ttu-id="6a407-175">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="6a407-175">Boolean</span></span>|<span data-ttu-id="6a407-176">Ob die Firewall aktiviert werden soll oder nicht.</span><span class="sxs-lookup"><span data-stu-id="6a407-176">Whether the firewall should be enabled or not.</span></span>|
|<span data-ttu-id="6a407-177">firewallBlockAllIncoming</span><span class="sxs-lookup"><span data-stu-id="6a407-177">firewallBlockAllIncoming</span></span>|<span data-ttu-id="6a407-178">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="6a407-178">Boolean</span></span>|<span data-ttu-id="6a407-179">Entspricht der Option "alle eingehenden Verbindungen blockieren".</span><span class="sxs-lookup"><span data-stu-id="6a407-179">Corresponds to the “Block all incoming connections” option.</span></span>|
|<span data-ttu-id="6a407-180">firewallEnableStealthMode</span><span class="sxs-lookup"><span data-stu-id="6a407-180">firewallEnableStealthMode</span></span>|<span data-ttu-id="6a407-181">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="6a407-181">Boolean</span></span>|<span data-ttu-id="6a407-182">Entspricht "Stealth-Modus aktivieren".</span><span class="sxs-lookup"><span data-stu-id="6a407-182">Corresponds to “Enable stealth mode.”</span></span>|
|<span data-ttu-id="6a407-183">firewallApplications</span><span class="sxs-lookup"><span data-stu-id="6a407-183">firewallApplications</span></span>|<span data-ttu-id="6a407-184">[macOSFirewallApplication](../resources/intune-deviceconfig-macosfirewallapplication.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="6a407-184">[macOSFirewallApplication](../resources/intune-deviceconfig-macosfirewallapplication.md) collection</span></span>|<span data-ttu-id="6a407-185">Liste der Anwendungen mit Firewalleinstellungen.</span><span class="sxs-lookup"><span data-stu-id="6a407-185">List of applications with firewall settings.</span></span> <span data-ttu-id="6a407-186">Firewalleinstellungen für Anwendungen, die nicht in dieser Liste aufgeführt sind, werden vom Benutzer festgelegt.</span><span class="sxs-lookup"><span data-stu-id="6a407-186">Firewall settings for applications not on this list are determined by the user.</span></span> <span data-ttu-id="6a407-187">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="6a407-187">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="6a407-188">Antwort</span><span class="sxs-lookup"><span data-stu-id="6a407-188">Response</span></span>
<span data-ttu-id="6a407-189">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="6a407-189">If successful, this method returns a `201 Created` response code and a [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6a407-190">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6a407-190">Example</span></span>

### <a name="request"></a><span data-ttu-id="6a407-191">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6a407-191">Request</span></span>
<span data-ttu-id="6a407-192">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6a407-192">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 647

{
  "@odata.type": "#microsoft.graph.macOSEndpointProtectionConfiguration",
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

### <a name="response"></a><span data-ttu-id="6a407-193">Antwort</span><span class="sxs-lookup"><span data-stu-id="6a407-193">Response</span></span>
<span data-ttu-id="6a407-p112">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6a407-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




