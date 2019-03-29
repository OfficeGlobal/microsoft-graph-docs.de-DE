---
title: deviceEnrollmentWindowsHelloForBusinessConfiguration aktualisieren
description: Aktualisieren der Eigenschaften eines deviceEnrollmentWindowsHelloForBusinessConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9a9cd26f0a57df1e46f15ddf80599dd275c2adcf
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30956877"
---
# <a name="update-deviceenrollmentwindowshelloforbusinessconfiguration"></a><span data-ttu-id="a35ae-103">deviceEnrollmentWindowsHelloForBusinessConfiguration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="a35ae-103">Update deviceEnrollmentWindowsHelloForBusinessConfiguration</span></span>

> <span data-ttu-id="a35ae-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a35ae-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a35ae-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="a35ae-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a35ae-106">Aktualisieren der Eigenschaften eines [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="a35ae-106">Update the properties of a [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a35ae-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="a35ae-107">Prerequisites</span></span>
<span data-ttu-id="a35ae-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a35ae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a35ae-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a35ae-110">Permission type</span></span>|<span data-ttu-id="a35ae-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a35ae-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a35ae-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a35ae-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a35ae-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a35ae-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="a35ae-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a35ae-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a35ae-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a35ae-115">Not supported.</span></span>|
|<span data-ttu-id="a35ae-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a35ae-116">Application</span></span>|<span data-ttu-id="a35ae-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a35ae-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a35ae-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a35ae-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="a35ae-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a35ae-119">Request headers</span></span>
|<span data-ttu-id="a35ae-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="a35ae-120">Header</span></span>|<span data-ttu-id="a35ae-121">Wert</span><span class="sxs-lookup"><span data-stu-id="a35ae-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a35ae-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a35ae-122">Authorization</span></span>|<span data-ttu-id="a35ae-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="a35ae-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a35ae-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="a35ae-124">Accept</span></span>|<span data-ttu-id="a35ae-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a35ae-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a35ae-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a35ae-126">Request body</span></span>
<span data-ttu-id="a35ae-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md)-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="a35ae-127">In the request body, supply a JSON representation for the [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>

<span data-ttu-id="a35ae-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="a35ae-128">The following table shows the properties that are required when you create the [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md).</span></span>

