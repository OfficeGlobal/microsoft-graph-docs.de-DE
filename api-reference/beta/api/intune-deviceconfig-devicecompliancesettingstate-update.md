---
title: deviceComplianceSettingState aktualisieren
description: Aktualisieren der Eigenschaften eines deviceComplianceSettingState-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 0f607b699f4a89d925f099724851d92800ed9ddc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27807135"
---
# <a name="update-devicecompliancesettingstate"></a><span data-ttu-id="dec48-103">deviceComplianceSettingState aktualisieren</span><span class="sxs-lookup"><span data-stu-id="dec48-103">Update deviceComplianceSettingState</span></span>

> <span data-ttu-id="dec48-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="dec48-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dec48-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="dec48-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="dec48-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="dec48-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dec48-107">Aktualisieren der Eigenschaften eines [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="dec48-107">Update the properties of a [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="dec48-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="dec48-108">Prerequisites</span></span>
<span data-ttu-id="dec48-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dec48-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dec48-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="dec48-111">Permission type</span></span>|<span data-ttu-id="dec48-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="dec48-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dec48-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="dec48-113">Delegated (work or school account)</span></span>|<span data-ttu-id="dec48-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dec48-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="dec48-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="dec48-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dec48-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="dec48-116">Not supported.</span></span>|
|<span data-ttu-id="dec48-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="dec48-117">Application</span></span>|<span data-ttu-id="dec48-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="dec48-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dec48-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="dec48-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates/{deviceComplianceSettingStateId}
```

## <a name="request-headers"></a><span data-ttu-id="dec48-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="dec48-120">Request headers</span></span>
|<span data-ttu-id="dec48-121">Header</span><span class="sxs-lookup"><span data-stu-id="dec48-121">Header</span></span>|<span data-ttu-id="dec48-122">Wert</span><span class="sxs-lookup"><span data-stu-id="dec48-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dec48-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="dec48-123">Authorization</span></span>|<span data-ttu-id="dec48-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="dec48-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dec48-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="dec48-125">Accept</span></span>|<span data-ttu-id="dec48-126">application/json</span><span class="sxs-lookup"><span data-stu-id="dec48-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dec48-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="dec48-127">Request body</span></span>
<span data-ttu-id="dec48-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) an.</span><span class="sxs-lookup"><span data-stu-id="dec48-128">In the request body, supply a JSON representation for the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>

<span data-ttu-id="dec48-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="dec48-129">The following table shows the properties that are required when you create the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span></span>

|<span data-ttu-id="dec48-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="dec48-130">Property</span></span>|<span data-ttu-id="dec48-131">Typ</span><span class="sxs-lookup"><span data-stu-id="dec48-131">Type</span></span>|<span data-ttu-id="dec48-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="dec48-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dec48-133">id</span><span class="sxs-lookup"><span data-stu-id="dec48-133">id</span></span>|<span data-ttu-id="dec48-134">String</span><span class="sxs-lookup"><span data-stu-id="dec48-134">String</span></span>|<span data-ttu-id="dec48-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="dec48-135">Key of the entity</span></span>|
|<span data-ttu-id="dec48-136">platformType</span><span class="sxs-lookup"><span data-stu-id="dec48-136">platformType</span></span>|[<span data-ttu-id="dec48-137">deviceType</span><span class="sxs-lookup"><span data-stu-id="dec48-137">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="dec48-138">Gerätetyp-Plattform.</span><span class="sxs-lookup"><span data-stu-id="dec48-138">Device platform type.</span></span> <span data-ttu-id="dec48-139">Mögliche Werte sind: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise` , `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="dec48-139">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="dec48-140">setting</span><span class="sxs-lookup"><span data-stu-id="dec48-140">setting</span></span>|<span data-ttu-id="dec48-141">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="dec48-141">String</span></span>|<span data-ttu-id="dec48-142">Klassenname und Eigenschaftenname der Einstellung</span><span class="sxs-lookup"><span data-stu-id="dec48-142">The setting class name and property name.</span></span>|
|<span data-ttu-id="dec48-143">settingName</span><span class="sxs-lookup"><span data-stu-id="dec48-143">settingName</span></span>|<span data-ttu-id="dec48-144">String</span><span class="sxs-lookup"><span data-stu-id="dec48-144">String</span></span>|<span data-ttu-id="dec48-145">Gemeldeter Einstellungsname</span><span class="sxs-lookup"><span data-stu-id="dec48-145">The Setting Name that is being reported</span></span>|
|<span data-ttu-id="dec48-146">deviceId</span><span class="sxs-lookup"><span data-stu-id="dec48-146">deviceId</span></span>|<span data-ttu-id="dec48-147">String</span><span class="sxs-lookup"><span data-stu-id="dec48-147">String</span></span>|<span data-ttu-id="dec48-148">Gemeldete Geräte-ID</span><span class="sxs-lookup"><span data-stu-id="dec48-148">The Device Id that is being reported</span></span>|
|<span data-ttu-id="dec48-149">deviceName</span><span class="sxs-lookup"><span data-stu-id="dec48-149">deviceName</span></span>|<span data-ttu-id="dec48-150">String</span><span class="sxs-lookup"><span data-stu-id="dec48-150">String</span></span>|<span data-ttu-id="dec48-151">Gemeldeter Gerätename</span><span class="sxs-lookup"><span data-stu-id="dec48-151">The Device Name that is being reported</span></span>|
|<span data-ttu-id="dec48-152">userId</span><span class="sxs-lookup"><span data-stu-id="dec48-152">userId</span></span>|<span data-ttu-id="dec48-153">String</span><span class="sxs-lookup"><span data-stu-id="dec48-153">String</span></span>|<span data-ttu-id="dec48-154">Gemeldete Benutzer-ID</span><span class="sxs-lookup"><span data-stu-id="dec48-154">The user Id that is being reported</span></span>|
|<span data-ttu-id="dec48-155">userEmail</span><span class="sxs-lookup"><span data-stu-id="dec48-155">userEmail</span></span>|<span data-ttu-id="dec48-156">String</span><span class="sxs-lookup"><span data-stu-id="dec48-156">String</span></span>|<span data-ttu-id="dec48-157">Gemeldete Benutzer-E-Mail-Adresse</span><span class="sxs-lookup"><span data-stu-id="dec48-157">The User email address that is being reported</span></span>|
|<span data-ttu-id="dec48-158">userName</span><span class="sxs-lookup"><span data-stu-id="dec48-158">userName</span></span>|<span data-ttu-id="dec48-159">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="dec48-159">String</span></span>|<span data-ttu-id="dec48-160">Gemeldeter Benutzername</span><span class="sxs-lookup"><span data-stu-id="dec48-160">The User Name that is being reported</span></span>|
|<span data-ttu-id="dec48-161">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="dec48-161">userPrincipalName</span></span>|<span data-ttu-id="dec48-162">String</span><span class="sxs-lookup"><span data-stu-id="dec48-162">String</span></span>|<span data-ttu-id="dec48-163">Gemeldeter Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="dec48-163">The User PrincipalName that is being reported</span></span>|
|<span data-ttu-id="dec48-164">deviceModel</span><span class="sxs-lookup"><span data-stu-id="dec48-164">deviceModel</span></span>|<span data-ttu-id="dec48-165">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="dec48-165">String</span></span>|<span data-ttu-id="dec48-166">Gemeldetes Gerätemodell</span><span class="sxs-lookup"><span data-stu-id="dec48-166">The device model that is being reported</span></span>|
|<span data-ttu-id="dec48-167">state</span><span class="sxs-lookup"><span data-stu-id="dec48-167">state</span></span>|[<span data-ttu-id="dec48-168">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="dec48-168">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="dec48-169">Der Compliance-Zustand der Einstellung.</span><span class="sxs-lookup"><span data-stu-id="dec48-169">The compliance state of the setting.</span></span> <span data-ttu-id="dec48-170">Mögliche Werte sind: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict` und `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="dec48-170">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="dec48-171">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="dec48-171">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="dec48-172">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dec48-172">DateTimeOffset</span></span>|<span data-ttu-id="dec48-173">Datum und Uhrzeit des Ablaufs der Toleranzperiode für die Gerätekonformität</span><span class="sxs-lookup"><span data-stu-id="dec48-173">The DateTime when device compliance grace period expires</span></span>|



## <a name="response"></a><span data-ttu-id="dec48-174">Antwort</span><span class="sxs-lookup"><span data-stu-id="dec48-174">Response</span></span>
<span data-ttu-id="dec48-175">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein aktualisiertes [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="dec48-175">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dec48-176">Beispiel</span><span class="sxs-lookup"><span data-stu-id="dec48-176">Example</span></span>
### <a name="request"></a><span data-ttu-id="dec48-177">Anforderung</span><span class="sxs-lookup"><span data-stu-id="dec48-177">Request</span></span>
<span data-ttu-id="dec48-178">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="dec48-178">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates/{deviceComplianceSettingStateId}
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

### <a name="response"></a><span data-ttu-id="dec48-179">Antwort</span><span class="sxs-lookup"><span data-stu-id="dec48-179">Response</span></span>
<span data-ttu-id="dec48-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="dec48-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





