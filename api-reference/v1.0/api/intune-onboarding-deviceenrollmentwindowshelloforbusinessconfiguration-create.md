---
title: deviceEnrollmentWindowsHelloForBusinessConfiguration erstellen
description: Erstellen eines neuen deviceEnrollmentWindowsHelloForBusinessConfiguration-Objekts.
author: tfitzmac
ms.openlocfilehash: 1c17cfccfd6875b11a392e5d8c00785e1f10673b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27348601"
---
# <a name="create-deviceenrollmentwindowshelloforbusinessconfiguration"></a><span data-ttu-id="3ff3a-103">deviceEnrollmentWindowsHelloForBusinessConfiguration erstellen</span><span class="sxs-lookup"><span data-stu-id="3ff3a-103">Create deviceEnrollmentWindowsHelloForBusinessConfiguration</span></span>

> <span data-ttu-id="3ff3a-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="3ff3a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3ff3a-105">Erstellen eines neuen [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="3ff3a-105">Create a new [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3ff3a-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="3ff3a-106">Prerequisites</span></span>
<span data-ttu-id="3ff3a-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3ff3a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3ff3a-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3ff3a-109">Permission type</span></span>|<span data-ttu-id="3ff3a-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3ff3a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3ff3a-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3ff3a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3ff3a-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ff3a-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="3ff3a-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3ff3a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3ff3a-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3ff3a-114">Not supported.</span></span>|
|<span data-ttu-id="3ff3a-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3ff3a-115">Application</span></span>|<span data-ttu-id="3ff3a-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3ff3a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3ff3a-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3ff3a-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="3ff3a-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3ff3a-118">Request headers</span></span>
|<span data-ttu-id="3ff3a-119">Header</span><span class="sxs-lookup"><span data-stu-id="3ff3a-119">Header</span></span>|<span data-ttu-id="3ff3a-120">Wert</span><span class="sxs-lookup"><span data-stu-id="3ff3a-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3ff3a-121">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="3ff3a-121">Authorization</span></span>|<span data-ttu-id="3ff3a-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="3ff3a-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3ff3a-123">Accept</span><span class="sxs-lookup"><span data-stu-id="3ff3a-123">Accept</span></span>|<span data-ttu-id="3ff3a-124">application/json</span><span class="sxs-lookup"><span data-stu-id="3ff3a-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3ff3a-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3ff3a-125">Request body</span></span>
<span data-ttu-id="3ff3a-126">Geben Sie im Anforderungstext eine JSON-Darstellung für das deviceEnrollmentWindowsHelloForBusinessConfiguration-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="3ff3a-126">In the request body, supply a JSON representation for the deviceEnrollmentWindowsHelloForBusinessConfiguration object.</span></span>

<span data-ttu-id="3ff3a-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der deviceEnrollmentWindowsHelloForBusinessConfiguration erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="3ff3a-127">The following table shows the properties that are required when you create the deviceEnrollmentWindowsHelloForBusinessConfiguration.</span></span>

