---
title: AndroidForWorkEnterpriseWiFiConfiguration aktualisieren
description: Aktualisieren Sie die Eigenschaften eines AndroidForWorkEnterpriseWiFiConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: af6dee5a2459788a78ad2111123531f0b477213f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27828371"
---
# <a name="update-androidforworkenterprisewificonfiguration"></a><span data-ttu-id="f2cff-103">AndroidForWorkEnterpriseWiFiConfiguration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="f2cff-103">Update androidForWorkEnterpriseWiFiConfiguration</span></span>

> <span data-ttu-id="f2cff-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f2cff-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f2cff-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f2cff-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f2cff-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="f2cff-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f2cff-107">Aktualisieren Sie die Eigenschaften eines [AndroidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="f2cff-107">Update the properties of a [androidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f2cff-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f2cff-108">Prerequisites</span></span>
<span data-ttu-id="f2cff-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f2cff-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f2cff-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f2cff-111">Permission type</span></span>|<span data-ttu-id="f2cff-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f2cff-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f2cff-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f2cff-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f2cff-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2cff-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f2cff-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f2cff-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f2cff-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f2cff-116">Not supported.</span></span>|
|<span data-ttu-id="f2cff-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f2cff-117">Application</span></span>|<span data-ttu-id="f2cff-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f2cff-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f2cff-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f2cff-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="f2cff-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f2cff-120">Request headers</span></span>
|<span data-ttu-id="f2cff-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="f2cff-121">Header</span></span>|<span data-ttu-id="f2cff-122">Wert</span><span class="sxs-lookup"><span data-stu-id="f2cff-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f2cff-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f2cff-123">Authorization</span></span>|<span data-ttu-id="f2cff-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="f2cff-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f2cff-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="f2cff-125">Accept</span></span>|<span data-ttu-id="f2cff-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f2cff-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f2cff-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f2cff-127">Request body</span></span>
<span data-ttu-id="f2cff-128">Geben Sie im Textkörper Anforderung für das Objekt [AndroidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="f2cff-128">In the request body, supply a JSON representation for the [androidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md) object.</span></span>

<span data-ttu-id="f2cff-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [AndroidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="f2cff-129">The following table shows the properties that are required when you create the [androidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md).</span></span>

|<span data-ttu-id="f2cff-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f2cff-130">Property</span></span>|<span data-ttu-id="f2cff-131">Typ</span><span class="sxs-lookup"><span data-stu-id="f2cff-131">Type</span></span>|<span data-ttu-id="f2cff-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f2cff-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f2cff-133">id</span><span class="sxs-lookup"><span data-stu-id="f2cff-133">id</span></span>|<span data-ttu-id="f2cff-134">String</span><span class="sxs-lookup"><span data-stu-id="f2cff-134">String</span></span>|<span data-ttu-id="f2cff-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="f2cff-135">Key of the entity.</span></span> <span data-ttu-id="f2cff-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f2cff-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f2cff-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f2cff-137">lastModifiedDateTime</span></span>|<span data-ttu-id="f2cff-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f2cff-138">DateTimeOffset</span></span>|<span data-ttu-id="f2cff-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="f2cff-139">DateTime the object was last modified.</span></span> <span data-ttu-id="f2cff-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f2cff-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f2cff-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f2cff-141">roleScopeTagIds</span></span>|<span data-ttu-id="f2cff-142">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="f2cff-142">String collection</span></span>|<span data-ttu-id="f2cff-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="f2cff-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f2cff-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f2cff-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f2cff-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="f2cff-145">supportsScopeTags</span></span>|<span data-ttu-id="f2cff-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="f2cff-146">Boolean</span></span>|<span data-ttu-id="f2cff-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f2cff-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f2cff-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="f2cff-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f2cff-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="f2cff-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f2cff-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="f2cff-150">This property is read-only.</span></span> <span data-ttu-id="f2cff-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f2cff-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f2cff-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f2cff-152">createdDateTime</span></span>|<span data-ttu-id="f2cff-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f2cff-153">DateTimeOffset</span></span>|<span data-ttu-id="f2cff-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="f2cff-154">DateTime the object was created.</span></span> <span data-ttu-id="f2cff-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f2cff-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f2cff-156">description</span><span class="sxs-lookup"><span data-stu-id="f2cff-156">description</span></span>|<span data-ttu-id="f2cff-157">String</span><span class="sxs-lookup"><span data-stu-id="f2cff-157">String</span></span>|<span data-ttu-id="f2cff-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="f2cff-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f2cff-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f2cff-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f2cff-160">displayName</span><span class="sxs-lookup"><span data-stu-id="f2cff-160">displayName</span></span>|<span data-ttu-id="f2cff-161">String</span><span class="sxs-lookup"><span data-stu-id="f2cff-161">String</span></span>|<span data-ttu-id="f2cff-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="f2cff-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f2cff-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f2cff-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f2cff-164">Version</span><span class="sxs-lookup"><span data-stu-id="f2cff-164">version</span></span>|<span data-ttu-id="f2cff-165">Int32</span><span class="sxs-lookup"><span data-stu-id="f2cff-165">Int32</span></span>|<span data-ttu-id="f2cff-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="f2cff-166">Version of the device configuration.</span></span> <span data-ttu-id="f2cff-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f2cff-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f2cff-168">Netzwerkname</span><span class="sxs-lookup"><span data-stu-id="f2cff-168">networkName</span></span>|<span data-ttu-id="f2cff-169">String</span><span class="sxs-lookup"><span data-stu-id="f2cff-169">String</span></span>|<span data-ttu-id="f2cff-170">Netzwerk Namen von [AndroidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md) geerbt.</span><span class="sxs-lookup"><span data-stu-id="f2cff-170">Network Name Inherited from [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)</span></span>|
|<span data-ttu-id="f2cff-171">SSID</span><span class="sxs-lookup"><span data-stu-id="f2cff-171">ssid</span></span>|<span data-ttu-id="f2cff-172">String</span><span class="sxs-lookup"><span data-stu-id="f2cff-172">String</span></span>|<span data-ttu-id="f2cff-173">Dies ist der Name des Netzwerks Wi-Fi, die an alle Geräte gesendet wird.</span><span class="sxs-lookup"><span data-stu-id="f2cff-173">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span> <span data-ttu-id="f2cff-174">Geerbt von [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f2cff-174">Inherited from [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)</span></span>|
|<span data-ttu-id="f2cff-175">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="f2cff-175">connectAutomatically</span></span>|<span data-ttu-id="f2cff-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="f2cff-176">Boolean</span></span>|<span data-ttu-id="f2cff-177">Verbinden Sie automatisch, wenn dieses Netzwerk im Bereich befindet.</span><span class="sxs-lookup"><span data-stu-id="f2cff-177">Connect automatically when this network is in range.</span></span> <span data-ttu-id="f2cff-178">Eine Einstellung auf "true" überspringt die Aufforderung der Benutzer und automatisch mit Wi-Fi-Netzwerk verbinden.</span><span class="sxs-lookup"><span data-stu-id="f2cff-178">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span> <span data-ttu-id="f2cff-179">Geerbt von [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f2cff-179">Inherited from [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)</span></span>|
|<span data-ttu-id="f2cff-180">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="f2cff-180">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="f2cff-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="f2cff-181">Boolean</span></span>|<span data-ttu-id="f2cff-182">Bei Festlegung auf true festgelegt ist, dieses Profil erzwingt, dass das Gerät für die Verbindung mit einem Netzwerk SSID nicht, die an alle Geräte seine.</span><span class="sxs-lookup"><span data-stu-id="f2cff-182">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span> <span data-ttu-id="f2cff-183">Geerbt von [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f2cff-183">Inherited from [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)</span></span>|
|<span data-ttu-id="f2cff-184">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="f2cff-184">wiFiSecurityType</span></span>|[<span data-ttu-id="f2cff-185">androidWiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="f2cff-185">androidWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androidwifisecuritytype.md)|<span data-ttu-id="f2cff-186">Gibt an, ob Wi-Fi-Endpunkt einen EAP-basierte Sicherheitstyp verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="f2cff-186">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="f2cff-187">Geerbt von [AndroidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f2cff-187">Inherited from [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md).</span></span> <span data-ttu-id="f2cff-188">Mögliche Werte sind: `open` und `wpaEnterprise`.</span><span class="sxs-lookup"><span data-stu-id="f2cff-188">Possible values are: `open`, `wpaEnterprise`.</span></span>|
|<span data-ttu-id="f2cff-189">eapType</span><span class="sxs-lookup"><span data-stu-id="f2cff-189">eapType</span></span>|[<span data-ttu-id="f2cff-190">androidEapType</span><span class="sxs-lookup"><span data-stu-id="f2cff-190">androidEapType</span></span>](../resources/intune-deviceconfig-androideaptype.md)|<span data-ttu-id="f2cff-191">Gibt den Typ des EAP-Protokolls festlegen für den die Wi-Fi-Endpunkt (Router).</span><span class="sxs-lookup"><span data-stu-id="f2cff-191">Indicates the type of EAP protocol set on the the Wi-Fi endpoint (router).</span></span> <span data-ttu-id="f2cff-192">Mögliche Werte sind: `eapTls`, `eapTtls` und `peap`.</span><span class="sxs-lookup"><span data-stu-id="f2cff-192">Possible values are: `eapTls`, `eapTtls`, `peap`.</span></span>|
|<span data-ttu-id="f2cff-193">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="f2cff-193">authenticationMethod</span></span>|[<span data-ttu-id="f2cff-194">wiFiAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="f2cff-194">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="f2cff-195">Gibt die Authentifizierungsmethode muss der Client (Gerät) verwenden, wenn Sie den EAP-Typ PEAP oder EAP-TTLS konfiguriert ist.</span><span class="sxs-lookup"><span data-stu-id="f2cff-195">Indicates the Authentication Method the client (device) needs to use when the EAP Type is configured to PEAP or EAP-TTLS.</span></span> <span data-ttu-id="f2cff-196">Mögliche Werte sind: `certificate` und `usernameAndPassword`.</span><span class="sxs-lookup"><span data-stu-id="f2cff-196">Possible values are: `certificate`, `usernameAndPassword`.</span></span>|
|<span data-ttu-id="f2cff-197">innerAuthenticationProtocolForEapTtls</span><span class="sxs-lookup"><span data-stu-id="f2cff-197">innerAuthenticationProtocolForEapTtls</span></span>|[<span data-ttu-id="f2cff-198">nonEapAuthenticationMethodForEapTtlsType</span><span class="sxs-lookup"><span data-stu-id="f2cff-198">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="f2cff-199">Nicht-EAP-Methode für die Authentifizierung (innere) beim Identität EAP-Typ EAP-TTLS ist und AuthenticationMethod-ist Benutzername und Kennwort.</span><span class="sxs-lookup"><span data-stu-id="f2cff-199">Non-EAP Method for Authentication (Inner Identity) when EAP Type is EAP-TTLS and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="f2cff-200">Mögliche Werte: sind `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap` und `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="f2cff-200">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="f2cff-201">innerAuthenticationProtocolForPeap</span><span class="sxs-lookup"><span data-stu-id="f2cff-201">innerAuthenticationProtocolForPeap</span></span>|[<span data-ttu-id="f2cff-202">nonEapAuthenticationMethodForPeap</span><span class="sxs-lookup"><span data-stu-id="f2cff-202">nonEapAuthenticationMethodForPeap</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforpeap.md)|<span data-ttu-id="f2cff-203">Nicht-EAP-Methode für die Authentifizierung (innere) beim Identität EAP-Typ PEAP ist und AuthenticationMethod-ist Benutzername und Kennwort.</span><span class="sxs-lookup"><span data-stu-id="f2cff-203">Non-EAP Method for Authentication (Inner Identity) when EAP Type is PEAP and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="f2cff-204">Mögliche Werte sind: `none` und `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="f2cff-204">Possible values are: `none`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="f2cff-205">outerIdentityPrivacyTemporaryValue</span><span class="sxs-lookup"><span data-stu-id="f2cff-205">outerIdentityPrivacyTemporaryValue</span></span>|<span data-ttu-id="f2cff-206">String</span><span class="sxs-lookup"><span data-stu-id="f2cff-206">String</span></span>|<span data-ttu-id="f2cff-207">Aktivieren Sie Identität Privacy (externe Identität), wenn EAP-Typ EAP-TTLS oder PEAP konfiguriert ist.</span><span class="sxs-lookup"><span data-stu-id="f2cff-207">Enable identity privacy (Outer Identity) when EAP Type is configured to EAP-TTLS or PEAP.</span></span> <span data-ttu-id="f2cff-208">Die hier angegebene Zeichenfolge wird verwendet, um den Benutzernamen des einzelne Benutzer aktivieren, wenn sie versuchen, mit Wi-Fi-Netzwerk zu verbinden.</span><span class="sxs-lookup"><span data-stu-id="f2cff-208">The String provided here is used to mask the username of individual users when they attempt to connect to Wi-Fi network.</span></span>|



## <a name="response"></a><span data-ttu-id="f2cff-209">Antwort</span><span class="sxs-lookup"><span data-stu-id="f2cff-209">Response</span></span>
<span data-ttu-id="f2cff-210">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [AndroidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="f2cff-210">If successful, this method returns a `200 OK` response code and an updated [androidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f2cff-211">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f2cff-211">Example</span></span>
### <a name="request"></a><span data-ttu-id="f2cff-212">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f2cff-212">Request</span></span>
<span data-ttu-id="f2cff-213">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f2cff-213">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 756

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "networkName": "Network Name value",
  "ssid": "Ssid value",
  "connectAutomatically": true,
  "connectWhenNetworkNameIsHidden": true,
  "wiFiSecurityType": "wpaEnterprise",
  "eapType": "eapTtls",
  "authenticationMethod": "usernameAndPassword",
  "innerAuthenticationProtocolForEapTtls": "challengeHandshakeAuthenticationProtocol",
  "innerAuthenticationProtocolForPeap": "microsoftChapVersionTwo",
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value"
}
```

### <a name="response"></a><span data-ttu-id="f2cff-214">Antwort</span><span class="sxs-lookup"><span data-stu-id="f2cff-214">Response</span></span>
<span data-ttu-id="f2cff-p120">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f2cff-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 944

{
  "@odata.type": "#microsoft.graph.androidForWorkEnterpriseWiFiConfiguration",
  "id": "742d953a-953a-742d-3a95-2d743a952d74",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "networkName": "Network Name value",
  "ssid": "Ssid value",
  "connectAutomatically": true,
  "connectWhenNetworkNameIsHidden": true,
  "wiFiSecurityType": "wpaEnterprise",
  "eapType": "eapTtls",
  "authenticationMethod": "usernameAndPassword",
  "innerAuthenticationProtocolForEapTtls": "challengeHandshakeAuthenticationProtocol",
  "innerAuthenticationProtocolForPeap": "microsoftChapVersionTwo",
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value"
}
```





