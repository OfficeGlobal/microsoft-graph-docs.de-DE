---
title: deviceComplianceSettingState aktualisieren
description: Aktualisieren der Eigenschaften eines deviceComplianceSettingState-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: ce9dbae6f3b0ffe3b84323018ff37036a554518f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398254"
---
# <a name="update-devicecompliancesettingstate"></a><span data-ttu-id="c0358-103">deviceComplianceSettingState aktualisieren</span><span class="sxs-lookup"><span data-stu-id="c0358-103">Update deviceComplianceSettingState</span></span>

> <span data-ttu-id="c0358-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="c0358-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c0358-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c0358-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c0358-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c0358-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c0358-107">Aktualisieren der Eigenschaften eines [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="c0358-107">Update the properties of a [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c0358-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c0358-108">Prerequisites</span></span>
<span data-ttu-id="c0358-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="c0358-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="c0358-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c0358-111">Permission type</span></span>|<span data-ttu-id="c0358-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c0358-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c0358-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c0358-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c0358-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0358-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c0358-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c0358-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c0358-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c0358-116">Not supported.</span></span>|
|<span data-ttu-id="c0358-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c0358-117">Application</span></span>|<span data-ttu-id="c0358-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c0358-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c0358-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c0358-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates/{deviceComplianceSettingStateId}
```

## <a name="request-headers"></a><span data-ttu-id="c0358-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c0358-120">Request headers</span></span>
|<span data-ttu-id="c0358-121">Header</span><span class="sxs-lookup"><span data-stu-id="c0358-121">Header</span></span>|<span data-ttu-id="c0358-122">Wert</span><span class="sxs-lookup"><span data-stu-id="c0358-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c0358-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="c0358-123">Authorization</span></span>|<span data-ttu-id="c0358-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c0358-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c0358-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="c0358-125">Accept</span></span>|<span data-ttu-id="c0358-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c0358-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c0358-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c0358-127">Request body</span></span>
<span data-ttu-id="c0358-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) an.</span><span class="sxs-lookup"><span data-stu-id="c0358-128">In the request body, supply a JSON representation for the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>

<span data-ttu-id="c0358-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="c0358-129">The following table shows the properties that are required when you create the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span></span>

|<span data-ttu-id="c0358-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c0358-130">Property</span></span>|<span data-ttu-id="c0358-131">Typ</span><span class="sxs-lookup"><span data-stu-id="c0358-131">Type</span></span>|<span data-ttu-id="c0358-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c0358-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c0358-133">id</span><span class="sxs-lookup"><span data-stu-id="c0358-133">id</span></span>|<span data-ttu-id="c0358-134">String</span><span class="sxs-lookup"><span data-stu-id="c0358-134">String</span></span>|<span data-ttu-id="c0358-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="c0358-135">Key of the entity</span></span>|
|<span data-ttu-id="c0358-136">platformType</span><span class="sxs-lookup"><span data-stu-id="c0358-136">platformType</span></span>|[<span data-ttu-id="c0358-137">deviceType</span><span class="sxs-lookup"><span data-stu-id="c0358-137">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="c0358-138">Gerätetyp-Plattform.</span><span class="sxs-lookup"><span data-stu-id="c0358-138">Device platform type.</span></span> <span data-ttu-id="c0358-139">Mögliche Werte sind: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise` , `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="c0358-139">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="c0358-140">setting</span><span class="sxs-lookup"><span data-stu-id="c0358-140">setting</span></span>|<span data-ttu-id="c0358-141">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c0358-141">String</span></span>|<span data-ttu-id="c0358-142">Klassenname und Eigenschaftenname der Einstellung</span><span class="sxs-lookup"><span data-stu-id="c0358-142">The setting class name and property name.</span></span>|
|<span data-ttu-id="c0358-143">settingName</span><span class="sxs-lookup"><span data-stu-id="c0358-143">settingName</span></span>|<span data-ttu-id="c0358-144">String</span><span class="sxs-lookup"><span data-stu-id="c0358-144">String</span></span>|<span data-ttu-id="c0358-145">Gemeldeter Einstellungsname</span><span class="sxs-lookup"><span data-stu-id="c0358-145">The Setting Name that is being reported</span></span>|
|<span data-ttu-id="c0358-146">deviceId</span><span class="sxs-lookup"><span data-stu-id="c0358-146">deviceId</span></span>|<span data-ttu-id="c0358-147">String</span><span class="sxs-lookup"><span data-stu-id="c0358-147">String</span></span>|<span data-ttu-id="c0358-148">Gemeldete Geräte-ID</span><span class="sxs-lookup"><span data-stu-id="c0358-148">The Device Id that is being reported</span></span>|
|<span data-ttu-id="c0358-149">deviceName</span><span class="sxs-lookup"><span data-stu-id="c0358-149">deviceName</span></span>|<span data-ttu-id="c0358-150">String</span><span class="sxs-lookup"><span data-stu-id="c0358-150">String</span></span>|<span data-ttu-id="c0358-151">Gemeldeter Gerätename</span><span class="sxs-lookup"><span data-stu-id="c0358-151">The Device Name that is being reported</span></span>|
|<span data-ttu-id="c0358-152">userId</span><span class="sxs-lookup"><span data-stu-id="c0358-152">userId</span></span>|<span data-ttu-id="c0358-153">String</span><span class="sxs-lookup"><span data-stu-id="c0358-153">String</span></span>|<span data-ttu-id="c0358-154">Gemeldete Benutzer-ID</span><span class="sxs-lookup"><span data-stu-id="c0358-154">The user Id that is being reported</span></span>|
|<span data-ttu-id="c0358-155">userEmail</span><span class="sxs-lookup"><span data-stu-id="c0358-155">userEmail</span></span>|<span data-ttu-id="c0358-156">String</span><span class="sxs-lookup"><span data-stu-id="c0358-156">String</span></span>|<span data-ttu-id="c0358-157">Gemeldete Benutzer-E-Mail-Adresse</span><span class="sxs-lookup"><span data-stu-id="c0358-157">The User email address that is being reported</span></span>|
|<span data-ttu-id="c0358-158">userName</span><span class="sxs-lookup"><span data-stu-id="c0358-158">userName</span></span>|<span data-ttu-id="c0358-159">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c0358-159">String</span></span>|<span data-ttu-id="c0358-160">Gemeldeter Benutzername</span><span class="sxs-lookup"><span data-stu-id="c0358-160">The User Name that is being reported</span></span>|
|<span data-ttu-id="c0358-161">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="c0358-161">userPrincipalName</span></span>|<span data-ttu-id="c0358-162">String</span><span class="sxs-lookup"><span data-stu-id="c0358-162">String</span></span>|<span data-ttu-id="c0358-163">Gemeldeter Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="c0358-163">The User PrincipalName that is being reported</span></span>|
|<span data-ttu-id="c0358-164">deviceModel</span><span class="sxs-lookup"><span data-stu-id="c0358-164">deviceModel</span></span>|<span data-ttu-id="c0358-165">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c0358-165">String</span></span>|<span data-ttu-id="c0358-166">Gemeldetes Gerätemodell</span><span class="sxs-lookup"><span data-stu-id="c0358-166">The device model that is being reported</span></span>|
|<span data-ttu-id="c0358-167">state</span><span class="sxs-lookup"><span data-stu-id="c0358-167">state</span></span>|[<span data-ttu-id="c0358-168">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="c0358-168">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="c0358-169">Der Compliance-Zustand der Einstellung.</span><span class="sxs-lookup"><span data-stu-id="c0358-169">The compliance state of the setting.</span></span> <span data-ttu-id="c0358-170">Mögliche Werte sind: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict` und `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="c0358-170">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="c0358-171">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="c0358-171">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="c0358-172">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c0358-172">DateTimeOffset</span></span>|<span data-ttu-id="c0358-173">Datum und Uhrzeit des Ablaufs der Toleranzperiode für die Gerätekonformität</span><span class="sxs-lookup"><span data-stu-id="c0358-173">The DateTime when device compliance grace period expires</span></span>|



## <a name="response"></a><span data-ttu-id="c0358-174">Antwort</span><span class="sxs-lookup"><span data-stu-id="c0358-174">Response</span></span>
<span data-ttu-id="c0358-175">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein aktualisiertes [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c0358-175">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c0358-176">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c0358-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="c0358-177">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c0358-177">Request</span></span>
<span data-ttu-id="c0358-178">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c0358-178">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c0358-179">Antwort</span><span class="sxs-lookup"><span data-stu-id="c0358-179">Response</span></span>
<span data-ttu-id="c0358-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c0358-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




