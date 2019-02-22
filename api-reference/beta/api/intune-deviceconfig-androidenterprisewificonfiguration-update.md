---
title: AndroidEnterpriseWiFiConfiguration aktualisieren
description: Aktualisieren der Eigenschaften eines androidEnterpriseWiFiConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5dbbee8aef2db80b5d49e1bb7cd801e97bf08923
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30153543"
---
# <a name="update-androidenterprisewificonfiguration"></a><span data-ttu-id="b857f-103">AndroidEnterpriseWiFiConfiguration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="b857f-103">Update androidEnterpriseWiFiConfiguration</span></span>

> <span data-ttu-id="b857f-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b857f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b857f-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="b857f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b857f-106">Aktualisieren der Eigenschaften eines [androidEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidenterprisewificonfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="b857f-106">Update the properties of a [androidEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidenterprisewificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b857f-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b857f-107">Prerequisites</span></span>
<span data-ttu-id="b857f-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="b857f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b857f-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b857f-110">Permission type</span></span>|<span data-ttu-id="b857f-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b857f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b857f-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b857f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b857f-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b857f-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b857f-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b857f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b857f-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b857f-115">Not supported.</span></span>|
|<span data-ttu-id="b857f-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b857f-116">Application</span></span>|<span data-ttu-id="b857f-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b857f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b857f-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b857f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="b857f-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b857f-119">Request headers</span></span>
|<span data-ttu-id="b857f-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="b857f-120">Header</span></span>|<span data-ttu-id="b857f-121">Wert</span><span class="sxs-lookup"><span data-stu-id="b857f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b857f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b857f-122">Authorization</span></span>|<span data-ttu-id="b857f-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b857f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b857f-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="b857f-124">Accept</span></span>|<span data-ttu-id="b857f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b857f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b857f-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b857f-126">Request body</span></span>
<span data-ttu-id="b857f-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [androidEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidenterprisewificonfiguration.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="b857f-127">In the request body, supply a JSON representation for the [androidEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidenterprisewificonfiguration.md) object.</span></span>

<span data-ttu-id="b857f-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [androidEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidenterprisewificonfiguration.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="b857f-128">The following table shows the properties that are required when you create the [androidEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidenterprisewificonfiguration.md).</span></span>

