---
title: deviceComplianceSettingState aktualisieren
description: Aktualisieren der Eigenschaften eines deviceComplianceSettingState-Objekts.
ms.openlocfilehash: 583cd56930347f1e8fda9ada9e5e2c6b4effd62a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016137"
---
# <a name="update-devicecompliancesettingstate"></a><span data-ttu-id="ea4c6-103">deviceComplianceSettingState aktualisieren</span><span class="sxs-lookup"><span data-stu-id="ea4c6-103">Update deviceComplianceSettingState</span></span>

> <span data-ttu-id="ea4c6-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="ea4c6-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ea4c6-105">Aktualisieren der Eigenschaften eines [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="ea4c6-105">Update the properties of a [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ea4c6-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="ea4c6-106">Prerequisites</span></span>
<span data-ttu-id="ea4c6-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ea4c6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ea4c6-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ea4c6-109">Permission type</span></span>|<span data-ttu-id="ea4c6-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ea4c6-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ea4c6-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ea4c6-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ea4c6-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea4c6-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ea4c6-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ea4c6-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ea4c6-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ea4c6-114">Not supported.</span></span>|
|<span data-ttu-id="ea4c6-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ea4c6-115">Application</span></span>|<span data-ttu-id="ea4c6-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ea4c6-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ea4c6-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ea4c6-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates/{deviceComplianceSettingStateId}
```

## <a name="request-headers"></a><span data-ttu-id="ea4c6-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ea4c6-118">Request headers</span></span>
|<span data-ttu-id="ea4c6-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="ea4c6-119">Header</span></span>|<span data-ttu-id="ea4c6-120">Wert</span><span class="sxs-lookup"><span data-stu-id="ea4c6-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ea4c6-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ea4c6-121">Authorization</span></span>|<span data-ttu-id="ea4c6-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="ea4c6-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ea4c6-123">Accept</span><span class="sxs-lookup"><span data-stu-id="ea4c6-123">Accept</span></span>|<span data-ttu-id="ea4c6-124">application/json</span><span class="sxs-lookup"><span data-stu-id="ea4c6-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ea4c6-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ea4c6-125">Request body</span></span>
<span data-ttu-id="ea4c6-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) an.</span><span class="sxs-lookup"><span data-stu-id="ea4c6-126">In the request body, supply a JSON representation for the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>

<span data-ttu-id="ea4c6-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="ea4c6-127">The following table shows the properties that are required when you create the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span></span>

|<span data-ttu-id="ea4c6-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ea4c6-128">Property</span></span>|<span data-ttu-id="ea4c6-129">Typ</span><span class="sxs-lookup"><span data-stu-id="ea4c6-129">Type</span></span>|<span data-ttu-id="ea4c6-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ea4c6-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ea4c6-131">id</span><span class="sxs-lookup"><span data-stu-id="ea4c6-131">id</span></span>|<span data-ttu-id="ea4c6-132">String</span><span class="sxs-lookup"><span data-stu-id="ea4c6-132">String</span></span>|<span data-ttu-id="ea4c6-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="ea4c6-133">Key of the entity</span></span>|
|<span data-ttu-id="ea4c6-134">setting</span><span class="sxs-lookup"><span data-stu-id="ea4c6-134">setting</span></span>|<span data-ttu-id="ea4c6-135">String</span><span class="sxs-lookup"><span data-stu-id="ea4c6-135">String</span></span>|<span data-ttu-id="ea4c6-136">Klassenname und Eigenschaftenname der Einstellung</span><span class="sxs-lookup"><span data-stu-id="ea4c6-136">The setting class name and property name.</span></span>|
|<span data-ttu-id="ea4c6-137">settingName</span><span class="sxs-lookup"><span data-stu-id="ea4c6-137">settingName</span></span>|<span data-ttu-id="ea4c6-138">String</span><span class="sxs-lookup"><span data-stu-id="ea4c6-138">String</span></span>|<span data-ttu-id="ea4c6-139">Gemeldeter Einstellungsname</span><span class="sxs-lookup"><span data-stu-id="ea4c6-139">The Setting Name that is being reported</span></span>|
|<span data-ttu-id="ea4c6-140">deviceId</span><span class="sxs-lookup"><span data-stu-id="ea4c6-140">deviceId</span></span>|<span data-ttu-id="ea4c6-141">String</span><span class="sxs-lookup"><span data-stu-id="ea4c6-141">String</span></span>|<span data-ttu-id="ea4c6-142">Gemeldete Geräte-ID</span><span class="sxs-lookup"><span data-stu-id="ea4c6-142">The Device Id that is being reported</span></span>|
|<span data-ttu-id="ea4c6-143">deviceName</span><span class="sxs-lookup"><span data-stu-id="ea4c6-143">deviceName</span></span>|<span data-ttu-id="ea4c6-144">String</span><span class="sxs-lookup"><span data-stu-id="ea4c6-144">String</span></span>|<span data-ttu-id="ea4c6-145">Gemeldeter Gerätename</span><span class="sxs-lookup"><span data-stu-id="ea4c6-145">The Device Name that is being reported</span></span>|
|<span data-ttu-id="ea4c6-146">userId</span><span class="sxs-lookup"><span data-stu-id="ea4c6-146">userId</span></span>|<span data-ttu-id="ea4c6-147">String</span><span class="sxs-lookup"><span data-stu-id="ea4c6-147">String</span></span>|<span data-ttu-id="ea4c6-148">Gemeldete Benutzer-ID</span><span class="sxs-lookup"><span data-stu-id="ea4c6-148">The user Id that is being reported</span></span>|
|<span data-ttu-id="ea4c6-149">userEmail</span><span class="sxs-lookup"><span data-stu-id="ea4c6-149">userEmail</span></span>|<span data-ttu-id="ea4c6-150">String</span><span class="sxs-lookup"><span data-stu-id="ea4c6-150">String</span></span>|<span data-ttu-id="ea4c6-151">Gemeldete Benutzer-E-Mail-Adresse</span><span class="sxs-lookup"><span data-stu-id="ea4c6-151">The User email address that is being reported</span></span>|
|<span data-ttu-id="ea4c6-152">userName</span><span class="sxs-lookup"><span data-stu-id="ea4c6-152">userName</span></span>|<span data-ttu-id="ea4c6-153">String</span><span class="sxs-lookup"><span data-stu-id="ea4c6-153">String</span></span>|<span data-ttu-id="ea4c6-154">Gemeldeter Benutzername</span><span class="sxs-lookup"><span data-stu-id="ea4c6-154">The User Name that is being reported</span></span>|
|<span data-ttu-id="ea4c6-155">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ea4c6-155">userPrincipalName</span></span>|<span data-ttu-id="ea4c6-156">String</span><span class="sxs-lookup"><span data-stu-id="ea4c6-156">String</span></span>|<span data-ttu-id="ea4c6-157">Gemeldeter Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="ea4c6-157">The User PrincipalName that is being reported</span></span>|
|<span data-ttu-id="ea4c6-158">deviceModel</span><span class="sxs-lookup"><span data-stu-id="ea4c6-158">deviceModel</span></span>|<span data-ttu-id="ea4c6-159">String</span><span class="sxs-lookup"><span data-stu-id="ea4c6-159">String</span></span>|<span data-ttu-id="ea4c6-160">Gemeldetes Gerätemodell</span><span class="sxs-lookup"><span data-stu-id="ea4c6-160">The device model that is being reported</span></span>|
|<span data-ttu-id="ea4c6-161">state</span><span class="sxs-lookup"><span data-stu-id="ea4c6-161">state</span></span>|[<span data-ttu-id="ea4c6-162">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="ea4c6-162">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="ea4c6-163">Der Compliance-Zustand der Einstellung.</span><span class="sxs-lookup"><span data-stu-id="ea4c6-163">The compliance state of the setting.</span></span> <span data-ttu-id="ea4c6-164">Mögliche Werte sind: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict` und `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="ea4c6-164">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="ea4c6-165">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="ea4c6-165">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="ea4c6-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ea4c6-166">DateTimeOffset</span></span>|<span data-ttu-id="ea4c6-167">Datum und Uhrzeit des Ablaufs der Toleranzperiode für die Gerätekonformität</span><span class="sxs-lookup"><span data-stu-id="ea4c6-167">The DateTime when device compliance grace period expires</span></span>|



## <a name="response"></a><span data-ttu-id="ea4c6-168">Antwort</span><span class="sxs-lookup"><span data-stu-id="ea4c6-168">Response</span></span>
<span data-ttu-id="ea4c6-169">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein aktualisiertes [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ea4c6-169">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ea4c6-170">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ea4c6-170">Example</span></span>
### <a name="request"></a><span data-ttu-id="ea4c6-171">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ea4c6-171">Request</span></span>
<span data-ttu-id="ea4c6-172">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ea4c6-172">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates/{deviceComplianceSettingStateId}
Content-type: application/json
Content-length: 517

{
  "@odata.type": "#microsoft.graph.deviceComplianceSettingState",
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

### <a name="response"></a><span data-ttu-id="ea4c6-173">Antwort</span><span class="sxs-lookup"><span data-stu-id="ea4c6-173">Response</span></span>
<span data-ttu-id="ea4c6-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ea4c6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 566

{
  "@odata.type": "#microsoft.graph.deviceComplianceSettingState",
  "id": "9905f955-f955-9905-55f9-059955f90599",
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



