---
title: deviceEnrollmentWindowsHelloForBusinessConfiguration erstellen
description: Erstellen eines neuen deviceEnrollmentWindowsHelloForBusinessConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 17c8dac652a317020771cbe522295d9a2f5e207d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860725"
---
# <a name="create-deviceenrollmentwindowshelloforbusinessconfiguration"></a><span data-ttu-id="42b73-103">deviceEnrollmentWindowsHelloForBusinessConfiguration erstellen</span><span class="sxs-lookup"><span data-stu-id="42b73-103">Create deviceEnrollmentWindowsHelloForBusinessConfiguration</span></span>

> <span data-ttu-id="42b73-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="42b73-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="42b73-105">Erstellen eines neuen [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="42b73-105">Create a new [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="42b73-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="42b73-106">Prerequisites</span></span>
<span data-ttu-id="42b73-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="42b73-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="42b73-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="42b73-109">Permission type</span></span>|<span data-ttu-id="42b73-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="42b73-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="42b73-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="42b73-111">Delegated (work or school account)</span></span>|<span data-ttu-id="42b73-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42b73-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="42b73-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="42b73-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="42b73-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="42b73-114">Not supported.</span></span>|
|<span data-ttu-id="42b73-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="42b73-115">Application</span></span>|<span data-ttu-id="42b73-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="42b73-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="42b73-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="42b73-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="42b73-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="42b73-118">Request headers</span></span>
|<span data-ttu-id="42b73-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="42b73-119">Header</span></span>|<span data-ttu-id="42b73-120">Wert</span><span class="sxs-lookup"><span data-stu-id="42b73-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="42b73-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="42b73-121">Authorization</span></span>|<span data-ttu-id="42b73-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="42b73-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="42b73-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="42b73-123">Accept</span></span>|<span data-ttu-id="42b73-124">application/json</span><span class="sxs-lookup"><span data-stu-id="42b73-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="42b73-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="42b73-125">Request body</span></span>
<span data-ttu-id="42b73-126">Geben Sie im Anforderungstext eine JSON-Darstellung für das deviceEnrollmentWindowsHelloForBusinessConfiguration-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="42b73-126">In the request body, supply a JSON representation for the deviceEnrollmentWindowsHelloForBusinessConfiguration object.</span></span>

<span data-ttu-id="42b73-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der deviceEnrollmentWindowsHelloForBusinessConfiguration erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="42b73-127">The following table shows the properties that are required when you create the deviceEnrollmentWindowsHelloForBusinessConfiguration.</span></span>

|<span data-ttu-id="42b73-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="42b73-128">Property</span></span>|<span data-ttu-id="42b73-129">Typ</span><span class="sxs-lookup"><span data-stu-id="42b73-129">Type</span></span>|<span data-ttu-id="42b73-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="42b73-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="42b73-131">id</span><span class="sxs-lookup"><span data-stu-id="42b73-131">id</span></span>|<span data-ttu-id="42b73-132">String</span><span class="sxs-lookup"><span data-stu-id="42b73-132">String</span></span>|<span data-ttu-id="42b73-133">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="42b73-133">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="42b73-134">displayName</span><span class="sxs-lookup"><span data-stu-id="42b73-134">displayName</span></span>|<span data-ttu-id="42b73-135">String</span><span class="sxs-lookup"><span data-stu-id="42b73-135">String</span></span>|<span data-ttu-id="42b73-136">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="42b73-136">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="42b73-137">description</span><span class="sxs-lookup"><span data-stu-id="42b73-137">description</span></span>|<span data-ttu-id="42b73-138">String</span><span class="sxs-lookup"><span data-stu-id="42b73-138">String</span></span>|<span data-ttu-id="42b73-139">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="42b73-139">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="42b73-140">Priorität</span><span class="sxs-lookup"><span data-stu-id="42b73-140">priority</span></span>|<span data-ttu-id="42b73-141">Int32</span><span class="sxs-lookup"><span data-stu-id="42b73-141">Int32</span></span>|<span data-ttu-id="42b73-142">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="42b73-142">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="42b73-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="42b73-143">createdDateTime</span></span>|<span data-ttu-id="42b73-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="42b73-144">DateTimeOffset</span></span>|<span data-ttu-id="42b73-145">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="42b73-145">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="42b73-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="42b73-146">lastModifiedDateTime</span></span>|<span data-ttu-id="42b73-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="42b73-147">DateTimeOffset</span></span>|<span data-ttu-id="42b73-148">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="42b73-148">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="42b73-149">Version</span><span class="sxs-lookup"><span data-stu-id="42b73-149">version</span></span>|<span data-ttu-id="42b73-150">Int32</span><span class="sxs-lookup"><span data-stu-id="42b73-150">Int32</span></span>|<span data-ttu-id="42b73-151">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="42b73-151">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="42b73-152">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="42b73-152">pinMinimumLength</span></span>|<span data-ttu-id="42b73-153">Int32</span><span class="sxs-lookup"><span data-stu-id="42b73-153">Int32</span></span>|<span data-ttu-id="42b73-154">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="42b73-154">Not yet documented</span></span>|
|<span data-ttu-id="42b73-155">pinMaximumLength</span><span class="sxs-lookup"><span data-stu-id="42b73-155">pinMaximumLength</span></span>|<span data-ttu-id="42b73-156">Int32</span><span class="sxs-lookup"><span data-stu-id="42b73-156">Int32</span></span>|<span data-ttu-id="42b73-157">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="42b73-157">Not yet documented</span></span>|
|<span data-ttu-id="42b73-158">pinUppercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="42b73-158">pinUppercaseCharactersUsage</span></span>|[<span data-ttu-id="42b73-159">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="42b73-159">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="42b73-160">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="42b73-160">Not yet documented.</span></span> <span data-ttu-id="42b73-161">Mögliche Werte sind: `allowed`, `required` und `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="42b73-161">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="42b73-162">pinLowercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="42b73-162">pinLowercaseCharactersUsage</span></span>|[<span data-ttu-id="42b73-163">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="42b73-163">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="42b73-164">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="42b73-164">Not yet documented.</span></span> <span data-ttu-id="42b73-165">Mögliche Werte sind: `allowed`, `required` und `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="42b73-165">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="42b73-166">pinSpecialCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="42b73-166">pinSpecialCharactersUsage</span></span>|[<span data-ttu-id="42b73-167">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="42b73-167">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="42b73-168">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="42b73-168">Not yet documented.</span></span> <span data-ttu-id="42b73-169">Mögliche Werte sind: `allowed`, `required` und `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="42b73-169">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="42b73-170">state</span><span class="sxs-lookup"><span data-stu-id="42b73-170">state</span></span>|[<span data-ttu-id="42b73-171">Aktivierung von Steuerelementen</span><span class="sxs-lookup"><span data-stu-id="42b73-171">enablement</span></span>](../resources/intune-onboarding-enablement.md)|<span data-ttu-id="42b73-172">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="42b73-172">Not yet documented.</span></span> <span data-ttu-id="42b73-173">Mögliche Werte sind: `notConfigured`, `enabled` und `disabled`.</span><span class="sxs-lookup"><span data-stu-id="42b73-173">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="42b73-174">securityDeviceRequired</span><span class="sxs-lookup"><span data-stu-id="42b73-174">securityDeviceRequired</span></span>|<span data-ttu-id="42b73-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="42b73-175">Boolean</span></span>|<span data-ttu-id="42b73-176">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="42b73-176">Not yet documented</span></span>|
|<span data-ttu-id="42b73-177">unlockWithBiometricsEnabled</span><span class="sxs-lookup"><span data-stu-id="42b73-177">unlockWithBiometricsEnabled</span></span>|<span data-ttu-id="42b73-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="42b73-178">Boolean</span></span>|<span data-ttu-id="42b73-179">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="42b73-179">Not yet documented</span></span>|
|<span data-ttu-id="42b73-180">remotePassportEnabled</span><span class="sxs-lookup"><span data-stu-id="42b73-180">remotePassportEnabled</span></span>|<span data-ttu-id="42b73-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="42b73-181">Boolean</span></span>|<span data-ttu-id="42b73-182">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="42b73-182">Not yet documented</span></span>|
|<span data-ttu-id="42b73-183">pinPreviousBlockCount</span><span class="sxs-lookup"><span data-stu-id="42b73-183">pinPreviousBlockCount</span></span>|<span data-ttu-id="42b73-184">Int32</span><span class="sxs-lookup"><span data-stu-id="42b73-184">Int32</span></span>|<span data-ttu-id="42b73-185">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="42b73-185">Not yet documented</span></span>|
|<span data-ttu-id="42b73-186">pinExpirationInDays</span><span class="sxs-lookup"><span data-stu-id="42b73-186">pinExpirationInDays</span></span>|<span data-ttu-id="42b73-187">Int32</span><span class="sxs-lookup"><span data-stu-id="42b73-187">Int32</span></span>|<span data-ttu-id="42b73-188">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="42b73-188">Not yet documented</span></span>|
|<span data-ttu-id="42b73-189">enhancedBiometricsState</span><span class="sxs-lookup"><span data-stu-id="42b73-189">enhancedBiometricsState</span></span>|[<span data-ttu-id="42b73-190">Aktivierung von Steuerelementen</span><span class="sxs-lookup"><span data-stu-id="42b73-190">enablement</span></span>](../resources/intune-onboarding-enablement.md)|<span data-ttu-id="42b73-191">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="42b73-191">Not yet documented.</span></span> <span data-ttu-id="42b73-192">Mögliche Werte sind: `notConfigured`, `enabled` und `disabled`.</span><span class="sxs-lookup"><span data-stu-id="42b73-192">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|



## <a name="response"></a><span data-ttu-id="42b73-193">Antwort</span><span class="sxs-lookup"><span data-stu-id="42b73-193">Response</span></span>
<span data-ttu-id="42b73-194">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="42b73-194">If successful, this method returns a `201 Created` response code and a [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="42b73-195">Beispiel</span><span class="sxs-lookup"><span data-stu-id="42b73-195">Example</span></span>
### <a name="request"></a><span data-ttu-id="42b73-196">Anforderung</span><span class="sxs-lookup"><span data-stu-id="42b73-196">Request</span></span>
<span data-ttu-id="42b73-197">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="42b73-197">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="42b73-198">Antwort</span><span class="sxs-lookup"><span data-stu-id="42b73-198">Response</span></span>
<span data-ttu-id="42b73-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="42b73-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



