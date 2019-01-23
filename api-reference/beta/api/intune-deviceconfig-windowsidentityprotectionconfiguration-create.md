---
title: Erstellen von windowsIdentityProtectionConfiguration
description: Erstellen eines neuen WindowsIdentityProtectionConfiguration-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: be9c6ad30eb869bfd47b20863fc41e103eabe1c2
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29408992"
---
# <a name="create-windowsidentityprotectionconfiguration"></a><span data-ttu-id="c5537-103">Erstellen von windowsIdentityProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="c5537-103">Create windowsIdentityProtectionConfiguration</span></span>

> <span data-ttu-id="c5537-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="c5537-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c5537-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c5537-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c5537-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c5537-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c5537-107">Erstellen eines neuen [WindowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="c5537-107">Create a new [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c5537-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c5537-108">Prerequisites</span></span>
<span data-ttu-id="c5537-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="c5537-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="c5537-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c5537-111">Permission type</span></span>|<span data-ttu-id="c5537-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c5537-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c5537-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c5537-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c5537-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5537-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c5537-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c5537-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c5537-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c5537-116">Not supported.</span></span>|
|<span data-ttu-id="c5537-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c5537-117">Application</span></span>|<span data-ttu-id="c5537-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c5537-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c5537-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c5537-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="c5537-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c5537-120">Request headers</span></span>
|<span data-ttu-id="c5537-121">Header</span><span class="sxs-lookup"><span data-stu-id="c5537-121">Header</span></span>|<span data-ttu-id="c5537-122">Wert</span><span class="sxs-lookup"><span data-stu-id="c5537-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c5537-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="c5537-123">Authorization</span></span>|<span data-ttu-id="c5537-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c5537-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c5537-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="c5537-125">Accept</span></span>|<span data-ttu-id="c5537-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c5537-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c5537-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c5537-127">Request body</span></span>
<span data-ttu-id="c5537-128">Geben Sie im Textkörper Anforderung für das Objekt WindowsIdentityProtectionConfiguration eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="c5537-128">In the request body, supply a JSON representation for the windowsIdentityProtectionConfiguration object.</span></span>

<span data-ttu-id="c5537-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die WindowsIdentityProtectionConfiguration erstellen.</span><span class="sxs-lookup"><span data-stu-id="c5537-129">The following table shows the properties that are required when you create the windowsIdentityProtectionConfiguration.</span></span>

