---
title: WindowsIdentityProtectionConfiguration erstellen
description: Erstellen eines neuen windowsIdentityProtectionConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 061d4796c25bf04306ede1001bfa18cb61fa5020
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30144457"
---
# <a name="create-windowsidentityprotectionconfiguration"></a><span data-ttu-id="d4cb9-103">WindowsIdentityProtectionConfiguration erstellen</span><span class="sxs-lookup"><span data-stu-id="d4cb9-103">Create windowsIdentityProtectionConfiguration</span></span>

> <span data-ttu-id="d4cb9-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d4cb9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d4cb9-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="d4cb9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d4cb9-106">Erstellen eines neuen [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="d4cb9-106">Create a new [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d4cb9-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="d4cb9-107">Prerequisites</span></span>
<span data-ttu-id="d4cb9-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="d4cb9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="d4cb9-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d4cb9-110">Permission type</span></span>|<span data-ttu-id="d4cb9-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d4cb9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d4cb9-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d4cb9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d4cb9-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4cb9-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d4cb9-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d4cb9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d4cb9-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d4cb9-115">Not supported.</span></span>|
|<span data-ttu-id="d4cb9-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d4cb9-116">Application</span></span>|<span data-ttu-id="d4cb9-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d4cb9-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d4cb9-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d4cb9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="d4cb9-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d4cb9-119">Request headers</span></span>
|<span data-ttu-id="d4cb9-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="d4cb9-120">Header</span></span>|<span data-ttu-id="d4cb9-121">Wert</span><span class="sxs-lookup"><span data-stu-id="d4cb9-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d4cb9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d4cb9-122">Authorization</span></span>|<span data-ttu-id="d4cb9-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="d4cb9-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d4cb9-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="d4cb9-124">Accept</span></span>|<span data-ttu-id="d4cb9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d4cb9-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d4cb9-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d4cb9-126">Request body</span></span>
<span data-ttu-id="d4cb9-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das windowsIdentityProtectionConfiguration-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="d4cb9-127">In the request body, supply a JSON representation for the windowsIdentityProtectionConfiguration object.</span></span>

<span data-ttu-id="d4cb9-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der windowsIdentityProtectionConfiguration erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="d4cb9-128">The following table shows the properties that are required when you create the windowsIdentityProtectionConfiguration.</span></span>

