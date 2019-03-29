---
title: Aktualisieren von „windowsPhone81CompliancePolicy“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs windowsPhone81CompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 840504bf54f70e6a15cbf486946247fa33c0b3b5
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30959831"
---
# <a name="update-windowsphone81compliancepolicy"></a><span data-ttu-id="f0a83-103">Aktualisieren von „windowsPhone81CompliancePolicy“</span><span class="sxs-lookup"><span data-stu-id="f0a83-103">Update windowsPhone81CompliancePolicy</span></span>

> <span data-ttu-id="f0a83-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="f0a83-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f0a83-105">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f0a83-105">Update the properties of a [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f0a83-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f0a83-106">Prerequisites</span></span>
<span data-ttu-id="f0a83-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f0a83-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f0a83-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f0a83-109">Permission type</span></span>|<span data-ttu-id="f0a83-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f0a83-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f0a83-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f0a83-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f0a83-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f0a83-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f0a83-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f0a83-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f0a83-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f0a83-114">Not supported.</span></span>|
|<span data-ttu-id="f0a83-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f0a83-115">Application</span></span>|<span data-ttu-id="f0a83-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f0a83-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f0a83-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f0a83-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="f0a83-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f0a83-118">Request headers</span></span>
|<span data-ttu-id="f0a83-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="f0a83-119">Header</span></span>|<span data-ttu-id="f0a83-120">Wert</span><span class="sxs-lookup"><span data-stu-id="f0a83-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f0a83-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f0a83-121">Authorization</span></span>|<span data-ttu-id="f0a83-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="f0a83-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f0a83-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="f0a83-123">Accept</span></span>|<span data-ttu-id="f0a83-124">application/json</span><span class="sxs-lookup"><span data-stu-id="f0a83-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f0a83-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f0a83-125">Request body</span></span>
<span data-ttu-id="f0a83-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) an.</span><span class="sxs-lookup"><span data-stu-id="f0a83-126">In the request body, supply a JSON representation for the [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object.</span></span>

<span data-ttu-id="f0a83-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="f0a83-127">The following table shows the properties that are required when you create the [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md).</span></span>

|<span data-ttu-id="f0a83-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f0a83-128">Property</span></span>|<span data-ttu-id="f0a83-129">Typ</span><span class="sxs-lookup"><span data-stu-id="f0a83-129">Type</span></span>|<span data-ttu-id="f0a83-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f0a83-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f0a83-131">id</span><span class="sxs-lookup"><span data-stu-id="f0a83-131">id</span></span>|<span data-ttu-id="f0a83-132">String</span><span class="sxs-lookup"><span data-stu-id="f0a83-132">String</span></span>|<span data-ttu-id="f0a83-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="f0a83-133">Key of the entity.</span></span> <span data-ttu-id="f0a83-134">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f0a83-134">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f0a83-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f0a83-135">createdDateTime</span></span>|<span data-ttu-id="f0a83-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f0a83-136">DateTimeOffset</span></span>|<span data-ttu-id="f0a83-137">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="f0a83-137">DateTime the object was created.</span></span> <span data-ttu-id="f0a83-138">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f0a83-138">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f0a83-139">description</span><span class="sxs-lookup"><span data-stu-id="f0a83-139">description</span></span>|<span data-ttu-id="f0a83-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f0a83-140">String</span></span>|<span data-ttu-id="f0a83-141">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="f0a83-141">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f0a83-142">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f0a83-142">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f0a83-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f0a83-143">lastModifiedDateTime</span></span>|<span data-ttu-id="f0a83-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f0a83-144">DateTimeOffset</span></span>|<span data-ttu-id="f0a83-145">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="f0a83-145">DateTime the object was last modified.</span></span> <span data-ttu-id="f0a83-146">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f0a83-146">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f0a83-147">displayName</span><span class="sxs-lookup"><span data-stu-id="f0a83-147">displayName</span></span>|<span data-ttu-id="f0a83-148">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f0a83-148">String</span></span>|<span data-ttu-id="f0a83-149">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="f0a83-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f0a83-150">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f0a83-150">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f0a83-151">Version</span><span class="sxs-lookup"><span data-stu-id="f0a83-151">version</span></span>|<span data-ttu-id="f0a83-152">Int32</span><span class="sxs-lookup"><span data-stu-id="f0a83-152">Int32</span></span>|<span data-ttu-id="f0a83-153">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="f0a83-153">Version of the device configuration.</span></span> <span data-ttu-id="f0a83-154">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f0a83-154">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f0a83-155">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="f0a83-155">passwordBlockSimple</span></span>|<span data-ttu-id="f0a83-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0a83-156">Boolean</span></span>|<span data-ttu-id="f0a83-157">Gibt an, ob die Kalendersynchronisierung blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="f0a83-157">Whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="f0a83-158">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="f0a83-158">passwordExpirationDays</span></span>|<span data-ttu-id="f0a83-159">Int32</span><span class="sxs-lookup"><span data-stu-id="f0a83-159">Int32</span></span>|<span data-ttu-id="f0a83-160">Zeit in Tagen bis zum Ablaufen des Kennworts</span><span class="sxs-lookup"><span data-stu-id="f0a83-160">Number of days before the password expires.</span></span>|
|<span data-ttu-id="f0a83-161">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="f0a83-161">passwordMinimumLength</span></span>|<span data-ttu-id="f0a83-162">Int32</span><span class="sxs-lookup"><span data-stu-id="f0a83-162">Int32</span></span>|<span data-ttu-id="f0a83-163">Mindestlänge von Kennwörtern</span><span class="sxs-lookup"><span data-stu-id="f0a83-163">Minimum length of passwords.</span></span>|
|<span data-ttu-id="f0a83-164">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="f0a83-164">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="f0a83-165">Int32</span><span class="sxs-lookup"><span data-stu-id="f0a83-165">Int32</span></span>|<span data-ttu-id="f0a83-166">Zeitraum von Inaktivität in Minuten, nach dem die Eingabe eines Kennworts gefordert wird</span><span class="sxs-lookup"><span data-stu-id="f0a83-166">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="f0a83-167">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="f0a83-167">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="f0a83-168">Int32</span><span class="sxs-lookup"><span data-stu-id="f0a83-168">Int32</span></span>|<span data-ttu-id="f0a83-169">Anzahl der Zeichensätze, die im Kennwort enthalten sein müssen.</span><span class="sxs-lookup"><span data-stu-id="f0a83-169">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="f0a83-170">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="f0a83-170">passwordRequiredType</span></span>|[<span data-ttu-id="f0a83-171">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="f0a83-171">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="f0a83-172">Geforderter Kennworttyp.</span><span class="sxs-lookup"><span data-stu-id="f0a83-172">The required password type.</span></span> <span data-ttu-id="f0a83-173">Mögliche Werte sind: `deviceDefault`, `alphanumeric` und `numeric`.</span><span class="sxs-lookup"><span data-stu-id="f0a83-173">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="f0a83-174">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="f0a83-174">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="f0a83-175">Int32</span><span class="sxs-lookup"><span data-stu-id="f0a83-175">Int32</span></span>|<span data-ttu-id="f0a83-176">Anzahl der zuletzt verwendeten Kennwörter, die nicht erneut verwendet werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="f0a83-176">Number of previous passwords to block.</span></span> <span data-ttu-id="f0a83-177">Gültige Werte: 0 bis 24.</span><span class="sxs-lookup"><span data-stu-id="f0a83-177">Valid values 0 to 24</span></span>|
|<span data-ttu-id="f0a83-178">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="f0a83-178">passwordRequired</span></span>|<span data-ttu-id="f0a83-179">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f0a83-179">Boolean</span></span>|<span data-ttu-id="f0a83-180">Legt fest, ob ein Kennwort gefordert wird.</span><span class="sxs-lookup"><span data-stu-id="f0a83-180">Whether or not to require a password.</span></span>|
|<span data-ttu-id="f0a83-181">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="f0a83-181">osMinimumVersion</span></span>|<span data-ttu-id="f0a83-182">String</span><span class="sxs-lookup"><span data-stu-id="f0a83-182">String</span></span>|<span data-ttu-id="f0a83-183">Mindestversion von Windows Phone</span><span class="sxs-lookup"><span data-stu-id="f0a83-183">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="f0a83-184">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="f0a83-184">osMaximumVersion</span></span>|<span data-ttu-id="f0a83-185">String</span><span class="sxs-lookup"><span data-stu-id="f0a83-185">String</span></span>|<span data-ttu-id="f0a83-186">Maximalversion von Windows Phone</span><span class="sxs-lookup"><span data-stu-id="f0a83-186">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="f0a83-187">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="f0a83-187">storageRequireEncryption</span></span>|<span data-ttu-id="f0a83-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0a83-188">Boolean</span></span>|<span data-ttu-id="f0a83-189">Legt fest, dass auf Windows Phone-Geräten Verschlüsselung gefordert wird.</span><span class="sxs-lookup"><span data-stu-id="f0a83-189">Require encryption on windows phone devices.</span></span>|



## <a name="response"></a><span data-ttu-id="f0a83-190">Antwort</span><span class="sxs-lookup"><span data-stu-id="f0a83-190">Response</span></span>
<span data-ttu-id="f0a83-191">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="f0a83-191">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f0a83-192">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f0a83-192">Example</span></span>

### <a name="request"></a><span data-ttu-id="f0a83-193">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f0a83-193">Request</span></span>
<span data-ttu-id="f0a83-194">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f0a83-194">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 607

{
  "@odata.type": "#microsoft.graph.windowsPhone81CompliancePolicy",
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

### <a name="response"></a><span data-ttu-id="f0a83-195">Antwort</span><span class="sxs-lookup"><span data-stu-id="f0a83-195">Response</span></span>
<span data-ttu-id="f0a83-p110">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f0a83-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 779

{
  "@odata.type": "#microsoft.graph.windowsPhone81CompliancePolicy",
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



