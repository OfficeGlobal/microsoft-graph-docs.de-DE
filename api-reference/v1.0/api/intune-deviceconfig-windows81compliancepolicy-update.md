---
title: windows81CompliancePolicy aktualsieren
description: Aktualisiert die Eigenschaften von Objekten des Typs windows81CompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: fa6d62931617eb20fd4bb2fe304ca6422f37fa00
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826516"
---
# <a name="update-windows81compliancepolicy"></a><span data-ttu-id="9401a-103">windows81CompliancePolicy aktualsieren</span><span class="sxs-lookup"><span data-stu-id="9401a-103">Update windows81CompliancePolicy</span></span>

> <span data-ttu-id="9401a-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="9401a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9401a-105">Aktualisiert die Eigenschaften von Objekten des Typs [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="9401a-105">Update the properties of a [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9401a-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="9401a-106">Prerequisites</span></span>
<span data-ttu-id="9401a-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9401a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9401a-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9401a-109">Permission type</span></span>|<span data-ttu-id="9401a-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9401a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9401a-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9401a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9401a-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9401a-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9401a-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9401a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9401a-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9401a-114">Not supported.</span></span>|
|<span data-ttu-id="9401a-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9401a-115">Application</span></span>|<span data-ttu-id="9401a-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9401a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9401a-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9401a-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="9401a-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9401a-118">Request headers</span></span>
|<span data-ttu-id="9401a-119">Header</span><span class="sxs-lookup"><span data-stu-id="9401a-119">Header</span></span>|<span data-ttu-id="9401a-120">Wert</span><span class="sxs-lookup"><span data-stu-id="9401a-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9401a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="9401a-121">Authorization</span></span>|<span data-ttu-id="9401a-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="9401a-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9401a-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="9401a-123">Accept</span></span>|<span data-ttu-id="9401a-124">application/json</span><span class="sxs-lookup"><span data-stu-id="9401a-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9401a-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9401a-125">Request body</span></span>
<span data-ttu-id="9401a-126">Geben Sie im Anforderungstext eine JSON-Darstellung des [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="9401a-126">In the request body, supply a JSON representation for the [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object.</span></span>

<span data-ttu-id="9401a-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="9401a-127">The following table shows the properties that are required when you create the [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md).</span></span>

|<span data-ttu-id="9401a-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9401a-128">Property</span></span>|<span data-ttu-id="9401a-129">Typ</span><span class="sxs-lookup"><span data-stu-id="9401a-129">Type</span></span>|<span data-ttu-id="9401a-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9401a-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9401a-131">id</span><span class="sxs-lookup"><span data-stu-id="9401a-131">id</span></span>|<span data-ttu-id="9401a-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9401a-132">String</span></span>|<span data-ttu-id="9401a-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="9401a-133">Key of the entity.</span></span> <span data-ttu-id="9401a-134">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="9401a-134">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="9401a-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9401a-135">createdDateTime</span></span>|<span data-ttu-id="9401a-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9401a-136">DateTimeOffset</span></span>|<span data-ttu-id="9401a-137">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="9401a-137">DateTime the object was created.</span></span> <span data-ttu-id="9401a-138">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="9401a-138">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="9401a-139">description</span><span class="sxs-lookup"><span data-stu-id="9401a-139">description</span></span>|<span data-ttu-id="9401a-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9401a-140">String</span></span>|<span data-ttu-id="9401a-141">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="9401a-141">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="9401a-142">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="9401a-142">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="9401a-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9401a-143">lastModifiedDateTime</span></span>|<span data-ttu-id="9401a-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9401a-144">DateTimeOffset</span></span>|<span data-ttu-id="9401a-145">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="9401a-145">DateTime the object was last modified.</span></span> <span data-ttu-id="9401a-146">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="9401a-146">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="9401a-147">displayName</span><span class="sxs-lookup"><span data-stu-id="9401a-147">displayName</span></span>|<span data-ttu-id="9401a-148">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9401a-148">String</span></span>|<span data-ttu-id="9401a-149">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="9401a-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="9401a-150">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="9401a-150">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="9401a-151">Version</span><span class="sxs-lookup"><span data-stu-id="9401a-151">version</span></span>|<span data-ttu-id="9401a-152">Int32</span><span class="sxs-lookup"><span data-stu-id="9401a-152">Int32</span></span>|<span data-ttu-id="9401a-153">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="9401a-153">Version of the device configuration.</span></span> <span data-ttu-id="9401a-154">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="9401a-154">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="9401a-155">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="9401a-155">passwordRequired</span></span>|<span data-ttu-id="9401a-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="9401a-156">Boolean</span></span>|<span data-ttu-id="9401a-157">Legt fest, dass zum Entsperren des Windows-Geräts ein Kennwort erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="9401a-157">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="9401a-158">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="9401a-158">passwordBlockSimple</span></span>|<span data-ttu-id="9401a-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="9401a-159">Boolean</span></span>|<span data-ttu-id="9401a-160">Gibt an, ob einfache Kennwörter erlaubt sind.</span><span class="sxs-lookup"><span data-stu-id="9401a-160">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="9401a-161">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="9401a-161">passwordExpirationDays</span></span>|<span data-ttu-id="9401a-162">Int32</span><span class="sxs-lookup"><span data-stu-id="9401a-162">Int32</span></span>|<span data-ttu-id="9401a-163">Zeit bis zum Ablaufen des Kennworts in Tagen</span><span class="sxs-lookup"><span data-stu-id="9401a-163">Password expiration in days.</span></span>|
|<span data-ttu-id="9401a-164">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="9401a-164">passwordMinimumLength</span></span>|<span data-ttu-id="9401a-165">Int32</span><span class="sxs-lookup"><span data-stu-id="9401a-165">Int32</span></span>|<span data-ttu-id="9401a-166">Mindestlänge des Kennworts</span><span class="sxs-lookup"><span data-stu-id="9401a-166">The minimum password length.</span></span>|
|<span data-ttu-id="9401a-167">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="9401a-167">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="9401a-168">Int32</span><span class="sxs-lookup"><span data-stu-id="9401a-168">Int32</span></span>|<span data-ttu-id="9401a-169">Zeitraum von Inaktivität in Minuten, nach dem die Eingabe eines Kennworts gefordert wird</span><span class="sxs-lookup"><span data-stu-id="9401a-169">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="9401a-170">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="9401a-170">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="9401a-171">Int32</span><span class="sxs-lookup"><span data-stu-id="9401a-171">Int32</span></span>|<span data-ttu-id="9401a-172">Anzahl der Zeichensätze, die im Kennwort enthalten sein müssen</span><span class="sxs-lookup"><span data-stu-id="9401a-172">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="9401a-173">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="9401a-173">passwordRequiredType</span></span>|[<span data-ttu-id="9401a-174">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="9401a-174">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="9401a-175">Geforderter Kennworttyp.</span><span class="sxs-lookup"><span data-stu-id="9401a-175">The required password type.</span></span> <span data-ttu-id="9401a-176">Mögliche Werte sind: `deviceDefault`, `alphanumeric` und `numeric`.</span><span class="sxs-lookup"><span data-stu-id="9401a-176">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="9401a-177">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="9401a-177">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="9401a-178">Int32</span><span class="sxs-lookup"><span data-stu-id="9401a-178">Int32</span></span>|<span data-ttu-id="9401a-179">Grenze für die Wiederverwendung von Kennwörtern. Der festgelegte Wert gibt an, von wie vielen der zuletzt genutzten Kennwörter sich das Kennwort unterscheiden muss.</span><span class="sxs-lookup"><span data-stu-id="9401a-179">The number of previous passwords to prevent re-use of.</span></span> <span data-ttu-id="9401a-180">Gültige Werte: 0 bis 24.</span><span class="sxs-lookup"><span data-stu-id="9401a-180">Valid values 0 to 24</span></span>|
|<span data-ttu-id="9401a-181">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="9401a-181">osMinimumVersion</span></span>|<span data-ttu-id="9401a-182">String</span><span class="sxs-lookup"><span data-stu-id="9401a-182">String</span></span>|<span data-ttu-id="9401a-183">Mindestversion von Windows 8.1</span><span class="sxs-lookup"><span data-stu-id="9401a-183">Minimum Windows 8.1 version.</span></span>|
|<span data-ttu-id="9401a-184">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="9401a-184">osMaximumVersion</span></span>|<span data-ttu-id="9401a-185">String</span><span class="sxs-lookup"><span data-stu-id="9401a-185">String</span></span>|<span data-ttu-id="9401a-186">Maximalversion von Windows 8.1</span><span class="sxs-lookup"><span data-stu-id="9401a-186">Maximum Windows 8.1 version.</span></span>|
|<span data-ttu-id="9401a-187">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="9401a-187">storageRequireEncryption</span></span>|<span data-ttu-id="9401a-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="9401a-188">Boolean</span></span>|<span data-ttu-id="9401a-189">Gibt an, ob für ein Windows 8.1-Gerät Verschlüsselung gefordert wird.</span><span class="sxs-lookup"><span data-stu-id="9401a-189">Indicates whether or not to require encryption on a windows 8.1 device.</span></span>|



## <a name="response"></a><span data-ttu-id="9401a-190">Antwort</span><span class="sxs-lookup"><span data-stu-id="9401a-190">Response</span></span>
<span data-ttu-id="9401a-191">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte  [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9401a-191">If successful, this method returns a `200 OK` response code and an updated [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9401a-192">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9401a-192">Example</span></span>
### <a name="request"></a><span data-ttu-id="9401a-193">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9401a-193">Request</span></span>
<span data-ttu-id="9401a-194">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9401a-194">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9401a-195">Antwort</span><span class="sxs-lookup"><span data-stu-id="9401a-195">Response</span></span>
<span data-ttu-id="9401a-p110">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9401a-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



