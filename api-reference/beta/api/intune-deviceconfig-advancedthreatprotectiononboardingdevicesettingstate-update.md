---
title: AdvancedThreatProtectionOnboardingDeviceSettingState aktualisieren
description: Aktualisieren Sie die Eigenschaften eines AdvancedThreatProtectionOnboardingDeviceSettingState-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: de136488c24c3de4136b953e120d8ed4fbd3fec6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27828315"
---
# <a name="update-advancedthreatprotectiononboardingdevicesettingstate"></a><span data-ttu-id="6f7fb-103">AdvancedThreatProtectionOnboardingDeviceSettingState aktualisieren</span><span class="sxs-lookup"><span data-stu-id="6f7fb-103">Update advancedThreatProtectionOnboardingDeviceSettingState</span></span>

> <span data-ttu-id="6f7fb-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="6f7fb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6f7fb-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6f7fb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6f7fb-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="6f7fb-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6f7fb-107">Aktualisieren Sie die Eigenschaften eines [AdvancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="6f7fb-107">Update the properties of a [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6f7fb-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="6f7fb-108">Prerequisites</span></span>
<span data-ttu-id="6f7fb-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6f7fb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6f7fb-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6f7fb-111">Permission type</span></span>|<span data-ttu-id="6f7fb-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6f7fb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6f7fb-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6f7fb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6f7fb-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f7fb-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6f7fb-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6f7fb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6f7fb-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6f7fb-116">Not supported.</span></span>|
|<span data-ttu-id="6f7fb-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6f7fb-117">Application</span></span>|<span data-ttu-id="6f7fb-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6f7fb-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6f7fb-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6f7fb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/advancedThreatProtectionOnboardingStateSummary/advancedThreatProtectionOnboardingDeviceSettingStates/{advancedThreatProtectionOnboardingDeviceSettingStateId}
```

## <a name="request-headers"></a><span data-ttu-id="6f7fb-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6f7fb-120">Request headers</span></span>
|<span data-ttu-id="6f7fb-121">Header</span><span class="sxs-lookup"><span data-stu-id="6f7fb-121">Header</span></span>|<span data-ttu-id="6f7fb-122">Wert</span><span class="sxs-lookup"><span data-stu-id="6f7fb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6f7fb-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6f7fb-123">Authorization</span></span>|<span data-ttu-id="6f7fb-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="6f7fb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6f7fb-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="6f7fb-125">Accept</span></span>|<span data-ttu-id="6f7fb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6f7fb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6f7fb-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6f7fb-127">Request body</span></span>
<span data-ttu-id="6f7fb-128">Geben Sie im Textkörper Anforderung für das Objekt [AdvancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="6f7fb-128">In the request body, supply a JSON representation for the [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) object.</span></span>

<span data-ttu-id="6f7fb-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [AdvancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="6f7fb-129">The following table shows the properties that are required when you create the [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md).</span></span>

|<span data-ttu-id="6f7fb-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6f7fb-130">Property</span></span>|<span data-ttu-id="6f7fb-131">Typ</span><span class="sxs-lookup"><span data-stu-id="6f7fb-131">Type</span></span>|<span data-ttu-id="6f7fb-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6f7fb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6f7fb-133">id</span><span class="sxs-lookup"><span data-stu-id="6f7fb-133">id</span></span>|<span data-ttu-id="6f7fb-134">String</span><span class="sxs-lookup"><span data-stu-id="6f7fb-134">String</span></span>|<span data-ttu-id="6f7fb-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="6f7fb-135">Key of the entity</span></span>|
|<span data-ttu-id="6f7fb-136">platformType</span><span class="sxs-lookup"><span data-stu-id="6f7fb-136">platformType</span></span>|[<span data-ttu-id="6f7fb-137">deviceType</span><span class="sxs-lookup"><span data-stu-id="6f7fb-137">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="6f7fb-138">Gerätetyp-Plattform.</span><span class="sxs-lookup"><span data-stu-id="6f7fb-138">Device platform type.</span></span> <span data-ttu-id="6f7fb-139">Mögliche Werte sind: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise` , `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="6f7fb-139">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="6f7fb-140">setting</span><span class="sxs-lookup"><span data-stu-id="6f7fb-140">setting</span></span>|<span data-ttu-id="6f7fb-141">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6f7fb-141">String</span></span>|<span data-ttu-id="6f7fb-142">Klassenname und Eigenschaftenname der Einstellung</span><span class="sxs-lookup"><span data-stu-id="6f7fb-142">The setting class name and property name.</span></span>|
|<span data-ttu-id="6f7fb-143">settingName</span><span class="sxs-lookup"><span data-stu-id="6f7fb-143">settingName</span></span>|<span data-ttu-id="6f7fb-144">String</span><span class="sxs-lookup"><span data-stu-id="6f7fb-144">String</span></span>|<span data-ttu-id="6f7fb-145">Gemeldeter Einstellungsname</span><span class="sxs-lookup"><span data-stu-id="6f7fb-145">The Setting Name that is being reported</span></span>|
|<span data-ttu-id="6f7fb-146">deviceId</span><span class="sxs-lookup"><span data-stu-id="6f7fb-146">deviceId</span></span>|<span data-ttu-id="6f7fb-147">String</span><span class="sxs-lookup"><span data-stu-id="6f7fb-147">String</span></span>|<span data-ttu-id="6f7fb-148">Gemeldete Geräte-ID</span><span class="sxs-lookup"><span data-stu-id="6f7fb-148">The Device Id that is being reported</span></span>|
|<span data-ttu-id="6f7fb-149">deviceName</span><span class="sxs-lookup"><span data-stu-id="6f7fb-149">deviceName</span></span>|<span data-ttu-id="6f7fb-150">String</span><span class="sxs-lookup"><span data-stu-id="6f7fb-150">String</span></span>|<span data-ttu-id="6f7fb-151">Gemeldeter Gerätename</span><span class="sxs-lookup"><span data-stu-id="6f7fb-151">The Device Name that is being reported</span></span>|
|<span data-ttu-id="6f7fb-152">userId</span><span class="sxs-lookup"><span data-stu-id="6f7fb-152">userId</span></span>|<span data-ttu-id="6f7fb-153">String</span><span class="sxs-lookup"><span data-stu-id="6f7fb-153">String</span></span>|<span data-ttu-id="6f7fb-154">Gemeldete Benutzer-ID</span><span class="sxs-lookup"><span data-stu-id="6f7fb-154">The user Id that is being reported</span></span>|
|<span data-ttu-id="6f7fb-155">userEmail</span><span class="sxs-lookup"><span data-stu-id="6f7fb-155">userEmail</span></span>|<span data-ttu-id="6f7fb-156">String</span><span class="sxs-lookup"><span data-stu-id="6f7fb-156">String</span></span>|<span data-ttu-id="6f7fb-157">Gemeldete Benutzer-E-Mail-Adresse</span><span class="sxs-lookup"><span data-stu-id="6f7fb-157">The User email address that is being reported</span></span>|
|<span data-ttu-id="6f7fb-158">userName</span><span class="sxs-lookup"><span data-stu-id="6f7fb-158">userName</span></span>|<span data-ttu-id="6f7fb-159">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6f7fb-159">String</span></span>|<span data-ttu-id="6f7fb-160">Gemeldeter Benutzername</span><span class="sxs-lookup"><span data-stu-id="6f7fb-160">The User Name that is being reported</span></span>|
|<span data-ttu-id="6f7fb-161">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="6f7fb-161">userPrincipalName</span></span>|<span data-ttu-id="6f7fb-162">String</span><span class="sxs-lookup"><span data-stu-id="6f7fb-162">String</span></span>|<span data-ttu-id="6f7fb-163">Gemeldeter Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="6f7fb-163">The User PrincipalName that is being reported</span></span>|
|<span data-ttu-id="6f7fb-164">deviceModel</span><span class="sxs-lookup"><span data-stu-id="6f7fb-164">deviceModel</span></span>|<span data-ttu-id="6f7fb-165">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6f7fb-165">String</span></span>|<span data-ttu-id="6f7fb-166">Gemeldetes Gerätemodell</span><span class="sxs-lookup"><span data-stu-id="6f7fb-166">The device model that is being reported</span></span>|
|<span data-ttu-id="6f7fb-167">state</span><span class="sxs-lookup"><span data-stu-id="6f7fb-167">state</span></span>|[<span data-ttu-id="6f7fb-168">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="6f7fb-168">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="6f7fb-169">Der Compliance-Zustand der Einstellung.</span><span class="sxs-lookup"><span data-stu-id="6f7fb-169">The compliance state of the setting.</span></span> <span data-ttu-id="6f7fb-170">Mögliche Werte sind: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict` und `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="6f7fb-170">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="6f7fb-171">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="6f7fb-171">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="6f7fb-172">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6f7fb-172">DateTimeOffset</span></span>|<span data-ttu-id="6f7fb-173">Datum und Uhrzeit des Ablaufs der Toleranzperiode für die Gerätekonformität</span><span class="sxs-lookup"><span data-stu-id="6f7fb-173">The DateTime when device compliance grace period expires</span></span>|



## <a name="response"></a><span data-ttu-id="6f7fb-174">Antwort</span><span class="sxs-lookup"><span data-stu-id="6f7fb-174">Response</span></span>
<span data-ttu-id="6f7fb-175">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [AdvancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="6f7fb-175">If successful, this method returns a `200 OK` response code and an updated [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6f7fb-176">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6f7fb-176">Example</span></span>
### <a name="request"></a><span data-ttu-id="6f7fb-177">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6f7fb-177">Request</span></span>
<span data-ttu-id="6f7fb-178">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6f7fb-178">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/advancedThreatProtectionOnboardingStateSummary/advancedThreatProtectionOnboardingDeviceSettingStates/{advancedThreatProtectionOnboardingDeviceSettingStateId}
Content-type: application/json
Content-length: 482

{
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

### <a name="response"></a><span data-ttu-id="6f7fb-179">Antwort</span><span class="sxs-lookup"><span data-stu-id="6f7fb-179">Response</span></span>
<span data-ttu-id="6f7fb-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6f7fb-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





