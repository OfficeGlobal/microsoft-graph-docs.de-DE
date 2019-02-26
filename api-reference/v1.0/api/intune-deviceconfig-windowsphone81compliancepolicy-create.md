---
title: windowsPhone81CompliancePolicy erstellen
description: Erstellen eines neuen windowsPhone81CompliancePolicy-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a71c679916574b51966207df93bbe12b62b27a57
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30257309"
---
# <a name="create-windowsphone81compliancepolicy"></a><span data-ttu-id="f1e82-103">windowsPhone81CompliancePolicy erstellen</span><span class="sxs-lookup"><span data-stu-id="f1e82-103">Create windowsPhone81CompliancePolicy</span></span>

> <span data-ttu-id="f1e82-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="f1e82-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f1e82-105">Erstellen eines neuen [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="f1e82-105">Create a new [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f1e82-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f1e82-106">Prerequisites</span></span>
<span data-ttu-id="f1e82-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="f1e82-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f1e82-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f1e82-109">Permission type</span></span>|<span data-ttu-id="f1e82-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f1e82-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f1e82-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f1e82-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f1e82-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1e82-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f1e82-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f1e82-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f1e82-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f1e82-114">Not supported.</span></span>|
|<span data-ttu-id="f1e82-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f1e82-115">Application</span></span>|<span data-ttu-id="f1e82-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f1e82-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f1e82-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f1e82-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="f1e82-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f1e82-118">Request headers</span></span>
|<span data-ttu-id="f1e82-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="f1e82-119">Header</span></span>|<span data-ttu-id="f1e82-120">Wert</span><span class="sxs-lookup"><span data-stu-id="f1e82-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f1e82-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f1e82-121">Authorization</span></span>|<span data-ttu-id="f1e82-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="f1e82-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f1e82-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="f1e82-123">Accept</span></span>|<span data-ttu-id="f1e82-124">application/json</span><span class="sxs-lookup"><span data-stu-id="f1e82-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f1e82-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f1e82-125">Request body</span></span>
<span data-ttu-id="f1e82-126">Geben Sie im Anforderungstext eine JSON-Darstellung des windowsPhone81CompliancePolicy-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="f1e82-126">In the request body, supply a JSON representation for the windowsPhone81CompliancePolicy object.</span></span>

<span data-ttu-id="f1e82-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der windowsPhone81CompliancePolicy erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="f1e82-127">The following table shows the properties that are required when you create the windowsPhone81CompliancePolicy.</span></span>

