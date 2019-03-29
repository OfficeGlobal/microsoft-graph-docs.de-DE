---
title: Erstellen von „macOSGeneralDeviceConfiguration“
description: Diese Methode erstellt ein neues Objekt des Typs macOSGeneralDeviceConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e02159e9f577e001a675de5ee64768f63d1090c0
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30979522"
---
# <a name="create-macosgeneraldeviceconfiguration"></a><span data-ttu-id="d9711-103">Erstellen von „macOSGeneralDeviceConfiguration“</span><span class="sxs-lookup"><span data-stu-id="d9711-103">Create macOSGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="d9711-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="d9711-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d9711-105">Diese Methode erstellt ein neues Objekt des Typs [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d9711-105">Create a new [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d9711-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="d9711-106">Prerequisites</span></span>
<span data-ttu-id="d9711-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d9711-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d9711-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d9711-109">Permission type</span></span>|<span data-ttu-id="d9711-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d9711-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d9711-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d9711-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d9711-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9711-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d9711-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d9711-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d9711-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d9711-114">Not supported.</span></span>|
|<span data-ttu-id="d9711-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d9711-115">Application</span></span>|<span data-ttu-id="d9711-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d9711-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d9711-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d9711-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="d9711-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d9711-118">Request headers</span></span>
|<span data-ttu-id="d9711-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="d9711-119">Header</span></span>|<span data-ttu-id="d9711-120">Wert</span><span class="sxs-lookup"><span data-stu-id="d9711-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d9711-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d9711-121">Authorization</span></span>|<span data-ttu-id="d9711-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="d9711-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d9711-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="d9711-123">Accept</span></span>|<span data-ttu-id="d9711-124">application/json</span><span class="sxs-lookup"><span data-stu-id="d9711-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d9711-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d9711-125">Request body</span></span>
<span data-ttu-id="d9711-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „macOSGeneralDeviceConfiguration“ an.</span><span class="sxs-lookup"><span data-stu-id="d9711-126">In the request body, supply a JSON representation for the macOSGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="d9711-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „macOSGeneralDeviceConfiguration“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="d9711-127">The following table shows the properties that are required when you create the macOSGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="d9711-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d9711-128">Property</span></span>|<span data-ttu-id="d9711-129">Typ</span><span class="sxs-lookup"><span data-stu-id="d9711-129">Type</span></span>|<span data-ttu-id="d9711-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d9711-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d9711-131">id</span><span class="sxs-lookup"><span data-stu-id="d9711-131">id</span></span>|<span data-ttu-id="d9711-132">String</span><span class="sxs-lookup"><span data-stu-id="d9711-132">String</span></span>|<span data-ttu-id="d9711-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="d9711-133">Key of the entity.</span></span> <span data-ttu-id="d9711-134">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d9711-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d9711-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d9711-135">lastModifiedDateTime</span></span>|<span data-ttu-id="d9711-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d9711-136">DateTimeOffset</span></span>|<span data-ttu-id="d9711-137">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="d9711-137">DateTime the object was last modified.</span></span> <span data-ttu-id="d9711-138">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d9711-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d9711-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d9711-139">createdDateTime</span></span>|<span data-ttu-id="d9711-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d9711-140">DateTimeOffset</span></span>|<span data-ttu-id="d9711-141">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="d9711-141">DateTime the object was created.</span></span> <span data-ttu-id="d9711-142">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d9711-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d9711-143">description</span><span class="sxs-lookup"><span data-stu-id="d9711-143">description</span></span>|<span data-ttu-id="d9711-144">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d9711-144">String</span></span>|<span data-ttu-id="d9711-145">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="d9711-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d9711-146">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d9711-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d9711-147">displayName</span><span class="sxs-lookup"><span data-stu-id="d9711-147">displayName</span></span>|<span data-ttu-id="d9711-148">String</span><span class="sxs-lookup"><span data-stu-id="d9711-148">String</span></span>|<span data-ttu-id="d9711-149">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="d9711-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d9711-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d9711-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d9711-151">Version</span><span class="sxs-lookup"><span data-stu-id="d9711-151">version</span></span>|<span data-ttu-id="d9711-152">Int32</span><span class="sxs-lookup"><span data-stu-id="d9711-152">Int32</span></span>|<span data-ttu-id="d9711-153">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="d9711-153">Version of the device configuration.</span></span> <span data-ttu-id="d9711-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d9711-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d9711-155">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="d9711-155">compliantAppsList</span></span>|<span data-ttu-id="d9711-156">Collection von Objekten des Typs [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="d9711-156">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="d9711-157">Liste aller Apps, für die die Konformitätsrichtlinie gilt (Zulassungsliste oder Sperrliste, gesteuert über „compliantAppListType“).</span><span class="sxs-lookup"><span data-stu-id="d9711-157">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="d9711-158">Diese Collection darf maximal 10.000 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="d9711-158">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="d9711-159">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="d9711-159">compliantAppListType</span></span>|[<span data-ttu-id="d9711-160">appListType</span><span class="sxs-lookup"><span data-stu-id="d9711-160">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="d9711-161">Typ der in „compliantAppsList“ definierten Liste.</span><span class="sxs-lookup"><span data-stu-id="d9711-161">List that is in the CompliantAppsList.</span></span> <span data-ttu-id="d9711-162">Mögliche Werte sind: `none`, `appsInListCompliant` und `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="d9711-162">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="d9711-163">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="d9711-163">emailInDomainSuffixes</span></span>|<span data-ttu-id="d9711-164">String-Sammlung</span><span class="sxs-lookup"><span data-stu-id="d9711-164">String collection</span></span>|<span data-ttu-id="d9711-165">E-Mail-Adressen, deren Suffix keiner dieser Zeichenfolgen entspricht, gelten als domänenextern.</span><span class="sxs-lookup"><span data-stu-id="d9711-165">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="d9711-166">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="d9711-166">passwordBlockSimple</span></span>|<span data-ttu-id="d9711-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9711-167">Boolean</span></span>|<span data-ttu-id="d9711-168">Unterbindet die Verwendung einfacher Kennwörter.</span><span class="sxs-lookup"><span data-stu-id="d9711-168">Block simple passwords.</span></span>|
|<span data-ttu-id="d9711-169">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="d9711-169">passwordExpirationDays</span></span>|<span data-ttu-id="d9711-170">Int32</span><span class="sxs-lookup"><span data-stu-id="d9711-170">Int32</span></span>|<span data-ttu-id="d9711-171">Zeit in Tagen bis zum Ablaufen des Kennworts</span><span class="sxs-lookup"><span data-stu-id="d9711-171">Number of days before the password expires.</span></span>|
|<span data-ttu-id="d9711-172">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="d9711-172">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="d9711-173">Int32</span><span class="sxs-lookup"><span data-stu-id="d9711-173">Int32</span></span>|<span data-ttu-id="d9711-174">Anzahl von Zeichensätzen, die ein Kennwort enthalten muss.</span><span class="sxs-lookup"><span data-stu-id="d9711-174">Number of character sets a password must contain.</span></span> <span data-ttu-id="d9711-175">Gültige Werte: 0 bis 4.</span><span class="sxs-lookup"><span data-stu-id="d9711-175">Valid values 0 to 4</span></span>|
|<span data-ttu-id="d9711-176">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="d9711-176">passwordMinimumLength</span></span>|<span data-ttu-id="d9711-177">Int32</span><span class="sxs-lookup"><span data-stu-id="d9711-177">Int32</span></span>|<span data-ttu-id="d9711-178">Mindestlänge von Kennwörtern</span><span class="sxs-lookup"><span data-stu-id="d9711-178">Minimum length of passwords.</span></span>|
|<span data-ttu-id="d9711-179">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="d9711-179">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="d9711-180">Int32</span><span class="sxs-lookup"><span data-stu-id="d9711-180">Int32</span></span>|<span data-ttu-id="d9711-181">Zeitraum von Inaktivität in Minuten, nach dem die Eingabe eines Kennworts gefordert wird</span><span class="sxs-lookup"><span data-stu-id="d9711-181">Minutes of inactivity required before a password is required.</span></span>|
|<span data-ttu-id="d9711-182">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="d9711-182">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="d9711-183">Int32</span><span class="sxs-lookup"><span data-stu-id="d9711-183">Int32</span></span>|<span data-ttu-id="d9711-184">Zeitraum von Inaktivität in Minuten, nach dem es zu einem Bildschirmtimeout kommt</span><span class="sxs-lookup"><span data-stu-id="d9711-184">Minutes of inactivity required before the screen times out.</span></span>|
|<span data-ttu-id="d9711-185">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="d9711-185">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="d9711-186">Int32</span><span class="sxs-lookup"><span data-stu-id="d9711-186">Int32</span></span>|<span data-ttu-id="d9711-187">Anzahl der zuletzt verwendeten Kennwörter, die nicht erneut verwendet werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="d9711-187">Number of previous passwords to block.</span></span>|
|<span data-ttu-id="d9711-188">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="d9711-188">passwordRequiredType</span></span>|[<span data-ttu-id="d9711-189">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="d9711-189">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="d9711-190">Geforderter Kennworttyp.</span><span class="sxs-lookup"><span data-stu-id="d9711-190">Type of password that is required.</span></span> <span data-ttu-id="d9711-191">Mögliche Werte sind: `deviceDefault`, `alphanumeric` und `numeric`.</span><span class="sxs-lookup"><span data-stu-id="d9711-191">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="d9711-192">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="d9711-192">passwordRequired</span></span>|<span data-ttu-id="d9711-193">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d9711-193">Boolean</span></span>|<span data-ttu-id="d9711-194">Legt fest, ob ein Kennwort gefordert wird.</span><span class="sxs-lookup"><span data-stu-id="d9711-194">Whether or not to require a password.</span></span>|



## <a name="response"></a><span data-ttu-id="d9711-195">Antwort</span><span class="sxs-lookup"><span data-stu-id="d9711-195">Response</span></span>
<span data-ttu-id="d9711-196">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="d9711-196">If successful, this method returns a `201 Created` response code and a [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d9711-197">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d9711-197">Example</span></span>

### <a name="request"></a><span data-ttu-id="d9711-198">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d9711-198">Request</span></span>
<span data-ttu-id="d9711-199">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d9711-199">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="d9711-200">Antwort</span><span class="sxs-lookup"><span data-stu-id="d9711-200">Response</span></span>
<span data-ttu-id="d9711-p112">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d9711-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



