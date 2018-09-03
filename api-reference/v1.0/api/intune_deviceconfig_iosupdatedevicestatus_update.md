# <a name="update-iosupdatedevicestatus"></a><span data-ttu-id="7cafb-101">iosUpdateDeviceStatus aktualisieren</span><span class="sxs-lookup"><span data-stu-id="7cafb-101">Update iosUpdateDeviceStatus</span></span>

> <span data-ttu-id="7cafb-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="7cafb-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7cafb-103">Aktualisieren der Eigenschaften eines [iosUpdateDeviceStatus](../resources/intune_deviceconfig_iosupdatedevicestatus.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="7cafb-103">Update the properties of a [iosUpdateDeviceStatus](../resources/intune_deviceconfig_iosupdatedevicestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7cafb-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="7cafb-104">Prerequisites</span></span>
<span data-ttu-id="7cafb-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="7cafb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="7cafb-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7cafb-107">Permission type</span></span>|<span data-ttu-id="7cafb-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7cafb-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7cafb-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7cafb-109">Delegated (work or school account)</span></span>|<span data-ttu-id="7cafb-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7cafb-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7cafb-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7cafb-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7cafb-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7cafb-112">Not supported.</span></span>|
|<span data-ttu-id="7cafb-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7cafb-113">Application</span></span>|<span data-ttu-id="7cafb-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7cafb-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7cafb-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7cafb-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/iosUpdateStatuses/{iosUpdateDeviceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="7cafb-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7cafb-116">Request headers</span></span>
|<span data-ttu-id="7cafb-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="7cafb-117">Header</span></span>|<span data-ttu-id="7cafb-118">Wert</span><span class="sxs-lookup"><span data-stu-id="7cafb-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7cafb-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="7cafb-119">Authorization</span></span>|<span data-ttu-id="7cafb-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="7cafb-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7cafb-121">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="7cafb-121">Accept</span></span>|<span data-ttu-id="7cafb-122">Anwendung/json</span><span class="sxs-lookup"><span data-stu-id="7cafb-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7cafb-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7cafb-123">Request body</span></span>
<span data-ttu-id="7cafb-124">Geben Sie im Anforderungstext eine JSON Darstellung für das Objekt des Typs [iosUpdateDeviceStatus](../resources/intune_deviceconfig_iosupdatedevicestatus.md) an.</span><span class="sxs-lookup"><span data-stu-id="7cafb-124">In the request body, supply a JSON representation for the [iosUpdateDeviceStatus](../resources/intune_deviceconfig_iosupdatedevicestatus.md) object.</span></span>