|<span data-ttu-id="d4cb9-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d4cb9-129">Property</span></span>|<span data-ttu-id="d4cb9-130">Typ</span><span class="sxs-lookup"><span data-stu-id="d4cb9-130">Type</span></span>|<span data-ttu-id="d4cb9-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d4cb9-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d4cb9-132">id</span><span class="sxs-lookup"><span data-stu-id="d4cb9-132">id</span></span>|<span data-ttu-id="d4cb9-133">string</span><span class="sxs-lookup"><span data-stu-id="d4cb9-133">String</span></span>|<span data-ttu-id="d4cb9-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="d4cb9-134">Key of the entity.</span></span> <span data-ttu-id="d4cb9-135">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d4cb9-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d4cb9-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d4cb9-136">lastModifiedDateTime</span></span>|<span data-ttu-id="d4cb9-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d4cb9-137">DateTimeOffset</span></span>|<span data-ttu-id="d4cb9-138">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="d4cb9-138">DateTime the object was last modified.</span></span> <span data-ttu-id="d4cb9-139">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d4cb9-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d4cb9-140">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="d4cb9-140">roleScopeTagIds</span></span>|<span data-ttu-id="d4cb9-141">String collection</span><span class="sxs-lookup"><span data-stu-id="d4cb9-141">String collection</span></span>|<span data-ttu-id="d4cb9-142">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="d4cb9-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d4cb9-143">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d4cb9-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d4cb9-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="d4cb9-144">supportsScopeTags</span></span>|<span data-ttu-id="d4cb9-145">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d4cb9-145">Boolean</span></span>|<span data-ttu-id="d4cb9-146">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereichs Tags unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d4cb9-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="d4cb9-147">Das Zuweisen zur ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert auf false festgelegt ist und Entitäten für bereichsbezogene Benutzer nicht sichtbar sind.</span><span class="sxs-lookup"><span data-stu-id="d4cb9-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="d4cb9-148">Dies geschieht für in Silverlight erstellte Legacy Richtlinien und kann durch Löschen und erneutes Erstellen der Richtlinie im Azure-Portal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="d4cb9-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="d4cb9-149">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d4cb9-149">This property is read-only.</span></span> <span data-ttu-id="d4cb9-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d4cb9-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d4cb9-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d4cb9-151">createdDateTime</span></span>|<span data-ttu-id="d4cb9-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d4cb9-152">DateTimeOffset</span></span>|<span data-ttu-id="d4cb9-153">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="d4cb9-153">DateTime the object was created.</span></span> <span data-ttu-id="d4cb9-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d4cb9-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d4cb9-155">description</span><span class="sxs-lookup"><span data-stu-id="d4cb9-155">description</span></span>|<span data-ttu-id="d4cb9-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d4cb9-156">String</span></span>|<span data-ttu-id="d4cb9-157">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="d4cb9-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d4cb9-158">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d4cb9-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d4cb9-159">displayName</span><span class="sxs-lookup"><span data-stu-id="d4cb9-159">displayName</span></span>|<span data-ttu-id="d4cb9-160">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d4cb9-160">String</span></span>|<span data-ttu-id="d4cb9-161">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="d4cb9-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d4cb9-162">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d4cb9-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d4cb9-163">Version</span><span class="sxs-lookup"><span data-stu-id="d4cb9-163">version</span></span>|<span data-ttu-id="d4cb9-164">Int32</span><span class="sxs-lookup"><span data-stu-id="d4cb9-164">Int32</span></span>|<span data-ttu-id="d4cb9-165">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="d4cb9-165">Version of the device configuration.</span></span> <span data-ttu-id="d4cb9-166">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d4cb9-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d4cb9-167">useSecurityKeyForSignin</span><span class="sxs-lookup"><span data-stu-id="d4cb9-167">useSecurityKeyForSignin</span></span>|<span data-ttu-id="d4cb9-168">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d4cb9-168">Boolean</span></span>|<span data-ttu-id="d4cb9-169">Boolescher Wert, der zum Aktivieren des Windows Hello-Sicherheitsschlüssels als Anmeldeinformationen verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="d4cb9-169">Boolean value used to enable the Windows Hello security key as a logon credential.</span></span>|
|<span data-ttu-id="d4cb9-170">enhancedAntiSpoofingForFacialFeaturesEnabled</span><span class="sxs-lookup"><span data-stu-id="d4cb9-170">enhancedAntiSpoofingForFacialFeaturesEnabled</span></span>|<span data-ttu-id="d4cb9-171">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d4cb9-171">Boolean</span></span>|<span data-ttu-id="d4cb9-172">Boolescher Wert, mit dem Enhanced Anti-Spoofing für die Erkennung von gesichtsfunktionen unter Windows Hello Face Authentication aktiviert wird.</span><span class="sxs-lookup"><span data-stu-id="d4cb9-172">Boolean value used to enable enhanced anti-spoofing for facial feature recognition on Windows Hello face authentication.</span></span>|
|<span data-ttu-id="d4cb9-173">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="d4cb9-173">pinMinimumLength</span></span>|<span data-ttu-id="d4cb9-174">Int32</span><span class="sxs-lookup"><span data-stu-id="d4cb9-174">Int32</span></span>|<span data-ttu-id="d4cb9-175">Ganzzahliger Wert, der die Mindestanzahl von Zeichen für die Windows-Hello for Business-PIN festlegt.</span><span class="sxs-lookup"><span data-stu-id="d4cb9-175">Integer value that sets the minimum number of characters required for the Windows Hello for Business PIN.</span></span> <span data-ttu-id="d4cb9-176">Gültige Werte sind 4 bis 127 inklusive und kleiner als oder gleich dem Wert, der für die maximale PIN festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="d4cb9-176">Valid values are 4 to 127 inclusive and less than or equal to the value set for the maximum PIN.</span></span> <span data-ttu-id="d4cb9-177">Gültige Werte 4 bis 127</span><span class="sxs-lookup"><span data-stu-id="d4cb9-177">Valid values 4 to 127</span></span>|
|<span data-ttu-id="d4cb9-178">pinMaximumLength</span><span class="sxs-lookup"><span data-stu-id="d4cb9-178">pinMaximumLength</span></span>|<span data-ttu-id="d4cb9-179">Int32</span><span class="sxs-lookup"><span data-stu-id="d4cb9-179">Int32</span></span>|<span data-ttu-id="d4cb9-180">Ganzzahliger Wert, der die maximale Anzahl der zulässigen Zeichen für die Arbeits-PIN festlegt.</span><span class="sxs-lookup"><span data-stu-id="d4cb9-180">Integer value that sets the maximum number of characters allowed for the work PIN.</span></span> <span data-ttu-id="d4cb9-181">Gültige Werte sind 4 bis 127 inklusive und größer oder gleich dem Wert, der für die minimale PIN festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="d4cb9-181">Valid values are 4 to 127 inclusive and greater than or equal to the value set for the minimum PIN.</span></span> <span data-ttu-id="d4cb9-182">Gültige Werte 4 bis 127</span><span class="sxs-lookup"><span data-stu-id="d4cb9-182">Valid values 4 to 127</span></span>|
|<span data-ttu-id="d4cb9-183">pinUppercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="d4cb9-183">pinUppercaseCharactersUsage</span></span>|[<span data-ttu-id="d4cb9-184">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="d4cb9-184">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="d4cb9-185">Dieser Wert konfiguriert die Verwendung von Großbuchstaben in der Windows Hello for Business-PIN.</span><span class="sxs-lookup"><span data-stu-id="d4cb9-185">This value configures the use of uppercase characters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="d4cb9-186">Mögliche Werte sind: `blocked`, `required` und `allowed`.</span><span class="sxs-lookup"><span data-stu-id="d4cb9-186">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="d4cb9-187">pinLowercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="d4cb9-187">pinLowercaseCharactersUsage</span></span>|[<span data-ttu-id="d4cb9-188">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="d4cb9-188">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="d4cb9-189">Dieser Wert konfiguriert die Verwendung von Kleinbuchstaben in der Windows Hello for Business-PIN.</span><span class="sxs-lookup"><span data-stu-id="d4cb9-189">This value configures the use of lowercase characters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="d4cb9-190">Mögliche Werte sind: `blocked`, `required` und `allowed`.</span><span class="sxs-lookup"><span data-stu-id="d4cb9-190">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="d4cb9-191">pinSpecialCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="d4cb9-191">pinSpecialCharactersUsage</span></span>|[<span data-ttu-id="d4cb9-192">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="d4cb9-192">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="d4cb9-193">Steuert die Möglichkeit, Sonderzeichen in der Windows Hello for Business-PIN zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="d4cb9-193">Controls the ability to use special characters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="d4cb9-194">Mögliche Werte sind: `blocked`, `required` und `allowed`.</span><span class="sxs-lookup"><span data-stu-id="d4cb9-194">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="d4cb9-195">pinExpirationInDays</span><span class="sxs-lookup"><span data-stu-id="d4cb9-195">pinExpirationInDays</span></span>|<span data-ttu-id="d4cb9-196">Int32</span><span class="sxs-lookup"><span data-stu-id="d4cb9-196">Int32</span></span>|<span data-ttu-id="d4cb9-197">Ganzzahliger Wert gibt den Zeitraum (in Tagen) an, an dem eine PIN verwendet werden kann, bevor das System den Benutzer zum Ändern benötigt.</span><span class="sxs-lookup"><span data-stu-id="d4cb9-197">Integer value specifies the period (in days) that a PIN can be used before the system requires the user to change it.</span></span> <span data-ttu-id="d4cb9-198">Gültige Werte sind 0 bis 730 inklusive.</span><span class="sxs-lookup"><span data-stu-id="d4cb9-198">Valid values are 0 to 730 inclusive.</span></span> <span data-ttu-id="d4cb9-199">Gültige Werte: 0 bis 730.</span><span class="sxs-lookup"><span data-stu-id="d4cb9-199">Valid values 0 to 730</span></span>|
|<span data-ttu-id="d4cb9-200">pinPreviousBlockCount</span><span class="sxs-lookup"><span data-stu-id="d4cb9-200">pinPreviousBlockCount</span></span>|<span data-ttu-id="d4cb9-201">Int32</span><span class="sxs-lookup"><span data-stu-id="d4cb9-201">Int32</span></span>|<span data-ttu-id="d4cb9-202">Steuert, wie verhindert werden kann, dass Benutzer frühere PINs verwenden.</span><span class="sxs-lookup"><span data-stu-id="d4cb9-202">Controls the ability to prevent users from using past PINs.</span></span> <span data-ttu-id="d4cb9-203">Dieser muss zwischen 0 und 50 einschließlich festgelegt werden, und die aktuelle PIN des Benutzers ist in dieser Anzahl enthalten.</span><span class="sxs-lookup"><span data-stu-id="d4cb9-203">This must be set between 0 and 50, inclusive, and the current PIN of the user is included in that count.</span></span> <span data-ttu-id="d4cb9-204">Bei Festlegung auf 0 werden frühere PINs nicht gespeichert.</span><span class="sxs-lookup"><span data-stu-id="d4cb9-204">If set to 0, previous PINs are not stored.</span></span> <span data-ttu-id="d4cb9-205">Der PIN-Verlauf wird nicht durch eine PIN-Zurücksetzung beibehalten.</span><span class="sxs-lookup"><span data-stu-id="d4cb9-205">PIN history is not preserved through a PIN reset.</span></span> <span data-ttu-id="d4cb9-206">Gültige Werte: 0 bis 50.</span><span class="sxs-lookup"><span data-stu-id="d4cb9-206">Valid values 0 to 50</span></span>|
|<span data-ttu-id="d4cb9-207">pinRecoveryEnabled</span><span class="sxs-lookup"><span data-stu-id="d4cb9-207">pinRecoveryEnabled</span></span>|<span data-ttu-id="d4cb9-208">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d4cb9-208">Boolean</span></span>|<span data-ttu-id="d4cb9-209">Boolescher Wert, der es einem Benutzer ermöglicht, seine PIN mithilfe des Windows Hello for Business-PIN-Wiederherstellungs Diensts zu ändern.</span><span class="sxs-lookup"><span data-stu-id="d4cb9-209">Boolean value that enables a user to change their PIN by using the Windows Hello for Business PIN recovery service.</span></span>|
|<span data-ttu-id="d4cb9-210">securityDeviceRequired</span><span class="sxs-lookup"><span data-stu-id="d4cb9-210">securityDeviceRequired</span></span>|<span data-ttu-id="d4cb9-211">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d4cb9-211">Boolean</span></span>|<span data-ttu-id="d4cb9-212">Steuert, ob ein Trusted Platform Module (TPM) für die Einrichtung von Windows Hello for Business erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="d4cb9-212">Controls whether to require a Trusted Platform Module (TPM) for provisioning Windows Hello for Business.</span></span> <span data-ttu-id="d4cb9-213">Ein TPM bietet einen zusätzlichen Sicherheitsvorteil, da darin gespeicherte Daten nicht auf anderen Geräten verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="d4cb9-213">A TPM provides an additional security benefit in that data stored on it cannot be used on other devices.</span></span> <span data-ttu-id="d4cb9-214">Wenn dieser Wert auf false festgelegt ist, können alle Geräte Windows Hello for Business auch dann zur Verfügung stellen, wenn kein TPM verfügbar ist.</span><span class="sxs-lookup"><span data-stu-id="d4cb9-214">If set to False, all devices can provision Windows Hello for Business even if there is not a usable TPM.</span></span>|
|<span data-ttu-id="d4cb9-215">unlockWithBiometricsEnabled</span><span class="sxs-lookup"><span data-stu-id="d4cb9-215">unlockWithBiometricsEnabled</span></span>|<span data-ttu-id="d4cb9-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="d4cb9-216">Boolean</span></span>|<span data-ttu-id="d4cb9-217">Steuert die Verwendung von biometrischen Gesten wie Gesicht und Fingerabdruck als Alternative zur Windows Hello for Business-PIN.</span><span class="sxs-lookup"><span data-stu-id="d4cb9-217">Controls the use of biometric gestures, such as face and fingerprint, as an alternative to the Windows Hello for Business PIN.</span></span>  <span data-ttu-id="d4cb9-218">Wenn dieser Wert auf false festgelegt ist, sind biometrische Gesten nicht zulässig.</span><span class="sxs-lookup"><span data-stu-id="d4cb9-218">If set to False, biometric gestures are not allowed.</span></span> <span data-ttu-id="d4cb9-219">Benutzer müssen bei Fehlern weiterhin eine PIN als Sicherung konfigurieren.</span><span class="sxs-lookup"><span data-stu-id="d4cb9-219">Users must still configure a PIN as a backup in case of failures.</span></span>|
|<span data-ttu-id="d4cb9-220">useCertificatesForOnPremisesAuthEnabled</span><span class="sxs-lookup"><span data-stu-id="d4cb9-220">useCertificatesForOnPremisesAuthEnabled</span></span>|<span data-ttu-id="d4cb9-221">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d4cb9-221">Boolean</span></span>|<span data-ttu-id="d4cb9-222">Boolescher Wert, der es Windows Hello for Business ermöglicht, Zertifikate zur Authentifizierung lokaler Ressourcen zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="d4cb9-222">Boolean value that enables Windows Hello for Business to use certificates to authenticate on-premise resources.</span></span>|
|<span data-ttu-id="d4cb9-223">windowsHelloForBusinessBlocked</span><span class="sxs-lookup"><span data-stu-id="d4cb9-223">windowsHelloForBusinessBlocked</span></span>|<span data-ttu-id="d4cb9-224">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d4cb9-224">Boolean</span></span>|<span data-ttu-id="d4cb9-225">Boolescher Wert, der Windows Hello for Business als Methode für die Anmeldung an Windows blockiert.</span><span class="sxs-lookup"><span data-stu-id="d4cb9-225">Boolean value that blocks Windows Hello for Business as a method for signing into Windows.</span></span>|



## <a name="response"></a><span data-ttu-id="d4cb9-226">Antwort</span><span class="sxs-lookup"><span data-stu-id="d4cb9-226">Response</span></span>
<span data-ttu-id="d4cb9-227">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="d4cb9-227">If successful, this method returns a `201 Created` response code and a [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d4cb9-228">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d4cb9-228">Example</span></span>

### <a name="request"></a><span data-ttu-id="d4cb9-229">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d4cb9-229">Request</span></span>
<span data-ttu-id="d4cb9-230">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d4cb9-230">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 810

{
  "@odata.type": "#microsoft.graph.windowsIdentityProtectionConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "useSecurityKeyForSignin": true,
  "enhancedAntiSpoofingForFacialFeaturesEnabled": true,
  "pinMinimumLength": 0,
  "pinMaximumLength": 0,
  "pinUppercaseCharactersUsage": "required",
  "pinLowercaseCharactersUsage": "required",
  "pinSpecialCharactersUsage": "required",
  "pinExpirationInDays": 3,
  "pinPreviousBlockCount": 5,
  "pinRecoveryEnabled": true,
  "securityDeviceRequired": true,
  "unlockWithBiometricsEnabled": true,
  "useCertificatesForOnPremisesAuthEnabled": true,
  "windowsHelloForBusinessBlocked": true
}
```

### <a name="response"></a><span data-ttu-id="d4cb9-231">Antwort</span><span class="sxs-lookup"><span data-stu-id="d4cb9-231">Response</span></span>
<span data-ttu-id="d4cb9-p119">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d4cb9-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 982

{
  "@odata.type": "#microsoft.graph.windowsIdentityProtectionConfiguration",
  "id": "b2e64303-4303-b2e6-0343-e6b20343e6b2",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "useSecurityKeyForSignin": true,
  "enhancedAntiSpoofingForFacialFeaturesEnabled": true,
  "pinMinimumLength": 0,
  "pinMaximumLength": 0,
  "pinUppercaseCharactersUsage": "required",
  "pinLowercaseCharactersUsage": "required",
  "pinSpecialCharactersUsage": "required",
  "pinExpirationInDays": 3,
  "pinPreviousBlockCount": 5,
  "pinRecoveryEnabled": true,
  "securityDeviceRequired": true,
  "unlockWithBiometricsEnabled": true,
  "useCertificatesForOnPremisesAuthEnabled": true,
  "windowsHelloForBusinessBlocked": true
}
```