|<span data-ttu-id="a35ae-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a35ae-129">Property</span></span>|<span data-ttu-id="a35ae-130">Typ</span><span class="sxs-lookup"><span data-stu-id="a35ae-130">Type</span></span>|<span data-ttu-id="a35ae-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a35ae-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a35ae-132">id</span><span class="sxs-lookup"><span data-stu-id="a35ae-132">id</span></span>|<span data-ttu-id="a35ae-133">String</span><span class="sxs-lookup"><span data-stu-id="a35ae-133">String</span></span>|<span data-ttu-id="a35ae-134">ID der von [DeviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) geerbten Konfiguration der Registrierungs Status Seite</span><span class="sxs-lookup"><span data-stu-id="a35ae-134">Id of the Enrollment Status Page configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="a35ae-135">displayName</span><span class="sxs-lookup"><span data-stu-id="a35ae-135">displayName</span></span>|<span data-ttu-id="a35ae-136">String</span><span class="sxs-lookup"><span data-stu-id="a35ae-136">String</span></span>|<span data-ttu-id="a35ae-137">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a35ae-137">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="a35ae-138">description</span><span class="sxs-lookup"><span data-stu-id="a35ae-138">description</span></span>|<span data-ttu-id="a35ae-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a35ae-139">String</span></span>|<span data-ttu-id="a35ae-140">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a35ae-140">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="a35ae-141">Priorität</span><span class="sxs-lookup"><span data-stu-id="a35ae-141">priority</span></span>|<span data-ttu-id="a35ae-142">Int32</span><span class="sxs-lookup"><span data-stu-id="a35ae-142">Int32</span></span>|<span data-ttu-id="a35ae-143">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a35ae-143">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="a35ae-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a35ae-144">createdDateTime</span></span>|<span data-ttu-id="a35ae-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a35ae-145">DateTimeOffset</span></span>|<span data-ttu-id="a35ae-146">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a35ae-146">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="a35ae-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a35ae-147">lastModifiedDateTime</span></span>|<span data-ttu-id="a35ae-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a35ae-148">DateTimeOffset</span></span>|<span data-ttu-id="a35ae-149">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a35ae-149">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="a35ae-150">Version</span><span class="sxs-lookup"><span data-stu-id="a35ae-150">version</span></span>|<span data-ttu-id="a35ae-151">Int32</span><span class="sxs-lookup"><span data-stu-id="a35ae-151">Int32</span></span>|<span data-ttu-id="a35ae-152">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a35ae-152">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="a35ae-153">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="a35ae-153">pinMinimumLength</span></span>|<span data-ttu-id="a35ae-154">Int32</span><span class="sxs-lookup"><span data-stu-id="a35ae-154">Int32</span></span>|<span data-ttu-id="a35ae-155">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="a35ae-155">Not yet documented</span></span>|
|<span data-ttu-id="a35ae-156">pinMaximumLength</span><span class="sxs-lookup"><span data-stu-id="a35ae-156">pinMaximumLength</span></span>|<span data-ttu-id="a35ae-157">Int32</span><span class="sxs-lookup"><span data-stu-id="a35ae-157">Int32</span></span>|<span data-ttu-id="a35ae-158">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="a35ae-158">Not yet documented</span></span>|
|<span data-ttu-id="a35ae-159">pinUppercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="a35ae-159">pinUppercaseCharactersUsage</span></span>|[<span data-ttu-id="a35ae-160">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="a35ae-160">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="a35ae-161">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="a35ae-161">Not yet documented.</span></span> <span data-ttu-id="a35ae-162">Mögliche Werte sind: `allowed`, `required` und `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="a35ae-162">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="a35ae-163">pinLowercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="a35ae-163">pinLowercaseCharactersUsage</span></span>|[<span data-ttu-id="a35ae-164">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="a35ae-164">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="a35ae-165">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="a35ae-165">Not yet documented.</span></span> <span data-ttu-id="a35ae-166">Mögliche Werte sind: `allowed`, `required` und `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="a35ae-166">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="a35ae-167">pinSpecialCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="a35ae-167">pinSpecialCharactersUsage</span></span>|[<span data-ttu-id="a35ae-168">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="a35ae-168">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="a35ae-169">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="a35ae-169">Not yet documented.</span></span> <span data-ttu-id="a35ae-170">Mögliche Werte sind: `allowed`, `required` und `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="a35ae-170">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="a35ae-171">state</span><span class="sxs-lookup"><span data-stu-id="a35ae-171">state</span></span>|[<span data-ttu-id="a35ae-172">Aktivierung</span><span class="sxs-lookup"><span data-stu-id="a35ae-172">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="a35ae-173">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="a35ae-173">Not yet documented.</span></span> <span data-ttu-id="a35ae-174">Mögliche Werte sind: `notConfigured`, `enabled` und `disabled`.</span><span class="sxs-lookup"><span data-stu-id="a35ae-174">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="a35ae-175">securityDeviceRequired</span><span class="sxs-lookup"><span data-stu-id="a35ae-175">securityDeviceRequired</span></span>|<span data-ttu-id="a35ae-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="a35ae-176">Boolean</span></span>|<span data-ttu-id="a35ae-177">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="a35ae-177">Not yet documented</span></span>|
|<span data-ttu-id="a35ae-178">unlockWithBiometricsEnabled</span><span class="sxs-lookup"><span data-stu-id="a35ae-178">unlockWithBiometricsEnabled</span></span>|<span data-ttu-id="a35ae-179">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="a35ae-179">Boolean</span></span>|<span data-ttu-id="a35ae-180">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="a35ae-180">Not yet documented</span></span>|
|<span data-ttu-id="a35ae-181">remotePassportEnabled</span><span class="sxs-lookup"><span data-stu-id="a35ae-181">remotePassportEnabled</span></span>|<span data-ttu-id="a35ae-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="a35ae-182">Boolean</span></span>|<span data-ttu-id="a35ae-183">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="a35ae-183">Not yet documented</span></span>|
|<span data-ttu-id="a35ae-184">pinPreviousBlockCount</span><span class="sxs-lookup"><span data-stu-id="a35ae-184">pinPreviousBlockCount</span></span>|<span data-ttu-id="a35ae-185">Int32</span><span class="sxs-lookup"><span data-stu-id="a35ae-185">Int32</span></span>|<span data-ttu-id="a35ae-186">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="a35ae-186">Not yet documented</span></span>|
|<span data-ttu-id="a35ae-187">pinExpirationInDays</span><span class="sxs-lookup"><span data-stu-id="a35ae-187">pinExpirationInDays</span></span>|<span data-ttu-id="a35ae-188">Int32</span><span class="sxs-lookup"><span data-stu-id="a35ae-188">Int32</span></span>|<span data-ttu-id="a35ae-189">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="a35ae-189">Not yet documented</span></span>|
|<span data-ttu-id="a35ae-190">enhancedBiometricsState</span><span class="sxs-lookup"><span data-stu-id="a35ae-190">enhancedBiometricsState</span></span>|[<span data-ttu-id="a35ae-191">Aktivierung</span><span class="sxs-lookup"><span data-stu-id="a35ae-191">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="a35ae-192">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="a35ae-192">Not yet documented.</span></span> <span data-ttu-id="a35ae-193">Mögliche Werte sind: `notConfigured`, `enabled` und `disabled`.</span><span class="sxs-lookup"><span data-stu-id="a35ae-193">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|



## <a name="response"></a><span data-ttu-id="a35ae-194">Antwort</span><span class="sxs-lookup"><span data-stu-id="a35ae-194">Response</span></span>
<span data-ttu-id="a35ae-195">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="a35ae-195">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a35ae-196">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a35ae-196">Example</span></span>

### <a name="request"></a><span data-ttu-id="a35ae-197">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a35ae-197">Request</span></span>
<span data-ttu-id="a35ae-198">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a35ae-198">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
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

### <a name="response"></a><span data-ttu-id="a35ae-199">Antwort</span><span class="sxs-lookup"><span data-stu-id="a35ae-199">Response</span></span>
<span data-ttu-id="a35ae-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a35ae-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




