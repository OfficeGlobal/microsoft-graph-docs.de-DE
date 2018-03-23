# <a name="create-iosupdatedevicestatus"></a><span data-ttu-id="ee004-101">Erstellen von „iosUpdateDeviceStatus“</span><span class="sxs-lookup"><span data-stu-id="ee004-101">Create iosUpdateDeviceStatus</span></span>

> <span data-ttu-id="ee004-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="ee004-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ee004-103">Diese Methode erstellt ein neues Objekt des Typs [iosUpdateDeviceStatus](../resources/intune_deviceconfig_iosupdatedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="ee004-103">Create a new [plannerBucket](../resources/intune_deviceconfig_iosupdatedevicestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ee004-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="ee004-104">Prerequisites</span></span>
<span data-ttu-id="ee004-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="ee004-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ee004-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ee004-107">Permission type</span></span>|<span data-ttu-id="ee004-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ee004-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ee004-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ee004-109">Delegated (work or school account)</span></span>|<span data-ttu-id="ee004-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee004-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ee004-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ee004-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ee004-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ee004-112">Not supported.</span></span>|
|<span data-ttu-id="ee004-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ee004-113">Application</span></span>|<span data-ttu-id="ee004-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ee004-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ee004-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ee004-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/iosUpdateStatuses
```

## <a name="request-headers"></a><span data-ttu-id="ee004-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ee004-116">Request headers</span></span>
|<span data-ttu-id="ee004-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="ee004-117">Header</span></span>|<span data-ttu-id="ee004-118">Wert</span><span class="sxs-lookup"><span data-stu-id="ee004-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ee004-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="ee004-119">Authorization</span></span>|<span data-ttu-id="ee004-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="ee004-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="ee004-121">Accept</span><span class="sxs-lookup"><span data-stu-id="ee004-121">Accept</span></span>|<span data-ttu-id="ee004-122">application/json</span><span class="sxs-lookup"><span data-stu-id="ee004-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ee004-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ee004-123">Request body</span></span>
<span data-ttu-id="ee004-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „iosUpdateDeviceStatus“ an.</span><span class="sxs-lookup"><span data-stu-id="ee004-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="ee004-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „iosUpdateDeviceStatus“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="ee004-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="ee004-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ee004-126">Property</span></span>|<span data-ttu-id="ee004-127">Typ</span><span class="sxs-lookup"><span data-stu-id="ee004-127">Type</span></span>|<span data-ttu-id="ee004-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ee004-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ee004-129">id</span><span class="sxs-lookup"><span data-stu-id="ee004-129">id</span></span>|<span data-ttu-id="ee004-130">String</span><span class="sxs-lookup"><span data-stu-id="ee004-130">String</span></span>|<span data-ttu-id="ee004-131">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="ee004-131">Key of the setting.</span></span>|
|<span data-ttu-id="ee004-132">installStatus</span><span class="sxs-lookup"><span data-stu-id="ee004-132">installStatus</span></span>|<span data-ttu-id="ee004-133">String</span><span class="sxs-lookup"><span data-stu-id="ee004-133">String</span></span>|<span data-ttu-id="ee004-134">Installationsstatus des Richtlinienberichts.</span><span class="sxs-lookup"><span data-stu-id="ee004-134">The installation status of the policy report.</span></span> <span data-ttu-id="ee004-135">Mögliche Werte sind: `success`, `available`, `idle`, `downloading`, `downloadFailed`, `downloadRequiresComputer`, `downloadInsufficientSpace`, `downloadInsufficientPower`, `downloadInsufficientNetwork`, `installing`, `installInsufficientSpace`, `installInsufficientPower`, `installPhoneCallInProgress`, `installFailed`, `notSupportedOperation` und `sharedDeviceUserLoggedInError`.</span><span class="sxs-lookup"><span data-stu-id="ee004-135">Possible values are: `success`, `available`, `idle`, `downloading`, `downloadFailed`, `downloadRequiresComputer`, `downloadInsufficientSpace`, `downloadInsufficientPower`, `downloadInsufficientNetwork`, `installing`, `installInsufficientSpace`, `installInsufficientPower`, `installPhoneCallInProgress`, `installFailed`, `notSupportedOperation`, `sharedDeviceUserLoggedInError`.</span></span>|
|<span data-ttu-id="ee004-136">osVersion</span><span class="sxs-lookup"><span data-stu-id="ee004-136">osVersion</span></span>|<span data-ttu-id="ee004-137">String</span><span class="sxs-lookup"><span data-stu-id="ee004-137">String</span></span>|<span data-ttu-id="ee004-138">Gemeldete Geräteversion</span><span class="sxs-lookup"><span data-stu-id="ee004-138">The device version that is being reported.</span></span>|
|<span data-ttu-id="ee004-139">deviceId</span><span class="sxs-lookup"><span data-stu-id="ee004-139">deviceId</span></span>|<span data-ttu-id="ee004-140">String</span><span class="sxs-lookup"><span data-stu-id="ee004-140">String</span></span>|<span data-ttu-id="ee004-141">Gemeldete Geräte-ID</span><span class="sxs-lookup"><span data-stu-id="ee004-141">The device id that is being reported.</span></span>|
|<span data-ttu-id="ee004-142">userId</span><span class="sxs-lookup"><span data-stu-id="ee004-142">userID</span></span>|<span data-ttu-id="ee004-143">String</span><span class="sxs-lookup"><span data-stu-id="ee004-143">String</span></span>|<span data-ttu-id="ee004-144">Gemeldete Benutzer-ID</span><span class="sxs-lookup"><span data-stu-id="ee004-144">The User id that is being reported.</span></span>|
|<span data-ttu-id="ee004-145">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="ee004-145">deviceDisplayName</span></span>|<span data-ttu-id="ee004-146">String</span><span class="sxs-lookup"><span data-stu-id="ee004-146">String</span></span>|<span data-ttu-id="ee004-147">Gerätename, der dem Objekt des Typs „DevicePolicyStatus“ zugeordnet ist</span><span class="sxs-lookup"><span data-stu-id="ee004-147">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="ee004-148">userName</span><span class="sxs-lookup"><span data-stu-id="ee004-148">UserName</span></span>|<span data-ttu-id="ee004-149">String</span><span class="sxs-lookup"><span data-stu-id="ee004-149">String</span></span>|<span data-ttu-id="ee004-150">Gemeldeter Benutzername</span><span class="sxs-lookup"><span data-stu-id="ee004-150">The User Name that is being reported</span></span>|
|<span data-ttu-id="ee004-151">deviceModel</span><span class="sxs-lookup"><span data-stu-id="ee004-151">deviceModel</span></span>|<span data-ttu-id="ee004-152">String</span><span class="sxs-lookup"><span data-stu-id="ee004-152">String</span></span>|<span data-ttu-id="ee004-153">Gemeldetes Gerätemodell</span><span class="sxs-lookup"><span data-stu-id="ee004-153">The device model that is being reported</span></span>|
|<span data-ttu-id="ee004-154">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="ee004-154">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="ee004-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ee004-155">DateTimeOffset</span></span>|<span data-ttu-id="ee004-156">Datum und Uhrzeit des Ablaufs der Toleranzperiode für die Gerätekonformität</span><span class="sxs-lookup"><span data-stu-id="ee004-156">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="ee004-157">status</span><span class="sxs-lookup"><span data-stu-id="ee004-157">status</span></span>|<span data-ttu-id="ee004-158">String</span><span class="sxs-lookup"><span data-stu-id="ee004-158">String</span></span>|<span data-ttu-id="ee004-159">Konformitätsstatus des Richtlinienberichts.</span><span class="sxs-lookup"><span data-stu-id="ee004-159">Compliance status of the policy report.</span></span> <span data-ttu-id="ee004-160">Mögliche Werte sind: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error` und `conflict`.</span><span class="sxs-lookup"><span data-stu-id="ee004-160">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`.</span></span>|
|<span data-ttu-id="ee004-161">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="ee004-161">lastReportedDateTime</span></span>|<span data-ttu-id="ee004-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ee004-162">DateTimeOffset</span></span>|<span data-ttu-id="ee004-163">Datum und Uhrzeit der letzten Änderung des Richtlinienberichts</span><span class="sxs-lookup"><span data-stu-id="ee004-163">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="ee004-164">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ee004-164">userPrincipalName</span></span>|<span data-ttu-id="ee004-165">String</span><span class="sxs-lookup"><span data-stu-id="ee004-165">String</span></span>|<span data-ttu-id="ee004-166">Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="ee004-166">userPrincipalName</span></span>|



## <a name="response"></a><span data-ttu-id="ee004-167">Antwort</span><span class="sxs-lookup"><span data-stu-id="ee004-167">Response</span></span>
<span data-ttu-id="ee004-168">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [iosUpdateDeviceStatus](../resources/intune_deviceconfig_iosupdatedevicestatus.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="ee004-168">If successful, this method returns a `201 Created` response code and a [section](../resources/intune_deviceconfig_iosupdatedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ee004-169">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ee004-169">Example</span></span>
### <a name="request"></a><span data-ttu-id="ee004-170">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ee004-170">Request</span></span>
<span data-ttu-id="ee004-171">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ee004-171">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ee004-172">Antwort</span><span class="sxs-lookup"><span data-stu-id="ee004-172">Response</span></span>
<span data-ttu-id="ee004-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ee004-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



