# <a name="create-manageddevicemobileappconfigurationdevicestatus"></a><span data-ttu-id="43bed-101">Erstellen von managedDeviceMobileAppConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="43bed-101">Create managedDeviceMobileAppConfigurationDeviceStatus</span></span>

> <span data-ttu-id="43bed-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="43bed-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="43bed-103">Erstellen eines neuen [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune_apps_manageddevicemobileappconfigurationdevicestatus.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="43bed-103">Create a new [deviceConfigurationAssignment](../resources/intune_apps_manageddevicemobileappconfigurationdevicestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="43bed-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="43bed-104">Prerequisites</span></span>
<span data-ttu-id="43bed-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="43bed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="43bed-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="43bed-107">Permission type</span></span>|<span data-ttu-id="43bed-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="43bed-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="43bed-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="43bed-109">Delegated (work or school account)</span></span>|<span data-ttu-id="43bed-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="43bed-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="43bed-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="43bed-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="43bed-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="43bed-112">Not supported.</span></span>|
|<span data-ttu-id="43bed-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="43bed-113">Application</span></span>|<span data-ttu-id="43bed-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="43bed-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="43bed-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="43bed-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="43bed-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="43bed-116">Request headers</span></span>
|<span data-ttu-id="43bed-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="43bed-117">Header</span></span>|<span data-ttu-id="43bed-118">Wert</span><span class="sxs-lookup"><span data-stu-id="43bed-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="43bed-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="43bed-119">Authorization</span></span>|<span data-ttu-id="43bed-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="43bed-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="43bed-121">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="43bed-121">Accept</span></span>|<span data-ttu-id="43bed-122">Anwendung/json</span><span class="sxs-lookup"><span data-stu-id="43bed-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="43bed-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="43bed-123">Request body</span></span>
<span data-ttu-id="43bed-124">Geben Sie im Anforderungstext eine JSON-Darstellung des managedDeviceMobileAppConfigurationDeviceStatus-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="43bed-124">In the request body, supply a JSON representation for the deviceManagementTroubleshootingEvent object.</span></span>

<span data-ttu-id="43bed-125">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen von managedDeviceMobileAppConfigurationDeviceStatus erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="43bed-125">The following table shows the properties that are required when you create the deviceAppManagement.</span></span>

|<span data-ttu-id="43bed-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="43bed-126">Property</span></span>|<span data-ttu-id="43bed-127">Typ</span><span class="sxs-lookup"><span data-stu-id="43bed-127">Type</span></span>|<span data-ttu-id="43bed-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="43bed-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="43bed-129">ID</span><span class="sxs-lookup"><span data-stu-id="43bed-129">id</span></span>|<span data-ttu-id="43bed-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="43bed-130">String</span></span>|<span data-ttu-id="43bed-131">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="43bed-131">Key of the entity.</span></span>|
|<span data-ttu-id="43bed-132">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="43bed-132">deviceDisplayName</span></span>|<span data-ttu-id="43bed-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="43bed-133">String</span></span>|<span data-ttu-id="43bed-134">Gerätename, der dem Objekt des Typs „DevicePolicyStatus“ zugeordnet ist</span><span class="sxs-lookup"><span data-stu-id="43bed-134">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="43bed-135">userName</span><span class="sxs-lookup"><span data-stu-id="43bed-135">userName</span></span>|<span data-ttu-id="43bed-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="43bed-136">String</span></span>|<span data-ttu-id="43bed-137">Gemeldeter Benutzername</span><span class="sxs-lookup"><span data-stu-id="43bed-137">The User Name that is being reported</span></span>|
|<span data-ttu-id="43bed-138">deviceModel</span><span class="sxs-lookup"><span data-stu-id="43bed-138">deviceModel</span></span>|<span data-ttu-id="43bed-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="43bed-139">String</span></span>|<span data-ttu-id="43bed-140">Gemeldetes Gerätemodell</span><span class="sxs-lookup"><span data-stu-id="43bed-140">The device model that is being reported</span></span>|
|<span data-ttu-id="43bed-141">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="43bed-141">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="43bed-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="43bed-142">DateTimeOffset</span></span>|<span data-ttu-id="43bed-143">Datum und Uhrzeit des Ablaufs der Toleranzperiode für die Gerätekonformität</span><span class="sxs-lookup"><span data-stu-id="43bed-143">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="43bed-144">Status</span><span class="sxs-lookup"><span data-stu-id="43bed-144">status</span></span>|[<span data-ttu-id="43bed-145">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="43bed-145">complianceStatus</span></span>](../resources/intune_shared_compliancestatus.md)|<span data-ttu-id="43bed-p102">Compliance-Status des Richtlinienberichts. Mögliche Werte: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="43bed-p102">Compliance status of the policy report. The possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`.</span></span>|
|<span data-ttu-id="43bed-148">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="43bed-148">lastReportedDateTime</span></span>|<span data-ttu-id="43bed-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="43bed-149">DateTimeOffset</span></span>|<span data-ttu-id="43bed-150">Datum und Uhrzeit der letzten Änderung des Richtlinienberichts</span><span class="sxs-lookup"><span data-stu-id="43bed-150">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="43bed-151">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="43bed-151">userPrincipalName</span></span>|<span data-ttu-id="43bed-152">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="43bed-152">String</span></span>|<span data-ttu-id="43bed-153">Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="43bed-153">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="43bed-154">Antwort</span><span class="sxs-lookup"><span data-stu-id="43bed-154">Response</span></span>
<span data-ttu-id="43bed-155">Wenn diese Methode erfolgreich verläuft, werden der `201 Created` Antwortcode und ein [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune_apps_manageddevicemobileappconfigurationdevicestatus.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="43bed-155">If successful, this method returns a `201 Created` response code and a [mobileThreatDefenseConnector](../resources/intune_apps_manageddevicemobileappconfigurationdevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="43bed-156">Beispiel</span><span class="sxs-lookup"><span data-stu-id="43bed-156">Example</span></span>
### <a name="request"></a><span data-ttu-id="43bed-157">Anforderung</span><span class="sxs-lookup"><span data-stu-id="43bed-157">Request</span></span>
<span data-ttu-id="43bed-158">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="43bed-158">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses
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

### <a name="response"></a><span data-ttu-id="43bed-159">Antwort</span><span class="sxs-lookup"><span data-stu-id="43bed-159">Response</span></span>
<span data-ttu-id="43bed-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="43bed-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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








