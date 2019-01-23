---
title: deviceEnrollmentWindowsHelloForBusinessConfiguration aktualisieren
description: Aktualisieren der Eigenschaften eines deviceEnrollmentWindowsHelloForBusinessConfiguration-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 83b475f1fe467ad73d0bdc63a3c25e3a95761e83
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29411470"
---
# <a name="update-deviceenrollmentwindowshelloforbusinessconfiguration"></a><span data-ttu-id="8105d-103">deviceEnrollmentWindowsHelloForBusinessConfiguration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="8105d-103">Update deviceEnrollmentWindowsHelloForBusinessConfiguration</span></span>

> <span data-ttu-id="8105d-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="8105d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="8105d-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8105d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8105d-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8105d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8105d-107">Aktualisieren der Eigenschaften eines [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="8105d-107">Update the properties of a [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8105d-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="8105d-108">Prerequisites</span></span>
<span data-ttu-id="8105d-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="8105d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="8105d-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8105d-111">Permission type</span></span>|<span data-ttu-id="8105d-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8105d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8105d-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8105d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8105d-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8105d-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="8105d-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8105d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8105d-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8105d-116">Not supported.</span></span>|
|<span data-ttu-id="8105d-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8105d-117">Application</span></span>|<span data-ttu-id="8105d-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8105d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8105d-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8105d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="8105d-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8105d-120">Request headers</span></span>
|<span data-ttu-id="8105d-121">Header</span><span class="sxs-lookup"><span data-stu-id="8105d-121">Header</span></span>|<span data-ttu-id="8105d-122">Wert</span><span class="sxs-lookup"><span data-stu-id="8105d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8105d-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="8105d-123">Authorization</span></span>|<span data-ttu-id="8105d-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="8105d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8105d-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="8105d-125">Accept</span></span>|<span data-ttu-id="8105d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8105d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8105d-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8105d-127">Request body</span></span>
<span data-ttu-id="8105d-128">Geben Sie im Anforderungstext eine JSON-Darstellung für das [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md)-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="8105d-128">In the request body, supply a JSON representation for the [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>

<span data-ttu-id="8105d-129">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="8105d-129">The following table shows the properties that are required when you create the [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md).</span></span>

|<span data-ttu-id="8105d-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8105d-130">Property</span></span>|<span data-ttu-id="8105d-131">Typ</span><span class="sxs-lookup"><span data-stu-id="8105d-131">Type</span></span>|<span data-ttu-id="8105d-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8105d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8105d-133">id</span><span class="sxs-lookup"><span data-stu-id="8105d-133">id</span></span>|<span data-ttu-id="8105d-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8105d-134">String</span></span>|<span data-ttu-id="8105d-135">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8105d-135">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="8105d-136">displayName</span><span class="sxs-lookup"><span data-stu-id="8105d-136">displayName</span></span>|<span data-ttu-id="8105d-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8105d-137">String</span></span>|<span data-ttu-id="8105d-138">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8105d-138">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="8105d-139">description</span><span class="sxs-lookup"><span data-stu-id="8105d-139">description</span></span>|<span data-ttu-id="8105d-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8105d-140">String</span></span>|<span data-ttu-id="8105d-141">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8105d-141">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="8105d-142">Priorität</span><span class="sxs-lookup"><span data-stu-id="8105d-142">priority</span></span>|<span data-ttu-id="8105d-143">Int32</span><span class="sxs-lookup"><span data-stu-id="8105d-143">Int32</span></span>|<span data-ttu-id="8105d-144">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8105d-144">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="8105d-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8105d-145">createdDateTime</span></span>|<span data-ttu-id="8105d-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8105d-146">DateTimeOffset</span></span>|<span data-ttu-id="8105d-147">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8105d-147">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="8105d-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8105d-148">lastModifiedDateTime</span></span>|<span data-ttu-id="8105d-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8105d-149">DateTimeOffset</span></span>|<span data-ttu-id="8105d-150">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8105d-150">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="8105d-151">Version</span><span class="sxs-lookup"><span data-stu-id="8105d-151">version</span></span>|<span data-ttu-id="8105d-152">Int32</span><span class="sxs-lookup"><span data-stu-id="8105d-152">Int32</span></span>|<span data-ttu-id="8105d-153">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8105d-153">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="8105d-154">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="8105d-154">pinMinimumLength</span></span>|<span data-ttu-id="8105d-155">Int32</span><span class="sxs-lookup"><span data-stu-id="8105d-155">Int32</span></span>|<span data-ttu-id="8105d-156">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="8105d-156">Not yet documented</span></span>|
|<span data-ttu-id="8105d-157">pinMaximumLength</span><span class="sxs-lookup"><span data-stu-id="8105d-157">pinMaximumLength</span></span>|<span data-ttu-id="8105d-158">Int32</span><span class="sxs-lookup"><span data-stu-id="8105d-158">Int32</span></span>|<span data-ttu-id="8105d-159">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="8105d-159">Not yet documented</span></span>|
|<span data-ttu-id="8105d-160">pinUppercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="8105d-160">pinUppercaseCharactersUsage</span></span>|[<span data-ttu-id="8105d-161">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="8105d-161">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="8105d-162">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="8105d-162">Not yet documented.</span></span> <span data-ttu-id="8105d-163">Mögliche Werte sind: `allowed`, `required` und `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="8105d-163">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="8105d-164">pinLowercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="8105d-164">pinLowercaseCharactersUsage</span></span>|[<span data-ttu-id="8105d-165">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="8105d-165">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="8105d-166">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="8105d-166">Not yet documented.</span></span> <span data-ttu-id="8105d-167">Mögliche Werte sind: `allowed`, `required` und `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="8105d-167">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="8105d-168">pinSpecialCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="8105d-168">pinSpecialCharactersUsage</span></span>|[<span data-ttu-id="8105d-169">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="8105d-169">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="8105d-170">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="8105d-170">Not yet documented.</span></span> <span data-ttu-id="8105d-171">Mögliche Werte sind: `allowed`, `required` und `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="8105d-171">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="8105d-172">Zustand</span><span class="sxs-lookup"><span data-stu-id="8105d-172">state</span></span>|[<span data-ttu-id="8105d-173">Aktivierung von Steuerelementen</span><span class="sxs-lookup"><span data-stu-id="8105d-173">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="8105d-174">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="8105d-174">Not yet documented.</span></span> <span data-ttu-id="8105d-175">Mögliche Werte sind: `notConfigured`, `enabled` und `disabled`.</span><span class="sxs-lookup"><span data-stu-id="8105d-175">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="8105d-176">securityDeviceRequired</span><span class="sxs-lookup"><span data-stu-id="8105d-176">securityDeviceRequired</span></span>|<span data-ttu-id="8105d-177">Boolean</span><span class="sxs-lookup"><span data-stu-id="8105d-177">Boolean</span></span>|<span data-ttu-id="8105d-178">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="8105d-178">Not yet documented</span></span>|
|<span data-ttu-id="8105d-179">unlockWithBiometricsEnabled</span><span class="sxs-lookup"><span data-stu-id="8105d-179">unlockWithBiometricsEnabled</span></span>|<span data-ttu-id="8105d-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="8105d-180">Boolean</span></span>|<span data-ttu-id="8105d-181">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="8105d-181">Not yet documented</span></span>|
|<span data-ttu-id="8105d-182">remotePassportEnabled</span><span class="sxs-lookup"><span data-stu-id="8105d-182">remotePassportEnabled</span></span>|<span data-ttu-id="8105d-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="8105d-183">Boolean</span></span>|<span data-ttu-id="8105d-184">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="8105d-184">Not yet documented</span></span>|
|<span data-ttu-id="8105d-185">pinPreviousBlockCount</span><span class="sxs-lookup"><span data-stu-id="8105d-185">pinPreviousBlockCount</span></span>|<span data-ttu-id="8105d-186">Int32</span><span class="sxs-lookup"><span data-stu-id="8105d-186">Int32</span></span>|<span data-ttu-id="8105d-187">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="8105d-187">Not yet documented</span></span>|
|<span data-ttu-id="8105d-188">pinExpirationInDays</span><span class="sxs-lookup"><span data-stu-id="8105d-188">pinExpirationInDays</span></span>|<span data-ttu-id="8105d-189">Int32</span><span class="sxs-lookup"><span data-stu-id="8105d-189">Int32</span></span>|<span data-ttu-id="8105d-190">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="8105d-190">Not yet documented</span></span>|
|<span data-ttu-id="8105d-191">enhancedBiometricsState</span><span class="sxs-lookup"><span data-stu-id="8105d-191">enhancedBiometricsState</span></span>|[<span data-ttu-id="8105d-192">Aktivierung von Steuerelementen</span><span class="sxs-lookup"><span data-stu-id="8105d-192">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="8105d-193">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="8105d-193">Not yet documented.</span></span> <span data-ttu-id="8105d-194">Mögliche Werte sind: `notConfigured`, `enabled` und `disabled`.</span><span class="sxs-lookup"><span data-stu-id="8105d-194">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|



## <a name="response"></a><span data-ttu-id="8105d-195">Antwort</span><span class="sxs-lookup"><span data-stu-id="8105d-195">Response</span></span>
<span data-ttu-id="8105d-196">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="8105d-196">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8105d-197">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8105d-197">Example</span></span>

### <a name="request"></a><span data-ttu-id="8105d-198">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8105d-198">Request</span></span>
<span data-ttu-id="8105d-199">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8105d-199">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8105d-200">Antwort</span><span class="sxs-lookup"><span data-stu-id="8105d-200">Response</span></span>
<span data-ttu-id="8105d-p108">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8105d-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




