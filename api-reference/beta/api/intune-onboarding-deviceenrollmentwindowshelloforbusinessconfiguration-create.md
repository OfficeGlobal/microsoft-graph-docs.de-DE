---
title: deviceEnrollmentWindowsHelloForBusinessConfiguration erstellen
description: Erstellen eines neuen deviceEnrollmentWindowsHelloForBusinessConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6f3e3188293455ca8ae7fd36b5040eec890df35d
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30985305"
---
# <a name="create-deviceenrollmentwindowshelloforbusinessconfiguration"></a><span data-ttu-id="b9146-103">deviceEnrollmentWindowsHelloForBusinessConfiguration erstellen</span><span class="sxs-lookup"><span data-stu-id="b9146-103">Create deviceEnrollmentWindowsHelloForBusinessConfiguration</span></span>

> <span data-ttu-id="b9146-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b9146-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b9146-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="b9146-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b9146-106">Erstellen eines neuen [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="b9146-106">Create a new [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b9146-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b9146-107">Prerequisites</span></span>
<span data-ttu-id="b9146-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b9146-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b9146-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b9146-110">Permission type</span></span>|<span data-ttu-id="b9146-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b9146-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b9146-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b9146-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b9146-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9146-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="b9146-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b9146-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b9146-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b9146-115">Not supported.</span></span>|
|<span data-ttu-id="b9146-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b9146-116">Application</span></span>|<span data-ttu-id="b9146-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b9146-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b9146-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b9146-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="b9146-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b9146-119">Request headers</span></span>
|<span data-ttu-id="b9146-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="b9146-120">Header</span></span>|<span data-ttu-id="b9146-121">Wert</span><span class="sxs-lookup"><span data-stu-id="b9146-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b9146-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b9146-122">Authorization</span></span>|<span data-ttu-id="b9146-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b9146-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b9146-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="b9146-124">Accept</span></span>|<span data-ttu-id="b9146-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b9146-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b9146-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b9146-126">Request body</span></span>
<span data-ttu-id="b9146-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das deviceEnrollmentWindowsHelloForBusinessConfiguration-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="b9146-127">In the request body, supply a JSON representation for the deviceEnrollmentWindowsHelloForBusinessConfiguration object.</span></span>

<span data-ttu-id="b9146-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der deviceEnrollmentWindowsHelloForBusinessConfiguration erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="b9146-128">The following table shows the properties that are required when you create the deviceEnrollmentWindowsHelloForBusinessConfiguration.</span></span>

