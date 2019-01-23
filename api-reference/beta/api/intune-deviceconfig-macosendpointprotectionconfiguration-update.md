---
title: MacOSEndpointProtectionConfiguration aktualisieren
description: Aktualisieren Sie die Eigenschaften eines MacOSEndpointProtectionConfiguration-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f1659141c75ec003b4cfe2cd47279e02917e59dc
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29407641"
---
# <a name="update-macosendpointprotectionconfiguration"></a><span data-ttu-id="65c51-103">MacOSEndpointProtectionConfiguration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="65c51-103">Update macOSEndpointProtectionConfiguration</span></span>

> <span data-ttu-id="65c51-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="65c51-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="65c51-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="65c51-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="65c51-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="65c51-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="65c51-107">Aktualisieren Sie die Eigenschaften eines [MacOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="65c51-107">Update the properties of a [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="65c51-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="65c51-108">Prerequisites</span></span>
<span data-ttu-id="65c51-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="65c51-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="65c51-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="65c51-111">Permission type</span></span>|<span data-ttu-id="65c51-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="65c51-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="65c51-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="65c51-113">Delegated (work or school account)</span></span>|<span data-ttu-id="65c51-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="65c51-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="65c51-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="65c51-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="65c51-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="65c51-116">Not supported.</span></span>|
|<span data-ttu-id="65c51-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="65c51-117">Application</span></span>|<span data-ttu-id="65c51-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="65c51-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="65c51-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="65c51-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="65c51-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="65c51-120">Request headers</span></span>
|<span data-ttu-id="65c51-121">Header</span><span class="sxs-lookup"><span data-stu-id="65c51-121">Header</span></span>|<span data-ttu-id="65c51-122">Wert</span><span class="sxs-lookup"><span data-stu-id="65c51-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="65c51-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="65c51-123">Authorization</span></span>|<span data-ttu-id="65c51-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="65c51-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="65c51-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="65c51-125">Accept</span></span>|<span data-ttu-id="65c51-126">application/json</span><span class="sxs-lookup"><span data-stu-id="65c51-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="65c51-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="65c51-127">Request body</span></span>
<span data-ttu-id="65c51-128">Geben Sie im Textkörper Anforderung für das Objekt [MacOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="65c51-128">In the request body, supply a JSON representation for the [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) object.</span></span>

<span data-ttu-id="65c51-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [MacOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="65c51-129">The following table shows the properties that are required when you create the [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md).</span></span>

|<span data-ttu-id="65c51-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="65c51-130">Property</span></span>|<span data-ttu-id="65c51-131">Typ</span><span class="sxs-lookup"><span data-stu-id="65c51-131">Type</span></span>|<span data-ttu-id="65c51-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="65c51-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65c51-133">id</span><span class="sxs-lookup"><span data-stu-id="65c51-133">id</span></span>|<span data-ttu-id="65c51-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="65c51-134">String</span></span>|<span data-ttu-id="65c51-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="65c51-135">Key of the entity.</span></span> <span data-ttu-id="65c51-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="65c51-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="65c51-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="65c51-137">lastModifiedDateTime</span></span>|<span data-ttu-id="65c51-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="65c51-138">DateTimeOffset</span></span>|<span data-ttu-id="65c51-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="65c51-139">DateTime the object was last modified.</span></span> <span data-ttu-id="65c51-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="65c51-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="65c51-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="65c51-141">roleScopeTagIds</span></span>|<span data-ttu-id="65c51-142">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="65c51-142">String collection</span></span>|<span data-ttu-id="65c51-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="65c51-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="65c51-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="65c51-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="65c51-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="65c51-145">supportsScopeTags</span></span>|<span data-ttu-id="65c51-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="65c51-146">Boolean</span></span>|<span data-ttu-id="65c51-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="65c51-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="65c51-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="65c51-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="65c51-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="65c51-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="65c51-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="65c51-150">This property is read-only.</span></span> <span data-ttu-id="65c51-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="65c51-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="65c51-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="65c51-152">createdDateTime</span></span>|<span data-ttu-id="65c51-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="65c51-153">DateTimeOffset</span></span>|<span data-ttu-id="65c51-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="65c51-154">DateTime the object was created.</span></span> <span data-ttu-id="65c51-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="65c51-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="65c51-156">description</span><span class="sxs-lookup"><span data-stu-id="65c51-156">description</span></span>|<span data-ttu-id="65c51-157">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="65c51-157">String</span></span>|<span data-ttu-id="65c51-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="65c51-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="65c51-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="65c51-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="65c51-160">displayName</span><span class="sxs-lookup"><span data-stu-id="65c51-160">displayName</span></span>|<span data-ttu-id="65c51-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="65c51-161">String</span></span>|<span data-ttu-id="65c51-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="65c51-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="65c51-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="65c51-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="65c51-164">Version</span><span class="sxs-lookup"><span data-stu-id="65c51-164">version</span></span>|<span data-ttu-id="65c51-165">Int32</span><span class="sxs-lookup"><span data-stu-id="65c51-165">Int32</span></span>|<span data-ttu-id="65c51-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="65c51-166">Version of the device configuration.</span></span> <span data-ttu-id="65c51-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="65c51-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="65c51-168">gatekeeperAllowedAppSource</span><span class="sxs-lookup"><span data-stu-id="65c51-168">gatekeeperAllowedAppSource</span></span>|[<span data-ttu-id="65c51-169">macOSGatekeeperAppSources</span><span class="sxs-lookup"><span data-stu-id="65c51-169">macOSGatekeeperAppSources</span></span>](../resources/intune-deviceconfig-macosgatekeeperappsources.md)|<span data-ttu-id="65c51-170">System und den Datenschutz, der bestimmt, welche Download Speicherorte apps auf einem Mac OS-Gerät aus ausgeführt werden können.</span><span class="sxs-lookup"><span data-stu-id="65c51-170">System and Privacy setting that determines which download locations apps can be run from on a macOS device.</span></span> <span data-ttu-id="65c51-171">Mögliche Werte: sind `notConfigured`, `macAppStore`, `macAppStoreAndIdentifiedDevelopers` und `anywhere`.</span><span class="sxs-lookup"><span data-stu-id="65c51-171">Possible values are: `notConfigured`, `macAppStore`, `macAppStoreAndIdentifiedDevelopers`, `anywhere`.</span></span>|
|<span data-ttu-id="65c51-172">gatekeeperBlockOverride</span><span class="sxs-lookup"><span data-stu-id="65c51-172">gatekeeperBlockOverride</span></span>|<span data-ttu-id="65c51-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="65c51-173">Boolean</span></span>|<span data-ttu-id="65c51-174">Wenn auf True festgelegt, der Benutzer außer Kraft setzen für Gatekeeper deaktiviert wird.</span><span class="sxs-lookup"><span data-stu-id="65c51-174">If set to true, the user override for Gatekeeper will be disabled.</span></span>|
|<span data-ttu-id="65c51-175">firewallEnabled</span><span class="sxs-lookup"><span data-stu-id="65c51-175">firewallEnabled</span></span>|<span data-ttu-id="65c51-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="65c51-176">Boolean</span></span>|<span data-ttu-id="65c51-177">Gibt an, ob die Firewall oder nicht aktiviert werden soll.</span><span class="sxs-lookup"><span data-stu-id="65c51-177">Whether the firewall should be enabled or not.</span></span>|
|<span data-ttu-id="65c51-178">firewallBlockAllIncoming</span><span class="sxs-lookup"><span data-stu-id="65c51-178">firewallBlockAllIncoming</span></span>|<span data-ttu-id="65c51-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="65c51-179">Boolean</span></span>|<span data-ttu-id="65c51-180">Entspricht der Option "Alle eingehende Verbindungen blockieren".</span><span class="sxs-lookup"><span data-stu-id="65c51-180">Corresponds to the “Block all incoming connections” option.</span></span>|
|<span data-ttu-id="65c51-181">firewallEnableStealthMode</span><span class="sxs-lookup"><span data-stu-id="65c51-181">firewallEnableStealthMode</span></span>|<span data-ttu-id="65c51-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="65c51-182">Boolean</span></span>|<span data-ttu-id="65c51-183">Entspricht "Enable Tarnmodus."</span><span class="sxs-lookup"><span data-stu-id="65c51-183">Corresponds to “Enable stealth mode.”</span></span>|
|<span data-ttu-id="65c51-184">firewallApplications</span><span class="sxs-lookup"><span data-stu-id="65c51-184">firewallApplications</span></span>|<span data-ttu-id="65c51-185">[MacOSFirewallApplication](../resources/intune-deviceconfig-macosfirewallapplication.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="65c51-185">[macOSFirewallApplication](../resources/intune-deviceconfig-macosfirewallapplication.md) collection</span></span>|<span data-ttu-id="65c51-186">Liste von Anwendungen mit Firewalleinstellungen.</span><span class="sxs-lookup"><span data-stu-id="65c51-186">List of applications with firewall settings.</span></span> <span data-ttu-id="65c51-187">Firewalleinstellungen für Applikationen nicht in dieser Liste werden vom Benutzer festgelegt.</span><span class="sxs-lookup"><span data-stu-id="65c51-187">Firewall settings for applications not on this list are determined by the user.</span></span> <span data-ttu-id="65c51-188">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="65c51-188">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="65c51-189">Antwort</span><span class="sxs-lookup"><span data-stu-id="65c51-189">Response</span></span>
<span data-ttu-id="65c51-190">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [MacOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="65c51-190">If successful, this method returns a `200 OK` response code and an updated [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="65c51-191">Beispiel</span><span class="sxs-lookup"><span data-stu-id="65c51-191">Example</span></span>

### <a name="request"></a><span data-ttu-id="65c51-192">Anforderung</span><span class="sxs-lookup"><span data-stu-id="65c51-192">Request</span></span>
<span data-ttu-id="65c51-193">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="65c51-193">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="65c51-194">Antwort</span><span class="sxs-lookup"><span data-stu-id="65c51-194">Response</span></span>
<span data-ttu-id="65c51-p113">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="65c51-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




