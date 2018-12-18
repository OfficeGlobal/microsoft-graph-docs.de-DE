---
title: iosCompliancePolicy erstellen
description: Erstellen eines neuen iosCompliancePolicy-Objekts.
author: tfitzmac
ms.openlocfilehash: c1084d5b3333ef9747edfbaf2a1830b14f6a5ccd
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27355377"
---
# <a name="create-ioscompliancepolicy"></a><span data-ttu-id="bd276-103">iosCompliancePolicy erstellen</span><span class="sxs-lookup"><span data-stu-id="bd276-103">Create iosCompliancePolicy</span></span>

> <span data-ttu-id="bd276-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="bd276-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bd276-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="bd276-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bd276-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="bd276-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bd276-107">Erstellen eines neuen [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="bd276-107">Create a new [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="bd276-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="bd276-108">Prerequisites</span></span>
<span data-ttu-id="bd276-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bd276-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bd276-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="bd276-111">Permission type</span></span>|<span data-ttu-id="bd276-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="bd276-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bd276-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="bd276-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bd276-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bd276-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bd276-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="bd276-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bd276-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bd276-116">Not supported.</span></span>|
|<span data-ttu-id="bd276-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="bd276-117">Application</span></span>|<span data-ttu-id="bd276-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bd276-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bd276-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="bd276-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="bd276-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="bd276-120">Request headers</span></span>
|<span data-ttu-id="bd276-121">Header</span><span class="sxs-lookup"><span data-stu-id="bd276-121">Header</span></span>|<span data-ttu-id="bd276-122">Wert</span><span class="sxs-lookup"><span data-stu-id="bd276-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bd276-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="bd276-123">Authorization</span></span>|<span data-ttu-id="bd276-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="bd276-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bd276-125">Accept</span><span class="sxs-lookup"><span data-stu-id="bd276-125">Accept</span></span>|<span data-ttu-id="bd276-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bd276-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bd276-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="bd276-127">Request body</span></span>
<span data-ttu-id="bd276-128">Geben Sie im Anforderungstext eine JSON-Darstellung des iosCompliancePolicy-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="bd276-128">In the request body, supply a JSON representation for the iosCompliancePolicy object.</span></span>

<span data-ttu-id="bd276-129">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der iosCompliancePolicy erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="bd276-129">The following table shows the properties that are required when you create the iosCompliancePolicy.</span></span>

