---
title: Erstellen von „deviceComplianceSettingState“
description: Diese Methode erstellt ein neues Objekt des Typs deviceComplianceSettingState.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3bb79b130b1e77167ad8aecbd87d462b15581cce
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29402720"
---
# <a name="create-devicecompliancesettingstate"></a><span data-ttu-id="92e7c-103">Erstellen von „deviceComplianceSettingState“</span><span class="sxs-lookup"><span data-stu-id="92e7c-103">Create deviceComplianceSettingState</span></span>

> <span data-ttu-id="92e7c-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="92e7c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="92e7c-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="92e7c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="92e7c-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="92e7c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="92e7c-107">Diese Methode erstellt ein neues Objekt des Typs [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span><span class="sxs-lookup"><span data-stu-id="92e7c-107">Create a new [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="92e7c-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="92e7c-108">Prerequisites</span></span>
<span data-ttu-id="92e7c-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="92e7c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="92e7c-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="92e7c-111">Permission type</span></span>|<span data-ttu-id="92e7c-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="92e7c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="92e7c-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="92e7c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="92e7c-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92e7c-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="92e7c-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="92e7c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="92e7c-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="92e7c-116">Not supported.</span></span>|
|<span data-ttu-id="92e7c-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="92e7c-117">Application</span></span>|<span data-ttu-id="92e7c-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="92e7c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="92e7c-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="92e7c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates
```

## <a name="request-headers"></a><span data-ttu-id="92e7c-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="92e7c-120">Request headers</span></span>
|<span data-ttu-id="92e7c-121">Header</span><span class="sxs-lookup"><span data-stu-id="92e7c-121">Header</span></span>|<span data-ttu-id="92e7c-122">Wert</span><span class="sxs-lookup"><span data-stu-id="92e7c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="92e7c-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="92e7c-123">Authorization</span></span>|<span data-ttu-id="92e7c-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="92e7c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="92e7c-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="92e7c-125">Accept</span></span>|<span data-ttu-id="92e7c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="92e7c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="92e7c-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="92e7c-127">Request body</span></span>
<span data-ttu-id="92e7c-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „deviceComplianceSettingState“ an.</span><span class="sxs-lookup"><span data-stu-id="92e7c-128">In the request body, supply a JSON representation for the deviceComplianceSettingState object.</span></span>

<span data-ttu-id="92e7c-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „deviceComplianceSettingState“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="92e7c-129">The following table shows the properties that are required when you create the deviceComplianceSettingState.</span></span>

|<span data-ttu-id="92e7c-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="92e7c-130">Property</span></span>|<span data-ttu-id="92e7c-131">Typ</span><span class="sxs-lookup"><span data-stu-id="92e7c-131">Type</span></span>|<span data-ttu-id="92e7c-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="92e7c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="92e7c-133">id</span><span class="sxs-lookup"><span data-stu-id="92e7c-133">id</span></span>|<span data-ttu-id="92e7c-134">String</span><span class="sxs-lookup"><span data-stu-id="92e7c-134">String</span></span>|<span data-ttu-id="92e7c-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="92e7c-135">Key of the entity</span></span>|
|<span data-ttu-id="92e7c-136">platformType</span><span class="sxs-lookup"><span data-stu-id="92e7c-136">platformType</span></span>|[<span data-ttu-id="92e7c-137">deviceType</span><span class="sxs-lookup"><span data-stu-id="92e7c-137">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="92e7c-138">Gerätetyp-Plattform.</span><span class="sxs-lookup"><span data-stu-id="92e7c-138">Device platform type.</span></span> <span data-ttu-id="92e7c-139">Mögliche Werte sind: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise` , `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="92e7c-139">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="92e7c-140">setting</span><span class="sxs-lookup"><span data-stu-id="92e7c-140">setting</span></span>|<span data-ttu-id="92e7c-141">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="92e7c-141">String</span></span>|<span data-ttu-id="92e7c-142">Klassenname und Eigenschaftenname der Einstellung</span><span class="sxs-lookup"><span data-stu-id="92e7c-142">The setting class name and property name.</span></span>|
|<span data-ttu-id="92e7c-143">settingName</span><span class="sxs-lookup"><span data-stu-id="92e7c-143">settingName</span></span>|<span data-ttu-id="92e7c-144">String</span><span class="sxs-lookup"><span data-stu-id="92e7c-144">String</span></span>|<span data-ttu-id="92e7c-145">Gemeldeter Einstellungsname</span><span class="sxs-lookup"><span data-stu-id="92e7c-145">The Setting Name that is being reported</span></span>|
|<span data-ttu-id="92e7c-146">deviceId</span><span class="sxs-lookup"><span data-stu-id="92e7c-146">deviceId</span></span>|<span data-ttu-id="92e7c-147">String</span><span class="sxs-lookup"><span data-stu-id="92e7c-147">String</span></span>|<span data-ttu-id="92e7c-148">Gemeldete Geräte-ID</span><span class="sxs-lookup"><span data-stu-id="92e7c-148">The Device Id that is being reported</span></span>|
|<span data-ttu-id="92e7c-149">deviceName</span><span class="sxs-lookup"><span data-stu-id="92e7c-149">deviceName</span></span>|<span data-ttu-id="92e7c-150">String</span><span class="sxs-lookup"><span data-stu-id="92e7c-150">String</span></span>|<span data-ttu-id="92e7c-151">Gemeldeter Gerätename</span><span class="sxs-lookup"><span data-stu-id="92e7c-151">The Device Name that is being reported</span></span>|
|<span data-ttu-id="92e7c-152">userId</span><span class="sxs-lookup"><span data-stu-id="92e7c-152">userId</span></span>|<span data-ttu-id="92e7c-153">String</span><span class="sxs-lookup"><span data-stu-id="92e7c-153">String</span></span>|<span data-ttu-id="92e7c-154">Gemeldete Benutzer-ID</span><span class="sxs-lookup"><span data-stu-id="92e7c-154">The user Id that is being reported</span></span>|
|<span data-ttu-id="92e7c-155">userEmail</span><span class="sxs-lookup"><span data-stu-id="92e7c-155">userEmail</span></span>|<span data-ttu-id="92e7c-156">String</span><span class="sxs-lookup"><span data-stu-id="92e7c-156">String</span></span>|<span data-ttu-id="92e7c-157">Gemeldete Benutzer-E-Mail-Adresse</span><span class="sxs-lookup"><span data-stu-id="92e7c-157">The User email address that is being reported</span></span>|
|<span data-ttu-id="92e7c-158">userName</span><span class="sxs-lookup"><span data-stu-id="92e7c-158">userName</span></span>|<span data-ttu-id="92e7c-159">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="92e7c-159">String</span></span>|<span data-ttu-id="92e7c-160">Gemeldeter Benutzername</span><span class="sxs-lookup"><span data-stu-id="92e7c-160">The User Name that is being reported</span></span>|
|<span data-ttu-id="92e7c-161">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="92e7c-161">userPrincipalName</span></span>|<span data-ttu-id="92e7c-162">String</span><span class="sxs-lookup"><span data-stu-id="92e7c-162">String</span></span>|<span data-ttu-id="92e7c-163">Gemeldeter Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="92e7c-163">The User PrincipalName that is being reported</span></span>|
|<span data-ttu-id="92e7c-164">deviceModel</span><span class="sxs-lookup"><span data-stu-id="92e7c-164">deviceModel</span></span>|<span data-ttu-id="92e7c-165">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="92e7c-165">String</span></span>|<span data-ttu-id="92e7c-166">Gemeldetes Gerätemodell</span><span class="sxs-lookup"><span data-stu-id="92e7c-166">The device model that is being reported</span></span>|
|<span data-ttu-id="92e7c-167">state</span><span class="sxs-lookup"><span data-stu-id="92e7c-167">state</span></span>|[<span data-ttu-id="92e7c-168">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="92e7c-168">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="92e7c-169">Der Compliance-Zustand der Einstellung.</span><span class="sxs-lookup"><span data-stu-id="92e7c-169">The compliance state of the setting.</span></span> <span data-ttu-id="92e7c-170">Mögliche Werte sind: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict` und `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="92e7c-170">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="92e7c-171">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="92e7c-171">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="92e7c-172">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="92e7c-172">DateTimeOffset</span></span>|<span data-ttu-id="92e7c-173">Datum und Uhrzeit des Ablaufs der Toleranzperiode für die Gerätekonformität</span><span class="sxs-lookup"><span data-stu-id="92e7c-173">The DateTime when device compliance grace period expires</span></span>|



## <a name="response"></a><span data-ttu-id="92e7c-174">Antwort</span><span class="sxs-lookup"><span data-stu-id="92e7c-174">Response</span></span>
<span data-ttu-id="92e7c-175">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="92e7c-175">If successful, this method returns a `201 Created` response code and a [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="92e7c-176">Beispiel</span><span class="sxs-lookup"><span data-stu-id="92e7c-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="92e7c-177">Anforderung</span><span class="sxs-lookup"><span data-stu-id="92e7c-177">Request</span></span>
<span data-ttu-id="92e7c-178">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="92e7c-178">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="92e7c-179">Antwort</span><span class="sxs-lookup"><span data-stu-id="92e7c-179">Response</span></span>
<span data-ttu-id="92e7c-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="92e7c-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




