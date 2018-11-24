# <a name="create-devicecompliancesettingstate"></a><span data-ttu-id="baf25-101">Erstellen von „deviceComplianceSettingState“</span><span class="sxs-lookup"><span data-stu-id="baf25-101">Create deviceComplianceSettingState</span></span>

> <span data-ttu-id="baf25-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="baf25-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="baf25-103">Diese Methode erstellt ein neues Objekt des Typs [deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md).</span><span class="sxs-lookup"><span data-stu-id="baf25-103">Create a new [deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="baf25-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="baf25-104">Prerequisites</span></span>
<span data-ttu-id="baf25-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="baf25-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="baf25-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="baf25-107">Permission type</span></span>|<span data-ttu-id="baf25-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="baf25-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="baf25-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="baf25-109">Delegated (work or school account)</span></span>|<span data-ttu-id="baf25-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="baf25-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="baf25-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="baf25-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="baf25-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="baf25-112">Not supported.</span></span>|
|<span data-ttu-id="baf25-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="baf25-113">Application</span></span>|<span data-ttu-id="baf25-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="baf25-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="baf25-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="baf25-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates
```

## <a name="request-headers"></a><span data-ttu-id="baf25-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="baf25-116">Request headers</span></span>
|<span data-ttu-id="baf25-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="baf25-117">Header</span></span>|<span data-ttu-id="baf25-118">Wert</span><span class="sxs-lookup"><span data-stu-id="baf25-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="baf25-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="baf25-119">Authorization</span></span>|<span data-ttu-id="baf25-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="baf25-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="baf25-121">Accept</span><span class="sxs-lookup"><span data-stu-id="baf25-121">Accept</span></span>|<span data-ttu-id="baf25-122">application/json</span><span class="sxs-lookup"><span data-stu-id="baf25-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="baf25-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="baf25-123">Request body</span></span>
<span data-ttu-id="baf25-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „deviceComplianceSettingState“ an.</span><span class="sxs-lookup"><span data-stu-id="baf25-124">In the request body, supply a JSON representation for the deviceComplianceSettingState object.</span></span>

<span data-ttu-id="baf25-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „deviceComplianceSettingState“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="baf25-125">The following table shows the properties that are required when you create the deviceComplianceSettingState.</span></span>

|<span data-ttu-id="baf25-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="baf25-126">Property</span></span>|<span data-ttu-id="baf25-127">Typ</span><span class="sxs-lookup"><span data-stu-id="baf25-127">Type</span></span>|<span data-ttu-id="baf25-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="baf25-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="baf25-129">id</span><span class="sxs-lookup"><span data-stu-id="baf25-129">id</span></span>|<span data-ttu-id="baf25-130">String</span><span class="sxs-lookup"><span data-stu-id="baf25-130">String</span></span>|<span data-ttu-id="baf25-131">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="baf25-131">Key of the entity</span></span>|
|<span data-ttu-id="baf25-132">setting</span><span class="sxs-lookup"><span data-stu-id="baf25-132">setting</span></span>|<span data-ttu-id="baf25-133">String</span><span class="sxs-lookup"><span data-stu-id="baf25-133">String</span></span>|<span data-ttu-id="baf25-134">Klassenname und Eigenschaftenname der Einstellung</span><span class="sxs-lookup"><span data-stu-id="baf25-134">The setting class name and property name.</span></span>|
|<span data-ttu-id="baf25-135">settingName</span><span class="sxs-lookup"><span data-stu-id="baf25-135">settingName</span></span>|<span data-ttu-id="baf25-136">String</span><span class="sxs-lookup"><span data-stu-id="baf25-136">String</span></span>|<span data-ttu-id="baf25-137">Gemeldeter Einstellungsname</span><span class="sxs-lookup"><span data-stu-id="baf25-137">The Setting Name that is being reported</span></span>|
|<span data-ttu-id="baf25-138">deviceId</span><span class="sxs-lookup"><span data-stu-id="baf25-138">deviceId</span></span>|<span data-ttu-id="baf25-139">String</span><span class="sxs-lookup"><span data-stu-id="baf25-139">String</span></span>|<span data-ttu-id="baf25-140">Gemeldete Geräte-ID</span><span class="sxs-lookup"><span data-stu-id="baf25-140">The Device Id that is being reported</span></span>|
|<span data-ttu-id="baf25-141">deviceName</span><span class="sxs-lookup"><span data-stu-id="baf25-141">deviceName</span></span>|<span data-ttu-id="baf25-142">String</span><span class="sxs-lookup"><span data-stu-id="baf25-142">String</span></span>|<span data-ttu-id="baf25-143">Gemeldeter Gerätename</span><span class="sxs-lookup"><span data-stu-id="baf25-143">The Device Name that is being reported</span></span>|
|<span data-ttu-id="baf25-144">userId</span><span class="sxs-lookup"><span data-stu-id="baf25-144">userId</span></span>|<span data-ttu-id="baf25-145">String</span><span class="sxs-lookup"><span data-stu-id="baf25-145">String</span></span>|<span data-ttu-id="baf25-146">Gemeldete Benutzer-ID</span><span class="sxs-lookup"><span data-stu-id="baf25-146">The user Id that is being reported</span></span>|
|<span data-ttu-id="baf25-147">userEmail</span><span class="sxs-lookup"><span data-stu-id="baf25-147">userEmail</span></span>|<span data-ttu-id="baf25-148">String</span><span class="sxs-lookup"><span data-stu-id="baf25-148">String</span></span>|<span data-ttu-id="baf25-149">Gemeldete Benutzer-E-Mail-Adresse</span><span class="sxs-lookup"><span data-stu-id="baf25-149">The User email address that is being reported</span></span>|
|<span data-ttu-id="baf25-150">userName</span><span class="sxs-lookup"><span data-stu-id="baf25-150">userName</span></span>|<span data-ttu-id="baf25-151">String</span><span class="sxs-lookup"><span data-stu-id="baf25-151">String</span></span>|<span data-ttu-id="baf25-152">Gemeldeter Benutzername</span><span class="sxs-lookup"><span data-stu-id="baf25-152">The User Name that is being reported</span></span>|
|<span data-ttu-id="baf25-153">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="baf25-153">userPrincipalName</span></span>|<span data-ttu-id="baf25-154">String</span><span class="sxs-lookup"><span data-stu-id="baf25-154">String</span></span>|<span data-ttu-id="baf25-155">Gemeldeter Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="baf25-155">The User PrincipalName that is being reported</span></span>|
|<span data-ttu-id="baf25-156">deviceModel</span><span class="sxs-lookup"><span data-stu-id="baf25-156">deviceModel</span></span>|<span data-ttu-id="baf25-157">String</span><span class="sxs-lookup"><span data-stu-id="baf25-157">String</span></span>|<span data-ttu-id="baf25-158">Gemeldetes Gerätemodell</span><span class="sxs-lookup"><span data-stu-id="baf25-158">The device model that is being reported</span></span>|
|<span data-ttu-id="baf25-159">state</span><span class="sxs-lookup"><span data-stu-id="baf25-159">state</span></span>|[<span data-ttu-id="baf25-160">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="baf25-160">complianceStatus</span></span>](../resources/intune_shared_compliancestatus.md)|<span data-ttu-id="baf25-161">Der Compliance-Zustand der Einstellung.</span><span class="sxs-lookup"><span data-stu-id="baf25-161">The compliance state of the setting.</span></span> <span data-ttu-id="baf25-162">Mögliche Werte sind: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict` und `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="baf25-162">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="baf25-163">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="baf25-163">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="baf25-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="baf25-164">DateTimeOffset</span></span>|<span data-ttu-id="baf25-165">Datum und Uhrzeit des Ablaufs der Toleranzperiode für die Gerätekonformität</span><span class="sxs-lookup"><span data-stu-id="baf25-165">The DateTime when device compliance grace period expires</span></span>|



## <a name="response"></a><span data-ttu-id="baf25-166">Antwort</span><span class="sxs-lookup"><span data-stu-id="baf25-166">Response</span></span>
<span data-ttu-id="baf25-167">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="baf25-167">If successful, this method returns a `201 Created` response code and a [deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="baf25-168">Beispiel</span><span class="sxs-lookup"><span data-stu-id="baf25-168">Example</span></span>
### <a name="request"></a><span data-ttu-id="baf25-169">Anforderung</span><span class="sxs-lookup"><span data-stu-id="baf25-169">Request</span></span>
<span data-ttu-id="baf25-170">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="baf25-170">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="baf25-171">Antwort</span><span class="sxs-lookup"><span data-stu-id="baf25-171">Response</span></span>
<span data-ttu-id="baf25-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="baf25-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



