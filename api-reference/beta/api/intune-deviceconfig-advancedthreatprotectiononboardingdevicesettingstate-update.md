---
title: AdvancedThreatProtectionOnboardingDeviceSettingState aktualisieren
description: Aktualisieren der Eigenschaften eines advancedThreatProtectionOnboardingDeviceSettingState-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 320fe73fd1ba54c888d5e56af215cc43b080965b
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30982336"
---
# <a name="update-advancedthreatprotectiononboardingdevicesettingstate"></a><span data-ttu-id="f6435-103">AdvancedThreatProtectionOnboardingDeviceSettingState aktualisieren</span><span class="sxs-lookup"><span data-stu-id="f6435-103">Update advancedThreatProtectionOnboardingDeviceSettingState</span></span>

> <span data-ttu-id="f6435-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f6435-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f6435-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="f6435-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f6435-106">Aktualisieren der Eigenschaften eines [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="f6435-106">Update the properties of a [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f6435-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f6435-107">Prerequisites</span></span>
<span data-ttu-id="f6435-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f6435-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f6435-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f6435-110">Permission type</span></span>|<span data-ttu-id="f6435-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f6435-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f6435-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f6435-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f6435-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6435-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f6435-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f6435-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f6435-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f6435-115">Not supported.</span></span>|
|<span data-ttu-id="f6435-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f6435-116">Application</span></span>|<span data-ttu-id="f6435-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f6435-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f6435-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f6435-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/advancedThreatProtectionOnboardingStateSummary/advancedThreatProtectionOnboardingDeviceSettingStates/{advancedThreatProtectionOnboardingDeviceSettingStateId}
```

## <a name="request-headers"></a><span data-ttu-id="f6435-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f6435-119">Request headers</span></span>
|<span data-ttu-id="f6435-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="f6435-120">Header</span></span>|<span data-ttu-id="f6435-121">Wert</span><span class="sxs-lookup"><span data-stu-id="f6435-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f6435-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f6435-122">Authorization</span></span>|<span data-ttu-id="f6435-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="f6435-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f6435-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="f6435-124">Accept</span></span>|<span data-ttu-id="f6435-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f6435-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f6435-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f6435-126">Request body</span></span>
<span data-ttu-id="f6435-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="f6435-127">In the request body, supply a JSON representation for the [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) object.</span></span>

<span data-ttu-id="f6435-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="f6435-128">The following table shows the properties that are required when you create the [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md).</span></span>

|<span data-ttu-id="f6435-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f6435-129">Property</span></span>|<span data-ttu-id="f6435-130">Typ</span><span class="sxs-lookup"><span data-stu-id="f6435-130">Type</span></span>|<span data-ttu-id="f6435-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f6435-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f6435-132">id</span><span class="sxs-lookup"><span data-stu-id="f6435-132">id</span></span>|<span data-ttu-id="f6435-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f6435-133">String</span></span>|<span data-ttu-id="f6435-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="f6435-134">Key of the entity</span></span>|
|<span data-ttu-id="f6435-135">platformType</span><span class="sxs-lookup"><span data-stu-id="f6435-135">platformType</span></span>|[<span data-ttu-id="f6435-136">deviceType</span><span class="sxs-lookup"><span data-stu-id="f6435-136">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="f6435-137">Geräte Plattformtyp.</span><span class="sxs-lookup"><span data-stu-id="f6435-137">Device platform type.</span></span> <span data-ttu-id="f6435-138">Mögliche Werte sind: `desktop`, `windowsRT`, `winMO6` `nokia` `windowsPhone` `mac` `winCE` `iPhone` `iPad` `iPod` `android` `iSocConsumer` `unix` `macMDM`,,,,,,,, `holoLens`,, `androidEnterprise` ,,,,,, `surfaceHub` `androidForWork` `winEmbedded` , `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="f6435-138">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="f6435-139">Einstellung</span><span class="sxs-lookup"><span data-stu-id="f6435-139">setting</span></span>|<span data-ttu-id="f6435-140">String</span><span class="sxs-lookup"><span data-stu-id="f6435-140">String</span></span>|<span data-ttu-id="f6435-141">Der Klassenname und der Eigenschaftenname der Einstellung.</span><span class="sxs-lookup"><span data-stu-id="f6435-141">The setting class name and property name.</span></span>|
|<span data-ttu-id="f6435-142">settingName</span><span class="sxs-lookup"><span data-stu-id="f6435-142">settingName</span></span>|<span data-ttu-id="f6435-143">String</span><span class="sxs-lookup"><span data-stu-id="f6435-143">String</span></span>|<span data-ttu-id="f6435-144">Der gemeldete Einstellungsname</span><span class="sxs-lookup"><span data-stu-id="f6435-144">The Setting Name that is being reported</span></span>|
|<span data-ttu-id="f6435-145">deviceId</span><span class="sxs-lookup"><span data-stu-id="f6435-145">deviceId</span></span>|<span data-ttu-id="f6435-146">String</span><span class="sxs-lookup"><span data-stu-id="f6435-146">String</span></span>|<span data-ttu-id="f6435-147">Die gemeldete Geräte-ID</span><span class="sxs-lookup"><span data-stu-id="f6435-147">The Device Id that is being reported</span></span>|
|<span data-ttu-id="f6435-148">deviceName</span><span class="sxs-lookup"><span data-stu-id="f6435-148">deviceName</span></span>|<span data-ttu-id="f6435-149">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f6435-149">String</span></span>|<span data-ttu-id="f6435-150">Der gemeldete Gerätename</span><span class="sxs-lookup"><span data-stu-id="f6435-150">The Device Name that is being reported</span></span>|
|<span data-ttu-id="f6435-151">userId</span><span class="sxs-lookup"><span data-stu-id="f6435-151">userId</span></span>|<span data-ttu-id="f6435-152">String</span><span class="sxs-lookup"><span data-stu-id="f6435-152">String</span></span>|<span data-ttu-id="f6435-153">Die gemeldete Benutzer-ID</span><span class="sxs-lookup"><span data-stu-id="f6435-153">The user Id that is being reported</span></span>|
|<span data-ttu-id="f6435-154">userEmail</span><span class="sxs-lookup"><span data-stu-id="f6435-154">userEmail</span></span>|<span data-ttu-id="f6435-155">String</span><span class="sxs-lookup"><span data-stu-id="f6435-155">String</span></span>|<span data-ttu-id="f6435-156">Die gemeldete Benutzer-E-Mail-Adresse</span><span class="sxs-lookup"><span data-stu-id="f6435-156">The User email address that is being reported</span></span>|
|<span data-ttu-id="f6435-157">userName</span><span class="sxs-lookup"><span data-stu-id="f6435-157">userName</span></span>|<span data-ttu-id="f6435-158">String</span><span class="sxs-lookup"><span data-stu-id="f6435-158">String</span></span>|<span data-ttu-id="f6435-159">Gemeldeter Benutzername</span><span class="sxs-lookup"><span data-stu-id="f6435-159">The User Name that is being reported</span></span>|
|<span data-ttu-id="f6435-160">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f6435-160">userPrincipalName</span></span>|<span data-ttu-id="f6435-161">String</span><span class="sxs-lookup"><span data-stu-id="f6435-161">String</span></span>|<span data-ttu-id="f6435-162">Der gemeldete Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="f6435-162">The User PrincipalName that is being reported</span></span>|
|<span data-ttu-id="f6435-163">deviceModel</span><span class="sxs-lookup"><span data-stu-id="f6435-163">deviceModel</span></span>|<span data-ttu-id="f6435-164">String</span><span class="sxs-lookup"><span data-stu-id="f6435-164">String</span></span>|<span data-ttu-id="f6435-165">Gemeldetes Gerätemodell</span><span class="sxs-lookup"><span data-stu-id="f6435-165">The device model that is being reported</span></span>|
|<span data-ttu-id="f6435-166">state</span><span class="sxs-lookup"><span data-stu-id="f6435-166">state</span></span>|[<span data-ttu-id="f6435-167">Wurde</span><span class="sxs-lookup"><span data-stu-id="f6435-167">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="f6435-168">Der Kompatibilitätsstatus der Einstellung.</span><span class="sxs-lookup"><span data-stu-id="f6435-168">The compliance state of the setting.</span></span> <span data-ttu-id="f6435-169">Mögliche Werte: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="f6435-169">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="f6435-170">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="f6435-170">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="f6435-171">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f6435-171">DateTimeOffset</span></span>|<span data-ttu-id="f6435-172">Datum und Uhrzeit des Ablaufs der Toleranzperiode für die Gerätekonformität</span><span class="sxs-lookup"><span data-stu-id="f6435-172">The DateTime when device compliance grace period expires</span></span>|



## <a name="response"></a><span data-ttu-id="f6435-173">Antwort</span><span class="sxs-lookup"><span data-stu-id="f6435-173">Response</span></span>
<span data-ttu-id="f6435-174">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="f6435-174">If successful, this method returns a `200 OK` response code and an updated [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f6435-175">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f6435-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="f6435-176">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f6435-176">Request</span></span>
<span data-ttu-id="f6435-177">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f6435-177">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f6435-178">Antwort</span><span class="sxs-lookup"><span data-stu-id="f6435-178">Response</span></span>
<span data-ttu-id="f6435-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f6435-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




