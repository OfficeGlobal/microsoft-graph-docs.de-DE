---
title: Erstellen von „deviceComplianceSettingState“
description: Diese Methode erstellt ein neues Objekt des Typs deviceComplianceSettingState.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 113960b55d75f84a463b6d49ad769b46de294ea5
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30253113"
---
# <a name="create-devicecompliancesettingstate"></a><span data-ttu-id="3be8b-103">Erstellen von „deviceComplianceSettingState“</span><span class="sxs-lookup"><span data-stu-id="3be8b-103">Create deviceComplianceSettingState</span></span>

> <span data-ttu-id="3be8b-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="3be8b-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3be8b-105">Diese Methode erstellt ein neues Objekt des Typs [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span><span class="sxs-lookup"><span data-stu-id="3be8b-105">Create a new [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3be8b-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="3be8b-106">Prerequisites</span></span>
<span data-ttu-id="3be8b-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="3be8b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="3be8b-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3be8b-109">Permission type</span></span>|<span data-ttu-id="3be8b-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3be8b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3be8b-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3be8b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3be8b-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3be8b-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3be8b-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3be8b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3be8b-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3be8b-114">Not supported.</span></span>|
|<span data-ttu-id="3be8b-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3be8b-115">Application</span></span>|<span data-ttu-id="3be8b-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3be8b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3be8b-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3be8b-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates
```

## <a name="request-headers"></a><span data-ttu-id="3be8b-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3be8b-118">Request headers</span></span>
|<span data-ttu-id="3be8b-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="3be8b-119">Header</span></span>|<span data-ttu-id="3be8b-120">Wert</span><span class="sxs-lookup"><span data-stu-id="3be8b-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3be8b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="3be8b-121">Authorization</span></span>|<span data-ttu-id="3be8b-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="3be8b-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3be8b-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="3be8b-123">Accept</span></span>|<span data-ttu-id="3be8b-124">application/json</span><span class="sxs-lookup"><span data-stu-id="3be8b-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3be8b-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3be8b-125">Request body</span></span>
<span data-ttu-id="3be8b-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „deviceComplianceSettingState“ an.</span><span class="sxs-lookup"><span data-stu-id="3be8b-126">In the request body, supply a JSON representation for the deviceComplianceSettingState object.</span></span>

<span data-ttu-id="3be8b-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „deviceComplianceSettingState“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="3be8b-127">The following table shows the properties that are required when you create the deviceComplianceSettingState.</span></span>

|<span data-ttu-id="3be8b-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3be8b-128">Property</span></span>|<span data-ttu-id="3be8b-129">Typ</span><span class="sxs-lookup"><span data-stu-id="3be8b-129">Type</span></span>|<span data-ttu-id="3be8b-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3be8b-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3be8b-131">id</span><span class="sxs-lookup"><span data-stu-id="3be8b-131">id</span></span>|<span data-ttu-id="3be8b-132">string</span><span class="sxs-lookup"><span data-stu-id="3be8b-132">String</span></span>|<span data-ttu-id="3be8b-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="3be8b-133">Key of the entity</span></span>|
|<span data-ttu-id="3be8b-134">setting</span><span class="sxs-lookup"><span data-stu-id="3be8b-134">setting</span></span>|<span data-ttu-id="3be8b-135">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3be8b-135">String</span></span>|<span data-ttu-id="3be8b-136">Klassenname und Eigenschaftenname der Einstellung</span><span class="sxs-lookup"><span data-stu-id="3be8b-136">The setting class name and property name.</span></span>|
|<span data-ttu-id="3be8b-137">settingName</span><span class="sxs-lookup"><span data-stu-id="3be8b-137">settingName</span></span>|<span data-ttu-id="3be8b-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3be8b-138">String</span></span>|<span data-ttu-id="3be8b-139">Gemeldeter Einstellungsname</span><span class="sxs-lookup"><span data-stu-id="3be8b-139">The Setting Name that is being reported</span></span>|
|<span data-ttu-id="3be8b-140">deviceId</span><span class="sxs-lookup"><span data-stu-id="3be8b-140">deviceId</span></span>|<span data-ttu-id="3be8b-141">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3be8b-141">String</span></span>|<span data-ttu-id="3be8b-142">Gemeldete Geräte-ID</span><span class="sxs-lookup"><span data-stu-id="3be8b-142">The Device Id that is being reported</span></span>|
|<span data-ttu-id="3be8b-143">deviceName</span><span class="sxs-lookup"><span data-stu-id="3be8b-143">deviceName</span></span>|<span data-ttu-id="3be8b-144">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3be8b-144">String</span></span>|<span data-ttu-id="3be8b-145">Gemeldeter Gerätename</span><span class="sxs-lookup"><span data-stu-id="3be8b-145">The Device Name that is being reported</span></span>|
|<span data-ttu-id="3be8b-146">userId</span><span class="sxs-lookup"><span data-stu-id="3be8b-146">userId</span></span>|<span data-ttu-id="3be8b-147">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3be8b-147">String</span></span>|<span data-ttu-id="3be8b-148">Gemeldete Benutzer-ID</span><span class="sxs-lookup"><span data-stu-id="3be8b-148">The user Id that is being reported</span></span>|
|<span data-ttu-id="3be8b-149">userEmail</span><span class="sxs-lookup"><span data-stu-id="3be8b-149">userEmail</span></span>|<span data-ttu-id="3be8b-150">String</span><span class="sxs-lookup"><span data-stu-id="3be8b-150">String</span></span>|<span data-ttu-id="3be8b-151">Gemeldete Benutzer-E-Mail-Adresse</span><span class="sxs-lookup"><span data-stu-id="3be8b-151">The User email address that is being reported</span></span>|
|<span data-ttu-id="3be8b-152">userName</span><span class="sxs-lookup"><span data-stu-id="3be8b-152">userName</span></span>|<span data-ttu-id="3be8b-153">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3be8b-153">String</span></span>|<span data-ttu-id="3be8b-154">Gemeldeter Benutzername</span><span class="sxs-lookup"><span data-stu-id="3be8b-154">The User Name that is being reported</span></span>|
|<span data-ttu-id="3be8b-155">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="3be8b-155">userPrincipalName</span></span>|<span data-ttu-id="3be8b-156">String</span><span class="sxs-lookup"><span data-stu-id="3be8b-156">String</span></span>|<span data-ttu-id="3be8b-157">Gemeldeter Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="3be8b-157">The User PrincipalName that is being reported</span></span>|
|<span data-ttu-id="3be8b-158">deviceModel</span><span class="sxs-lookup"><span data-stu-id="3be8b-158">deviceModel</span></span>|<span data-ttu-id="3be8b-159">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3be8b-159">String</span></span>|<span data-ttu-id="3be8b-160">Gemeldetes Gerätemodell</span><span class="sxs-lookup"><span data-stu-id="3be8b-160">The device model that is being reported</span></span>|
|<span data-ttu-id="3be8b-161">state</span><span class="sxs-lookup"><span data-stu-id="3be8b-161">state</span></span>|[<span data-ttu-id="3be8b-162">Wurde</span><span class="sxs-lookup"><span data-stu-id="3be8b-162">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="3be8b-163">Der Kompatibilitätsstatus der Einstellung.</span><span class="sxs-lookup"><span data-stu-id="3be8b-163">The compliance state of the setting.</span></span> <span data-ttu-id="3be8b-164">Mögliche Werte sind: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict` und `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="3be8b-164">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="3be8b-165">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="3be8b-165">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="3be8b-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3be8b-166">DateTimeOffset</span></span>|<span data-ttu-id="3be8b-167">Datum und Uhrzeit des Ablaufs der Toleranzperiode für die Gerätekonformität</span><span class="sxs-lookup"><span data-stu-id="3be8b-167">The DateTime when device compliance grace period expires</span></span>|



## <a name="response"></a><span data-ttu-id="3be8b-168">Antwort</span><span class="sxs-lookup"><span data-stu-id="3be8b-168">Response</span></span>
<span data-ttu-id="3be8b-169">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="3be8b-169">If successful, this method returns a `201 Created` response code and a [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3be8b-170">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3be8b-170">Example</span></span>

### <a name="request"></a><span data-ttu-id="3be8b-171">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3be8b-171">Request</span></span>
<span data-ttu-id="3be8b-172">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3be8b-172">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="3be8b-173">Antwort</span><span class="sxs-lookup"><span data-stu-id="3be8b-173">Response</span></span>
<span data-ttu-id="3be8b-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3be8b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



