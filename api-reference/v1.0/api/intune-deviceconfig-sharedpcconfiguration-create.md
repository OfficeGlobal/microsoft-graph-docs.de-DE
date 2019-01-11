---
title: Erstellen von „sharedPCConfiguration“
description: Diese Methode erstellt ein neues Objekt des Typs sharedPCConfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 76b88f1b42a2009232de7691c1daebd6e7315280
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27857659"
---
# <a name="create-sharedpcconfiguration"></a><span data-ttu-id="a3b62-103">Erstellen von „sharedPCConfiguration“</span><span class="sxs-lookup"><span data-stu-id="a3b62-103">Create sharedPCConfiguration</span></span>

> <span data-ttu-id="a3b62-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="a3b62-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a3b62-105">Diese Methode erstellt ein neues Objekt des Typs [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a3b62-105">Create a new [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a3b62-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="a3b62-106">Prerequisites</span></span>
<span data-ttu-id="a3b62-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a3b62-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a3b62-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a3b62-109">Permission type</span></span>|<span data-ttu-id="a3b62-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a3b62-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a3b62-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a3b62-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a3b62-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a3b62-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a3b62-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a3b62-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a3b62-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a3b62-114">Not supported.</span></span>|
|<span data-ttu-id="a3b62-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a3b62-115">Application</span></span>|<span data-ttu-id="a3b62-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a3b62-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a3b62-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a3b62-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a3b62-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a3b62-118">Request headers</span></span>
|<span data-ttu-id="a3b62-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="a3b62-119">Header</span></span>|<span data-ttu-id="a3b62-120">Wert</span><span class="sxs-lookup"><span data-stu-id="a3b62-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a3b62-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a3b62-121">Authorization</span></span>|<span data-ttu-id="a3b62-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="a3b62-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a3b62-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="a3b62-123">Accept</span></span>|<span data-ttu-id="a3b62-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a3b62-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a3b62-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a3b62-125">Request body</span></span>
<span data-ttu-id="a3b62-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „sharedPCConfiguration“ an.</span><span class="sxs-lookup"><span data-stu-id="a3b62-126">In the request body, supply a JSON representation for the sharedPCConfiguration object.</span></span>

<span data-ttu-id="a3b62-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „sharedPCConfiguration“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="a3b62-127">The following table shows the properties that are required when you create the sharedPCConfiguration.</span></span>

|<span data-ttu-id="a3b62-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a3b62-128">Property</span></span>|<span data-ttu-id="a3b62-129">Typ</span><span class="sxs-lookup"><span data-stu-id="a3b62-129">Type</span></span>|<span data-ttu-id="a3b62-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a3b62-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a3b62-131">id</span><span class="sxs-lookup"><span data-stu-id="a3b62-131">id</span></span>|<span data-ttu-id="a3b62-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a3b62-132">String</span></span>|<span data-ttu-id="a3b62-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="a3b62-133">Key of the entity.</span></span> <span data-ttu-id="a3b62-134">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a3b62-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a3b62-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a3b62-135">lastModifiedDateTime</span></span>|<span data-ttu-id="a3b62-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a3b62-136">DateTimeOffset</span></span>|<span data-ttu-id="a3b62-137">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="a3b62-137">DateTime the object was last modified.</span></span> <span data-ttu-id="a3b62-138">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a3b62-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a3b62-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a3b62-139">createdDateTime</span></span>|<span data-ttu-id="a3b62-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a3b62-140">DateTimeOffset</span></span>|<span data-ttu-id="a3b62-141">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="a3b62-141">DateTime the object was created.</span></span> <span data-ttu-id="a3b62-142">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a3b62-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a3b62-143">description</span><span class="sxs-lookup"><span data-stu-id="a3b62-143">description</span></span>|<span data-ttu-id="a3b62-144">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a3b62-144">String</span></span>|<span data-ttu-id="a3b62-145">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="a3b62-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a3b62-146">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a3b62-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a3b62-147">displayName</span><span class="sxs-lookup"><span data-stu-id="a3b62-147">displayName</span></span>|<span data-ttu-id="a3b62-148">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a3b62-148">String</span></span>|<span data-ttu-id="a3b62-149">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="a3b62-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a3b62-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a3b62-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a3b62-151">Version</span><span class="sxs-lookup"><span data-stu-id="a3b62-151">version</span></span>|<span data-ttu-id="a3b62-152">Int32</span><span class="sxs-lookup"><span data-stu-id="a3b62-152">Int32</span></span>|<span data-ttu-id="a3b62-153">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="a3b62-153">Version of the device configuration.</span></span> <span data-ttu-id="a3b62-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a3b62-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a3b62-155">accountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="a3b62-155">accountManagerPolicy</span></span>|[<span data-ttu-id="a3b62-156">sharedPCAccountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="a3b62-156">sharedPCAccountManagerPolicy</span></span>](../resources/intune-deviceconfig-sharedpcaccountmanagerpolicy.md)|<span data-ttu-id="a3b62-157">Gibt an, wie die Konten auf dem freigegebenen PC verwaltet werden sollen.</span><span class="sxs-lookup"><span data-stu-id="a3b62-157">Specifies how accounts are managed on a shared PC.</span></span> <span data-ttu-id="a3b62-158">Gilt nur, wenn für „disableAccountManager“ der Wert „false“ gesetzt ist.</span><span class="sxs-lookup"><span data-stu-id="a3b62-158">Only applies when disableAccountManager is false.</span></span>|
|<span data-ttu-id="a3b62-159">allowedAccounts</span><span class="sxs-lookup"><span data-stu-id="a3b62-159">allowedAccounts</span></span>|[<span data-ttu-id="a3b62-160">sharedPCAllowedAccountType</span><span class="sxs-lookup"><span data-stu-id="a3b62-160">sharedPCAllowedAccountType</span></span>](../resources/intune-deviceconfig-sharedpcallowedaccounttype.md)|<span data-ttu-id="a3b62-161">Gibt an, welche Typen von Konten auf einem freigegebenen PC verwendet werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="a3b62-161">Indicates which type of accounts are allowed to use on a shared PC.</span></span> <span data-ttu-id="a3b62-162">Mögliche Werte sind: `guest` und `domain`.</span><span class="sxs-lookup"><span data-stu-id="a3b62-162">Possible values are: `guest`, `domain`.</span></span>|
|<span data-ttu-id="a3b62-163">allowLocalStorage</span><span class="sxs-lookup"><span data-stu-id="a3b62-163">allowLocalStorage</span></span>|<span data-ttu-id="a3b62-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="a3b62-164">Boolean</span></span>|<span data-ttu-id="a3b62-165">Gibt an, ob eine lokale Speicherung auf dem freigegebenen PC erlaubt ist.</span><span class="sxs-lookup"><span data-stu-id="a3b62-165">Specifies whether local storage is allowed on a shared PC.</span></span>|
|<span data-ttu-id="a3b62-166">disableAccountManager</span><span class="sxs-lookup"><span data-stu-id="a3b62-166">disableAccountManager</span></span>|<span data-ttu-id="a3b62-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="a3b62-167">Boolean</span></span>|<span data-ttu-id="a3b62-168">Deaktiviert den Konto-Manager im Modus „Freigegebener PC“.</span><span class="sxs-lookup"><span data-stu-id="a3b62-168">Disables the account manager for shared PC mode.</span></span>|
|<span data-ttu-id="a3b62-169">disableEduPolicies</span><span class="sxs-lookup"><span data-stu-id="a3b62-169">disableEduPolicies</span></span>|<span data-ttu-id="a3b62-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="a3b62-170">Boolean</span></span>|<span data-ttu-id="a3b62-171">Gibt an, ob die standardmäßigen Schulungsumgebungsrichtlinien für freigegebene PCs deaktiviert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="a3b62-171">Specifies whether the default shared PC education environment policies should be disabled.</span></span> <span data-ttu-id="a3b62-172">Ab Windows 10 RS2 wird diese Richtlinie auch dann angewendet, wenn „enabled“ nicht auf „true“ gesetzt ist.</span><span class="sxs-lookup"><span data-stu-id="a3b62-172">For Windows 10 RS2 and later, this policy will be applied without setting Enabled to true.</span></span>|
|<span data-ttu-id="a3b62-173">disablePowerPolicies</span><span class="sxs-lookup"><span data-stu-id="a3b62-173">disablePowerPolicies</span></span>|<span data-ttu-id="a3b62-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="a3b62-174">Boolean</span></span>|<span data-ttu-id="a3b62-175">Gibt an, ob die standardmäßigen Energierichtlinien für freigegebene PCs deaktiviert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="a3b62-175">Specifies whether the default shared PC power policies should be disabled.</span></span>|
|<span data-ttu-id="a3b62-176">disableSignInOnResume</span><span class="sxs-lookup"><span data-stu-id="a3b62-176">disableSignInOnResume</span></span>|<span data-ttu-id="a3b62-177">Boolean</span><span class="sxs-lookup"><span data-stu-id="a3b62-177">Boolean</span></span>|<span data-ttu-id="a3b62-178">Legt fest, dass nicht bei jedem Aufwachen des Geräts aus dem Energiesparmodus eine erneute Anmeldung erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="a3b62-178">Disables the requirement to sign in whenever the device wakes up from sleep mode.</span></span>|
|<span data-ttu-id="a3b62-179">enabled</span><span class="sxs-lookup"><span data-stu-id="a3b62-179">enabled</span></span>|<span data-ttu-id="a3b62-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="a3b62-180">Boolean</span></span>|<span data-ttu-id="a3b62-181">Aktiviert den Modus „Freigegebener PC“ und wendet die Richtlinien für freigegebene PCs an.</span><span class="sxs-lookup"><span data-stu-id="a3b62-181">Enables shared PC mode and applies the shared pc policies.</span></span>|
|<span data-ttu-id="a3b62-182">idleTimeBeforeSleepInSeconds</span><span class="sxs-lookup"><span data-stu-id="a3b62-182">idleTimeBeforeSleepInSeconds</span></span>|<span data-ttu-id="a3b62-183">Int32</span><span class="sxs-lookup"><span data-stu-id="a3b62-183">Int32</span></span>|<span data-ttu-id="a3b62-184">Gibt an, wie viele Sekunden sich der PC im Leerlauf befinden muss, bevor er in den Energiesparmodus geschaltet wird.</span><span class="sxs-lookup"><span data-stu-id="a3b62-184">Specifies the time in seconds that a device must sit idle before the PC goes to sleep.</span></span> <span data-ttu-id="a3b62-185">Wird dieser Wert auf „0“ gesetzt, greift kein Timeout, das den PC in den Energiesparmodus versetzt.</span><span class="sxs-lookup"><span data-stu-id="a3b62-185">Setting this value to 0 prevents the sleep timeout from occurring.</span></span>|
|<span data-ttu-id="a3b62-186">kioskAppDisplayName</span><span class="sxs-lookup"><span data-stu-id="a3b62-186">kioskAppDisplayName</span></span>|<span data-ttu-id="a3b62-187">String</span><span class="sxs-lookup"><span data-stu-id="a3b62-187">String</span></span>|<span data-ttu-id="a3b62-188">Gibt den Anzeigetext an, der dem Konto im Anmeldebildschirm angezeigt wird, über den die in „SetKioskAppUserModelId“ angegebene App gestartet wird.</span><span class="sxs-lookup"><span data-stu-id="a3b62-188">Specifies the display text for the account shown on the sign-in screen which launches the app specified by SetKioskAppUserModelId.</span></span> <span data-ttu-id="a3b62-189">Gilt nur, wenn für „kioskAppUserModelId“ ein Wert festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="a3b62-189">Only applies when KioskAppUserModelId is set.</span></span>|
|<span data-ttu-id="a3b62-190">kioskAppUserModelId</span><span class="sxs-lookup"><span data-stu-id="a3b62-190">kioskAppUserModelId</span></span>|<span data-ttu-id="a3b62-191">String</span><span class="sxs-lookup"><span data-stu-id="a3b62-191">String</span></span>|<span data-ttu-id="a3b62-192">Gibt die Anwendungsbenutzer-Modell-ID der App an, die über das Feature „Zugewiesener Zugriff“ genutzt werden darf.</span><span class="sxs-lookup"><span data-stu-id="a3b62-192">Specifies the application user model ID of the app to use with assigned access.</span></span>|
|<span data-ttu-id="a3b62-193">maintenanceStartTime</span><span class="sxs-lookup"><span data-stu-id="a3b62-193">maintenanceStartTime</span></span>|<span data-ttu-id="a3b62-194">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="a3b62-194">TimeOfDay</span></span>|<span data-ttu-id="a3b62-195">Gibt den Beginn des täglichen Wartungszeitraums an.</span><span class="sxs-lookup"><span data-stu-id="a3b62-195">Specifies the daily start time of maintenance hour.</span></span>|



## <a name="response"></a><span data-ttu-id="a3b62-196">Antwort</span><span class="sxs-lookup"><span data-stu-id="a3b62-196">Response</span></span>
<span data-ttu-id="a3b62-197">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) im Antworttext an.</span><span class="sxs-lookup"><span data-stu-id="a3b62-197">If successful, this method returns a `201 Created` response code and a [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a3b62-198">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a3b62-198">Example</span></span>
### <a name="request"></a><span data-ttu-id="a3b62-199">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a3b62-199">Request</span></span>
<span data-ttu-id="a3b62-200">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a3b62-200">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 860

{
  "@odata.type": "#microsoft.graph.sharedPCConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "accountManagerPolicy": {
    "@odata.type": "microsoft.graph.sharedPCAccountManagerPolicy",
    "accountDeletionPolicy": "diskSpaceThreshold",
    "cacheAccountsAboveDiskFreePercentage": 4,
    "inactiveThresholdDays": 5,
    "removeAccountsBelowDiskFreePercentage": 5
  },
  "allowedAccounts": "domain",
  "allowLocalStorage": true,
  "disableAccountManager": true,
  "disableEduPolicies": true,
  "disablePowerPolicies": true,
  "disableSignInOnResume": true,
  "enabled": true,
  "idleTimeBeforeSleepInSeconds": 12,
  "kioskAppDisplayName": "Kiosk App Display Name value",
  "kioskAppUserModelId": "Kiosk App User Model Id value",
  "maintenanceStartTime": "11:59:24.7240000"
}
```

### <a name="response"></a><span data-ttu-id="a3b62-201">Antwort</span><span class="sxs-lookup"><span data-stu-id="a3b62-201">Response</span></span>
<span data-ttu-id="a3b62-p113">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a3b62-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1032

{
  "@odata.type": "#microsoft.graph.sharedPCConfiguration",
  "id": "5206be3b-be3b-5206-3bbe-06523bbe0652",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "accountManagerPolicy": {
    "@odata.type": "microsoft.graph.sharedPCAccountManagerPolicy",
    "accountDeletionPolicy": "diskSpaceThreshold",
    "cacheAccountsAboveDiskFreePercentage": 4,
    "inactiveThresholdDays": 5,
    "removeAccountsBelowDiskFreePercentage": 5
  },
  "allowedAccounts": "domain",
  "allowLocalStorage": true,
  "disableAccountManager": true,
  "disableEduPolicies": true,
  "disablePowerPolicies": true,
  "disableSignInOnResume": true,
  "enabled": true,
  "idleTimeBeforeSleepInSeconds": 12,
  "kioskAppDisplayName": "Kiosk App Display Name value",
  "kioskAppUserModelId": "Kiosk App User Model Id value",
  "maintenanceStartTime": "11:59:24.7240000"
}
```



