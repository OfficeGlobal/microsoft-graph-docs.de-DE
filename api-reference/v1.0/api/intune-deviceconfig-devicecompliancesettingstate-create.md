---
title: Erstellen von „deviceComplianceSettingState“
description: Diese Methode erstellt ein neues Objekt des Typs deviceComplianceSettingState.
ms.openlocfilehash: d9d1e8fb4d30fbb63381cdf90928ab815539ffca
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27015977"
---
# <a name="create-devicecompliancesettingstate"></a><span data-ttu-id="6f39d-103">Erstellen von „deviceComplianceSettingState“</span><span class="sxs-lookup"><span data-stu-id="6f39d-103">Create deviceComplianceSettingState</span></span>

> <span data-ttu-id="6f39d-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="6f39d-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6f39d-105">Diese Methode erstellt ein neues Objekt des Typs [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span><span class="sxs-lookup"><span data-stu-id="6f39d-105">Create a new [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6f39d-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="6f39d-106">Prerequisites</span></span>
<span data-ttu-id="6f39d-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6f39d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6f39d-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6f39d-109">Permission type</span></span>|<span data-ttu-id="6f39d-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6f39d-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6f39d-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6f39d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6f39d-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f39d-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6f39d-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6f39d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6f39d-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6f39d-114">Not supported.</span></span>|
|<span data-ttu-id="6f39d-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6f39d-115">Application</span></span>|<span data-ttu-id="6f39d-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6f39d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6f39d-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6f39d-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates
```

## <a name="request-headers"></a><span data-ttu-id="6f39d-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6f39d-118">Request headers</span></span>
|<span data-ttu-id="6f39d-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="6f39d-119">Header</span></span>|<span data-ttu-id="6f39d-120">Wert</span><span class="sxs-lookup"><span data-stu-id="6f39d-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6f39d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="6f39d-121">Authorization</span></span>|<span data-ttu-id="6f39d-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="6f39d-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6f39d-123">Accept</span><span class="sxs-lookup"><span data-stu-id="6f39d-123">Accept</span></span>|<span data-ttu-id="6f39d-124">application/json</span><span class="sxs-lookup"><span data-stu-id="6f39d-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6f39d-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6f39d-125">Request body</span></span>
<span data-ttu-id="6f39d-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „deviceComplianceSettingState“ an.</span><span class="sxs-lookup"><span data-stu-id="6f39d-126">In the request body, supply a JSON representation for the deviceComplianceSettingState object.</span></span>

<span data-ttu-id="6f39d-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „deviceComplianceSettingState“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="6f39d-127">The following table shows the properties that are required when you create the deviceComplianceSettingState.</span></span>

|<span data-ttu-id="6f39d-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6f39d-128">Property</span></span>|<span data-ttu-id="6f39d-129">Typ</span><span class="sxs-lookup"><span data-stu-id="6f39d-129">Type</span></span>|<span data-ttu-id="6f39d-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6f39d-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6f39d-131">id</span><span class="sxs-lookup"><span data-stu-id="6f39d-131">id</span></span>|<span data-ttu-id="6f39d-132">String</span><span class="sxs-lookup"><span data-stu-id="6f39d-132">String</span></span>|<span data-ttu-id="6f39d-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="6f39d-133">Key of the entity</span></span>|
|<span data-ttu-id="6f39d-134">setting</span><span class="sxs-lookup"><span data-stu-id="6f39d-134">setting</span></span>|<span data-ttu-id="6f39d-135">String</span><span class="sxs-lookup"><span data-stu-id="6f39d-135">String</span></span>|<span data-ttu-id="6f39d-136">Klassenname und Eigenschaftenname der Einstellung</span><span class="sxs-lookup"><span data-stu-id="6f39d-136">The setting class name and property name.</span></span>|
|<span data-ttu-id="6f39d-137">settingName</span><span class="sxs-lookup"><span data-stu-id="6f39d-137">settingName</span></span>|<span data-ttu-id="6f39d-138">String</span><span class="sxs-lookup"><span data-stu-id="6f39d-138">String</span></span>|<span data-ttu-id="6f39d-139">Gemeldeter Einstellungsname</span><span class="sxs-lookup"><span data-stu-id="6f39d-139">The Setting Name that is being reported</span></span>|
|<span data-ttu-id="6f39d-140">deviceId</span><span class="sxs-lookup"><span data-stu-id="6f39d-140">deviceId</span></span>|<span data-ttu-id="6f39d-141">String</span><span class="sxs-lookup"><span data-stu-id="6f39d-141">String</span></span>|<span data-ttu-id="6f39d-142">Gemeldete Geräte-ID</span><span class="sxs-lookup"><span data-stu-id="6f39d-142">The Device Id that is being reported</span></span>|
|<span data-ttu-id="6f39d-143">deviceName</span><span class="sxs-lookup"><span data-stu-id="6f39d-143">deviceName</span></span>|<span data-ttu-id="6f39d-144">String</span><span class="sxs-lookup"><span data-stu-id="6f39d-144">String</span></span>|<span data-ttu-id="6f39d-145">Gemeldeter Gerätename</span><span class="sxs-lookup"><span data-stu-id="6f39d-145">The Device Name that is being reported</span></span>|
|<span data-ttu-id="6f39d-146">userId</span><span class="sxs-lookup"><span data-stu-id="6f39d-146">userId</span></span>|<span data-ttu-id="6f39d-147">String</span><span class="sxs-lookup"><span data-stu-id="6f39d-147">String</span></span>|<span data-ttu-id="6f39d-148">Gemeldete Benutzer-ID</span><span class="sxs-lookup"><span data-stu-id="6f39d-148">The user Id that is being reported</span></span>|
|<span data-ttu-id="6f39d-149">userEmail</span><span class="sxs-lookup"><span data-stu-id="6f39d-149">userEmail</span></span>|<span data-ttu-id="6f39d-150">String</span><span class="sxs-lookup"><span data-stu-id="6f39d-150">String</span></span>|<span data-ttu-id="6f39d-151">Gemeldete Benutzer-E-Mail-Adresse</span><span class="sxs-lookup"><span data-stu-id="6f39d-151">The User email address that is being reported</span></span>|
|<span data-ttu-id="6f39d-152">userName</span><span class="sxs-lookup"><span data-stu-id="6f39d-152">userName</span></span>|<span data-ttu-id="6f39d-153">String</span><span class="sxs-lookup"><span data-stu-id="6f39d-153">String</span></span>|<span data-ttu-id="6f39d-154">Gemeldeter Benutzername</span><span class="sxs-lookup"><span data-stu-id="6f39d-154">The User Name that is being reported</span></span>|
|<span data-ttu-id="6f39d-155">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="6f39d-155">userPrincipalName</span></span>|<span data-ttu-id="6f39d-156">String</span><span class="sxs-lookup"><span data-stu-id="6f39d-156">String</span></span>|<span data-ttu-id="6f39d-157">Gemeldeter Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="6f39d-157">The User PrincipalName that is being reported</span></span>|
|<span data-ttu-id="6f39d-158">deviceModel</span><span class="sxs-lookup"><span data-stu-id="6f39d-158">deviceModel</span></span>|<span data-ttu-id="6f39d-159">String</span><span class="sxs-lookup"><span data-stu-id="6f39d-159">String</span></span>|<span data-ttu-id="6f39d-160">Gemeldetes Gerätemodell</span><span class="sxs-lookup"><span data-stu-id="6f39d-160">The device model that is being reported</span></span>|
|<span data-ttu-id="6f39d-161">state</span><span class="sxs-lookup"><span data-stu-id="6f39d-161">state</span></span>|[<span data-ttu-id="6f39d-162">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="6f39d-162">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="6f39d-163">Der Compliance-Zustand der Einstellung.</span><span class="sxs-lookup"><span data-stu-id="6f39d-163">The compliance state of the setting.</span></span> <span data-ttu-id="6f39d-164">Mögliche Werte sind: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict` und `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="6f39d-164">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="6f39d-165">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="6f39d-165">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="6f39d-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6f39d-166">DateTimeOffset</span></span>|<span data-ttu-id="6f39d-167">Datum und Uhrzeit des Ablaufs der Toleranzperiode für die Gerätekonformität</span><span class="sxs-lookup"><span data-stu-id="6f39d-167">The DateTime when device compliance grace period expires</span></span>|



## <a name="response"></a><span data-ttu-id="6f39d-168">Antwort</span><span class="sxs-lookup"><span data-stu-id="6f39d-168">Response</span></span>
<span data-ttu-id="6f39d-169">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="6f39d-169">If successful, this method returns a `201 Created` response code and a [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6f39d-170">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6f39d-170">Example</span></span>
### <a name="request"></a><span data-ttu-id="6f39d-171">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6f39d-171">Request</span></span>
<span data-ttu-id="6f39d-172">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6f39d-172">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates
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

### <a name="response"></a><span data-ttu-id="6f39d-173">Antwort</span><span class="sxs-lookup"><span data-stu-id="6f39d-173">Response</span></span>
<span data-ttu-id="6f39d-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6f39d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



