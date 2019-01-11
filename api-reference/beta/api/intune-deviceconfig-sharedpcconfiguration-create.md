---
title: Erstellen von „sharedPCConfiguration“
description: Diese Methode erstellt ein neues Objekt des Typs sharedPCConfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 454f70ba8a89bd502e541638a9ba8b3d24ae4f7a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27882054"
---
# <a name="create-sharedpcconfiguration"></a><span data-ttu-id="ed97b-103">Erstellen von „sharedPCConfiguration“</span><span class="sxs-lookup"><span data-stu-id="ed97b-103">Create sharedPCConfiguration</span></span>

> <span data-ttu-id="ed97b-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="ed97b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ed97b-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ed97b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ed97b-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="ed97b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ed97b-107">Diese Methode erstellt ein neues Objekt des Typs [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ed97b-107">Create a new [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ed97b-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="ed97b-108">Prerequisites</span></span>
<span data-ttu-id="ed97b-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ed97b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ed97b-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ed97b-111">Permission type</span></span>|<span data-ttu-id="ed97b-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ed97b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ed97b-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ed97b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ed97b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ed97b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ed97b-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ed97b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ed97b-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ed97b-116">Not supported.</span></span>|
|<span data-ttu-id="ed97b-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ed97b-117">Application</span></span>|<span data-ttu-id="ed97b-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ed97b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ed97b-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ed97b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="ed97b-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ed97b-120">Request headers</span></span>
|<span data-ttu-id="ed97b-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="ed97b-121">Header</span></span>|<span data-ttu-id="ed97b-122">Wert</span><span class="sxs-lookup"><span data-stu-id="ed97b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ed97b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ed97b-123">Authorization</span></span>|<span data-ttu-id="ed97b-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="ed97b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ed97b-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="ed97b-125">Accept</span></span>|<span data-ttu-id="ed97b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ed97b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ed97b-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ed97b-127">Request body</span></span>
<span data-ttu-id="ed97b-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „sharedPCConfiguration“ an.</span><span class="sxs-lookup"><span data-stu-id="ed97b-128">In the request body, supply a JSON representation for the sharedPCConfiguration object.</span></span>

<span data-ttu-id="ed97b-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „sharedPCConfiguration“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="ed97b-129">The following table shows the properties that are required when you create the sharedPCConfiguration.</span></span>

|<span data-ttu-id="ed97b-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ed97b-130">Property</span></span>|<span data-ttu-id="ed97b-131">Typ</span><span class="sxs-lookup"><span data-stu-id="ed97b-131">Type</span></span>|<span data-ttu-id="ed97b-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ed97b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ed97b-133">id</span><span class="sxs-lookup"><span data-stu-id="ed97b-133">id</span></span>|<span data-ttu-id="ed97b-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ed97b-134">String</span></span>|<span data-ttu-id="ed97b-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="ed97b-135">Key of the entity.</span></span> <span data-ttu-id="ed97b-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ed97b-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ed97b-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ed97b-137">lastModifiedDateTime</span></span>|<span data-ttu-id="ed97b-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ed97b-138">DateTimeOffset</span></span>|<span data-ttu-id="ed97b-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="ed97b-139">DateTime the object was last modified.</span></span> <span data-ttu-id="ed97b-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ed97b-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ed97b-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ed97b-141">roleScopeTagIds</span></span>|<span data-ttu-id="ed97b-142">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="ed97b-142">String collection</span></span>|<span data-ttu-id="ed97b-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="ed97b-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ed97b-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ed97b-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ed97b-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="ed97b-145">supportsScopeTags</span></span>|<span data-ttu-id="ed97b-146">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="ed97b-146">Boolean</span></span>|<span data-ttu-id="ed97b-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ed97b-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="ed97b-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="ed97b-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="ed97b-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="ed97b-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="ed97b-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="ed97b-150">This property is read-only.</span></span> <span data-ttu-id="ed97b-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ed97b-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ed97b-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ed97b-152">createdDateTime</span></span>|<span data-ttu-id="ed97b-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ed97b-153">DateTimeOffset</span></span>|<span data-ttu-id="ed97b-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="ed97b-154">DateTime the object was created.</span></span> <span data-ttu-id="ed97b-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ed97b-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ed97b-156">description</span><span class="sxs-lookup"><span data-stu-id="ed97b-156">description</span></span>|<span data-ttu-id="ed97b-157">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ed97b-157">String</span></span>|<span data-ttu-id="ed97b-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="ed97b-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ed97b-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ed97b-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ed97b-160">displayName</span><span class="sxs-lookup"><span data-stu-id="ed97b-160">displayName</span></span>|<span data-ttu-id="ed97b-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ed97b-161">String</span></span>|<span data-ttu-id="ed97b-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="ed97b-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ed97b-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ed97b-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ed97b-164">Version</span><span class="sxs-lookup"><span data-stu-id="ed97b-164">version</span></span>|<span data-ttu-id="ed97b-165">Int32</span><span class="sxs-lookup"><span data-stu-id="ed97b-165">Int32</span></span>|<span data-ttu-id="ed97b-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="ed97b-166">Version of the device configuration.</span></span> <span data-ttu-id="ed97b-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ed97b-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ed97b-168">accountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="ed97b-168">accountManagerPolicy</span></span>|[<span data-ttu-id="ed97b-169">sharedPCAccountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="ed97b-169">sharedPCAccountManagerPolicy</span></span>](../resources/intune-deviceconfig-sharedpcaccountmanagerpolicy.md)|<span data-ttu-id="ed97b-170">Gibt an, wie die Konten auf dem freigegebenen PC verwaltet werden sollen.</span><span class="sxs-lookup"><span data-stu-id="ed97b-170">Specifies how accounts are managed on a shared PC.</span></span> <span data-ttu-id="ed97b-171">Gilt nur, wenn für „disableAccountManager“ der Wert „false“ gesetzt ist.</span><span class="sxs-lookup"><span data-stu-id="ed97b-171">Only applies when disableAccountManager is false.</span></span>|
|<span data-ttu-id="ed97b-172">allowedAccounts</span><span class="sxs-lookup"><span data-stu-id="ed97b-172">allowedAccounts</span></span>|[<span data-ttu-id="ed97b-173">sharedPCAllowedAccountType</span><span class="sxs-lookup"><span data-stu-id="ed97b-173">sharedPCAllowedAccountType</span></span>](../resources/intune-deviceconfig-sharedpcallowedaccounttype.md)|<span data-ttu-id="ed97b-174">Gibt an, welche Typen von Konten auf einem freigegebenen PC verwendet werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="ed97b-174">Indicates which type of accounts are allowed to use on a shared PC.</span></span> <span data-ttu-id="ed97b-175">Mögliche Werte sind: `guest` und `domain`.</span><span class="sxs-lookup"><span data-stu-id="ed97b-175">Possible values are: `guest`, `domain`.</span></span>|
|<span data-ttu-id="ed97b-176">localStorage</span><span class="sxs-lookup"><span data-stu-id="ed97b-176">localStorage</span></span>|[<span data-ttu-id="ed97b-177">Aktivierung von Steuerelementen</span><span class="sxs-lookup"><span data-stu-id="ed97b-177">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="ed97b-178">Gibt an, ob eine lokale Speicherung auf dem freigegebenen PC erlaubt ist.</span><span class="sxs-lookup"><span data-stu-id="ed97b-178">Specifies whether local storage is allowed on a shared PC.</span></span> <span data-ttu-id="ed97b-179">Mögliche Werte sind: `notConfigured`, `enabled` und `disabled`.</span><span class="sxs-lookup"><span data-stu-id="ed97b-179">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="ed97b-180">allowLocalStorage</span><span class="sxs-lookup"><span data-stu-id="ed97b-180">allowLocalStorage</span></span>|<span data-ttu-id="ed97b-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="ed97b-181">Boolean</span></span>|<span data-ttu-id="ed97b-182">Gibt an, ob eine lokale Speicherung auf dem freigegebenen PC erlaubt ist.</span><span class="sxs-lookup"><span data-stu-id="ed97b-182">Specifies whether local storage is allowed on a shared PC.</span></span>|
|<span data-ttu-id="ed97b-183">setAccountManager</span><span class="sxs-lookup"><span data-stu-id="ed97b-183">setAccountManager</span></span>|[<span data-ttu-id="ed97b-184">Aktivierung von Steuerelementen</span><span class="sxs-lookup"><span data-stu-id="ed97b-184">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="ed97b-185">Deaktiviert den Konto-Manager im Modus „Freigegebener PC“.</span><span class="sxs-lookup"><span data-stu-id="ed97b-185">Disables the account manager for shared PC mode.</span></span> <span data-ttu-id="ed97b-186">Mögliche Werte sind: `notConfigured`, `enabled` und `disabled`.</span><span class="sxs-lookup"><span data-stu-id="ed97b-186">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="ed97b-187">disableAccountManager</span><span class="sxs-lookup"><span data-stu-id="ed97b-187">disableAccountManager</span></span>|<span data-ttu-id="ed97b-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="ed97b-188">Boolean</span></span>|<span data-ttu-id="ed97b-189">Deaktiviert den Konto-Manager im Modus „Freigegebener PC“.</span><span class="sxs-lookup"><span data-stu-id="ed97b-189">Disables the account manager for shared PC mode.</span></span>|
|<span data-ttu-id="ed97b-190">setEduPolicies</span><span class="sxs-lookup"><span data-stu-id="ed97b-190">setEduPolicies</span></span>|[<span data-ttu-id="ed97b-191">Aktivierung von Steuerelementen</span><span class="sxs-lookup"><span data-stu-id="ed97b-191">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="ed97b-192">Gibt an, ob die standardmäßigen gemeinsamen PC Education-Umgebung Richtlinien aktiviert/deaktiviert/nicht konfiguriert werden soll.</span><span class="sxs-lookup"><span data-stu-id="ed97b-192">Specifies whether the default shared PC education environment policies should be enabled/disabled/not configured.</span></span> <span data-ttu-id="ed97b-193">Ab Windows 10 RS2 wird diese Richtlinie auch dann angewendet, wenn „enabled“ nicht auf „true“ gesetzt ist.</span><span class="sxs-lookup"><span data-stu-id="ed97b-193">For Windows 10 RS2 and later, this policy will be applied without setting Enabled to true.</span></span> <span data-ttu-id="ed97b-194">Mögliche Werte sind: `notConfigured`, `enabled` und `disabled`.</span><span class="sxs-lookup"><span data-stu-id="ed97b-194">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="ed97b-195">disableEduPolicies</span><span class="sxs-lookup"><span data-stu-id="ed97b-195">disableEduPolicies</span></span>|<span data-ttu-id="ed97b-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="ed97b-196">Boolean</span></span>|<span data-ttu-id="ed97b-197">Gibt an, ob die standardmäßigen Schulungsumgebungsrichtlinien für freigegebene PCs deaktiviert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="ed97b-197">Specifies whether the default shared PC education environment policies should be disabled.</span></span> <span data-ttu-id="ed97b-198">Ab Windows 10 RS2 wird diese Richtlinie auch dann angewendet, wenn „enabled“ nicht auf „true“ gesetzt ist.</span><span class="sxs-lookup"><span data-stu-id="ed97b-198">For Windows 10 RS2 and later, this policy will be applied without setting Enabled to true.</span></span>|
|<span data-ttu-id="ed97b-199">setPowerPolicies</span><span class="sxs-lookup"><span data-stu-id="ed97b-199">setPowerPolicies</span></span>|[<span data-ttu-id="ed97b-200">Aktivierung von Steuerelementen</span><span class="sxs-lookup"><span data-stu-id="ed97b-200">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="ed97b-201">Gibt an, ob die standardmäßigen gemeinsamen PC Power Richtlinien aktiviert/deaktiviert sollte sein.</span><span class="sxs-lookup"><span data-stu-id="ed97b-201">Specifies whether the default shared PC power policies should be enabled/disabled.</span></span> <span data-ttu-id="ed97b-202">Mögliche Werte sind: `notConfigured`, `enabled` und `disabled`.</span><span class="sxs-lookup"><span data-stu-id="ed97b-202">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="ed97b-203">disablePowerPolicies</span><span class="sxs-lookup"><span data-stu-id="ed97b-203">disablePowerPolicies</span></span>|<span data-ttu-id="ed97b-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="ed97b-204">Boolean</span></span>|<span data-ttu-id="ed97b-205">Gibt an, ob die standardmäßigen Energierichtlinien für freigegebene PCs deaktiviert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="ed97b-205">Specifies whether the default shared PC power policies should be disabled.</span></span>|
|<span data-ttu-id="ed97b-206">signInOnResume</span><span class="sxs-lookup"><span data-stu-id="ed97b-206">signInOnResume</span></span>|[<span data-ttu-id="ed97b-207">Aktivierung von Steuerelementen</span><span class="sxs-lookup"><span data-stu-id="ed97b-207">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="ed97b-208">Gibt die Anforderung zum Signieren in immer das Gerät reaktiviert aus dem Standbymodus.</span><span class="sxs-lookup"><span data-stu-id="ed97b-208">Specifies the requirement to sign in whenever the device wakes up from sleep mode.</span></span> <span data-ttu-id="ed97b-209">Mögliche Werte sind: `notConfigured`, `enabled` und `disabled`.</span><span class="sxs-lookup"><span data-stu-id="ed97b-209">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="ed97b-210">disableSignInOnResume</span><span class="sxs-lookup"><span data-stu-id="ed97b-210">disableSignInOnResume</span></span>|<span data-ttu-id="ed97b-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="ed97b-211">Boolean</span></span>|<span data-ttu-id="ed97b-212">Legt fest, dass nicht bei jedem Aufwachen des Geräts aus dem Energiesparmodus eine erneute Anmeldung erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="ed97b-212">Disables the requirement to sign in whenever the device wakes up from sleep mode.</span></span>|
|<span data-ttu-id="ed97b-213">enabled</span><span class="sxs-lookup"><span data-stu-id="ed97b-213">enabled</span></span>|<span data-ttu-id="ed97b-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="ed97b-214">Boolean</span></span>|<span data-ttu-id="ed97b-215">Aktiviert den Modus „Freigegebener PC“ und wendet die Richtlinien für freigegebene PCs an.</span><span class="sxs-lookup"><span data-stu-id="ed97b-215">Enables shared PC mode and applies the shared pc policies.</span></span>|
|<span data-ttu-id="ed97b-216">idleTimeBeforeSleepInSeconds</span><span class="sxs-lookup"><span data-stu-id="ed97b-216">idleTimeBeforeSleepInSeconds</span></span>|<span data-ttu-id="ed97b-217">Int32</span><span class="sxs-lookup"><span data-stu-id="ed97b-217">Int32</span></span>|<span data-ttu-id="ed97b-218">Gibt an, wie viele Sekunden sich der PC im Leerlauf befinden muss, bevor er in den Energiesparmodus geschaltet wird.</span><span class="sxs-lookup"><span data-stu-id="ed97b-218">Specifies the time in seconds that a device must sit idle before the PC goes to sleep.</span></span> <span data-ttu-id="ed97b-219">Wird dieser Wert auf „0“ gesetzt, greift kein Timeout, das den PC in den Energiesparmodus versetzt.</span><span class="sxs-lookup"><span data-stu-id="ed97b-219">Setting this value to 0 prevents the sleep timeout from occurring.</span></span>|
|<span data-ttu-id="ed97b-220">kioskAppDisplayName</span><span class="sxs-lookup"><span data-stu-id="ed97b-220">kioskAppDisplayName</span></span>|<span data-ttu-id="ed97b-221">String</span><span class="sxs-lookup"><span data-stu-id="ed97b-221">String</span></span>|<span data-ttu-id="ed97b-222">Gibt den Anzeigetext an, der dem Konto im Anmeldebildschirm angezeigt wird, über den die in „SetKioskAppUserModelId“ angegebene App gestartet wird.</span><span class="sxs-lookup"><span data-stu-id="ed97b-222">Specifies the display text for the account shown on the sign-in screen which launches the app specified by SetKioskAppUserModelId.</span></span> <span data-ttu-id="ed97b-223">Gilt nur, wenn für „kioskAppUserModelId“ ein Wert festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="ed97b-223">Only applies when KioskAppUserModelId is set.</span></span>|
|<span data-ttu-id="ed97b-224">kioskAppUserModelId</span><span class="sxs-lookup"><span data-stu-id="ed97b-224">kioskAppUserModelId</span></span>|<span data-ttu-id="ed97b-225">String</span><span class="sxs-lookup"><span data-stu-id="ed97b-225">String</span></span>|<span data-ttu-id="ed97b-226">Gibt die Anwendungsbenutzer-Modell-ID der App an, die über das Feature „Zugewiesener Zugriff“ genutzt werden darf.</span><span class="sxs-lookup"><span data-stu-id="ed97b-226">Specifies the application user model ID of the app to use with assigned access.</span></span>|
|<span data-ttu-id="ed97b-227">maintenanceStartTime</span><span class="sxs-lookup"><span data-stu-id="ed97b-227">maintenanceStartTime</span></span>|<span data-ttu-id="ed97b-228">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="ed97b-228">TimeOfDay</span></span>|<span data-ttu-id="ed97b-229">Gibt den Beginn des täglichen Wartungszeitraums an.</span><span class="sxs-lookup"><span data-stu-id="ed97b-229">Specifies the daily start time of maintenance hour.</span></span>|



## <a name="response"></a><span data-ttu-id="ed97b-230">Antwort</span><span class="sxs-lookup"><span data-stu-id="ed97b-230">Response</span></span>
<span data-ttu-id="ed97b-231">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) im Antworttext an.</span><span class="sxs-lookup"><span data-stu-id="ed97b-231">If successful, this method returns a `201 Created` response code and a [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ed97b-232">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ed97b-232">Example</span></span>
### <a name="request"></a><span data-ttu-id="ed97b-233">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ed97b-233">Request</span></span>
<span data-ttu-id="ed97b-234">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ed97b-234">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1179

{
  "@odata.type": "#microsoft.graph.sharedPCConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "accountManagerPolicy": {
    "@odata.type": "microsoft.graph.sharedPCAccountManagerPolicy",
    "accountDeletionPolicy": "diskSpaceThreshold",
    "cacheAccountsAboveDiskFreePercentage": 4,
    "inactiveThresholdDays": 5,
    "removeAccountsBelowDiskFreePercentage": 5
  },
  "allowedAccounts": "domain",
  "localStorage": "enabled",
  "allowLocalStorage": true,
  "setAccountManager": "enabled",
  "disableAccountManager": true,
  "setEduPolicies": "enabled",
  "disableEduPolicies": true,
  "setPowerPolicies": "enabled",
  "disablePowerPolicies": true,
  "signInOnResume": "enabled",
  "disableSignInOnResume": true,
  "enabled": true,
  "idleTimeBeforeSleepInSeconds": 12,
  "kioskAppDisplayName": "Kiosk App Display Name value",
  "kioskAppUserModelId": "Kiosk App User Model Id value",
  "maintenanceStartTime": "11:59:24.7240000"
}
```

### <a name="response"></a><span data-ttu-id="ed97b-235">Antwort</span><span class="sxs-lookup"><span data-stu-id="ed97b-235">Response</span></span>
<span data-ttu-id="ed97b-p121">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ed97b-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1287

{
  "@odata.type": "#microsoft.graph.sharedPCConfiguration",
  "id": "5206be3b-be3b-5206-3bbe-06523bbe0652",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "accountManagerPolicy": {
    "@odata.type": "microsoft.graph.sharedPCAccountManagerPolicy",
    "accountDeletionPolicy": "diskSpaceThreshold",
    "cacheAccountsAboveDiskFreePercentage": 4,
    "inactiveThresholdDays": 5,
    "removeAccountsBelowDiskFreePercentage": 5
  },
  "allowedAccounts": "domain",
  "localStorage": "enabled",
  "allowLocalStorage": true,
  "setAccountManager": "enabled",
  "disableAccountManager": true,
  "setEduPolicies": "enabled",
  "disableEduPolicies": true,
  "setPowerPolicies": "enabled",
  "disablePowerPolicies": true,
  "signInOnResume": "enabled",
  "disableSignInOnResume": true,
  "enabled": true,
  "idleTimeBeforeSleepInSeconds": 12,
  "kioskAppDisplayName": "Kiosk App Display Name value",
  "kioskAppUserModelId": "Kiosk App User Model Id value",
  "maintenanceStartTime": "11:59:24.7240000"
}
```





