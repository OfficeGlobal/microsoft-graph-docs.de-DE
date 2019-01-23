---
title: windows81CompliancePolicy aktualsieren
description: Aktualisiert die Eigenschaften von Objekten des Typs windows81CompliancePolicy.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 77b744aa62fddf7427496855a2e8a20239ff53ee
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29413577"
---
# <a name="update-windows81compliancepolicy"></a><span data-ttu-id="901e7-103">windows81CompliancePolicy aktualsieren</span><span class="sxs-lookup"><span data-stu-id="901e7-103">Update windows81CompliancePolicy</span></span>

> <span data-ttu-id="901e7-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="901e7-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="901e7-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="901e7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="901e7-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="901e7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="901e7-107">Aktualisiert die Eigenschaften von Objekten des Typs [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="901e7-107">Update the properties of a [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="901e7-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="901e7-108">Prerequisites</span></span>
<span data-ttu-id="901e7-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="901e7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="901e7-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="901e7-111">Permission type</span></span>|<span data-ttu-id="901e7-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="901e7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="901e7-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="901e7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="901e7-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="901e7-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="901e7-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="901e7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="901e7-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="901e7-116">Not supported.</span></span>|
|<span data-ttu-id="901e7-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="901e7-117">Application</span></span>|<span data-ttu-id="901e7-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="901e7-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="901e7-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="901e7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="901e7-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="901e7-120">Request headers</span></span>
|<span data-ttu-id="901e7-121">Header</span><span class="sxs-lookup"><span data-stu-id="901e7-121">Header</span></span>|<span data-ttu-id="901e7-122">Wert</span><span class="sxs-lookup"><span data-stu-id="901e7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="901e7-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="901e7-123">Authorization</span></span>|<span data-ttu-id="901e7-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="901e7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="901e7-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="901e7-125">Accept</span></span>|<span data-ttu-id="901e7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="901e7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="901e7-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="901e7-127">Request body</span></span>
<span data-ttu-id="901e7-128">Geben Sie im Anforderungstext eine JSON-Darstellung des [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="901e7-128">In the request body, supply a JSON representation for the [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object.</span></span>

<span data-ttu-id="901e7-129">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="901e7-129">The following table shows the properties that are required when you create the [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md).</span></span>

|<span data-ttu-id="901e7-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="901e7-130">Property</span></span>|<span data-ttu-id="901e7-131">Typ</span><span class="sxs-lookup"><span data-stu-id="901e7-131">Type</span></span>|<span data-ttu-id="901e7-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="901e7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="901e7-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="901e7-133">roleScopeTagIds</span></span>|<span data-ttu-id="901e7-134">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="901e7-134">String collection</span></span>|<span data-ttu-id="901e7-135">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="901e7-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="901e7-136">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="901e7-136">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="901e7-137">id</span><span class="sxs-lookup"><span data-stu-id="901e7-137">id</span></span>|<span data-ttu-id="901e7-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="901e7-138">String</span></span>|<span data-ttu-id="901e7-139">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="901e7-139">Key of the entity.</span></span> <span data-ttu-id="901e7-140">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="901e7-140">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="901e7-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="901e7-141">createdDateTime</span></span>|<span data-ttu-id="901e7-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="901e7-142">DateTimeOffset</span></span>|<span data-ttu-id="901e7-143">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="901e7-143">DateTime the object was created.</span></span> <span data-ttu-id="901e7-144">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="901e7-144">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="901e7-145">description</span><span class="sxs-lookup"><span data-stu-id="901e7-145">description</span></span>|<span data-ttu-id="901e7-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="901e7-146">String</span></span>|<span data-ttu-id="901e7-147">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="901e7-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="901e7-148">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="901e7-148">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="901e7-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="901e7-149">lastModifiedDateTime</span></span>|<span data-ttu-id="901e7-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="901e7-150">DateTimeOffset</span></span>|<span data-ttu-id="901e7-151">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="901e7-151">DateTime the object was last modified.</span></span> <span data-ttu-id="901e7-152">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="901e7-152">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="901e7-153">displayName</span><span class="sxs-lookup"><span data-stu-id="901e7-153">displayName</span></span>|<span data-ttu-id="901e7-154">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="901e7-154">String</span></span>|<span data-ttu-id="901e7-155">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="901e7-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="901e7-156">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="901e7-156">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="901e7-157">Version</span><span class="sxs-lookup"><span data-stu-id="901e7-157">version</span></span>|<span data-ttu-id="901e7-158">Int32</span><span class="sxs-lookup"><span data-stu-id="901e7-158">Int32</span></span>|<span data-ttu-id="901e7-159">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="901e7-159">Version of the device configuration.</span></span> <span data-ttu-id="901e7-160">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="901e7-160">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="901e7-161">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="901e7-161">passwordRequired</span></span>|<span data-ttu-id="901e7-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="901e7-162">Boolean</span></span>|<span data-ttu-id="901e7-163">Legt fest, dass zum Entsperren des Windows-Geräts ein Kennwort erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="901e7-163">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="901e7-164">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="901e7-164">passwordBlockSimple</span></span>|<span data-ttu-id="901e7-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="901e7-165">Boolean</span></span>|<span data-ttu-id="901e7-166">Gibt an, ob einfache Kennwörter erlaubt sind.</span><span class="sxs-lookup"><span data-stu-id="901e7-166">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="901e7-167">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="901e7-167">passwordExpirationDays</span></span>|<span data-ttu-id="901e7-168">Int32</span><span class="sxs-lookup"><span data-stu-id="901e7-168">Int32</span></span>|<span data-ttu-id="901e7-169">Zeit bis zum Ablaufen des Kennworts in Tagen</span><span class="sxs-lookup"><span data-stu-id="901e7-169">Password expiration in days.</span></span>|
|<span data-ttu-id="901e7-170">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="901e7-170">passwordMinimumLength</span></span>|<span data-ttu-id="901e7-171">Int32</span><span class="sxs-lookup"><span data-stu-id="901e7-171">Int32</span></span>|<span data-ttu-id="901e7-172">Mindestlänge des Kennworts</span><span class="sxs-lookup"><span data-stu-id="901e7-172">The minimum password length.</span></span>|
|<span data-ttu-id="901e7-173">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="901e7-173">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="901e7-174">Int32</span><span class="sxs-lookup"><span data-stu-id="901e7-174">Int32</span></span>|<span data-ttu-id="901e7-175">Zeitraum von Inaktivität in Minuten, nach dem die Eingabe eines Kennworts gefordert wird</span><span class="sxs-lookup"><span data-stu-id="901e7-175">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="901e7-176">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="901e7-176">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="901e7-177">Int32</span><span class="sxs-lookup"><span data-stu-id="901e7-177">Int32</span></span>|<span data-ttu-id="901e7-178">Anzahl der Zeichensätze, die im Kennwort enthalten sein müssen</span><span class="sxs-lookup"><span data-stu-id="901e7-178">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="901e7-179">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="901e7-179">passwordRequiredType</span></span>|[<span data-ttu-id="901e7-180">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="901e7-180">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="901e7-181">Geforderter Kennworttyp.</span><span class="sxs-lookup"><span data-stu-id="901e7-181">The required password type.</span></span> <span data-ttu-id="901e7-182">Mögliche Werte sind: `deviceDefault`, `alphanumeric` und `numeric`.</span><span class="sxs-lookup"><span data-stu-id="901e7-182">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="901e7-183">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="901e7-183">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="901e7-184">Int32</span><span class="sxs-lookup"><span data-stu-id="901e7-184">Int32</span></span>|<span data-ttu-id="901e7-185">Grenze für die Wiederverwendung von Kennwörtern. Der festgelegte Wert gibt an, von wie vielen der zuletzt genutzten Kennwörter sich das Kennwort unterscheiden muss.</span><span class="sxs-lookup"><span data-stu-id="901e7-185">The number of previous passwords to prevent re-use of.</span></span> <span data-ttu-id="901e7-186">Gültige Werte: 0 bis 24.</span><span class="sxs-lookup"><span data-stu-id="901e7-186">Valid values 0 to 24</span></span>|
|<span data-ttu-id="901e7-187">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="901e7-187">osMinimumVersion</span></span>|<span data-ttu-id="901e7-188">String</span><span class="sxs-lookup"><span data-stu-id="901e7-188">String</span></span>|<span data-ttu-id="901e7-189">Mindestversion von Windows 8.1</span><span class="sxs-lookup"><span data-stu-id="901e7-189">Minimum Windows 8.1 version.</span></span>|
|<span data-ttu-id="901e7-190">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="901e7-190">osMaximumVersion</span></span>|<span data-ttu-id="901e7-191">String</span><span class="sxs-lookup"><span data-stu-id="901e7-191">String</span></span>|<span data-ttu-id="901e7-192">Maximalversion von Windows 8.1</span><span class="sxs-lookup"><span data-stu-id="901e7-192">Maximum Windows 8.1 version.</span></span>|
|<span data-ttu-id="901e7-193">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="901e7-193">storageRequireEncryption</span></span>|<span data-ttu-id="901e7-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="901e7-194">Boolean</span></span>|<span data-ttu-id="901e7-195">Gibt an, ob für ein Windows 8.1-Gerät Verschlüsselung gefordert wird.</span><span class="sxs-lookup"><span data-stu-id="901e7-195">Indicates whether or not to require encryption on a windows 8.1 device.</span></span>|



## <a name="response"></a><span data-ttu-id="901e7-196">Antwort</span><span class="sxs-lookup"><span data-stu-id="901e7-196">Response</span></span>
<span data-ttu-id="901e7-197">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte  [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="901e7-197">If successful, this method returns a `200 OK` response code and an updated [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="901e7-198">Beispiel</span><span class="sxs-lookup"><span data-stu-id="901e7-198">Example</span></span>

### <a name="request"></a><span data-ttu-id="901e7-199">Anforderung</span><span class="sxs-lookup"><span data-stu-id="901e7-199">Request</span></span>
<span data-ttu-id="901e7-200">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="901e7-200">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
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

### <a name="response"></a><span data-ttu-id="901e7-201">Antwort</span><span class="sxs-lookup"><span data-stu-id="901e7-201">Response</span></span>
<span data-ttu-id="901e7-p112">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="901e7-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




