---
title: AdvancedThreatProtectionOnboardingDeviceSettingState erstellen
description: Erstellen eines neuen advancedThreatProtectionOnboardingDeviceSettingState-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d877edcdc82cee35c7fc75c556ca5ac0035221ad
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30980663"
---
# <a name="create-advancedthreatprotectiononboardingdevicesettingstate"></a><span data-ttu-id="5089c-103">AdvancedThreatProtectionOnboardingDeviceSettingState erstellen</span><span class="sxs-lookup"><span data-stu-id="5089c-103">Create advancedThreatProtectionOnboardingDeviceSettingState</span></span>

> <span data-ttu-id="5089c-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5089c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5089c-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="5089c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5089c-106">Erstellen eines neuen [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="5089c-106">Create a new [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5089c-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="5089c-107">Prerequisites</span></span>
<span data-ttu-id="5089c-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5089c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5089c-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5089c-110">Permission type</span></span>|<span data-ttu-id="5089c-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5089c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5089c-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5089c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5089c-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5089c-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5089c-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5089c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5089c-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5089c-115">Not supported.</span></span>|
|<span data-ttu-id="5089c-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5089c-116">Application</span></span>|<span data-ttu-id="5089c-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5089c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5089c-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5089c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/advancedThreatProtectionOnboardingStateSummary/advancedThreatProtectionOnboardingDeviceSettingStates
```

## <a name="request-headers"></a><span data-ttu-id="5089c-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5089c-119">Request headers</span></span>
|<span data-ttu-id="5089c-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="5089c-120">Header</span></span>|<span data-ttu-id="5089c-121">Wert</span><span class="sxs-lookup"><span data-stu-id="5089c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5089c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5089c-122">Authorization</span></span>|<span data-ttu-id="5089c-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="5089c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5089c-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="5089c-124">Accept</span></span>|<span data-ttu-id="5089c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5089c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5089c-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5089c-126">Request body</span></span>
<span data-ttu-id="5089c-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das advancedThreatProtectionOnboardingDeviceSettingState-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="5089c-127">In the request body, supply a JSON representation for the advancedThreatProtectionOnboardingDeviceSettingState object.</span></span>

<span data-ttu-id="5089c-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der advancedThreatProtectionOnboardingDeviceSettingState erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="5089c-128">The following table shows the properties that are required when you create the advancedThreatProtectionOnboardingDeviceSettingState.</span></span>

|<span data-ttu-id="5089c-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5089c-129">Property</span></span>|<span data-ttu-id="5089c-130">Typ</span><span class="sxs-lookup"><span data-stu-id="5089c-130">Type</span></span>|<span data-ttu-id="5089c-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5089c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5089c-132">id</span><span class="sxs-lookup"><span data-stu-id="5089c-132">id</span></span>|<span data-ttu-id="5089c-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5089c-133">String</span></span>|<span data-ttu-id="5089c-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="5089c-134">Key of the entity</span></span>|
|<span data-ttu-id="5089c-135">platformType</span><span class="sxs-lookup"><span data-stu-id="5089c-135">platformType</span></span>|[<span data-ttu-id="5089c-136">deviceType</span><span class="sxs-lookup"><span data-stu-id="5089c-136">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="5089c-137">Geräte Plattformtyp.</span><span class="sxs-lookup"><span data-stu-id="5089c-137">Device platform type.</span></span> <span data-ttu-id="5089c-138">Mögliche Werte sind: `desktop`, `windowsRT`, `winMO6` `nokia` `windowsPhone` `mac` `winCE` `iPhone` `iPad` `iPod` `android` `iSocConsumer` `unix` `macMDM`,,,,,,,, `holoLens`,, `androidEnterprise` ,,,,,, `surfaceHub` `androidForWork` `winEmbedded` , `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="5089c-138">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="5089c-139">Einstellung</span><span class="sxs-lookup"><span data-stu-id="5089c-139">setting</span></span>|<span data-ttu-id="5089c-140">String</span><span class="sxs-lookup"><span data-stu-id="5089c-140">String</span></span>|<span data-ttu-id="5089c-141">Der Klassenname und der Eigenschaftenname der Einstellung.</span><span class="sxs-lookup"><span data-stu-id="5089c-141">The setting class name and property name.</span></span>|
|<span data-ttu-id="5089c-142">settingName</span><span class="sxs-lookup"><span data-stu-id="5089c-142">settingName</span></span>|<span data-ttu-id="5089c-143">String</span><span class="sxs-lookup"><span data-stu-id="5089c-143">String</span></span>|<span data-ttu-id="5089c-144">Der gemeldete Einstellungsname</span><span class="sxs-lookup"><span data-stu-id="5089c-144">The Setting Name that is being reported</span></span>|
|<span data-ttu-id="5089c-145">deviceId</span><span class="sxs-lookup"><span data-stu-id="5089c-145">deviceId</span></span>|<span data-ttu-id="5089c-146">String</span><span class="sxs-lookup"><span data-stu-id="5089c-146">String</span></span>|<span data-ttu-id="5089c-147">Die gemeldete Geräte-ID</span><span class="sxs-lookup"><span data-stu-id="5089c-147">The Device Id that is being reported</span></span>|
|<span data-ttu-id="5089c-148">deviceName</span><span class="sxs-lookup"><span data-stu-id="5089c-148">deviceName</span></span>|<span data-ttu-id="5089c-149">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5089c-149">String</span></span>|<span data-ttu-id="5089c-150">Der gemeldete Gerätename</span><span class="sxs-lookup"><span data-stu-id="5089c-150">The Device Name that is being reported</span></span>|
|<span data-ttu-id="5089c-151">userId</span><span class="sxs-lookup"><span data-stu-id="5089c-151">userId</span></span>|<span data-ttu-id="5089c-152">String</span><span class="sxs-lookup"><span data-stu-id="5089c-152">String</span></span>|<span data-ttu-id="5089c-153">Die gemeldete Benutzer-ID</span><span class="sxs-lookup"><span data-stu-id="5089c-153">The user Id that is being reported</span></span>|
|<span data-ttu-id="5089c-154">userEmail</span><span class="sxs-lookup"><span data-stu-id="5089c-154">userEmail</span></span>|<span data-ttu-id="5089c-155">String</span><span class="sxs-lookup"><span data-stu-id="5089c-155">String</span></span>|<span data-ttu-id="5089c-156">Die gemeldete Benutzer-E-Mail-Adresse</span><span class="sxs-lookup"><span data-stu-id="5089c-156">The User email address that is being reported</span></span>|
|<span data-ttu-id="5089c-157">userName</span><span class="sxs-lookup"><span data-stu-id="5089c-157">userName</span></span>|<span data-ttu-id="5089c-158">String</span><span class="sxs-lookup"><span data-stu-id="5089c-158">String</span></span>|<span data-ttu-id="5089c-159">Gemeldeter Benutzername</span><span class="sxs-lookup"><span data-stu-id="5089c-159">The User Name that is being reported</span></span>|
|<span data-ttu-id="5089c-160">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="5089c-160">userPrincipalName</span></span>|<span data-ttu-id="5089c-161">String</span><span class="sxs-lookup"><span data-stu-id="5089c-161">String</span></span>|<span data-ttu-id="5089c-162">Der gemeldete Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="5089c-162">The User PrincipalName that is being reported</span></span>|
|<span data-ttu-id="5089c-163">deviceModel</span><span class="sxs-lookup"><span data-stu-id="5089c-163">deviceModel</span></span>|<span data-ttu-id="5089c-164">String</span><span class="sxs-lookup"><span data-stu-id="5089c-164">String</span></span>|<span data-ttu-id="5089c-165">Gemeldetes Gerätemodell</span><span class="sxs-lookup"><span data-stu-id="5089c-165">The device model that is being reported</span></span>|
|<span data-ttu-id="5089c-166">state</span><span class="sxs-lookup"><span data-stu-id="5089c-166">state</span></span>|[<span data-ttu-id="5089c-167">Wurde</span><span class="sxs-lookup"><span data-stu-id="5089c-167">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="5089c-168">Der Kompatibilitätsstatus der Einstellung.</span><span class="sxs-lookup"><span data-stu-id="5089c-168">The compliance state of the setting.</span></span> <span data-ttu-id="5089c-169">Mögliche Werte: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="5089c-169">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="5089c-170">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="5089c-170">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="5089c-171">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5089c-171">DateTimeOffset</span></span>|<span data-ttu-id="5089c-172">Datum und Uhrzeit des Ablaufs der Toleranzperiode für die Gerätekonformität</span><span class="sxs-lookup"><span data-stu-id="5089c-172">The DateTime when device compliance grace period expires</span></span>|



## <a name="response"></a><span data-ttu-id="5089c-173">Antwort</span><span class="sxs-lookup"><span data-stu-id="5089c-173">Response</span></span>
<span data-ttu-id="5089c-174">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="5089c-174">If successful, this method returns a `201 Created` response code and a [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5089c-175">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5089c-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="5089c-176">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5089c-176">Request</span></span>
<span data-ttu-id="5089c-177">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5089c-177">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5089c-178">Antwort</span><span class="sxs-lookup"><span data-stu-id="5089c-178">Response</span></span>
<span data-ttu-id="5089c-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5089c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




