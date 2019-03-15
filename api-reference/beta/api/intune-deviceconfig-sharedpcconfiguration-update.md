---
title: sharedPCConfiguration aktualisieren
description: Aktualisiert die Eigenschaften von Objekten des Typs sharedPCConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 88fb3da5ceb11cc58fb0e963d5adc9b5c5e227b9
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/14/2019
ms.locfileid: "30571518"
---
# <a name="update-sharedpcconfiguration"></a><span data-ttu-id="f1a0f-103">sharedPCConfiguration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="f1a0f-103">Update sharedPCConfiguration</span></span>

> <span data-ttu-id="f1a0f-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f1a0f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f1a0f-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="f1a0f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f1a0f-106">Aktualisiert die Eigenschaften von Objekten des Typs [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f1a0f-106">Update the properties of a [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f1a0f-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f1a0f-107">Prerequisites</span></span>
<span data-ttu-id="f1a0f-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="f1a0f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f1a0f-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f1a0f-110">Permission type</span></span>|<span data-ttu-id="f1a0f-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f1a0f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f1a0f-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f1a0f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f1a0f-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1a0f-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f1a0f-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f1a0f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f1a0f-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f1a0f-115">Not supported.</span></span>|
|<span data-ttu-id="f1a0f-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f1a0f-116">Application</span></span>|<span data-ttu-id="f1a0f-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f1a0f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f1a0f-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f1a0f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="f1a0f-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f1a0f-119">Request headers</span></span>
|<span data-ttu-id="f1a0f-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="f1a0f-120">Header</span></span>|<span data-ttu-id="f1a0f-121">Wert</span><span class="sxs-lookup"><span data-stu-id="f1a0f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f1a0f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f1a0f-122">Authorization</span></span>|<span data-ttu-id="f1a0f-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="f1a0f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f1a0f-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="f1a0f-124">Accept</span></span>|<span data-ttu-id="f1a0f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f1a0f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f1a0f-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f1a0f-126">Request body</span></span>
<span data-ttu-id="f1a0f-127">Geben Sie im Anforderungstext eine JSON-Darstellung des [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="f1a0f-127">In the request body, supply a JSON representation for the [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object.</span></span>

<span data-ttu-id="f1a0f-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md)-Objekts erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="f1a0f-128">The following table shows the properties that are required when you create the [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).</span></span>

|<span data-ttu-id="f1a0f-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f1a0f-129">Property</span></span>|<span data-ttu-id="f1a0f-130">Typ</span><span class="sxs-lookup"><span data-stu-id="f1a0f-130">Type</span></span>|<span data-ttu-id="f1a0f-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f1a0f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1a0f-132">id</span><span class="sxs-lookup"><span data-stu-id="f1a0f-132">id</span></span>|<span data-ttu-id="f1a0f-133">String</span><span class="sxs-lookup"><span data-stu-id="f1a0f-133">String</span></span>|<span data-ttu-id="f1a0f-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="f1a0f-134">Key of the entity.</span></span> <span data-ttu-id="f1a0f-135">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f1a0f-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1a0f-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f1a0f-136">lastModifiedDateTime</span></span>|<span data-ttu-id="f1a0f-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f1a0f-137">DateTimeOffset</span></span>|<span data-ttu-id="f1a0f-138">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="f1a0f-138">DateTime the object was last modified.</span></span> <span data-ttu-id="f1a0f-139">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f1a0f-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1a0f-140">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="f1a0f-140">roleScopeTagIds</span></span>|<span data-ttu-id="f1a0f-141">String collection</span><span class="sxs-lookup"><span data-stu-id="f1a0f-141">String collection</span></span>|<span data-ttu-id="f1a0f-142">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="f1a0f-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f1a0f-143">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f1a0f-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1a0f-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="f1a0f-144">supportsScopeTags</span></span>|<span data-ttu-id="f1a0f-145">Boolesch</span><span class="sxs-lookup"><span data-stu-id="f1a0f-145">Boolean</span></span>|<span data-ttu-id="f1a0f-146">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereichs Tags unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f1a0f-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f1a0f-147">Das Zuweisen zur ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert auf false festgelegt ist und Entitäten für bereichsbezogene Benutzer nicht sichtbar sind.</span><span class="sxs-lookup"><span data-stu-id="f1a0f-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f1a0f-148">Dies geschieht für in Silverlight erstellte Legacy Richtlinien und kann durch Löschen und erneutes Erstellen der Richtlinie im Azure-Portal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="f1a0f-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f1a0f-149">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="f1a0f-149">This property is read-only.</span></span> <span data-ttu-id="f1a0f-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f1a0f-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1a0f-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f1a0f-151">createdDateTime</span></span>|<span data-ttu-id="f1a0f-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f1a0f-152">DateTimeOffset</span></span>|<span data-ttu-id="f1a0f-153">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="f1a0f-153">DateTime the object was created.</span></span> <span data-ttu-id="f1a0f-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f1a0f-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1a0f-155">description</span><span class="sxs-lookup"><span data-stu-id="f1a0f-155">description</span></span>|<span data-ttu-id="f1a0f-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f1a0f-156">String</span></span>|<span data-ttu-id="f1a0f-157">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="f1a0f-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f1a0f-158">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f1a0f-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1a0f-159">displayName</span><span class="sxs-lookup"><span data-stu-id="f1a0f-159">displayName</span></span>|<span data-ttu-id="f1a0f-160">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f1a0f-160">String</span></span>|<span data-ttu-id="f1a0f-161">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="f1a0f-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f1a0f-162">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f1a0f-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1a0f-163">Version</span><span class="sxs-lookup"><span data-stu-id="f1a0f-163">version</span></span>|<span data-ttu-id="f1a0f-164">Int32</span><span class="sxs-lookup"><span data-stu-id="f1a0f-164">Int32</span></span>|<span data-ttu-id="f1a0f-165">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="f1a0f-165">Version of the device configuration.</span></span> <span data-ttu-id="f1a0f-166">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f1a0f-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1a0f-167">accountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="f1a0f-167">accountManagerPolicy</span></span>|[<span data-ttu-id="f1a0f-168">sharedPCAccountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="f1a0f-168">sharedPCAccountManagerPolicy</span></span>](../resources/intune-deviceconfig-sharedpcaccountmanagerpolicy.md)|<span data-ttu-id="f1a0f-169">Gibt an, wie die Konten auf dem freigegebenen PC verwaltet werden sollen.</span><span class="sxs-lookup"><span data-stu-id="f1a0f-169">Specifies how accounts are managed on a shared PC.</span></span> <span data-ttu-id="f1a0f-170">Gilt nur, wenn für „disableAccountManager“ der Wert „false“ gesetzt ist.</span><span class="sxs-lookup"><span data-stu-id="f1a0f-170">Only applies when disableAccountManager is false.</span></span>|
|<span data-ttu-id="f1a0f-171">allowedAccounts</span><span class="sxs-lookup"><span data-stu-id="f1a0f-171">allowedAccounts</span></span>|[<span data-ttu-id="f1a0f-172">sharedPCAllowedAccountType</span><span class="sxs-lookup"><span data-stu-id="f1a0f-172">sharedPCAllowedAccountType</span></span>](../resources/intune-deviceconfig-sharedpcallowedaccounttype.md)|<span data-ttu-id="f1a0f-173">Gibt an, welche Typen von Konten auf einem freigegebenen PC verwendet werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="f1a0f-173">Indicates which type of accounts are allowed to use on a shared PC.</span></span> <span data-ttu-id="f1a0f-174">Mögliche Werte sind: `notConfigured`, `guest` und `domain`.</span><span class="sxs-lookup"><span data-stu-id="f1a0f-174">Possible values are: `notConfigured`, `guest`, `domain`.</span></span>|
|<span data-ttu-id="f1a0f-175">localStorage</span><span class="sxs-lookup"><span data-stu-id="f1a0f-175">localStorage</span></span>|[<span data-ttu-id="f1a0f-176">Aktivierung</span><span class="sxs-lookup"><span data-stu-id="f1a0f-176">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="f1a0f-177">Gibt an, ob eine lokale Speicherung auf dem freigegebenen PC erlaubt ist.</span><span class="sxs-lookup"><span data-stu-id="f1a0f-177">Specifies whether local storage is allowed on a shared PC.</span></span> <span data-ttu-id="f1a0f-178">Mögliche Werte sind: `notConfigured`, `enabled` und `disabled`.</span><span class="sxs-lookup"><span data-stu-id="f1a0f-178">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="f1a0f-179">allowLocalStorage</span><span class="sxs-lookup"><span data-stu-id="f1a0f-179">allowLocalStorage</span></span>|<span data-ttu-id="f1a0f-180">Boolesch</span><span class="sxs-lookup"><span data-stu-id="f1a0f-180">Boolean</span></span>|<span data-ttu-id="f1a0f-181">Gibt an, ob eine lokale Speicherung auf dem freigegebenen PC erlaubt ist.</span><span class="sxs-lookup"><span data-stu-id="f1a0f-181">Specifies whether local storage is allowed on a shared PC.</span></span>|
|<span data-ttu-id="f1a0f-182">setAccountmanager</span><span class="sxs-lookup"><span data-stu-id="f1a0f-182">setAccountManager</span></span>|[<span data-ttu-id="f1a0f-183">Aktivierung</span><span class="sxs-lookup"><span data-stu-id="f1a0f-183">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="f1a0f-184">Deaktiviert den Konto-Manager im Modus „Freigegebener PC“.</span><span class="sxs-lookup"><span data-stu-id="f1a0f-184">Disables the account manager for shared PC mode.</span></span> <span data-ttu-id="f1a0f-185">Mögliche Werte sind: `notConfigured`, `enabled` und `disabled`.</span><span class="sxs-lookup"><span data-stu-id="f1a0f-185">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="f1a0f-186">disableAccountManager</span><span class="sxs-lookup"><span data-stu-id="f1a0f-186">disableAccountManager</span></span>|<span data-ttu-id="f1a0f-187">Boolesch</span><span class="sxs-lookup"><span data-stu-id="f1a0f-187">Boolean</span></span>|<span data-ttu-id="f1a0f-188">Deaktiviert den Konto-Manager im Modus „Freigegebener PC“.</span><span class="sxs-lookup"><span data-stu-id="f1a0f-188">Disables the account manager for shared PC mode.</span></span>|
|<span data-ttu-id="f1a0f-189">setEduPolicies</span><span class="sxs-lookup"><span data-stu-id="f1a0f-189">setEduPolicies</span></span>|[<span data-ttu-id="f1a0f-190">Aktivierung</span><span class="sxs-lookup"><span data-stu-id="f1a0f-190">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="f1a0f-191">Gibt an, ob die Standardrichtlinien für freigegebene PC Education-Umgebungen aktiviert/deaktiviert/nicht konfiguriert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="f1a0f-191">Specifies whether the default shared PC education environment policies should be enabled/disabled/not configured.</span></span> <span data-ttu-id="f1a0f-192">Ab Windows 10 RS2 wird diese Richtlinie auch dann angewendet, wenn „enabled“ nicht auf „true“ gesetzt ist.</span><span class="sxs-lookup"><span data-stu-id="f1a0f-192">For Windows 10 RS2 and later, this policy will be applied without setting Enabled to true.</span></span> <span data-ttu-id="f1a0f-193">Mögliche Werte sind: `notConfigured`, `enabled` und `disabled`.</span><span class="sxs-lookup"><span data-stu-id="f1a0f-193">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="f1a0f-194">disableEduPolicies</span><span class="sxs-lookup"><span data-stu-id="f1a0f-194">disableEduPolicies</span></span>|<span data-ttu-id="f1a0f-195">Boolesch</span><span class="sxs-lookup"><span data-stu-id="f1a0f-195">Boolean</span></span>|<span data-ttu-id="f1a0f-196">Gibt an, ob die standardmäßigen Schulungsumgebungsrichtlinien für freigegebene PCs deaktiviert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="f1a0f-196">Specifies whether the default shared PC education environment policies should be disabled.</span></span> <span data-ttu-id="f1a0f-197">Ab Windows 10 RS2 wird diese Richtlinie auch dann angewendet, wenn „enabled“ nicht auf „true“ gesetzt ist.</span><span class="sxs-lookup"><span data-stu-id="f1a0f-197">For Windows 10 RS2 and later, this policy will be applied without setting Enabled to true.</span></span>|
|<span data-ttu-id="f1a0f-198">setPowerPolicies</span><span class="sxs-lookup"><span data-stu-id="f1a0f-198">setPowerPolicies</span></span>|[<span data-ttu-id="f1a0f-199">Aktivierung</span><span class="sxs-lookup"><span data-stu-id="f1a0f-199">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="f1a0f-200">Gibt an, ob die standardmäßigen freigegebenen PC-Energierichtlinien aktiviert/deaktiviert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="f1a0f-200">Specifies whether the default shared PC power policies should be enabled/disabled.</span></span> <span data-ttu-id="f1a0f-201">Mögliche Werte sind: `notConfigured`, `enabled` und `disabled`.</span><span class="sxs-lookup"><span data-stu-id="f1a0f-201">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="f1a0f-202">disablePowerPolicies</span><span class="sxs-lookup"><span data-stu-id="f1a0f-202">disablePowerPolicies</span></span>|<span data-ttu-id="f1a0f-203">Boolesch</span><span class="sxs-lookup"><span data-stu-id="f1a0f-203">Boolean</span></span>|<span data-ttu-id="f1a0f-204">Gibt an, ob die standardmäßigen Energierichtlinien für freigegebene PCs deaktiviert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="f1a0f-204">Specifies whether the default shared PC power policies should be disabled.</span></span>|
|<span data-ttu-id="f1a0f-205">signInOnResume</span><span class="sxs-lookup"><span data-stu-id="f1a0f-205">signInOnResume</span></span>|[<span data-ttu-id="f1a0f-206">Aktivierung</span><span class="sxs-lookup"><span data-stu-id="f1a0f-206">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="f1a0f-207">Gibt die Anforderung an, sich anzumelden, wenn das Gerät aus dem Energiesparmodus aktiviert wird.</span><span class="sxs-lookup"><span data-stu-id="f1a0f-207">Specifies the requirement to sign in whenever the device wakes up from sleep mode.</span></span> <span data-ttu-id="f1a0f-208">Mögliche Werte sind: `notConfigured`, `enabled` und `disabled`.</span><span class="sxs-lookup"><span data-stu-id="f1a0f-208">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="f1a0f-209">disableSignInOnResume</span><span class="sxs-lookup"><span data-stu-id="f1a0f-209">disableSignInOnResume</span></span>|<span data-ttu-id="f1a0f-210">Boolesch</span><span class="sxs-lookup"><span data-stu-id="f1a0f-210">Boolean</span></span>|<span data-ttu-id="f1a0f-211">Legt fest, dass nicht bei jedem Aufwachen des Geräts aus dem Energiesparmodus eine erneute Anmeldung erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="f1a0f-211">Disables the requirement to sign in whenever the device wakes up from sleep mode.</span></span>|
|<span data-ttu-id="f1a0f-212">aktiviert</span><span class="sxs-lookup"><span data-stu-id="f1a0f-212">enabled</span></span>|<span data-ttu-id="f1a0f-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="f1a0f-213">Boolean</span></span>|<span data-ttu-id="f1a0f-214">Aktiviert den Modus „Freigegebener PC“ und wendet die Richtlinien für freigegebene PCs an.</span><span class="sxs-lookup"><span data-stu-id="f1a0f-214">Enables shared PC mode and applies the shared pc policies.</span></span>|
|<span data-ttu-id="f1a0f-215">idleTimeBeforeSleepInSeconds</span><span class="sxs-lookup"><span data-stu-id="f1a0f-215">idleTimeBeforeSleepInSeconds</span></span>|<span data-ttu-id="f1a0f-216">Int32</span><span class="sxs-lookup"><span data-stu-id="f1a0f-216">Int32</span></span>|<span data-ttu-id="f1a0f-217">Gibt an, wie viele Sekunden sich der PC im Leerlauf befinden muss, bevor er in den Energiesparmodus geschaltet wird.</span><span class="sxs-lookup"><span data-stu-id="f1a0f-217">Specifies the time in seconds that a device must sit idle before the PC goes to sleep.</span></span> <span data-ttu-id="f1a0f-218">Wird dieser Wert auf „0“ gesetzt, greift kein Timeout, das den PC in den Energiesparmodus versetzt.</span><span class="sxs-lookup"><span data-stu-id="f1a0f-218">Setting this value to 0 prevents the sleep timeout from occurring.</span></span>|
|<span data-ttu-id="f1a0f-219">kioskAppDisplayName</span><span class="sxs-lookup"><span data-stu-id="f1a0f-219">kioskAppDisplayName</span></span>|<span data-ttu-id="f1a0f-220">String</span><span class="sxs-lookup"><span data-stu-id="f1a0f-220">String</span></span>|<span data-ttu-id="f1a0f-221">Gibt den Anzeigetext an, der dem Konto im Anmeldebildschirm angezeigt wird, über den die in „SetKioskAppUserModelId“ angegebene App gestartet wird.</span><span class="sxs-lookup"><span data-stu-id="f1a0f-221">Specifies the display text for the account shown on the sign-in screen which launches the app specified by SetKioskAppUserModelId.</span></span> <span data-ttu-id="f1a0f-222">Gilt nur, wenn für „kioskAppUserModelId“ ein Wert festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="f1a0f-222">Only applies when KioskAppUserModelId is set.</span></span>|
|<span data-ttu-id="f1a0f-223">kioskAppUserModelId</span><span class="sxs-lookup"><span data-stu-id="f1a0f-223">kioskAppUserModelId</span></span>|<span data-ttu-id="f1a0f-224">String</span><span class="sxs-lookup"><span data-stu-id="f1a0f-224">String</span></span>|<span data-ttu-id="f1a0f-225">Gibt die Anwendungsbenutzer-Modell-ID der App an, die über das Feature „Zugewiesener Zugriff“ genutzt werden darf.</span><span class="sxs-lookup"><span data-stu-id="f1a0f-225">Specifies the application user model ID of the app to use with assigned access.</span></span>|
|<span data-ttu-id="f1a0f-226">maintenanceStartTime</span><span class="sxs-lookup"><span data-stu-id="f1a0f-226">maintenanceStartTime</span></span>|<span data-ttu-id="f1a0f-227">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="f1a0f-227">TimeOfDay</span></span>|<span data-ttu-id="f1a0f-228">Gibt den Beginn des täglichen Wartungszeitraums an.</span><span class="sxs-lookup"><span data-stu-id="f1a0f-228">Specifies the daily start time of maintenance hour.</span></span>|
|<span data-ttu-id="f1a0f-229">fastFirstSignIn</span><span class="sxs-lookup"><span data-stu-id="f1a0f-229">fastFirstSignIn</span></span>|[<span data-ttu-id="f1a0f-230">Aktivierung</span><span class="sxs-lookup"><span data-stu-id="f1a0f-230">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="f1a0f-231">Gibt an, ob neue nicht-Administrator-Azure AD-Konten mit vorkonfigurierten Kandidaten lokalen Konten automatisch verbunden werden sollen.</span><span class="sxs-lookup"><span data-stu-id="f1a0f-231">Specifies whether to auto connect new non-admin Azure AD accounts to pre-configured candidate local accounts.</span></span> <span data-ttu-id="f1a0f-232">Mögliche Werte sind: `notConfigured`, `enabled` und `disabled`.</span><span class="sxs-lookup"><span data-stu-id="f1a0f-232">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|



## <a name="response"></a><span data-ttu-id="f1a0f-233">Antwort</span><span class="sxs-lookup"><span data-stu-id="f1a0f-233">Response</span></span>
<span data-ttu-id="f1a0f-234">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein aktualisiertes [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f1a0f-234">If successful, this method returns a `200 OK` response code and an updated [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f1a0f-235">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f1a0f-235">Example</span></span>

### <a name="request"></a><span data-ttu-id="f1a0f-236">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f1a0f-236">Request</span></span>
<span data-ttu-id="f1a0f-237">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f1a0f-237">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1147

{
  "@odata.type": "#microsoft.graph.sharedPCConfiguration",
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
  "allowedAccounts": "guest",
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
  "maintenanceStartTime": "11:59:24.7240000",
  "fastFirstSignIn": "enabled"
}
```

### <a name="response"></a><span data-ttu-id="f1a0f-238">Antwort</span><span class="sxs-lookup"><span data-stu-id="f1a0f-238">Response</span></span>
<span data-ttu-id="f1a0f-p121">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f1a0f-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1319

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
  "allowedAccounts": "guest",
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
  "maintenanceStartTime": "11:59:24.7240000",
  "fastFirstSignIn": "enabled"
}
```




