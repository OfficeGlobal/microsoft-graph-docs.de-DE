---
title: Erstellen von „deviceComplianceSettingState“
description: Diese Methode erstellt ein neues Objekt des Typs deviceComplianceSettingState.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 0ef4061f659429b4e43f40fd502caaad77ef0894
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27868754"
---
# <a name="create-devicecompliancesettingstate"></a><span data-ttu-id="0f126-103">Erstellen von „deviceComplianceSettingState“</span><span class="sxs-lookup"><span data-stu-id="0f126-103">Create deviceComplianceSettingState</span></span>

> <span data-ttu-id="0f126-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="0f126-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0f126-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0f126-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0f126-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="0f126-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0f126-107">Diese Methode erstellt ein neues Objekt des Typs [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span><span class="sxs-lookup"><span data-stu-id="0f126-107">Create a new [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0f126-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="0f126-108">Prerequisites</span></span>
<span data-ttu-id="0f126-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0f126-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0f126-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0f126-111">Permission type</span></span>|<span data-ttu-id="0f126-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0f126-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0f126-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0f126-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0f126-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f126-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0f126-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0f126-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0f126-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0f126-116">Not supported.</span></span>|
|<span data-ttu-id="0f126-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0f126-117">Application</span></span>|<span data-ttu-id="0f126-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0f126-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0f126-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0f126-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates
```

## <a name="request-headers"></a><span data-ttu-id="0f126-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0f126-120">Request headers</span></span>
|<span data-ttu-id="0f126-121">Header</span><span class="sxs-lookup"><span data-stu-id="0f126-121">Header</span></span>|<span data-ttu-id="0f126-122">Wert</span><span class="sxs-lookup"><span data-stu-id="0f126-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0f126-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0f126-123">Authorization</span></span>|<span data-ttu-id="0f126-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="0f126-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0f126-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="0f126-125">Accept</span></span>|<span data-ttu-id="0f126-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0f126-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0f126-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0f126-127">Request body</span></span>
<span data-ttu-id="0f126-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „deviceComplianceSettingState“ an.</span><span class="sxs-lookup"><span data-stu-id="0f126-128">In the request body, supply a JSON representation for the deviceComplianceSettingState object.</span></span>

<span data-ttu-id="0f126-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „deviceComplianceSettingState“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="0f126-129">The following table shows the properties that are required when you create the deviceComplianceSettingState.</span></span>

|<span data-ttu-id="0f126-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0f126-130">Property</span></span>|<span data-ttu-id="0f126-131">Typ</span><span class="sxs-lookup"><span data-stu-id="0f126-131">Type</span></span>|<span data-ttu-id="0f126-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0f126-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f126-133">id</span><span class="sxs-lookup"><span data-stu-id="0f126-133">id</span></span>|<span data-ttu-id="0f126-134">String</span><span class="sxs-lookup"><span data-stu-id="0f126-134">String</span></span>|<span data-ttu-id="0f126-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="0f126-135">Key of the entity</span></span>|
|<span data-ttu-id="0f126-136">platformType</span><span class="sxs-lookup"><span data-stu-id="0f126-136">platformType</span></span>|[<span data-ttu-id="0f126-137">deviceType</span><span class="sxs-lookup"><span data-stu-id="0f126-137">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="0f126-138">Gerätetyp-Plattform.</span><span class="sxs-lookup"><span data-stu-id="0f126-138">Device platform type.</span></span> <span data-ttu-id="0f126-139">Mögliche Werte sind: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise` , `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="0f126-139">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="0f126-140">setting</span><span class="sxs-lookup"><span data-stu-id="0f126-140">setting</span></span>|<span data-ttu-id="0f126-141">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0f126-141">String</span></span>|<span data-ttu-id="0f126-142">Klassenname und Eigenschaftenname der Einstellung</span><span class="sxs-lookup"><span data-stu-id="0f126-142">The setting class name and property name.</span></span>|
|<span data-ttu-id="0f126-143">settingName</span><span class="sxs-lookup"><span data-stu-id="0f126-143">settingName</span></span>|<span data-ttu-id="0f126-144">String</span><span class="sxs-lookup"><span data-stu-id="0f126-144">String</span></span>|<span data-ttu-id="0f126-145">Gemeldeter Einstellungsname</span><span class="sxs-lookup"><span data-stu-id="0f126-145">The Setting Name that is being reported</span></span>|
|<span data-ttu-id="0f126-146">deviceId</span><span class="sxs-lookup"><span data-stu-id="0f126-146">deviceId</span></span>|<span data-ttu-id="0f126-147">String</span><span class="sxs-lookup"><span data-stu-id="0f126-147">String</span></span>|<span data-ttu-id="0f126-148">Gemeldete Geräte-ID</span><span class="sxs-lookup"><span data-stu-id="0f126-148">The Device Id that is being reported</span></span>|
|<span data-ttu-id="0f126-149">deviceName</span><span class="sxs-lookup"><span data-stu-id="0f126-149">deviceName</span></span>|<span data-ttu-id="0f126-150">String</span><span class="sxs-lookup"><span data-stu-id="0f126-150">String</span></span>|<span data-ttu-id="0f126-151">Gemeldeter Gerätename</span><span class="sxs-lookup"><span data-stu-id="0f126-151">The Device Name that is being reported</span></span>|
|<span data-ttu-id="0f126-152">userId</span><span class="sxs-lookup"><span data-stu-id="0f126-152">userId</span></span>|<span data-ttu-id="0f126-153">String</span><span class="sxs-lookup"><span data-stu-id="0f126-153">String</span></span>|<span data-ttu-id="0f126-154">Gemeldete Benutzer-ID</span><span class="sxs-lookup"><span data-stu-id="0f126-154">The user Id that is being reported</span></span>|
|<span data-ttu-id="0f126-155">userEmail</span><span class="sxs-lookup"><span data-stu-id="0f126-155">userEmail</span></span>|<span data-ttu-id="0f126-156">String</span><span class="sxs-lookup"><span data-stu-id="0f126-156">String</span></span>|<span data-ttu-id="0f126-157">Gemeldete Benutzer-E-Mail-Adresse</span><span class="sxs-lookup"><span data-stu-id="0f126-157">The User email address that is being reported</span></span>|
|<span data-ttu-id="0f126-158">userName</span><span class="sxs-lookup"><span data-stu-id="0f126-158">userName</span></span>|<span data-ttu-id="0f126-159">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0f126-159">String</span></span>|<span data-ttu-id="0f126-160">Gemeldeter Benutzername</span><span class="sxs-lookup"><span data-stu-id="0f126-160">The User Name that is being reported</span></span>|
|<span data-ttu-id="0f126-161">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="0f126-161">userPrincipalName</span></span>|<span data-ttu-id="0f126-162">String</span><span class="sxs-lookup"><span data-stu-id="0f126-162">String</span></span>|<span data-ttu-id="0f126-163">Gemeldeter Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="0f126-163">The User PrincipalName that is being reported</span></span>|
|<span data-ttu-id="0f126-164">deviceModel</span><span class="sxs-lookup"><span data-stu-id="0f126-164">deviceModel</span></span>|<span data-ttu-id="0f126-165">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0f126-165">String</span></span>|<span data-ttu-id="0f126-166">Gemeldetes Gerätemodell</span><span class="sxs-lookup"><span data-stu-id="0f126-166">The device model that is being reported</span></span>|
|<span data-ttu-id="0f126-167">state</span><span class="sxs-lookup"><span data-stu-id="0f126-167">state</span></span>|[<span data-ttu-id="0f126-168">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="0f126-168">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="0f126-169">Der Compliance-Zustand der Einstellung.</span><span class="sxs-lookup"><span data-stu-id="0f126-169">The compliance state of the setting.</span></span> <span data-ttu-id="0f126-170">Mögliche Werte sind: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict` und `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="0f126-170">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="0f126-171">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="0f126-171">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="0f126-172">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0f126-172">DateTimeOffset</span></span>|<span data-ttu-id="0f126-173">Datum und Uhrzeit des Ablaufs der Toleranzperiode für die Gerätekonformität</span><span class="sxs-lookup"><span data-stu-id="0f126-173">The DateTime when device compliance grace period expires</span></span>|



## <a name="response"></a><span data-ttu-id="0f126-174">Antwort</span><span class="sxs-lookup"><span data-stu-id="0f126-174">Response</span></span>
<span data-ttu-id="0f126-175">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="0f126-175">If successful, this method returns a `201 Created` response code and a [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0f126-176">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0f126-176">Example</span></span>
### <a name="request"></a><span data-ttu-id="0f126-177">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0f126-177">Request</span></span>
<span data-ttu-id="0f126-178">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0f126-178">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates
Content-type: application/json
Content-length: 549

{
  "@odata.type": "#microsoft.graph.deviceComplianceSettingState",
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

### <a name="response"></a><span data-ttu-id="0f126-179">Antwort</span><span class="sxs-lookup"><span data-stu-id="0f126-179">Response</span></span>
<span data-ttu-id="0f126-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0f126-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 598

{
  "@odata.type": "#microsoft.graph.deviceComplianceSettingState",
  "id": "9905f955-f955-9905-55f9-059955f90599",
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





