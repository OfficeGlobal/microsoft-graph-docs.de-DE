---
title: Aktualisieren von „windowsPhone81CompliancePolicy“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs windowsPhone81CompliancePolicy.
author: tfitzmac
ms.openlocfilehash: f4d17c63d7c22542b94527f508ca40ebcea28562
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27311165"
---
# <a name="update-windowsphone81compliancepolicy"></a><span data-ttu-id="8c5bd-103">Aktualisieren von „windowsPhone81CompliancePolicy“</span><span class="sxs-lookup"><span data-stu-id="8c5bd-103">Update windowsPhone81CompliancePolicy</span></span>

> <span data-ttu-id="8c5bd-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="8c5bd-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8c5bd-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8c5bd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8c5bd-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="8c5bd-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8c5bd-107">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="8c5bd-107">Update the properties of a [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8c5bd-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="8c5bd-108">Prerequisites</span></span>
<span data-ttu-id="8c5bd-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8c5bd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8c5bd-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8c5bd-111">Permission type</span></span>|<span data-ttu-id="8c5bd-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8c5bd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8c5bd-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8c5bd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8c5bd-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c5bd-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8c5bd-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8c5bd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8c5bd-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8c5bd-116">Not supported.</span></span>|
|<span data-ttu-id="8c5bd-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8c5bd-117">Application</span></span>|<span data-ttu-id="8c5bd-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8c5bd-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8c5bd-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8c5bd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="8c5bd-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8c5bd-120">Request headers</span></span>
|<span data-ttu-id="8c5bd-121">Header</span><span class="sxs-lookup"><span data-stu-id="8c5bd-121">Header</span></span>|<span data-ttu-id="8c5bd-122">Wert</span><span class="sxs-lookup"><span data-stu-id="8c5bd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8c5bd-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="8c5bd-123">Authorization</span></span>|<span data-ttu-id="8c5bd-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="8c5bd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8c5bd-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8c5bd-125">Accept</span></span>|<span data-ttu-id="8c5bd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8c5bd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8c5bd-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8c5bd-127">Request body</span></span>
<span data-ttu-id="8c5bd-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) an.</span><span class="sxs-lookup"><span data-stu-id="8c5bd-128">In the request body, supply a JSON representation for the [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object.</span></span>

<span data-ttu-id="8c5bd-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="8c5bd-129">The following table shows the properties that are required when you create the [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md).</span></span>

|<span data-ttu-id="8c5bd-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8c5bd-130">Property</span></span>|<span data-ttu-id="8c5bd-131">Typ</span><span class="sxs-lookup"><span data-stu-id="8c5bd-131">Type</span></span>|<span data-ttu-id="8c5bd-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8c5bd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8c5bd-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8c5bd-133">roleScopeTagIds</span></span>|<span data-ttu-id="8c5bd-134">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="8c5bd-134">String collection</span></span>|<span data-ttu-id="8c5bd-135">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="8c5bd-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="8c5bd-136">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="8c5bd-136">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="8c5bd-137">id</span><span class="sxs-lookup"><span data-stu-id="8c5bd-137">id</span></span>|<span data-ttu-id="8c5bd-138">String</span><span class="sxs-lookup"><span data-stu-id="8c5bd-138">String</span></span>|<span data-ttu-id="8c5bd-139">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="8c5bd-139">Key of the entity.</span></span> <span data-ttu-id="8c5bd-140">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="8c5bd-140">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="8c5bd-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8c5bd-141">createdDateTime</span></span>|<span data-ttu-id="8c5bd-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8c5bd-142">DateTimeOffset</span></span>|<span data-ttu-id="8c5bd-143">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="8c5bd-143">DateTime the object was created.</span></span> <span data-ttu-id="8c5bd-144">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="8c5bd-144">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="8c5bd-145">description</span><span class="sxs-lookup"><span data-stu-id="8c5bd-145">description</span></span>|<span data-ttu-id="8c5bd-146">String</span><span class="sxs-lookup"><span data-stu-id="8c5bd-146">String</span></span>|<span data-ttu-id="8c5bd-147">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="8c5bd-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="8c5bd-148">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="8c5bd-148">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="8c5bd-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8c5bd-149">lastModifiedDateTime</span></span>|<span data-ttu-id="8c5bd-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8c5bd-150">DateTimeOffset</span></span>|<span data-ttu-id="8c5bd-151">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="8c5bd-151">DateTime the object was last modified.</span></span> <span data-ttu-id="8c5bd-152">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="8c5bd-152">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="8c5bd-153">displayName</span><span class="sxs-lookup"><span data-stu-id="8c5bd-153">displayName</span></span>|<span data-ttu-id="8c5bd-154">String</span><span class="sxs-lookup"><span data-stu-id="8c5bd-154">String</span></span>|<span data-ttu-id="8c5bd-155">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="8c5bd-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="8c5bd-156">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="8c5bd-156">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="8c5bd-157">Version</span><span class="sxs-lookup"><span data-stu-id="8c5bd-157">version</span></span>|<span data-ttu-id="8c5bd-158">Int32</span><span class="sxs-lookup"><span data-stu-id="8c5bd-158">Int32</span></span>|<span data-ttu-id="8c5bd-159">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="8c5bd-159">Version of the device configuration.</span></span> <span data-ttu-id="8c5bd-160">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="8c5bd-160">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="8c5bd-161">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="8c5bd-161">passwordBlockSimple</span></span>|<span data-ttu-id="8c5bd-162">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="8c5bd-162">Boolean</span></span>|<span data-ttu-id="8c5bd-163">Gibt an, ob die Kalendersynchronisierung blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="8c5bd-163">Whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="8c5bd-164">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="8c5bd-164">passwordExpirationDays</span></span>|<span data-ttu-id="8c5bd-165">Int32</span><span class="sxs-lookup"><span data-stu-id="8c5bd-165">Int32</span></span>|<span data-ttu-id="8c5bd-166">Zeit in Tagen bis zum Ablaufen des Kennworts.</span><span class="sxs-lookup"><span data-stu-id="8c5bd-166">Number of days before the password expires.</span></span>|
|<span data-ttu-id="8c5bd-167">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="8c5bd-167">passwordMinimumLength</span></span>|<span data-ttu-id="8c5bd-168">Int32</span><span class="sxs-lookup"><span data-stu-id="8c5bd-168">Int32</span></span>|<span data-ttu-id="8c5bd-169">Mindestlänge von Kennwörtern</span><span class="sxs-lookup"><span data-stu-id="8c5bd-169">Minimum length of passwords.</span></span>|
|<span data-ttu-id="8c5bd-170">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="8c5bd-170">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="8c5bd-171">Int32</span><span class="sxs-lookup"><span data-stu-id="8c5bd-171">Int32</span></span>|<span data-ttu-id="8c5bd-172">Zeitraum von Inaktivität in Minuten, nach dem die Eingabe eines Kennworts gefordert wird</span><span class="sxs-lookup"><span data-stu-id="8c5bd-172">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="8c5bd-173">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="8c5bd-173">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="8c5bd-174">Int32</span><span class="sxs-lookup"><span data-stu-id="8c5bd-174">Int32</span></span>|<span data-ttu-id="8c5bd-175">Anzahl der Zeichensätze, die im Kennwort enthalten sein müssen</span><span class="sxs-lookup"><span data-stu-id="8c5bd-175">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="8c5bd-176">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="8c5bd-176">passwordRequiredType</span></span>|[<span data-ttu-id="8c5bd-177">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="8c5bd-177">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="8c5bd-178">Geforderter Kennworttyp.</span><span class="sxs-lookup"><span data-stu-id="8c5bd-178">The required password type.</span></span> <span data-ttu-id="8c5bd-179">Mögliche Werte sind: `deviceDefault`, `alphanumeric` und `numeric`.</span><span class="sxs-lookup"><span data-stu-id="8c5bd-179">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="8c5bd-180">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="8c5bd-180">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="8c5bd-181">Int32</span><span class="sxs-lookup"><span data-stu-id="8c5bd-181">Int32</span></span>|<span data-ttu-id="8c5bd-182">Anzahl der zuletzt verwendeten Kennwörter, die nicht erneut verwendet werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="8c5bd-182">Number of previous passwords to block.</span></span> <span data-ttu-id="8c5bd-183">Gültige Werte: 0 bis 24.</span><span class="sxs-lookup"><span data-stu-id="8c5bd-183">Valid values 0 to 24</span></span>|
|<span data-ttu-id="8c5bd-184">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="8c5bd-184">passwordRequired</span></span>|<span data-ttu-id="8c5bd-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="8c5bd-185">Boolean</span></span>|<span data-ttu-id="8c5bd-186">Legt fest, ob ein Kennwort gefordert wird.</span><span class="sxs-lookup"><span data-stu-id="8c5bd-186">Whether or not to require a password.</span></span>|
|<span data-ttu-id="8c5bd-187">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="8c5bd-187">osMinimumVersion</span></span>|<span data-ttu-id="8c5bd-188">String</span><span class="sxs-lookup"><span data-stu-id="8c5bd-188">String</span></span>|<span data-ttu-id="8c5bd-189">Mindestversion von Windows Phone</span><span class="sxs-lookup"><span data-stu-id="8c5bd-189">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="8c5bd-190">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="8c5bd-190">osMaximumVersion</span></span>|<span data-ttu-id="8c5bd-191">String</span><span class="sxs-lookup"><span data-stu-id="8c5bd-191">String</span></span>|<span data-ttu-id="8c5bd-192">Maximalversion von Windows Phone</span><span class="sxs-lookup"><span data-stu-id="8c5bd-192">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="8c5bd-193">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="8c5bd-193">storageRequireEncryption</span></span>|<span data-ttu-id="8c5bd-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="8c5bd-194">Boolean</span></span>|<span data-ttu-id="8c5bd-195">Legt fest, dass auf Windows Phone-Geräten Verschlüsselung gefordert wird.</span><span class="sxs-lookup"><span data-stu-id="8c5bd-195">Require encryption on windows phone devices.</span></span>|



## <a name="response"></a><span data-ttu-id="8c5bd-196">Antwort</span><span class="sxs-lookup"><span data-stu-id="8c5bd-196">Response</span></span>
<span data-ttu-id="8c5bd-197">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="8c5bd-197">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8c5bd-198">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8c5bd-198">Example</span></span>
### <a name="request"></a><span data-ttu-id="8c5bd-199">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8c5bd-199">Request</span></span>
<span data-ttu-id="8c5bd-200">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8c5bd-200">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 664

{
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
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

### <a name="response"></a><span data-ttu-id="8c5bd-201">Antwort</span><span class="sxs-lookup"><span data-stu-id="8c5bd-201">Response</span></span>
<span data-ttu-id="8c5bd-p112">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8c5bd-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





