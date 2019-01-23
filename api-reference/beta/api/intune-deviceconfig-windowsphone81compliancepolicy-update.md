---
title: Aktualisieren von „windowsPhone81CompliancePolicy“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs windowsPhone81CompliancePolicy.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 190bdcabd7662295c3c02a8fadac48d9ec966ba0
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425575"
---
# <a name="update-windowsphone81compliancepolicy"></a><span data-ttu-id="7c351-103">Aktualisieren von „windowsPhone81CompliancePolicy“</span><span class="sxs-lookup"><span data-stu-id="7c351-103">Update windowsPhone81CompliancePolicy</span></span>

> <span data-ttu-id="7c351-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="7c351-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="7c351-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7c351-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7c351-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="7c351-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7c351-107">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="7c351-107">Update the properties of a [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7c351-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="7c351-108">Prerequisites</span></span>
<span data-ttu-id="7c351-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="7c351-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="7c351-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7c351-111">Permission type</span></span>|<span data-ttu-id="7c351-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7c351-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7c351-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7c351-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7c351-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c351-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7c351-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7c351-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7c351-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7c351-116">Not supported.</span></span>|
|<span data-ttu-id="7c351-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7c351-117">Application</span></span>|<span data-ttu-id="7c351-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7c351-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7c351-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7c351-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="7c351-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7c351-120">Request headers</span></span>
|<span data-ttu-id="7c351-121">Header</span><span class="sxs-lookup"><span data-stu-id="7c351-121">Header</span></span>|<span data-ttu-id="7c351-122">Wert</span><span class="sxs-lookup"><span data-stu-id="7c351-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7c351-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="7c351-123">Authorization</span></span>|<span data-ttu-id="7c351-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="7c351-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7c351-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="7c351-125">Accept</span></span>|<span data-ttu-id="7c351-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7c351-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7c351-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7c351-127">Request body</span></span>
<span data-ttu-id="7c351-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) an.</span><span class="sxs-lookup"><span data-stu-id="7c351-128">In the request body, supply a JSON representation for the [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object.</span></span>

<span data-ttu-id="7c351-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="7c351-129">The following table shows the properties that are required when you create the [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md).</span></span>

