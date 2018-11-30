---
title: macOSGeneralDeviceConfiguration aktualisieren
description: Aktualisiert die Eigenschaften von Objekten des Typs macOSGeneralDeviceConfiguration.
ms.openlocfilehash: a2ed3f7aa939f7df18389306cc840e3afdcaf856
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27015988"
---
# <a name="update-macosgeneraldeviceconfiguration"></a><span data-ttu-id="bfda6-103">macOSGeneralDeviceConfiguration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="bfda6-103">Update macOSGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="bfda6-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="bfda6-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bfda6-105">Aktualisiert die Eigenschaften von Objekten des Typs [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bfda6-105">Update the properties of a [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="bfda6-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="bfda6-106">Prerequisites</span></span>
<span data-ttu-id="bfda6-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bfda6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bfda6-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="bfda6-109">Permission type</span></span>|<span data-ttu-id="bfda6-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="bfda6-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bfda6-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="bfda6-111">Delegated (work or school account)</span></span>|<span data-ttu-id="bfda6-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bfda6-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bfda6-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="bfda6-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bfda6-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bfda6-114">Not supported.</span></span>|
|<span data-ttu-id="bfda6-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="bfda6-115">Application</span></span>|<span data-ttu-id="bfda6-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bfda6-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bfda6-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="bfda6-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="bfda6-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="bfda6-118">Request headers</span></span>
|<span data-ttu-id="bfda6-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="bfda6-119">Header</span></span>|<span data-ttu-id="bfda6-120">Wert</span><span class="sxs-lookup"><span data-stu-id="bfda6-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bfda6-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="bfda6-121">Authorization</span></span>|<span data-ttu-id="bfda6-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="bfda6-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bfda6-123">Accept</span><span class="sxs-lookup"><span data-stu-id="bfda6-123">Accept</span></span>|<span data-ttu-id="bfda6-124">application/json</span><span class="sxs-lookup"><span data-stu-id="bfda6-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bfda6-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="bfda6-125">Request body</span></span>
<span data-ttu-id="bfda6-126">Geben Sie im Anforderungstext eine JSON-Darstellung des [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="bfda6-126">In the request body, supply a JSON representation for the [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="bfda6-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="bfda6-127">The following table shows the properties that are required when you create the [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="bfda6-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="bfda6-128">Property</span></span>|<span data-ttu-id="bfda6-129">Typ</span><span class="sxs-lookup"><span data-stu-id="bfda6-129">Type</span></span>|<span data-ttu-id="bfda6-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bfda6-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bfda6-131">id</span><span class="sxs-lookup"><span data-stu-id="bfda6-131">id</span></span>|<span data-ttu-id="bfda6-132">String</span><span class="sxs-lookup"><span data-stu-id="bfda6-132">String</span></span>|<span data-ttu-id="bfda6-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="bfda6-133">Key of the entity.</span></span> <span data-ttu-id="bfda6-134">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bfda6-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bfda6-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bfda6-135">lastModifiedDateTime</span></span>|<span data-ttu-id="bfda6-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bfda6-136">DateTimeOffset</span></span>|<span data-ttu-id="bfda6-137">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="bfda6-137">DateTime the object was last modified.</span></span> <span data-ttu-id="bfda6-138">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bfda6-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bfda6-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bfda6-139">createdDateTime</span></span>|<span data-ttu-id="bfda6-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bfda6-140">DateTimeOffset</span></span>|<span data-ttu-id="bfda6-141">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="bfda6-141">DateTime the object was created.</span></span> <span data-ttu-id="bfda6-142">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bfda6-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bfda6-143">description</span><span class="sxs-lookup"><span data-stu-id="bfda6-143">description</span></span>|<span data-ttu-id="bfda6-144">String</span><span class="sxs-lookup"><span data-stu-id="bfda6-144">String</span></span>|<span data-ttu-id="bfda6-145">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="bfda6-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="bfda6-146">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bfda6-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bfda6-147">displayName</span><span class="sxs-lookup"><span data-stu-id="bfda6-147">displayName</span></span>|<span data-ttu-id="bfda6-148">String</span><span class="sxs-lookup"><span data-stu-id="bfda6-148">String</span></span>|<span data-ttu-id="bfda6-149">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="bfda6-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="bfda6-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bfda6-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bfda6-151">Version</span><span class="sxs-lookup"><span data-stu-id="bfda6-151">version</span></span>|<span data-ttu-id="bfda6-152">Int32</span><span class="sxs-lookup"><span data-stu-id="bfda6-152">Int32</span></span>|<span data-ttu-id="bfda6-153">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="bfda6-153">Version of the device configuration.</span></span> <span data-ttu-id="bfda6-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bfda6-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bfda6-155">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="bfda6-155">compliantAppsList</span></span>|<span data-ttu-id="bfda6-156">Collection von Objekten des Typs [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="bfda6-156">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="bfda6-157">Liste aller Apps, für die die Konformitätsrichtlinie gilt (Zulassungsliste oder Sperrliste, gesteuert über „compliantAppListType“).</span><span class="sxs-lookup"><span data-stu-id="bfda6-157">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="bfda6-158">Diese Collection darf maximal 10.000 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="bfda6-158">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="bfda6-159">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="bfda6-159">compliantAppListType</span></span>|[<span data-ttu-id="bfda6-160">appListType</span><span class="sxs-lookup"><span data-stu-id="bfda6-160">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="bfda6-161">Typ der in „compliantAppsList“ definierten Liste.</span><span class="sxs-lookup"><span data-stu-id="bfda6-161">List that is in the CompliantAppsList.</span></span> <span data-ttu-id="bfda6-162">Mögliche Werte sind: `none`, `appsInListCompliant` und `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="bfda6-162">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="bfda6-163">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="bfda6-163">emailInDomainSuffixes</span></span>|<span data-ttu-id="bfda6-164">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="bfda6-164">String collection</span></span>|<span data-ttu-id="bfda6-165">E-Mail-Adressen, deren Suffix keiner dieser Zeichenfolgen entspricht, gelten als domänenextern.</span><span class="sxs-lookup"><span data-stu-id="bfda6-165">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="bfda6-166">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="bfda6-166">passwordBlockSimple</span></span>|<span data-ttu-id="bfda6-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="bfda6-167">Boolean</span></span>|<span data-ttu-id="bfda6-168">Unterbindet die Verwendung einfacher Kennwörter.</span><span class="sxs-lookup"><span data-stu-id="bfda6-168">Block simple passwords.</span></span>|
|<span data-ttu-id="bfda6-169">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="bfda6-169">passwordExpirationDays</span></span>|<span data-ttu-id="bfda6-170">Int32</span><span class="sxs-lookup"><span data-stu-id="bfda6-170">Int32</span></span>|<span data-ttu-id="bfda6-171">Zeit in Tagen bis zum Ablaufen des Kennworts</span><span class="sxs-lookup"><span data-stu-id="bfda6-171">Number of days before the password expires.</span></span>|
|<span data-ttu-id="bfda6-172">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="bfda6-172">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="bfda6-173">Int32</span><span class="sxs-lookup"><span data-stu-id="bfda6-173">Int32</span></span>|<span data-ttu-id="bfda6-174">Anzahl von Zeichensätzen, die ein Kennwort enthalten muss.</span><span class="sxs-lookup"><span data-stu-id="bfda6-174">Number of character sets a password must contain.</span></span> <span data-ttu-id="bfda6-175">Gültige Werte: 0 bis 4.</span><span class="sxs-lookup"><span data-stu-id="bfda6-175">Valid values 0 to 4</span></span>|
|<span data-ttu-id="bfda6-176">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="bfda6-176">passwordMinimumLength</span></span>|<span data-ttu-id="bfda6-177">Int32</span><span class="sxs-lookup"><span data-stu-id="bfda6-177">Int32</span></span>|<span data-ttu-id="bfda6-178">Mindestlänge von Kennwörtern</span><span class="sxs-lookup"><span data-stu-id="bfda6-178">Minimum length of passwords.</span></span>|
|<span data-ttu-id="bfda6-179">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="bfda6-179">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="bfda6-180">Int32</span><span class="sxs-lookup"><span data-stu-id="bfda6-180">Int32</span></span>|<span data-ttu-id="bfda6-181">Zeitraum von Inaktivität in Minuten, nach dem die Eingabe eines Kennworts gefordert wird</span><span class="sxs-lookup"><span data-stu-id="bfda6-181">Minutes of inactivity required before a password is required.</span></span>|
|<span data-ttu-id="bfda6-182">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="bfda6-182">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="bfda6-183">Int32</span><span class="sxs-lookup"><span data-stu-id="bfda6-183">Int32</span></span>|<span data-ttu-id="bfda6-184">Zeitraum von Inaktivität in Minuten, nach dem es zu einem Bildschirmtimeout kommt</span><span class="sxs-lookup"><span data-stu-id="bfda6-184">Minutes of inactivity required before the screen times out.</span></span>|
|<span data-ttu-id="bfda6-185">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="bfda6-185">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="bfda6-186">Int32</span><span class="sxs-lookup"><span data-stu-id="bfda6-186">Int32</span></span>|<span data-ttu-id="bfda6-187">Anzahl der zuletzt verwendeten Kennwörter, die nicht erneut verwendet werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="bfda6-187">Number of previous passwords to block.</span></span>|
|<span data-ttu-id="bfda6-188">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="bfda6-188">passwordRequiredType</span></span>|[<span data-ttu-id="bfda6-189">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="bfda6-189">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="bfda6-190">Geforderter Kennworttyp.</span><span class="sxs-lookup"><span data-stu-id="bfda6-190">Type of password that is required.</span></span> <span data-ttu-id="bfda6-191">Mögliche Werte sind: `deviceDefault`, `alphanumeric` und `numeric`.</span><span class="sxs-lookup"><span data-stu-id="bfda6-191">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="bfda6-192">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="bfda6-192">passwordRequired</span></span>|<span data-ttu-id="bfda6-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="bfda6-193">Boolean</span></span>|<span data-ttu-id="bfda6-194">Legt fest, ob ein Kennwort gefordert wird.</span><span class="sxs-lookup"><span data-stu-id="bfda6-194">Whether or not to require a password.</span></span>|



## <a name="response"></a><span data-ttu-id="bfda6-195">Antwort</span><span class="sxs-lookup"><span data-stu-id="bfda6-195">Response</span></span>
<span data-ttu-id="bfda6-196">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="bfda6-196">If successful, this method returns a `200 OK` response code and an updated [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bfda6-197">Beispiel</span><span class="sxs-lookup"><span data-stu-id="bfda6-197">Example</span></span>
### <a name="request"></a><span data-ttu-id="bfda6-198">Anforderung</span><span class="sxs-lookup"><span data-stu-id="bfda6-198">Request</span></span>
<span data-ttu-id="bfda6-199">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="bfda6-199">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 906

{
  "@odata.type": "#microsoft.graph.macOSGeneralDeviceConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "compliantAppsList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "compliantAppListType": "appsInListCompliant",
  "emailInDomainSuffixes": [
    "Email In Domain Suffixes value"
  ],
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumCharacterSetCount": 0,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequiredType": "alphanumeric",
  "passwordRequired": true
}
```

### <a name="response"></a><span data-ttu-id="bfda6-200">Antwort</span><span class="sxs-lookup"><span data-stu-id="bfda6-200">Response</span></span>
<span data-ttu-id="bfda6-p112">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="bfda6-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1078

{
  "@odata.type": "#microsoft.graph.macOSGeneralDeviceConfiguration",
  "id": "dc356aee-6aee-dc35-ee6a-35dcee6a35dc",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "compliantAppsList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "compliantAppListType": "appsInListCompliant",
  "emailInDomainSuffixes": [
    "Email In Domain Suffixes value"
  ],
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumCharacterSetCount": 0,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequiredType": "alphanumeric",
  "passwordRequired": true
}
```



