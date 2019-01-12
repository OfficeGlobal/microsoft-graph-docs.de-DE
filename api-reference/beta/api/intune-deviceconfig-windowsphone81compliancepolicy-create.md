---
title: windowsPhone81CompliancePolicy erstellen
description: Erstellen eines neuen windowsPhone81CompliancePolicy-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8c03ca815b01c2b05d26c9a642a09d54005005e7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27929963"
---
# <a name="create-windowsphone81compliancepolicy"></a><span data-ttu-id="8ad77-103">windowsPhone81CompliancePolicy erstellen</span><span class="sxs-lookup"><span data-stu-id="8ad77-103">Create windowsPhone81CompliancePolicy</span></span>

> <span data-ttu-id="8ad77-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="8ad77-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8ad77-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8ad77-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8ad77-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="8ad77-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8ad77-107">Erstellen eines neuen [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="8ad77-107">Create a new [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8ad77-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="8ad77-108">Prerequisites</span></span>
<span data-ttu-id="8ad77-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8ad77-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8ad77-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8ad77-111">Permission type</span></span>|<span data-ttu-id="8ad77-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8ad77-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8ad77-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8ad77-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8ad77-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8ad77-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8ad77-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8ad77-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8ad77-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8ad77-116">Not supported.</span></span>|
|<span data-ttu-id="8ad77-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8ad77-117">Application</span></span>|<span data-ttu-id="8ad77-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8ad77-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8ad77-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8ad77-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="8ad77-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8ad77-120">Request headers</span></span>
|<span data-ttu-id="8ad77-121">Header</span><span class="sxs-lookup"><span data-stu-id="8ad77-121">Header</span></span>|<span data-ttu-id="8ad77-122">Wert</span><span class="sxs-lookup"><span data-stu-id="8ad77-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8ad77-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8ad77-123">Authorization</span></span>|<span data-ttu-id="8ad77-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="8ad77-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8ad77-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="8ad77-125">Accept</span></span>|<span data-ttu-id="8ad77-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8ad77-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8ad77-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8ad77-127">Request body</span></span>
<span data-ttu-id="8ad77-128">Geben Sie im Anforderungstext eine JSON-Darstellung des windowsPhone81CompliancePolicy-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="8ad77-128">In the request body, supply a JSON representation for the windowsPhone81CompliancePolicy object.</span></span>

<span data-ttu-id="8ad77-129">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der windowsPhone81CompliancePolicy erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="8ad77-129">The following table shows the properties that are required when you create the windowsPhone81CompliancePolicy.</span></span>

|<span data-ttu-id="8ad77-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8ad77-130">Property</span></span>|<span data-ttu-id="8ad77-131">Typ</span><span class="sxs-lookup"><span data-stu-id="8ad77-131">Type</span></span>|<span data-ttu-id="8ad77-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8ad77-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8ad77-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8ad77-133">roleScopeTagIds</span></span>|<span data-ttu-id="8ad77-134">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="8ad77-134">String collection</span></span>|<span data-ttu-id="8ad77-135">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="8ad77-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="8ad77-136">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="8ad77-136">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="8ad77-137">id</span><span class="sxs-lookup"><span data-stu-id="8ad77-137">id</span></span>|<span data-ttu-id="8ad77-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8ad77-138">String</span></span>|<span data-ttu-id="8ad77-139">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="8ad77-139">Key of the entity.</span></span> <span data-ttu-id="8ad77-140">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="8ad77-140">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="8ad77-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8ad77-141">createdDateTime</span></span>|<span data-ttu-id="8ad77-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8ad77-142">DateTimeOffset</span></span>|<span data-ttu-id="8ad77-143">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="8ad77-143">DateTime the object was created.</span></span> <span data-ttu-id="8ad77-144">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="8ad77-144">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="8ad77-145">description</span><span class="sxs-lookup"><span data-stu-id="8ad77-145">description</span></span>|<span data-ttu-id="8ad77-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8ad77-146">String</span></span>|<span data-ttu-id="8ad77-147">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="8ad77-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="8ad77-148">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="8ad77-148">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="8ad77-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8ad77-149">lastModifiedDateTime</span></span>|<span data-ttu-id="8ad77-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8ad77-150">DateTimeOffset</span></span>|<span data-ttu-id="8ad77-151">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="8ad77-151">DateTime the object was last modified.</span></span> <span data-ttu-id="8ad77-152">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="8ad77-152">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="8ad77-153">displayName</span><span class="sxs-lookup"><span data-stu-id="8ad77-153">displayName</span></span>|<span data-ttu-id="8ad77-154">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8ad77-154">String</span></span>|<span data-ttu-id="8ad77-155">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="8ad77-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="8ad77-156">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="8ad77-156">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="8ad77-157">Version</span><span class="sxs-lookup"><span data-stu-id="8ad77-157">version</span></span>|<span data-ttu-id="8ad77-158">Int32</span><span class="sxs-lookup"><span data-stu-id="8ad77-158">Int32</span></span>|<span data-ttu-id="8ad77-159">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="8ad77-159">Version of the device configuration.</span></span> <span data-ttu-id="8ad77-160">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="8ad77-160">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="8ad77-161">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="8ad77-161">passwordBlockSimple</span></span>|<span data-ttu-id="8ad77-162">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="8ad77-162">Boolean</span></span>|<span data-ttu-id="8ad77-163">Gibt an, ob die Kalendersynchronisierung blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="8ad77-163">Whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="8ad77-164">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="8ad77-164">passwordExpirationDays</span></span>|<span data-ttu-id="8ad77-165">Int32</span><span class="sxs-lookup"><span data-stu-id="8ad77-165">Int32</span></span>|<span data-ttu-id="8ad77-166">Zeit in Tagen bis zum Ablaufen des Kennworts.</span><span class="sxs-lookup"><span data-stu-id="8ad77-166">Number of days before the password expires.</span></span>|
|<span data-ttu-id="8ad77-167">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="8ad77-167">passwordMinimumLength</span></span>|<span data-ttu-id="8ad77-168">Int32</span><span class="sxs-lookup"><span data-stu-id="8ad77-168">Int32</span></span>|<span data-ttu-id="8ad77-169">Mindestlänge von Kennwörtern</span><span class="sxs-lookup"><span data-stu-id="8ad77-169">Minimum length of passwords.</span></span>|
|<span data-ttu-id="8ad77-170">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="8ad77-170">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="8ad77-171">Int32</span><span class="sxs-lookup"><span data-stu-id="8ad77-171">Int32</span></span>|<span data-ttu-id="8ad77-172">Zeitraum von Inaktivität in Minuten, nach dem die Eingabe eines Kennworts gefordert wird</span><span class="sxs-lookup"><span data-stu-id="8ad77-172">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="8ad77-173">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="8ad77-173">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="8ad77-174">Int32</span><span class="sxs-lookup"><span data-stu-id="8ad77-174">Int32</span></span>|<span data-ttu-id="8ad77-175">Anzahl der Zeichensätze, die im Kennwort enthalten sein müssen</span><span class="sxs-lookup"><span data-stu-id="8ad77-175">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="8ad77-176">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="8ad77-176">passwordRequiredType</span></span>|[<span data-ttu-id="8ad77-177">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="8ad77-177">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="8ad77-178">Geforderter Kennworttyp.</span><span class="sxs-lookup"><span data-stu-id="8ad77-178">The required password type.</span></span> <span data-ttu-id="8ad77-179">Mögliche Werte sind: `deviceDefault`, `alphanumeric` und `numeric`.</span><span class="sxs-lookup"><span data-stu-id="8ad77-179">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="8ad77-180">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="8ad77-180">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="8ad77-181">Int32</span><span class="sxs-lookup"><span data-stu-id="8ad77-181">Int32</span></span>|<span data-ttu-id="8ad77-182">Anzahl der zuletzt verwendeten Kennwörter, die nicht erneut verwendet werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="8ad77-182">Number of previous passwords to block.</span></span> <span data-ttu-id="8ad77-183">Gültige Werte: 0 bis 24.</span><span class="sxs-lookup"><span data-stu-id="8ad77-183">Valid values 0 to 24</span></span>|
|<span data-ttu-id="8ad77-184">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="8ad77-184">passwordRequired</span></span>|<span data-ttu-id="8ad77-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="8ad77-185">Boolean</span></span>|<span data-ttu-id="8ad77-186">Legt fest, ob ein Kennwort gefordert wird.</span><span class="sxs-lookup"><span data-stu-id="8ad77-186">Whether or not to require a password.</span></span>|
|<span data-ttu-id="8ad77-187">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="8ad77-187">osMinimumVersion</span></span>|<span data-ttu-id="8ad77-188">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8ad77-188">String</span></span>|<span data-ttu-id="8ad77-189">Mindestversion von Windows Phone</span><span class="sxs-lookup"><span data-stu-id="8ad77-189">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="8ad77-190">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="8ad77-190">osMaximumVersion</span></span>|<span data-ttu-id="8ad77-191">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8ad77-191">String</span></span>|<span data-ttu-id="8ad77-192">Maximalversion von Windows Phone</span><span class="sxs-lookup"><span data-stu-id="8ad77-192">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="8ad77-193">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="8ad77-193">storageRequireEncryption</span></span>|<span data-ttu-id="8ad77-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="8ad77-194">Boolean</span></span>|<span data-ttu-id="8ad77-195">Legt fest, dass auf Windows Phone-Geräten Verschlüsselung gefordert wird.</span><span class="sxs-lookup"><span data-stu-id="8ad77-195">Require encryption on windows phone devices.</span></span>|



## <a name="response"></a><span data-ttu-id="8ad77-196">Antwort</span><span class="sxs-lookup"><span data-stu-id="8ad77-196">Response</span></span>
<span data-ttu-id="8ad77-197">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="8ad77-197">If successful, this method returns a `201 Created` response code and a [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8ad77-198">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8ad77-198">Example</span></span>
### <a name="request"></a><span data-ttu-id="8ad77-199">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8ad77-199">Request</span></span>
<span data-ttu-id="8ad77-200">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8ad77-200">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 733

{
  "@odata.type": "#microsoft.graph.windowsPhone81CompliancePolicy",
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

### <a name="response"></a><span data-ttu-id="8ad77-201">Antwort</span><span class="sxs-lookup"><span data-stu-id="8ad77-201">Response</span></span>
<span data-ttu-id="8ad77-p112">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8ad77-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





