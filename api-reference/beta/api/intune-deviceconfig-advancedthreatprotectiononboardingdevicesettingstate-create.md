---
title: Erstellen von advancedThreatProtectionOnboardingDeviceSettingState
description: Erstellen eines neuen AdvancedThreatProtectionOnboardingDeviceSettingState-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 87db4f3c58a8f205ec6c72805d766e510dbb4188
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29394691"
---
# <a name="create-advancedthreatprotectiononboardingdevicesettingstate"></a><span data-ttu-id="79f1d-103">Erstellen von advancedThreatProtectionOnboardingDeviceSettingState</span><span class="sxs-lookup"><span data-stu-id="79f1d-103">Create advancedThreatProtectionOnboardingDeviceSettingState</span></span>

> <span data-ttu-id="79f1d-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="79f1d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="79f1d-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="79f1d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="79f1d-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="79f1d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="79f1d-107">Erstellen eines neuen [AdvancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="79f1d-107">Create a new [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="79f1d-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="79f1d-108">Prerequisites</span></span>
<span data-ttu-id="79f1d-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="79f1d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="79f1d-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="79f1d-111">Permission type</span></span>|<span data-ttu-id="79f1d-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="79f1d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="79f1d-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="79f1d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="79f1d-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79f1d-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="79f1d-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="79f1d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="79f1d-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="79f1d-116">Not supported.</span></span>|
|<span data-ttu-id="79f1d-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="79f1d-117">Application</span></span>|<span data-ttu-id="79f1d-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="79f1d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="79f1d-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="79f1d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/advancedThreatProtectionOnboardingStateSummary/advancedThreatProtectionOnboardingDeviceSettingStates
```

## <a name="request-headers"></a><span data-ttu-id="79f1d-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="79f1d-120">Request headers</span></span>
|<span data-ttu-id="79f1d-121">Header</span><span class="sxs-lookup"><span data-stu-id="79f1d-121">Header</span></span>|<span data-ttu-id="79f1d-122">Wert</span><span class="sxs-lookup"><span data-stu-id="79f1d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="79f1d-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="79f1d-123">Authorization</span></span>|<span data-ttu-id="79f1d-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="79f1d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="79f1d-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="79f1d-125">Accept</span></span>|<span data-ttu-id="79f1d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="79f1d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="79f1d-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="79f1d-127">Request body</span></span>
<span data-ttu-id="79f1d-128">Geben Sie im Textkörper Anforderung für das Objekt AdvancedThreatProtectionOnboardingDeviceSettingState eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="79f1d-128">In the request body, supply a JSON representation for the advancedThreatProtectionOnboardingDeviceSettingState object.</span></span>

<span data-ttu-id="79f1d-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die AdvancedThreatProtectionOnboardingDeviceSettingState erstellen.</span><span class="sxs-lookup"><span data-stu-id="79f1d-129">The following table shows the properties that are required when you create the advancedThreatProtectionOnboardingDeviceSettingState.</span></span>

|<span data-ttu-id="79f1d-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="79f1d-130">Property</span></span>|<span data-ttu-id="79f1d-131">Typ</span><span class="sxs-lookup"><span data-stu-id="79f1d-131">Type</span></span>|<span data-ttu-id="79f1d-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="79f1d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="79f1d-133">id</span><span class="sxs-lookup"><span data-stu-id="79f1d-133">id</span></span>|<span data-ttu-id="79f1d-134">String</span><span class="sxs-lookup"><span data-stu-id="79f1d-134">String</span></span>|<span data-ttu-id="79f1d-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="79f1d-135">Key of the entity</span></span>|
|<span data-ttu-id="79f1d-136">platformType</span><span class="sxs-lookup"><span data-stu-id="79f1d-136">platformType</span></span>|[<span data-ttu-id="79f1d-137">deviceType</span><span class="sxs-lookup"><span data-stu-id="79f1d-137">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="79f1d-138">Gerätetyp-Plattform.</span><span class="sxs-lookup"><span data-stu-id="79f1d-138">Device platform type.</span></span> <span data-ttu-id="79f1d-139">Mögliche Werte sind: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise` , `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="79f1d-139">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="79f1d-140">setting</span><span class="sxs-lookup"><span data-stu-id="79f1d-140">setting</span></span>|<span data-ttu-id="79f1d-141">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="79f1d-141">String</span></span>|<span data-ttu-id="79f1d-142">Klassenname und Eigenschaftenname der Einstellung</span><span class="sxs-lookup"><span data-stu-id="79f1d-142">The setting class name and property name.</span></span>|
|<span data-ttu-id="79f1d-143">settingName</span><span class="sxs-lookup"><span data-stu-id="79f1d-143">settingName</span></span>|<span data-ttu-id="79f1d-144">String</span><span class="sxs-lookup"><span data-stu-id="79f1d-144">String</span></span>|<span data-ttu-id="79f1d-145">Gemeldeter Einstellungsname</span><span class="sxs-lookup"><span data-stu-id="79f1d-145">The Setting Name that is being reported</span></span>|
|<span data-ttu-id="79f1d-146">deviceId</span><span class="sxs-lookup"><span data-stu-id="79f1d-146">deviceId</span></span>|<span data-ttu-id="79f1d-147">String</span><span class="sxs-lookup"><span data-stu-id="79f1d-147">String</span></span>|<span data-ttu-id="79f1d-148">Gemeldete Geräte-ID</span><span class="sxs-lookup"><span data-stu-id="79f1d-148">The Device Id that is being reported</span></span>|
|<span data-ttu-id="79f1d-149">deviceName</span><span class="sxs-lookup"><span data-stu-id="79f1d-149">deviceName</span></span>|<span data-ttu-id="79f1d-150">String</span><span class="sxs-lookup"><span data-stu-id="79f1d-150">String</span></span>|<span data-ttu-id="79f1d-151">Gemeldeter Gerätename</span><span class="sxs-lookup"><span data-stu-id="79f1d-151">The Device Name that is being reported</span></span>|
|<span data-ttu-id="79f1d-152">userId</span><span class="sxs-lookup"><span data-stu-id="79f1d-152">userId</span></span>|<span data-ttu-id="79f1d-153">String</span><span class="sxs-lookup"><span data-stu-id="79f1d-153">String</span></span>|<span data-ttu-id="79f1d-154">Gemeldete Benutzer-ID</span><span class="sxs-lookup"><span data-stu-id="79f1d-154">The user Id that is being reported</span></span>|
|<span data-ttu-id="79f1d-155">userEmail</span><span class="sxs-lookup"><span data-stu-id="79f1d-155">userEmail</span></span>|<span data-ttu-id="79f1d-156">String</span><span class="sxs-lookup"><span data-stu-id="79f1d-156">String</span></span>|<span data-ttu-id="79f1d-157">Gemeldete Benutzer-E-Mail-Adresse</span><span class="sxs-lookup"><span data-stu-id="79f1d-157">The User email address that is being reported</span></span>|
|<span data-ttu-id="79f1d-158">userName</span><span class="sxs-lookup"><span data-stu-id="79f1d-158">userName</span></span>|<span data-ttu-id="79f1d-159">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="79f1d-159">String</span></span>|<span data-ttu-id="79f1d-160">Gemeldeter Benutzername</span><span class="sxs-lookup"><span data-stu-id="79f1d-160">The User Name that is being reported</span></span>|
|<span data-ttu-id="79f1d-161">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="79f1d-161">userPrincipalName</span></span>|<span data-ttu-id="79f1d-162">String</span><span class="sxs-lookup"><span data-stu-id="79f1d-162">String</span></span>|<span data-ttu-id="79f1d-163">Gemeldeter Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="79f1d-163">The User PrincipalName that is being reported</span></span>|
|<span data-ttu-id="79f1d-164">deviceModel</span><span class="sxs-lookup"><span data-stu-id="79f1d-164">deviceModel</span></span>|<span data-ttu-id="79f1d-165">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="79f1d-165">String</span></span>|<span data-ttu-id="79f1d-166">Gemeldetes Gerätemodell</span><span class="sxs-lookup"><span data-stu-id="79f1d-166">The device model that is being reported</span></span>|
|<span data-ttu-id="79f1d-167">state</span><span class="sxs-lookup"><span data-stu-id="79f1d-167">state</span></span>|[<span data-ttu-id="79f1d-168">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="79f1d-168">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="79f1d-169">Der Compliance-Zustand der Einstellung.</span><span class="sxs-lookup"><span data-stu-id="79f1d-169">The compliance state of the setting.</span></span> <span data-ttu-id="79f1d-170">Mögliche Werte sind: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict` und `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="79f1d-170">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="79f1d-171">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="79f1d-171">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="79f1d-172">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="79f1d-172">DateTimeOffset</span></span>|<span data-ttu-id="79f1d-173">Datum und Uhrzeit des Ablaufs der Toleranzperiode für die Gerätekonformität</span><span class="sxs-lookup"><span data-stu-id="79f1d-173">The DateTime when device compliance grace period expires</span></span>|



## <a name="response"></a><span data-ttu-id="79f1d-174">Antwort</span><span class="sxs-lookup"><span data-stu-id="79f1d-174">Response</span></span>
<span data-ttu-id="79f1d-175">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [AdvancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="79f1d-175">If successful, this method returns a `201 Created` response code and a [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="79f1d-176">Beispiel</span><span class="sxs-lookup"><span data-stu-id="79f1d-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="79f1d-177">Anforderung</span><span class="sxs-lookup"><span data-stu-id="79f1d-177">Request</span></span>
<span data-ttu-id="79f1d-178">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="79f1d-178">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/advancedThreatProtectionOnboardingStateSummary/advancedThreatProtectionOnboardingDeviceSettingStates
Content-type: application/json
Content-length: 573

{
  "@odata.type": "#microsoft.graph.advancedThreatProtectionOnboardingDeviceSettingState",
  "platformType": "windowsRT",
  "setting": "Setting value",
  "settingName": "Setting Name value",
  "deviceId": "Device Id value",
  "deviceName": "Device Name value",
  "userId": "User Id value",
  "userEmail": "User Email value",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value",
  "deviceModel": "Device Model value",
  "state": "notApplicable",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00"
}
```

### <a name="response"></a><span data-ttu-id="79f1d-179">Antwort</span><span class="sxs-lookup"><span data-stu-id="79f1d-179">Response</span></span>
<span data-ttu-id="79f1d-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="79f1d-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 622

{
  "@odata.type": "#microsoft.graph.advancedThreatProtectionOnboardingDeviceSettingState",
  "id": "63593fc6-3fc6-6359-c63f-5963c63f5963",
  "platformType": "windowsRT",
  "setting": "Setting value",
  "settingName": "Setting Name value",
  "deviceId": "Device Id value",
  "deviceName": "Device Name value",
  "userId": "User Id value",
  "userEmail": "User Email value",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value",
  "deviceModel": "Device Model value",
  "state": "notApplicable",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00"
}
```




