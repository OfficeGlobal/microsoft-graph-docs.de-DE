---
title: deviceEnrollmentWindowsHelloForBusinessConfiguration erstellen
description: Erstellen eines neuen deviceEnrollmentWindowsHelloForBusinessConfiguration-Objekts.
ms.openlocfilehash: de4eff1e68157a2f1069e031b209171e90a198fd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017212"
---
# <a name="create-deviceenrollmentwindowshelloforbusinessconfiguration"></a><span data-ttu-id="d3692-103">deviceEnrollmentWindowsHelloForBusinessConfiguration erstellen</span><span class="sxs-lookup"><span data-stu-id="d3692-103">Create deviceEnrollmentWindowsHelloForBusinessConfiguration</span></span>

> <span data-ttu-id="d3692-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="d3692-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d3692-105">Erstellen eines neuen [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="d3692-105">Create a new [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d3692-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="d3692-106">Prerequisites</span></span>
<span data-ttu-id="d3692-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d3692-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d3692-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d3692-109">Permission type</span></span>|<span data-ttu-id="d3692-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d3692-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d3692-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d3692-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d3692-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3692-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="d3692-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d3692-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d3692-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d3692-114">Not supported.</span></span>|
|<span data-ttu-id="d3692-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d3692-115">Application</span></span>|<span data-ttu-id="d3692-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d3692-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d3692-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d3692-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="d3692-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d3692-118">Request headers</span></span>
|<span data-ttu-id="d3692-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="d3692-119">Header</span></span>|<span data-ttu-id="d3692-120">Wert</span><span class="sxs-lookup"><span data-stu-id="d3692-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d3692-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d3692-121">Authorization</span></span>|<span data-ttu-id="d3692-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="d3692-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d3692-123">Accept</span><span class="sxs-lookup"><span data-stu-id="d3692-123">Accept</span></span>|<span data-ttu-id="d3692-124">application/json</span><span class="sxs-lookup"><span data-stu-id="d3692-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d3692-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d3692-125">Request body</span></span>
<span data-ttu-id="d3692-126">Geben Sie im Anforderungstext eine JSON-Darstellung für das deviceEnrollmentWindowsHelloForBusinessConfiguration-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="d3692-126">In the request body, supply a JSON representation for the deviceEnrollmentWindowsHelloForBusinessConfiguration object.</span></span>

<span data-ttu-id="d3692-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der deviceEnrollmentWindowsHelloForBusinessConfiguration erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="d3692-127">The following table shows the properties that are required when you create the deviceEnrollmentWindowsHelloForBusinessConfiguration.</span></span>