|<span data-ttu-id="c5537-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c5537-130">Property</span></span>|<span data-ttu-id="c5537-131">Typ</span><span class="sxs-lookup"><span data-stu-id="c5537-131">Type</span></span>|<span data-ttu-id="c5537-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c5537-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c5537-133">id</span><span class="sxs-lookup"><span data-stu-id="c5537-133">id</span></span>|<span data-ttu-id="c5537-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c5537-134">String</span></span>|<span data-ttu-id="c5537-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="c5537-135">Key of the entity.</span></span> <span data-ttu-id="c5537-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c5537-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c5537-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c5537-137">lastModifiedDateTime</span></span>|<span data-ttu-id="c5537-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c5537-138">DateTimeOffset</span></span>|<span data-ttu-id="c5537-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="c5537-139">DateTime the object was last modified.</span></span> <span data-ttu-id="c5537-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c5537-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c5537-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c5537-141">roleScopeTagIds</span></span>|<span data-ttu-id="c5537-142">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="c5537-142">String collection</span></span>|<span data-ttu-id="c5537-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="c5537-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c5537-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c5537-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c5537-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="c5537-145">supportsScopeTags</span></span>|<span data-ttu-id="c5537-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5537-146">Boolean</span></span>|<span data-ttu-id="c5537-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c5537-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="c5537-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="c5537-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="c5537-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="c5537-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="c5537-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="c5537-150">This property is read-only.</span></span> <span data-ttu-id="c5537-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c5537-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c5537-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c5537-152">createdDateTime</span></span>|<span data-ttu-id="c5537-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c5537-153">DateTimeOffset</span></span>|<span data-ttu-id="c5537-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="c5537-154">DateTime the object was created.</span></span> <span data-ttu-id="c5537-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c5537-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c5537-156">description</span><span class="sxs-lookup"><span data-stu-id="c5537-156">description</span></span>|<span data-ttu-id="c5537-157">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c5537-157">String</span></span>|<span data-ttu-id="c5537-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="c5537-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c5537-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c5537-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c5537-160">displayName</span><span class="sxs-lookup"><span data-stu-id="c5537-160">displayName</span></span>|<span data-ttu-id="c5537-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c5537-161">String</span></span>|<span data-ttu-id="c5537-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="c5537-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c5537-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c5537-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c5537-164">Version</span><span class="sxs-lookup"><span data-stu-id="c5537-164">version</span></span>|<span data-ttu-id="c5537-165">Int32</span><span class="sxs-lookup"><span data-stu-id="c5537-165">Int32</span></span>|<span data-ttu-id="c5537-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="c5537-166">Version of the device configuration.</span></span> <span data-ttu-id="c5537-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c5537-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c5537-168">useSecurityKeyForSignin</span><span class="sxs-lookup"><span data-stu-id="c5537-168">useSecurityKeyForSignin</span></span>|<span data-ttu-id="c5537-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5537-169">Boolean</span></span>|<span data-ttu-id="c5537-170">Boolescher Wert zum Aktivieren des Windows-Hello Sicherheitsschlüssel als eine-Anmeldeinformationen verwendet.</span><span class="sxs-lookup"><span data-stu-id="c5537-170">Boolean value used to enable the Windows Hello security key as a logon credential.</span></span>|
|<span data-ttu-id="c5537-171">enhancedAntiSpoofingForFacialFeaturesEnabled</span><span class="sxs-lookup"><span data-stu-id="c5537-171">enhancedAntiSpoofingForFacialFeaturesEnabled</span></span>|<span data-ttu-id="c5537-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5537-172">Boolean</span></span>|<span data-ttu-id="c5537-173">Boolescher Wert verwendet, um erweiterte Anti-spoofing für die Spracherkennung auf Windows Hello Gesicht Authentifizierung Gesichtsausdruck Feature aktivieren.</span><span class="sxs-lookup"><span data-stu-id="c5537-173">Boolean value used to enable enhanced anti-spoofing for facial feature recognition on Windows Hello face authentication.</span></span>|
|<span data-ttu-id="c5537-174">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="c5537-174">pinMinimumLength</span></span>|<span data-ttu-id="c5537-175">Int32</span><span class="sxs-lookup"><span data-stu-id="c5537-175">Int32</span></span>|<span data-ttu-id="c5537-176">Integer-Wert, der die Mindestanzahl der Zeichen für den Windows Hello für Business PIN benötigt wird.</span><span class="sxs-lookup"><span data-stu-id="c5537-176">Integer value that sets the minimum number of characters required for the Windows Hello for Business PIN.</span></span> <span data-ttu-id="c5537-177">Gültige Werte sind 4 bis 127 und kleiner als oder gleich dem Wert für die maximale PIN festlegen.</span><span class="sxs-lookup"><span data-stu-id="c5537-177">Valid values are 4 to 127 inclusive and less than or equal to the value set for the maximum PIN.</span></span> <span data-ttu-id="c5537-178">Gültige Werte 4 bis 127</span><span class="sxs-lookup"><span data-stu-id="c5537-178">Valid values 4 to 127</span></span>|
|<span data-ttu-id="c5537-179">pinMaximumLength</span><span class="sxs-lookup"><span data-stu-id="c5537-179">pinMaximumLength</span></span>|<span data-ttu-id="c5537-180">Int32</span><span class="sxs-lookup"><span data-stu-id="c5537-180">Int32</span></span>|<span data-ttu-id="c5537-181">Integer-Wert, der die maximale Anzahl der zulässigen Zeichen für die Arbeit PIN festlegt.</span><span class="sxs-lookup"><span data-stu-id="c5537-181">Integer value that sets the maximum number of characters allowed for the work PIN.</span></span> <span data-ttu-id="c5537-182">Gültige Werte sind 4 bis 127 inklusive und größer als oder gleich dem Wert für die minimale PIN festlegen.</span><span class="sxs-lookup"><span data-stu-id="c5537-182">Valid values are 4 to 127 inclusive and greater than or equal to the value set for the minimum PIN.</span></span> <span data-ttu-id="c5537-183">Gültige Werte 4 bis 127</span><span class="sxs-lookup"><span data-stu-id="c5537-183">Valid values 4 to 127</span></span>|
|<span data-ttu-id="c5537-184">pinUppercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="c5537-184">pinUppercaseCharactersUsage</span></span>|[<span data-ttu-id="c5537-185">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="c5537-185">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="c5537-186">Dieser Wert konfiguriert die Verwendung von Großbuchstaben in der Windows Hello für Business PIN ein.</span><span class="sxs-lookup"><span data-stu-id="c5537-186">This value configures the use of uppercase characters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="c5537-187">Mögliche Werte sind: `blocked`, `required` und `allowed`.</span><span class="sxs-lookup"><span data-stu-id="c5537-187">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="c5537-188">pinLowercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="c5537-188">pinLowercaseCharactersUsage</span></span>|[<span data-ttu-id="c5537-189">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="c5537-189">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="c5537-190">Dieser Wert konfiguriert die Verwendung von Kleinbuchstaben in der Windows Hello für Business PIN ein.</span><span class="sxs-lookup"><span data-stu-id="c5537-190">This value configures the use of lowercase characters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="c5537-191">Mögliche Werte sind: `blocked`, `required` und `allowed`.</span><span class="sxs-lookup"><span data-stu-id="c5537-191">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="c5537-192">pinSpecialCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="c5537-192">pinSpecialCharactersUsage</span></span>|[<span data-ttu-id="c5537-193">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="c5537-193">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="c5537-194">Steuert die Möglichkeit, Sonderzeichen in der Windows Hello für Business PIN verwenden.</span><span class="sxs-lookup"><span data-stu-id="c5537-194">Controls the ability to use special characters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="c5537-195">Mögliche Werte sind: `blocked`, `required` und `allowed`.</span><span class="sxs-lookup"><span data-stu-id="c5537-195">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="c5537-196">pinExpirationInDays</span><span class="sxs-lookup"><span data-stu-id="c5537-196">pinExpirationInDays</span></span>|<span data-ttu-id="c5537-197">Int32</span><span class="sxs-lookup"><span data-stu-id="c5537-197">Int32</span></span>|<span data-ttu-id="c5537-198">Integer-Wert gibt den Zeitraum (in Tagen) an, dass eine PIN-Nummer verwendet werden kann, bevor das System den Benutzer es ändern müssen.</span><span class="sxs-lookup"><span data-stu-id="c5537-198">Integer value specifies the period (in days) that a PIN can be used before the system requires the user to change it.</span></span> <span data-ttu-id="c5537-199">Gültige Werte sind 0, 730.</span><span class="sxs-lookup"><span data-stu-id="c5537-199">Valid values are 0 to 730 inclusive.</span></span> <span data-ttu-id="c5537-200">Gültige Werte: 0 bis 730.</span><span class="sxs-lookup"><span data-stu-id="c5537-200">Valid values 0 to 730</span></span>|
|<span data-ttu-id="c5537-201">pinPreviousBlockCount</span><span class="sxs-lookup"><span data-stu-id="c5537-201">pinPreviousBlockCount</span></span>|<span data-ttu-id="c5537-202">Int32</span><span class="sxs-lookup"><span data-stu-id="c5537-202">Int32</span></span>|<span data-ttu-id="c5537-203">Steuert die Möglichkeit, zu verhindern, dass Benutzer die ältere PINs verwenden.</span><span class="sxs-lookup"><span data-stu-id="c5537-203">Controls the ability to prevent users from using past PINs.</span></span> <span data-ttu-id="c5537-204">Dies muss zwischen 0 und 50, einschließlich festgelegt werden, und die aktuelle PIN des Benutzers in diese Zählung eingeschlossen ist.</span><span class="sxs-lookup"><span data-stu-id="c5537-204">This must be set between 0 and 50, inclusive, and the current PIN of the user is included in that count.</span></span> <span data-ttu-id="c5537-205">Wenn auf 0 gesetzt, vorherigen PINs nicht gespeichert werden.</span><span class="sxs-lookup"><span data-stu-id="c5537-205">If set to 0, previous PINs are not stored.</span></span> <span data-ttu-id="c5537-206">PIN-Verlauf wird nicht beibehalten, über eine PIN zurücksetzen.</span><span class="sxs-lookup"><span data-stu-id="c5537-206">PIN history is not preserved through a PIN reset.</span></span> <span data-ttu-id="c5537-207">Gültige Werte: 0 bis 50.</span><span class="sxs-lookup"><span data-stu-id="c5537-207">Valid values 0 to 50</span></span>|
|<span data-ttu-id="c5537-208">pinRecoveryEnabled</span><span class="sxs-lookup"><span data-stu-id="c5537-208">pinRecoveryEnabled</span></span>|<span data-ttu-id="c5537-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5537-209">Boolean</span></span>|<span data-ttu-id="c5537-210">Boolescher Wert, mit der einen Benutzer seine PIN mithilfe der Windows Hello für Recovery-Service Business PIN ändern kann.</span><span class="sxs-lookup"><span data-stu-id="c5537-210">Boolean value that enables a user to change their PIN by using the Windows Hello for Business PIN recovery service.</span></span>|
|<span data-ttu-id="c5537-211">securityDeviceRequired</span><span class="sxs-lookup"><span data-stu-id="c5537-211">securityDeviceRequired</span></span>|<span data-ttu-id="c5537-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5537-212">Boolean</span></span>|<span data-ttu-id="c5537-213">Steuert, ob ein vertrauenswürdiger Platform-Modul (TPM) für die Bereitstellung von Windows Hello für Unternehmen erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="c5537-213">Controls whether to require a Trusted Platform Module (TPM) for provisioning Windows Hello for Business.</span></span> <span data-ttu-id="c5537-214">Ein TPM bietet einen zusätzliche Sicherheit-Vorteil, dass darauf gespeicherte Daten auf anderen Geräten verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="c5537-214">A TPM provides an additional security benefit in that data stored on it cannot be used on other devices.</span></span> <span data-ttu-id="c5537-215">Wenn auf False festgelegt, alle Geräte Windows Hello für Unternehmen bereitstellen können, auch wenn ein verwendbar TPM nicht vorhanden ist.</span><span class="sxs-lookup"><span data-stu-id="c5537-215">If set to False, all devices can provision Windows Hello for Business even if there is not a usable TPM.</span></span>|
|<span data-ttu-id="c5537-216">unlockWithBiometricsEnabled</span><span class="sxs-lookup"><span data-stu-id="c5537-216">unlockWithBiometricsEnabled</span></span>|<span data-ttu-id="c5537-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5537-217">Boolean</span></span>|<span data-ttu-id="c5537-218">Steuert die Verwendung von biometrische Gesten, wie das Standardsymbol zurück und Fingerabdruck, als Alternative zu den Windows Hello für Business PIN an.</span><span class="sxs-lookup"><span data-stu-id="c5537-218">Controls the use of biometric gestures, such as face and fingerprint, as an alternative to the Windows Hello for Business PIN.</span></span>  <span data-ttu-id="c5537-219">Wenn es sich bei Festlegung auf "false", biometrische Gesten nicht zulässig sind.</span><span class="sxs-lookup"><span data-stu-id="c5537-219">If set to False, biometric gestures are not allowed.</span></span> <span data-ttu-id="c5537-220">Benutzer müssen eine PIN weiterhin als Sicherungskopie bei Fehlern konfigurieren.</span><span class="sxs-lookup"><span data-stu-id="c5537-220">Users must still configure a PIN as a backup in case of failures.</span></span>|
|<span data-ttu-id="c5537-221">useCertificatesForOnPremisesAuthEnabled</span><span class="sxs-lookup"><span data-stu-id="c5537-221">useCertificatesForOnPremisesAuthEnabled</span></span>|<span data-ttu-id="c5537-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5537-222">Boolean</span></span>|<span data-ttu-id="c5537-223">Boolescher Wert, mit der Windows Hello für Unternehmen von Zertifikaten auf Standortbasierte Ressourcen authentifizieren kann.</span><span class="sxs-lookup"><span data-stu-id="c5537-223">Boolean value that enables Windows Hello for Business to use certificates to authenticate on-premise resources.</span></span>|
|<span data-ttu-id="c5537-224">windowsHelloForBusinessBlocked</span><span class="sxs-lookup"><span data-stu-id="c5537-224">windowsHelloForBusinessBlocked</span></span>|<span data-ttu-id="c5537-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5537-225">Boolean</span></span>|<span data-ttu-id="c5537-226">Boolescher Wert, der Windows Hello für Unternehmen als Methode für die Anmeldung bei Windows blockiert.</span><span class="sxs-lookup"><span data-stu-id="c5537-226">Boolean value that blocks Windows Hello for Business as a method for signing into Windows.</span></span>|



## <a name="response"></a><span data-ttu-id="c5537-227">Antwort</span><span class="sxs-lookup"><span data-stu-id="c5537-227">Response</span></span>
<span data-ttu-id="c5537-228">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [WindowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="c5537-228">If successful, this method returns a `201 Created` response code and a [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c5537-229">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c5537-229">Example</span></span>

### <a name="request"></a><span data-ttu-id="c5537-230">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c5537-230">Request</span></span>
<span data-ttu-id="c5537-231">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c5537-231">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c5537-232">Antwort</span><span class="sxs-lookup"><span data-stu-id="c5537-232">Response</span></span>
<span data-ttu-id="c5537-p120">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c5537-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




