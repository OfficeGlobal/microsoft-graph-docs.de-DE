# <a name="update-manageddevicemobileappconfigurationdevicestatus"></a><span data-ttu-id="6da84-101">ManagedDeviceMobileAppConfigurationDeviceStatus aktualisieren</span><span class="sxs-lookup"><span data-stu-id="6da84-101">Update managedDeviceMobileAppConfigurationDeviceStatus</span></span>

> <span data-ttu-id="6da84-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="6da84-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6da84-103">Aktualisieren Sie die Eigenschaften eines [ManagedDeviceMobileAppConfigurationDeviceStatus](../resources/intune_apps_manageddevicemobileappconfigurationdevicestatus.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="6da84-103">Update the properties of a [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune_apps_manageddevicemobileappconfigurationdevicestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6da84-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="6da84-104">Prerequisites</span></span>
<span data-ttu-id="6da84-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="6da84-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="6da84-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6da84-107">Permission type</span></span>|<span data-ttu-id="6da84-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6da84-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6da84-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6da84-109">Delegated (work or school account)</span></span>|<span data-ttu-id="6da84-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6da84-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="6da84-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6da84-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6da84-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6da84-112">Not supported.</span></span>|
|<span data-ttu-id="6da84-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6da84-113">Application</span></span>|<span data-ttu-id="6da84-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6da84-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6da84-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6da84-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses/{managedDeviceMobileAppConfigurationDeviceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="6da84-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6da84-116">Request headers</span></span>
|<span data-ttu-id="6da84-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="6da84-117">Header</span></span>|<span data-ttu-id="6da84-118">Wert</span><span class="sxs-lookup"><span data-stu-id="6da84-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6da84-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="6da84-119">Authorization</span></span>|<span data-ttu-id="6da84-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="6da84-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6da84-121">Accept</span><span class="sxs-lookup"><span data-stu-id="6da84-121">Accept</span></span>|<span data-ttu-id="6da84-122">application/json</span><span class="sxs-lookup"><span data-stu-id="6da84-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6da84-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6da84-123">Request body</span></span>
<span data-ttu-id="6da84-124">Geben Sie im Textkörper Anforderung für das Objekt [ManagedDeviceMobileAppConfigurationDeviceStatus](../resources/intune_apps_manageddevicemobileappconfigurationdevicestatus.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="6da84-124">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune_apps_manageddevicemobileappconfigurationdevicestatus.md) object.</span></span>

<span data-ttu-id="6da84-125">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [ManagedDeviceMobileAppConfigurationDeviceStatus](../resources/intune_apps_manageddevicemobileappconfigurationdevicestatus.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="6da84-125">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune_apps_manageddevicemobileappconfigurationdevicestatus.md).</span></span>

|<span data-ttu-id="6da84-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6da84-126">Property</span></span>|<span data-ttu-id="6da84-127">Typ</span><span class="sxs-lookup"><span data-stu-id="6da84-127">Type</span></span>|<span data-ttu-id="6da84-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6da84-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6da84-129">id</span><span class="sxs-lookup"><span data-stu-id="6da84-129">id</span></span>|<span data-ttu-id="6da84-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6da84-130">String</span></span>|<span data-ttu-id="6da84-131">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="6da84-131">Key of the entity.</span></span>|
|<span data-ttu-id="6da84-132">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="6da84-132">deviceDisplayName</span></span>|<span data-ttu-id="6da84-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6da84-133">String</span></span>|<span data-ttu-id="6da84-134">Gerätename, der dem Objekt des Typs „DevicePolicyStatus“ zugeordnet ist</span><span class="sxs-lookup"><span data-stu-id="6da84-134">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="6da84-135">userName</span><span class="sxs-lookup"><span data-stu-id="6da84-135">userName</span></span>|<span data-ttu-id="6da84-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6da84-136">String</span></span>|<span data-ttu-id="6da84-137">Gemeldeter Benutzername</span><span class="sxs-lookup"><span data-stu-id="6da84-137">The User Name that is being reported</span></span>|
|<span data-ttu-id="6da84-138">deviceModel</span><span class="sxs-lookup"><span data-stu-id="6da84-138">deviceModel</span></span>|<span data-ttu-id="6da84-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6da84-139">String</span></span>|<span data-ttu-id="6da84-140">Gemeldetes Gerätemodell</span><span class="sxs-lookup"><span data-stu-id="6da84-140">The device model that is being reported</span></span>|
|<span data-ttu-id="6da84-141">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="6da84-141">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="6da84-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6da84-142">DateTimeOffset</span></span>|<span data-ttu-id="6da84-143">Datum und Uhrzeit des Ablaufs der Toleranzperiode für die Gerätekonformität</span><span class="sxs-lookup"><span data-stu-id="6da84-143">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="6da84-144">status</span><span class="sxs-lookup"><span data-stu-id="6da84-144">status</span></span>|[<span data-ttu-id="6da84-145">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="6da84-145">complianceStatus</span></span>](../resources/intune_shared_compliancestatus.md)|<span data-ttu-id="6da84-146">Konformitätsstatus des Richtlinienberichts.</span><span class="sxs-lookup"><span data-stu-id="6da84-146">Compliance status of the policy report.</span></span> <span data-ttu-id="6da84-147">Mögliche Werte sind: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict` und `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="6da84-147">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="6da84-148">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="6da84-148">lastReportedDateTime</span></span>|<span data-ttu-id="6da84-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6da84-149">DateTimeOffset</span></span>|<span data-ttu-id="6da84-150">Datum und Uhrzeit der letzten Änderung des Richtlinienberichts</span><span class="sxs-lookup"><span data-stu-id="6da84-150">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="6da84-151">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="6da84-151">userPrincipalName</span></span>|<span data-ttu-id="6da84-152">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6da84-152">String</span></span>|<span data-ttu-id="6da84-153">Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="6da84-153">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="6da84-154">Antwort</span><span class="sxs-lookup"><span data-stu-id="6da84-154">Response</span></span>
<span data-ttu-id="6da84-155">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [ManagedDeviceMobileAppConfigurationDeviceStatus](../resources/intune_apps_manageddevicemobileappconfigurationdevicestatus.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="6da84-155">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune_apps_manageddevicemobileappconfigurationdevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6da84-156">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6da84-156">Example</span></span>
### <a name="request"></a><span data-ttu-id="6da84-157">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6da84-157">Request</span></span>
<span data-ttu-id="6da84-158">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6da84-158">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses/{managedDeviceMobileAppConfigurationDeviceStatusId}
Content-type: application/json
Content-length: 445

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceStatus",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="6da84-159">Antwort</span><span class="sxs-lookup"><span data-stu-id="6da84-159">Response</span></span>
<span data-ttu-id="6da84-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6da84-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 494

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceStatus",
  "id": "477d3651-3651-477d-5136-7d4751367d47",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```



