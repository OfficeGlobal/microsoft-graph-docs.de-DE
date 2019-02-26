---
title: AdvancedThreatProtectionOnboardingDeviceSettingState aktualisieren
description: Aktualisieren der Eigenschaften eines advancedThreatProtectionOnboardingDeviceSettingState-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 42a292d824c4e4c80cf4cb47e3812b05f8f733ab
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30142784"
---
# <a name="update-advancedthreatprotectiononboardingdevicesettingstate"></a><span data-ttu-id="7a154-103">AdvancedThreatProtectionOnboardingDeviceSettingState aktualisieren</span><span class="sxs-lookup"><span data-stu-id="7a154-103">Update advancedThreatProtectionOnboardingDeviceSettingState</span></span>

> <span data-ttu-id="7a154-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7a154-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7a154-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="7a154-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7a154-106">Aktualisieren der Eigenschaften eines [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="7a154-106">Update the properties of a [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7a154-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="7a154-107">Prerequisites</span></span>
<span data-ttu-id="7a154-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="7a154-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="7a154-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7a154-110">Permission type</span></span>|<span data-ttu-id="7a154-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7a154-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7a154-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7a154-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7a154-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7a154-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7a154-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7a154-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7a154-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7a154-115">Not supported.</span></span>|
|<span data-ttu-id="7a154-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7a154-116">Application</span></span>|<span data-ttu-id="7a154-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7a154-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7a154-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7a154-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/advancedThreatProtectionOnboardingStateSummary/advancedThreatProtectionOnboardingDeviceSettingStates/{advancedThreatProtectionOnboardingDeviceSettingStateId}
```

## <a name="request-headers"></a><span data-ttu-id="7a154-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7a154-119">Request headers</span></span>
|<span data-ttu-id="7a154-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="7a154-120">Header</span></span>|<span data-ttu-id="7a154-121">Wert</span><span class="sxs-lookup"><span data-stu-id="7a154-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7a154-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7a154-122">Authorization</span></span>|<span data-ttu-id="7a154-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="7a154-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7a154-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="7a154-124">Accept</span></span>|<span data-ttu-id="7a154-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7a154-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7a154-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7a154-126">Request body</span></span>
<span data-ttu-id="7a154-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="7a154-127">In the request body, supply a JSON representation for the [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) object.</span></span>

<span data-ttu-id="7a154-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="7a154-128">The following table shows the properties that are required when you create the [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md).</span></span>

|<span data-ttu-id="7a154-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7a154-129">Property</span></span>|<span data-ttu-id="7a154-130">Typ</span><span class="sxs-lookup"><span data-stu-id="7a154-130">Type</span></span>|<span data-ttu-id="7a154-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7a154-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7a154-132">id</span><span class="sxs-lookup"><span data-stu-id="7a154-132">id</span></span>|<span data-ttu-id="7a154-133">string</span><span class="sxs-lookup"><span data-stu-id="7a154-133">String</span></span>|<span data-ttu-id="7a154-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="7a154-134">Key of the entity</span></span>|
|<span data-ttu-id="7a154-135">platformType</span><span class="sxs-lookup"><span data-stu-id="7a154-135">platformType</span></span>|[<span data-ttu-id="7a154-136">deviceType</span><span class="sxs-lookup"><span data-stu-id="7a154-136">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="7a154-137">Geräte Plattformtyp.</span><span class="sxs-lookup"><span data-stu-id="7a154-137">Device platform type.</span></span> <span data-ttu-id="7a154-138">Mögliche Werte sind: `desktop`, `windowsRT`, `winMO6` `nokia` `windowsPhone` `mac` `winCE` `iPhone` `iPad` `iPod` `android` `iSocConsumer` `unix` `macMDM`,,,,,,,, `holoLens`,, `androidEnterprise` ,,,,,, `surfaceHub` `androidForWork` `winEmbedded` , `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="7a154-138">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="7a154-139">setting</span><span class="sxs-lookup"><span data-stu-id="7a154-139">setting</span></span>|<span data-ttu-id="7a154-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7a154-140">String</span></span>|<span data-ttu-id="7a154-141">Klassenname und Eigenschaftenname der Einstellung</span><span class="sxs-lookup"><span data-stu-id="7a154-141">The setting class name and property name.</span></span>|
|<span data-ttu-id="7a154-142">settingName</span><span class="sxs-lookup"><span data-stu-id="7a154-142">settingName</span></span>|<span data-ttu-id="7a154-143">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7a154-143">String</span></span>|<span data-ttu-id="7a154-144">Gemeldeter Einstellungsname</span><span class="sxs-lookup"><span data-stu-id="7a154-144">The Setting Name that is being reported</span></span>|
|<span data-ttu-id="7a154-145">deviceId</span><span class="sxs-lookup"><span data-stu-id="7a154-145">deviceId</span></span>|<span data-ttu-id="7a154-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7a154-146">String</span></span>|<span data-ttu-id="7a154-147">Gemeldete Geräte-ID</span><span class="sxs-lookup"><span data-stu-id="7a154-147">The Device Id that is being reported</span></span>|
|<span data-ttu-id="7a154-148">deviceName</span><span class="sxs-lookup"><span data-stu-id="7a154-148">deviceName</span></span>|<span data-ttu-id="7a154-149">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7a154-149">String</span></span>|<span data-ttu-id="7a154-150">Gemeldeter Gerätename</span><span class="sxs-lookup"><span data-stu-id="7a154-150">The Device Name that is being reported</span></span>|
|<span data-ttu-id="7a154-151">userId</span><span class="sxs-lookup"><span data-stu-id="7a154-151">userId</span></span>|<span data-ttu-id="7a154-152">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7a154-152">String</span></span>|<span data-ttu-id="7a154-153">Gemeldete Benutzer-ID</span><span class="sxs-lookup"><span data-stu-id="7a154-153">The user Id that is being reported</span></span>|
|<span data-ttu-id="7a154-154">userEmail</span><span class="sxs-lookup"><span data-stu-id="7a154-154">userEmail</span></span>|<span data-ttu-id="7a154-155">String</span><span class="sxs-lookup"><span data-stu-id="7a154-155">String</span></span>|<span data-ttu-id="7a154-156">Gemeldete Benutzer-E-Mail-Adresse</span><span class="sxs-lookup"><span data-stu-id="7a154-156">The User email address that is being reported</span></span>|
|<span data-ttu-id="7a154-157">userName</span><span class="sxs-lookup"><span data-stu-id="7a154-157">userName</span></span>|<span data-ttu-id="7a154-158">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7a154-158">String</span></span>|<span data-ttu-id="7a154-159">Gemeldeter Benutzername</span><span class="sxs-lookup"><span data-stu-id="7a154-159">The User Name that is being reported</span></span>|
|<span data-ttu-id="7a154-160">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="7a154-160">userPrincipalName</span></span>|<span data-ttu-id="7a154-161">String</span><span class="sxs-lookup"><span data-stu-id="7a154-161">String</span></span>|<span data-ttu-id="7a154-162">Gemeldeter Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="7a154-162">The User PrincipalName that is being reported</span></span>|
|<span data-ttu-id="7a154-163">deviceModel</span><span class="sxs-lookup"><span data-stu-id="7a154-163">deviceModel</span></span>|<span data-ttu-id="7a154-164">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7a154-164">String</span></span>|<span data-ttu-id="7a154-165">Gemeldetes Gerätemodell</span><span class="sxs-lookup"><span data-stu-id="7a154-165">The device model that is being reported</span></span>|
|<span data-ttu-id="7a154-166">state</span><span class="sxs-lookup"><span data-stu-id="7a154-166">state</span></span>|[<span data-ttu-id="7a154-167">Wurde</span><span class="sxs-lookup"><span data-stu-id="7a154-167">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="7a154-168">Der Kompatibilitätsstatus der Einstellung.</span><span class="sxs-lookup"><span data-stu-id="7a154-168">The compliance state of the setting.</span></span> <span data-ttu-id="7a154-169">Mögliche Werte sind: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict` und `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="7a154-169">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="7a154-170">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="7a154-170">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="7a154-171">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7a154-171">DateTimeOffset</span></span>|<span data-ttu-id="7a154-172">Datum und Uhrzeit des Ablaufs der Toleranzperiode für die Gerätekonformität</span><span class="sxs-lookup"><span data-stu-id="7a154-172">The DateTime when device compliance grace period expires</span></span>|



## <a name="response"></a><span data-ttu-id="7a154-173">Antwort</span><span class="sxs-lookup"><span data-stu-id="7a154-173">Response</span></span>
<span data-ttu-id="7a154-174">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="7a154-174">If successful, this method returns a `200 OK` response code and an updated [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7a154-175">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7a154-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="7a154-176">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7a154-176">Request</span></span>
<span data-ttu-id="7a154-177">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7a154-177">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/advancedThreatProtectionOnboardingStateSummary/advancedThreatProtectionOnboardingDeviceSettingStates/{advancedThreatProtectionOnboardingDeviceSettingStateId}
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

### <a name="response"></a><span data-ttu-id="7a154-178">Antwort</span><span class="sxs-lookup"><span data-stu-id="7a154-178">Response</span></span>
<span data-ttu-id="7a154-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7a154-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




