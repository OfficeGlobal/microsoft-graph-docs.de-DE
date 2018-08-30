# <a name="update-deviceconfigurationdevicestatus"></a><span data-ttu-id="667ed-101">Aktualisieren von „deviceConfigurationDeviceStatus“</span><span class="sxs-lookup"><span data-stu-id="667ed-101">Update deviceConfigurationDeviceStatus</span></span>

> <span data-ttu-id="667ed-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="667ed-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="667ed-103">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [deviceConfigurationDeviceStatus](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="667ed-103">Update the properties of a [deviceConfigurationDeviceStatus](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="667ed-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="667ed-104">Prerequisites</span></span>
<span data-ttu-id="667ed-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="667ed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="667ed-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="667ed-107">Permission type</span></span>|<span data-ttu-id="667ed-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="667ed-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="667ed-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="667ed-109">Delegated (work or school account)</span></span>|<span data-ttu-id="667ed-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="667ed-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="667ed-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="667ed-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="667ed-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="667ed-112">Not supported.</span></span>|
|<span data-ttu-id="667ed-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="667ed-113">Application</span></span>|<span data-ttu-id="667ed-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="667ed-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="667ed-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="667ed-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses/{deviceConfigurationDeviceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="667ed-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="667ed-116">Request headers</span></span>
|<span data-ttu-id="667ed-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="667ed-117">Header</span></span>|<span data-ttu-id="667ed-118">Wert</span><span class="sxs-lookup"><span data-stu-id="667ed-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="667ed-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="667ed-119">Authorization</span></span>|<span data-ttu-id="667ed-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="667ed-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="667ed-121">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="667ed-121">Accept</span></span>|<span data-ttu-id="667ed-122">Anwendung/json</span><span class="sxs-lookup"><span data-stu-id="667ed-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="667ed-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="667ed-123">Request body</span></span>
<span data-ttu-id="667ed-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceConfigurationDeviceStatus](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md) an.</span><span class="sxs-lookup"><span data-stu-id="667ed-124">In the request body, supply a JSON representation for the [deviceConfigurationDeviceStatus](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md) object.</span></span>

<span data-ttu-id="667ed-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceConfigurationDeviceStatus](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="667ed-125">The following table shows the properties that are required when you create the [deviceConfigurationDeviceStatus](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md).</span></span>

|<span data-ttu-id="667ed-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="667ed-126">Property</span></span>|<span data-ttu-id="667ed-127">Typ</span><span class="sxs-lookup"><span data-stu-id="667ed-127">Type</span></span>|<span data-ttu-id="667ed-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="667ed-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="667ed-129">ID</span><span class="sxs-lookup"><span data-stu-id="667ed-129">id</span></span>|<span data-ttu-id="667ed-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="667ed-130">String</span></span>|<span data-ttu-id="667ed-131">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="667ed-131">Key of the entity.</span></span>|
|<span data-ttu-id="667ed-132">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="667ed-132">deviceDisplayName</span></span>|<span data-ttu-id="667ed-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="667ed-133">String</span></span>|<span data-ttu-id="667ed-134">Gerätename, der dem Objekt des Typs „DevicePolicyStatus“ zugeordnet ist</span><span class="sxs-lookup"><span data-stu-id="667ed-134">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="667ed-135">userName</span><span class="sxs-lookup"><span data-stu-id="667ed-135">userName</span></span>|<span data-ttu-id="667ed-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="667ed-136">String</span></span>|<span data-ttu-id="667ed-137">Gemeldeter Benutzername</span><span class="sxs-lookup"><span data-stu-id="667ed-137">The User Name that is being reported</span></span>|
|<span data-ttu-id="667ed-138">deviceModel</span><span class="sxs-lookup"><span data-stu-id="667ed-138">deviceModel</span></span>|<span data-ttu-id="667ed-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="667ed-139">String</span></span>|<span data-ttu-id="667ed-140">Gemeldetes Gerätemodell</span><span class="sxs-lookup"><span data-stu-id="667ed-140">The device model that is being reported</span></span>|
|<span data-ttu-id="667ed-141">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="667ed-141">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="667ed-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="667ed-142">DateTimeOffset</span></span>|<span data-ttu-id="667ed-143">Datum und Uhrzeit des Ablaufs der Toleranzperiode für die Gerätekonformität</span><span class="sxs-lookup"><span data-stu-id="667ed-143">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="667ed-144">Status</span><span class="sxs-lookup"><span data-stu-id="667ed-144">status</span></span>|[<span data-ttu-id="667ed-145">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="667ed-145">complianceStatus</span></span>](../resources/intune_shared_compliancestatus.md)|<span data-ttu-id="667ed-146">Compliance-Status des Richtlinienberichts.</span><span class="sxs-lookup"><span data-stu-id="667ed-146">Compliance status of the policy report.</span></span> <span data-ttu-id="667ed-147">Mögliche Werte: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`.</span><span class="sxs-lookup"><span data-stu-id="667ed-147">The possible values are `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, , , , , or .</span></span>|
|<span data-ttu-id="667ed-148">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="667ed-148">lastReportedDateTime</span></span>|<span data-ttu-id="667ed-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="667ed-149">DateTimeOffset</span></span>|<span data-ttu-id="667ed-150">Datum und Uhrzeit der letzten Änderung des Richtlinienberichts</span><span class="sxs-lookup"><span data-stu-id="667ed-150">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="667ed-151">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="667ed-151">userPrincipalName</span></span>|<span data-ttu-id="667ed-152">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="667ed-152">String</span></span>|<span data-ttu-id="667ed-153">Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="667ed-153">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="667ed-154">Antwort</span><span class="sxs-lookup"><span data-stu-id="667ed-154">Response</span></span>
<span data-ttu-id="667ed-155">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [deviceConfigurationDeviceStatus](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="667ed-155">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationDeviceStatus](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="667ed-156">Beispiel</span><span class="sxs-lookup"><span data-stu-id="667ed-156">Example</span></span>
### <a name="request"></a><span data-ttu-id="667ed-157">Anforderung</span><span class="sxs-lookup"><span data-stu-id="667ed-157">Request</span></span>
<span data-ttu-id="667ed-158">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="667ed-158">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses/{deviceConfigurationDeviceStatusId}
Content-type: application/json
Content-length: 359

{
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="667ed-159">Antwort</span><span class="sxs-lookup"><span data-stu-id="667ed-159">Response</span></span>
<span data-ttu-id="667ed-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="667ed-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 478

{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceStatus",
  "id": "674e98e5-98e5-674e-e598-4e67e5984e67",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```



