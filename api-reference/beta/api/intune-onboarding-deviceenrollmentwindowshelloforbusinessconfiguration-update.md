---
title: deviceEnrollmentWindowsHelloForBusinessConfiguration aktualisieren
description: Aktualisieren der Eigenschaften eines deviceEnrollmentWindowsHelloForBusinessConfiguration-Objekts.
ms.openlocfilehash: 44624aaf7f073d67f8623bdaee8266c80596a90d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059390"
---
# <a name="update-deviceenrollmentwindowshelloforbusinessconfiguration"></a><span data-ttu-id="d14f5-103">deviceEnrollmentWindowsHelloForBusinessConfiguration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="d14f5-103">Update deviceEnrollmentWindowsHelloForBusinessConfiguration</span></span>

> <span data-ttu-id="d14f5-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="d14f5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d14f5-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d14f5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d14f5-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="d14f5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d14f5-107">Aktualisieren der Eigenschaften eines [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="d14f5-107">Update the properties of a [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d14f5-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="d14f5-108">Prerequisites</span></span>
<span data-ttu-id="d14f5-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d14f5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d14f5-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d14f5-111">Permission type</span></span>|<span data-ttu-id="d14f5-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d14f5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d14f5-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d14f5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d14f5-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d14f5-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="d14f5-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d14f5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d14f5-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d14f5-116">Not supported.</span></span>|
|<span data-ttu-id="d14f5-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d14f5-117">Application</span></span>|<span data-ttu-id="d14f5-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d14f5-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d14f5-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d14f5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="d14f5-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d14f5-120">Request headers</span></span>
|<span data-ttu-id="d14f5-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="d14f5-121">Header</span></span>|<span data-ttu-id="d14f5-122">Wert</span><span class="sxs-lookup"><span data-stu-id="d14f5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d14f5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d14f5-123">Authorization</span></span>|<span data-ttu-id="d14f5-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="d14f5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d14f5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d14f5-125">Accept</span></span>|<span data-ttu-id="d14f5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d14f5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d14f5-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d14f5-127">Request body</span></span>
<span data-ttu-id="d14f5-128">Geben Sie im Anforderungstext eine JSON-Darstellung für das [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md)-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="d14f5-128">In the request body, supply a JSON representation for the [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>

<span data-ttu-id="d14f5-129">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="d14f5-129">The following table shows the properties that are required when you create the [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md).</span></span>

|<span data-ttu-id="d14f5-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d14f5-130">Property</span></span>|<span data-ttu-id="d14f5-131">Typ</span><span class="sxs-lookup"><span data-stu-id="d14f5-131">Type</span></span>|<span data-ttu-id="d14f5-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d14f5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d14f5-133">id</span><span class="sxs-lookup"><span data-stu-id="d14f5-133">id</span></span>|<span data-ttu-id="d14f5-134">String</span><span class="sxs-lookup"><span data-stu-id="d14f5-134">String</span></span>|<span data-ttu-id="d14f5-135">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d14f5-135">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d14f5-136">displayName</span><span class="sxs-lookup"><span data-stu-id="d14f5-136">displayName</span></span>|<span data-ttu-id="d14f5-137">String</span><span class="sxs-lookup"><span data-stu-id="d14f5-137">String</span></span>|<span data-ttu-id="d14f5-138">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d14f5-138">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d14f5-139">description</span><span class="sxs-lookup"><span data-stu-id="d14f5-139">description</span></span>|<span data-ttu-id="d14f5-140">String</span><span class="sxs-lookup"><span data-stu-id="d14f5-140">String</span></span>|<span data-ttu-id="d14f5-141">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d14f5-141">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d14f5-142">Priorität</span><span class="sxs-lookup"><span data-stu-id="d14f5-142">priority</span></span>|<span data-ttu-id="d14f5-143">Int32</span><span class="sxs-lookup"><span data-stu-id="d14f5-143">Int32</span></span>|<span data-ttu-id="d14f5-144">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d14f5-144">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d14f5-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d14f5-145">createdDateTime</span></span>|<span data-ttu-id="d14f5-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d14f5-146">DateTimeOffset</span></span>|<span data-ttu-id="d14f5-147">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d14f5-147">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d14f5-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d14f5-148">lastModifiedDateTime</span></span>|<span data-ttu-id="d14f5-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d14f5-149">DateTimeOffset</span></span>|<span data-ttu-id="d14f5-150">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d14f5-150">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d14f5-151">Version</span><span class="sxs-lookup"><span data-stu-id="d14f5-151">version</span></span>|<span data-ttu-id="d14f5-152">Int32</span><span class="sxs-lookup"><span data-stu-id="d14f5-152">Int32</span></span>|<span data-ttu-id="d14f5-153">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d14f5-153">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d14f5-154">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="d14f5-154">pinMinimumLength</span></span>|<span data-ttu-id="d14f5-155">Int32</span><span class="sxs-lookup"><span data-stu-id="d14f5-155">Int32</span></span>|<span data-ttu-id="d14f5-156">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="d14f5-156">Not yet documented</span></span>|
|<span data-ttu-id="d14f5-157">pinMaximumLength</span><span class="sxs-lookup"><span data-stu-id="d14f5-157">pinMaximumLength</span></span>|<span data-ttu-id="d14f5-158">Int32</span><span class="sxs-lookup"><span data-stu-id="d14f5-158">Int32</span></span>|<span data-ttu-id="d14f5-159">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="d14f5-159">Not yet documented</span></span>|
|<span data-ttu-id="d14f5-160">pinUppercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="d14f5-160">pinUppercaseCharactersUsage</span></span>|[<span data-ttu-id="d14f5-161">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="d14f5-161">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="d14f5-162">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="d14f5-162">Not yet documented.</span></span> <span data-ttu-id="d14f5-163">Mögliche Werte sind: `allowed`, `required` und `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="d14f5-163">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="d14f5-164">pinLowercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="d14f5-164">pinLowercaseCharactersUsage</span></span>|[<span data-ttu-id="d14f5-165">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="d14f5-165">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="d14f5-166">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="d14f5-166">Not yet documented.</span></span> <span data-ttu-id="d14f5-167">Mögliche Werte sind: `allowed`, `required` und `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="d14f5-167">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="d14f5-168">pinSpecialCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="d14f5-168">pinSpecialCharactersUsage</span></span>|[<span data-ttu-id="d14f5-169">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="d14f5-169">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="d14f5-170">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="d14f5-170">Not yet documented.</span></span> <span data-ttu-id="d14f5-171">Mögliche Werte sind: `allowed`, `required` und `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="d14f5-171">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="d14f5-172">state</span><span class="sxs-lookup"><span data-stu-id="d14f5-172">state</span></span>|[<span data-ttu-id="d14f5-173">Aktivierung von Steuerelementen</span><span class="sxs-lookup"><span data-stu-id="d14f5-173">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="d14f5-174">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="d14f5-174">Not yet documented.</span></span> <span data-ttu-id="d14f5-175">Mögliche Werte sind: `notConfigured`, `enabled` und `disabled`.</span><span class="sxs-lookup"><span data-stu-id="d14f5-175">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="d14f5-176">securityDeviceRequired</span><span class="sxs-lookup"><span data-stu-id="d14f5-176">securityDeviceRequired</span></span>|<span data-ttu-id="d14f5-177">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d14f5-177">Boolean</span></span>|<span data-ttu-id="d14f5-178">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="d14f5-178">Not yet documented</span></span>|
|<span data-ttu-id="d14f5-179">unlockWithBiometricsEnabled</span><span class="sxs-lookup"><span data-stu-id="d14f5-179">unlockWithBiometricsEnabled</span></span>|<span data-ttu-id="d14f5-180">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d14f5-180">Boolean</span></span>|<span data-ttu-id="d14f5-181">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="d14f5-181">Not yet documented</span></span>|
|<span data-ttu-id="d14f5-182">remotePassportEnabled</span><span class="sxs-lookup"><span data-stu-id="d14f5-182">remotePassportEnabled</span></span>|<span data-ttu-id="d14f5-183">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d14f5-183">Boolean</span></span>|<span data-ttu-id="d14f5-184">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="d14f5-184">Not yet documented</span></span>|
|<span data-ttu-id="d14f5-185">pinPreviousBlockCount</span><span class="sxs-lookup"><span data-stu-id="d14f5-185">pinPreviousBlockCount</span></span>|<span data-ttu-id="d14f5-186">Int32</span><span class="sxs-lookup"><span data-stu-id="d14f5-186">Int32</span></span>|<span data-ttu-id="d14f5-187">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="d14f5-187">Not yet documented</span></span>|
|<span data-ttu-id="d14f5-188">pinExpirationInDays</span><span class="sxs-lookup"><span data-stu-id="d14f5-188">pinExpirationInDays</span></span>|<span data-ttu-id="d14f5-189">Int32</span><span class="sxs-lookup"><span data-stu-id="d14f5-189">Int32</span></span>|<span data-ttu-id="d14f5-190">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="d14f5-190">Not yet documented</span></span>|
|<span data-ttu-id="d14f5-191">enhancedBiometricsState</span><span class="sxs-lookup"><span data-stu-id="d14f5-191">enhancedBiometricsState</span></span>|[<span data-ttu-id="d14f5-192">Aktivierung von Steuerelementen</span><span class="sxs-lookup"><span data-stu-id="d14f5-192">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="d14f5-193">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="d14f5-193">Not yet documented.</span></span> <span data-ttu-id="d14f5-194">Mögliche Werte sind: `notConfigured`, `enabled` und `disabled`.</span><span class="sxs-lookup"><span data-stu-id="d14f5-194">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|



## <a name="response"></a><span data-ttu-id="d14f5-195">Antwort</span><span class="sxs-lookup"><span data-stu-id="d14f5-195">Response</span></span>
<span data-ttu-id="d14f5-196">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="d14f5-196">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d14f5-197">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d14f5-197">Example</span></span>
### <a name="request"></a><span data-ttu-id="d14f5-198">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d14f5-198">Request</span></span>
<span data-ttu-id="d14f5-199">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d14f5-199">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
Content-type: application/json
Content-length: 602

{
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
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

### <a name="response"></a><span data-ttu-id="d14f5-200">Antwort</span><span class="sxs-lookup"><span data-stu-id="d14f5-200">Response</span></span>
<span data-ttu-id="d14f5-p108">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d14f5-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





