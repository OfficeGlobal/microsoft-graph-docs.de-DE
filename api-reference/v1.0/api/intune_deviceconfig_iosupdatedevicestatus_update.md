# <a name="update-iosupdatedevicestatus"></a><span data-ttu-id="4137b-101">iosUpdateDeviceStatus aktualisieren</span><span class="sxs-lookup"><span data-stu-id="4137b-101">Update iosUpdateDeviceStatus</span></span>

> <span data-ttu-id="4137b-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="4137b-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4137b-103">Aktualisieren der Eigenschaften eines [iosUpdateDeviceStatus](../resources/intune_deviceconfig_iosupdatedevicestatus.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="4137b-103">Update the properties of a [calendar](../resources/intune_deviceconfig_iosupdatedevicestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4137b-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="4137b-104">Prerequisites</span></span>
<span data-ttu-id="4137b-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="4137b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="4137b-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4137b-107">Permission type</span></span>|<span data-ttu-id="4137b-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4137b-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4137b-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4137b-109">Delegated (work or school account)</span></span>|<span data-ttu-id="4137b-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4137b-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4137b-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4137b-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4137b-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4137b-112">Not supported.</span></span>|
|<span data-ttu-id="4137b-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4137b-113">Application</span></span>|<span data-ttu-id="4137b-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4137b-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4137b-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4137b-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/iosUpdateStatuses/{iosUpdateDeviceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="4137b-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4137b-116">Request headers</span></span>
|<span data-ttu-id="4137b-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="4137b-117">Header</span></span>|<span data-ttu-id="4137b-118">Wert</span><span class="sxs-lookup"><span data-stu-id="4137b-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4137b-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="4137b-119">Authorization</span></span>|<span data-ttu-id="4137b-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="4137b-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="4137b-121">Annehmen</span><span class="sxs-lookup"><span data-stu-id="4137b-121">Accept</span></span>|<span data-ttu-id="4137b-122">application/json</span><span class="sxs-lookup"><span data-stu-id="4137b-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4137b-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4137b-123">Request body</span></span>
<span data-ttu-id="4137b-124">Geben Sie im Anforderungstext eine JSON Darstellung für das Objekt des Typs [iosUpdateDeviceStatus](../resources/intune_deviceconfig_iosupdatedevicestatus.md) an.</span><span class="sxs-lookup"><span data-stu-id="4137b-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_deviceconfig_iosupdatedevicestatus.md) object.</span></span>