|<span data-ttu-id="b857f-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b857f-129">Property</span></span>|<span data-ttu-id="b857f-130">Typ</span><span class="sxs-lookup"><span data-stu-id="b857f-130">Type</span></span>|<span data-ttu-id="b857f-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b857f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b857f-132">id</span><span class="sxs-lookup"><span data-stu-id="b857f-132">id</span></span>|<span data-ttu-id="b857f-133">string</span><span class="sxs-lookup"><span data-stu-id="b857f-133">String</span></span>|<span data-ttu-id="b857f-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="b857f-134">Key of the entity.</span></span> <span data-ttu-id="b857f-135">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b857f-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b857f-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b857f-136">lastModifiedDateTime</span></span>|<span data-ttu-id="b857f-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b857f-137">DateTimeOffset</span></span>|<span data-ttu-id="b857f-138">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="b857f-138">DateTime the object was last modified.</span></span> <span data-ttu-id="b857f-139">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b857f-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b857f-140">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="b857f-140">roleScopeTagIds</span></span>|<span data-ttu-id="b857f-141">String collection</span><span class="sxs-lookup"><span data-stu-id="b857f-141">String collection</span></span>|<span data-ttu-id="b857f-142">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="b857f-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b857f-143">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b857f-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b857f-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="b857f-144">supportsScopeTags</span></span>|<span data-ttu-id="b857f-145">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b857f-145">Boolean</span></span>|<span data-ttu-id="b857f-146">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereichs Tags unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b857f-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="b857f-147">Das Zuweisen zur ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert auf false festgelegt ist und Entitäten für bereichsbezogene Benutzer nicht sichtbar sind.</span><span class="sxs-lookup"><span data-stu-id="b857f-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="b857f-148">Dies geschieht für in Silverlight erstellte Legacy Richtlinien und kann durch Löschen und erneutes Erstellen der Richtlinie im Azure-Portal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="b857f-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="b857f-149">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="b857f-149">This property is read-only.</span></span> <span data-ttu-id="b857f-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b857f-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b857f-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b857f-151">createdDateTime</span></span>|<span data-ttu-id="b857f-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b857f-152">DateTimeOffset</span></span>|<span data-ttu-id="b857f-153">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="b857f-153">DateTime the object was created.</span></span> <span data-ttu-id="b857f-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b857f-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b857f-155">description</span><span class="sxs-lookup"><span data-stu-id="b857f-155">description</span></span>|<span data-ttu-id="b857f-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b857f-156">String</span></span>|<span data-ttu-id="b857f-157">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="b857f-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b857f-158">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b857f-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b857f-159">displayName</span><span class="sxs-lookup"><span data-stu-id="b857f-159">displayName</span></span>|<span data-ttu-id="b857f-160">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b857f-160">String</span></span>|<span data-ttu-id="b857f-161">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="b857f-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b857f-162">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b857f-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b857f-163">Version</span><span class="sxs-lookup"><span data-stu-id="b857f-163">version</span></span>|<span data-ttu-id="b857f-164">Int32</span><span class="sxs-lookup"><span data-stu-id="b857f-164">Int32</span></span>|<span data-ttu-id="b857f-165">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="b857f-165">Version of the device configuration.</span></span> <span data-ttu-id="b857f-166">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b857f-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b857f-167">networkName</span><span class="sxs-lookup"><span data-stu-id="b857f-167">networkName</span></span>|<span data-ttu-id="b857f-168">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b857f-168">String</span></span>|<span data-ttu-id="b857f-169">Netzwerk Name geerbt von [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b857f-169">Network Name Inherited from [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md)</span></span>|
|<span data-ttu-id="b857f-170">SSID</span><span class="sxs-lookup"><span data-stu-id="b857f-170">ssid</span></span>|<span data-ttu-id="b857f-171">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b857f-171">String</span></span>|<span data-ttu-id="b857f-172">Dies ist der Name des WLAN-Netzwerks, das auf alle Geräte übertragen wird.</span><span class="sxs-lookup"><span data-stu-id="b857f-172">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span> <span data-ttu-id="b857f-173">Geerbt von [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b857f-173">Inherited from [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md)</span></span>|
|<span data-ttu-id="b857f-174">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="b857f-174">connectAutomatically</span></span>|<span data-ttu-id="b857f-175">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b857f-175">Boolean</span></span>|<span data-ttu-id="b857f-176">Verbinden Sie sich automatisch, wenn sich dieses Netzwerk in Reichweite befindet.</span><span class="sxs-lookup"><span data-stu-id="b857f-176">Connect automatically when this network is in range.</span></span> <span data-ttu-id="b857f-177">Wenn Sie diesen Wert auf true festlegen, wird die Benutzereingabe übersprungen, und das Gerät wird automatisch mit dem WLAN verbunden.</span><span class="sxs-lookup"><span data-stu-id="b857f-177">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span> <span data-ttu-id="b857f-178">Geerbt von [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b857f-178">Inherited from [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md)</span></span>|
|<span data-ttu-id="b857f-179">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="b857f-179">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="b857f-180">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b857f-180">Boolean</span></span>|<span data-ttu-id="b857f-181">Wenn dieser Wert auf "true" festgelegt ist, wird das Gerät gezwungen, eine Verbindung mit einem Netzwerk herzustellen, das seine SSID nicht auf alle Geräte übermittelt.</span><span class="sxs-lookup"><span data-stu-id="b857f-181">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span> <span data-ttu-id="b857f-182">Geerbt von [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b857f-182">Inherited from [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md)</span></span>|
|<span data-ttu-id="b857f-183">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="b857f-183">wiFiSecurityType</span></span>|[<span data-ttu-id="b857f-184">androidWiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="b857f-184">androidWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androidwifisecuritytype.md)|<span data-ttu-id="b857f-185">Gibt an, ob der WLAN-Endpunkt einen EAP-basierten Sicherheitstyp verwendet.</span><span class="sxs-lookup"><span data-stu-id="b857f-185">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="b857f-186">Von [AndroidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="b857f-186">Inherited from [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md).</span></span> <span data-ttu-id="b857f-187">Mögliche Werte sind: `open` und `wpaEnterprise`.</span><span class="sxs-lookup"><span data-stu-id="b857f-187">Possible values are: `open`, `wpaEnterprise`.</span></span>|
|<span data-ttu-id="b857f-188">eapType</span><span class="sxs-lookup"><span data-stu-id="b857f-188">eapType</span></span>|[<span data-ttu-id="b857f-189">androidEapType</span><span class="sxs-lookup"><span data-stu-id="b857f-189">androidEapType</span></span>](../resources/intune-deviceconfig-androideaptype.md)|<span data-ttu-id="b857f-190">Gibt den Typ des EAP-Protokolls an, das auf dem WLAN-Endpunkt (Router) festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="b857f-190">Indicates the type of EAP protocol set on the the Wi-Fi endpoint (router).</span></span> <span data-ttu-id="b857f-191">Mögliche Werte sind: `eapTls`, `eapTtls` und `peap`.</span><span class="sxs-lookup"><span data-stu-id="b857f-191">Possible values are: `eapTls`, `eapTtls`, `peap`.</span></span>|
|<span data-ttu-id="b857f-192">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="b857f-192">authenticationMethod</span></span>|[<span data-ttu-id="b857f-193">wiFiAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="b857f-193">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="b857f-194">Gibt die AuthentifizierungsMethode an, die der Client (Gerät) verwenden muss, wenn der EAP-Typ auf PEAP oder EAP-TTLS konfiguriert ist.</span><span class="sxs-lookup"><span data-stu-id="b857f-194">Indicates the Authentication Method the client (device) needs to use when the EAP Type is configured to PEAP or EAP-TTLS.</span></span> <span data-ttu-id="b857f-195">Mögliche Werte sind: `certificate` und `usernameAndPassword`.</span><span class="sxs-lookup"><span data-stu-id="b857f-195">Possible values are: `certificate`, `usernameAndPassword`.</span></span>|
|<span data-ttu-id="b857f-196">innerAuthenticationProtocolForEapTtls</span><span class="sxs-lookup"><span data-stu-id="b857f-196">innerAuthenticationProtocolForEapTtls</span></span>|[<span data-ttu-id="b857f-197">nonEapAuthenticationMethodForEapTtlsType</span><span class="sxs-lookup"><span data-stu-id="b857f-197">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="b857f-198">Nicht-EAP-Methode für die Authentifizierung (innere Identität) bei EAP-TTLS und AuthenticationMethod ist username und Password.</span><span class="sxs-lookup"><span data-stu-id="b857f-198">Non-EAP Method for Authentication (Inner Identity) when EAP Type is EAP-TTLS and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="b857f-199">Mögliche Werte: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="b857f-199">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="b857f-200">innerAuthenticationProtocolForPeap</span><span class="sxs-lookup"><span data-stu-id="b857f-200">innerAuthenticationProtocolForPeap</span></span>|[<span data-ttu-id="b857f-201">nonEapAuthenticationMethodForPeap</span><span class="sxs-lookup"><span data-stu-id="b857f-201">nonEapAuthenticationMethodForPeap</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforpeap.md)|<span data-ttu-id="b857f-202">Nicht-EAP-Methode für die Authentifizierung (innere Identität), wenn EAP-Typ PEAP und AuthenticationMethod der Benutzername und das Kennwort ist.</span><span class="sxs-lookup"><span data-stu-id="b857f-202">Non-EAP Method for Authentication (Inner Identity) when EAP Type is PEAP and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="b857f-203">Mögliche Werte sind: `none` und `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="b857f-203">Possible values are: `none`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="b857f-204">Outeridentityprivacytemporaryvalue wurden</span><span class="sxs-lookup"><span data-stu-id="b857f-204">outerIdentityPrivacyTemporaryValue</span></span>|<span data-ttu-id="b857f-205">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b857f-205">String</span></span>|<span data-ttu-id="b857f-206">Aktivieren Sie Identitätsdatenschutz (äußere Identität), wenn der EAP-Typ für EAP-TTLS oder PEAP konfiguriert ist.</span><span class="sxs-lookup"><span data-stu-id="b857f-206">Enable identity privacy (Outer Identity) when EAP Type is configured to EAP-TTLS or PEAP.</span></span> <span data-ttu-id="b857f-207">Die hier angegebene Zeichenfolge wird verwendet, um den Benutzernamen einzelner Benutzer zu maskieren, wenn Sie versuchen, eine Verbindung mit dem WLAN herzustellen.</span><span class="sxs-lookup"><span data-stu-id="b857f-207">The String provided here is used to mask the username of individual users when they attempt to connect to Wi-Fi network.</span></span>|



## <a name="response"></a><span data-ttu-id="b857f-208">Antwort</span><span class="sxs-lookup"><span data-stu-id="b857f-208">Response</span></span>
<span data-ttu-id="b857f-209">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [androidEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidenterprisewificonfiguration.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="b857f-209">If successful, this method returns a `200 OK` response code and an updated [androidEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidenterprisewificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b857f-210">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b857f-210">Example</span></span>

### <a name="request"></a><span data-ttu-id="b857f-211">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b857f-211">Request</span></span>
<span data-ttu-id="b857f-212">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b857f-212">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 765

{
  "@odata.type": "#microsoft.graph.androidEnterpriseWiFiConfiguration",
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

### <a name="response"></a><span data-ttu-id="b857f-213">Antwort</span><span class="sxs-lookup"><span data-stu-id="b857f-213">Response</span></span>
<span data-ttu-id="b857f-p119">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b857f-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 937

{
  "@odata.type": "#microsoft.graph.androidEnterpriseWiFiConfiguration",
  "id": "972edff4-dff4-972e-f4df-2e97f4df2e97",
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




