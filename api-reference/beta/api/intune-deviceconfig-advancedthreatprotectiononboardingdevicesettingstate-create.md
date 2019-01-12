---
title: Erstellen von advancedThreatProtectionOnboardingDeviceSettingState
description: Erstellen eines neuen AdvancedThreatProtectionOnboardingDeviceSettingState-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 878d887ff792558e9fa82d04490254d1e7190308
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27933785"
---
# <a name="create-advancedthreatprotectiononboardingdevicesettingstate"></a><span data-ttu-id="b6cf7-103">Erstellen von advancedThreatProtectionOnboardingDeviceSettingState</span><span class="sxs-lookup"><span data-stu-id="b6cf7-103">Create advancedThreatProtectionOnboardingDeviceSettingState</span></span>

> <span data-ttu-id="b6cf7-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b6cf7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b6cf7-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b6cf7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b6cf7-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="b6cf7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b6cf7-107">Erstellen eines neuen [AdvancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="b6cf7-107">Create a new [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b6cf7-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b6cf7-108">Prerequisites</span></span>
<span data-ttu-id="b6cf7-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b6cf7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b6cf7-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b6cf7-111">Permission type</span></span>|<span data-ttu-id="b6cf7-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b6cf7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b6cf7-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b6cf7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b6cf7-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6cf7-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b6cf7-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b6cf7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b6cf7-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b6cf7-116">Not supported.</span></span>|
|<span data-ttu-id="b6cf7-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b6cf7-117">Application</span></span>|<span data-ttu-id="b6cf7-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b6cf7-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b6cf7-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b6cf7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/advancedThreatProtectionOnboardingStateSummary/advancedThreatProtectionOnboardingDeviceSettingStates
```

## <a name="request-headers"></a><span data-ttu-id="b6cf7-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b6cf7-120">Request headers</span></span>
|<span data-ttu-id="b6cf7-121">Header</span><span class="sxs-lookup"><span data-stu-id="b6cf7-121">Header</span></span>|<span data-ttu-id="b6cf7-122">Wert</span><span class="sxs-lookup"><span data-stu-id="b6cf7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b6cf7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b6cf7-123">Authorization</span></span>|<span data-ttu-id="b6cf7-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b6cf7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b6cf7-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="b6cf7-125">Accept</span></span>|<span data-ttu-id="b6cf7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b6cf7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b6cf7-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b6cf7-127">Request body</span></span>
<span data-ttu-id="b6cf7-128">Geben Sie im Textkörper Anforderung für das Objekt AdvancedThreatProtectionOnboardingDeviceSettingState eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="b6cf7-128">In the request body, supply a JSON representation for the advancedThreatProtectionOnboardingDeviceSettingState object.</span></span>

<span data-ttu-id="b6cf7-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die AdvancedThreatProtectionOnboardingDeviceSettingState erstellen.</span><span class="sxs-lookup"><span data-stu-id="b6cf7-129">The following table shows the properties that are required when you create the advancedThreatProtectionOnboardingDeviceSettingState.</span></span>

|<span data-ttu-id="b6cf7-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b6cf7-130">Property</span></span>|<span data-ttu-id="b6cf7-131">Typ</span><span class="sxs-lookup"><span data-stu-id="b6cf7-131">Type</span></span>|<span data-ttu-id="b6cf7-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b6cf7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b6cf7-133">id</span><span class="sxs-lookup"><span data-stu-id="b6cf7-133">id</span></span>|<span data-ttu-id="b6cf7-134">String</span><span class="sxs-lookup"><span data-stu-id="b6cf7-134">String</span></span>|<span data-ttu-id="b6cf7-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="b6cf7-135">Key of the entity</span></span>|
|<span data-ttu-id="b6cf7-136">platformType</span><span class="sxs-lookup"><span data-stu-id="b6cf7-136">platformType</span></span>|[<span data-ttu-id="b6cf7-137">deviceType</span><span class="sxs-lookup"><span data-stu-id="b6cf7-137">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="b6cf7-138">Gerätetyp-Plattform.</span><span class="sxs-lookup"><span data-stu-id="b6cf7-138">Device platform type.</span></span> <span data-ttu-id="b6cf7-139">Mögliche Werte sind: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise` , `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="b6cf7-139">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="b6cf7-140">setting</span><span class="sxs-lookup"><span data-stu-id="b6cf7-140">setting</span></span>|<span data-ttu-id="b6cf7-141">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b6cf7-141">String</span></span>|<span data-ttu-id="b6cf7-142">Klassenname und Eigenschaftenname der Einstellung</span><span class="sxs-lookup"><span data-stu-id="b6cf7-142">The setting class name and property name.</span></span>|
|<span data-ttu-id="b6cf7-143">settingName</span><span class="sxs-lookup"><span data-stu-id="b6cf7-143">settingName</span></span>|<span data-ttu-id="b6cf7-144">String</span><span class="sxs-lookup"><span data-stu-id="b6cf7-144">String</span></span>|<span data-ttu-id="b6cf7-145">Gemeldeter Einstellungsname</span><span class="sxs-lookup"><span data-stu-id="b6cf7-145">The Setting Name that is being reported</span></span>|
|<span data-ttu-id="b6cf7-146">deviceId</span><span class="sxs-lookup"><span data-stu-id="b6cf7-146">deviceId</span></span>|<span data-ttu-id="b6cf7-147">String</span><span class="sxs-lookup"><span data-stu-id="b6cf7-147">String</span></span>|<span data-ttu-id="b6cf7-148">Gemeldete Geräte-ID</span><span class="sxs-lookup"><span data-stu-id="b6cf7-148">The Device Id that is being reported</span></span>|
|<span data-ttu-id="b6cf7-149">deviceName</span><span class="sxs-lookup"><span data-stu-id="b6cf7-149">deviceName</span></span>|<span data-ttu-id="b6cf7-150">String</span><span class="sxs-lookup"><span data-stu-id="b6cf7-150">String</span></span>|<span data-ttu-id="b6cf7-151">Gemeldeter Gerätename</span><span class="sxs-lookup"><span data-stu-id="b6cf7-151">The Device Name that is being reported</span></span>|
|<span data-ttu-id="b6cf7-152">userId</span><span class="sxs-lookup"><span data-stu-id="b6cf7-152">userId</span></span>|<span data-ttu-id="b6cf7-153">String</span><span class="sxs-lookup"><span data-stu-id="b6cf7-153">String</span></span>|<span data-ttu-id="b6cf7-154">Gemeldete Benutzer-ID</span><span class="sxs-lookup"><span data-stu-id="b6cf7-154">The user Id that is being reported</span></span>|
|<span data-ttu-id="b6cf7-155">userEmail</span><span class="sxs-lookup"><span data-stu-id="b6cf7-155">userEmail</span></span>|<span data-ttu-id="b6cf7-156">String</span><span class="sxs-lookup"><span data-stu-id="b6cf7-156">String</span></span>|<span data-ttu-id="b6cf7-157">Gemeldete Benutzer-E-Mail-Adresse</span><span class="sxs-lookup"><span data-stu-id="b6cf7-157">The User email address that is being reported</span></span>|
|<span data-ttu-id="b6cf7-158">userName</span><span class="sxs-lookup"><span data-stu-id="b6cf7-158">userName</span></span>|<span data-ttu-id="b6cf7-159">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b6cf7-159">String</span></span>|<span data-ttu-id="b6cf7-160">Gemeldeter Benutzername</span><span class="sxs-lookup"><span data-stu-id="b6cf7-160">The User Name that is being reported</span></span>|
|<span data-ttu-id="b6cf7-161">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b6cf7-161">userPrincipalName</span></span>|<span data-ttu-id="b6cf7-162">String</span><span class="sxs-lookup"><span data-stu-id="b6cf7-162">String</span></span>|<span data-ttu-id="b6cf7-163">Gemeldeter Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="b6cf7-163">The User PrincipalName that is being reported</span></span>|
|<span data-ttu-id="b6cf7-164">deviceModel</span><span class="sxs-lookup"><span data-stu-id="b6cf7-164">deviceModel</span></span>|<span data-ttu-id="b6cf7-165">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b6cf7-165">String</span></span>|<span data-ttu-id="b6cf7-166">Gemeldetes Gerätemodell</span><span class="sxs-lookup"><span data-stu-id="b6cf7-166">The device model that is being reported</span></span>|
|<span data-ttu-id="b6cf7-167">state</span><span class="sxs-lookup"><span data-stu-id="b6cf7-167">state</span></span>|[<span data-ttu-id="b6cf7-168">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="b6cf7-168">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="b6cf7-169">Der Compliance-Zustand der Einstellung.</span><span class="sxs-lookup"><span data-stu-id="b6cf7-169">The compliance state of the setting.</span></span> <span data-ttu-id="b6cf7-170">Mögliche Werte sind: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict` und `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="b6cf7-170">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="b6cf7-171">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="b6cf7-171">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="b6cf7-172">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b6cf7-172">DateTimeOffset</span></span>|<span data-ttu-id="b6cf7-173">Datum und Uhrzeit des Ablaufs der Toleranzperiode für die Gerätekonformität</span><span class="sxs-lookup"><span data-stu-id="b6cf7-173">The DateTime when device compliance grace period expires</span></span>|



## <a name="response"></a><span data-ttu-id="b6cf7-174">Antwort</span><span class="sxs-lookup"><span data-stu-id="b6cf7-174">Response</span></span>
<span data-ttu-id="b6cf7-175">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [AdvancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="b6cf7-175">If successful, this method returns a `201 Created` response code and a [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b6cf7-176">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b6cf7-176">Example</span></span>
### <a name="request"></a><span data-ttu-id="b6cf7-177">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b6cf7-177">Request</span></span>
<span data-ttu-id="b6cf7-178">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b6cf7-178">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b6cf7-179">Antwort</span><span class="sxs-lookup"><span data-stu-id="b6cf7-179">Response</span></span>
<span data-ttu-id="b6cf7-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b6cf7-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





