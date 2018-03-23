# <a name="update-devicecomplianceuserstatus"></a><span data-ttu-id="d0459-101">Aktualisieren von „deviceComplianceUserStatus“</span><span class="sxs-lookup"><span data-stu-id="d0459-101">Update deviceComplianceUserStatus</span></span>

> <span data-ttu-id="d0459-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="d0459-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d0459-103">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [deviceComplianceUserStatus](../resources/intune_deviceconfig_devicecomplianceuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="d0459-103">Update the properties of a [calendar](../resources/intune_deviceconfig_devicecomplianceuserstatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d0459-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="d0459-104">Prerequisites</span></span>
<span data-ttu-id="d0459-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="d0459-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d0459-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d0459-107">Permission type</span></span>|<span data-ttu-id="d0459-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d0459-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d0459-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d0459-109">Delegated (work or school account)</span></span>|<span data-ttu-id="d0459-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0459-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d0459-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d0459-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d0459-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d0459-112">Not supported.</span></span>|
|<span data-ttu-id="d0459-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d0459-113">Application</span></span>|<span data-ttu-id="d0459-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d0459-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d0459-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d0459-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatuses/{deviceComplianceUserStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="d0459-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d0459-116">Request headers</span></span>
|<span data-ttu-id="d0459-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="d0459-117">Header</span></span>|<span data-ttu-id="d0459-118">Wert</span><span class="sxs-lookup"><span data-stu-id="d0459-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d0459-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="d0459-119">Authorization</span></span>|<span data-ttu-id="d0459-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="d0459-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="d0459-121">Accept</span><span class="sxs-lookup"><span data-stu-id="d0459-121">Accept</span></span>|<span data-ttu-id="d0459-122">application/json</span><span class="sxs-lookup"><span data-stu-id="d0459-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d0459-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d0459-123">Request body</span></span>
<span data-ttu-id="d0459-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceComplianceUserStatus](../resources/intune_deviceconfig_devicecomplianceuserstatus.md) an.</span><span class="sxs-lookup"><span data-stu-id="d0459-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_deviceconfig_devicecomplianceuserstatus.md) object.</span></span>

<span data-ttu-id="d0459-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceComplianceUserStatus](../resources/intune_deviceconfig_devicecomplianceuserstatus.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="d0459-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="d0459-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d0459-126">Property</span></span>|<span data-ttu-id="d0459-127">Typ</span><span class="sxs-lookup"><span data-stu-id="d0459-127">Type</span></span>|<span data-ttu-id="d0459-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d0459-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d0459-129">id</span><span class="sxs-lookup"><span data-stu-id="d0459-129">id</span></span>|<span data-ttu-id="d0459-130">String</span><span class="sxs-lookup"><span data-stu-id="d0459-130">String</span></span>|<span data-ttu-id="d0459-131">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="d0459-131">Key of the setting.</span></span>|
|<span data-ttu-id="d0459-132">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="d0459-132">userDisplayName</span></span>|<span data-ttu-id="d0459-133">String</span><span class="sxs-lookup"><span data-stu-id="d0459-133">String</span></span>|<span data-ttu-id="d0459-134">Benutzername, der zu dem Objekt des Typs „DevicePolicyStatus“ gehört</span><span class="sxs-lookup"><span data-stu-id="d0459-134">User name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="d0459-135">devicesCount</span><span class="sxs-lookup"><span data-stu-id="d0459-135">devicesCount</span></span>|<span data-ttu-id="d0459-136">Int32</span><span class="sxs-lookup"><span data-stu-id="d0459-136">Int32</span></span>|<span data-ttu-id="d0459-137">Geräteanzahl für den Benutzer</span><span class="sxs-lookup"><span data-stu-id="d0459-137">Devices count for that user.</span></span>|
|<span data-ttu-id="d0459-138">status</span><span class="sxs-lookup"><span data-stu-id="d0459-138">status</span></span>|<span data-ttu-id="d0459-139">String</span><span class="sxs-lookup"><span data-stu-id="d0459-139">String</span></span>|<span data-ttu-id="d0459-140">Konformitätsstatus des Richtlinienberichts.</span><span class="sxs-lookup"><span data-stu-id="d0459-140">Compliance status of the policy report.</span></span> <span data-ttu-id="d0459-141">Mögliche Werte sind: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error` und `conflict`.</span><span class="sxs-lookup"><span data-stu-id="d0459-141">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`.</span></span>|
|<span data-ttu-id="d0459-142">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="d0459-142">lastReportedDateTime</span></span>|<span data-ttu-id="d0459-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d0459-143">DateTimeOffset</span></span>|<span data-ttu-id="d0459-144">Datum und Uhrzeit der letzten Änderung des Richtlinienberichts</span><span class="sxs-lookup"><span data-stu-id="d0459-144">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="d0459-145">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="d0459-145">userPrincipalName</span></span>|<span data-ttu-id="d0459-146">String</span><span class="sxs-lookup"><span data-stu-id="d0459-146">String</span></span>|<span data-ttu-id="d0459-147">Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="d0459-147">userPrincipalName</span></span>|



## <a name="response"></a><span data-ttu-id="d0459-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="d0459-148">Response</span></span>
<span data-ttu-id="d0459-149">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [deviceComplianceUserStatus](../resources/intune_deviceconfig_devicecomplianceuserstatus.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="d0459-149">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_deviceconfig_devicecomplianceuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d0459-150">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d0459-150">Example</span></span>
### <a name="request"></a><span data-ttu-id="d0459-151">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d0459-151">Request</span></span>
<span data-ttu-id="d0459-152">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d0459-152">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatuses/{deviceComplianceUserStatusId}
Content-type: application/json
Content-length: 222

{
  "userDisplayName": "User Display Name value",
  "devicesCount": 12,
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="d0459-153">Antwort</span><span class="sxs-lookup"><span data-stu-id="d0459-153">Response</span></span>
<span data-ttu-id="d0459-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d0459-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



