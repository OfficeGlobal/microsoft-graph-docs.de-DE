---
title: deviceEnrollmentWindowsHelloForBusinessConfiguration erstellen
description: Erstellen eines neuen deviceEnrollmentWindowsHelloForBusinessConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 7f86fd9fc1a8028ab983dce46998046b1515c761
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27983079"
---
# <a name="create-deviceenrollmentwindowshelloforbusinessconfiguration"></a><span data-ttu-id="e1cdb-103">deviceEnrollmentWindowsHelloForBusinessConfiguration erstellen</span><span class="sxs-lookup"><span data-stu-id="e1cdb-103">Create deviceEnrollmentWindowsHelloForBusinessConfiguration</span></span>

> <span data-ttu-id="e1cdb-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="e1cdb-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e1cdb-105">Erstellen eines neuen [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="e1cdb-105">Create a new [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e1cdb-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="e1cdb-106">Prerequisites</span></span>
<span data-ttu-id="e1cdb-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e1cdb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e1cdb-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e1cdb-109">Permission type</span></span>|<span data-ttu-id="e1cdb-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e1cdb-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e1cdb-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e1cdb-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e1cdb-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1cdb-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="e1cdb-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e1cdb-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e1cdb-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e1cdb-114">Not supported.</span></span>|
|<span data-ttu-id="e1cdb-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e1cdb-115">Application</span></span>|<span data-ttu-id="e1cdb-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e1cdb-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e1cdb-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e1cdb-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="e1cdb-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e1cdb-118">Request headers</span></span>
|<span data-ttu-id="e1cdb-119">Header</span><span class="sxs-lookup"><span data-stu-id="e1cdb-119">Header</span></span>|<span data-ttu-id="e1cdb-120">Wert</span><span class="sxs-lookup"><span data-stu-id="e1cdb-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e1cdb-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e1cdb-121">Authorization</span></span>|<span data-ttu-id="e1cdb-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="e1cdb-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e1cdb-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="e1cdb-123">Accept</span></span>|<span data-ttu-id="e1cdb-124">application/json</span><span class="sxs-lookup"><span data-stu-id="e1cdb-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e1cdb-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e1cdb-125">Request body</span></span>
<span data-ttu-id="e1cdb-126">Geben Sie im Anforderungstext eine JSON-Darstellung für das deviceEnrollmentWindowsHelloForBusinessConfiguration-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="e1cdb-126">In the request body, supply a JSON representation for the deviceEnrollmentWindowsHelloForBusinessConfiguration object.</span></span>

<span data-ttu-id="e1cdb-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der deviceEnrollmentWindowsHelloForBusinessConfiguration erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="e1cdb-127">The following table shows the properties that are required when you create the deviceEnrollmentWindowsHelloForBusinessConfiguration.</span></span>