|<span data-ttu-id="b9146-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b9146-129">Property</span></span>|<span data-ttu-id="b9146-130">Typ</span><span class="sxs-lookup"><span data-stu-id="b9146-130">Type</span></span>|<span data-ttu-id="b9146-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b9146-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b9146-132">id</span><span class="sxs-lookup"><span data-stu-id="b9146-132">id</span></span>|<span data-ttu-id="b9146-133">String</span><span class="sxs-lookup"><span data-stu-id="b9146-133">String</span></span>|<span data-ttu-id="b9146-134">ID der von [DeviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) geerbten Konfiguration der Registrierungs Status Seite</span><span class="sxs-lookup"><span data-stu-id="b9146-134">Id of the Enrollment Status Page configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="b9146-135">displayName</span><span class="sxs-lookup"><span data-stu-id="b9146-135">displayName</span></span>|<span data-ttu-id="b9146-136">String</span><span class="sxs-lookup"><span data-stu-id="b9146-136">String</span></span>|<span data-ttu-id="b9146-137">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b9146-137">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="b9146-138">description</span><span class="sxs-lookup"><span data-stu-id="b9146-138">description</span></span>|<span data-ttu-id="b9146-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b9146-139">String</span></span>|<span data-ttu-id="b9146-140">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b9146-140">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="b9146-141">Priorität</span><span class="sxs-lookup"><span data-stu-id="b9146-141">priority</span></span>|<span data-ttu-id="b9146-142">Int32</span><span class="sxs-lookup"><span data-stu-id="b9146-142">Int32</span></span>|<span data-ttu-id="b9146-143">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b9146-143">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="b9146-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b9146-144">createdDateTime</span></span>|<span data-ttu-id="b9146-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b9146-145">DateTimeOffset</span></span>|<span data-ttu-id="b9146-146">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b9146-146">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="b9146-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b9146-147">lastModifiedDateTime</span></span>|<span data-ttu-id="b9146-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b9146-148">DateTimeOffset</span></span>|<span data-ttu-id="b9146-149">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b9146-149">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="b9146-150">Version</span><span class="sxs-lookup"><span data-stu-id="b9146-150">version</span></span>|<span data-ttu-id="b9146-151">Int32</span><span class="sxs-lookup"><span data-stu-id="b9146-151">Int32</span></span>|<span data-ttu-id="b9146-152">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b9146-152">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="b9146-153">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="b9146-153">pinMinimumLength</span></span>|<span data-ttu-id="b9146-154">Int32</span><span class="sxs-lookup"><span data-stu-id="b9146-154">Int32</span></span>|<span data-ttu-id="b9146-155">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="b9146-155">Not yet documented</span></span>|
|<span data-ttu-id="b9146-156">pinMaximumLength</span><span class="sxs-lookup"><span data-stu-id="b9146-156">pinMaximumLength</span></span>|<span data-ttu-id="b9146-157">Int32</span><span class="sxs-lookup"><span data-stu-id="b9146-157">Int32</span></span>|<span data-ttu-id="b9146-158">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="b9146-158">Not yet documented</span></span>|
|<span data-ttu-id="b9146-159">pinUppercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="b9146-159">pinUppercaseCharactersUsage</span></span>|[<span data-ttu-id="b9146-160">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="b9146-160">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="b9146-161">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="b9146-161">Not yet documented.</span></span> <span data-ttu-id="b9146-162">Mögliche Werte sind: `allowed`, `required` und `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="b9146-162">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="b9146-163">pinLowercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="b9146-163">pinLowercaseCharactersUsage</span></span>|[<span data-ttu-id="b9146-164">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="b9146-164">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="b9146-165">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="b9146-165">Not yet documented.</span></span> <span data-ttu-id="b9146-166">Mögliche Werte sind: `allowed`, `required` und `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="b9146-166">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="b9146-167">pinSpecialCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="b9146-167">pinSpecialCharactersUsage</span></span>|[<span data-ttu-id="b9146-168">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="b9146-168">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="b9146-169">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="b9146-169">Not yet documented.</span></span> <span data-ttu-id="b9146-170">Mögliche Werte sind: `allowed`, `required` und `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="b9146-170">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="b9146-171">state</span><span class="sxs-lookup"><span data-stu-id="b9146-171">state</span></span>|[<span data-ttu-id="b9146-172">Aktivierung</span><span class="sxs-lookup"><span data-stu-id="b9146-172">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="b9146-173">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="b9146-173">Not yet documented.</span></span> <span data-ttu-id="b9146-174">Mögliche Werte sind: `notConfigured`, `enabled` und `disabled`.</span><span class="sxs-lookup"><span data-stu-id="b9146-174">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="b9146-175">securityDeviceRequired</span><span class="sxs-lookup"><span data-stu-id="b9146-175">securityDeviceRequired</span></span>|<span data-ttu-id="b9146-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9146-176">Boolean</span></span>|<span data-ttu-id="b9146-177">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="b9146-177">Not yet documented</span></span>|
|<span data-ttu-id="b9146-178">unlockWithBiometricsEnabled</span><span class="sxs-lookup"><span data-stu-id="b9146-178">unlockWithBiometricsEnabled</span></span>|<span data-ttu-id="b9146-179">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b9146-179">Boolean</span></span>|<span data-ttu-id="b9146-180">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="b9146-180">Not yet documented</span></span>|
|<span data-ttu-id="b9146-181">remotePassportEnabled</span><span class="sxs-lookup"><span data-stu-id="b9146-181">remotePassportEnabled</span></span>|<span data-ttu-id="b9146-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9146-182">Boolean</span></span>|<span data-ttu-id="b9146-183">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="b9146-183">Not yet documented</span></span>|
|<span data-ttu-id="b9146-184">pinPreviousBlockCount</span><span class="sxs-lookup"><span data-stu-id="b9146-184">pinPreviousBlockCount</span></span>|<span data-ttu-id="b9146-185">Int32</span><span class="sxs-lookup"><span data-stu-id="b9146-185">Int32</span></span>|<span data-ttu-id="b9146-186">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="b9146-186">Not yet documented</span></span>|
|<span data-ttu-id="b9146-187">pinExpirationInDays</span><span class="sxs-lookup"><span data-stu-id="b9146-187">pinExpirationInDays</span></span>|<span data-ttu-id="b9146-188">Int32</span><span class="sxs-lookup"><span data-stu-id="b9146-188">Int32</span></span>|<span data-ttu-id="b9146-189">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="b9146-189">Not yet documented</span></span>|
|<span data-ttu-id="b9146-190">enhancedBiometricsState</span><span class="sxs-lookup"><span data-stu-id="b9146-190">enhancedBiometricsState</span></span>|[<span data-ttu-id="b9146-191">Aktivierung</span><span class="sxs-lookup"><span data-stu-id="b9146-191">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="b9146-192">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="b9146-192">Not yet documented.</span></span> <span data-ttu-id="b9146-193">Mögliche Werte sind: `notConfigured`, `enabled` und `disabled`.</span><span class="sxs-lookup"><span data-stu-id="b9146-193">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|



## <a name="response"></a><span data-ttu-id="b9146-194">Antwort</span><span class="sxs-lookup"><span data-stu-id="b9146-194">Response</span></span>
<span data-ttu-id="b9146-195">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="b9146-195">If successful, this method returns a `201 Created` response code and a [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b9146-196">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b9146-196">Example</span></span>

### <a name="request"></a><span data-ttu-id="b9146-197">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b9146-197">Request</span></span>
<span data-ttu-id="b9146-198">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b9146-198">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations
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

### <a name="response"></a><span data-ttu-id="b9146-199">Antwort</span><span class="sxs-lookup"><span data-stu-id="b9146-199">Response</span></span>
<span data-ttu-id="b9146-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b9146-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




