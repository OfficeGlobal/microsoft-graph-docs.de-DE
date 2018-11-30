---
title: Erstellen von „windows81CompliancePolicy“
description: Diese Methode erstellt ein neues Objekt des Typs windows81CompliancePolicy.
ms.openlocfilehash: a2e82d6040941365d5a5b03b2aa648f819d8b80c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017228"
---
# <a name="create-windows81compliancepolicy"></a><span data-ttu-id="e1ae5-103">Erstellen von „windows81CompliancePolicy“</span><span class="sxs-lookup"><span data-stu-id="e1ae5-103">Create windows81CompliancePolicy</span></span>

> <span data-ttu-id="e1ae5-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="e1ae5-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e1ae5-105">Diese Methode erstellt ein neues Objekt des Typs [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e1ae5-105">Create a new [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e1ae5-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="e1ae5-106">Prerequisites</span></span>
<span data-ttu-id="e1ae5-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e1ae5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e1ae5-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e1ae5-109">Permission type</span></span>|<span data-ttu-id="e1ae5-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e1ae5-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e1ae5-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e1ae5-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e1ae5-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1ae5-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e1ae5-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e1ae5-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e1ae5-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e1ae5-114">Not supported.</span></span>|
|<span data-ttu-id="e1ae5-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e1ae5-115">Application</span></span>|<span data-ttu-id="e1ae5-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e1ae5-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e1ae5-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e1ae5-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="e1ae5-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e1ae5-118">Request headers</span></span>
|<span data-ttu-id="e1ae5-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="e1ae5-119">Header</span></span>|<span data-ttu-id="e1ae5-120">Wert</span><span class="sxs-lookup"><span data-stu-id="e1ae5-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e1ae5-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e1ae5-121">Authorization</span></span>|<span data-ttu-id="e1ae5-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="e1ae5-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e1ae5-123">Accept</span><span class="sxs-lookup"><span data-stu-id="e1ae5-123">Accept</span></span>|<span data-ttu-id="e1ae5-124">application/json</span><span class="sxs-lookup"><span data-stu-id="e1ae5-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e1ae5-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e1ae5-125">Request body</span></span>
<span data-ttu-id="e1ae5-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „windows81CompliancePolicy“ an.</span><span class="sxs-lookup"><span data-stu-id="e1ae5-126">In the request body, supply a JSON representation for the windows81CompliancePolicy object.</span></span>

<span data-ttu-id="e1ae5-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „windows81CompliancePolicy“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="e1ae5-127">The following table shows the properties that are required when you create the windows81CompliancePolicy.</span></span>

|<span data-ttu-id="e1ae5-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e1ae5-128">Property</span></span>|<span data-ttu-id="e1ae5-129">Typ</span><span class="sxs-lookup"><span data-stu-id="e1ae5-129">Type</span></span>|<span data-ttu-id="e1ae5-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e1ae5-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e1ae5-131">id</span><span class="sxs-lookup"><span data-stu-id="e1ae5-131">id</span></span>|<span data-ttu-id="e1ae5-132">String</span><span class="sxs-lookup"><span data-stu-id="e1ae5-132">String</span></span>|<span data-ttu-id="e1ae5-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="e1ae5-133">Key of the entity.</span></span> <span data-ttu-id="e1ae5-134">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e1ae5-134">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e1ae5-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e1ae5-135">createdDateTime</span></span>|<span data-ttu-id="e1ae5-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e1ae5-136">DateTimeOffset</span></span>|<span data-ttu-id="e1ae5-137">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="e1ae5-137">DateTime the object was created.</span></span> <span data-ttu-id="e1ae5-138">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e1ae5-138">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e1ae5-139">description</span><span class="sxs-lookup"><span data-stu-id="e1ae5-139">description</span></span>|<span data-ttu-id="e1ae5-140">String</span><span class="sxs-lookup"><span data-stu-id="e1ae5-140">String</span></span>|<span data-ttu-id="e1ae5-141">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="e1ae5-141">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e1ae5-142">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e1ae5-142">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e1ae5-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e1ae5-143">lastModifiedDateTime</span></span>|<span data-ttu-id="e1ae5-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e1ae5-144">DateTimeOffset</span></span>|<span data-ttu-id="e1ae5-145">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="e1ae5-145">DateTime the object was last modified.</span></span> <span data-ttu-id="e1ae5-146">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e1ae5-146">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e1ae5-147">displayName</span><span class="sxs-lookup"><span data-stu-id="e1ae5-147">displayName</span></span>|<span data-ttu-id="e1ae5-148">String</span><span class="sxs-lookup"><span data-stu-id="e1ae5-148">String</span></span>|<span data-ttu-id="e1ae5-149">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="e1ae5-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e1ae5-150">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e1ae5-150">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e1ae5-151">Version</span><span class="sxs-lookup"><span data-stu-id="e1ae5-151">version</span></span>|<span data-ttu-id="e1ae5-152">Int32</span><span class="sxs-lookup"><span data-stu-id="e1ae5-152">Int32</span></span>|<span data-ttu-id="e1ae5-153">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="e1ae5-153">Version of the device configuration.</span></span> <span data-ttu-id="e1ae5-154">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e1ae5-154">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e1ae5-155">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="e1ae5-155">passwordRequired</span></span>|<span data-ttu-id="e1ae5-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="e1ae5-156">Boolean</span></span>|<span data-ttu-id="e1ae5-157">Legt fest, dass zum Entsperren des Windows-Geräts ein Kennwort erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="e1ae5-157">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="e1ae5-158">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="e1ae5-158">passwordBlockSimple</span></span>|<span data-ttu-id="e1ae5-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="e1ae5-159">Boolean</span></span>|<span data-ttu-id="e1ae5-160">Gibt an, ob einfache Kennwörter erlaubt sind.</span><span class="sxs-lookup"><span data-stu-id="e1ae5-160">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="e1ae5-161">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="e1ae5-161">passwordExpirationDays</span></span>|<span data-ttu-id="e1ae5-162">Int32</span><span class="sxs-lookup"><span data-stu-id="e1ae5-162">Int32</span></span>|<span data-ttu-id="e1ae5-163">Zeit bis zum Ablaufen des Kennworts in Tagen</span><span class="sxs-lookup"><span data-stu-id="e1ae5-163">Password expiration in days.</span></span>|
|<span data-ttu-id="e1ae5-164">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="e1ae5-164">passwordMinimumLength</span></span>|<span data-ttu-id="e1ae5-165">Int32</span><span class="sxs-lookup"><span data-stu-id="e1ae5-165">Int32</span></span>|<span data-ttu-id="e1ae5-166">Mindestlänge des Kennworts</span><span class="sxs-lookup"><span data-stu-id="e1ae5-166">The minimum password length.</span></span>|
|<span data-ttu-id="e1ae5-167">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="e1ae5-167">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="e1ae5-168">Int32</span><span class="sxs-lookup"><span data-stu-id="e1ae5-168">Int32</span></span>|<span data-ttu-id="e1ae5-169">Zeitraum von Inaktivität in Minuten, nach dem die Eingabe eines Kennworts gefordert wird</span><span class="sxs-lookup"><span data-stu-id="e1ae5-169">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="e1ae5-170">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="e1ae5-170">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="e1ae5-171">Int32</span><span class="sxs-lookup"><span data-stu-id="e1ae5-171">Int32</span></span>|<span data-ttu-id="e1ae5-172">Anzahl der Zeichensätze, die im Kennwort enthalten sein müssen</span><span class="sxs-lookup"><span data-stu-id="e1ae5-172">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="e1ae5-173">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="e1ae5-173">passwordRequiredType</span></span>|[<span data-ttu-id="e1ae5-174">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="e1ae5-174">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="e1ae5-175">Geforderter Kennworttyp.</span><span class="sxs-lookup"><span data-stu-id="e1ae5-175">The required password type.</span></span> <span data-ttu-id="e1ae5-176">Mögliche Werte sind: `deviceDefault`, `alphanumeric` und `numeric`.</span><span class="sxs-lookup"><span data-stu-id="e1ae5-176">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="e1ae5-177">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="e1ae5-177">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="e1ae5-178">Int32</span><span class="sxs-lookup"><span data-stu-id="e1ae5-178">Int32</span></span>|<span data-ttu-id="e1ae5-179">Grenze für die Wiederverwendung von Kennwörtern. Der festgelegte Wert gibt an, von wie vielen der zuletzt genutzten Kennwörter sich das Kennwort unterscheiden muss.</span><span class="sxs-lookup"><span data-stu-id="e1ae5-179">The number of previous passwords to prevent re-use of.</span></span> <span data-ttu-id="e1ae5-180">Gültige Werte: 0 bis 24.</span><span class="sxs-lookup"><span data-stu-id="e1ae5-180">Valid values 0 to 24</span></span>|
|<span data-ttu-id="e1ae5-181">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="e1ae5-181">osMinimumVersion</span></span>|<span data-ttu-id="e1ae5-182">String</span><span class="sxs-lookup"><span data-stu-id="e1ae5-182">String</span></span>|<span data-ttu-id="e1ae5-183">Mindestversion von Windows 8.1</span><span class="sxs-lookup"><span data-stu-id="e1ae5-183">Minimum Windows 8.1 version.</span></span>|
|<span data-ttu-id="e1ae5-184">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="e1ae5-184">osMaximumVersion</span></span>|<span data-ttu-id="e1ae5-185">String</span><span class="sxs-lookup"><span data-stu-id="e1ae5-185">String</span></span>|<span data-ttu-id="e1ae5-186">Maximalversion von Windows 8.1</span><span class="sxs-lookup"><span data-stu-id="e1ae5-186">Maximum Windows 8.1 version.</span></span>|
|<span data-ttu-id="e1ae5-187">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="e1ae5-187">storageRequireEncryption</span></span>|<span data-ttu-id="e1ae5-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="e1ae5-188">Boolean</span></span>|<span data-ttu-id="e1ae5-189">Gibt an, ob für ein Windows 8.1-Gerät Verschlüsselung gefordert wird.</span><span class="sxs-lookup"><span data-stu-id="e1ae5-189">Indicates whether or not to require encryption on a windows 8.1 device.</span></span>|



## <a name="response"></a><span data-ttu-id="e1ae5-190">Antwort</span><span class="sxs-lookup"><span data-stu-id="e1ae5-190">Response</span></span>
<span data-ttu-id="e1ae5-191">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="e1ae5-191">If successful, this method returns a `201 Created` response code and a [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e1ae5-192">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e1ae5-192">Example</span></span>
### <a name="request"></a><span data-ttu-id="e1ae5-193">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e1ae5-193">Request</span></span>
<span data-ttu-id="e1ae5-194">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e1ae5-194">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 602

{
  "@odata.type": "#microsoft.graph.windows81CompliancePolicy",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "passwordPreviousPasswordBlockCount": 2,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "storageRequireEncryption": true
}
```

### <a name="response"></a><span data-ttu-id="e1ae5-195">Antwort</span><span class="sxs-lookup"><span data-stu-id="e1ae5-195">Response</span></span>
<span data-ttu-id="e1ae5-p110">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e1ae5-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 774

{
  "@odata.type": "#microsoft.graph.windows81CompliancePolicy",
  "id": "6bb4b7e0-b7e0-6bb4-e0b7-b46be0b7b46b",
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
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "passwordPreviousPasswordBlockCount": 2,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "storageRequireEncryption": true
}
```