|<span data-ttu-id="f1e82-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f1e82-128">Property</span></span>|<span data-ttu-id="f1e82-129">Typ</span><span class="sxs-lookup"><span data-stu-id="f1e82-129">Type</span></span>|<span data-ttu-id="f1e82-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f1e82-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1e82-131">id</span><span class="sxs-lookup"><span data-stu-id="f1e82-131">id</span></span>|<span data-ttu-id="f1e82-132">string</span><span class="sxs-lookup"><span data-stu-id="f1e82-132">String</span></span>|<span data-ttu-id="f1e82-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="f1e82-133">Key of the entity.</span></span> <span data-ttu-id="f1e82-134">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f1e82-134">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f1e82-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f1e82-135">createdDateTime</span></span>|<span data-ttu-id="f1e82-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f1e82-136">DateTimeOffset</span></span>|<span data-ttu-id="f1e82-137">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="f1e82-137">DateTime the object was created.</span></span> <span data-ttu-id="f1e82-138">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f1e82-138">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f1e82-139">description</span><span class="sxs-lookup"><span data-stu-id="f1e82-139">description</span></span>|<span data-ttu-id="f1e82-140">String</span><span class="sxs-lookup"><span data-stu-id="f1e82-140">String</span></span>|<span data-ttu-id="f1e82-141">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="f1e82-141">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f1e82-142">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f1e82-142">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f1e82-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f1e82-143">lastModifiedDateTime</span></span>|<span data-ttu-id="f1e82-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f1e82-144">DateTimeOffset</span></span>|<span data-ttu-id="f1e82-145">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="f1e82-145">DateTime the object was last modified.</span></span> <span data-ttu-id="f1e82-146">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f1e82-146">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f1e82-147">displayName</span><span class="sxs-lookup"><span data-stu-id="f1e82-147">displayName</span></span>|<span data-ttu-id="f1e82-148">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f1e82-148">String</span></span>|<span data-ttu-id="f1e82-149">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="f1e82-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f1e82-150">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f1e82-150">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f1e82-151">Version</span><span class="sxs-lookup"><span data-stu-id="f1e82-151">version</span></span>|<span data-ttu-id="f1e82-152">Int32</span><span class="sxs-lookup"><span data-stu-id="f1e82-152">Int32</span></span>|<span data-ttu-id="f1e82-153">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="f1e82-153">Version of the device configuration.</span></span> <span data-ttu-id="f1e82-154">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f1e82-154">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f1e82-155">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="f1e82-155">passwordBlockSimple</span></span>|<span data-ttu-id="f1e82-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="f1e82-156">Boolean</span></span>|<span data-ttu-id="f1e82-157">Gibt an, ob die Kalendersynchronisierung blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="f1e82-157">Whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="f1e82-158">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="f1e82-158">passwordExpirationDays</span></span>|<span data-ttu-id="f1e82-159">Int32</span><span class="sxs-lookup"><span data-stu-id="f1e82-159">Int32</span></span>|<span data-ttu-id="f1e82-160">Zeit in Tagen bis zum Ablaufen des Kennworts.</span><span class="sxs-lookup"><span data-stu-id="f1e82-160">Number of days before the password expires.</span></span>|
|<span data-ttu-id="f1e82-161">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="f1e82-161">passwordMinimumLength</span></span>|<span data-ttu-id="f1e82-162">Int32</span><span class="sxs-lookup"><span data-stu-id="f1e82-162">Int32</span></span>|<span data-ttu-id="f1e82-163">Mindestlänge von Kennwörtern</span><span class="sxs-lookup"><span data-stu-id="f1e82-163">Minimum length of passwords.</span></span>|
|<span data-ttu-id="f1e82-164">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="f1e82-164">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="f1e82-165">Int32</span><span class="sxs-lookup"><span data-stu-id="f1e82-165">Int32</span></span>|<span data-ttu-id="f1e82-166">Zeitraum von Inaktivität in Minuten, nach dem die Eingabe eines Kennworts gefordert wird</span><span class="sxs-lookup"><span data-stu-id="f1e82-166">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="f1e82-167">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="f1e82-167">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="f1e82-168">Int32</span><span class="sxs-lookup"><span data-stu-id="f1e82-168">Int32</span></span>|<span data-ttu-id="f1e82-169">Anzahl der Zeichensätze, die im Kennwort enthalten sein müssen</span><span class="sxs-lookup"><span data-stu-id="f1e82-169">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="f1e82-170">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="f1e82-170">passwordRequiredType</span></span>|[<span data-ttu-id="f1e82-171">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="f1e82-171">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="f1e82-172">Geforderter Kennworttyp.</span><span class="sxs-lookup"><span data-stu-id="f1e82-172">The required password type.</span></span> <span data-ttu-id="f1e82-173">Mögliche Werte sind: `deviceDefault`, `alphanumeric` und `numeric`.</span><span class="sxs-lookup"><span data-stu-id="f1e82-173">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="f1e82-174">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="f1e82-174">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="f1e82-175">Int32</span><span class="sxs-lookup"><span data-stu-id="f1e82-175">Int32</span></span>|<span data-ttu-id="f1e82-176">Anzahl der zuletzt verwendeten Kennwörter, die nicht erneut verwendet werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="f1e82-176">Number of previous passwords to block.</span></span> <span data-ttu-id="f1e82-177">Gültige Werte: 0 bis 24.</span><span class="sxs-lookup"><span data-stu-id="f1e82-177">Valid values 0 to 24</span></span>|
|<span data-ttu-id="f1e82-178">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="f1e82-178">passwordRequired</span></span>|<span data-ttu-id="f1e82-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="f1e82-179">Boolean</span></span>|<span data-ttu-id="f1e82-180">Legt fest, ob ein Kennwort gefordert wird.</span><span class="sxs-lookup"><span data-stu-id="f1e82-180">Whether or not to require a password.</span></span>|
|<span data-ttu-id="f1e82-181">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="f1e82-181">osMinimumVersion</span></span>|<span data-ttu-id="f1e82-182">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f1e82-182">String</span></span>|<span data-ttu-id="f1e82-183">Mindestversion von Windows Phone</span><span class="sxs-lookup"><span data-stu-id="f1e82-183">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="f1e82-184">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="f1e82-184">osMaximumVersion</span></span>|<span data-ttu-id="f1e82-185">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f1e82-185">String</span></span>|<span data-ttu-id="f1e82-186">Maximalversion von Windows Phone</span><span class="sxs-lookup"><span data-stu-id="f1e82-186">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="f1e82-187">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="f1e82-187">storageRequireEncryption</span></span>|<span data-ttu-id="f1e82-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="f1e82-188">Boolean</span></span>|<span data-ttu-id="f1e82-189">Legt fest, dass auf Windows Phone-Geräten Verschlüsselung gefordert wird.</span><span class="sxs-lookup"><span data-stu-id="f1e82-189">Require encryption on windows phone devices.</span></span>|



## <a name="response"></a><span data-ttu-id="f1e82-190">Antwort</span><span class="sxs-lookup"><span data-stu-id="f1e82-190">Response</span></span>
<span data-ttu-id="f1e82-191">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="f1e82-191">If successful, this method returns a `201 Created` response code and a [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f1e82-192">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f1e82-192">Example</span></span>

### <a name="request"></a><span data-ttu-id="f1e82-193">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f1e82-193">Request</span></span>
<span data-ttu-id="f1e82-194">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f1e82-194">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
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

### <a name="response"></a><span data-ttu-id="f1e82-195">Antwort</span><span class="sxs-lookup"><span data-stu-id="f1e82-195">Response</span></span>
<span data-ttu-id="f1e82-p110">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f1e82-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



