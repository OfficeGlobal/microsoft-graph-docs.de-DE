---
title: deviceComplianceSettingState aktualisieren
description: Aktualisieren der Eigenschaften eines deviceComplianceSettingState-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 735f9f3b564d7e810347d63a1c90233be7ff1de7
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30963100"
---
# <a name="update-devicecompliancesettingstate"></a><span data-ttu-id="70075-103">deviceComplianceSettingState aktualisieren</span><span class="sxs-lookup"><span data-stu-id="70075-103">Update deviceComplianceSettingState</span></span>

> <span data-ttu-id="70075-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="70075-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="70075-105">Aktualisieren der Eigenschaften eines [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="70075-105">Update the properties of a [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="70075-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="70075-106">Prerequisites</span></span>
<span data-ttu-id="70075-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="70075-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="70075-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="70075-109">Permission type</span></span>|<span data-ttu-id="70075-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="70075-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="70075-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="70075-111">Delegated (work or school account)</span></span>|<span data-ttu-id="70075-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="70075-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="70075-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="70075-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="70075-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="70075-114">Not supported.</span></span>|
|<span data-ttu-id="70075-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="70075-115">Application</span></span>|<span data-ttu-id="70075-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="70075-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="70075-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="70075-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates/{deviceComplianceSettingStateId}
```

## <a name="request-headers"></a><span data-ttu-id="70075-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="70075-118">Request headers</span></span>
|<span data-ttu-id="70075-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="70075-119">Header</span></span>|<span data-ttu-id="70075-120">Wert</span><span class="sxs-lookup"><span data-stu-id="70075-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="70075-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="70075-121">Authorization</span></span>|<span data-ttu-id="70075-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="70075-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="70075-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="70075-123">Accept</span></span>|<span data-ttu-id="70075-124">application/json</span><span class="sxs-lookup"><span data-stu-id="70075-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="70075-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="70075-125">Request body</span></span>
<span data-ttu-id="70075-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) an.</span><span class="sxs-lookup"><span data-stu-id="70075-126">In the request body, supply a JSON representation for the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>

<span data-ttu-id="70075-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="70075-127">The following table shows the properties that are required when you create the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span></span>

|<span data-ttu-id="70075-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="70075-128">Property</span></span>|<span data-ttu-id="70075-129">Typ</span><span class="sxs-lookup"><span data-stu-id="70075-129">Type</span></span>|<span data-ttu-id="70075-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="70075-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="70075-131">id</span><span class="sxs-lookup"><span data-stu-id="70075-131">id</span></span>|<span data-ttu-id="70075-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="70075-132">String</span></span>|<span data-ttu-id="70075-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="70075-133">Key of the entity</span></span>|
|<span data-ttu-id="70075-134">Einstellung</span><span class="sxs-lookup"><span data-stu-id="70075-134">setting</span></span>|<span data-ttu-id="70075-135">String</span><span class="sxs-lookup"><span data-stu-id="70075-135">String</span></span>|<span data-ttu-id="70075-136">Der Klassenname und der Eigenschaftenname der Einstellung.</span><span class="sxs-lookup"><span data-stu-id="70075-136">The setting class name and property name.</span></span>|
|<span data-ttu-id="70075-137">settingName</span><span class="sxs-lookup"><span data-stu-id="70075-137">settingName</span></span>|<span data-ttu-id="70075-138">String</span><span class="sxs-lookup"><span data-stu-id="70075-138">String</span></span>|<span data-ttu-id="70075-139">Der gemeldete Einstellungsname</span><span class="sxs-lookup"><span data-stu-id="70075-139">The Setting Name that is being reported</span></span>|
|<span data-ttu-id="70075-140">deviceId</span><span class="sxs-lookup"><span data-stu-id="70075-140">deviceId</span></span>|<span data-ttu-id="70075-141">String</span><span class="sxs-lookup"><span data-stu-id="70075-141">String</span></span>|<span data-ttu-id="70075-142">Die gemeldete Geräte-ID</span><span class="sxs-lookup"><span data-stu-id="70075-142">The Device Id that is being reported</span></span>|
|<span data-ttu-id="70075-143">deviceName</span><span class="sxs-lookup"><span data-stu-id="70075-143">deviceName</span></span>|<span data-ttu-id="70075-144">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="70075-144">String</span></span>|<span data-ttu-id="70075-145">Der gemeldete Gerätename</span><span class="sxs-lookup"><span data-stu-id="70075-145">The Device Name that is being reported</span></span>|
|<span data-ttu-id="70075-146">userId</span><span class="sxs-lookup"><span data-stu-id="70075-146">userId</span></span>|<span data-ttu-id="70075-147">String</span><span class="sxs-lookup"><span data-stu-id="70075-147">String</span></span>|<span data-ttu-id="70075-148">Die gemeldete Benutzer-ID</span><span class="sxs-lookup"><span data-stu-id="70075-148">The user Id that is being reported</span></span>|
|<span data-ttu-id="70075-149">userEmail</span><span class="sxs-lookup"><span data-stu-id="70075-149">userEmail</span></span>|<span data-ttu-id="70075-150">String</span><span class="sxs-lookup"><span data-stu-id="70075-150">String</span></span>|<span data-ttu-id="70075-151">Die gemeldete Benutzer-E-Mail-Adresse</span><span class="sxs-lookup"><span data-stu-id="70075-151">The User email address that is being reported</span></span>|
|<span data-ttu-id="70075-152">userName</span><span class="sxs-lookup"><span data-stu-id="70075-152">userName</span></span>|<span data-ttu-id="70075-153">String</span><span class="sxs-lookup"><span data-stu-id="70075-153">String</span></span>|<span data-ttu-id="70075-154">Gemeldeter Benutzername</span><span class="sxs-lookup"><span data-stu-id="70075-154">The User Name that is being reported</span></span>|
|<span data-ttu-id="70075-155">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="70075-155">userPrincipalName</span></span>|<span data-ttu-id="70075-156">String</span><span class="sxs-lookup"><span data-stu-id="70075-156">String</span></span>|<span data-ttu-id="70075-157">Der gemeldete Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="70075-157">The User PrincipalName that is being reported</span></span>|
|<span data-ttu-id="70075-158">deviceModel</span><span class="sxs-lookup"><span data-stu-id="70075-158">deviceModel</span></span>|<span data-ttu-id="70075-159">String</span><span class="sxs-lookup"><span data-stu-id="70075-159">String</span></span>|<span data-ttu-id="70075-160">Gemeldetes Gerätemodell</span><span class="sxs-lookup"><span data-stu-id="70075-160">The device model that is being reported</span></span>|
|<span data-ttu-id="70075-161">state</span><span class="sxs-lookup"><span data-stu-id="70075-161">state</span></span>|[<span data-ttu-id="70075-162">Wurde</span><span class="sxs-lookup"><span data-stu-id="70075-162">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="70075-163">Der Kompatibilitätsstatus der Einstellung.</span><span class="sxs-lookup"><span data-stu-id="70075-163">The compliance state of the setting.</span></span> <span data-ttu-id="70075-164">Mögliche Werte: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="70075-164">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="70075-165">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="70075-165">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="70075-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="70075-166">DateTimeOffset</span></span>|<span data-ttu-id="70075-167">Datum und Uhrzeit des Ablaufs der Toleranzperiode für die Gerätekonformität</span><span class="sxs-lookup"><span data-stu-id="70075-167">The DateTime when device compliance grace period expires</span></span>|



## <a name="response"></a><span data-ttu-id="70075-168">Antwort</span><span class="sxs-lookup"><span data-stu-id="70075-168">Response</span></span>
<span data-ttu-id="70075-169">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein aktualisiertes [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="70075-169">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="70075-170">Beispiel</span><span class="sxs-lookup"><span data-stu-id="70075-170">Example</span></span>

### <a name="request"></a><span data-ttu-id="70075-171">Anforderung</span><span class="sxs-lookup"><span data-stu-id="70075-171">Request</span></span>
<span data-ttu-id="70075-172">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="70075-172">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="70075-173">Antwort</span><span class="sxs-lookup"><span data-stu-id="70075-173">Response</span></span>
<span data-ttu-id="70075-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="70075-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



