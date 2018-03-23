# <a name="create-devicecompliancesettingstate"></a><span data-ttu-id="5e2d3-101">Erstellen von „deviceComplianceSettingState“</span><span class="sxs-lookup"><span data-stu-id="5e2d3-101">Create deviceComplianceSettingState</span></span>

> <span data-ttu-id="5e2d3-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="5e2d3-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5e2d3-103">Diese Methode erstellt ein neues Objekt des Typs [deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md).</span><span class="sxs-lookup"><span data-stu-id="5e2d3-103">Create a new [plannerBucket](../resources/intune_deviceconfig_devicecompliancesettingstate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5e2d3-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="5e2d3-104">Prerequisites</span></span>
<span data-ttu-id="5e2d3-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="5e2d3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="5e2d3-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5e2d3-107">Permission type</span></span>|<span data-ttu-id="5e2d3-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5e2d3-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5e2d3-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5e2d3-109">Delegated (work or school account)</span></span>|<span data-ttu-id="5e2d3-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5e2d3-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5e2d3-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5e2d3-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5e2d3-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5e2d3-112">Not supported.</span></span>|
|<span data-ttu-id="5e2d3-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5e2d3-113">Application</span></span>|<span data-ttu-id="5e2d3-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5e2d3-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5e2d3-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5e2d3-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates
```

## <a name="request-headers"></a><span data-ttu-id="5e2d3-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5e2d3-116">Request headers</span></span>
|<span data-ttu-id="5e2d3-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="5e2d3-117">Header</span></span>|<span data-ttu-id="5e2d3-118">Wert</span><span class="sxs-lookup"><span data-stu-id="5e2d3-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5e2d3-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="5e2d3-119">Authorization</span></span>|<span data-ttu-id="5e2d3-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="5e2d3-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="5e2d3-121">Accept</span><span class="sxs-lookup"><span data-stu-id="5e2d3-121">Accept</span></span>|<span data-ttu-id="5e2d3-122">application/json</span><span class="sxs-lookup"><span data-stu-id="5e2d3-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5e2d3-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5e2d3-123">Request body</span></span>
<span data-ttu-id="5e2d3-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „deviceComplianceSettingState“ an.</span><span class="sxs-lookup"><span data-stu-id="5e2d3-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="5e2d3-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „deviceComplianceSettingState“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="5e2d3-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="5e2d3-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5e2d3-126">Property</span></span>|<span data-ttu-id="5e2d3-127">Typ</span><span class="sxs-lookup"><span data-stu-id="5e2d3-127">Type</span></span>|<span data-ttu-id="5e2d3-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5e2d3-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5e2d3-129">id</span><span class="sxs-lookup"><span data-stu-id="5e2d3-129">id</span></span>|<span data-ttu-id="5e2d3-130">String</span><span class="sxs-lookup"><span data-stu-id="5e2d3-130">String</span></span>|<span data-ttu-id="5e2d3-131">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="5e2d3-131">Key of the setting.</span></span>|
|<span data-ttu-id="5e2d3-132">setting</span><span class="sxs-lookup"><span data-stu-id="5e2d3-132">setting</span></span>|<span data-ttu-id="5e2d3-133">String</span><span class="sxs-lookup"><span data-stu-id="5e2d3-133">String</span></span>|<span data-ttu-id="5e2d3-134">Klassenname und Eigenschaftenname der Einstellung</span><span class="sxs-lookup"><span data-stu-id="5e2d3-134">The setting class name and property name.</span></span>|
|<span data-ttu-id="5e2d3-135">settingName</span><span class="sxs-lookup"><span data-stu-id="5e2d3-135">settingName</span></span>|<span data-ttu-id="5e2d3-136">String</span><span class="sxs-lookup"><span data-stu-id="5e2d3-136">String</span></span>|<span data-ttu-id="5e2d3-137">Gemeldeter Einstellungsname</span><span class="sxs-lookup"><span data-stu-id="5e2d3-137">The Setting Name that is being reported</span></span>|
|<span data-ttu-id="5e2d3-138">deviceId</span><span class="sxs-lookup"><span data-stu-id="5e2d3-138">deviceId</span></span>|<span data-ttu-id="5e2d3-139">String</span><span class="sxs-lookup"><span data-stu-id="5e2d3-139">String</span></span>|<span data-ttu-id="5e2d3-140">Gemeldete Geräte-ID</span><span class="sxs-lookup"><span data-stu-id="5e2d3-140">The Device Id that is being reported</span></span>|
|<span data-ttu-id="5e2d3-141">deviceName</span><span class="sxs-lookup"><span data-stu-id="5e2d3-141">deviceName</span></span>|<span data-ttu-id="5e2d3-142">String</span><span class="sxs-lookup"><span data-stu-id="5e2d3-142">String</span></span>|<span data-ttu-id="5e2d3-143">Gemeldeter Gerätename</span><span class="sxs-lookup"><span data-stu-id="5e2d3-143">The Device Name that is being reported</span></span>|
|<span data-ttu-id="5e2d3-144">userId</span><span class="sxs-lookup"><span data-stu-id="5e2d3-144">userID</span></span>|<span data-ttu-id="5e2d3-145">String</span><span class="sxs-lookup"><span data-stu-id="5e2d3-145">String</span></span>|<span data-ttu-id="5e2d3-146">Gemeldete Benutzer-ID</span><span class="sxs-lookup"><span data-stu-id="5e2d3-146">The user Id that is being reported</span></span>|
|<span data-ttu-id="5e2d3-147">userEmail</span><span class="sxs-lookup"><span data-stu-id="5e2d3-147">userEmail</span></span>|<span data-ttu-id="5e2d3-148">String</span><span class="sxs-lookup"><span data-stu-id="5e2d3-148">String</span></span>|<span data-ttu-id="5e2d3-149">Gemeldete Benutzer-E-Mail-Adresse</span><span class="sxs-lookup"><span data-stu-id="5e2d3-149">The User email address that is being reported</span></span>|
|<span data-ttu-id="5e2d3-150">userName</span><span class="sxs-lookup"><span data-stu-id="5e2d3-150">UserName</span></span>|<span data-ttu-id="5e2d3-151">String</span><span class="sxs-lookup"><span data-stu-id="5e2d3-151">String</span></span>|<span data-ttu-id="5e2d3-152">Gemeldeter Benutzername</span><span class="sxs-lookup"><span data-stu-id="5e2d3-152">The User Name that is being reported</span></span>|
|<span data-ttu-id="5e2d3-153">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="5e2d3-153">userPrincipalName</span></span>|<span data-ttu-id="5e2d3-154">String</span><span class="sxs-lookup"><span data-stu-id="5e2d3-154">String</span></span>|<span data-ttu-id="5e2d3-155">Gemeldeter Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="5e2d3-155">The User PrincipalName that is being reported</span></span>|
|<span data-ttu-id="5e2d3-156">deviceModel</span><span class="sxs-lookup"><span data-stu-id="5e2d3-156">deviceModel</span></span>|<span data-ttu-id="5e2d3-157">String</span><span class="sxs-lookup"><span data-stu-id="5e2d3-157">String</span></span>|<span data-ttu-id="5e2d3-158">Gemeldetes Gerätemodell</span><span class="sxs-lookup"><span data-stu-id="5e2d3-158">The device model that is being reported</span></span>|
|<span data-ttu-id="5e2d3-159">state</span><span class="sxs-lookup"><span data-stu-id="5e2d3-159">state</span></span>|<span data-ttu-id="5e2d3-160">String</span><span class="sxs-lookup"><span data-stu-id="5e2d3-160">String</span></span>|<span data-ttu-id="5e2d3-161">Konformitätsstatus der Einstellung. Mögliche Werte sind: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error` und `conflict`.</span><span class="sxs-lookup"><span data-stu-id="5e2d3-161">The compliance state of the setting Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`.</span></span>|
|<span data-ttu-id="5e2d3-162">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="5e2d3-162">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="5e2d3-163">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5e2d3-163">DateTimeOffset</span></span>|<span data-ttu-id="5e2d3-164">Datum und Uhrzeit des Ablaufs der Toleranzperiode für die Gerätekonformität</span><span class="sxs-lookup"><span data-stu-id="5e2d3-164">The DateTime when device compliance grace period expires</span></span>|



## <a name="response"></a><span data-ttu-id="5e2d3-165">Antwort</span><span class="sxs-lookup"><span data-stu-id="5e2d3-165">Response</span></span>
<span data-ttu-id="5e2d3-166">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="5e2d3-166">If successful, this method returns a `201 Created` response code and a [section](../resources/intune_deviceconfig_devicecompliancesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5e2d3-167">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5e2d3-167">Example</span></span>
### <a name="request"></a><span data-ttu-id="5e2d3-168">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5e2d3-168">Request</span></span>
<span data-ttu-id="5e2d3-169">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5e2d3-169">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5e2d3-170">Antwort</span><span class="sxs-lookup"><span data-stu-id="5e2d3-170">Response</span></span>
<span data-ttu-id="5e2d3-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5e2d3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



