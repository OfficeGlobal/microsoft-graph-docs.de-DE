# <a name="update-devicecompliancesettingstate"></a><span data-ttu-id="9f1b5-101">deviceComplianceSettingState aktualisieren</span><span class="sxs-lookup"><span data-stu-id="9f1b5-101">Update deviceComplianceSettingState</span></span>

> <span data-ttu-id="9f1b5-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="9f1b5-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9f1b5-103">Aktualisieren der Eigenschaften eines [deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="9f1b5-103">Update the properties of a [calendar](../resources/intune_deviceconfig_devicecompliancesettingstate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9f1b5-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="9f1b5-104">Prerequisites</span></span>
<span data-ttu-id="9f1b5-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="9f1b5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="9f1b5-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9f1b5-107">Permission type</span></span>|<span data-ttu-id="9f1b5-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9f1b5-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9f1b5-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9f1b5-109">Delegated (work or school account)</span></span>|<span data-ttu-id="9f1b5-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f1b5-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9f1b5-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9f1b5-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9f1b5-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9f1b5-112">Not supported.</span></span>|
|<span data-ttu-id="9f1b5-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9f1b5-113">Application</span></span>|<span data-ttu-id="9f1b5-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9f1b5-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9f1b5-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9f1b5-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates/{deviceComplianceSettingStateId}
```

## <a name="request-headers"></a><span data-ttu-id="9f1b5-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9f1b5-116">Request headers</span></span>
|<span data-ttu-id="9f1b5-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="9f1b5-117">Header</span></span>|<span data-ttu-id="9f1b5-118">Wert</span><span class="sxs-lookup"><span data-stu-id="9f1b5-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9f1b5-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="9f1b5-119">Authorization</span></span>|<span data-ttu-id="9f1b5-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="9f1b5-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="9f1b5-121">Annehmen</span><span class="sxs-lookup"><span data-stu-id="9f1b5-121">Accept</span></span>|<span data-ttu-id="9f1b5-122">application/json</span><span class="sxs-lookup"><span data-stu-id="9f1b5-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9f1b5-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9f1b5-123">Request body</span></span>
<span data-ttu-id="9f1b5-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md) an.</span><span class="sxs-lookup"><span data-stu-id="9f1b5-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_deviceconfig_devicecompliancesettingstate.md) object.</span></span>

<span data-ttu-id="9f1b5-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="9f1b5-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="9f1b5-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9f1b5-126">Property</span></span>|<span data-ttu-id="9f1b5-127">Typ</span><span class="sxs-lookup"><span data-stu-id="9f1b5-127">Type</span></span>|<span data-ttu-id="9f1b5-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9f1b5-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9f1b5-129">id</span><span class="sxs-lookup"><span data-stu-id="9f1b5-129">id</span></span>|<span data-ttu-id="9f1b5-130">String</span><span class="sxs-lookup"><span data-stu-id="9f1b5-130">String</span></span>|<span data-ttu-id="9f1b5-131">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="9f1b5-131">Key of the setting.</span></span>|
|<span data-ttu-id="9f1b5-132">Einstellung</span><span class="sxs-lookup"><span data-stu-id="9f1b5-132">setting</span></span>|<span data-ttu-id="9f1b5-133">String</span><span class="sxs-lookup"><span data-stu-id="9f1b5-133">String</span></span>|<span data-ttu-id="9f1b5-134">Der Klassenname und der Eigenschaftenname der Einstellung.</span><span class="sxs-lookup"><span data-stu-id="9f1b5-134">The setting class name and property name.</span></span>|
|<span data-ttu-id="9f1b5-135">settingName</span><span class="sxs-lookup"><span data-stu-id="9f1b5-135">settingName</span></span>|<span data-ttu-id="9f1b5-136">String</span><span class="sxs-lookup"><span data-stu-id="9f1b5-136">String</span></span>|<span data-ttu-id="9f1b5-137">Der gemeldete Einstellungsname</span><span class="sxs-lookup"><span data-stu-id="9f1b5-137">The Setting Name that is being reported</span></span>|
|<span data-ttu-id="9f1b5-138">deviceId</span><span class="sxs-lookup"><span data-stu-id="9f1b5-138">deviceId</span></span>|<span data-ttu-id="9f1b5-139">String</span><span class="sxs-lookup"><span data-stu-id="9f1b5-139">String</span></span>|<span data-ttu-id="9f1b5-140">Die gemeldete Geräte-ID</span><span class="sxs-lookup"><span data-stu-id="9f1b5-140">The Device Id that is being reported</span></span>|
|<span data-ttu-id="9f1b5-141">deviceName</span><span class="sxs-lookup"><span data-stu-id="9f1b5-141">deviceName</span></span>|<span data-ttu-id="9f1b5-142">String</span><span class="sxs-lookup"><span data-stu-id="9f1b5-142">String</span></span>|<span data-ttu-id="9f1b5-143">Der gemeldete Gerätename</span><span class="sxs-lookup"><span data-stu-id="9f1b5-143">The Device Name that is being reported</span></span>|
|<span data-ttu-id="9f1b5-144">userId</span><span class="sxs-lookup"><span data-stu-id="9f1b5-144">userID</span></span>|<span data-ttu-id="9f1b5-145">String</span><span class="sxs-lookup"><span data-stu-id="9f1b5-145">String</span></span>|<span data-ttu-id="9f1b5-146">Die gemeldete Benutzer-ID</span><span class="sxs-lookup"><span data-stu-id="9f1b5-146">The user Id that is being reported</span></span>|
|<span data-ttu-id="9f1b5-147">userEmail</span><span class="sxs-lookup"><span data-stu-id="9f1b5-147">userEmail</span></span>|<span data-ttu-id="9f1b5-148">String</span><span class="sxs-lookup"><span data-stu-id="9f1b5-148">String</span></span>|<span data-ttu-id="9f1b5-149">Die gemeldete Benutzer-E-Mail-Adresse</span><span class="sxs-lookup"><span data-stu-id="9f1b5-149">The User email address that is being reported</span></span>|
|<span data-ttu-id="9f1b5-150">userName</span><span class="sxs-lookup"><span data-stu-id="9f1b5-150">UserName</span></span>|<span data-ttu-id="9f1b5-151">String</span><span class="sxs-lookup"><span data-stu-id="9f1b5-151">String</span></span>|<span data-ttu-id="9f1b5-152">Der gemeldete Benutzername</span><span class="sxs-lookup"><span data-stu-id="9f1b5-152">The User Name that is being reported</span></span>|
|<span data-ttu-id="9f1b5-153">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="9f1b5-153">userPrincipalName</span></span>|<span data-ttu-id="9f1b5-154">String</span><span class="sxs-lookup"><span data-stu-id="9f1b5-154">String</span></span>|<span data-ttu-id="9f1b5-155">Der gemeldete Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="9f1b5-155">The User PrincipalName that is being reported</span></span>|
|<span data-ttu-id="9f1b5-156">deviceModel</span><span class="sxs-lookup"><span data-stu-id="9f1b5-156">deviceModel</span></span>|<span data-ttu-id="9f1b5-157">String</span><span class="sxs-lookup"><span data-stu-id="9f1b5-157">String</span></span>|<span data-ttu-id="9f1b5-158">Das gemeldete Gerätemodell</span><span class="sxs-lookup"><span data-stu-id="9f1b5-158">The device model that is being reported</span></span>|
|<span data-ttu-id="9f1b5-159">state</span><span class="sxs-lookup"><span data-stu-id="9f1b5-159">state</span></span>|<span data-ttu-id="9f1b5-160">String</span><span class="sxs-lookup"><span data-stu-id="9f1b5-160">String</span></span>|<span data-ttu-id="9f1b5-161">Der Konformitätsstatus der Einstellung. Mögliche Werte: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`.</span><span class="sxs-lookup"><span data-stu-id="9f1b5-161">The compliance state of the setting Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`.</span></span>|
|<span data-ttu-id="9f1b5-162">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="9f1b5-162">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="9f1b5-163">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9f1b5-163">DateTimeOffset</span></span>|<span data-ttu-id="9f1b5-164">Datum und Uhrzeit des Ablaufs der Toleranzperiode für die Gerätekonformität</span><span class="sxs-lookup"><span data-stu-id="9f1b5-164">The DateTime when device compliance grace period expires</span></span>|



## <a name="response"></a><span data-ttu-id="9f1b5-165">Antwort</span><span class="sxs-lookup"><span data-stu-id="9f1b5-165">Response</span></span>
<span data-ttu-id="9f1b5-166">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein aktualisiertes [deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9f1b5-166">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_deviceconfig_devicecompliancesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9f1b5-167">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9f1b5-167">Example</span></span>
### <a name="request"></a><span data-ttu-id="9f1b5-168">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9f1b5-168">Request</span></span>
<span data-ttu-id="9f1b5-169">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9f1b5-169">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates/{deviceComplianceSettingStateId}
Content-type: application/json
Content-length: 450

{
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

### <a name="response"></a><span data-ttu-id="9f1b5-170">Antwort</span><span class="sxs-lookup"><span data-stu-id="9f1b5-170">Response</span></span>
<span data-ttu-id="9f1b5-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9f1b5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



