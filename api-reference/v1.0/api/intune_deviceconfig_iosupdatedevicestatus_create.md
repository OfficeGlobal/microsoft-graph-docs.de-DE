# <a name="create-iosupdatedevicestatus"></a><span data-ttu-id="23a43-101">Erstellen von „iosUpdateDeviceStatus“</span><span class="sxs-lookup"><span data-stu-id="23a43-101">Create iosUpdateDeviceStatus</span></span>

> <span data-ttu-id="23a43-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="23a43-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="23a43-103">Diese Methode erstellt ein neues Objekt des Typs [iosUpdateDeviceStatus](../resources/intune_deviceconfig_iosupdatedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="23a43-103">Create a new [iosUpdateDeviceStatus](../resources/intune_deviceconfig_iosupdatedevicestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="23a43-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="23a43-104">Prerequisites</span></span>
<span data-ttu-id="23a43-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="23a43-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="23a43-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="23a43-107">Permission type</span></span>|<span data-ttu-id="23a43-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="23a43-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="23a43-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="23a43-109">Delegated (work or school account)</span></span>|<span data-ttu-id="23a43-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="23a43-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="23a43-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="23a43-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="23a43-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="23a43-112">Not supported.</span></span>|
|<span data-ttu-id="23a43-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="23a43-113">Application</span></span>|<span data-ttu-id="23a43-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="23a43-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="23a43-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="23a43-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/iosUpdateStatuses
```

## <a name="request-headers"></a><span data-ttu-id="23a43-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="23a43-116">Request headers</span></span>
|<span data-ttu-id="23a43-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="23a43-117">Header</span></span>|<span data-ttu-id="23a43-118">Wert</span><span class="sxs-lookup"><span data-stu-id="23a43-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="23a43-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="23a43-119">Authorization</span></span>|<span data-ttu-id="23a43-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="23a43-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="23a43-121">Accept</span><span class="sxs-lookup"><span data-stu-id="23a43-121">Accept</span></span>|<span data-ttu-id="23a43-122">application/json</span><span class="sxs-lookup"><span data-stu-id="23a43-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="23a43-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="23a43-123">Request body</span></span>
<span data-ttu-id="23a43-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „iosUpdateDeviceStatus“ an.</span><span class="sxs-lookup"><span data-stu-id="23a43-124">In the request body, supply a JSON representation for the iosUpdateDeviceStatus object.</span></span>

<span data-ttu-id="23a43-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „iosUpdateDeviceStatus“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="23a43-125">The following table shows the properties that are required when you create the iosUpdateDeviceStatus.</span></span>

|<span data-ttu-id="23a43-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="23a43-126">Property</span></span>|<span data-ttu-id="23a43-127">Typ</span><span class="sxs-lookup"><span data-stu-id="23a43-127">Type</span></span>|<span data-ttu-id="23a43-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="23a43-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23a43-129">id</span><span class="sxs-lookup"><span data-stu-id="23a43-129">id</span></span>|<span data-ttu-id="23a43-130">String</span><span class="sxs-lookup"><span data-stu-id="23a43-130">String</span></span>|<span data-ttu-id="23a43-131">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="23a43-131">Key of the entity.</span></span>|
|<span data-ttu-id="23a43-132">installStatus</span><span class="sxs-lookup"><span data-stu-id="23a43-132">installStatus</span></span>|[<span data-ttu-id="23a43-133">iosUpdatesInstallStatus</span><span class="sxs-lookup"><span data-stu-id="23a43-133">iosUpdatesInstallStatus</span></span>](../resources/intune_deviceconfig_iosupdatesinstallstatus.md)|<span data-ttu-id="23a43-134">Installationsstatus des Richtlinienberichts.</span><span class="sxs-lookup"><span data-stu-id="23a43-134">The installation status of the policy report.</span></span> <span data-ttu-id="23a43-135">Mögliche Werte sind: `success`, `available`, `idle`, `unknown`, `downloading`, `downloadFailed`, `downloadRequiresComputer`, `downloadInsufficientSpace`, `downloadInsufficientPower`, `downloadInsufficientNetwork`, `installing`, `installInsufficientSpace`, `installInsufficientPower`, `installPhoneCallInProgress`, `installFailed`, `notSupportedOperation`, `sharedDeviceUserLoggedInError`.</span><span class="sxs-lookup"><span data-stu-id="23a43-135">Possible values are: `success`, `available`, `idle`, `unknown`, `downloading`, `downloadFailed`, `downloadRequiresComputer`, `downloadInsufficientSpace`, `downloadInsufficientPower`, `downloadInsufficientNetwork`, `installing`, `installInsufficientSpace`, `installInsufficientPower`, `installPhoneCallInProgress`, `installFailed`, `notSupportedOperation`, `sharedDeviceUserLoggedInError`.</span></span>|
|<span data-ttu-id="23a43-136">osVersion</span><span class="sxs-lookup"><span data-stu-id="23a43-136">osVersion</span></span>|<span data-ttu-id="23a43-137">String</span><span class="sxs-lookup"><span data-stu-id="23a43-137">String</span></span>|<span data-ttu-id="23a43-138">Gemeldete Geräteversion</span><span class="sxs-lookup"><span data-stu-id="23a43-138">The device version that is being reported.</span></span>|
|<span data-ttu-id="23a43-139">deviceId</span><span class="sxs-lookup"><span data-stu-id="23a43-139">deviceId</span></span>|<span data-ttu-id="23a43-140">String</span><span class="sxs-lookup"><span data-stu-id="23a43-140">String</span></span>|<span data-ttu-id="23a43-141">Gemeldete Geräte-ID</span><span class="sxs-lookup"><span data-stu-id="23a43-141">The device id that is being reported.</span></span>|
|<span data-ttu-id="23a43-142">userId</span><span class="sxs-lookup"><span data-stu-id="23a43-142">userId</span></span>|<span data-ttu-id="23a43-143">String</span><span class="sxs-lookup"><span data-stu-id="23a43-143">String</span></span>|<span data-ttu-id="23a43-144">Gemeldete Benutzer-ID</span><span class="sxs-lookup"><span data-stu-id="23a43-144">The User id that is being reported.</span></span>|
|<span data-ttu-id="23a43-145">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="23a43-145">deviceDisplayName</span></span>|<span data-ttu-id="23a43-146">String</span><span class="sxs-lookup"><span data-stu-id="23a43-146">String</span></span>|<span data-ttu-id="23a43-147">Gerätename, der dem Objekt des Typs „DevicePolicyStatus“ zugeordnet ist</span><span class="sxs-lookup"><span data-stu-id="23a43-147">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="23a43-148">userName</span><span class="sxs-lookup"><span data-stu-id="23a43-148">userName</span></span>|<span data-ttu-id="23a43-149">String</span><span class="sxs-lookup"><span data-stu-id="23a43-149">String</span></span>|<span data-ttu-id="23a43-150">Gemeldeter Benutzername</span><span class="sxs-lookup"><span data-stu-id="23a43-150">The User Name that is being reported</span></span>|
|<span data-ttu-id="23a43-151">deviceModel</span><span class="sxs-lookup"><span data-stu-id="23a43-151">deviceModel</span></span>|<span data-ttu-id="23a43-152">String</span><span class="sxs-lookup"><span data-stu-id="23a43-152">String</span></span>|<span data-ttu-id="23a43-153">Gemeldetes Gerätemodell</span><span class="sxs-lookup"><span data-stu-id="23a43-153">The device model that is being reported</span></span>|
|<span data-ttu-id="23a43-154">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="23a43-154">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="23a43-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="23a43-155">DateTimeOffset</span></span>|<span data-ttu-id="23a43-156">Datum und Uhrzeit des Ablaufs der Toleranzperiode für die Gerätekonformität</span><span class="sxs-lookup"><span data-stu-id="23a43-156">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="23a43-157">status</span><span class="sxs-lookup"><span data-stu-id="23a43-157">status</span></span>|[<span data-ttu-id="23a43-158">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="23a43-158">complianceStatus</span></span>](../resources/intune_shared_compliancestatus.md)|<span data-ttu-id="23a43-159">Konformitätsstatus des Richtlinienberichts.</span><span class="sxs-lookup"><span data-stu-id="23a43-159">Compliance status of the policy report.</span></span> <span data-ttu-id="23a43-160">Mögliche Werte sind: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict` und `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="23a43-160">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="23a43-161">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="23a43-161">lastReportedDateTime</span></span>|<span data-ttu-id="23a43-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="23a43-162">DateTimeOffset</span></span>|<span data-ttu-id="23a43-163">Datum und Uhrzeit der letzten Änderung des Richtlinienberichts</span><span class="sxs-lookup"><span data-stu-id="23a43-163">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="23a43-164">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="23a43-164">userPrincipalName</span></span>|<span data-ttu-id="23a43-165">String</span><span class="sxs-lookup"><span data-stu-id="23a43-165">String</span></span>|<span data-ttu-id="23a43-166">Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="23a43-166">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="23a43-167">Antwort</span><span class="sxs-lookup"><span data-stu-id="23a43-167">Response</span></span>
<span data-ttu-id="23a43-168">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [iosUpdateDeviceStatus](../resources/intune_deviceconfig_iosupdatedevicestatus.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="23a43-168">If successful, this method returns a `201 Created` response code and a [iosUpdateDeviceStatus](../resources/intune_deviceconfig_iosupdatedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="23a43-169">Beispiel</span><span class="sxs-lookup"><span data-stu-id="23a43-169">Example</span></span>
### <a name="request"></a><span data-ttu-id="23a43-170">Anforderung</span><span class="sxs-lookup"><span data-stu-id="23a43-170">Request</span></span>
<span data-ttu-id="23a43-171">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="23a43-171">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/iosUpdateStatuses
Content-type: application/json
Content-length: 552

{
  "@odata.type": "#microsoft.graph.iosUpdateDeviceStatus",
  "installStatus": "available",
  "osVersion": "Os Version value",
  "deviceId": "Device Id value",
  "userId": "User Id value",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="23a43-172">Antwort</span><span class="sxs-lookup"><span data-stu-id="23a43-172">Response</span></span>
<span data-ttu-id="23a43-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="23a43-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 601

{
  "@odata.type": "#microsoft.graph.iosUpdateDeviceStatus",
  "id": "63a79499-9499-63a7-9994-a7639994a763",
  "installStatus": "available",
  "osVersion": "Os Version value",
  "deviceId": "Device Id value",
  "userId": "User Id value",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```



