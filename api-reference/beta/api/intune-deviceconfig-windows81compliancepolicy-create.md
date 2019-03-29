---
title: Erstellen von „windows81CompliancePolicy“
description: Erstellt neue Objekte des Typs windows81CompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2c2c8646185ca0355aceab0863f375768e390d38
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30985179"
---
# <a name="create-windows81compliancepolicy"></a><span data-ttu-id="28db9-103">Erstellen von „windows81CompliancePolicy“</span><span class="sxs-lookup"><span data-stu-id="28db9-103">Create windows81CompliancePolicy</span></span>

> <span data-ttu-id="28db9-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="28db9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="28db9-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="28db9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="28db9-106">Diese Methode erstellt ein neues Objekt des Typs [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="28db9-106">Create a new [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="28db9-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="28db9-107">Prerequisites</span></span>
<span data-ttu-id="28db9-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="28db9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="28db9-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="28db9-110">Permission type</span></span>|<span data-ttu-id="28db9-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="28db9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="28db9-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="28db9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="28db9-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="28db9-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="28db9-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="28db9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="28db9-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="28db9-115">Not supported.</span></span>|
|<span data-ttu-id="28db9-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="28db9-116">Application</span></span>|<span data-ttu-id="28db9-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="28db9-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="28db9-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="28db9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="28db9-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="28db9-119">Request headers</span></span>
|<span data-ttu-id="28db9-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="28db9-120">Header</span></span>|<span data-ttu-id="28db9-121">Wert</span><span class="sxs-lookup"><span data-stu-id="28db9-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="28db9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="28db9-122">Authorization</span></span>|<span data-ttu-id="28db9-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="28db9-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="28db9-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="28db9-124">Accept</span></span>|<span data-ttu-id="28db9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="28db9-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="28db9-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="28db9-126">Request body</span></span>
<span data-ttu-id="28db9-127">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „windows81CompliancePolicy“ an.</span><span class="sxs-lookup"><span data-stu-id="28db9-127">In the request body, supply a JSON representation for the windows81CompliancePolicy object.</span></span>

<span data-ttu-id="28db9-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „windows81CompliancePolicy“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="28db9-128">The following table shows the properties that are required when you create the windows81CompliancePolicy.</span></span>

|<span data-ttu-id="28db9-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="28db9-129">Property</span></span>|<span data-ttu-id="28db9-130">Typ</span><span class="sxs-lookup"><span data-stu-id="28db9-130">Type</span></span>|<span data-ttu-id="28db9-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="28db9-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="28db9-132">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="28db9-132">roleScopeTagIds</span></span>|<span data-ttu-id="28db9-133">String collection</span><span class="sxs-lookup"><span data-stu-id="28db9-133">String collection</span></span>|<span data-ttu-id="28db9-134">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="28db9-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="28db9-135">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="28db9-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="28db9-136">id</span><span class="sxs-lookup"><span data-stu-id="28db9-136">id</span></span>|<span data-ttu-id="28db9-137">String</span><span class="sxs-lookup"><span data-stu-id="28db9-137">String</span></span>|<span data-ttu-id="28db9-138">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="28db9-138">Key of the entity.</span></span> <span data-ttu-id="28db9-139">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="28db9-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="28db9-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="28db9-140">createdDateTime</span></span>|<span data-ttu-id="28db9-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="28db9-141">DateTimeOffset</span></span>|<span data-ttu-id="28db9-142">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="28db9-142">DateTime the object was created.</span></span> <span data-ttu-id="28db9-143">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="28db9-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="28db9-144">description</span><span class="sxs-lookup"><span data-stu-id="28db9-144">description</span></span>|<span data-ttu-id="28db9-145">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="28db9-145">String</span></span>|<span data-ttu-id="28db9-146">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="28db9-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="28db9-147">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="28db9-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="28db9-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="28db9-148">lastModifiedDateTime</span></span>|<span data-ttu-id="28db9-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="28db9-149">DateTimeOffset</span></span>|<span data-ttu-id="28db9-150">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="28db9-150">DateTime the object was last modified.</span></span> <span data-ttu-id="28db9-151">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="28db9-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="28db9-152">displayName</span><span class="sxs-lookup"><span data-stu-id="28db9-152">displayName</span></span>|<span data-ttu-id="28db9-153">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="28db9-153">String</span></span>|<span data-ttu-id="28db9-154">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="28db9-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="28db9-155">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="28db9-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="28db9-156">Version</span><span class="sxs-lookup"><span data-stu-id="28db9-156">version</span></span>|<span data-ttu-id="28db9-157">Int32</span><span class="sxs-lookup"><span data-stu-id="28db9-157">Int32</span></span>|<span data-ttu-id="28db9-158">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="28db9-158">Version of the device configuration.</span></span> <span data-ttu-id="28db9-159">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="28db9-159">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="28db9-160">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="28db9-160">passwordRequired</span></span>|<span data-ttu-id="28db9-161">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="28db9-161">Boolean</span></span>|<span data-ttu-id="28db9-162">Legt fest, dass zum Entsperren des Windows-Geräts ein Kennwort erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="28db9-162">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="28db9-163">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="28db9-163">passwordBlockSimple</span></span>|<span data-ttu-id="28db9-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="28db9-164">Boolean</span></span>|<span data-ttu-id="28db9-165">Gibt an, ob einfache Kennwörter erlaubt sind.</span><span class="sxs-lookup"><span data-stu-id="28db9-165">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="28db9-166">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="28db9-166">passwordExpirationDays</span></span>|<span data-ttu-id="28db9-167">Int32</span><span class="sxs-lookup"><span data-stu-id="28db9-167">Int32</span></span>|<span data-ttu-id="28db9-168">Zeit bis zum Ablaufen des Kennworts in Tagen</span><span class="sxs-lookup"><span data-stu-id="28db9-168">Password expiration in days.</span></span>|
|<span data-ttu-id="28db9-169">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="28db9-169">passwordMinimumLength</span></span>|<span data-ttu-id="28db9-170">Int32</span><span class="sxs-lookup"><span data-stu-id="28db9-170">Int32</span></span>|<span data-ttu-id="28db9-171">Mindestlänge des Kennworts</span><span class="sxs-lookup"><span data-stu-id="28db9-171">The minimum password length.</span></span>|
|<span data-ttu-id="28db9-172">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="28db9-172">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="28db9-173">Int32</span><span class="sxs-lookup"><span data-stu-id="28db9-173">Int32</span></span>|<span data-ttu-id="28db9-174">Zeitraum von Inaktivität in Minuten, nach dem die Eingabe eines Kennworts gefordert wird</span><span class="sxs-lookup"><span data-stu-id="28db9-174">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="28db9-175">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="28db9-175">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="28db9-176">Int32</span><span class="sxs-lookup"><span data-stu-id="28db9-176">Int32</span></span>|<span data-ttu-id="28db9-177">Anzahl der Zeichensätze, die im Kennwort enthalten sein müssen.</span><span class="sxs-lookup"><span data-stu-id="28db9-177">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="28db9-178">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="28db9-178">passwordRequiredType</span></span>|[<span data-ttu-id="28db9-179">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="28db9-179">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="28db9-180">Geforderter Kennworttyp.</span><span class="sxs-lookup"><span data-stu-id="28db9-180">The required password type.</span></span> <span data-ttu-id="28db9-181">Mögliche Werte sind: `deviceDefault`, `alphanumeric` und `numeric`.</span><span class="sxs-lookup"><span data-stu-id="28db9-181">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="28db9-182">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="28db9-182">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="28db9-183">Int32</span><span class="sxs-lookup"><span data-stu-id="28db9-183">Int32</span></span>|<span data-ttu-id="28db9-184">Grenze für die Wiederverwendung von Kennwörtern. Der festgelegte Wert gibt an, von wie vielen der zuletzt genutzten Kennwörter sich das Kennwort unterscheiden muss.</span><span class="sxs-lookup"><span data-stu-id="28db9-184">The number of previous passwords to prevent re-use of.</span></span> <span data-ttu-id="28db9-185">Gültige Werte: 0 bis 24.</span><span class="sxs-lookup"><span data-stu-id="28db9-185">Valid values 0 to 24</span></span>|
|<span data-ttu-id="28db9-186">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="28db9-186">osMinimumVersion</span></span>|<span data-ttu-id="28db9-187">String</span><span class="sxs-lookup"><span data-stu-id="28db9-187">String</span></span>|<span data-ttu-id="28db9-188">Mindestversion von Windows 8.1</span><span class="sxs-lookup"><span data-stu-id="28db9-188">Minimum Windows 8.1 version.</span></span>|
|<span data-ttu-id="28db9-189">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="28db9-189">osMaximumVersion</span></span>|<span data-ttu-id="28db9-190">String</span><span class="sxs-lookup"><span data-stu-id="28db9-190">String</span></span>|<span data-ttu-id="28db9-191">Maximalversion von Windows 8.1</span><span class="sxs-lookup"><span data-stu-id="28db9-191">Maximum Windows 8.1 version.</span></span>|
|<span data-ttu-id="28db9-192">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="28db9-192">storageRequireEncryption</span></span>|<span data-ttu-id="28db9-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="28db9-193">Boolean</span></span>|<span data-ttu-id="28db9-194">Gibt an, ob für ein Windows 8.1-Gerät Verschlüsselung gefordert wird.</span><span class="sxs-lookup"><span data-stu-id="28db9-194">Indicates whether or not to require encryption on a windows 8.1 device.</span></span>|



## <a name="response"></a><span data-ttu-id="28db9-195">Antwort</span><span class="sxs-lookup"><span data-stu-id="28db9-195">Response</span></span>
<span data-ttu-id="28db9-196">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="28db9-196">If successful, this method returns a `201 Created` response code and a [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="28db9-197">Beispiel</span><span class="sxs-lookup"><span data-stu-id="28db9-197">Example</span></span>

### <a name="request"></a><span data-ttu-id="28db9-198">Anforderung</span><span class="sxs-lookup"><span data-stu-id="28db9-198">Request</span></span>
<span data-ttu-id="28db9-199">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="28db9-199">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 664

{
  "@odata.type": "#microsoft.graph.windows81CompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
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

### <a name="response"></a><span data-ttu-id="28db9-200">Antwort</span><span class="sxs-lookup"><span data-stu-id="28db9-200">Response</span></span>
<span data-ttu-id="28db9-p111">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="28db9-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 836

{
  "@odata.type": "#microsoft.graph.windows81CompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
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




