# <a name="create-manageddevicemobileappconfigurationuserstatus"></a><span data-ttu-id="27fa4-101">Erstellen von „managedDeviceMobileAppConfigurationUserStatus“</span><span class="sxs-lookup"><span data-stu-id="27fa4-101">Create managedDeviceMobileAppConfigurationUserStatus</span></span>

> <span data-ttu-id="27fa4-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="27fa4-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="27fa4-103">Diese Methode erstellt ein neues Objekt des Typs [managedDeviceMobileAppConfigurationUserStatus](../resources/intune_apps_manageddevicemobileappconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="27fa4-103">Create a new [plannerBucket](../resources/intune_apps_manageddevicemobileappconfigurationuserstatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="27fa4-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="27fa4-104">Prerequisites</span></span>
<span data-ttu-id="27fa4-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="27fa4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="27fa4-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="27fa4-107">Permission type</span></span>|<span data-ttu-id="27fa4-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="27fa4-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="27fa4-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="27fa4-109">Delegated (work or school account)</span></span>|<span data-ttu-id="27fa4-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27fa4-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="27fa4-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="27fa4-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="27fa4-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="27fa4-112">Not supported.</span></span>|
|<span data-ttu-id="27fa4-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="27fa4-113">Application</span></span>|<span data-ttu-id="27fa4-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="27fa4-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="27fa4-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="27fa4-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="27fa4-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="27fa4-116">Request headers</span></span>
|<span data-ttu-id="27fa4-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="27fa4-117">Header</span></span>|<span data-ttu-id="27fa4-118">Wert</span><span class="sxs-lookup"><span data-stu-id="27fa4-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="27fa4-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="27fa4-119">Authorization</span></span>|<span data-ttu-id="27fa4-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="27fa4-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="27fa4-121">Accept</span><span class="sxs-lookup"><span data-stu-id="27fa4-121">Accept</span></span>|<span data-ttu-id="27fa4-122">application/json</span><span class="sxs-lookup"><span data-stu-id="27fa4-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="27fa4-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="27fa4-123">Request body</span></span>
<span data-ttu-id="27fa4-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „managedDeviceMobileAppConfigurationUserStatus“ an.</span><span class="sxs-lookup"><span data-stu-id="27fa4-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="27fa4-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „managedDeviceMobileAppConfigurationUserStatus“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="27fa4-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="27fa4-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="27fa4-126">Property</span></span>|<span data-ttu-id="27fa4-127">Typ</span><span class="sxs-lookup"><span data-stu-id="27fa4-127">Type</span></span>|<span data-ttu-id="27fa4-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="27fa4-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="27fa4-129">id</span><span class="sxs-lookup"><span data-stu-id="27fa4-129">id</span></span>|<span data-ttu-id="27fa4-130">String</span><span class="sxs-lookup"><span data-stu-id="27fa4-130">String</span></span>|<span data-ttu-id="27fa4-131">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="27fa4-131">Key of the setting.</span></span>|
|<span data-ttu-id="27fa4-132">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="27fa4-132">userDisplayName</span></span>|<span data-ttu-id="27fa4-133">String</span><span class="sxs-lookup"><span data-stu-id="27fa4-133">String</span></span>|<span data-ttu-id="27fa4-134">Benutzername, der zu dem Objekt des Typs „DevicePolicyStatus“ gehört</span><span class="sxs-lookup"><span data-stu-id="27fa4-134">User name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="27fa4-135">devicesCount</span><span class="sxs-lookup"><span data-stu-id="27fa4-135">devicesCount</span></span>|<span data-ttu-id="27fa4-136">Int32</span><span class="sxs-lookup"><span data-stu-id="27fa4-136">Int32</span></span>|<span data-ttu-id="27fa4-137">Geräteanzahl für den Benutzer</span><span class="sxs-lookup"><span data-stu-id="27fa4-137">Devices count for that user.</span></span>|
|<span data-ttu-id="27fa4-138">status</span><span class="sxs-lookup"><span data-stu-id="27fa4-138">status</span></span>|<span data-ttu-id="27fa4-139">String</span><span class="sxs-lookup"><span data-stu-id="27fa4-139">String</span></span>|<span data-ttu-id="27fa4-140">Konformitätsstatus des Richtlinienberichts.</span><span class="sxs-lookup"><span data-stu-id="27fa4-140">Compliance status of the policy report.</span></span> <span data-ttu-id="27fa4-141">Mögliche Werte sind: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error` und `conflict`.</span><span class="sxs-lookup"><span data-stu-id="27fa4-141">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`.</span></span>|
|<span data-ttu-id="27fa4-142">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="27fa4-142">lastReportedDateTime</span></span>|<span data-ttu-id="27fa4-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="27fa4-143">DateTimeOffset</span></span>|<span data-ttu-id="27fa4-144">Datum und Uhrzeit der letzten Änderung des Richtlinienberichts</span><span class="sxs-lookup"><span data-stu-id="27fa4-144">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="27fa4-145">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="27fa4-145">userPrincipalName</span></span>|<span data-ttu-id="27fa4-146">String</span><span class="sxs-lookup"><span data-stu-id="27fa4-146">String</span></span>|<span data-ttu-id="27fa4-147">Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="27fa4-147">userPrincipalName</span></span>|



## <a name="response"></a><span data-ttu-id="27fa4-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="27fa4-148">Response</span></span>
<span data-ttu-id="27fa4-149">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [managedDeviceMobileAppConfigurationUserStatus](../resources/intune_apps_manageddevicemobileappconfigurationuserstatus.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="27fa4-149">If successful, this method returns a `201 Created` response code and a [DriveItemVersion](../resources/intune_apps_manageddevicemobileappconfigurationuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="27fa4-150">Beispiel</span><span class="sxs-lookup"><span data-stu-id="27fa4-150">Example</span></span>
### <a name="request"></a><span data-ttu-id="27fa4-151">Anforderung</span><span class="sxs-lookup"><span data-stu-id="27fa4-151">Request</span></span>
<span data-ttu-id="27fa4-152">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="27fa4-152">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatuses
Content-type: application/json
Content-length: 306

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationUserStatus",
  "userDisplayName": "User Display Name value",
  "devicesCount": 12,
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="27fa4-153">Antwort</span><span class="sxs-lookup"><span data-stu-id="27fa4-153">Response</span></span>
<span data-ttu-id="27fa4-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="27fa4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 355

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationUserStatus",
  "id": "44960944-0944-4496-4409-964444099644",
  "userDisplayName": "User Display Name value",
  "devicesCount": 12,
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```



