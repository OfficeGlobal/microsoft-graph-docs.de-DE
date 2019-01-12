---
title: windows81CompliancePolicy aktualsieren
description: Aktualisiert die Eigenschaften von Objekten des Typs windows81CompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ecdd69fa115e4352b2470df263df83f889f8c36a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27979362"
---
# <a name="update-windows81compliancepolicy"></a><span data-ttu-id="fa402-103">windows81CompliancePolicy aktualsieren</span><span class="sxs-lookup"><span data-stu-id="fa402-103">Update windows81CompliancePolicy</span></span>

> <span data-ttu-id="fa402-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="fa402-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fa402-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="fa402-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fa402-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="fa402-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fa402-107">Aktualisiert die Eigenschaften von Objekten des Typs [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="fa402-107">Update the properties of a [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fa402-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="fa402-108">Prerequisites</span></span>
<span data-ttu-id="fa402-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fa402-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fa402-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="fa402-111">Permission type</span></span>|<span data-ttu-id="fa402-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="fa402-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fa402-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="fa402-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fa402-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fa402-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="fa402-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="fa402-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fa402-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fa402-116">Not supported.</span></span>|
|<span data-ttu-id="fa402-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="fa402-117">Application</span></span>|<span data-ttu-id="fa402-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fa402-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fa402-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="fa402-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="fa402-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="fa402-120">Request headers</span></span>
|<span data-ttu-id="fa402-121">Header</span><span class="sxs-lookup"><span data-stu-id="fa402-121">Header</span></span>|<span data-ttu-id="fa402-122">Wert</span><span class="sxs-lookup"><span data-stu-id="fa402-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fa402-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fa402-123">Authorization</span></span>|<span data-ttu-id="fa402-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="fa402-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fa402-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="fa402-125">Accept</span></span>|<span data-ttu-id="fa402-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fa402-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fa402-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="fa402-127">Request body</span></span>
<span data-ttu-id="fa402-128">Geben Sie im Anforderungstext eine JSON-Darstellung des [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="fa402-128">In the request body, supply a JSON representation for the [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object.</span></span>

<span data-ttu-id="fa402-129">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="fa402-129">The following table shows the properties that are required when you create the [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md).</span></span>

|<span data-ttu-id="fa402-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="fa402-130">Property</span></span>|<span data-ttu-id="fa402-131">Typ</span><span class="sxs-lookup"><span data-stu-id="fa402-131">Type</span></span>|<span data-ttu-id="fa402-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fa402-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fa402-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="fa402-133">roleScopeTagIds</span></span>|<span data-ttu-id="fa402-134">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="fa402-134">String collection</span></span>|<span data-ttu-id="fa402-135">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="fa402-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="fa402-136">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="fa402-136">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="fa402-137">id</span><span class="sxs-lookup"><span data-stu-id="fa402-137">id</span></span>|<span data-ttu-id="fa402-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fa402-138">String</span></span>|<span data-ttu-id="fa402-139">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="fa402-139">Key of the entity.</span></span> <span data-ttu-id="fa402-140">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="fa402-140">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="fa402-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fa402-141">createdDateTime</span></span>|<span data-ttu-id="fa402-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fa402-142">DateTimeOffset</span></span>|<span data-ttu-id="fa402-143">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="fa402-143">DateTime the object was created.</span></span> <span data-ttu-id="fa402-144">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="fa402-144">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="fa402-145">description</span><span class="sxs-lookup"><span data-stu-id="fa402-145">description</span></span>|<span data-ttu-id="fa402-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fa402-146">String</span></span>|<span data-ttu-id="fa402-147">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="fa402-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="fa402-148">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="fa402-148">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="fa402-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fa402-149">lastModifiedDateTime</span></span>|<span data-ttu-id="fa402-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fa402-150">DateTimeOffset</span></span>|<span data-ttu-id="fa402-151">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="fa402-151">DateTime the object was last modified.</span></span> <span data-ttu-id="fa402-152">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="fa402-152">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="fa402-153">displayName</span><span class="sxs-lookup"><span data-stu-id="fa402-153">displayName</span></span>|<span data-ttu-id="fa402-154">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fa402-154">String</span></span>|<span data-ttu-id="fa402-155">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="fa402-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="fa402-156">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="fa402-156">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="fa402-157">Version</span><span class="sxs-lookup"><span data-stu-id="fa402-157">version</span></span>|<span data-ttu-id="fa402-158">Int32</span><span class="sxs-lookup"><span data-stu-id="fa402-158">Int32</span></span>|<span data-ttu-id="fa402-159">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="fa402-159">Version of the device configuration.</span></span> <span data-ttu-id="fa402-160">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="fa402-160">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="fa402-161">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="fa402-161">passwordRequired</span></span>|<span data-ttu-id="fa402-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="fa402-162">Boolean</span></span>|<span data-ttu-id="fa402-163">Legt fest, dass zum Entsperren des Windows-Geräts ein Kennwort erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="fa402-163">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="fa402-164">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="fa402-164">passwordBlockSimple</span></span>|<span data-ttu-id="fa402-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="fa402-165">Boolean</span></span>|<span data-ttu-id="fa402-166">Gibt an, ob einfache Kennwörter erlaubt sind.</span><span class="sxs-lookup"><span data-stu-id="fa402-166">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="fa402-167">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="fa402-167">passwordExpirationDays</span></span>|<span data-ttu-id="fa402-168">Int32</span><span class="sxs-lookup"><span data-stu-id="fa402-168">Int32</span></span>|<span data-ttu-id="fa402-169">Zeit bis zum Ablaufen des Kennworts in Tagen</span><span class="sxs-lookup"><span data-stu-id="fa402-169">Password expiration in days.</span></span>|
|<span data-ttu-id="fa402-170">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="fa402-170">passwordMinimumLength</span></span>|<span data-ttu-id="fa402-171">Int32</span><span class="sxs-lookup"><span data-stu-id="fa402-171">Int32</span></span>|<span data-ttu-id="fa402-172">Mindestlänge des Kennworts</span><span class="sxs-lookup"><span data-stu-id="fa402-172">The minimum password length.</span></span>|
|<span data-ttu-id="fa402-173">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="fa402-173">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="fa402-174">Int32</span><span class="sxs-lookup"><span data-stu-id="fa402-174">Int32</span></span>|<span data-ttu-id="fa402-175">Zeitraum von Inaktivität in Minuten, nach dem die Eingabe eines Kennworts gefordert wird</span><span class="sxs-lookup"><span data-stu-id="fa402-175">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="fa402-176">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="fa402-176">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="fa402-177">Int32</span><span class="sxs-lookup"><span data-stu-id="fa402-177">Int32</span></span>|<span data-ttu-id="fa402-178">Anzahl der Zeichensätze, die im Kennwort enthalten sein müssen</span><span class="sxs-lookup"><span data-stu-id="fa402-178">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="fa402-179">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="fa402-179">passwordRequiredType</span></span>|[<span data-ttu-id="fa402-180">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="fa402-180">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="fa402-181">Geforderter Kennworttyp.</span><span class="sxs-lookup"><span data-stu-id="fa402-181">The required password type.</span></span> <span data-ttu-id="fa402-182">Mögliche Werte sind: `deviceDefault`, `alphanumeric` und `numeric`.</span><span class="sxs-lookup"><span data-stu-id="fa402-182">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="fa402-183">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="fa402-183">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="fa402-184">Int32</span><span class="sxs-lookup"><span data-stu-id="fa402-184">Int32</span></span>|<span data-ttu-id="fa402-185">Grenze für die Wiederverwendung von Kennwörtern. Der festgelegte Wert gibt an, von wie vielen der zuletzt genutzten Kennwörter sich das Kennwort unterscheiden muss.</span><span class="sxs-lookup"><span data-stu-id="fa402-185">The number of previous passwords to prevent re-use of.</span></span> <span data-ttu-id="fa402-186">Gültige Werte: 0 bis 24.</span><span class="sxs-lookup"><span data-stu-id="fa402-186">Valid values 0 to 24</span></span>|
|<span data-ttu-id="fa402-187">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="fa402-187">osMinimumVersion</span></span>|<span data-ttu-id="fa402-188">String</span><span class="sxs-lookup"><span data-stu-id="fa402-188">String</span></span>|<span data-ttu-id="fa402-189">Mindestversion von Windows 8.1</span><span class="sxs-lookup"><span data-stu-id="fa402-189">Minimum Windows 8.1 version.</span></span>|
|<span data-ttu-id="fa402-190">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="fa402-190">osMaximumVersion</span></span>|<span data-ttu-id="fa402-191">String</span><span class="sxs-lookup"><span data-stu-id="fa402-191">String</span></span>|<span data-ttu-id="fa402-192">Maximalversion von Windows 8.1</span><span class="sxs-lookup"><span data-stu-id="fa402-192">Maximum Windows 8.1 version.</span></span>|
|<span data-ttu-id="fa402-193">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="fa402-193">storageRequireEncryption</span></span>|<span data-ttu-id="fa402-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="fa402-194">Boolean</span></span>|<span data-ttu-id="fa402-195">Gibt an, ob für ein Windows 8.1-Gerät Verschlüsselung gefordert wird.</span><span class="sxs-lookup"><span data-stu-id="fa402-195">Indicates whether or not to require encryption on a windows 8.1 device.</span></span>|



## <a name="response"></a><span data-ttu-id="fa402-196">Antwort</span><span class="sxs-lookup"><span data-stu-id="fa402-196">Response</span></span>
<span data-ttu-id="fa402-197">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte  [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fa402-197">If successful, this method returns a `200 OK` response code and an updated [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fa402-198">Beispiel</span><span class="sxs-lookup"><span data-stu-id="fa402-198">Example</span></span>
### <a name="request"></a><span data-ttu-id="fa402-199">Anforderung</span><span class="sxs-lookup"><span data-stu-id="fa402-199">Request</span></span>
<span data-ttu-id="fa402-200">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="fa402-200">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="fa402-201">Antwort</span><span class="sxs-lookup"><span data-stu-id="fa402-201">Response</span></span>
<span data-ttu-id="fa402-p112">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fa402-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





