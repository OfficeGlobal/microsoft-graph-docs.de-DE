---
title: deviceEnrollmentWindowsHelloForBusinessConfiguration aktualisieren
description: Aktualisieren der Eigenschaften eines deviceEnrollmentWindowsHelloForBusinessConfiguration-Objekts.
ms.openlocfilehash: f91067a57dc4da7dc7d4850f72fbe267f364c6e6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27020086"
---
# <a name="update-deviceenrollmentwindowshelloforbusinessconfiguration"></a><span data-ttu-id="1dae0-103">deviceEnrollmentWindowsHelloForBusinessConfiguration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="1dae0-103">Update deviceEnrollmentWindowsHelloForBusinessConfiguration</span></span>

> <span data-ttu-id="1dae0-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="1dae0-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1dae0-105">Aktualisieren der Eigenschaften eines [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="1dae0-105">Update the properties of a [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1dae0-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="1dae0-106">Prerequisites</span></span>
<span data-ttu-id="1dae0-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1dae0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1dae0-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1dae0-109">Permission type</span></span>|<span data-ttu-id="1dae0-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1dae0-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1dae0-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1dae0-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1dae0-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1dae0-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="1dae0-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1dae0-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1dae0-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1dae0-114">Not supported.</span></span>|
|<span data-ttu-id="1dae0-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1dae0-115">Application</span></span>|<span data-ttu-id="1dae0-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1dae0-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1dae0-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1dae0-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="1dae0-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1dae0-118">Request headers</span></span>
|<span data-ttu-id="1dae0-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="1dae0-119">Header</span></span>|<span data-ttu-id="1dae0-120">Wert</span><span class="sxs-lookup"><span data-stu-id="1dae0-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1dae0-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1dae0-121">Authorization</span></span>|<span data-ttu-id="1dae0-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="1dae0-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1dae0-123">Accept</span><span class="sxs-lookup"><span data-stu-id="1dae0-123">Accept</span></span>|<span data-ttu-id="1dae0-124">application/json</span><span class="sxs-lookup"><span data-stu-id="1dae0-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1dae0-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1dae0-125">Request body</span></span>
<span data-ttu-id="1dae0-126">Geben Sie im Anforderungstext eine JSON-Darstellung für das [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md)-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="1dae0-126">In the request body, supply a JSON representation for the [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>

<span data-ttu-id="1dae0-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="1dae0-127">The following table shows the properties that are required when you create the [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md).</span></span>

|<span data-ttu-id="1dae0-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1dae0-128">Property</span></span>|<span data-ttu-id="1dae0-129">Typ</span><span class="sxs-lookup"><span data-stu-id="1dae0-129">Type</span></span>|<span data-ttu-id="1dae0-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1dae0-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1dae0-131">id</span><span class="sxs-lookup"><span data-stu-id="1dae0-131">id</span></span>|<span data-ttu-id="1dae0-132">String</span><span class="sxs-lookup"><span data-stu-id="1dae0-132">String</span></span>|<span data-ttu-id="1dae0-133">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1dae0-133">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="1dae0-134">displayName</span><span class="sxs-lookup"><span data-stu-id="1dae0-134">displayName</span></span>|<span data-ttu-id="1dae0-135">String</span><span class="sxs-lookup"><span data-stu-id="1dae0-135">String</span></span>|<span data-ttu-id="1dae0-136">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1dae0-136">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="1dae0-137">description</span><span class="sxs-lookup"><span data-stu-id="1dae0-137">description</span></span>|<span data-ttu-id="1dae0-138">String</span><span class="sxs-lookup"><span data-stu-id="1dae0-138">String</span></span>|<span data-ttu-id="1dae0-139">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1dae0-139">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="1dae0-140">Priorität</span><span class="sxs-lookup"><span data-stu-id="1dae0-140">priority</span></span>|<span data-ttu-id="1dae0-141">Int32</span><span class="sxs-lookup"><span data-stu-id="1dae0-141">Int32</span></span>|<span data-ttu-id="1dae0-142">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1dae0-142">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="1dae0-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1dae0-143">createdDateTime</span></span>|<span data-ttu-id="1dae0-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1dae0-144">DateTimeOffset</span></span>|<span data-ttu-id="1dae0-145">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1dae0-145">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="1dae0-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1dae0-146">lastModifiedDateTime</span></span>|<span data-ttu-id="1dae0-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1dae0-147">DateTimeOffset</span></span>|<span data-ttu-id="1dae0-148">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1dae0-148">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="1dae0-149">Version</span><span class="sxs-lookup"><span data-stu-id="1dae0-149">version</span></span>|<span data-ttu-id="1dae0-150">Int32</span><span class="sxs-lookup"><span data-stu-id="1dae0-150">Int32</span></span>|<span data-ttu-id="1dae0-151">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1dae0-151">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="1dae0-152">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="1dae0-152">pinMinimumLength</span></span>|<span data-ttu-id="1dae0-153">Int32</span><span class="sxs-lookup"><span data-stu-id="1dae0-153">Int32</span></span>|<span data-ttu-id="1dae0-154">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="1dae0-154">Not yet documented</span></span>|
|<span data-ttu-id="1dae0-155">pinMaximumLength</span><span class="sxs-lookup"><span data-stu-id="1dae0-155">pinMaximumLength</span></span>|<span data-ttu-id="1dae0-156">Int32</span><span class="sxs-lookup"><span data-stu-id="1dae0-156">Int32</span></span>|<span data-ttu-id="1dae0-157">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="1dae0-157">Not yet documented</span></span>|
|<span data-ttu-id="1dae0-158">pinUppercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="1dae0-158">pinUppercaseCharactersUsage</span></span>|[<span data-ttu-id="1dae0-159">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="1dae0-159">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="1dae0-160">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="1dae0-160">Not yet documented.</span></span> <span data-ttu-id="1dae0-161">Mögliche Werte sind: `allowed`, `required` und `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="1dae0-161">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="1dae0-162">pinLowercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="1dae0-162">pinLowercaseCharactersUsage</span></span>|[<span data-ttu-id="1dae0-163">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="1dae0-163">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="1dae0-164">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="1dae0-164">Not yet documented.</span></span> <span data-ttu-id="1dae0-165">Mögliche Werte sind: `allowed`, `required` und `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="1dae0-165">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="1dae0-166">pinSpecialCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="1dae0-166">pinSpecialCharactersUsage</span></span>|[<span data-ttu-id="1dae0-167">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="1dae0-167">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="1dae0-168">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="1dae0-168">Not yet documented.</span></span> <span data-ttu-id="1dae0-169">Mögliche Werte sind: `allowed`, `required` und `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="1dae0-169">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="1dae0-170">state</span><span class="sxs-lookup"><span data-stu-id="1dae0-170">state</span></span>|[<span data-ttu-id="1dae0-171">Aktivierung von Steuerelementen</span><span class="sxs-lookup"><span data-stu-id="1dae0-171">enablement</span></span>](../resources/intune-onboarding-enablement.md)|<span data-ttu-id="1dae0-172">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="1dae0-172">Not yet documented.</span></span> <span data-ttu-id="1dae0-173">Mögliche Werte sind: `notConfigured`, `enabled` und `disabled`.</span><span class="sxs-lookup"><span data-stu-id="1dae0-173">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="1dae0-174">securityDeviceRequired</span><span class="sxs-lookup"><span data-stu-id="1dae0-174">securityDeviceRequired</span></span>|<span data-ttu-id="1dae0-175">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="1dae0-175">Boolean</span></span>|<span data-ttu-id="1dae0-176">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="1dae0-176">Not yet documented</span></span>|
|<span data-ttu-id="1dae0-177">unlockWithBiometricsEnabled</span><span class="sxs-lookup"><span data-stu-id="1dae0-177">unlockWithBiometricsEnabled</span></span>|<span data-ttu-id="1dae0-178">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="1dae0-178">Boolean</span></span>|<span data-ttu-id="1dae0-179">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="1dae0-179">Not yet documented</span></span>|
|<span data-ttu-id="1dae0-180">remotePassportEnabled</span><span class="sxs-lookup"><span data-stu-id="1dae0-180">remotePassportEnabled</span></span>|<span data-ttu-id="1dae0-181">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="1dae0-181">Boolean</span></span>|<span data-ttu-id="1dae0-182">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="1dae0-182">Not yet documented</span></span>|
|<span data-ttu-id="1dae0-183">pinPreviousBlockCount</span><span class="sxs-lookup"><span data-stu-id="1dae0-183">pinPreviousBlockCount</span></span>|<span data-ttu-id="1dae0-184">Int32</span><span class="sxs-lookup"><span data-stu-id="1dae0-184">Int32</span></span>|<span data-ttu-id="1dae0-185">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="1dae0-185">Not yet documented</span></span>|
|<span data-ttu-id="1dae0-186">pinExpirationInDays</span><span class="sxs-lookup"><span data-stu-id="1dae0-186">pinExpirationInDays</span></span>|<span data-ttu-id="1dae0-187">Int32</span><span class="sxs-lookup"><span data-stu-id="1dae0-187">Int32</span></span>|<span data-ttu-id="1dae0-188">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="1dae0-188">Not yet documented</span></span>|
|<span data-ttu-id="1dae0-189">enhancedBiometricsState</span><span class="sxs-lookup"><span data-stu-id="1dae0-189">enhancedBiometricsState</span></span>|[<span data-ttu-id="1dae0-190">Aktivierung von Steuerelementen</span><span class="sxs-lookup"><span data-stu-id="1dae0-190">enablement</span></span>](../resources/intune-onboarding-enablement.md)|<span data-ttu-id="1dae0-191">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="1dae0-191">Not yet documented.</span></span> <span data-ttu-id="1dae0-192">Mögliche Werte sind: `notConfigured`, `enabled` und `disabled`.</span><span class="sxs-lookup"><span data-stu-id="1dae0-192">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|



## <a name="response"></a><span data-ttu-id="1dae0-193">Antwort</span><span class="sxs-lookup"><span data-stu-id="1dae0-193">Response</span></span>
<span data-ttu-id="1dae0-194">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="1dae0-194">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1dae0-195">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1dae0-195">Example</span></span>
### <a name="request"></a><span data-ttu-id="1dae0-196">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1dae0-196">Request</span></span>
<span data-ttu-id="1dae0-197">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1dae0-197">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1dae0-198">Antwort</span><span class="sxs-lookup"><span data-stu-id="1dae0-198">Response</span></span>
<span data-ttu-id="1dae0-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1dae0-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



