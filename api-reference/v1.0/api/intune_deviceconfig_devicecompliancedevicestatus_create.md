# <a name="create-devicecompliancedevicestatus"></a><span data-ttu-id="595df-101">Erstellen von „deviceComplianceDeviceStatus“</span><span class="sxs-lookup"><span data-stu-id="595df-101">Create deviceComplianceDeviceStatus</span></span>

> <span data-ttu-id="595df-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="595df-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="595df-103">Diese Methode erstellt ein neues Objekt des Typs [deviceComplianceDeviceStatus](../resources/intune_deviceconfig_devicecompliancedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="595df-103">Create a new [deviceComplianceDeviceStatus](../resources/intune_deviceconfig_devicecompliancedevicestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="595df-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="595df-104">Prerequisites</span></span>
<span data-ttu-id="595df-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="595df-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="595df-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="595df-107">Permission type</span></span>|<span data-ttu-id="595df-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="595df-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="595df-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="595df-109">Delegated (work or school account)</span></span>|<span data-ttu-id="595df-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="595df-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="595df-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="595df-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="595df-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="595df-112">Not supported.</span></span>|
|<span data-ttu-id="595df-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="595df-113">Application</span></span>|<span data-ttu-id="595df-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="595df-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="595df-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="595df-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="595df-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="595df-116">Request headers</span></span>
|<span data-ttu-id="595df-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="595df-117">Header</span></span>|<span data-ttu-id="595df-118">Wert</span><span class="sxs-lookup"><span data-stu-id="595df-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="595df-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="595df-119">Authorization</span></span>|<span data-ttu-id="595df-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="595df-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="595df-121">Accept</span><span class="sxs-lookup"><span data-stu-id="595df-121">Accept</span></span>|<span data-ttu-id="595df-122">application/json</span><span class="sxs-lookup"><span data-stu-id="595df-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="595df-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="595df-123">Request body</span></span>
<span data-ttu-id="595df-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „deviceComplianceDeviceStatus“ an.</span><span class="sxs-lookup"><span data-stu-id="595df-124">In the request body, supply a JSON representation for the deviceComplianceDeviceStatus object.</span></span>

<span data-ttu-id="595df-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „deviceComplianceDeviceStatus“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="595df-125">The following table shows the properties that are required when you create the deviceComplianceDeviceStatus.</span></span>

|<span data-ttu-id="595df-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="595df-126">Property</span></span>|<span data-ttu-id="595df-127">Typ</span><span class="sxs-lookup"><span data-stu-id="595df-127">Type</span></span>|<span data-ttu-id="595df-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="595df-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="595df-129">id</span><span class="sxs-lookup"><span data-stu-id="595df-129">id</span></span>|<span data-ttu-id="595df-130">String</span><span class="sxs-lookup"><span data-stu-id="595df-130">String</span></span>|<span data-ttu-id="595df-131">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="595df-131">Key of the entity.</span></span>|
|<span data-ttu-id="595df-132">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="595df-132">deviceDisplayName</span></span>|<span data-ttu-id="595df-133">String</span><span class="sxs-lookup"><span data-stu-id="595df-133">String</span></span>|<span data-ttu-id="595df-134">Gerätename, der dem Objekt des Typs „DevicePolicyStatus“ zugeordnet ist</span><span class="sxs-lookup"><span data-stu-id="595df-134">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="595df-135">userName</span><span class="sxs-lookup"><span data-stu-id="595df-135">userName</span></span>|<span data-ttu-id="595df-136">String</span><span class="sxs-lookup"><span data-stu-id="595df-136">String</span></span>|<span data-ttu-id="595df-137">Gemeldeter Benutzername</span><span class="sxs-lookup"><span data-stu-id="595df-137">The User Name that is being reported</span></span>|
|<span data-ttu-id="595df-138">deviceModel</span><span class="sxs-lookup"><span data-stu-id="595df-138">deviceModel</span></span>|<span data-ttu-id="595df-139">String</span><span class="sxs-lookup"><span data-stu-id="595df-139">String</span></span>|<span data-ttu-id="595df-140">Gemeldetes Gerätemodell</span><span class="sxs-lookup"><span data-stu-id="595df-140">The device model that is being reported</span></span>|
|<span data-ttu-id="595df-141">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="595df-141">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="595df-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="595df-142">DateTimeOffset</span></span>|<span data-ttu-id="595df-143">Datum und Uhrzeit des Ablaufs der Toleranzperiode für die Gerätekonformität</span><span class="sxs-lookup"><span data-stu-id="595df-143">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="595df-144">status</span><span class="sxs-lookup"><span data-stu-id="595df-144">status</span></span>|[<span data-ttu-id="595df-145">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="595df-145">complianceStatus</span></span>](../resources/intune_shared_compliancestatus.md)|<span data-ttu-id="595df-146">Konformitätsstatus des Richtlinienberichts.</span><span class="sxs-lookup"><span data-stu-id="595df-146">Compliance status of the policy report.</span></span> <span data-ttu-id="595df-147">Mögliche Werte sind: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict` und `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="595df-147">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="595df-148">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="595df-148">lastReportedDateTime</span></span>|<span data-ttu-id="595df-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="595df-149">DateTimeOffset</span></span>|<span data-ttu-id="595df-150">Datum und Uhrzeit der letzten Änderung des Richtlinienberichts</span><span class="sxs-lookup"><span data-stu-id="595df-150">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="595df-151">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="595df-151">userPrincipalName</span></span>|<span data-ttu-id="595df-152">String</span><span class="sxs-lookup"><span data-stu-id="595df-152">String</span></span>|<span data-ttu-id="595df-153">Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="595df-153">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="595df-154">Antwort</span><span class="sxs-lookup"><span data-stu-id="595df-154">Response</span></span>
<span data-ttu-id="595df-155">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [deviceComplianceDeviceStatus](../resources/intune_deviceconfig_devicecompliancedevicestatus.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="595df-155">If successful, this method returns a `201 Created` response code and a [deviceComplianceDeviceStatus](../resources/intune_deviceconfig_devicecompliancedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="595df-156">Beispiel</span><span class="sxs-lookup"><span data-stu-id="595df-156">Example</span></span>
### <a name="request"></a><span data-ttu-id="595df-157">Anforderung</span><span class="sxs-lookup"><span data-stu-id="595df-157">Request</span></span>
<span data-ttu-id="595df-158">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="595df-158">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses
Content-type: application/json
Content-length: 426

{
  "@odata.type": "#microsoft.graph.deviceComplianceDeviceStatus",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="595df-159">Antwort</span><span class="sxs-lookup"><span data-stu-id="595df-159">Response</span></span>
<span data-ttu-id="595df-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="595df-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 475

{
  "@odata.type": "#microsoft.graph.deviceComplianceDeviceStatus",
  "id": "c6c78124-8124-c6c7-2481-c7c62481c7c6",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```



