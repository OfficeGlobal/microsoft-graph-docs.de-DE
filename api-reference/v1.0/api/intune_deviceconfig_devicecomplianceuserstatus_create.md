# <a name="create-devicecomplianceuserstatus"></a><span data-ttu-id="d8dc6-101">Erstellen von „deviceComplianceUserStatus“</span><span class="sxs-lookup"><span data-stu-id="d8dc6-101">Create deviceComplianceUserStatus</span></span>

> <span data-ttu-id="d8dc6-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="d8dc6-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d8dc6-103">Diese Methode erstellt ein neues Objekt des Typs [deviceComplianceUserStatus](../resources/intune_deviceconfig_devicecomplianceuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="d8dc6-103">Create a new [deviceComplianceUserStatus](../resources/intune_deviceconfig_devicecomplianceuserstatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d8dc6-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="d8dc6-104">Prerequisites</span></span>
<span data-ttu-id="d8dc6-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="d8dc6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d8dc6-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d8dc6-107">Permission type</span></span>|<span data-ttu-id="d8dc6-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d8dc6-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d8dc6-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d8dc6-109">Delegated (work or school account)</span></span>|<span data-ttu-id="d8dc6-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8dc6-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d8dc6-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d8dc6-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d8dc6-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d8dc6-112">Not supported.</span></span>|
|<span data-ttu-id="d8dc6-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d8dc6-113">Application</span></span>|<span data-ttu-id="d8dc6-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d8dc6-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d8dc6-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d8dc6-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="d8dc6-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d8dc6-116">Request headers</span></span>
|<span data-ttu-id="d8dc6-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="d8dc6-117">Header</span></span>|<span data-ttu-id="d8dc6-118">Wert</span><span class="sxs-lookup"><span data-stu-id="d8dc6-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d8dc6-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="d8dc6-119">Authorization</span></span>|<span data-ttu-id="d8dc6-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="d8dc6-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d8dc6-121">Accept</span><span class="sxs-lookup"><span data-stu-id="d8dc6-121">Accept</span></span>|<span data-ttu-id="d8dc6-122">application/json</span><span class="sxs-lookup"><span data-stu-id="d8dc6-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d8dc6-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d8dc6-123">Request body</span></span>
<span data-ttu-id="d8dc6-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „deviceComplianceUserStatus“ an.</span><span class="sxs-lookup"><span data-stu-id="d8dc6-124">In the request body, supply a JSON representation for the deviceComplianceUserStatus object.</span></span>

<span data-ttu-id="d8dc6-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „deviceComplianceUserStatus“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="d8dc6-125">The following table shows the properties that are required when you create the deviceComplianceUserStatus.</span></span>

|<span data-ttu-id="d8dc6-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d8dc6-126">Property</span></span>|<span data-ttu-id="d8dc6-127">Typ</span><span class="sxs-lookup"><span data-stu-id="d8dc6-127">Type</span></span>|<span data-ttu-id="d8dc6-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d8dc6-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d8dc6-129">id</span><span class="sxs-lookup"><span data-stu-id="d8dc6-129">id</span></span>|<span data-ttu-id="d8dc6-130">String</span><span class="sxs-lookup"><span data-stu-id="d8dc6-130">String</span></span>|<span data-ttu-id="d8dc6-131">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="d8dc6-131">Key of the entity.</span></span>|
|<span data-ttu-id="d8dc6-132">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="d8dc6-132">userDisplayName</span></span>|<span data-ttu-id="d8dc6-133">String</span><span class="sxs-lookup"><span data-stu-id="d8dc6-133">String</span></span>|<span data-ttu-id="d8dc6-134">Benutzername, der zu dem Objekt des Typs „DevicePolicyStatus“ gehört</span><span class="sxs-lookup"><span data-stu-id="d8dc6-134">User name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="d8dc6-135">devicesCount</span><span class="sxs-lookup"><span data-stu-id="d8dc6-135">devicesCount</span></span>|<span data-ttu-id="d8dc6-136">Int32</span><span class="sxs-lookup"><span data-stu-id="d8dc6-136">Int32</span></span>|<span data-ttu-id="d8dc6-137">Geräteanzahl für den Benutzer</span><span class="sxs-lookup"><span data-stu-id="d8dc6-137">Devices count for that user.</span></span>|
|<span data-ttu-id="d8dc6-138">status</span><span class="sxs-lookup"><span data-stu-id="d8dc6-138">status</span></span>|[<span data-ttu-id="d8dc6-139">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="d8dc6-139">complianceStatus</span></span>](../resources/intune_shared_compliancestatus.md)|<span data-ttu-id="d8dc6-140">Konformitätsstatus des Richtlinienberichts.</span><span class="sxs-lookup"><span data-stu-id="d8dc6-140">Compliance status of the policy report.</span></span> <span data-ttu-id="d8dc6-141">Mögliche Werte sind: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict` und `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="d8dc6-141">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="d8dc6-142">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="d8dc6-142">lastReportedDateTime</span></span>|<span data-ttu-id="d8dc6-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d8dc6-143">DateTimeOffset</span></span>|<span data-ttu-id="d8dc6-144">Datum und Uhrzeit der letzten Änderung des Richtlinienberichts</span><span class="sxs-lookup"><span data-stu-id="d8dc6-144">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="d8dc6-145">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="d8dc6-145">userPrincipalName</span></span>|<span data-ttu-id="d8dc6-146">String</span><span class="sxs-lookup"><span data-stu-id="d8dc6-146">String</span></span>|<span data-ttu-id="d8dc6-147">Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="d8dc6-147">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="d8dc6-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="d8dc6-148">Response</span></span>
<span data-ttu-id="d8dc6-149">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [deviceComplianceUserStatus](../resources/intune_deviceconfig_devicecomplianceuserstatus.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="d8dc6-149">If successful, this method returns a `201 Created` response code and a [deviceComplianceUserStatus](../resources/intune_deviceconfig_devicecomplianceuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d8dc6-150">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d8dc6-150">Example</span></span>
### <a name="request"></a><span data-ttu-id="d8dc6-151">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d8dc6-151">Request</span></span>
<span data-ttu-id="d8dc6-152">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d8dc6-152">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatuses
Content-type: application/json
Content-length: 287

{
  "@odata.type": "#microsoft.graph.deviceComplianceUserStatus",
  "userDisplayName": "User Display Name value",
  "devicesCount": 12,
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="d8dc6-153">Antwort</span><span class="sxs-lookup"><span data-stu-id="d8dc6-153">Response</span></span>
<span data-ttu-id="d8dc6-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d8dc6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 336

{
  "@odata.type": "#microsoft.graph.deviceComplianceUserStatus",
  "id": "a0b566cd-66cd-a0b5-cd66-b5a0cd66b5a0",
  "userDisplayName": "User Display Name value",
  "devicesCount": 12,
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```



