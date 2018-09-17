# <a name="create-devicecompliancesettingstate"></a><span data-ttu-id="fe8aa-101">Erstellen von „deviceComplianceSettingState“</span><span class="sxs-lookup"><span data-stu-id="fe8aa-101">Create deviceComplianceSettingState</span></span>

> <span data-ttu-id="fe8aa-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="fe8aa-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fe8aa-103">Diese Methode erstellt ein neues Objekt des Typs [deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md).</span><span class="sxs-lookup"><span data-stu-id="fe8aa-103">Create a new [deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fe8aa-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="fe8aa-104">Prerequisites</span></span>
<span data-ttu-id="fe8aa-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="fe8aa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="fe8aa-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="fe8aa-107">Permission type</span></span>|<span data-ttu-id="fe8aa-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="fe8aa-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fe8aa-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="fe8aa-109">Delegated (work or school account)</span></span>|<span data-ttu-id="fe8aa-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe8aa-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="fe8aa-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="fe8aa-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fe8aa-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fe8aa-112">Not supported.</span></span>|
|<span data-ttu-id="fe8aa-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="fe8aa-113">Application</span></span>|<span data-ttu-id="fe8aa-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fe8aa-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fe8aa-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="fe8aa-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates
```

## <a name="request-headers"></a><span data-ttu-id="fe8aa-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="fe8aa-116">Request headers</span></span>
|<span data-ttu-id="fe8aa-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="fe8aa-117">Header</span></span>|<span data-ttu-id="fe8aa-118">Wert</span><span class="sxs-lookup"><span data-stu-id="fe8aa-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fe8aa-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="fe8aa-119">Authorization</span></span>|<span data-ttu-id="fe8aa-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="fe8aa-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fe8aa-121">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="fe8aa-121">Accept</span></span>|<span data-ttu-id="fe8aa-122">Anwendung/json</span><span class="sxs-lookup"><span data-stu-id="fe8aa-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fe8aa-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="fe8aa-123">Request body</span></span>
<span data-ttu-id="fe8aa-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „deviceComplianceSettingState“ an.</span><span class="sxs-lookup"><span data-stu-id="fe8aa-124">In the request body, supply a JSON representation for the deviceComplianceSettingState object.</span></span>

<span data-ttu-id="fe8aa-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „deviceComplianceSettingState“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="fe8aa-125">The following table shows the properties that are required when you create the deviceComplianceSettingState.</span></span>

|<span data-ttu-id="fe8aa-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="fe8aa-126">Property</span></span>|<span data-ttu-id="fe8aa-127">Typ</span><span class="sxs-lookup"><span data-stu-id="fe8aa-127">Type</span></span>|<span data-ttu-id="fe8aa-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fe8aa-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fe8aa-129">id</span><span class="sxs-lookup"><span data-stu-id="fe8aa-129">id</span></span>|<span data-ttu-id="fe8aa-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fe8aa-130">String</span></span>|<span data-ttu-id="fe8aa-131">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="fe8aa-131">Key of the entity</span></span>|
|<span data-ttu-id="fe8aa-132">Einstellung</span><span class="sxs-lookup"><span data-stu-id="fe8aa-132">setting</span></span>|<span data-ttu-id="fe8aa-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fe8aa-133">String</span></span>|<span data-ttu-id="fe8aa-134">Klassenname und Eigenschaftenname der Einstellung</span><span class="sxs-lookup"><span data-stu-id="fe8aa-134">The setting class name and property name.</span></span>|
|<span data-ttu-id="fe8aa-135">settingName</span><span class="sxs-lookup"><span data-stu-id="fe8aa-135">settingName</span></span>|<span data-ttu-id="fe8aa-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fe8aa-136">String</span></span>|<span data-ttu-id="fe8aa-137">Gemeldeter Einstellungsname</span><span class="sxs-lookup"><span data-stu-id="fe8aa-137">The Setting Name that is being reported</span></span>|
|<span data-ttu-id="fe8aa-138">deviceId</span><span class="sxs-lookup"><span data-stu-id="fe8aa-138">deviceId</span></span>|<span data-ttu-id="fe8aa-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fe8aa-139">String</span></span>|<span data-ttu-id="fe8aa-140">Gemeldete Geräte-ID</span><span class="sxs-lookup"><span data-stu-id="fe8aa-140">The Device Id that is being reported</span></span>|
|<span data-ttu-id="fe8aa-141">deviceName</span><span class="sxs-lookup"><span data-stu-id="fe8aa-141">deviceName</span></span>|<span data-ttu-id="fe8aa-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fe8aa-142">String</span></span>|<span data-ttu-id="fe8aa-143">Gemeldeter Gerätename</span><span class="sxs-lookup"><span data-stu-id="fe8aa-143">The Device Name that is being reported</span></span>|
|<span data-ttu-id="fe8aa-144">userId</span><span class="sxs-lookup"><span data-stu-id="fe8aa-144">userId</span></span>|<span data-ttu-id="fe8aa-145">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fe8aa-145">String</span></span>|<span data-ttu-id="fe8aa-146">Gemeldete Benutzer-ID</span><span class="sxs-lookup"><span data-stu-id="fe8aa-146">The user Id that is being reported</span></span>|
|<span data-ttu-id="fe8aa-147">userEmail</span><span class="sxs-lookup"><span data-stu-id="fe8aa-147">userEmail</span></span>|<span data-ttu-id="fe8aa-148">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fe8aa-148">String</span></span>|<span data-ttu-id="fe8aa-149">Gemeldete Benutzer-E-Mail-Adresse</span><span class="sxs-lookup"><span data-stu-id="fe8aa-149">The User email address that is being reported</span></span>|
|<span data-ttu-id="fe8aa-150">userName</span><span class="sxs-lookup"><span data-stu-id="fe8aa-150">userName</span></span>|<span data-ttu-id="fe8aa-151">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fe8aa-151">String</span></span>|<span data-ttu-id="fe8aa-152">Gemeldeter Benutzername</span><span class="sxs-lookup"><span data-stu-id="fe8aa-152">The User Name that is being reported</span></span>|
|<span data-ttu-id="fe8aa-153">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="fe8aa-153">userPrincipalName</span></span>|<span data-ttu-id="fe8aa-154">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fe8aa-154">String</span></span>|<span data-ttu-id="fe8aa-155">Gemeldeter Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="fe8aa-155">The User PrincipalName that is being reported</span></span>|
|<span data-ttu-id="fe8aa-156">deviceModel</span><span class="sxs-lookup"><span data-stu-id="fe8aa-156">deviceModel</span></span>|<span data-ttu-id="fe8aa-157">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fe8aa-157">String</span></span>|<span data-ttu-id="fe8aa-158">Gemeldetes Gerätemodell</span><span class="sxs-lookup"><span data-stu-id="fe8aa-158">The device model that is being reported</span></span>|
|<span data-ttu-id="fe8aa-159">Zustand</span><span class="sxs-lookup"><span data-stu-id="fe8aa-159">state</span></span>|[<span data-ttu-id="fe8aa-160">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="fe8aa-160">complianceStatus</span></span>](../resources/intune_shared_compliancestatus.md)|<span data-ttu-id="fe8aa-p102">Der Compliance-Zustand der Einstellung. Mögliche Werte sind: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="fe8aa-p102">The compliance state of the setting Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`.</span></span>|
|<span data-ttu-id="fe8aa-163">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="fe8aa-163">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="fe8aa-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fe8aa-164">DateTimeOffset</span></span>|<span data-ttu-id="fe8aa-165">Datum und Uhrzeit des Ablaufs der Toleranzperiode für die Gerätekonformität</span><span class="sxs-lookup"><span data-stu-id="fe8aa-165">The DateTime when device compliance grace period expires</span></span>|



## <a name="response"></a><span data-ttu-id="fe8aa-166">Antwort</span><span class="sxs-lookup"><span data-stu-id="fe8aa-166">Response</span></span>
<span data-ttu-id="fe8aa-167">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="fe8aa-167">If successful, this method returns a `201 Created` response code and a [deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fe8aa-168">Beispiel</span><span class="sxs-lookup"><span data-stu-id="fe8aa-168">Example</span></span>
### <a name="request"></a><span data-ttu-id="fe8aa-169">Anforderung</span><span class="sxs-lookup"><span data-stu-id="fe8aa-169">Request</span></span>
<span data-ttu-id="fe8aa-170">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="fe8aa-170">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="fe8aa-171">Antwort</span><span class="sxs-lookup"><span data-stu-id="fe8aa-171">Response</span></span>
<span data-ttu-id="fe8aa-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fe8aa-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








