---
title: sharedPCConfiguration aktualisieren
description: Aktualisiert die Eigenschaften von Objekten des Typs sharedPCConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: da0cbba1de768fffd572728d3d416de83917e582
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396329"
---
# <a name="update-sharedpcconfiguration"></a><span data-ttu-id="8649a-103">sharedPCConfiguration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="8649a-103">Update sharedPCConfiguration</span></span>

> <span data-ttu-id="8649a-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="8649a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="8649a-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8649a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8649a-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8649a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8649a-107">Aktualisiert die Eigenschaften von Objekten des Typs [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8649a-107">Update the properties of a [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8649a-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="8649a-108">Prerequisites</span></span>
<span data-ttu-id="8649a-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="8649a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="8649a-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8649a-111">Permission type</span></span>|<span data-ttu-id="8649a-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8649a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8649a-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8649a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8649a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8649a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8649a-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8649a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8649a-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8649a-116">Not supported.</span></span>|
|<span data-ttu-id="8649a-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8649a-117">Application</span></span>|<span data-ttu-id="8649a-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8649a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8649a-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8649a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="8649a-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8649a-120">Request headers</span></span>
|<span data-ttu-id="8649a-121">Header</span><span class="sxs-lookup"><span data-stu-id="8649a-121">Header</span></span>|<span data-ttu-id="8649a-122">Wert</span><span class="sxs-lookup"><span data-stu-id="8649a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8649a-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="8649a-123">Authorization</span></span>|<span data-ttu-id="8649a-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="8649a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8649a-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="8649a-125">Accept</span></span>|<span data-ttu-id="8649a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8649a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8649a-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8649a-127">Request body</span></span>
<span data-ttu-id="8649a-128">Geben Sie im Anforderungstext eine JSON-Darstellung des [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="8649a-128">In the request body, supply a JSON representation for the [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object.</span></span>

<span data-ttu-id="8649a-129">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md)-Objekts erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="8649a-129">The following table shows the properties that are required when you create the [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).</span></span>

|<span data-ttu-id="8649a-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8649a-130">Property</span></span>|<span data-ttu-id="8649a-131">Typ</span><span class="sxs-lookup"><span data-stu-id="8649a-131">Type</span></span>|<span data-ttu-id="8649a-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8649a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8649a-133">id</span><span class="sxs-lookup"><span data-stu-id="8649a-133">id</span></span>|<span data-ttu-id="8649a-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8649a-134">String</span></span>|<span data-ttu-id="8649a-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="8649a-135">Key of the entity.</span></span> <span data-ttu-id="8649a-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8649a-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8649a-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8649a-137">lastModifiedDateTime</span></span>|<span data-ttu-id="8649a-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8649a-138">DateTimeOffset</span></span>|<span data-ttu-id="8649a-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="8649a-139">DateTime the object was last modified.</span></span> <span data-ttu-id="8649a-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8649a-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8649a-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8649a-141">roleScopeTagIds</span></span>|<span data-ttu-id="8649a-142">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="8649a-142">String collection</span></span>|<span data-ttu-id="8649a-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="8649a-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="8649a-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8649a-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8649a-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="8649a-145">supportsScopeTags</span></span>|<span data-ttu-id="8649a-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="8649a-146">Boolean</span></span>|<span data-ttu-id="8649a-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8649a-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="8649a-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="8649a-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="8649a-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="8649a-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="8649a-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="8649a-150">This property is read-only.</span></span> <span data-ttu-id="8649a-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8649a-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8649a-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8649a-152">createdDateTime</span></span>|<span data-ttu-id="8649a-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8649a-153">DateTimeOffset</span></span>|<span data-ttu-id="8649a-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="8649a-154">DateTime the object was created.</span></span> <span data-ttu-id="8649a-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8649a-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8649a-156">description</span><span class="sxs-lookup"><span data-stu-id="8649a-156">description</span></span>|<span data-ttu-id="8649a-157">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8649a-157">String</span></span>|<span data-ttu-id="8649a-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="8649a-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="8649a-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8649a-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8649a-160">displayName</span><span class="sxs-lookup"><span data-stu-id="8649a-160">displayName</span></span>|<span data-ttu-id="8649a-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8649a-161">String</span></span>|<span data-ttu-id="8649a-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="8649a-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="8649a-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8649a-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8649a-164">Version</span><span class="sxs-lookup"><span data-stu-id="8649a-164">version</span></span>|<span data-ttu-id="8649a-165">Int32</span><span class="sxs-lookup"><span data-stu-id="8649a-165">Int32</span></span>|<span data-ttu-id="8649a-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="8649a-166">Version of the device configuration.</span></span> <span data-ttu-id="8649a-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8649a-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8649a-168">accountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="8649a-168">accountManagerPolicy</span></span>|[<span data-ttu-id="8649a-169">sharedPCAccountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="8649a-169">sharedPCAccountManagerPolicy</span></span>](../resources/intune-deviceconfig-sharedpcaccountmanagerpolicy.md)|<span data-ttu-id="8649a-170">Gibt an, wie die Konten auf dem freigegebenen PC verwaltet werden sollen.</span><span class="sxs-lookup"><span data-stu-id="8649a-170">Specifies how accounts are managed on a shared PC.</span></span> <span data-ttu-id="8649a-171">Gilt nur, wenn für „disableAccountManager“ der Wert „false“ gesetzt ist.</span><span class="sxs-lookup"><span data-stu-id="8649a-171">Only applies when disableAccountManager is false.</span></span>|
|<span data-ttu-id="8649a-172">allowedAccounts</span><span class="sxs-lookup"><span data-stu-id="8649a-172">allowedAccounts</span></span>|[<span data-ttu-id="8649a-173">sharedPCAllowedAccountType</span><span class="sxs-lookup"><span data-stu-id="8649a-173">sharedPCAllowedAccountType</span></span>](../resources/intune-deviceconfig-sharedpcallowedaccounttype.md)|<span data-ttu-id="8649a-174">Gibt an, welche Typen von Konten auf einem freigegebenen PC verwendet werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="8649a-174">Indicates which type of accounts are allowed to use on a shared PC.</span></span> <span data-ttu-id="8649a-175">Mögliche Werte sind: `notConfigured`, `guest` und `domain`.</span><span class="sxs-lookup"><span data-stu-id="8649a-175">Possible values are: `notConfigured`, `guest`, `domain`.</span></span>|
|<span data-ttu-id="8649a-176">localStorage</span><span class="sxs-lookup"><span data-stu-id="8649a-176">localStorage</span></span>|<span data-ttu-id="8649a-177">[Aktivierung] (.. /Resources/Intune-Shared-Enablement</span><span class="sxs-lookup"><span data-stu-id="8649a-177">[enablement](../resources/intune-shared-enablement</span></span>
<span data-ttu-id="8649a-178">.MD)</span><span class="sxs-lookup"><span data-stu-id="8649a-178">.md)</span></span>|<span data-ttu-id="8649a-179">Gibt an, ob eine lokale Speicherung auf dem freigegebenen PC erlaubt ist.</span><span class="sxs-lookup"><span data-stu-id="8649a-179">Specifies whether local storage is allowed on a shared PC.</span></span> <span data-ttu-id="8649a-180">Mögliche Werte sind: `notConfigured`, `enabled` und `disabled`.</span><span class="sxs-lookup"><span data-stu-id="8649a-180">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="8649a-181">allowLocalStorage</span><span class="sxs-lookup"><span data-stu-id="8649a-181">allowLocalStorage</span></span>|<span data-ttu-id="8649a-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="8649a-182">Boolean</span></span>|<span data-ttu-id="8649a-183">Gibt an, ob eine lokale Speicherung auf dem freigegebenen PC erlaubt ist.</span><span class="sxs-lookup"><span data-stu-id="8649a-183">Specifies whether local storage is allowed on a shared PC.</span></span>|
|<span data-ttu-id="8649a-184">setAccountManager</span><span class="sxs-lookup"><span data-stu-id="8649a-184">setAccountManager</span></span>|<span data-ttu-id="8649a-185">[Aktivierung] (.. /Resources/Intune-Shared-Enablement</span><span class="sxs-lookup"><span data-stu-id="8649a-185">[enablement](../resources/intune-shared-enablement</span></span>
<span data-ttu-id="8649a-186">.MD)</span><span class="sxs-lookup"><span data-stu-id="8649a-186">.md)</span></span>|<span data-ttu-id="8649a-187">Deaktiviert den Konto-Manager im Modus „Freigegebener PC“.</span><span class="sxs-lookup"><span data-stu-id="8649a-187">Disables the account manager for shared PC mode.</span></span> <span data-ttu-id="8649a-188">Mögliche Werte sind: `notConfigured`, `enabled` und `disabled`.</span><span class="sxs-lookup"><span data-stu-id="8649a-188">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="8649a-189">disableAccountManager</span><span class="sxs-lookup"><span data-stu-id="8649a-189">disableAccountManager</span></span>|<span data-ttu-id="8649a-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="8649a-190">Boolean</span></span>|<span data-ttu-id="8649a-191">Deaktiviert den Konto-Manager im Modus „Freigegebener PC“.</span><span class="sxs-lookup"><span data-stu-id="8649a-191">Disables the account manager for shared PC mode.</span></span>|
|<span data-ttu-id="8649a-192">setEduPolicies</span><span class="sxs-lookup"><span data-stu-id="8649a-192">setEduPolicies</span></span>|<span data-ttu-id="8649a-193">[Aktivierung] (.. /Resources/Intune-Shared-Enablement</span><span class="sxs-lookup"><span data-stu-id="8649a-193">[enablement](../resources/intune-shared-enablement</span></span>
<span data-ttu-id="8649a-194">.MD)</span><span class="sxs-lookup"><span data-stu-id="8649a-194">.md)</span></span>|<span data-ttu-id="8649a-195">Gibt an, ob die standardmäßigen gemeinsamen PC Education-Umgebung Richtlinien aktiviert/deaktiviert/nicht konfiguriert werden soll.</span><span class="sxs-lookup"><span data-stu-id="8649a-195">Specifies whether the default shared PC education environment policies should be enabled/disabled/not configured.</span></span> <span data-ttu-id="8649a-196">Ab Windows 10 RS2 wird diese Richtlinie auch dann angewendet, wenn „enabled“ nicht auf „true“ gesetzt ist.</span><span class="sxs-lookup"><span data-stu-id="8649a-196">For Windows 10 RS2 and later, this policy will be applied without setting Enabled to true.</span></span> <span data-ttu-id="8649a-197">Mögliche Werte sind: `notConfigured`, `enabled` und `disabled`.</span><span class="sxs-lookup"><span data-stu-id="8649a-197">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="8649a-198">disableEduPolicies</span><span class="sxs-lookup"><span data-stu-id="8649a-198">disableEduPolicies</span></span>|<span data-ttu-id="8649a-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="8649a-199">Boolean</span></span>|<span data-ttu-id="8649a-200">Gibt an, ob die standardmäßigen Schulungsumgebungsrichtlinien für freigegebene PCs deaktiviert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="8649a-200">Specifies whether the default shared PC education environment policies should be disabled.</span></span> <span data-ttu-id="8649a-201">Ab Windows 10 RS2 wird diese Richtlinie auch dann angewendet, wenn „enabled“ nicht auf „true“ gesetzt ist.</span><span class="sxs-lookup"><span data-stu-id="8649a-201">For Windows 10 RS2 and later, this policy will be applied without setting Enabled to true.</span></span>|
|<span data-ttu-id="8649a-202">setPowerPolicies</span><span class="sxs-lookup"><span data-stu-id="8649a-202">setPowerPolicies</span></span>|<span data-ttu-id="8649a-203">[Aktivierung] (.. /Resources/Intune-Shared-Enablement</span><span class="sxs-lookup"><span data-stu-id="8649a-203">[enablement](../resources/intune-shared-enablement</span></span>
<span data-ttu-id="8649a-204">.MD)</span><span class="sxs-lookup"><span data-stu-id="8649a-204">.md)</span></span>|<span data-ttu-id="8649a-205">Gibt an, ob die standardmäßigen gemeinsamen PC Power Richtlinien aktiviert/deaktiviert sollte sein.</span><span class="sxs-lookup"><span data-stu-id="8649a-205">Specifies whether the default shared PC power policies should be enabled/disabled.</span></span> <span data-ttu-id="8649a-206">Mögliche Werte sind: `notConfigured`, `enabled` und `disabled`.</span><span class="sxs-lookup"><span data-stu-id="8649a-206">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="8649a-207">disablePowerPolicies</span><span class="sxs-lookup"><span data-stu-id="8649a-207">disablePowerPolicies</span></span>|<span data-ttu-id="8649a-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="8649a-208">Boolean</span></span>|<span data-ttu-id="8649a-209">Gibt an, ob die standardmäßigen Energierichtlinien für freigegebene PCs deaktiviert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="8649a-209">Specifies whether the default shared PC power policies should be disabled.</span></span>|
|<span data-ttu-id="8649a-210">signInOnResume</span><span class="sxs-lookup"><span data-stu-id="8649a-210">signInOnResume</span></span>|<span data-ttu-id="8649a-211">[Aktivierung] (.. /Resources/Intune-Shared-Enablement</span><span class="sxs-lookup"><span data-stu-id="8649a-211">[enablement](../resources/intune-shared-enablement</span></span>
<span data-ttu-id="8649a-212">.MD)</span><span class="sxs-lookup"><span data-stu-id="8649a-212">.md)</span></span>|<span data-ttu-id="8649a-213">Gibt die Anforderung zum Signieren in immer das Gerät reaktiviert aus dem Standbymodus.</span><span class="sxs-lookup"><span data-stu-id="8649a-213">Specifies the requirement to sign in whenever the device wakes up from sleep mode.</span></span> <span data-ttu-id="8649a-214">Mögliche Werte sind: `notConfigured`, `enabled` und `disabled`.</span><span class="sxs-lookup"><span data-stu-id="8649a-214">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="8649a-215">disableSignInOnResume</span><span class="sxs-lookup"><span data-stu-id="8649a-215">disableSignInOnResume</span></span>|<span data-ttu-id="8649a-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="8649a-216">Boolean</span></span>|<span data-ttu-id="8649a-217">Legt fest, dass nicht bei jedem Aufwachen des Geräts aus dem Energiesparmodus eine erneute Anmeldung erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="8649a-217">Disables the requirement to sign in whenever the device wakes up from sleep mode.</span></span>|
|<span data-ttu-id="8649a-218">enabled</span><span class="sxs-lookup"><span data-stu-id="8649a-218">enabled</span></span>|<span data-ttu-id="8649a-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="8649a-219">Boolean</span></span>|<span data-ttu-id="8649a-220">Aktiviert den Modus „Freigegebener PC“ und wendet die Richtlinien für freigegebene PCs an.</span><span class="sxs-lookup"><span data-stu-id="8649a-220">Enables shared PC mode and applies the shared pc policies.</span></span>|
|<span data-ttu-id="8649a-221">idleTimeBeforeSleepInSeconds</span><span class="sxs-lookup"><span data-stu-id="8649a-221">idleTimeBeforeSleepInSeconds</span></span>|<span data-ttu-id="8649a-222">Int32</span><span class="sxs-lookup"><span data-stu-id="8649a-222">Int32</span></span>|<span data-ttu-id="8649a-223">Gibt an, wie viele Sekunden sich der PC im Leerlauf befinden muss, bevor er in den Energiesparmodus geschaltet wird.</span><span class="sxs-lookup"><span data-stu-id="8649a-223">Specifies the time in seconds that a device must sit idle before the PC goes to sleep.</span></span> <span data-ttu-id="8649a-224">Wird dieser Wert auf „0“ gesetzt, greift kein Timeout, das den PC in den Energiesparmodus versetzt.</span><span class="sxs-lookup"><span data-stu-id="8649a-224">Setting this value to 0 prevents the sleep timeout from occurring.</span></span>|
|<span data-ttu-id="8649a-225">kioskAppDisplayName</span><span class="sxs-lookup"><span data-stu-id="8649a-225">kioskAppDisplayName</span></span>|<span data-ttu-id="8649a-226">String</span><span class="sxs-lookup"><span data-stu-id="8649a-226">String</span></span>|<span data-ttu-id="8649a-227">Gibt den Anzeigetext an, der dem Konto im Anmeldebildschirm angezeigt wird, über den die in „SetKioskAppUserModelId“ angegebene App gestartet wird.</span><span class="sxs-lookup"><span data-stu-id="8649a-227">Specifies the display text for the account shown on the sign-in screen which launches the app specified by SetKioskAppUserModelId.</span></span> <span data-ttu-id="8649a-228">Gilt nur, wenn für „kioskAppUserModelId“ ein Wert festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="8649a-228">Only applies when KioskAppUserModelId is set.</span></span>|
|<span data-ttu-id="8649a-229">kioskAppUserModelId</span><span class="sxs-lookup"><span data-stu-id="8649a-229">kioskAppUserModelId</span></span>|<span data-ttu-id="8649a-230">String</span><span class="sxs-lookup"><span data-stu-id="8649a-230">String</span></span>|<span data-ttu-id="8649a-231">Gibt die Anwendungsbenutzer-Modell-ID der App an, die über das Feature „Zugewiesener Zugriff“ genutzt werden darf.</span><span class="sxs-lookup"><span data-stu-id="8649a-231">Specifies the application user model ID of the app to use with assigned access.</span></span>|
|<span data-ttu-id="8649a-232">maintenanceStartTime</span><span class="sxs-lookup"><span data-stu-id="8649a-232">maintenanceStartTime</span></span>|<span data-ttu-id="8649a-233">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="8649a-233">TimeOfDay</span></span>|<span data-ttu-id="8649a-234">Gibt den Beginn des täglichen Wartungszeitraums an.</span><span class="sxs-lookup"><span data-stu-id="8649a-234">Specifies the daily start time of maintenance hour.</span></span>|



## <a name="response"></a><span data-ttu-id="8649a-235">Antwort</span><span class="sxs-lookup"><span data-stu-id="8649a-235">Response</span></span>
<span data-ttu-id="8649a-236">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein aktualisiertes [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8649a-236">If successful, this method returns a `200 OK` response code and an updated [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8649a-237">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8649a-237">Example</span></span>

### <a name="request"></a><span data-ttu-id="8649a-238">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8649a-238">Request</span></span>
<span data-ttu-id="8649a-239">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8649a-239">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1114

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
  "maintenanceStartTime": "11:59:24.7240000"
}
```

### <a name="response"></a><span data-ttu-id="8649a-240">Antwort</span><span class="sxs-lookup"><span data-stu-id="8649a-240">Response</span></span>
<span data-ttu-id="8649a-p121">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8649a-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1286

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
  "maintenanceStartTime": "11:59:24.7240000"
}
```




