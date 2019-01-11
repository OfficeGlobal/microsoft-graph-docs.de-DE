---
title: deviceEnrollmentWindowsHelloForBusinessConfiguration aktualisieren
description: Aktualisieren der Eigenschaften eines deviceEnrollmentWindowsHelloForBusinessConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 982d28cdea829afd9e569ff97628fcf19b3c4956
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27825816"
---
# <a name="update-deviceenrollmentwindowshelloforbusinessconfiguration"></a><span data-ttu-id="14a09-103">deviceEnrollmentWindowsHelloForBusinessConfiguration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="14a09-103">Update deviceEnrollmentWindowsHelloForBusinessConfiguration</span></span>

> <span data-ttu-id="14a09-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="14a09-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="14a09-105">Aktualisieren der Eigenschaften eines [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="14a09-105">Update the properties of a [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="14a09-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="14a09-106">Prerequisites</span></span>
<span data-ttu-id="14a09-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="14a09-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="14a09-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="14a09-109">Permission type</span></span>|<span data-ttu-id="14a09-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="14a09-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="14a09-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="14a09-111">Delegated (work or school account)</span></span>|<span data-ttu-id="14a09-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14a09-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="14a09-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="14a09-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="14a09-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="14a09-114">Not supported.</span></span>|
|<span data-ttu-id="14a09-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="14a09-115">Application</span></span>|<span data-ttu-id="14a09-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="14a09-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="14a09-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="14a09-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="14a09-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="14a09-118">Request headers</span></span>
|<span data-ttu-id="14a09-119">Header</span><span class="sxs-lookup"><span data-stu-id="14a09-119">Header</span></span>|<span data-ttu-id="14a09-120">Wert</span><span class="sxs-lookup"><span data-stu-id="14a09-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="14a09-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="14a09-121">Authorization</span></span>|<span data-ttu-id="14a09-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="14a09-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="14a09-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="14a09-123">Accept</span></span>|<span data-ttu-id="14a09-124">application/json</span><span class="sxs-lookup"><span data-stu-id="14a09-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="14a09-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="14a09-125">Request body</span></span>
<span data-ttu-id="14a09-126">Geben Sie im Anforderungstext eine JSON-Darstellung für das [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md)-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="14a09-126">In the request body, supply a JSON representation for the [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>

<span data-ttu-id="14a09-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="14a09-127">The following table shows the properties that are required when you create the [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md).</span></span>

|<span data-ttu-id="14a09-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="14a09-128">Property</span></span>|<span data-ttu-id="14a09-129">Typ</span><span class="sxs-lookup"><span data-stu-id="14a09-129">Type</span></span>|<span data-ttu-id="14a09-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="14a09-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="14a09-131">id</span><span class="sxs-lookup"><span data-stu-id="14a09-131">id</span></span>|<span data-ttu-id="14a09-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="14a09-132">String</span></span>|<span data-ttu-id="14a09-133">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="14a09-133">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="14a09-134">displayName</span><span class="sxs-lookup"><span data-stu-id="14a09-134">displayName</span></span>|<span data-ttu-id="14a09-135">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="14a09-135">String</span></span>|<span data-ttu-id="14a09-136">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="14a09-136">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="14a09-137">description</span><span class="sxs-lookup"><span data-stu-id="14a09-137">description</span></span>|<span data-ttu-id="14a09-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="14a09-138">String</span></span>|<span data-ttu-id="14a09-139">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="14a09-139">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="14a09-140">Priorität</span><span class="sxs-lookup"><span data-stu-id="14a09-140">priority</span></span>|<span data-ttu-id="14a09-141">Int32</span><span class="sxs-lookup"><span data-stu-id="14a09-141">Int32</span></span>|<span data-ttu-id="14a09-142">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="14a09-142">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="14a09-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="14a09-143">createdDateTime</span></span>|<span data-ttu-id="14a09-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="14a09-144">DateTimeOffset</span></span>|<span data-ttu-id="14a09-145">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="14a09-145">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="14a09-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="14a09-146">lastModifiedDateTime</span></span>|<span data-ttu-id="14a09-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="14a09-147">DateTimeOffset</span></span>|<span data-ttu-id="14a09-148">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="14a09-148">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="14a09-149">Version</span><span class="sxs-lookup"><span data-stu-id="14a09-149">version</span></span>|<span data-ttu-id="14a09-150">Int32</span><span class="sxs-lookup"><span data-stu-id="14a09-150">Int32</span></span>|<span data-ttu-id="14a09-151">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="14a09-151">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="14a09-152">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="14a09-152">pinMinimumLength</span></span>|<span data-ttu-id="14a09-153">Int32</span><span class="sxs-lookup"><span data-stu-id="14a09-153">Int32</span></span>|<span data-ttu-id="14a09-154">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="14a09-154">Not yet documented</span></span>|
|<span data-ttu-id="14a09-155">pinMaximumLength</span><span class="sxs-lookup"><span data-stu-id="14a09-155">pinMaximumLength</span></span>|<span data-ttu-id="14a09-156">Int32</span><span class="sxs-lookup"><span data-stu-id="14a09-156">Int32</span></span>|<span data-ttu-id="14a09-157">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="14a09-157">Not yet documented</span></span>|
|<span data-ttu-id="14a09-158">pinUppercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="14a09-158">pinUppercaseCharactersUsage</span></span>|[<span data-ttu-id="14a09-159">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="14a09-159">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="14a09-160">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="14a09-160">Not yet documented.</span></span> <span data-ttu-id="14a09-161">Mögliche Werte sind: `allowed`, `required` und `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="14a09-161">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="14a09-162">pinLowercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="14a09-162">pinLowercaseCharactersUsage</span></span>|[<span data-ttu-id="14a09-163">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="14a09-163">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="14a09-164">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="14a09-164">Not yet documented.</span></span> <span data-ttu-id="14a09-165">Mögliche Werte sind: `allowed`, `required` und `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="14a09-165">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="14a09-166">pinSpecialCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="14a09-166">pinSpecialCharactersUsage</span></span>|[<span data-ttu-id="14a09-167">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="14a09-167">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="14a09-168">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="14a09-168">Not yet documented.</span></span> <span data-ttu-id="14a09-169">Mögliche Werte sind: `allowed`, `required` und `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="14a09-169">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="14a09-170">state</span><span class="sxs-lookup"><span data-stu-id="14a09-170">state</span></span>|[<span data-ttu-id="14a09-171">Aktivierung von Steuerelementen</span><span class="sxs-lookup"><span data-stu-id="14a09-171">enablement</span></span>](../resources/intune-onboarding-enablement.md)|<span data-ttu-id="14a09-172">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="14a09-172">Not yet documented.</span></span> <span data-ttu-id="14a09-173">Mögliche Werte sind: `notConfigured`, `enabled` und `disabled`.</span><span class="sxs-lookup"><span data-stu-id="14a09-173">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="14a09-174">securityDeviceRequired</span><span class="sxs-lookup"><span data-stu-id="14a09-174">securityDeviceRequired</span></span>|<span data-ttu-id="14a09-175">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="14a09-175">Boolean</span></span>|<span data-ttu-id="14a09-176">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="14a09-176">Not yet documented</span></span>|
|<span data-ttu-id="14a09-177">unlockWithBiometricsEnabled</span><span class="sxs-lookup"><span data-stu-id="14a09-177">unlockWithBiometricsEnabled</span></span>|<span data-ttu-id="14a09-178">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="14a09-178">Boolean</span></span>|<span data-ttu-id="14a09-179">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="14a09-179">Not yet documented</span></span>|
|<span data-ttu-id="14a09-180">remotePassportEnabled</span><span class="sxs-lookup"><span data-stu-id="14a09-180">remotePassportEnabled</span></span>|<span data-ttu-id="14a09-181">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="14a09-181">Boolean</span></span>|<span data-ttu-id="14a09-182">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="14a09-182">Not yet documented</span></span>|
|<span data-ttu-id="14a09-183">pinPreviousBlockCount</span><span class="sxs-lookup"><span data-stu-id="14a09-183">pinPreviousBlockCount</span></span>|<span data-ttu-id="14a09-184">Int32</span><span class="sxs-lookup"><span data-stu-id="14a09-184">Int32</span></span>|<span data-ttu-id="14a09-185">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="14a09-185">Not yet documented</span></span>|
|<span data-ttu-id="14a09-186">pinExpirationInDays</span><span class="sxs-lookup"><span data-stu-id="14a09-186">pinExpirationInDays</span></span>|<span data-ttu-id="14a09-187">Int32</span><span class="sxs-lookup"><span data-stu-id="14a09-187">Int32</span></span>|<span data-ttu-id="14a09-188">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="14a09-188">Not yet documented</span></span>|
|<span data-ttu-id="14a09-189">enhancedBiometricsState</span><span class="sxs-lookup"><span data-stu-id="14a09-189">enhancedBiometricsState</span></span>|[<span data-ttu-id="14a09-190">Aktivierung von Steuerelementen</span><span class="sxs-lookup"><span data-stu-id="14a09-190">enablement</span></span>](../resources/intune-onboarding-enablement.md)|<span data-ttu-id="14a09-191">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="14a09-191">Not yet documented.</span></span> <span data-ttu-id="14a09-192">Mögliche Werte sind: `notConfigured`, `enabled` und `disabled`.</span><span class="sxs-lookup"><span data-stu-id="14a09-192">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|



## <a name="response"></a><span data-ttu-id="14a09-193">Antwort</span><span class="sxs-lookup"><span data-stu-id="14a09-193">Response</span></span>
<span data-ttu-id="14a09-194">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="14a09-194">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="14a09-195">Beispiel</span><span class="sxs-lookup"><span data-stu-id="14a09-195">Example</span></span>
### <a name="request"></a><span data-ttu-id="14a09-196">Anforderung</span><span class="sxs-lookup"><span data-stu-id="14a09-196">Request</span></span>
<span data-ttu-id="14a09-197">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="14a09-197">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="14a09-198">Antwort</span><span class="sxs-lookup"><span data-stu-id="14a09-198">Response</span></span>
<span data-ttu-id="14a09-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="14a09-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