|<span data-ttu-id="bd276-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="bd276-130">Property</span></span>|<span data-ttu-id="bd276-131">Typ</span><span class="sxs-lookup"><span data-stu-id="bd276-131">Type</span></span>|<span data-ttu-id="bd276-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bd276-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bd276-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="bd276-133">roleScopeTagIds</span></span>|<span data-ttu-id="bd276-134">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="bd276-134">String collection</span></span>|<span data-ttu-id="bd276-135">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="bd276-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="bd276-136">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="bd276-136">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="bd276-137">id</span><span class="sxs-lookup"><span data-stu-id="bd276-137">id</span></span>|<span data-ttu-id="bd276-138">String</span><span class="sxs-lookup"><span data-stu-id="bd276-138">String</span></span>|<span data-ttu-id="bd276-139">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="bd276-139">Key of the entity.</span></span> <span data-ttu-id="bd276-140">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="bd276-140">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="bd276-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bd276-141">createdDateTime</span></span>|<span data-ttu-id="bd276-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bd276-142">DateTimeOffset</span></span>|<span data-ttu-id="bd276-143">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="bd276-143">DateTime the object was created.</span></span> <span data-ttu-id="bd276-144">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="bd276-144">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="bd276-145">description</span><span class="sxs-lookup"><span data-stu-id="bd276-145">description</span></span>|<span data-ttu-id="bd276-146">String</span><span class="sxs-lookup"><span data-stu-id="bd276-146">String</span></span>|<span data-ttu-id="bd276-147">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="bd276-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="bd276-148">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="bd276-148">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="bd276-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bd276-149">lastModifiedDateTime</span></span>|<span data-ttu-id="bd276-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bd276-150">DateTimeOffset</span></span>|<span data-ttu-id="bd276-151">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="bd276-151">DateTime the object was last modified.</span></span> <span data-ttu-id="bd276-152">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="bd276-152">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="bd276-153">displayName</span><span class="sxs-lookup"><span data-stu-id="bd276-153">displayName</span></span>|<span data-ttu-id="bd276-154">String</span><span class="sxs-lookup"><span data-stu-id="bd276-154">String</span></span>|<span data-ttu-id="bd276-155">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="bd276-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="bd276-156">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="bd276-156">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="bd276-157">Version</span><span class="sxs-lookup"><span data-stu-id="bd276-157">version</span></span>|<span data-ttu-id="bd276-158">Int32</span><span class="sxs-lookup"><span data-stu-id="bd276-158">Int32</span></span>|<span data-ttu-id="bd276-159">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="bd276-159">Version of the device configuration.</span></span> <span data-ttu-id="bd276-160">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="bd276-160">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="bd276-161">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="bd276-161">passcodeBlockSimple</span></span>|<span data-ttu-id="bd276-162">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="bd276-162">Boolean</span></span>|<span data-ttu-id="bd276-163">Gibt an, ob einfache Kennungen erlaubt sind.</span><span class="sxs-lookup"><span data-stu-id="bd276-163">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="bd276-164">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="bd276-164">passcodeExpirationDays</span></span>|<span data-ttu-id="bd276-165">Int32</span><span class="sxs-lookup"><span data-stu-id="bd276-165">Int32</span></span>|<span data-ttu-id="bd276-166">Zeit in Tagen bis zum Ablaufen der Kennung.</span><span class="sxs-lookup"><span data-stu-id="bd276-166">Number of days before the passcode expires.</span></span> <span data-ttu-id="bd276-167">Gültige Werte: 1 bis 65535.</span><span class="sxs-lookup"><span data-stu-id="bd276-167">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="bd276-168">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="bd276-168">passcodeMinimumLength</span></span>|<span data-ttu-id="bd276-169">Int32</span><span class="sxs-lookup"><span data-stu-id="bd276-169">Int32</span></span>|<span data-ttu-id="bd276-170">Mindestlänge von Kennungen.</span><span class="sxs-lookup"><span data-stu-id="bd276-170">Minimum length of passcode.</span></span> <span data-ttu-id="bd276-171">Gültige Werte: 4 bis 14.</span><span class="sxs-lookup"><span data-stu-id="bd276-171">Valid values 4 to 14</span></span>|
|<span data-ttu-id="bd276-172">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="bd276-172">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="bd276-173">Int32</span><span class="sxs-lookup"><span data-stu-id="bd276-173">Int32</span></span>|<span data-ttu-id="bd276-174">Zeitraum von Inaktivität in Minuten, bevor die Eingabe einer Kennung erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="bd276-174">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="bd276-175">passcodeMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="bd276-175">passcodeMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="bd276-176">Int32</span><span class="sxs-lookup"><span data-stu-id="bd276-176">Int32</span></span>|<span data-ttu-id="bd276-177">Zeitraum von Inaktivität in Minuten, bevor es zu einem Bildschirmtimeout kommt</span><span class="sxs-lookup"><span data-stu-id="bd276-177">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="bd276-178">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="bd276-178">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="bd276-179">Int32</span><span class="sxs-lookup"><span data-stu-id="bd276-179">Int32</span></span>|<span data-ttu-id="bd276-180">Anzahl der zuletzt verwendeten Kennungen, die nicht erneut verwendet werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="bd276-180">Number of previous passcodes to block.</span></span> <span data-ttu-id="bd276-181">Gültige Werte: 1 bis 24.</span><span class="sxs-lookup"><span data-stu-id="bd276-181">Valid values 1 to 24</span></span>|
|<span data-ttu-id="bd276-182">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="bd276-182">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="bd276-183">Int32</span><span class="sxs-lookup"><span data-stu-id="bd276-183">Int32</span></span>|<span data-ttu-id="bd276-184">Anzahl der Zeichensätze, die im Kennwort enthalten sein müssen</span><span class="sxs-lookup"><span data-stu-id="bd276-184">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="bd276-185">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="bd276-185">passcodeRequiredType</span></span>|[<span data-ttu-id="bd276-186">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="bd276-186">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="bd276-187">Der erforderliche Kennungstyp.</span><span class="sxs-lookup"><span data-stu-id="bd276-187">The required passcode type.</span></span> <span data-ttu-id="bd276-188">Mögliche Werte sind: `deviceDefault`, `alphanumeric` und `numeric`.</span><span class="sxs-lookup"><span data-stu-id="bd276-188">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="bd276-189">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="bd276-189">passcodeRequired</span></span>|<span data-ttu-id="bd276-190">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="bd276-190">Boolean</span></span>|<span data-ttu-id="bd276-191">Gibt an, ob eine Kennung erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="bd276-191">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="bd276-192">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="bd276-192">osMinimumVersion</span></span>|<span data-ttu-id="bd276-193">String</span><span class="sxs-lookup"><span data-stu-id="bd276-193">String</span></span>|<span data-ttu-id="bd276-194">Mindestversion von IOS.</span><span class="sxs-lookup"><span data-stu-id="bd276-194">Minimum IOS version.</span></span>|
|<span data-ttu-id="bd276-195">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="bd276-195">osMaximumVersion</span></span>|<span data-ttu-id="bd276-196">String</span><span class="sxs-lookup"><span data-stu-id="bd276-196">String</span></span>|<span data-ttu-id="bd276-197">Höchstversion von IOS.</span><span class="sxs-lookup"><span data-stu-id="bd276-197">Maximum IOS version.</span></span>|
|<span data-ttu-id="bd276-198">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="bd276-198">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="bd276-199">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="bd276-199">Boolean</span></span>|<span data-ttu-id="bd276-200">Legt fest, dass weder gerootete Geräte verwendet werden dürfen noch Geräte, für die ein Jailbreak durchgeführt wurde.</span><span class="sxs-lookup"><span data-stu-id="bd276-200">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="bd276-201">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="bd276-201">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="bd276-202">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="bd276-202">Boolean</span></span>|<span data-ttu-id="bd276-203">Legt fest, dass auf Geräten der Gerätebedrohungsschutz aktiviert sein muss.</span><span class="sxs-lookup"><span data-stu-id="bd276-203">Require that devices have enabled device threat protection .</span></span>|
|<span data-ttu-id="bd276-204">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="bd276-204">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="bd276-205">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="bd276-205">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="bd276-206">Legt die Mindestrisikostufe fest, ab der Mobile Threat Protection einen Konformitätsverstoß melden soll.</span><span class="sxs-lookup"><span data-stu-id="bd276-206">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="bd276-207">Mögliche Werte sind: `unavailable`, `secured`, `low`, `medium`, `high` und `notSet`.</span><span class="sxs-lookup"><span data-stu-id="bd276-207">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="bd276-208">managedEmailProfileRequired</span><span class="sxs-lookup"><span data-stu-id="bd276-208">managedEmailProfileRequired</span></span>|<span data-ttu-id="bd276-209">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="bd276-209">Boolean</span></span>|<span data-ttu-id="bd276-210">Gibt an, ob ein verwaltetes E-Mail-Profil erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="bd276-210">Indicates whether or not to require a managed email profile.</span></span>|
|<span data-ttu-id="bd276-211">restrictedApps</span><span class="sxs-lookup"><span data-stu-id="bd276-211">restrictedApps</span></span>|<span data-ttu-id="bd276-212">Collection von Objekten des Typs [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="bd276-212">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="bd276-213">Benötigen Sie das Gerät nicht die angegebenen apps installiert haben.</span><span class="sxs-lookup"><span data-stu-id="bd276-213">Require the device to not have the specified apps installed.</span></span> <span data-ttu-id="bd276-214">Diese Collection darf maximal 10.000 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="bd276-214">This collection can contain a maximum of 10000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="bd276-215">Antwort</span><span class="sxs-lookup"><span data-stu-id="bd276-215">Response</span></span>
<span data-ttu-id="bd276-216">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="bd276-216">If successful, this method returns a `201 Created` response code and a [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bd276-217">Beispiel</span><span class="sxs-lookup"><span data-stu-id="bd276-217">Example</span></span>
### <a name="request"></a><span data-ttu-id="bd276-218">Anforderung</span><span class="sxs-lookup"><span data-stu-id="bd276-218">Request</span></span>
<span data-ttu-id="bd276-219">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="bd276-219">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 1181

{
  "@odata.type": "#microsoft.graph.iosCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passcodeBlockSimple": true,
  "passcodeExpirationDays": 6,
  "passcodeMinimumLength": 5,
  "passcodeMinutesOfInactivityBeforeLock": 5,
  "passcodeMinutesOfInactivityBeforeScreenTimeout": 14,
  "passcodePreviousPasscodeBlockCount": 2,
  "passcodeMinimumCharacterSetCount": 0,
  "passcodeRequiredType": "alphanumeric",
  "passcodeRequired": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "securityBlockJailbrokenDevices": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "managedEmailProfileRequired": true,
  "restrictedApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="bd276-220">Antwort</span><span class="sxs-lookup"><span data-stu-id="bd276-220">Response</span></span>
<span data-ttu-id="bd276-p116">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="bd276-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1289

{
  "@odata.type": "#microsoft.graph.iosCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "id": "4f501351-1351-4f50-5113-504f5113504f",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passcodeBlockSimple": true,
  "passcodeExpirationDays": 6,
  "passcodeMinimumLength": 5,
  "passcodeMinutesOfInactivityBeforeLock": 5,
  "passcodeMinutesOfInactivityBeforeScreenTimeout": 14,
  "passcodePreviousPasscodeBlockCount": 2,
  "passcodeMinimumCharacterSetCount": 0,
  "passcodeRequiredType": "alphanumeric",
  "passcodeRequired": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "securityBlockJailbrokenDevices": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "managedEmailProfileRequired": true,
  "restrictedApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ]
}
```





