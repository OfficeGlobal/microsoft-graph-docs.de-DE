---
title: deviceComplianceSettingState aktualisieren
description: Aktualisieren der Eigenschaften eines deviceComplianceSettingState-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2cba44ee5a012e173f1411da7db53c0d11f4adcb
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30981594"
---
# <a name="update-devicecompliancesettingstate"></a><span data-ttu-id="a4a3e-103">deviceComplianceSettingState aktualisieren</span><span class="sxs-lookup"><span data-stu-id="a4a3e-103">Update deviceComplianceSettingState</span></span>

> <span data-ttu-id="a4a3e-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a4a3e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a4a3e-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="a4a3e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a4a3e-106">Aktualisieren der Eigenschaften eines [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="a4a3e-106">Update the properties of a [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a4a3e-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="a4a3e-107">Prerequisites</span></span>
<span data-ttu-id="a4a3e-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a4a3e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a4a3e-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a4a3e-110">Permission type</span></span>|<span data-ttu-id="a4a3e-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a4a3e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a4a3e-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a4a3e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a4a3e-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4a3e-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a4a3e-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a4a3e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a4a3e-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a4a3e-115">Not supported.</span></span>|
|<span data-ttu-id="a4a3e-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a4a3e-116">Application</span></span>|<span data-ttu-id="a4a3e-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a4a3e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a4a3e-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a4a3e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates/{deviceComplianceSettingStateId}
```

## <a name="request-headers"></a><span data-ttu-id="a4a3e-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a4a3e-119">Request headers</span></span>
|<span data-ttu-id="a4a3e-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="a4a3e-120">Header</span></span>|<span data-ttu-id="a4a3e-121">Wert</span><span class="sxs-lookup"><span data-stu-id="a4a3e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a4a3e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a4a3e-122">Authorization</span></span>|<span data-ttu-id="a4a3e-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="a4a3e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a4a3e-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="a4a3e-124">Accept</span></span>|<span data-ttu-id="a4a3e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a4a3e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a4a3e-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a4a3e-126">Request body</span></span>
<span data-ttu-id="a4a3e-127">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) an.</span><span class="sxs-lookup"><span data-stu-id="a4a3e-127">In the request body, supply a JSON representation for the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>

<span data-ttu-id="a4a3e-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="a4a3e-128">The following table shows the properties that are required when you create the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span></span>

|<span data-ttu-id="a4a3e-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a4a3e-129">Property</span></span>|<span data-ttu-id="a4a3e-130">Typ</span><span class="sxs-lookup"><span data-stu-id="a4a3e-130">Type</span></span>|<span data-ttu-id="a4a3e-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a4a3e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a4a3e-132">id</span><span class="sxs-lookup"><span data-stu-id="a4a3e-132">id</span></span>|<span data-ttu-id="a4a3e-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a4a3e-133">String</span></span>|<span data-ttu-id="a4a3e-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="a4a3e-134">Key of the entity</span></span>|
|<span data-ttu-id="a4a3e-135">platformType</span><span class="sxs-lookup"><span data-stu-id="a4a3e-135">platformType</span></span>|[<span data-ttu-id="a4a3e-136">deviceType</span><span class="sxs-lookup"><span data-stu-id="a4a3e-136">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="a4a3e-137">Geräte Plattformtyp.</span><span class="sxs-lookup"><span data-stu-id="a4a3e-137">Device platform type.</span></span> <span data-ttu-id="a4a3e-138">Mögliche Werte sind: `desktop`, `windowsRT`, `winMO6` `nokia` `windowsPhone` `mac` `winCE` `iPhone` `iPad` `iPod` `android` `iSocConsumer` `unix` `macMDM`,,,,,,,, `holoLens`,, `androidEnterprise` ,,,,,, `surfaceHub` `androidForWork` `winEmbedded` , `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="a4a3e-138">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="a4a3e-139">Einstellung</span><span class="sxs-lookup"><span data-stu-id="a4a3e-139">setting</span></span>|<span data-ttu-id="a4a3e-140">String</span><span class="sxs-lookup"><span data-stu-id="a4a3e-140">String</span></span>|<span data-ttu-id="a4a3e-141">Der Klassenname und der Eigenschaftenname der Einstellung.</span><span class="sxs-lookup"><span data-stu-id="a4a3e-141">The setting class name and property name.</span></span>|
|<span data-ttu-id="a4a3e-142">settingName</span><span class="sxs-lookup"><span data-stu-id="a4a3e-142">settingName</span></span>|<span data-ttu-id="a4a3e-143">String</span><span class="sxs-lookup"><span data-stu-id="a4a3e-143">String</span></span>|<span data-ttu-id="a4a3e-144">Der gemeldete Einstellungsname</span><span class="sxs-lookup"><span data-stu-id="a4a3e-144">The Setting Name that is being reported</span></span>|
|<span data-ttu-id="a4a3e-145">deviceId</span><span class="sxs-lookup"><span data-stu-id="a4a3e-145">deviceId</span></span>|<span data-ttu-id="a4a3e-146">String</span><span class="sxs-lookup"><span data-stu-id="a4a3e-146">String</span></span>|<span data-ttu-id="a4a3e-147">Die gemeldete Geräte-ID</span><span class="sxs-lookup"><span data-stu-id="a4a3e-147">The Device Id that is being reported</span></span>|
|<span data-ttu-id="a4a3e-148">deviceName</span><span class="sxs-lookup"><span data-stu-id="a4a3e-148">deviceName</span></span>|<span data-ttu-id="a4a3e-149">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a4a3e-149">String</span></span>|<span data-ttu-id="a4a3e-150">Der gemeldete Gerätename</span><span class="sxs-lookup"><span data-stu-id="a4a3e-150">The Device Name that is being reported</span></span>|
|<span data-ttu-id="a4a3e-151">userId</span><span class="sxs-lookup"><span data-stu-id="a4a3e-151">userId</span></span>|<span data-ttu-id="a4a3e-152">String</span><span class="sxs-lookup"><span data-stu-id="a4a3e-152">String</span></span>|<span data-ttu-id="a4a3e-153">Die gemeldete Benutzer-ID</span><span class="sxs-lookup"><span data-stu-id="a4a3e-153">The user Id that is being reported</span></span>|
|<span data-ttu-id="a4a3e-154">userEmail</span><span class="sxs-lookup"><span data-stu-id="a4a3e-154">userEmail</span></span>|<span data-ttu-id="a4a3e-155">String</span><span class="sxs-lookup"><span data-stu-id="a4a3e-155">String</span></span>|<span data-ttu-id="a4a3e-156">Die gemeldete Benutzer-E-Mail-Adresse</span><span class="sxs-lookup"><span data-stu-id="a4a3e-156">The User email address that is being reported</span></span>|
|<span data-ttu-id="a4a3e-157">userName</span><span class="sxs-lookup"><span data-stu-id="a4a3e-157">userName</span></span>|<span data-ttu-id="a4a3e-158">String</span><span class="sxs-lookup"><span data-stu-id="a4a3e-158">String</span></span>|<span data-ttu-id="a4a3e-159">Gemeldeter Benutzername</span><span class="sxs-lookup"><span data-stu-id="a4a3e-159">The User Name that is being reported</span></span>|
|<span data-ttu-id="a4a3e-160">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a4a3e-160">userPrincipalName</span></span>|<span data-ttu-id="a4a3e-161">String</span><span class="sxs-lookup"><span data-stu-id="a4a3e-161">String</span></span>|<span data-ttu-id="a4a3e-162">Der gemeldete Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="a4a3e-162">The User PrincipalName that is being reported</span></span>|
|<span data-ttu-id="a4a3e-163">deviceModel</span><span class="sxs-lookup"><span data-stu-id="a4a3e-163">deviceModel</span></span>|<span data-ttu-id="a4a3e-164">String</span><span class="sxs-lookup"><span data-stu-id="a4a3e-164">String</span></span>|<span data-ttu-id="a4a3e-165">Gemeldetes Gerätemodell</span><span class="sxs-lookup"><span data-stu-id="a4a3e-165">The device model that is being reported</span></span>|
|<span data-ttu-id="a4a3e-166">state</span><span class="sxs-lookup"><span data-stu-id="a4a3e-166">state</span></span>|[<span data-ttu-id="a4a3e-167">Wurde</span><span class="sxs-lookup"><span data-stu-id="a4a3e-167">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="a4a3e-168">Der Kompatibilitätsstatus der Einstellung.</span><span class="sxs-lookup"><span data-stu-id="a4a3e-168">The compliance state of the setting.</span></span> <span data-ttu-id="a4a3e-169">Mögliche Werte: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="a4a3e-169">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="a4a3e-170">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="a4a3e-170">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="a4a3e-171">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a4a3e-171">DateTimeOffset</span></span>|<span data-ttu-id="a4a3e-172">Datum und Uhrzeit des Ablaufs der Toleranzperiode für die Gerätekonformität</span><span class="sxs-lookup"><span data-stu-id="a4a3e-172">The DateTime when device compliance grace period expires</span></span>|



## <a name="response"></a><span data-ttu-id="a4a3e-173">Antwort</span><span class="sxs-lookup"><span data-stu-id="a4a3e-173">Response</span></span>
<span data-ttu-id="a4a3e-174">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein aktualisiertes [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a4a3e-174">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a4a3e-175">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a4a3e-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="a4a3e-176">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a4a3e-176">Request</span></span>
<span data-ttu-id="a4a3e-177">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a4a3e-177">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates/{deviceComplianceSettingStateId}
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

### <a name="response"></a><span data-ttu-id="a4a3e-178">Antwort</span><span class="sxs-lookup"><span data-stu-id="a4a3e-178">Response</span></span>
<span data-ttu-id="a4a3e-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a4a3e-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




