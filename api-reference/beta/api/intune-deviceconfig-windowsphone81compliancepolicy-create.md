---
title: windowsPhone81CompliancePolicy erstellen
description: Erstellen eines neuen windowsPhone81CompliancePolicy-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b03a56e9b4f6ab7e1df0141e85190ac2e1191767
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30149294"
---
# <a name="create-windowsphone81compliancepolicy"></a><span data-ttu-id="11483-103">windowsPhone81CompliancePolicy erstellen</span><span class="sxs-lookup"><span data-stu-id="11483-103">Create windowsPhone81CompliancePolicy</span></span>

> <span data-ttu-id="11483-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="11483-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="11483-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="11483-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="11483-106">Erstellen eines neuen [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="11483-106">Create a new [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="11483-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="11483-107">Prerequisites</span></span>
<span data-ttu-id="11483-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="11483-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="11483-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="11483-110">Permission type</span></span>|<span data-ttu-id="11483-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="11483-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="11483-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="11483-112">Delegated (work or school account)</span></span>|<span data-ttu-id="11483-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="11483-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="11483-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="11483-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="11483-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="11483-115">Not supported.</span></span>|
|<span data-ttu-id="11483-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="11483-116">Application</span></span>|<span data-ttu-id="11483-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="11483-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="11483-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="11483-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="11483-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="11483-119">Request headers</span></span>
|<span data-ttu-id="11483-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="11483-120">Header</span></span>|<span data-ttu-id="11483-121">Wert</span><span class="sxs-lookup"><span data-stu-id="11483-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="11483-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="11483-122">Authorization</span></span>|<span data-ttu-id="11483-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="11483-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="11483-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="11483-124">Accept</span></span>|<span data-ttu-id="11483-125">application/json</span><span class="sxs-lookup"><span data-stu-id="11483-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="11483-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="11483-126">Request body</span></span>
<span data-ttu-id="11483-127">Geben Sie im Anforderungstext eine JSON-Darstellung des windowsPhone81CompliancePolicy-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="11483-127">In the request body, supply a JSON representation for the windowsPhone81CompliancePolicy object.</span></span>

<span data-ttu-id="11483-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der windowsPhone81CompliancePolicy erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="11483-128">The following table shows the properties that are required when you create the windowsPhone81CompliancePolicy.</span></span>

|<span data-ttu-id="11483-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="11483-129">Property</span></span>|<span data-ttu-id="11483-130">Typ</span><span class="sxs-lookup"><span data-stu-id="11483-130">Type</span></span>|<span data-ttu-id="11483-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="11483-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="11483-132">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="11483-132">roleScopeTagIds</span></span>|<span data-ttu-id="11483-133">String collection</span><span class="sxs-lookup"><span data-stu-id="11483-133">String collection</span></span>|<span data-ttu-id="11483-134">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="11483-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="11483-135">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="11483-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="11483-136">id</span><span class="sxs-lookup"><span data-stu-id="11483-136">id</span></span>|<span data-ttu-id="11483-137">string</span><span class="sxs-lookup"><span data-stu-id="11483-137">String</span></span>|<span data-ttu-id="11483-138">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="11483-138">Key of the entity.</span></span> <span data-ttu-id="11483-139">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="11483-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="11483-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="11483-140">createdDateTime</span></span>|<span data-ttu-id="11483-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="11483-141">DateTimeOffset</span></span>|<span data-ttu-id="11483-142">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="11483-142">DateTime the object was created.</span></span> <span data-ttu-id="11483-143">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="11483-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="11483-144">description</span><span class="sxs-lookup"><span data-stu-id="11483-144">description</span></span>|<span data-ttu-id="11483-145">String</span><span class="sxs-lookup"><span data-stu-id="11483-145">String</span></span>|<span data-ttu-id="11483-146">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="11483-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="11483-147">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="11483-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="11483-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="11483-148">lastModifiedDateTime</span></span>|<span data-ttu-id="11483-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="11483-149">DateTimeOffset</span></span>|<span data-ttu-id="11483-150">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="11483-150">DateTime the object was last modified.</span></span> <span data-ttu-id="11483-151">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="11483-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="11483-152">displayName</span><span class="sxs-lookup"><span data-stu-id="11483-152">displayName</span></span>|<span data-ttu-id="11483-153">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="11483-153">String</span></span>|<span data-ttu-id="11483-154">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="11483-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="11483-155">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="11483-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="11483-156">Version</span><span class="sxs-lookup"><span data-stu-id="11483-156">version</span></span>|<span data-ttu-id="11483-157">Int32</span><span class="sxs-lookup"><span data-stu-id="11483-157">Int32</span></span>|<span data-ttu-id="11483-158">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="11483-158">Version of the device configuration.</span></span> <span data-ttu-id="11483-159">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="11483-159">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="11483-160">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="11483-160">passwordBlockSimple</span></span>|<span data-ttu-id="11483-161">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="11483-161">Boolean</span></span>|<span data-ttu-id="11483-162">Gibt an, ob die Kalendersynchronisierung blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="11483-162">Whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="11483-163">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="11483-163">passwordExpirationDays</span></span>|<span data-ttu-id="11483-164">Int32</span><span class="sxs-lookup"><span data-stu-id="11483-164">Int32</span></span>|<span data-ttu-id="11483-165">Zeit in Tagen bis zum Ablaufen des Kennworts.</span><span class="sxs-lookup"><span data-stu-id="11483-165">Number of days before the password expires.</span></span>|
|<span data-ttu-id="11483-166">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="11483-166">passwordMinimumLength</span></span>|<span data-ttu-id="11483-167">Int32</span><span class="sxs-lookup"><span data-stu-id="11483-167">Int32</span></span>|<span data-ttu-id="11483-168">Mindestlänge von Kennwörtern</span><span class="sxs-lookup"><span data-stu-id="11483-168">Minimum length of passwords.</span></span>|
|<span data-ttu-id="11483-169">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="11483-169">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="11483-170">Int32</span><span class="sxs-lookup"><span data-stu-id="11483-170">Int32</span></span>|<span data-ttu-id="11483-171">Zeitraum von Inaktivität in Minuten, nach dem die Eingabe eines Kennworts gefordert wird</span><span class="sxs-lookup"><span data-stu-id="11483-171">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="11483-172">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="11483-172">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="11483-173">Int32</span><span class="sxs-lookup"><span data-stu-id="11483-173">Int32</span></span>|<span data-ttu-id="11483-174">Anzahl der Zeichensätze, die im Kennwort enthalten sein müssen</span><span class="sxs-lookup"><span data-stu-id="11483-174">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="11483-175">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="11483-175">passwordRequiredType</span></span>|[<span data-ttu-id="11483-176">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="11483-176">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="11483-177">Geforderter Kennworttyp.</span><span class="sxs-lookup"><span data-stu-id="11483-177">The required password type.</span></span> <span data-ttu-id="11483-178">Mögliche Werte sind: `deviceDefault`, `alphanumeric` und `numeric`.</span><span class="sxs-lookup"><span data-stu-id="11483-178">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="11483-179">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="11483-179">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="11483-180">Int32</span><span class="sxs-lookup"><span data-stu-id="11483-180">Int32</span></span>|<span data-ttu-id="11483-181">Anzahl der zuletzt verwendeten Kennwörter, die nicht erneut verwendet werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="11483-181">Number of previous passwords to block.</span></span> <span data-ttu-id="11483-182">Gültige Werte: 0 bis 24.</span><span class="sxs-lookup"><span data-stu-id="11483-182">Valid values 0 to 24</span></span>|
|<span data-ttu-id="11483-183">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="11483-183">passwordRequired</span></span>|<span data-ttu-id="11483-184">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="11483-184">Boolean</span></span>|<span data-ttu-id="11483-185">Legt fest, ob ein Kennwort gefordert wird.</span><span class="sxs-lookup"><span data-stu-id="11483-185">Whether or not to require a password.</span></span>|
|<span data-ttu-id="11483-186">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="11483-186">osMinimumVersion</span></span>|<span data-ttu-id="11483-187">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="11483-187">String</span></span>|<span data-ttu-id="11483-188">Mindestversion von Windows Phone</span><span class="sxs-lookup"><span data-stu-id="11483-188">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="11483-189">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="11483-189">osMaximumVersion</span></span>|<span data-ttu-id="11483-190">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="11483-190">String</span></span>|<span data-ttu-id="11483-191">Maximalversion von Windows Phone</span><span class="sxs-lookup"><span data-stu-id="11483-191">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="11483-192">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="11483-192">storageRequireEncryption</span></span>|<span data-ttu-id="11483-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="11483-193">Boolean</span></span>|<span data-ttu-id="11483-194">Legt fest, dass auf Windows Phone-Geräten Verschlüsselung gefordert wird.</span><span class="sxs-lookup"><span data-stu-id="11483-194">Require encryption on windows phone devices.</span></span>|



## <a name="response"></a><span data-ttu-id="11483-195">Antwort</span><span class="sxs-lookup"><span data-stu-id="11483-195">Response</span></span>
<span data-ttu-id="11483-196">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="11483-196">If successful, this method returns a `201 Created` response code and a [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="11483-197">Beispiel</span><span class="sxs-lookup"><span data-stu-id="11483-197">Example</span></span>

### <a name="request"></a><span data-ttu-id="11483-198">Anforderung</span><span class="sxs-lookup"><span data-stu-id="11483-198">Request</span></span>
<span data-ttu-id="11483-199">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="11483-199">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
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

### <a name="response"></a><span data-ttu-id="11483-200">Antwort</span><span class="sxs-lookup"><span data-stu-id="11483-200">Response</span></span>
<span data-ttu-id="11483-p111">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="11483-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




