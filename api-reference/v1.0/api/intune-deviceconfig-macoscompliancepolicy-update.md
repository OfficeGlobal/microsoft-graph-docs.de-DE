---
title: macOSCompliancePolicy aktualisieren
description: Aktualisieren der Eigenschaften eines macOSCompliancePolicy-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 922b63ba99ae17505e36a861c6d12a4b6a195c8c
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30978192"
---
# <a name="update-macoscompliancepolicy"></a><span data-ttu-id="6c2b5-103">macOSCompliancePolicy aktualisieren</span><span class="sxs-lookup"><span data-stu-id="6c2b5-103">Update macOSCompliancePolicy</span></span>

> <span data-ttu-id="6c2b5-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="6c2b5-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6c2b5-105">Aktualisieren der Eigenschaften eines [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="6c2b5-105">Update the properties of a [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6c2b5-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="6c2b5-106">Prerequisites</span></span>
<span data-ttu-id="6c2b5-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6c2b5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6c2b5-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6c2b5-109">Permission type</span></span>|<span data-ttu-id="6c2b5-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6c2b5-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6c2b5-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6c2b5-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6c2b5-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c2b5-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6c2b5-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6c2b5-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6c2b5-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6c2b5-114">Not supported.</span></span>|
|<span data-ttu-id="6c2b5-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6c2b5-115">Application</span></span>|<span data-ttu-id="6c2b5-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6c2b5-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6c2b5-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6c2b5-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="6c2b5-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6c2b5-118">Request headers</span></span>
|<span data-ttu-id="6c2b5-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="6c2b5-119">Header</span></span>|<span data-ttu-id="6c2b5-120">Wert</span><span class="sxs-lookup"><span data-stu-id="6c2b5-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6c2b5-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="6c2b5-121">Authorization</span></span>|<span data-ttu-id="6c2b5-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="6c2b5-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6c2b5-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="6c2b5-123">Accept</span></span>|<span data-ttu-id="6c2b5-124">application/json</span><span class="sxs-lookup"><span data-stu-id="6c2b5-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6c2b5-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6c2b5-125">Request body</span></span>
<span data-ttu-id="6c2b5-126">Geben Sie im Anforderungstext eine JSON-Darstellung des [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="6c2b5-126">In the request body, supply a JSON representation for the [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object.</span></span>

<span data-ttu-id="6c2b5-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="6c2b5-127">The following table shows the properties that are required when you create the [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md).</span></span>

|<span data-ttu-id="6c2b5-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6c2b5-128">Property</span></span>|<span data-ttu-id="6c2b5-129">Typ</span><span class="sxs-lookup"><span data-stu-id="6c2b5-129">Type</span></span>|<span data-ttu-id="6c2b5-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6c2b5-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6c2b5-131">id</span><span class="sxs-lookup"><span data-stu-id="6c2b5-131">id</span></span>|<span data-ttu-id="6c2b5-132">String</span><span class="sxs-lookup"><span data-stu-id="6c2b5-132">String</span></span>|<span data-ttu-id="6c2b5-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="6c2b5-133">Key of the entity.</span></span> <span data-ttu-id="6c2b5-134">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="6c2b5-134">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6c2b5-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6c2b5-135">createdDateTime</span></span>|<span data-ttu-id="6c2b5-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6c2b5-136">DateTimeOffset</span></span>|<span data-ttu-id="6c2b5-137">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="6c2b5-137">DateTime the object was created.</span></span> <span data-ttu-id="6c2b5-138">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="6c2b5-138">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6c2b5-139">description</span><span class="sxs-lookup"><span data-stu-id="6c2b5-139">description</span></span>|<span data-ttu-id="6c2b5-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6c2b5-140">String</span></span>|<span data-ttu-id="6c2b5-141">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="6c2b5-141">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6c2b5-142">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="6c2b5-142">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6c2b5-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6c2b5-143">lastModifiedDateTime</span></span>|<span data-ttu-id="6c2b5-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6c2b5-144">DateTimeOffset</span></span>|<span data-ttu-id="6c2b5-145">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="6c2b5-145">DateTime the object was last modified.</span></span> <span data-ttu-id="6c2b5-146">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="6c2b5-146">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6c2b5-147">displayName</span><span class="sxs-lookup"><span data-stu-id="6c2b5-147">displayName</span></span>|<span data-ttu-id="6c2b5-148">String</span><span class="sxs-lookup"><span data-stu-id="6c2b5-148">String</span></span>|<span data-ttu-id="6c2b5-149">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="6c2b5-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6c2b5-150">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="6c2b5-150">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6c2b5-151">Version</span><span class="sxs-lookup"><span data-stu-id="6c2b5-151">version</span></span>|<span data-ttu-id="6c2b5-152">Int32</span><span class="sxs-lookup"><span data-stu-id="6c2b5-152">Int32</span></span>|<span data-ttu-id="6c2b5-153">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="6c2b5-153">Version of the device configuration.</span></span> <span data-ttu-id="6c2b5-154">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="6c2b5-154">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6c2b5-155">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="6c2b5-155">passwordRequired</span></span>|<span data-ttu-id="6c2b5-156">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="6c2b5-156">Boolean</span></span>|<span data-ttu-id="6c2b5-157">Legt fest, ob ein Kennwort gefordert wird.</span><span class="sxs-lookup"><span data-stu-id="6c2b5-157">Whether or not to require a password.</span></span>|
|<span data-ttu-id="6c2b5-158">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="6c2b5-158">passwordBlockSimple</span></span>|<span data-ttu-id="6c2b5-159">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="6c2b5-159">Boolean</span></span>|<span data-ttu-id="6c2b5-160">Gibt an, ob einfache Kennwörter erlaubt sind.</span><span class="sxs-lookup"><span data-stu-id="6c2b5-160">Indicates whether or not to block simple passwords.</span></span>|
|<span data-ttu-id="6c2b5-161">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="6c2b5-161">passwordExpirationDays</span></span>|<span data-ttu-id="6c2b5-162">Int32</span><span class="sxs-lookup"><span data-stu-id="6c2b5-162">Int32</span></span>|<span data-ttu-id="6c2b5-163">Zeit in Tagen bis zum Ablaufen des Kennworts</span><span class="sxs-lookup"><span data-stu-id="6c2b5-163">Number of days before the password expires.</span></span> <span data-ttu-id="6c2b5-164">Gültige Werte: 1 bis 65535.</span><span class="sxs-lookup"><span data-stu-id="6c2b5-164">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="6c2b5-165">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="6c2b5-165">passwordMinimumLength</span></span>|<span data-ttu-id="6c2b5-166">Int32</span><span class="sxs-lookup"><span data-stu-id="6c2b5-166">Int32</span></span>|<span data-ttu-id="6c2b5-167">Mindestlänge von Kennwörtern.</span><span class="sxs-lookup"><span data-stu-id="6c2b5-167">Minimum length of password.</span></span> <span data-ttu-id="6c2b5-168">Gültige Werte: 4 bis 14.</span><span class="sxs-lookup"><span data-stu-id="6c2b5-168">Valid values 4 to 14</span></span>|
|<span data-ttu-id="6c2b5-169">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="6c2b5-169">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="6c2b5-170">Int32</span><span class="sxs-lookup"><span data-stu-id="6c2b5-170">Int32</span></span>|<span data-ttu-id="6c2b5-171">Zeitraum von Inaktivität in Minuten, nach dem die Eingabe eines Kennworts gefordert wird</span><span class="sxs-lookup"><span data-stu-id="6c2b5-171">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="6c2b5-172">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="6c2b5-172">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="6c2b5-173">Int32</span><span class="sxs-lookup"><span data-stu-id="6c2b5-173">Int32</span></span>|<span data-ttu-id="6c2b5-174">Anzahl der zuletzt verwendeten Kennwörter, die nicht erneut verwendet werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="6c2b5-174">Number of previous passwords to block.</span></span> <span data-ttu-id="6c2b5-175">Gültige Werte: 1 bis 24.</span><span class="sxs-lookup"><span data-stu-id="6c2b5-175">Valid values 1 to 24</span></span>|
|<span data-ttu-id="6c2b5-176">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="6c2b5-176">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="6c2b5-177">Int32</span><span class="sxs-lookup"><span data-stu-id="6c2b5-177">Int32</span></span>|<span data-ttu-id="6c2b5-178">Anzahl der Zeichensätze, die im Kennwort enthalten sein müssen.</span><span class="sxs-lookup"><span data-stu-id="6c2b5-178">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="6c2b5-179">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="6c2b5-179">passwordRequiredType</span></span>|[<span data-ttu-id="6c2b5-180">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="6c2b5-180">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="6c2b5-181">Geforderter Kennworttyp.</span><span class="sxs-lookup"><span data-stu-id="6c2b5-181">The required password type.</span></span> <span data-ttu-id="6c2b5-182">Mögliche Werte sind: `deviceDefault`, `alphanumeric` und `numeric`.</span><span class="sxs-lookup"><span data-stu-id="6c2b5-182">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="6c2b5-183">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="6c2b5-183">osMinimumVersion</span></span>|<span data-ttu-id="6c2b5-184">String</span><span class="sxs-lookup"><span data-stu-id="6c2b5-184">String</span></span>|<span data-ttu-id="6c2b5-185">Mindestens MacOS-Version.</span><span class="sxs-lookup"><span data-stu-id="6c2b5-185">Minimum MacOS version.</span></span>|
|<span data-ttu-id="6c2b5-186">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="6c2b5-186">osMaximumVersion</span></span>|<span data-ttu-id="6c2b5-187">String</span><span class="sxs-lookup"><span data-stu-id="6c2b5-187">String</span></span>|<span data-ttu-id="6c2b5-188">Maximale MacOS-Version.</span><span class="sxs-lookup"><span data-stu-id="6c2b5-188">Maximum MacOS version.</span></span>|
|<span data-ttu-id="6c2b5-189">systemIntegrityProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="6c2b5-189">systemIntegrityProtectionEnabled</span></span>|<span data-ttu-id="6c2b5-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="6c2b5-190">Boolean</span></span>|<span data-ttu-id="6c2b5-191">Gibt an, ob auf Geräten der Systemintegritätsschutz aktiviert sein muss.</span><span class="sxs-lookup"><span data-stu-id="6c2b5-191">Require that devices have enabled system integrity protection.</span></span>|
|<span data-ttu-id="6c2b5-192">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="6c2b5-192">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="6c2b5-193">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="6c2b5-193">Boolean</span></span>|<span data-ttu-id="6c2b5-194">Legt fest, dass auf Geräten der Gerätebedrohungsschutz aktiviert sein muss.</span><span class="sxs-lookup"><span data-stu-id="6c2b5-194">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="6c2b5-195">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="6c2b5-195">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="6c2b5-196">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="6c2b5-196">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="6c2b5-197">Legt die Mindestrisikostufe fest, ab der Mobile Threat Protection einen Konformitätsverstoß melden soll.</span><span class="sxs-lookup"><span data-stu-id="6c2b5-197">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="6c2b5-198">Mögliche Werte sind: `unavailable`, `secured`, `low`, `medium`, `high` und `notSet`.</span><span class="sxs-lookup"><span data-stu-id="6c2b5-198">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="6c2b5-199">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="6c2b5-199">storageRequireEncryption</span></span>|<span data-ttu-id="6c2b5-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="6c2b5-200">Boolean</span></span>|<span data-ttu-id="6c2b5-201">Gibt an, ob auf Mac OS-Geräten die Verschlüsselung erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="6c2b5-201">Require encryption on Mac OS devices.</span></span>|
|<span data-ttu-id="6c2b5-202">firewallEnabled</span><span class="sxs-lookup"><span data-stu-id="6c2b5-202">firewallEnabled</span></span>|<span data-ttu-id="6c2b5-203">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="6c2b5-203">Boolean</span></span>|<span data-ttu-id="6c2b5-204">Ob die Firewall aktiviert werden soll oder nicht.</span><span class="sxs-lookup"><span data-stu-id="6c2b5-204">Whether the firewall should be enabled or not.</span></span>|
|<span data-ttu-id="6c2b5-205">firewallBlockAllIncoming</span><span class="sxs-lookup"><span data-stu-id="6c2b5-205">firewallBlockAllIncoming</span></span>|<span data-ttu-id="6c2b5-206">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="6c2b5-206">Boolean</span></span>|<span data-ttu-id="6c2b5-207">Entspricht der Option "alle eingehenden Verbindungen blockieren".</span><span class="sxs-lookup"><span data-stu-id="6c2b5-207">Corresponds to the “Block all incoming connections” option.</span></span>|
|<span data-ttu-id="6c2b5-208">firewallEnableStealthMode</span><span class="sxs-lookup"><span data-stu-id="6c2b5-208">firewallEnableStealthMode</span></span>|<span data-ttu-id="6c2b5-209">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="6c2b5-209">Boolean</span></span>|<span data-ttu-id="6c2b5-210">Entspricht "Stealth-Modus aktivieren".</span><span class="sxs-lookup"><span data-stu-id="6c2b5-210">Corresponds to “Enable stealth mode.”</span></span>|



## <a name="response"></a><span data-ttu-id="6c2b5-211">Antwort</span><span class="sxs-lookup"><span data-stu-id="6c2b5-211">Response</span></span>
<span data-ttu-id="6c2b5-212">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="6c2b5-212">If successful, this method returns a `200 OK` response code and an updated [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6c2b5-213">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6c2b5-213">Example</span></span>

### <a name="request"></a><span data-ttu-id="6c2b5-214">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6c2b5-214">Request</span></span>
<span data-ttu-id="6c2b5-215">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6c2b5-215">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 849

{
  "@odata.type": "#microsoft.graph.macOSCompliancePolicy",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "systemIntegrityProtectionEnabled": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "storageRequireEncryption": true,
  "firewallEnabled": true,
  "firewallBlockAllIncoming": true,
  "firewallEnableStealthMode": true
}
```

### <a name="response"></a><span data-ttu-id="6c2b5-216">Antwort</span><span class="sxs-lookup"><span data-stu-id="6c2b5-216">Response</span></span>
<span data-ttu-id="6c2b5-p113">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6c2b5-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1021

{
  "@odata.type": "#microsoft.graph.macOSCompliancePolicy",
  "id": "ddbadff3-dff3-ddba-f3df-baddf3dfbadd",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "systemIntegrityProtectionEnabled": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "storageRequireEncryption": true,
  "firewallEnabled": true,
  "firewallBlockAllIncoming": true,
  "firewallEnableStealthMode": true
}
```



