---
title: deviceEnrollmentWindowsHelloForBusinessConfiguration aktualisieren
description: Aktualisieren der Eigenschaften eines deviceEnrollmentWindowsHelloForBusinessConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3225f7fe36f5ec8a66df8424a06d8569b7c92efd
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30968637"
---
# <a name="update-deviceenrollmentwindowshelloforbusinessconfiguration"></a><span data-ttu-id="438cd-103">deviceEnrollmentWindowsHelloForBusinessConfiguration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="438cd-103">Update deviceEnrollmentWindowsHelloForBusinessConfiguration</span></span>

> <span data-ttu-id="438cd-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="438cd-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="438cd-105">Aktualisieren der Eigenschaften eines [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="438cd-105">Update the properties of a [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="438cd-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="438cd-106">Prerequisites</span></span>
<span data-ttu-id="438cd-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="438cd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="438cd-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="438cd-109">Permission type</span></span>|<span data-ttu-id="438cd-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="438cd-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="438cd-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="438cd-111">Delegated (work or school account)</span></span>|<span data-ttu-id="438cd-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="438cd-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="438cd-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="438cd-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="438cd-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="438cd-114">Not supported.</span></span>|
|<span data-ttu-id="438cd-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="438cd-115">Application</span></span>|<span data-ttu-id="438cd-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="438cd-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="438cd-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="438cd-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="438cd-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="438cd-118">Request headers</span></span>
|<span data-ttu-id="438cd-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="438cd-119">Header</span></span>|<span data-ttu-id="438cd-120">Wert</span><span class="sxs-lookup"><span data-stu-id="438cd-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="438cd-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="438cd-121">Authorization</span></span>|<span data-ttu-id="438cd-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="438cd-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="438cd-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="438cd-123">Accept</span></span>|<span data-ttu-id="438cd-124">application/json</span><span class="sxs-lookup"><span data-stu-id="438cd-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="438cd-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="438cd-125">Request body</span></span>
<span data-ttu-id="438cd-126">Geben Sie im Anforderungstext eine JSON-Darstellung für das [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md)-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="438cd-126">In the request body, supply a JSON representation for the [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>

<span data-ttu-id="438cd-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="438cd-127">The following table shows the properties that are required when you create the [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md).</span></span>

|<span data-ttu-id="438cd-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="438cd-128">Property</span></span>|<span data-ttu-id="438cd-129">Typ</span><span class="sxs-lookup"><span data-stu-id="438cd-129">Type</span></span>|<span data-ttu-id="438cd-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="438cd-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="438cd-131">id</span><span class="sxs-lookup"><span data-stu-id="438cd-131">id</span></span>|<span data-ttu-id="438cd-132">String</span><span class="sxs-lookup"><span data-stu-id="438cd-132">String</span></span>|<span data-ttu-id="438cd-133">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="438cd-133">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="438cd-134">displayName</span><span class="sxs-lookup"><span data-stu-id="438cd-134">displayName</span></span>|<span data-ttu-id="438cd-135">String</span><span class="sxs-lookup"><span data-stu-id="438cd-135">String</span></span>|<span data-ttu-id="438cd-136">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="438cd-136">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="438cd-137">description</span><span class="sxs-lookup"><span data-stu-id="438cd-137">description</span></span>|<span data-ttu-id="438cd-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="438cd-138">String</span></span>|<span data-ttu-id="438cd-139">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="438cd-139">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="438cd-140">Priorität</span><span class="sxs-lookup"><span data-stu-id="438cd-140">priority</span></span>|<span data-ttu-id="438cd-141">Int32</span><span class="sxs-lookup"><span data-stu-id="438cd-141">Int32</span></span>|<span data-ttu-id="438cd-142">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="438cd-142">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="438cd-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="438cd-143">createdDateTime</span></span>|<span data-ttu-id="438cd-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="438cd-144">DateTimeOffset</span></span>|<span data-ttu-id="438cd-145">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="438cd-145">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="438cd-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="438cd-146">lastModifiedDateTime</span></span>|<span data-ttu-id="438cd-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="438cd-147">DateTimeOffset</span></span>|<span data-ttu-id="438cd-148">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="438cd-148">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="438cd-149">Version</span><span class="sxs-lookup"><span data-stu-id="438cd-149">version</span></span>|<span data-ttu-id="438cd-150">Int32</span><span class="sxs-lookup"><span data-stu-id="438cd-150">Int32</span></span>|<span data-ttu-id="438cd-151">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="438cd-151">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="438cd-152">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="438cd-152">pinMinimumLength</span></span>|<span data-ttu-id="438cd-153">Int32</span><span class="sxs-lookup"><span data-stu-id="438cd-153">Int32</span></span>|<span data-ttu-id="438cd-154">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="438cd-154">Not yet documented</span></span>|
|<span data-ttu-id="438cd-155">pinMaximumLength</span><span class="sxs-lookup"><span data-stu-id="438cd-155">pinMaximumLength</span></span>|<span data-ttu-id="438cd-156">Int32</span><span class="sxs-lookup"><span data-stu-id="438cd-156">Int32</span></span>|<span data-ttu-id="438cd-157">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="438cd-157">Not yet documented</span></span>|
|<span data-ttu-id="438cd-158">pinUppercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="438cd-158">pinUppercaseCharactersUsage</span></span>|[<span data-ttu-id="438cd-159">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="438cd-159">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="438cd-160">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="438cd-160">Not yet documented.</span></span> <span data-ttu-id="438cd-161">Mögliche Werte sind: `allowed`, `required` und `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="438cd-161">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="438cd-162">pinLowercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="438cd-162">pinLowercaseCharactersUsage</span></span>|[<span data-ttu-id="438cd-163">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="438cd-163">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="438cd-164">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="438cd-164">Not yet documented.</span></span> <span data-ttu-id="438cd-165">Mögliche Werte sind: `allowed`, `required` und `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="438cd-165">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="438cd-166">pinSpecialCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="438cd-166">pinSpecialCharactersUsage</span></span>|[<span data-ttu-id="438cd-167">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="438cd-167">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="438cd-168">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="438cd-168">Not yet documented.</span></span> <span data-ttu-id="438cd-169">Mögliche Werte sind: `allowed`, `required` und `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="438cd-169">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="438cd-170">state</span><span class="sxs-lookup"><span data-stu-id="438cd-170">state</span></span>|[<span data-ttu-id="438cd-171">Aktivierung</span><span class="sxs-lookup"><span data-stu-id="438cd-171">enablement</span></span>](../resources/intune-onboarding-enablement.md)|<span data-ttu-id="438cd-172">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="438cd-172">Not yet documented.</span></span> <span data-ttu-id="438cd-173">Mögliche Werte sind: `notConfigured`, `enabled` und `disabled`.</span><span class="sxs-lookup"><span data-stu-id="438cd-173">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="438cd-174">securityDeviceRequired</span><span class="sxs-lookup"><span data-stu-id="438cd-174">securityDeviceRequired</span></span>|<span data-ttu-id="438cd-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="438cd-175">Boolean</span></span>|<span data-ttu-id="438cd-176">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="438cd-176">Not yet documented</span></span>|
|<span data-ttu-id="438cd-177">unlockWithBiometricsEnabled</span><span class="sxs-lookup"><span data-stu-id="438cd-177">unlockWithBiometricsEnabled</span></span>|<span data-ttu-id="438cd-178">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="438cd-178">Boolean</span></span>|<span data-ttu-id="438cd-179">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="438cd-179">Not yet documented</span></span>|
|<span data-ttu-id="438cd-180">remotePassportEnabled</span><span class="sxs-lookup"><span data-stu-id="438cd-180">remotePassportEnabled</span></span>|<span data-ttu-id="438cd-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="438cd-181">Boolean</span></span>|<span data-ttu-id="438cd-182">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="438cd-182">Not yet documented</span></span>|
|<span data-ttu-id="438cd-183">pinPreviousBlockCount</span><span class="sxs-lookup"><span data-stu-id="438cd-183">pinPreviousBlockCount</span></span>|<span data-ttu-id="438cd-184">Int32</span><span class="sxs-lookup"><span data-stu-id="438cd-184">Int32</span></span>|<span data-ttu-id="438cd-185">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="438cd-185">Not yet documented</span></span>|
|<span data-ttu-id="438cd-186">pinExpirationInDays</span><span class="sxs-lookup"><span data-stu-id="438cd-186">pinExpirationInDays</span></span>|<span data-ttu-id="438cd-187">Int32</span><span class="sxs-lookup"><span data-stu-id="438cd-187">Int32</span></span>|<span data-ttu-id="438cd-188">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="438cd-188">Not yet documented</span></span>|
|<span data-ttu-id="438cd-189">enhancedBiometricsState</span><span class="sxs-lookup"><span data-stu-id="438cd-189">enhancedBiometricsState</span></span>|[<span data-ttu-id="438cd-190">Aktivierung</span><span class="sxs-lookup"><span data-stu-id="438cd-190">enablement</span></span>](../resources/intune-onboarding-enablement.md)|<span data-ttu-id="438cd-191">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="438cd-191">Not yet documented.</span></span> <span data-ttu-id="438cd-192">Mögliche Werte sind: `notConfigured`, `enabled` und `disabled`.</span><span class="sxs-lookup"><span data-stu-id="438cd-192">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|



## <a name="response"></a><span data-ttu-id="438cd-193">Antwort</span><span class="sxs-lookup"><span data-stu-id="438cd-193">Response</span></span>
<span data-ttu-id="438cd-194">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="438cd-194">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="438cd-195">Beispiel</span><span class="sxs-lookup"><span data-stu-id="438cd-195">Example</span></span>

### <a name="request"></a><span data-ttu-id="438cd-196">Anforderung</span><span class="sxs-lookup"><span data-stu-id="438cd-196">Request</span></span>
<span data-ttu-id="438cd-197">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="438cd-197">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
Content-type: application/json
Content-length: 629

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentWindowsHelloForBusinessConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "version": 7,
  "pinMinimumLength": 0,
  "pinMaximumLength": 0,
  "pinUppercaseCharactersUsage": "required",
  "pinLowercaseCharactersUsage": "required",
  "pinSpecialCharactersUsage": "required",
  "state": "enabled",
  "securityDeviceRequired": true,
  "unlockWithBiometricsEnabled": true,
  "remotePassportEnabled": true,
  "pinPreviousBlockCount": 5,
  "pinExpirationInDays": 3,
  "enhancedBiometricsState": "enabled"
}
```

### <a name="response"></a><span data-ttu-id="438cd-198">Antwort</span><span class="sxs-lookup"><span data-stu-id="438cd-198">Response</span></span>
<span data-ttu-id="438cd-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="438cd-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 801

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentWindowsHelloForBusinessConfiguration",
  "id": "3068e0cd-e0cd-3068-cde0-6830cde06830",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": 7,
  "pinMinimumLength": 0,
  "pinMaximumLength": 0,
  "pinUppercaseCharactersUsage": "required",
  "pinLowercaseCharactersUsage": "required",
  "pinSpecialCharactersUsage": "required",
  "state": "enabled",
  "securityDeviceRequired": true,
  "unlockWithBiometricsEnabled": true,
  "remotePassportEnabled": true,
  "pinPreviousBlockCount": 5,
  "pinExpirationInDays": 3,
  "enhancedBiometricsState": "enabled"
}
```