|<span data-ttu-id="d3692-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d3692-128">Property</span></span>|<span data-ttu-id="d3692-129">Typ</span><span class="sxs-lookup"><span data-stu-id="d3692-129">Type</span></span>|<span data-ttu-id="d3692-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d3692-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d3692-131">id</span><span class="sxs-lookup"><span data-stu-id="d3692-131">id</span></span>|<span data-ttu-id="d3692-132">String</span><span class="sxs-lookup"><span data-stu-id="d3692-132">String</span></span>|<span data-ttu-id="d3692-133">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d3692-133">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d3692-134">displayName</span><span class="sxs-lookup"><span data-stu-id="d3692-134">displayName</span></span>|<span data-ttu-id="d3692-135">String</span><span class="sxs-lookup"><span data-stu-id="d3692-135">String</span></span>|<span data-ttu-id="d3692-136">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d3692-136">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d3692-137">description</span><span class="sxs-lookup"><span data-stu-id="d3692-137">description</span></span>|<span data-ttu-id="d3692-138">String</span><span class="sxs-lookup"><span data-stu-id="d3692-138">String</span></span>|<span data-ttu-id="d3692-139">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d3692-139">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d3692-140">Priorität</span><span class="sxs-lookup"><span data-stu-id="d3692-140">priority</span></span>|<span data-ttu-id="d3692-141">Int32</span><span class="sxs-lookup"><span data-stu-id="d3692-141">Int32</span></span>|<span data-ttu-id="d3692-142">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d3692-142">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d3692-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d3692-143">createdDateTime</span></span>|<span data-ttu-id="d3692-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d3692-144">DateTimeOffset</span></span>|<span data-ttu-id="d3692-145">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d3692-145">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d3692-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d3692-146">lastModifiedDateTime</span></span>|<span data-ttu-id="d3692-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d3692-147">DateTimeOffset</span></span>|<span data-ttu-id="d3692-148">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d3692-148">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d3692-149">Version</span><span class="sxs-lookup"><span data-stu-id="d3692-149">version</span></span>|<span data-ttu-id="d3692-150">Int32</span><span class="sxs-lookup"><span data-stu-id="d3692-150">Int32</span></span>|<span data-ttu-id="d3692-151">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d3692-151">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d3692-152">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="d3692-152">pinMinimumLength</span></span>|<span data-ttu-id="d3692-153">Int32</span><span class="sxs-lookup"><span data-stu-id="d3692-153">Int32</span></span>|<span data-ttu-id="d3692-154">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="d3692-154">Not yet documented</span></span>|
|<span data-ttu-id="d3692-155">pinMaximumLength</span><span class="sxs-lookup"><span data-stu-id="d3692-155">pinMaximumLength</span></span>|<span data-ttu-id="d3692-156">Int32</span><span class="sxs-lookup"><span data-stu-id="d3692-156">Int32</span></span>|<span data-ttu-id="d3692-157">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="d3692-157">Not yet documented</span></span>|
|<span data-ttu-id="d3692-158">pinUppercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="d3692-158">pinUppercaseCharactersUsage</span></span>|[<span data-ttu-id="d3692-159">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="d3692-159">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="d3692-160">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="d3692-160">Not yet documented.</span></span> <span data-ttu-id="d3692-161">Mögliche Werte sind: `allowed`, `required` und `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="d3692-161">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="d3692-162">pinLowercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="d3692-162">pinLowercaseCharactersUsage</span></span>|[<span data-ttu-id="d3692-163">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="d3692-163">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="d3692-164">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="d3692-164">Not yet documented.</span></span> <span data-ttu-id="d3692-165">Mögliche Werte sind: `allowed`, `required` und `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="d3692-165">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="d3692-166">pinSpecialCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="d3692-166">pinSpecialCharactersUsage</span></span>|[<span data-ttu-id="d3692-167">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="d3692-167">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="d3692-168">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="d3692-168">Not yet documented.</span></span> <span data-ttu-id="d3692-169">Mögliche Werte sind: `allowed`, `required` und `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="d3692-169">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="d3692-170">state</span><span class="sxs-lookup"><span data-stu-id="d3692-170">state</span></span>|[<span data-ttu-id="d3692-171">Aktivierung von Steuerelementen</span><span class="sxs-lookup"><span data-stu-id="d3692-171">enablement</span></span>](../resources/intune-onboarding-enablement.md)|<span data-ttu-id="d3692-172">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="d3692-172">Not yet documented.</span></span> <span data-ttu-id="d3692-173">Mögliche Werte sind: `notConfigured`, `enabled` und `disabled`.</span><span class="sxs-lookup"><span data-stu-id="d3692-173">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="d3692-174">securityDeviceRequired</span><span class="sxs-lookup"><span data-stu-id="d3692-174">securityDeviceRequired</span></span>|<span data-ttu-id="d3692-175">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d3692-175">Boolean</span></span>|<span data-ttu-id="d3692-176">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="d3692-176">Not yet documented</span></span>|
|<span data-ttu-id="d3692-177">unlockWithBiometricsEnabled</span><span class="sxs-lookup"><span data-stu-id="d3692-177">unlockWithBiometricsEnabled</span></span>|<span data-ttu-id="d3692-178">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d3692-178">Boolean</span></span>|<span data-ttu-id="d3692-179">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="d3692-179">Not yet documented</span></span>|
|<span data-ttu-id="d3692-180">remotePassportEnabled</span><span class="sxs-lookup"><span data-stu-id="d3692-180">remotePassportEnabled</span></span>|<span data-ttu-id="d3692-181">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d3692-181">Boolean</span></span>|<span data-ttu-id="d3692-182">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="d3692-182">Not yet documented</span></span>|
|<span data-ttu-id="d3692-183">pinPreviousBlockCount</span><span class="sxs-lookup"><span data-stu-id="d3692-183">pinPreviousBlockCount</span></span>|<span data-ttu-id="d3692-184">Int32</span><span class="sxs-lookup"><span data-stu-id="d3692-184">Int32</span></span>|<span data-ttu-id="d3692-185">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="d3692-185">Not yet documented</span></span>|
|<span data-ttu-id="d3692-186">pinExpirationInDays</span><span class="sxs-lookup"><span data-stu-id="d3692-186">pinExpirationInDays</span></span>|<span data-ttu-id="d3692-187">Int32</span><span class="sxs-lookup"><span data-stu-id="d3692-187">Int32</span></span>|<span data-ttu-id="d3692-188">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="d3692-188">Not yet documented</span></span>|
|<span data-ttu-id="d3692-189">enhancedBiometricsState</span><span class="sxs-lookup"><span data-stu-id="d3692-189">enhancedBiometricsState</span></span>|[<span data-ttu-id="d3692-190">Aktivierung von Steuerelementen</span><span class="sxs-lookup"><span data-stu-id="d3692-190">enablement</span></span>](../resources/intune-onboarding-enablement.md)|<span data-ttu-id="d3692-191">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="d3692-191">Not yet documented.</span></span> <span data-ttu-id="d3692-192">Mögliche Werte sind: `notConfigured`, `enabled` und `disabled`.</span><span class="sxs-lookup"><span data-stu-id="d3692-192">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|



## <a name="response"></a><span data-ttu-id="d3692-193">Antwort</span><span class="sxs-lookup"><span data-stu-id="d3692-193">Response</span></span>
<span data-ttu-id="d3692-194">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="d3692-194">If successful, this method returns a `201 Created` response code and a [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d3692-195">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d3692-195">Example</span></span>
### <a name="request"></a><span data-ttu-id="d3692-196">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d3692-196">Request</span></span>
<span data-ttu-id="d3692-197">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d3692-197">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d3692-198">Antwort</span><span class="sxs-lookup"><span data-stu-id="d3692-198">Response</span></span>
<span data-ttu-id="d3692-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d3692-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