<span data-ttu-id="4137b-125">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen des [iosUpdateDeviceStatus](../resources/intune_deviceconfig_iosupdatedevicestatus.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="4137b-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="4137b-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4137b-126">Property</span></span>|<span data-ttu-id="4137b-127">Typ</span><span class="sxs-lookup"><span data-stu-id="4137b-127">Type</span></span>|<span data-ttu-id="4137b-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4137b-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4137b-129">id</span><span class="sxs-lookup"><span data-stu-id="4137b-129">id</span></span>|<span data-ttu-id="4137b-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4137b-130">String</span></span>|<span data-ttu-id="4137b-131">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="4137b-131">Key of the setting.</span></span>|
|<span data-ttu-id="4137b-132">installStatus</span><span class="sxs-lookup"><span data-stu-id="4137b-132">installStatus</span></span>|<span data-ttu-id="4137b-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4137b-133">String</span></span>|<span data-ttu-id="4137b-134">Installationsstatus des Richtlinienberichts</span><span class="sxs-lookup"><span data-stu-id="4137b-134">The installation status of the policy report.</span></span> <span data-ttu-id="4137b-135">Mögliche Werte: `success`, `available`, `idle`, `downloading`, `downloadFailed`, `downloadRequiresComputer`, `downloadInsufficientSpace`, `downloadInsufficientPower`, `downloadInsufficientNetwork`, `installing`, `installInsufficientSpace`, `installInsufficientPower`, `installPhoneCallInProgress`, `installFailed`, `notSupportedOperation`, `sharedDeviceUserLoggedInError`.</span><span class="sxs-lookup"><span data-stu-id="4137b-135">Possible values are: `success`, `available`, `idle`, `downloading`, `downloadFailed`, `downloadRequiresComputer`, `downloadInsufficientSpace`, `downloadInsufficientPower`, `downloadInsufficientNetwork`, `installing`, `installInsufficientSpace`, `installInsufficientPower`, `installPhoneCallInProgress`, `installFailed`, `notSupportedOperation`, `sharedDeviceUserLoggedInError`.</span></span>|
|<span data-ttu-id="4137b-136">osVersion</span><span class="sxs-lookup"><span data-stu-id="4137b-136">osVersion</span></span>|<span data-ttu-id="4137b-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4137b-137">String</span></span>|<span data-ttu-id="4137b-138">Gemeldete Geräteversion</span><span class="sxs-lookup"><span data-stu-id="4137b-138">The device version that is being reported.</span></span>|
|<span data-ttu-id="4137b-139">deviceId</span><span class="sxs-lookup"><span data-stu-id="4137b-139">deviceId</span></span>|<span data-ttu-id="4137b-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4137b-140">String</span></span>|<span data-ttu-id="4137b-141">Gemeldete Geräte-ID</span><span class="sxs-lookup"><span data-stu-id="4137b-141">The device id that is being reported.</span></span>|
|<span data-ttu-id="4137b-142">userId</span><span class="sxs-lookup"><span data-stu-id="4137b-142">userID</span></span>|<span data-ttu-id="4137b-143">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4137b-143">String</span></span>|<span data-ttu-id="4137b-144">Gemeldete Benutzer-ID</span><span class="sxs-lookup"><span data-stu-id="4137b-144">The User id that is being reported.</span></span>|
|<span data-ttu-id="4137b-145">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="4137b-145">deviceDisplayName</span></span>|<span data-ttu-id="4137b-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4137b-146">String</span></span>|<span data-ttu-id="4137b-147">Gerätename des DevicePolicyStatus</span><span class="sxs-lookup"><span data-stu-id="4137b-147">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="4137b-148">userName</span><span class="sxs-lookup"><span data-stu-id="4137b-148">UserName</span></span>|<span data-ttu-id="4137b-149">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4137b-149">String</span></span>|<span data-ttu-id="4137b-150">Gemeldeter Benutzername</span><span class="sxs-lookup"><span data-stu-id="4137b-150">The User Name that is being reported</span></span>|
|<span data-ttu-id="4137b-151">deviceModel</span><span class="sxs-lookup"><span data-stu-id="4137b-151">deviceModel</span></span>|<span data-ttu-id="4137b-152">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4137b-152">String</span></span>|<span data-ttu-id="4137b-153">Gemeldetes Gerätemodell</span><span class="sxs-lookup"><span data-stu-id="4137b-153">The device model that is being reported</span></span>|
|<span data-ttu-id="4137b-154">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="4137b-154">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="4137b-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4137b-155">DateTimeOffset</span></span>|<span data-ttu-id="4137b-156">Datum und Uhrzeit des Ablaufs der Karenzzeit für die Gerätekonformität</span><span class="sxs-lookup"><span data-stu-id="4137b-156">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="4137b-157">status</span><span class="sxs-lookup"><span data-stu-id="4137b-157">status</span></span>|<span data-ttu-id="4137b-158">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4137b-158">String</span></span>|<span data-ttu-id="4137b-159">Compliance-Status des Richtlinienberichts</span><span class="sxs-lookup"><span data-stu-id="4137b-159">Compliance status of the policy report.</span></span> <span data-ttu-id="4137b-160">Mögliche Werte: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`.</span><span class="sxs-lookup"><span data-stu-id="4137b-160">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`.</span></span>|
|<span data-ttu-id="4137b-161">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="4137b-161">lastReportedDateTime</span></span>|<span data-ttu-id="4137b-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4137b-162">DateTimeOffset</span></span>|<span data-ttu-id="4137b-163">Datum und Uhrzeit der letzten Änderung des Richtlinienberichts</span><span class="sxs-lookup"><span data-stu-id="4137b-163">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="4137b-164">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="4137b-164">userPrincipalName</span></span>|<span data-ttu-id="4137b-165">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4137b-165">String</span></span>|<span data-ttu-id="4137b-166">Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="4137b-166">userPrincipalName</span></span>|



## <a name="response"></a><span data-ttu-id="4137b-167">Antwort</span><span class="sxs-lookup"><span data-stu-id="4137b-167">Response</span></span>
<span data-ttu-id="4137b-168">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [iosUpdateDeviceStatus](../resources/intune_deviceconfig_iosupdatedevicestatus.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="4137b-168">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_deviceconfig_iosupdatedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4137b-169">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4137b-169">Example</span></span>
### <a name="request"></a><span data-ttu-id="4137b-170">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4137b-170">Request</span></span>
<span data-ttu-id="4137b-171">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4137b-171">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4137b-172">Antwort</span><span class="sxs-lookup"><span data-stu-id="4137b-172">Response</span></span>
<span data-ttu-id="4137b-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4137b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