|<span data-ttu-id="7c351-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7c351-130">Property</span></span>|<span data-ttu-id="7c351-131">Typ</span><span class="sxs-lookup"><span data-stu-id="7c351-131">Type</span></span>|<span data-ttu-id="7c351-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7c351-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7c351-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="7c351-133">roleScopeTagIds</span></span>|<span data-ttu-id="7c351-134">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="7c351-134">String collection</span></span>|<span data-ttu-id="7c351-135">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="7c351-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="7c351-136">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="7c351-136">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="7c351-137">id</span><span class="sxs-lookup"><span data-stu-id="7c351-137">id</span></span>|<span data-ttu-id="7c351-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7c351-138">String</span></span>|<span data-ttu-id="7c351-139">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="7c351-139">Key of the entity.</span></span> <span data-ttu-id="7c351-140">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="7c351-140">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="7c351-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7c351-141">createdDateTime</span></span>|<span data-ttu-id="7c351-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7c351-142">DateTimeOffset</span></span>|<span data-ttu-id="7c351-143">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="7c351-143">DateTime the object was created.</span></span> <span data-ttu-id="7c351-144">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="7c351-144">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="7c351-145">description</span><span class="sxs-lookup"><span data-stu-id="7c351-145">description</span></span>|<span data-ttu-id="7c351-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7c351-146">String</span></span>|<span data-ttu-id="7c351-147">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="7c351-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="7c351-148">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="7c351-148">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="7c351-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7c351-149">lastModifiedDateTime</span></span>|<span data-ttu-id="7c351-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7c351-150">DateTimeOffset</span></span>|<span data-ttu-id="7c351-151">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="7c351-151">DateTime the object was last modified.</span></span> <span data-ttu-id="7c351-152">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="7c351-152">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="7c351-153">displayName</span><span class="sxs-lookup"><span data-stu-id="7c351-153">displayName</span></span>|<span data-ttu-id="7c351-154">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7c351-154">String</span></span>|<span data-ttu-id="7c351-155">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="7c351-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="7c351-156">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="7c351-156">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="7c351-157">Version</span><span class="sxs-lookup"><span data-stu-id="7c351-157">version</span></span>|<span data-ttu-id="7c351-158">Int32</span><span class="sxs-lookup"><span data-stu-id="7c351-158">Int32</span></span>|<span data-ttu-id="7c351-159">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="7c351-159">Version of the device configuration.</span></span> <span data-ttu-id="7c351-160">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="7c351-160">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="7c351-161">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="7c351-161">passwordBlockSimple</span></span>|<span data-ttu-id="7c351-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="7c351-162">Boolean</span></span>|<span data-ttu-id="7c351-163">Gibt an, ob die Kalendersynchronisierung blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="7c351-163">Whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="7c351-164">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="7c351-164">passwordExpirationDays</span></span>|<span data-ttu-id="7c351-165">Int32</span><span class="sxs-lookup"><span data-stu-id="7c351-165">Int32</span></span>|<span data-ttu-id="7c351-166">Zeit in Tagen bis zum Ablaufen des Kennworts.</span><span class="sxs-lookup"><span data-stu-id="7c351-166">Number of days before the password expires.</span></span>|
|<span data-ttu-id="7c351-167">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="7c351-167">passwordMinimumLength</span></span>|<span data-ttu-id="7c351-168">Int32</span><span class="sxs-lookup"><span data-stu-id="7c351-168">Int32</span></span>|<span data-ttu-id="7c351-169">Mindestlänge von Kennwörtern</span><span class="sxs-lookup"><span data-stu-id="7c351-169">Minimum length of passwords.</span></span>|
|<span data-ttu-id="7c351-170">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="7c351-170">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="7c351-171">Int32</span><span class="sxs-lookup"><span data-stu-id="7c351-171">Int32</span></span>|<span data-ttu-id="7c351-172">Zeitraum von Inaktivität in Minuten, nach dem die Eingabe eines Kennworts gefordert wird</span><span class="sxs-lookup"><span data-stu-id="7c351-172">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="7c351-173">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="7c351-173">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="7c351-174">Int32</span><span class="sxs-lookup"><span data-stu-id="7c351-174">Int32</span></span>|<span data-ttu-id="7c351-175">Anzahl der Zeichensätze, die im Kennwort enthalten sein müssen</span><span class="sxs-lookup"><span data-stu-id="7c351-175">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="7c351-176">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="7c351-176">passwordRequiredType</span></span>|[<span data-ttu-id="7c351-177">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="7c351-177">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="7c351-178">Geforderter Kennworttyp.</span><span class="sxs-lookup"><span data-stu-id="7c351-178">The required password type.</span></span> <span data-ttu-id="7c351-179">Mögliche Werte sind: `deviceDefault`, `alphanumeric` und `numeric`.</span><span class="sxs-lookup"><span data-stu-id="7c351-179">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="7c351-180">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="7c351-180">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="7c351-181">Int32</span><span class="sxs-lookup"><span data-stu-id="7c351-181">Int32</span></span>|<span data-ttu-id="7c351-182">Anzahl der zuletzt verwendeten Kennwörter, die nicht erneut verwendet werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="7c351-182">Number of previous passwords to block.</span></span> <span data-ttu-id="7c351-183">Gültige Werte: 0 bis 24.</span><span class="sxs-lookup"><span data-stu-id="7c351-183">Valid values 0 to 24</span></span>|
|<span data-ttu-id="7c351-184">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="7c351-184">passwordRequired</span></span>|<span data-ttu-id="7c351-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="7c351-185">Boolean</span></span>|<span data-ttu-id="7c351-186">Legt fest, ob ein Kennwort gefordert wird.</span><span class="sxs-lookup"><span data-stu-id="7c351-186">Whether or not to require a password.</span></span>|
|<span data-ttu-id="7c351-187">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="7c351-187">osMinimumVersion</span></span>|<span data-ttu-id="7c351-188">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7c351-188">String</span></span>|<span data-ttu-id="7c351-189">Mindestversion von Windows Phone</span><span class="sxs-lookup"><span data-stu-id="7c351-189">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="7c351-190">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="7c351-190">osMaximumVersion</span></span>|<span data-ttu-id="7c351-191">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7c351-191">String</span></span>|<span data-ttu-id="7c351-192">Maximalversion von Windows Phone</span><span class="sxs-lookup"><span data-stu-id="7c351-192">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="7c351-193">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="7c351-193">storageRequireEncryption</span></span>|<span data-ttu-id="7c351-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="7c351-194">Boolean</span></span>|<span data-ttu-id="7c351-195">Legt fest, dass auf Windows Phone-Geräten Verschlüsselung gefordert wird.</span><span class="sxs-lookup"><span data-stu-id="7c351-195">Require encryption on windows phone devices.</span></span>|



## <a name="response"></a><span data-ttu-id="7c351-196">Antwort</span><span class="sxs-lookup"><span data-stu-id="7c351-196">Response</span></span>
<span data-ttu-id="7c351-197">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="7c351-197">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7c351-198">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7c351-198">Example</span></span>

### <a name="request"></a><span data-ttu-id="7c351-199">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7c351-199">Request</span></span>
<span data-ttu-id="7c351-200">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7c351-200">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7c351-201">Antwort</span><span class="sxs-lookup"><span data-stu-id="7c351-201">Response</span></span>
<span data-ttu-id="7c351-p112">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7c351-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