<span data-ttu-id="7cafb-125">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen des [iosUpdateDeviceStatus](../resources/intune_deviceconfig_iosupdatedevicestatus.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="7cafb-125">The following table shows the properties that are required when you create the [iosUpdateDeviceStatus](../resources/intune_deviceconfig_iosupdatedevicestatus.md).</span></span>

|<span data-ttu-id="7cafb-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7cafb-126">Property</span></span>|<span data-ttu-id="7cafb-127">Typ</span><span class="sxs-lookup"><span data-stu-id="7cafb-127">Type</span></span>|<span data-ttu-id="7cafb-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7cafb-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7cafb-129">id</span><span class="sxs-lookup"><span data-stu-id="7cafb-129">id</span></span>|<span data-ttu-id="7cafb-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7cafb-130">String</span></span>|<span data-ttu-id="7cafb-131">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="7cafb-131">Key of the entity.</span></span>|
|<span data-ttu-id="7cafb-132">installStatus</span><span class="sxs-lookup"><span data-stu-id="7cafb-132">installStatus</span></span>|[<span data-ttu-id="7cafb-133">iosUpdatesInstallStatus</span><span class="sxs-lookup"><span data-stu-id="7cafb-133">iosUpdatesInstallStatus</span></span>](../resources/intune_deviceconfig_iosupdatesinstallstatus.md)|<span data-ttu-id="7cafb-134">Installationsstatus des Richtlinienberichts.</span><span class="sxs-lookup"><span data-stu-id="7cafb-134">The installation status of the policy report.</span></span> <span data-ttu-id="7cafb-135">Die möglichen Werte sind: `success`, `available`, `idle`, `unknown`, `downloading`, `downloadFailed`, `downloadRequiresComputer`, `downloadInsufficientSpace`, `downloadInsufficientPower`, `downloadInsufficientNetwork`, `installing`, `installInsufficientSpace`, `installInsufficientPower`, `installPhoneCallInProgress`, `installFailed`, `notSupportedOperation`, `sharedDeviceUserLoggedInError`.</span><span class="sxs-lookup"><span data-stu-id="7cafb-135">The possible values are: `success`, `available`, `idle`, `unknown`, `downloading`, `downloadFailed`, `downloadRequiresComputer`, `downloadInsufficientSpace`, `downloadInsufficientPower`, `downloadInsufficientNetwork`, `installing`, `installInsufficientSpace`, `installInsufficientPower`, `installPhoneCallInProgress`, `installFailed`, `notSupportedOperation`, `sharedDeviceUserLoggedInError`.</span></span>|
|<span data-ttu-id="7cafb-136">osVersion</span><span class="sxs-lookup"><span data-stu-id="7cafb-136">osVersion</span></span>|<span data-ttu-id="7cafb-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7cafb-137">String</span></span>|<span data-ttu-id="7cafb-138">Gemeldete Geräteversion</span><span class="sxs-lookup"><span data-stu-id="7cafb-138">The device version that is being reported.</span></span>|
|<span data-ttu-id="7cafb-139">deviceId</span><span class="sxs-lookup"><span data-stu-id="7cafb-139">deviceId</span></span>|<span data-ttu-id="7cafb-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7cafb-140">String</span></span>|<span data-ttu-id="7cafb-141">Gemeldete Geräte-ID</span><span class="sxs-lookup"><span data-stu-id="7cafb-141">The device id that is being reported.</span></span>|
|<span data-ttu-id="7cafb-142">userId</span><span class="sxs-lookup"><span data-stu-id="7cafb-142">userId</span></span>|<span data-ttu-id="7cafb-143">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7cafb-143">String</span></span>|<span data-ttu-id="7cafb-144">Gemeldete Benutzer-ID</span><span class="sxs-lookup"><span data-stu-id="7cafb-144">The User id that is being reported.</span></span>|
|<span data-ttu-id="7cafb-145">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="7cafb-145">deviceDisplayName</span></span>|<span data-ttu-id="7cafb-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7cafb-146">String</span></span>|<span data-ttu-id="7cafb-147">Gerätename, der dem Objekt des Typs „DevicePolicyStatus“ zugeordnet ist</span><span class="sxs-lookup"><span data-stu-id="7cafb-147">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="7cafb-148">userName</span><span class="sxs-lookup"><span data-stu-id="7cafb-148">userName</span></span>|<span data-ttu-id="7cafb-149">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7cafb-149">String</span></span>|<span data-ttu-id="7cafb-150">Gemeldeter Benutzername</span><span class="sxs-lookup"><span data-stu-id="7cafb-150">The User Name that is being reported</span></span>|
|<span data-ttu-id="7cafb-151">deviceModel</span><span class="sxs-lookup"><span data-stu-id="7cafb-151">deviceModel</span></span>|<span data-ttu-id="7cafb-152">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7cafb-152">String</span></span>|<span data-ttu-id="7cafb-153">Gemeldetes Gerätemodell</span><span class="sxs-lookup"><span data-stu-id="7cafb-153">The device model that is being reported</span></span>|
|<span data-ttu-id="7cafb-154">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="7cafb-154">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="7cafb-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7cafb-155">DateTimeOffset</span></span>|<span data-ttu-id="7cafb-156">Datum und Uhrzeit des Ablaufs der Toleranzperiode für die Gerätekonformität</span><span class="sxs-lookup"><span data-stu-id="7cafb-156">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="7cafb-157">Status</span><span class="sxs-lookup"><span data-stu-id="7cafb-157">status</span></span>|[<span data-ttu-id="7cafb-158">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="7cafb-158">complianceStatus</span></span>](../resources/intune_shared_compliancestatus.md)|<span data-ttu-id="7cafb-159">Konformitätsstatus des Richtlinienberichts.</span><span class="sxs-lookup"><span data-stu-id="7cafb-159">Compliance status of the policy report.</span></span> <span data-ttu-id="7cafb-160">Die möglichen Werte sind: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`.</span><span class="sxs-lookup"><span data-stu-id="7cafb-160">The possible values are `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, , , , , or .</span></span>|
|<span data-ttu-id="7cafb-161">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="7cafb-161">lastReportedDateTime</span></span>|<span data-ttu-id="7cafb-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7cafb-162">DateTimeOffset</span></span>|<span data-ttu-id="7cafb-163">Datum und Uhrzeit der letzten Änderung des Richtlinienberichts</span><span class="sxs-lookup"><span data-stu-id="7cafb-163">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="7cafb-164">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="7cafb-164">userPrincipalName</span></span>|<span data-ttu-id="7cafb-165">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7cafb-165">String</span></span>|<span data-ttu-id="7cafb-166">Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="7cafb-166">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="7cafb-167">Antwort</span><span class="sxs-lookup"><span data-stu-id="7cafb-167">Response</span></span>
<span data-ttu-id="7cafb-168">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [iosUpdateDeviceStatus](../resources/intune_deviceconfig_iosupdatedevicestatus.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="7cafb-168">If successful, this method returns a `200 OK` response code and an updated [iosUpdateDeviceStatus](../resources/intune_deviceconfig_iosupdatedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7cafb-169">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7cafb-169">Example</span></span>
### <a name="request"></a><span data-ttu-id="7cafb-170">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7cafb-170">Request</span></span>
<span data-ttu-id="7cafb-171">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7cafb-171">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/iosUpdateStatuses/{iosUpdateDeviceStatusId}
Content-type: application/json
Content-length: 492

{
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

### <a name="response"></a><span data-ttu-id="7cafb-172">Antwort</span><span class="sxs-lookup"><span data-stu-id="7cafb-172">Response</span></span>
<span data-ttu-id="7cafb-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7cafb-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



