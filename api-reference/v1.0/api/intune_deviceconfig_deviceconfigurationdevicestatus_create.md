# <a name="create-deviceconfigurationdevicestatus"></a><span data-ttu-id="654f2-101">Erstellen von „deviceConfigurationDeviceStatus“</span><span class="sxs-lookup"><span data-stu-id="654f2-101">Create deviceConfigurationDeviceStatus</span></span>

> <span data-ttu-id="654f2-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="654f2-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="654f2-103">Diese Methode erstellt ein neues Objekt des Typs [deviceConfigurationDeviceStatus](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="654f2-103">Create a new [plannerBucket](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="654f2-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="654f2-104">Prerequisites</span></span>
<span data-ttu-id="654f2-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="654f2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="654f2-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="654f2-107">Permission type</span></span>|<span data-ttu-id="654f2-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="654f2-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="654f2-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="654f2-109">Delegated (work or school account)</span></span>|<span data-ttu-id="654f2-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="654f2-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="654f2-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="654f2-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="654f2-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="654f2-112">Not supported.</span></span>|
|<span data-ttu-id="654f2-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="654f2-113">Application</span></span>|<span data-ttu-id="654f2-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="654f2-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="654f2-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="654f2-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="654f2-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="654f2-116">Request headers</span></span>
|<span data-ttu-id="654f2-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="654f2-117">Header</span></span>|<span data-ttu-id="654f2-118">Wert</span><span class="sxs-lookup"><span data-stu-id="654f2-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="654f2-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="654f2-119">Authorization</span></span>|<span data-ttu-id="654f2-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="654f2-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="654f2-121">Accept</span><span class="sxs-lookup"><span data-stu-id="654f2-121">Accept</span></span>|<span data-ttu-id="654f2-122">application/json</span><span class="sxs-lookup"><span data-stu-id="654f2-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="654f2-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="654f2-123">Request body</span></span>
<span data-ttu-id="654f2-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „deviceConfigurationDeviceStatus“ an.</span><span class="sxs-lookup"><span data-stu-id="654f2-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="654f2-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „deviceConfigurationDeviceStatus“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="654f2-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="654f2-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="654f2-126">Property</span></span>|<span data-ttu-id="654f2-127">Typ</span><span class="sxs-lookup"><span data-stu-id="654f2-127">Type</span></span>|<span data-ttu-id="654f2-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="654f2-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="654f2-129">id</span><span class="sxs-lookup"><span data-stu-id="654f2-129">id</span></span>|<span data-ttu-id="654f2-130">String</span><span class="sxs-lookup"><span data-stu-id="654f2-130">String</span></span>|<span data-ttu-id="654f2-131">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="654f2-131">Key of the setting.</span></span>|
|<span data-ttu-id="654f2-132">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="654f2-132">deviceDisplayName</span></span>|<span data-ttu-id="654f2-133">String</span><span class="sxs-lookup"><span data-stu-id="654f2-133">String</span></span>|<span data-ttu-id="654f2-134">Gerätename, der dem Objekt des Typs „DevicePolicyStatus“ zugeordnet ist</span><span class="sxs-lookup"><span data-stu-id="654f2-134">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="654f2-135">userName</span><span class="sxs-lookup"><span data-stu-id="654f2-135">UserName</span></span>|<span data-ttu-id="654f2-136">String</span><span class="sxs-lookup"><span data-stu-id="654f2-136">String</span></span>|<span data-ttu-id="654f2-137">Gemeldeter Benutzername</span><span class="sxs-lookup"><span data-stu-id="654f2-137">The User Name that is being reported</span></span>|
|<span data-ttu-id="654f2-138">deviceModel</span><span class="sxs-lookup"><span data-stu-id="654f2-138">deviceModel</span></span>|<span data-ttu-id="654f2-139">String</span><span class="sxs-lookup"><span data-stu-id="654f2-139">String</span></span>|<span data-ttu-id="654f2-140">Gemeldetes Gerätemodell</span><span class="sxs-lookup"><span data-stu-id="654f2-140">The device model that is being reported</span></span>|
|<span data-ttu-id="654f2-141">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="654f2-141">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="654f2-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="654f2-142">DateTimeOffset</span></span>|<span data-ttu-id="654f2-143">Datum und Uhrzeit des Ablaufs der Toleranzperiode für die Gerätekonformität</span><span class="sxs-lookup"><span data-stu-id="654f2-143">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="654f2-144">status</span><span class="sxs-lookup"><span data-stu-id="654f2-144">status</span></span>|<span data-ttu-id="654f2-145">String</span><span class="sxs-lookup"><span data-stu-id="654f2-145">String</span></span>|<span data-ttu-id="654f2-146">Konformitätsstatus des Richtlinienberichts.</span><span class="sxs-lookup"><span data-stu-id="654f2-146">Compliance status of the policy report.</span></span> <span data-ttu-id="654f2-147">Mögliche Werte sind: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error` und `conflict`.</span><span class="sxs-lookup"><span data-stu-id="654f2-147">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`.</span></span>|
|<span data-ttu-id="654f2-148">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="654f2-148">lastReportedDateTime</span></span>|<span data-ttu-id="654f2-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="654f2-149">DateTimeOffset</span></span>|<span data-ttu-id="654f2-150">Datum und Uhrzeit der letzten Änderung des Richtlinienberichts</span><span class="sxs-lookup"><span data-stu-id="654f2-150">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="654f2-151">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="654f2-151">userPrincipalName</span></span>|<span data-ttu-id="654f2-152">String</span><span class="sxs-lookup"><span data-stu-id="654f2-152">String</span></span>|<span data-ttu-id="654f2-153">Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="654f2-153">userPrincipalName</span></span>|



## <a name="response"></a><span data-ttu-id="654f2-154">Antwort</span><span class="sxs-lookup"><span data-stu-id="654f2-154">Response</span></span>
<span data-ttu-id="654f2-155">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [deviceConfigurationDeviceStatus](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="654f2-155">If successful, this method returns a `201 Created` response code and a [section](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="654f2-156">Beispiel</span><span class="sxs-lookup"><span data-stu-id="654f2-156">Example</span></span>
### <a name="request"></a><span data-ttu-id="654f2-157">Anforderung</span><span class="sxs-lookup"><span data-stu-id="654f2-157">Request</span></span>
<span data-ttu-id="654f2-158">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="654f2-158">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses
Content-type: application/json
Content-length: 429

{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceStatus",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="654f2-159">Antwort</span><span class="sxs-lookup"><span data-stu-id="654f2-159">Response</span></span>
<span data-ttu-id="654f2-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="654f2-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