|<span data-ttu-id="e1cdb-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e1cdb-128">Property</span></span>|<span data-ttu-id="e1cdb-129">Typ</span><span class="sxs-lookup"><span data-stu-id="e1cdb-129">Type</span></span>|<span data-ttu-id="e1cdb-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e1cdb-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e1cdb-131">id</span><span class="sxs-lookup"><span data-stu-id="e1cdb-131">id</span></span>|<span data-ttu-id="e1cdb-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e1cdb-132">String</span></span>|<span data-ttu-id="e1cdb-133">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e1cdb-133">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="e1cdb-134">displayName</span><span class="sxs-lookup"><span data-stu-id="e1cdb-134">displayName</span></span>|<span data-ttu-id="e1cdb-135">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e1cdb-135">String</span></span>|<span data-ttu-id="e1cdb-136">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e1cdb-136">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="e1cdb-137">description</span><span class="sxs-lookup"><span data-stu-id="e1cdb-137">description</span></span>|<span data-ttu-id="e1cdb-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e1cdb-138">String</span></span>|<span data-ttu-id="e1cdb-139">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e1cdb-139">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="e1cdb-140">Priorität</span><span class="sxs-lookup"><span data-stu-id="e1cdb-140">priority</span></span>|<span data-ttu-id="e1cdb-141">Int32</span><span class="sxs-lookup"><span data-stu-id="e1cdb-141">Int32</span></span>|<span data-ttu-id="e1cdb-142">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e1cdb-142">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="e1cdb-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e1cdb-143">createdDateTime</span></span>|<span data-ttu-id="e1cdb-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e1cdb-144">DateTimeOffset</span></span>|<span data-ttu-id="e1cdb-145">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e1cdb-145">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="e1cdb-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e1cdb-146">lastModifiedDateTime</span></span>|<span data-ttu-id="e1cdb-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e1cdb-147">DateTimeOffset</span></span>|<span data-ttu-id="e1cdb-148">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e1cdb-148">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="e1cdb-149">Version</span><span class="sxs-lookup"><span data-stu-id="e1cdb-149">version</span></span>|<span data-ttu-id="e1cdb-150">Int32</span><span class="sxs-lookup"><span data-stu-id="e1cdb-150">Int32</span></span>|<span data-ttu-id="e1cdb-151">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e1cdb-151">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="e1cdb-152">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="e1cdb-152">pinMinimumLength</span></span>|<span data-ttu-id="e1cdb-153">Int32</span><span class="sxs-lookup"><span data-stu-id="e1cdb-153">Int32</span></span>|<span data-ttu-id="e1cdb-154">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="e1cdb-154">Not yet documented</span></span>|
|<span data-ttu-id="e1cdb-155">pinMaximumLength</span><span class="sxs-lookup"><span data-stu-id="e1cdb-155">pinMaximumLength</span></span>|<span data-ttu-id="e1cdb-156">Int32</span><span class="sxs-lookup"><span data-stu-id="e1cdb-156">Int32</span></span>|<span data-ttu-id="e1cdb-157">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="e1cdb-157">Not yet documented</span></span>|
|<span data-ttu-id="e1cdb-158">pinUppercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="e1cdb-158">pinUppercaseCharactersUsage</span></span>|[<span data-ttu-id="e1cdb-159">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="e1cdb-159">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="e1cdb-160">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="e1cdb-160">Not yet documented.</span></span> <span data-ttu-id="e1cdb-161">Mögliche Werte sind: `allowed`, `required` und `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="e1cdb-161">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="e1cdb-162">pinLowercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="e1cdb-162">pinLowercaseCharactersUsage</span></span>|[<span data-ttu-id="e1cdb-163">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="e1cdb-163">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="e1cdb-164">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="e1cdb-164">Not yet documented.</span></span> <span data-ttu-id="e1cdb-165">Mögliche Werte sind: `allowed`, `required` und `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="e1cdb-165">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="e1cdb-166">pinSpecialCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="e1cdb-166">pinSpecialCharactersUsage</span></span>|[<span data-ttu-id="e1cdb-167">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="e1cdb-167">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="e1cdb-168">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="e1cdb-168">Not yet documented.</span></span> <span data-ttu-id="e1cdb-169">Mögliche Werte sind: `allowed`, `required` und `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="e1cdb-169">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="e1cdb-170">Zustand</span><span class="sxs-lookup"><span data-stu-id="e1cdb-170">state</span></span>|[<span data-ttu-id="e1cdb-171">Aktivierung von Steuerelementen</span><span class="sxs-lookup"><span data-stu-id="e1cdb-171">enablement</span></span>](../resources/intune-onboarding-enablement.md)|<span data-ttu-id="e1cdb-172">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="e1cdb-172">Not yet documented.</span></span> <span data-ttu-id="e1cdb-173">Mögliche Werte sind: `notConfigured`, `enabled` und `disabled`.</span><span class="sxs-lookup"><span data-stu-id="e1cdb-173">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="e1cdb-174">securityDeviceRequired</span><span class="sxs-lookup"><span data-stu-id="e1cdb-174">securityDeviceRequired</span></span>|<span data-ttu-id="e1cdb-175">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="e1cdb-175">Boolean</span></span>|<span data-ttu-id="e1cdb-176">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="e1cdb-176">Not yet documented</span></span>|
|<span data-ttu-id="e1cdb-177">unlockWithBiometricsEnabled</span><span class="sxs-lookup"><span data-stu-id="e1cdb-177">unlockWithBiometricsEnabled</span></span>|<span data-ttu-id="e1cdb-178">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="e1cdb-178">Boolean</span></span>|<span data-ttu-id="e1cdb-179">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="e1cdb-179">Not yet documented</span></span>|
|<span data-ttu-id="e1cdb-180">remotePassportEnabled</span><span class="sxs-lookup"><span data-stu-id="e1cdb-180">remotePassportEnabled</span></span>|<span data-ttu-id="e1cdb-181">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="e1cdb-181">Boolean</span></span>|<span data-ttu-id="e1cdb-182">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="e1cdb-182">Not yet documented</span></span>|
|<span data-ttu-id="e1cdb-183">pinPreviousBlockCount</span><span class="sxs-lookup"><span data-stu-id="e1cdb-183">pinPreviousBlockCount</span></span>|<span data-ttu-id="e1cdb-184">Int32</span><span class="sxs-lookup"><span data-stu-id="e1cdb-184">Int32</span></span>|<span data-ttu-id="e1cdb-185">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="e1cdb-185">Not yet documented</span></span>|
|<span data-ttu-id="e1cdb-186">pinExpirationInDays</span><span class="sxs-lookup"><span data-stu-id="e1cdb-186">pinExpirationInDays</span></span>|<span data-ttu-id="e1cdb-187">Int32</span><span class="sxs-lookup"><span data-stu-id="e1cdb-187">Int32</span></span>|<span data-ttu-id="e1cdb-188">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="e1cdb-188">Not yet documented</span></span>|
|<span data-ttu-id="e1cdb-189">enhancedBiometricsState</span><span class="sxs-lookup"><span data-stu-id="e1cdb-189">enhancedBiometricsState</span></span>|[<span data-ttu-id="e1cdb-190">Aktivierung von Steuerelementen</span><span class="sxs-lookup"><span data-stu-id="e1cdb-190">enablement</span></span>](../resources/intune-onboarding-enablement.md)|<span data-ttu-id="e1cdb-191">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="e1cdb-191">Not yet documented.</span></span> <span data-ttu-id="e1cdb-192">Mögliche Werte sind: `notConfigured`, `enabled` und `disabled`.</span><span class="sxs-lookup"><span data-stu-id="e1cdb-192">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|



## <a name="response"></a><span data-ttu-id="e1cdb-193">Antwort</span><span class="sxs-lookup"><span data-stu-id="e1cdb-193">Response</span></span>
<span data-ttu-id="e1cdb-194">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="e1cdb-194">If successful, this method returns a `201 Created` response code and a [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e1cdb-195">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e1cdb-195">Example</span></span>
### <a name="request"></a><span data-ttu-id="e1cdb-196">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e1cdb-196">Request</span></span>
<span data-ttu-id="e1cdb-197">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e1cdb-197">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e1cdb-198">Antwort</span><span class="sxs-lookup"><span data-stu-id="e1cdb-198">Response</span></span>
<span data-ttu-id="e1cdb-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e1cdb-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



