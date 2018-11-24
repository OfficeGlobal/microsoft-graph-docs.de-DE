# <a name="update-devicecompliancesettingstate"></a><span data-ttu-id="8b95f-101">deviceComplianceSettingState aktualisieren</span><span class="sxs-lookup"><span data-stu-id="8b95f-101">Update deviceComplianceSettingState</span></span>

> <span data-ttu-id="8b95f-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="8b95f-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8b95f-103">Aktualisieren der Eigenschaften eines [deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="8b95f-103">Update the properties of a [deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8b95f-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="8b95f-104">Prerequisites</span></span>
<span data-ttu-id="8b95f-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="8b95f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="8b95f-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8b95f-107">Permission type</span></span>|<span data-ttu-id="8b95f-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8b95f-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8b95f-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8b95f-109">Delegated (work or school account)</span></span>|<span data-ttu-id="8b95f-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b95f-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8b95f-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8b95f-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8b95f-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8b95f-112">Not supported.</span></span>|
|<span data-ttu-id="8b95f-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8b95f-113">Application</span></span>|<span data-ttu-id="8b95f-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8b95f-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8b95f-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8b95f-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates/{deviceComplianceSettingStateId}
```

## <a name="request-headers"></a><span data-ttu-id="8b95f-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8b95f-116">Request headers</span></span>
|<span data-ttu-id="8b95f-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="8b95f-117">Header</span></span>|<span data-ttu-id="8b95f-118">Wert</span><span class="sxs-lookup"><span data-stu-id="8b95f-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8b95f-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="8b95f-119">Authorization</span></span>|<span data-ttu-id="8b95f-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="8b95f-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8b95f-121">Annehmen</span><span class="sxs-lookup"><span data-stu-id="8b95f-121">Accept</span></span>|<span data-ttu-id="8b95f-122">application/json</span><span class="sxs-lookup"><span data-stu-id="8b95f-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8b95f-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8b95f-123">Request body</span></span>
<span data-ttu-id="8b95f-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md) an.</span><span class="sxs-lookup"><span data-stu-id="8b95f-124">In the request body, supply a JSON representation for the [deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md) object.</span></span>

<span data-ttu-id="8b95f-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="8b95f-125">The following table shows the properties that are required when you create the [deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md).</span></span>

|<span data-ttu-id="8b95f-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8b95f-126">Property</span></span>|<span data-ttu-id="8b95f-127">Typ</span><span class="sxs-lookup"><span data-stu-id="8b95f-127">Type</span></span>|<span data-ttu-id="8b95f-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8b95f-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8b95f-129">id</span><span class="sxs-lookup"><span data-stu-id="8b95f-129">id</span></span>|<span data-ttu-id="8b95f-130">String</span><span class="sxs-lookup"><span data-stu-id="8b95f-130">String</span></span>|<span data-ttu-id="8b95f-131">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="8b95f-131">Key of the entity</span></span>|
|<span data-ttu-id="8b95f-132">Einstellung</span><span class="sxs-lookup"><span data-stu-id="8b95f-132">setting</span></span>|<span data-ttu-id="8b95f-133">String</span><span class="sxs-lookup"><span data-stu-id="8b95f-133">String</span></span>|<span data-ttu-id="8b95f-134">Der Klassenname und der Eigenschaftenname der Einstellung.</span><span class="sxs-lookup"><span data-stu-id="8b95f-134">The setting class name and property name.</span></span>|
|<span data-ttu-id="8b95f-135">settingName</span><span class="sxs-lookup"><span data-stu-id="8b95f-135">settingName</span></span>|<span data-ttu-id="8b95f-136">String</span><span class="sxs-lookup"><span data-stu-id="8b95f-136">String</span></span>|<span data-ttu-id="8b95f-137">Der gemeldete Einstellungsname</span><span class="sxs-lookup"><span data-stu-id="8b95f-137">The Setting Name that is being reported</span></span>|
|<span data-ttu-id="8b95f-138">deviceId</span><span class="sxs-lookup"><span data-stu-id="8b95f-138">deviceId</span></span>|<span data-ttu-id="8b95f-139">String</span><span class="sxs-lookup"><span data-stu-id="8b95f-139">String</span></span>|<span data-ttu-id="8b95f-140">Die gemeldete Geräte-ID</span><span class="sxs-lookup"><span data-stu-id="8b95f-140">The Device Id that is being reported</span></span>|
|<span data-ttu-id="8b95f-141">deviceName</span><span class="sxs-lookup"><span data-stu-id="8b95f-141">deviceName</span></span>|<span data-ttu-id="8b95f-142">String</span><span class="sxs-lookup"><span data-stu-id="8b95f-142">String</span></span>|<span data-ttu-id="8b95f-143">Der gemeldete Gerätename</span><span class="sxs-lookup"><span data-stu-id="8b95f-143">The Device Name that is being reported</span></span>|
|<span data-ttu-id="8b95f-144">userId</span><span class="sxs-lookup"><span data-stu-id="8b95f-144">userId</span></span>|<span data-ttu-id="8b95f-145">String</span><span class="sxs-lookup"><span data-stu-id="8b95f-145">String</span></span>|<span data-ttu-id="8b95f-146">Die gemeldete Benutzer-ID</span><span class="sxs-lookup"><span data-stu-id="8b95f-146">The user Id that is being reported</span></span>|
|<span data-ttu-id="8b95f-147">userEmail</span><span class="sxs-lookup"><span data-stu-id="8b95f-147">userEmail</span></span>|<span data-ttu-id="8b95f-148">String</span><span class="sxs-lookup"><span data-stu-id="8b95f-148">String</span></span>|<span data-ttu-id="8b95f-149">Die gemeldete Benutzer-E-Mail-Adresse</span><span class="sxs-lookup"><span data-stu-id="8b95f-149">The User email address that is being reported</span></span>|
|<span data-ttu-id="8b95f-150">userName</span><span class="sxs-lookup"><span data-stu-id="8b95f-150">userName</span></span>|<span data-ttu-id="8b95f-151">String</span><span class="sxs-lookup"><span data-stu-id="8b95f-151">String</span></span>|<span data-ttu-id="8b95f-152">Der gemeldete Benutzername</span><span class="sxs-lookup"><span data-stu-id="8b95f-152">The User Name that is being reported</span></span>|
|<span data-ttu-id="8b95f-153">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="8b95f-153">userPrincipalName</span></span>|<span data-ttu-id="8b95f-154">String</span><span class="sxs-lookup"><span data-stu-id="8b95f-154">String</span></span>|<span data-ttu-id="8b95f-155">Der gemeldete Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="8b95f-155">The User PrincipalName that is being reported</span></span>|
|<span data-ttu-id="8b95f-156">deviceModel</span><span class="sxs-lookup"><span data-stu-id="8b95f-156">deviceModel</span></span>|<span data-ttu-id="8b95f-157">String</span><span class="sxs-lookup"><span data-stu-id="8b95f-157">String</span></span>|<span data-ttu-id="8b95f-158">Das gemeldete Gerätemodell</span><span class="sxs-lookup"><span data-stu-id="8b95f-158">The device model that is being reported</span></span>|
|<span data-ttu-id="8b95f-159">state</span><span class="sxs-lookup"><span data-stu-id="8b95f-159">state</span></span>|[<span data-ttu-id="8b95f-160">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="8b95f-160">complianceStatus</span></span>](../resources/intune_shared_compliancestatus.md)|<span data-ttu-id="8b95f-161">Der Compliance-Zustand der Einstellung.</span><span class="sxs-lookup"><span data-stu-id="8b95f-161">The compliance state of the setting.</span></span> <span data-ttu-id="8b95f-162">Mögliche Werte sind: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict` und `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="8b95f-162">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="8b95f-163">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="8b95f-163">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="8b95f-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8b95f-164">DateTimeOffset</span></span>|<span data-ttu-id="8b95f-165">Datum und Uhrzeit des Ablaufs der Toleranzperiode für die Gerätekonformität</span><span class="sxs-lookup"><span data-stu-id="8b95f-165">The DateTime when device compliance grace period expires</span></span>|



## <a name="response"></a><span data-ttu-id="8b95f-166">Antwort</span><span class="sxs-lookup"><span data-stu-id="8b95f-166">Response</span></span>
<span data-ttu-id="8b95f-167">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein aktualisiertes [deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8b95f-167">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8b95f-168">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8b95f-168">Example</span></span>
### <a name="request"></a><span data-ttu-id="8b95f-169">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8b95f-169">Request</span></span>
<span data-ttu-id="8b95f-170">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8b95f-170">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8b95f-171">Antwort</span><span class="sxs-lookup"><span data-stu-id="8b95f-171">Response</span></span>
<span data-ttu-id="8b95f-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8b95f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



