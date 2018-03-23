# <a name="update-sharedpcconfiguration"></a><span data-ttu-id="d204c-101">sharedPCConfiguration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="d204c-101">Update sharedPCConfiguration</span></span>

> <span data-ttu-id="d204c-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="d204c-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d204c-103">Aktualisiert die Eigenschaften von Objekten des Typs [sharedPCConfiguration](../resources/intune_deviceconfig_sharedpcconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d204c-103">Update the properties of a [calendar](../resources/intune_deviceconfig_sharedpcconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d204c-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="d204c-104">Prerequisites</span></span>
<span data-ttu-id="d204c-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="d204c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d204c-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d204c-107">Permission type</span></span>|<span data-ttu-id="d204c-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d204c-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d204c-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d204c-109">Delegated (work or school account)</span></span>|<span data-ttu-id="d204c-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d204c-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d204c-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d204c-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d204c-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d204c-112">Not supported.</span></span>|
|<span data-ttu-id="d204c-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d204c-113">Application</span></span>|<span data-ttu-id="d204c-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d204c-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d204c-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d204c-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="d204c-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d204c-116">Request headers</span></span>
|<span data-ttu-id="d204c-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="d204c-117">Header</span></span>|<span data-ttu-id="d204c-118">Wert</span><span class="sxs-lookup"><span data-stu-id="d204c-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d204c-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="d204c-119">Authorization</span></span>|<span data-ttu-id="d204c-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="d204c-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="d204c-121">Annehmen</span><span class="sxs-lookup"><span data-stu-id="d204c-121">Accept</span></span>|<span data-ttu-id="d204c-122">application/json</span><span class="sxs-lookup"><span data-stu-id="d204c-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d204c-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d204c-123">Request body</span></span>
<span data-ttu-id="d204c-124">Geben Sie im Anforderungstext eine JSON-Darstellung des [sharedPCConfiguration](../resources/intune_deviceconfig_sharedpcconfiguration.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="d204c-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_deviceconfig_sharedpcconfiguration.md) object.</span></span>

<span data-ttu-id="d204c-125">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [sharedPCConfiguration](../resources/intune_deviceconfig_sharedpcconfiguration.md)-Objekts erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="d204c-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="d204c-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d204c-126">Property</span></span>|<span data-ttu-id="d204c-127">Typ</span><span class="sxs-lookup"><span data-stu-id="d204c-127">Type</span></span>|<span data-ttu-id="d204c-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d204c-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d204c-129">id</span><span class="sxs-lookup"><span data-stu-id="d204c-129">id</span></span>|<span data-ttu-id="d204c-130">String</span><span class="sxs-lookup"><span data-stu-id="d204c-130">String</span></span>|<span data-ttu-id="d204c-131">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="d204c-131">Key of the setting.</span></span> <span data-ttu-id="d204c-132">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d204c-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d204c-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d204c-133">lastModifiedDateTime</span></span>|<span data-ttu-id="d204c-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d204c-134">DateTimeOffset</span></span>|<span data-ttu-id="d204c-135">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="d204c-135">Indicates the date the object was last modified.</span></span> <span data-ttu-id="d204c-136">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d204c-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d204c-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d204c-137">createdDateTime</span></span>|<span data-ttu-id="d204c-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d204c-138">DateTimeOffset</span></span>|<span data-ttu-id="d204c-139">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="d204c-139">DateTime the object was created.</span></span> <span data-ttu-id="d204c-140">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d204c-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d204c-141">description</span><span class="sxs-lookup"><span data-stu-id="d204c-141">description</span></span>|<span data-ttu-id="d204c-142">String</span><span class="sxs-lookup"><span data-stu-id="d204c-142">String</span></span>|<span data-ttu-id="d204c-143">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="d204c-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d204c-144">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d204c-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d204c-145">displayName</span><span class="sxs-lookup"><span data-stu-id="d204c-145">displayName</span></span>|<span data-ttu-id="d204c-146">String</span><span class="sxs-lookup"><span data-stu-id="d204c-146">String</span></span>|<span data-ttu-id="d204c-147">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="d204c-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d204c-148">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d204c-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d204c-149">Version</span><span class="sxs-lookup"><span data-stu-id="d204c-149">version</span></span>|<span data-ttu-id="d204c-150">Int32</span><span class="sxs-lookup"><span data-stu-id="d204c-150">Int32</span></span>|<span data-ttu-id="d204c-151">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="d204c-151">Version of the device configuration.</span></span> <span data-ttu-id="d204c-152">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d204c-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d204c-153">accountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="d204c-153">accountManagerPolicy</span></span>|[<span data-ttu-id="d204c-154">sharedPCAccountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="d204c-154">sharedPCAccountManagerPolicy</span></span>](../resources/intune_deviceconfig_sharedpcaccountmanagerpolicy.md)|<span data-ttu-id="d204c-155">Gibt an, wie die Konten auf dem freigegebenen PC verwaltet werden sollen.</span><span class="sxs-lookup"><span data-stu-id="d204c-155">Specifies how accounts are managed on a shared PC.</span></span> <span data-ttu-id="d204c-156">Gilt nur, wenn für „disableAccountManager“ der Wert „false“ gesetzt ist.</span><span class="sxs-lookup"><span data-stu-id="d204c-156">Only applies when disableAccountManager is false.</span></span>|
|<span data-ttu-id="d204c-157">allowedAccounts</span><span class="sxs-lookup"><span data-stu-id="d204c-157">allowedAccounts</span></span>|<span data-ttu-id="d204c-158">String</span><span class="sxs-lookup"><span data-stu-id="d204c-158">String</span></span>|<span data-ttu-id="d204c-159">Gibt an, welche Typen von Konten auf einem freigegebenen PC verwendet werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="d204c-159">Indicates which type of accounts are allowed to use on a shared PC.</span></span> <span data-ttu-id="d204c-160">Mögliche Werte sind: `guest` und `domain`.</span><span class="sxs-lookup"><span data-stu-id="d204c-160">Possible values are: `guest`, `domain`.</span></span>|
|<span data-ttu-id="d204c-161">allowLocalStorage</span><span class="sxs-lookup"><span data-stu-id="d204c-161">allowLocalStorage</span></span>|<span data-ttu-id="d204c-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="d204c-162">Boolean</span></span>|<span data-ttu-id="d204c-163">Gibt an, ob eine lokale Speicherung auf dem freigegebenen PC erlaubt ist.</span><span class="sxs-lookup"><span data-stu-id="d204c-163">Specifies whether local storage is allowed on a shared PC.</span></span>|
|<span data-ttu-id="d204c-164">disableAccountManager</span><span class="sxs-lookup"><span data-stu-id="d204c-164">disableAccountManager</span></span>|<span data-ttu-id="d204c-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="d204c-165">Boolean</span></span>|<span data-ttu-id="d204c-166">Deaktiviert den Konto-Manager im Modus „Freigegebener PC“.</span><span class="sxs-lookup"><span data-stu-id="d204c-166">Disables the account manager for shared PC mode.</span></span>|
|<span data-ttu-id="d204c-167">disableEduPolicies</span><span class="sxs-lookup"><span data-stu-id="d204c-167">disableEduPolicies</span></span>|<span data-ttu-id="d204c-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="d204c-168">Boolean</span></span>|<span data-ttu-id="d204c-169">Gibt an, ob die standardmäßigen Schulungsumgebungsrichtlinien für freigegebene PCs deaktiviert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="d204c-169">Specifies whether the default shared PC education environment policies should be disabled.</span></span> <span data-ttu-id="d204c-170">Ab Windows 10 RS2 wird diese Richtlinie auch dann angewendet, wenn „enabled“ nicht auf „true“ gesetzt ist.</span><span class="sxs-lookup"><span data-stu-id="d204c-170">For Windows 10 RS2 and later, this policy will be applied without setting Enabled to true.</span></span>|
|<span data-ttu-id="d204c-171">disablePowerPolicies</span><span class="sxs-lookup"><span data-stu-id="d204c-171">disablePowerPolicies</span></span>|<span data-ttu-id="d204c-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="d204c-172">Boolean</span></span>|<span data-ttu-id="d204c-173">Gibt an, ob die standardmäßigen Energierichtlinien für freigegebene PCs deaktiviert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="d204c-173">Specifies whether the default shared PC power policies should be disabled.</span></span>|
|<span data-ttu-id="d204c-174">disableSignInOnResume</span><span class="sxs-lookup"><span data-stu-id="d204c-174">disableSignInOnResume</span></span>|<span data-ttu-id="d204c-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="d204c-175">Boolean</span></span>|<span data-ttu-id="d204c-176">Legt fest, dass nicht bei jedem Aufwachen des Geräts aus dem Energiesparmodus eine erneute Anmeldung erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="d204c-176">Disables the requirement to sign in whenever the device wakes up from sleep mode.</span></span>|
|<span data-ttu-id="d204c-177">aktiviert</span><span class="sxs-lookup"><span data-stu-id="d204c-177">enabled</span></span>|<span data-ttu-id="d204c-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="d204c-178">Boolean</span></span>|<span data-ttu-id="d204c-179">Aktiviert den Modus „Freigegebener PC“ und wendet die Richtlinien für freigegebene PCs an.</span><span class="sxs-lookup"><span data-stu-id="d204c-179">Enables shared PC mode and applies the shared pc policies.</span></span>|
|<span data-ttu-id="d204c-180">idleTimeBeforeSleepInSeconds</span><span class="sxs-lookup"><span data-stu-id="d204c-180">idleTimeBeforeSleepInSeconds</span></span>|<span data-ttu-id="d204c-181">Int32</span><span class="sxs-lookup"><span data-stu-id="d204c-181">Int32</span></span>|<span data-ttu-id="d204c-182">Gibt an, wie viele Sekunden sich der PC im Leerlauf befinden muss, bevor er in den Energiesparmodus geschaltet wird.</span><span class="sxs-lookup"><span data-stu-id="d204c-182">Specifies the time in seconds that a device must sit idle before the PC goes to sleep.</span></span> <span data-ttu-id="d204c-183">Wird dieser Wert auf „0“ gesetzt, greift kein Timeout, das den PC in den Energiesparmodus versetzt.</span><span class="sxs-lookup"><span data-stu-id="d204c-183">Setting this value to 0 prevents the sleep timeout from occurring.</span></span>|
|<span data-ttu-id="d204c-184">kioskAppDisplayName</span><span class="sxs-lookup"><span data-stu-id="d204c-184">kioskAppDisplayName</span></span>|<span data-ttu-id="d204c-185">String</span><span class="sxs-lookup"><span data-stu-id="d204c-185">String</span></span>|<span data-ttu-id="d204c-186">Gibt den Anzeigetext an, der dem Konto im Anmeldebildschirm angezeigt wird, über den die in „SetKioskAppUserModelId“ angegebene App gestartet wird.</span><span class="sxs-lookup"><span data-stu-id="d204c-186">Specifies the display text for the account shown on the sign-in screen which launches the app specified by SetKioskAppUserModelId.</span></span> <span data-ttu-id="d204c-187">Gilt nur, wenn für „kioskAppUserModelId“ ein Wert festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="d204c-187">Only applies when KioskAppUserModelId is set.</span></span>|
|<span data-ttu-id="d204c-188">kioskAppUserModelId</span><span class="sxs-lookup"><span data-stu-id="d204c-188">kioskAppUserModelId</span></span>|<span data-ttu-id="d204c-189">String</span><span class="sxs-lookup"><span data-stu-id="d204c-189">String</span></span>|<span data-ttu-id="d204c-190">Gibt die Anwendungsbenutzer-Modell-ID der App an, die über das Feature „Zugewiesener Zugriff“ genutzt werden darf.</span><span class="sxs-lookup"><span data-stu-id="d204c-190">Specifies the application user model ID of the app to use with assigned access.</span></span>|
|<span data-ttu-id="d204c-191">maintenanceStartTime</span><span class="sxs-lookup"><span data-stu-id="d204c-191">maintenanceStartTime</span></span>|<span data-ttu-id="d204c-192">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="d204c-192">TimeOfDay</span></span>|<span data-ttu-id="d204c-193">Gibt den Beginn des täglichen Wartungszeitraums an.</span><span class="sxs-lookup"><span data-stu-id="d204c-193">Specifies the daily start time of maintenance hour.</span></span>|



## <a name="response"></a><span data-ttu-id="d204c-194">Antwort</span><span class="sxs-lookup"><span data-stu-id="d204c-194">Response</span></span>
<span data-ttu-id="d204c-195">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein aktualisiertes [sharedPCConfiguration](../resources/intune_deviceconfig_sharedpcconfiguration.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d204c-195">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_deviceconfig_sharedpcconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d204c-196">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d204c-196">Example</span></span>
### <a name="request"></a><span data-ttu-id="d204c-197">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d204c-197">Request</span></span>
<span data-ttu-id="d204c-198">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d204c-198">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 864

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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

### <a name="response"></a><span data-ttu-id="d204c-199">Antwort</span><span class="sxs-lookup"><span data-stu-id="d204c-199">Response</span></span>
<span data-ttu-id="d204c-p113">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d204c-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



