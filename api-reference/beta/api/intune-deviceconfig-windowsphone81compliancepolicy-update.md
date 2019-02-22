---
title: Aktualisieren von „windowsPhone81CompliancePolicy“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs windowsPhone81CompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1b2b9d1fb0e661e16d8ae377a8674cfe1bbc482b
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30147670"
---
# <a name="update-windowsphone81compliancepolicy"></a><span data-ttu-id="19965-103">Aktualisieren von „windowsPhone81CompliancePolicy“</span><span class="sxs-lookup"><span data-stu-id="19965-103">Update windowsPhone81CompliancePolicy</span></span>

> <span data-ttu-id="19965-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="19965-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="19965-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="19965-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="19965-106">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="19965-106">Update the properties of a [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="19965-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="19965-107">Prerequisites</span></span>
<span data-ttu-id="19965-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="19965-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="19965-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="19965-110">Permission type</span></span>|<span data-ttu-id="19965-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="19965-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="19965-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="19965-112">Delegated (work or school account)</span></span>|<span data-ttu-id="19965-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="19965-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="19965-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="19965-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="19965-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="19965-115">Not supported.</span></span>|
|<span data-ttu-id="19965-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="19965-116">Application</span></span>|<span data-ttu-id="19965-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="19965-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="19965-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="19965-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="19965-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="19965-119">Request headers</span></span>
|<span data-ttu-id="19965-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="19965-120">Header</span></span>|<span data-ttu-id="19965-121">Wert</span><span class="sxs-lookup"><span data-stu-id="19965-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="19965-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="19965-122">Authorization</span></span>|<span data-ttu-id="19965-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="19965-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="19965-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="19965-124">Accept</span></span>|<span data-ttu-id="19965-125">application/json</span><span class="sxs-lookup"><span data-stu-id="19965-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="19965-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="19965-126">Request body</span></span>
<span data-ttu-id="19965-127">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) an.</span><span class="sxs-lookup"><span data-stu-id="19965-127">In the request body, supply a JSON representation for the [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object.</span></span>

<span data-ttu-id="19965-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="19965-128">The following table shows the properties that are required when you create the [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md).</span></span>

|<span data-ttu-id="19965-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="19965-129">Property</span></span>|<span data-ttu-id="19965-130">Typ</span><span class="sxs-lookup"><span data-stu-id="19965-130">Type</span></span>|<span data-ttu-id="19965-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="19965-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="19965-132">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="19965-132">roleScopeTagIds</span></span>|<span data-ttu-id="19965-133">String collection</span><span class="sxs-lookup"><span data-stu-id="19965-133">String collection</span></span>|<span data-ttu-id="19965-134">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="19965-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="19965-135">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="19965-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="19965-136">id</span><span class="sxs-lookup"><span data-stu-id="19965-136">id</span></span>|<span data-ttu-id="19965-137">string</span><span class="sxs-lookup"><span data-stu-id="19965-137">String</span></span>|<span data-ttu-id="19965-138">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="19965-138">Key of the entity.</span></span> <span data-ttu-id="19965-139">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="19965-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="19965-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="19965-140">createdDateTime</span></span>|<span data-ttu-id="19965-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="19965-141">DateTimeOffset</span></span>|<span data-ttu-id="19965-142">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="19965-142">DateTime the object was created.</span></span> <span data-ttu-id="19965-143">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="19965-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="19965-144">description</span><span class="sxs-lookup"><span data-stu-id="19965-144">description</span></span>|<span data-ttu-id="19965-145">String</span><span class="sxs-lookup"><span data-stu-id="19965-145">String</span></span>|<span data-ttu-id="19965-146">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="19965-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="19965-147">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="19965-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="19965-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="19965-148">lastModifiedDateTime</span></span>|<span data-ttu-id="19965-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="19965-149">DateTimeOffset</span></span>|<span data-ttu-id="19965-150">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="19965-150">DateTime the object was last modified.</span></span> <span data-ttu-id="19965-151">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="19965-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="19965-152">displayName</span><span class="sxs-lookup"><span data-stu-id="19965-152">displayName</span></span>|<span data-ttu-id="19965-153">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="19965-153">String</span></span>|<span data-ttu-id="19965-154">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="19965-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="19965-155">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="19965-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="19965-156">Version</span><span class="sxs-lookup"><span data-stu-id="19965-156">version</span></span>|<span data-ttu-id="19965-157">Int32</span><span class="sxs-lookup"><span data-stu-id="19965-157">Int32</span></span>|<span data-ttu-id="19965-158">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="19965-158">Version of the device configuration.</span></span> <span data-ttu-id="19965-159">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="19965-159">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="19965-160">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="19965-160">passwordBlockSimple</span></span>|<span data-ttu-id="19965-161">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="19965-161">Boolean</span></span>|<span data-ttu-id="19965-162">Gibt an, ob die Kalendersynchronisierung blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="19965-162">Whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="19965-163">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="19965-163">passwordExpirationDays</span></span>|<span data-ttu-id="19965-164">Int32</span><span class="sxs-lookup"><span data-stu-id="19965-164">Int32</span></span>|<span data-ttu-id="19965-165">Zeit in Tagen bis zum Ablaufen des Kennworts.</span><span class="sxs-lookup"><span data-stu-id="19965-165">Number of days before the password expires.</span></span>|
|<span data-ttu-id="19965-166">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="19965-166">passwordMinimumLength</span></span>|<span data-ttu-id="19965-167">Int32</span><span class="sxs-lookup"><span data-stu-id="19965-167">Int32</span></span>|<span data-ttu-id="19965-168">Mindestlänge von Kennwörtern</span><span class="sxs-lookup"><span data-stu-id="19965-168">Minimum length of passwords.</span></span>|
|<span data-ttu-id="19965-169">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="19965-169">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="19965-170">Int32</span><span class="sxs-lookup"><span data-stu-id="19965-170">Int32</span></span>|<span data-ttu-id="19965-171">Zeitraum von Inaktivität in Minuten, nach dem die Eingabe eines Kennworts gefordert wird</span><span class="sxs-lookup"><span data-stu-id="19965-171">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="19965-172">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="19965-172">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="19965-173">Int32</span><span class="sxs-lookup"><span data-stu-id="19965-173">Int32</span></span>|<span data-ttu-id="19965-174">Anzahl der Zeichensätze, die im Kennwort enthalten sein müssen</span><span class="sxs-lookup"><span data-stu-id="19965-174">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="19965-175">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="19965-175">passwordRequiredType</span></span>|[<span data-ttu-id="19965-176">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="19965-176">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="19965-177">Geforderter Kennworttyp.</span><span class="sxs-lookup"><span data-stu-id="19965-177">The required password type.</span></span> <span data-ttu-id="19965-178">Mögliche Werte sind: `deviceDefault`, `alphanumeric` und `numeric`.</span><span class="sxs-lookup"><span data-stu-id="19965-178">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="19965-179">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="19965-179">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="19965-180">Int32</span><span class="sxs-lookup"><span data-stu-id="19965-180">Int32</span></span>|<span data-ttu-id="19965-181">Anzahl der zuletzt verwendeten Kennwörter, die nicht erneut verwendet werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="19965-181">Number of previous passwords to block.</span></span> <span data-ttu-id="19965-182">Gültige Werte: 0 bis 24.</span><span class="sxs-lookup"><span data-stu-id="19965-182">Valid values 0 to 24</span></span>|
|<span data-ttu-id="19965-183">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="19965-183">passwordRequired</span></span>|<span data-ttu-id="19965-184">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="19965-184">Boolean</span></span>|<span data-ttu-id="19965-185">Legt fest, ob ein Kennwort gefordert wird.</span><span class="sxs-lookup"><span data-stu-id="19965-185">Whether or not to require a password.</span></span>|
|<span data-ttu-id="19965-186">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="19965-186">osMinimumVersion</span></span>|<span data-ttu-id="19965-187">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="19965-187">String</span></span>|<span data-ttu-id="19965-188">Mindestversion von Windows Phone</span><span class="sxs-lookup"><span data-stu-id="19965-188">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="19965-189">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="19965-189">osMaximumVersion</span></span>|<span data-ttu-id="19965-190">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="19965-190">String</span></span>|<span data-ttu-id="19965-191">Maximalversion von Windows Phone</span><span class="sxs-lookup"><span data-stu-id="19965-191">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="19965-192">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="19965-192">storageRequireEncryption</span></span>|<span data-ttu-id="19965-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="19965-193">Boolean</span></span>|<span data-ttu-id="19965-194">Legt fest, dass auf Windows Phone-Geräten Verschlüsselung gefordert wird.</span><span class="sxs-lookup"><span data-stu-id="19965-194">Require encryption on windows phone devices.</span></span>|



## <a name="response"></a><span data-ttu-id="19965-195">Antwort</span><span class="sxs-lookup"><span data-stu-id="19965-195">Response</span></span>
<span data-ttu-id="19965-196">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="19965-196">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="19965-197">Beispiel</span><span class="sxs-lookup"><span data-stu-id="19965-197">Example</span></span>

### <a name="request"></a><span data-ttu-id="19965-198">Anforderung</span><span class="sxs-lookup"><span data-stu-id="19965-198">Request</span></span>
<span data-ttu-id="19965-199">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="19965-199">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 669

{
  "@odata.type": "#microsoft.graph.windowsPhone81CompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequired": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "storageRequireEncryption": true
}
```

### <a name="response"></a><span data-ttu-id="19965-200">Antwort</span><span class="sxs-lookup"><span data-stu-id="19965-200">Response</span></span>
<span data-ttu-id="19965-p111">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="19965-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 841

{
  "@odata.type": "#microsoft.graph.windowsPhone81CompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "id": "e6021ad4-1ad4-e602-d41a-02e6d41a02e6",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequired": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "storageRequireEncryption": true
}
```




