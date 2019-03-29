---
title: windows81CompliancePolicy aktualsieren
description: Aktualisiert die Eigenschaften von Objekten des Typs windows81CompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3c9fcc9d06ec02db77de0a3608f80a44632e667c
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30975336"
---
# <a name="update-windows81compliancepolicy"></a><span data-ttu-id="515c8-103">windows81CompliancePolicy aktualsieren</span><span class="sxs-lookup"><span data-stu-id="515c8-103">Update windows81CompliancePolicy</span></span>

> <span data-ttu-id="515c8-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="515c8-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="515c8-105">Aktualisiert die Eigenschaften von Objekten des Typs [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="515c8-105">Update the properties of a [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="515c8-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="515c8-106">Prerequisites</span></span>
<span data-ttu-id="515c8-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="515c8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="515c8-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="515c8-109">Permission type</span></span>|<span data-ttu-id="515c8-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="515c8-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="515c8-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="515c8-111">Delegated (work or school account)</span></span>|<span data-ttu-id="515c8-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="515c8-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="515c8-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="515c8-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="515c8-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="515c8-114">Not supported.</span></span>|
|<span data-ttu-id="515c8-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="515c8-115">Application</span></span>|<span data-ttu-id="515c8-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="515c8-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="515c8-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="515c8-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="515c8-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="515c8-118">Request headers</span></span>
|<span data-ttu-id="515c8-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="515c8-119">Header</span></span>|<span data-ttu-id="515c8-120">Wert</span><span class="sxs-lookup"><span data-stu-id="515c8-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="515c8-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="515c8-121">Authorization</span></span>|<span data-ttu-id="515c8-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="515c8-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="515c8-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="515c8-123">Accept</span></span>|<span data-ttu-id="515c8-124">application/json</span><span class="sxs-lookup"><span data-stu-id="515c8-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="515c8-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="515c8-125">Request body</span></span>
<span data-ttu-id="515c8-126">Geben Sie im Anforderungstext eine JSON-Darstellung des [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="515c8-126">In the request body, supply a JSON representation for the [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object.</span></span>

<span data-ttu-id="515c8-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="515c8-127">The following table shows the properties that are required when you create the [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md).</span></span>

|<span data-ttu-id="515c8-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="515c8-128">Property</span></span>|<span data-ttu-id="515c8-129">Typ</span><span class="sxs-lookup"><span data-stu-id="515c8-129">Type</span></span>|<span data-ttu-id="515c8-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="515c8-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="515c8-131">id</span><span class="sxs-lookup"><span data-stu-id="515c8-131">id</span></span>|<span data-ttu-id="515c8-132">String</span><span class="sxs-lookup"><span data-stu-id="515c8-132">String</span></span>|<span data-ttu-id="515c8-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="515c8-133">Key of the entity.</span></span> <span data-ttu-id="515c8-134">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="515c8-134">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="515c8-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="515c8-135">createdDateTime</span></span>|<span data-ttu-id="515c8-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="515c8-136">DateTimeOffset</span></span>|<span data-ttu-id="515c8-137">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="515c8-137">DateTime the object was created.</span></span> <span data-ttu-id="515c8-138">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="515c8-138">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="515c8-139">description</span><span class="sxs-lookup"><span data-stu-id="515c8-139">description</span></span>|<span data-ttu-id="515c8-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="515c8-140">String</span></span>|<span data-ttu-id="515c8-141">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="515c8-141">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="515c8-142">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="515c8-142">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="515c8-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="515c8-143">lastModifiedDateTime</span></span>|<span data-ttu-id="515c8-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="515c8-144">DateTimeOffset</span></span>|<span data-ttu-id="515c8-145">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="515c8-145">DateTime the object was last modified.</span></span> <span data-ttu-id="515c8-146">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="515c8-146">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="515c8-147">displayName</span><span class="sxs-lookup"><span data-stu-id="515c8-147">displayName</span></span>|<span data-ttu-id="515c8-148">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="515c8-148">String</span></span>|<span data-ttu-id="515c8-149">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="515c8-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="515c8-150">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="515c8-150">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="515c8-151">Version</span><span class="sxs-lookup"><span data-stu-id="515c8-151">version</span></span>|<span data-ttu-id="515c8-152">Int32</span><span class="sxs-lookup"><span data-stu-id="515c8-152">Int32</span></span>|<span data-ttu-id="515c8-153">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="515c8-153">Version of the device configuration.</span></span> <span data-ttu-id="515c8-154">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="515c8-154">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="515c8-155">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="515c8-155">passwordRequired</span></span>|<span data-ttu-id="515c8-156">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="515c8-156">Boolean</span></span>|<span data-ttu-id="515c8-157">Legt fest, dass zum Entsperren des Windows-Geräts ein Kennwort erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="515c8-157">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="515c8-158">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="515c8-158">passwordBlockSimple</span></span>|<span data-ttu-id="515c8-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="515c8-159">Boolean</span></span>|<span data-ttu-id="515c8-160">Gibt an, ob einfache Kennwörter erlaubt sind.</span><span class="sxs-lookup"><span data-stu-id="515c8-160">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="515c8-161">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="515c8-161">passwordExpirationDays</span></span>|<span data-ttu-id="515c8-162">Int32</span><span class="sxs-lookup"><span data-stu-id="515c8-162">Int32</span></span>|<span data-ttu-id="515c8-163">Zeit bis zum Ablaufen des Kennworts in Tagen</span><span class="sxs-lookup"><span data-stu-id="515c8-163">Password expiration in days.</span></span>|
|<span data-ttu-id="515c8-164">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="515c8-164">passwordMinimumLength</span></span>|<span data-ttu-id="515c8-165">Int32</span><span class="sxs-lookup"><span data-stu-id="515c8-165">Int32</span></span>|<span data-ttu-id="515c8-166">Mindestlänge des Kennworts</span><span class="sxs-lookup"><span data-stu-id="515c8-166">The minimum password length.</span></span>|
|<span data-ttu-id="515c8-167">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="515c8-167">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="515c8-168">Int32</span><span class="sxs-lookup"><span data-stu-id="515c8-168">Int32</span></span>|<span data-ttu-id="515c8-169">Zeitraum von Inaktivität in Minuten, nach dem die Eingabe eines Kennworts gefordert wird</span><span class="sxs-lookup"><span data-stu-id="515c8-169">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="515c8-170">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="515c8-170">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="515c8-171">Int32</span><span class="sxs-lookup"><span data-stu-id="515c8-171">Int32</span></span>|<span data-ttu-id="515c8-172">Anzahl der Zeichensätze, die im Kennwort enthalten sein müssen.</span><span class="sxs-lookup"><span data-stu-id="515c8-172">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="515c8-173">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="515c8-173">passwordRequiredType</span></span>|[<span data-ttu-id="515c8-174">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="515c8-174">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="515c8-175">Geforderter Kennworttyp.</span><span class="sxs-lookup"><span data-stu-id="515c8-175">The required password type.</span></span> <span data-ttu-id="515c8-176">Mögliche Werte sind: `deviceDefault`, `alphanumeric` und `numeric`.</span><span class="sxs-lookup"><span data-stu-id="515c8-176">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="515c8-177">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="515c8-177">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="515c8-178">Int32</span><span class="sxs-lookup"><span data-stu-id="515c8-178">Int32</span></span>|<span data-ttu-id="515c8-179">Grenze für die Wiederverwendung von Kennwörtern. Der festgelegte Wert gibt an, von wie vielen der zuletzt genutzten Kennwörter sich das Kennwort unterscheiden muss.</span><span class="sxs-lookup"><span data-stu-id="515c8-179">The number of previous passwords to prevent re-use of.</span></span> <span data-ttu-id="515c8-180">Gültige Werte: 0 bis 24.</span><span class="sxs-lookup"><span data-stu-id="515c8-180">Valid values 0 to 24</span></span>|
|<span data-ttu-id="515c8-181">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="515c8-181">osMinimumVersion</span></span>|<span data-ttu-id="515c8-182">String</span><span class="sxs-lookup"><span data-stu-id="515c8-182">String</span></span>|<span data-ttu-id="515c8-183">Mindestversion von Windows 8.1</span><span class="sxs-lookup"><span data-stu-id="515c8-183">Minimum Windows 8.1 version.</span></span>|
|<span data-ttu-id="515c8-184">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="515c8-184">osMaximumVersion</span></span>|<span data-ttu-id="515c8-185">String</span><span class="sxs-lookup"><span data-stu-id="515c8-185">String</span></span>|<span data-ttu-id="515c8-186">Maximalversion von Windows 8.1</span><span class="sxs-lookup"><span data-stu-id="515c8-186">Maximum Windows 8.1 version.</span></span>|
|<span data-ttu-id="515c8-187">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="515c8-187">storageRequireEncryption</span></span>|<span data-ttu-id="515c8-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="515c8-188">Boolean</span></span>|<span data-ttu-id="515c8-189">Gibt an, ob für ein Windows 8.1-Gerät Verschlüsselung gefordert wird.</span><span class="sxs-lookup"><span data-stu-id="515c8-189">Indicates whether or not to require encryption on a windows 8.1 device.</span></span>|



## <a name="response"></a><span data-ttu-id="515c8-190">Antwort</span><span class="sxs-lookup"><span data-stu-id="515c8-190">Response</span></span>
<span data-ttu-id="515c8-191">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte  [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="515c8-191">If successful, this method returns a `200 OK` response code and an updated [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="515c8-192">Beispiel</span><span class="sxs-lookup"><span data-stu-id="515c8-192">Example</span></span>

### <a name="request"></a><span data-ttu-id="515c8-193">Anforderung</span><span class="sxs-lookup"><span data-stu-id="515c8-193">Request</span></span>
<span data-ttu-id="515c8-194">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="515c8-194">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
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

### <a name="response"></a><span data-ttu-id="515c8-195">Antwort</span><span class="sxs-lookup"><span data-stu-id="515c8-195">Response</span></span>
<span data-ttu-id="515c8-p110">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="515c8-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



