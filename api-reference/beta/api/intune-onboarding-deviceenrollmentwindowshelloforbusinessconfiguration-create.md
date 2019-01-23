---
title: deviceEnrollmentWindowsHelloForBusinessConfiguration erstellen
description: Erstellen eines neuen deviceEnrollmentWindowsHelloForBusinessConfiguration-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7ac406b338d70761c8b14c9100d2eca4cedcb7fd
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29416146"
---
# <a name="create-deviceenrollmentwindowshelloforbusinessconfiguration"></a><span data-ttu-id="04cbf-103">deviceEnrollmentWindowsHelloForBusinessConfiguration erstellen</span><span class="sxs-lookup"><span data-stu-id="04cbf-103">Create deviceEnrollmentWindowsHelloForBusinessConfiguration</span></span>

> <span data-ttu-id="04cbf-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="04cbf-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="04cbf-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="04cbf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="04cbf-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="04cbf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="04cbf-107">Erstellen eines neuen [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="04cbf-107">Create a new [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="04cbf-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="04cbf-108">Prerequisites</span></span>
<span data-ttu-id="04cbf-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="04cbf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="04cbf-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="04cbf-111">Permission type</span></span>|<span data-ttu-id="04cbf-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="04cbf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="04cbf-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="04cbf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="04cbf-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04cbf-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="04cbf-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="04cbf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="04cbf-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="04cbf-116">Not supported.</span></span>|
|<span data-ttu-id="04cbf-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="04cbf-117">Application</span></span>|<span data-ttu-id="04cbf-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="04cbf-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="04cbf-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="04cbf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="04cbf-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="04cbf-120">Request headers</span></span>
|<span data-ttu-id="04cbf-121">Header</span><span class="sxs-lookup"><span data-stu-id="04cbf-121">Header</span></span>|<span data-ttu-id="04cbf-122">Wert</span><span class="sxs-lookup"><span data-stu-id="04cbf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="04cbf-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="04cbf-123">Authorization</span></span>|<span data-ttu-id="04cbf-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="04cbf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="04cbf-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="04cbf-125">Accept</span></span>|<span data-ttu-id="04cbf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="04cbf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="04cbf-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="04cbf-127">Request body</span></span>
<span data-ttu-id="04cbf-128">Geben Sie im Anforderungstext eine JSON-Darstellung für das deviceEnrollmentWindowsHelloForBusinessConfiguration-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="04cbf-128">In the request body, supply a JSON representation for the deviceEnrollmentWindowsHelloForBusinessConfiguration object.</span></span>

<span data-ttu-id="04cbf-129">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der deviceEnrollmentWindowsHelloForBusinessConfiguration erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="04cbf-129">The following table shows the properties that are required when you create the deviceEnrollmentWindowsHelloForBusinessConfiguration.</span></span>

|<span data-ttu-id="04cbf-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="04cbf-130">Property</span></span>|<span data-ttu-id="04cbf-131">Typ</span><span class="sxs-lookup"><span data-stu-id="04cbf-131">Type</span></span>|<span data-ttu-id="04cbf-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="04cbf-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="04cbf-133">id</span><span class="sxs-lookup"><span data-stu-id="04cbf-133">id</span></span>|<span data-ttu-id="04cbf-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="04cbf-134">String</span></span>|<span data-ttu-id="04cbf-135">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="04cbf-135">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="04cbf-136">displayName</span><span class="sxs-lookup"><span data-stu-id="04cbf-136">displayName</span></span>|<span data-ttu-id="04cbf-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="04cbf-137">String</span></span>|<span data-ttu-id="04cbf-138">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="04cbf-138">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="04cbf-139">description</span><span class="sxs-lookup"><span data-stu-id="04cbf-139">description</span></span>|<span data-ttu-id="04cbf-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="04cbf-140">String</span></span>|<span data-ttu-id="04cbf-141">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="04cbf-141">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="04cbf-142">Priorität</span><span class="sxs-lookup"><span data-stu-id="04cbf-142">priority</span></span>|<span data-ttu-id="04cbf-143">Int32</span><span class="sxs-lookup"><span data-stu-id="04cbf-143">Int32</span></span>|<span data-ttu-id="04cbf-144">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="04cbf-144">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="04cbf-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="04cbf-145">createdDateTime</span></span>|<span data-ttu-id="04cbf-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="04cbf-146">DateTimeOffset</span></span>|<span data-ttu-id="04cbf-147">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="04cbf-147">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="04cbf-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="04cbf-148">lastModifiedDateTime</span></span>|<span data-ttu-id="04cbf-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="04cbf-149">DateTimeOffset</span></span>|<span data-ttu-id="04cbf-150">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="04cbf-150">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="04cbf-151">Version</span><span class="sxs-lookup"><span data-stu-id="04cbf-151">version</span></span>|<span data-ttu-id="04cbf-152">Int32</span><span class="sxs-lookup"><span data-stu-id="04cbf-152">Int32</span></span>|<span data-ttu-id="04cbf-153">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="04cbf-153">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="04cbf-154">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="04cbf-154">pinMinimumLength</span></span>|<span data-ttu-id="04cbf-155">Int32</span><span class="sxs-lookup"><span data-stu-id="04cbf-155">Int32</span></span>|<span data-ttu-id="04cbf-156">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="04cbf-156">Not yet documented</span></span>|
|<span data-ttu-id="04cbf-157">pinMaximumLength</span><span class="sxs-lookup"><span data-stu-id="04cbf-157">pinMaximumLength</span></span>|<span data-ttu-id="04cbf-158">Int32</span><span class="sxs-lookup"><span data-stu-id="04cbf-158">Int32</span></span>|<span data-ttu-id="04cbf-159">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="04cbf-159">Not yet documented</span></span>|
|<span data-ttu-id="04cbf-160">pinUppercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="04cbf-160">pinUppercaseCharactersUsage</span></span>|[<span data-ttu-id="04cbf-161">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="04cbf-161">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="04cbf-162">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="04cbf-162">Not yet documented.</span></span> <span data-ttu-id="04cbf-163">Mögliche Werte sind: `allowed`, `required` und `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="04cbf-163">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="04cbf-164">pinLowercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="04cbf-164">pinLowercaseCharactersUsage</span></span>|[<span data-ttu-id="04cbf-165">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="04cbf-165">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="04cbf-166">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="04cbf-166">Not yet documented.</span></span> <span data-ttu-id="04cbf-167">Mögliche Werte sind: `allowed`, `required` und `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="04cbf-167">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="04cbf-168">pinSpecialCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="04cbf-168">pinSpecialCharactersUsage</span></span>|[<span data-ttu-id="04cbf-169">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="04cbf-169">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="04cbf-170">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="04cbf-170">Not yet documented.</span></span> <span data-ttu-id="04cbf-171">Mögliche Werte sind: `allowed`, `required` und `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="04cbf-171">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="04cbf-172">Zustand</span><span class="sxs-lookup"><span data-stu-id="04cbf-172">state</span></span>|[<span data-ttu-id="04cbf-173">Aktivierung von Steuerelementen</span><span class="sxs-lookup"><span data-stu-id="04cbf-173">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="04cbf-174">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="04cbf-174">Not yet documented.</span></span> <span data-ttu-id="04cbf-175">Mögliche Werte sind: `notConfigured`, `enabled` und `disabled`.</span><span class="sxs-lookup"><span data-stu-id="04cbf-175">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="04cbf-176">securityDeviceRequired</span><span class="sxs-lookup"><span data-stu-id="04cbf-176">securityDeviceRequired</span></span>|<span data-ttu-id="04cbf-177">Boolean</span><span class="sxs-lookup"><span data-stu-id="04cbf-177">Boolean</span></span>|<span data-ttu-id="04cbf-178">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="04cbf-178">Not yet documented</span></span>|
|<span data-ttu-id="04cbf-179">unlockWithBiometricsEnabled</span><span class="sxs-lookup"><span data-stu-id="04cbf-179">unlockWithBiometricsEnabled</span></span>|<span data-ttu-id="04cbf-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="04cbf-180">Boolean</span></span>|<span data-ttu-id="04cbf-181">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="04cbf-181">Not yet documented</span></span>|
|<span data-ttu-id="04cbf-182">remotePassportEnabled</span><span class="sxs-lookup"><span data-stu-id="04cbf-182">remotePassportEnabled</span></span>|<span data-ttu-id="04cbf-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="04cbf-183">Boolean</span></span>|<span data-ttu-id="04cbf-184">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="04cbf-184">Not yet documented</span></span>|
|<span data-ttu-id="04cbf-185">pinPreviousBlockCount</span><span class="sxs-lookup"><span data-stu-id="04cbf-185">pinPreviousBlockCount</span></span>|<span data-ttu-id="04cbf-186">Int32</span><span class="sxs-lookup"><span data-stu-id="04cbf-186">Int32</span></span>|<span data-ttu-id="04cbf-187">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="04cbf-187">Not yet documented</span></span>|
|<span data-ttu-id="04cbf-188">pinExpirationInDays</span><span class="sxs-lookup"><span data-stu-id="04cbf-188">pinExpirationInDays</span></span>|<span data-ttu-id="04cbf-189">Int32</span><span class="sxs-lookup"><span data-stu-id="04cbf-189">Int32</span></span>|<span data-ttu-id="04cbf-190">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="04cbf-190">Not yet documented</span></span>|
|<span data-ttu-id="04cbf-191">enhancedBiometricsState</span><span class="sxs-lookup"><span data-stu-id="04cbf-191">enhancedBiometricsState</span></span>|[<span data-ttu-id="04cbf-192">Aktivierung von Steuerelementen</span><span class="sxs-lookup"><span data-stu-id="04cbf-192">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="04cbf-193">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="04cbf-193">Not yet documented.</span></span> <span data-ttu-id="04cbf-194">Mögliche Werte sind: `notConfigured`, `enabled` und `disabled`.</span><span class="sxs-lookup"><span data-stu-id="04cbf-194">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|



## <a name="response"></a><span data-ttu-id="04cbf-195">Antwort</span><span class="sxs-lookup"><span data-stu-id="04cbf-195">Response</span></span>
<span data-ttu-id="04cbf-196">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="04cbf-196">If successful, this method returns a `201 Created` response code and a [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="04cbf-197">Beispiel</span><span class="sxs-lookup"><span data-stu-id="04cbf-197">Example</span></span>

### <a name="request"></a><span data-ttu-id="04cbf-198">Anforderung</span><span class="sxs-lookup"><span data-stu-id="04cbf-198">Request</span></span>
<span data-ttu-id="04cbf-199">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="04cbf-199">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="04cbf-200">Antwort</span><span class="sxs-lookup"><span data-stu-id="04cbf-200">Response</span></span>
<span data-ttu-id="04cbf-p108">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="04cbf-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