|<span data-ttu-id="3ff3a-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3ff3a-128">Property</span></span>|<span data-ttu-id="3ff3a-129">Typ</span><span class="sxs-lookup"><span data-stu-id="3ff3a-129">Type</span></span>|<span data-ttu-id="3ff3a-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3ff3a-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3ff3a-131">id</span><span class="sxs-lookup"><span data-stu-id="3ff3a-131">id</span></span>|<span data-ttu-id="3ff3a-132">String</span><span class="sxs-lookup"><span data-stu-id="3ff3a-132">String</span></span>|<span data-ttu-id="3ff3a-133">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3ff3a-133">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="3ff3a-134">displayName</span><span class="sxs-lookup"><span data-stu-id="3ff3a-134">displayName</span></span>|<span data-ttu-id="3ff3a-135">String</span><span class="sxs-lookup"><span data-stu-id="3ff3a-135">String</span></span>|<span data-ttu-id="3ff3a-136">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3ff3a-136">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="3ff3a-137">description</span><span class="sxs-lookup"><span data-stu-id="3ff3a-137">description</span></span>|<span data-ttu-id="3ff3a-138">String</span><span class="sxs-lookup"><span data-stu-id="3ff3a-138">String</span></span>|<span data-ttu-id="3ff3a-139">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3ff3a-139">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="3ff3a-140">Priorität</span><span class="sxs-lookup"><span data-stu-id="3ff3a-140">priority</span></span>|<span data-ttu-id="3ff3a-141">Int32</span><span class="sxs-lookup"><span data-stu-id="3ff3a-141">Int32</span></span>|<span data-ttu-id="3ff3a-142">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3ff3a-142">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="3ff3a-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3ff3a-143">createdDateTime</span></span>|<span data-ttu-id="3ff3a-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3ff3a-144">DateTimeOffset</span></span>|<span data-ttu-id="3ff3a-145">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3ff3a-145">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="3ff3a-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3ff3a-146">lastModifiedDateTime</span></span>|<span data-ttu-id="3ff3a-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3ff3a-147">DateTimeOffset</span></span>|<span data-ttu-id="3ff3a-148">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3ff3a-148">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="3ff3a-149">Version</span><span class="sxs-lookup"><span data-stu-id="3ff3a-149">version</span></span>|<span data-ttu-id="3ff3a-150">Int32</span><span class="sxs-lookup"><span data-stu-id="3ff3a-150">Int32</span></span>|<span data-ttu-id="3ff3a-151">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3ff3a-151">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="3ff3a-152">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="3ff3a-152">pinMinimumLength</span></span>|<span data-ttu-id="3ff3a-153">Int32</span><span class="sxs-lookup"><span data-stu-id="3ff3a-153">Int32</span></span>|<span data-ttu-id="3ff3a-154">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="3ff3a-154">Not yet documented</span></span>|
|<span data-ttu-id="3ff3a-155">pinMaximumLength</span><span class="sxs-lookup"><span data-stu-id="3ff3a-155">pinMaximumLength</span></span>|<span data-ttu-id="3ff3a-156">Int32</span><span class="sxs-lookup"><span data-stu-id="3ff3a-156">Int32</span></span>|<span data-ttu-id="3ff3a-157">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="3ff3a-157">Not yet documented</span></span>|
|<span data-ttu-id="3ff3a-158">pinUppercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="3ff3a-158">pinUppercaseCharactersUsage</span></span>|[<span data-ttu-id="3ff3a-159">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="3ff3a-159">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="3ff3a-160">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="3ff3a-160">Not yet documented.</span></span> <span data-ttu-id="3ff3a-161">Mögliche Werte sind: `allowed`, `required` und `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="3ff3a-161">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="3ff3a-162">pinLowercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="3ff3a-162">pinLowercaseCharactersUsage</span></span>|[<span data-ttu-id="3ff3a-163">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="3ff3a-163">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="3ff3a-164">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="3ff3a-164">Not yet documented.</span></span> <span data-ttu-id="3ff3a-165">Mögliche Werte sind: `allowed`, `required` und `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="3ff3a-165">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="3ff3a-166">pinSpecialCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="3ff3a-166">pinSpecialCharactersUsage</span></span>|[<span data-ttu-id="3ff3a-167">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="3ff3a-167">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="3ff3a-168">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="3ff3a-168">Not yet documented.</span></span> <span data-ttu-id="3ff3a-169">Mögliche Werte sind: `allowed`, `required` und `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="3ff3a-169">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="3ff3a-170">state</span><span class="sxs-lookup"><span data-stu-id="3ff3a-170">state</span></span>|[<span data-ttu-id="3ff3a-171">Aktivierung von Steuerelementen</span><span class="sxs-lookup"><span data-stu-id="3ff3a-171">enablement</span></span>](../resources/intune-onboarding-enablement.md)|<span data-ttu-id="3ff3a-172">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="3ff3a-172">Not yet documented.</span></span> <span data-ttu-id="3ff3a-173">Mögliche Werte sind: `notConfigured`, `enabled` und `disabled`.</span><span class="sxs-lookup"><span data-stu-id="3ff3a-173">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="3ff3a-174">securityDeviceRequired</span><span class="sxs-lookup"><span data-stu-id="3ff3a-174">securityDeviceRequired</span></span>|<span data-ttu-id="3ff3a-175">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="3ff3a-175">Boolean</span></span>|<span data-ttu-id="3ff3a-176">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="3ff3a-176">Not yet documented</span></span>|
|<span data-ttu-id="3ff3a-177">unlockWithBiometricsEnabled</span><span class="sxs-lookup"><span data-stu-id="3ff3a-177">unlockWithBiometricsEnabled</span></span>|<span data-ttu-id="3ff3a-178">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="3ff3a-178">Boolean</span></span>|<span data-ttu-id="3ff3a-179">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="3ff3a-179">Not yet documented</span></span>|
|<span data-ttu-id="3ff3a-180">remotePassportEnabled</span><span class="sxs-lookup"><span data-stu-id="3ff3a-180">remotePassportEnabled</span></span>|<span data-ttu-id="3ff3a-181">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="3ff3a-181">Boolean</span></span>|<span data-ttu-id="3ff3a-182">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="3ff3a-182">Not yet documented</span></span>|
|<span data-ttu-id="3ff3a-183">pinPreviousBlockCount</span><span class="sxs-lookup"><span data-stu-id="3ff3a-183">pinPreviousBlockCount</span></span>|<span data-ttu-id="3ff3a-184">Int32</span><span class="sxs-lookup"><span data-stu-id="3ff3a-184">Int32</span></span>|<span data-ttu-id="3ff3a-185">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="3ff3a-185">Not yet documented</span></span>|
|<span data-ttu-id="3ff3a-186">pinExpirationInDays</span><span class="sxs-lookup"><span data-stu-id="3ff3a-186">pinExpirationInDays</span></span>|<span data-ttu-id="3ff3a-187">Int32</span><span class="sxs-lookup"><span data-stu-id="3ff3a-187">Int32</span></span>|<span data-ttu-id="3ff3a-188">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="3ff3a-188">Not yet documented</span></span>|
|<span data-ttu-id="3ff3a-189">enhancedBiometricsState</span><span class="sxs-lookup"><span data-stu-id="3ff3a-189">enhancedBiometricsState</span></span>|[<span data-ttu-id="3ff3a-190">Aktivierung von Steuerelementen</span><span class="sxs-lookup"><span data-stu-id="3ff3a-190">enablement</span></span>](../resources/intune-onboarding-enablement.md)|<span data-ttu-id="3ff3a-191">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="3ff3a-191">Not yet documented.</span></span> <span data-ttu-id="3ff3a-192">Mögliche Werte sind: `notConfigured`, `enabled` und `disabled`.</span><span class="sxs-lookup"><span data-stu-id="3ff3a-192">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|



## <a name="response"></a><span data-ttu-id="3ff3a-193">Antwort</span><span class="sxs-lookup"><span data-stu-id="3ff3a-193">Response</span></span>
<span data-ttu-id="3ff3a-194">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="3ff3a-194">If successful, this method returns a `201 Created` response code and a [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3ff3a-195">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3ff3a-195">Example</span></span>
### <a name="request"></a><span data-ttu-id="3ff3a-196">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3ff3a-196">Request</span></span>
<span data-ttu-id="3ff3a-197">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3ff3a-197">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations
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

### <a name="response"></a><span data-ttu-id="3ff3a-198">Antwort</span><span class="sxs-lookup"><span data-stu-id="3ff3a-198">Response</span></span>
<span data-ttu-id="3ff3a-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3ff3a-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



