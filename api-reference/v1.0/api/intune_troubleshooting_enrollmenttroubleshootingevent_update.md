# <a name="update-enrollmenttroubleshootingevent"></a><span data-ttu-id="d115f-101">enrollmentTroubleshootingEvent aktualisieren</span><span class="sxs-lookup"><span data-stu-id="d115f-101">Update enrollmentTroubleshootingEvent</span></span>

> <span data-ttu-id="d115f-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="d115f-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d115f-103">Aktualisieren der Eigenschaften eines [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="d115f-103">Update the properties of a [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d115f-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="d115f-104">Prerequisites</span></span>
<span data-ttu-id="d115f-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="d115f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d115f-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d115f-107">Permission type</span></span>|<span data-ttu-id="d115f-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d115f-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d115f-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d115f-109">Delegated (work or school account)</span></span>|<span data-ttu-id="d115f-110">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d115f-110">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="d115f-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d115f-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d115f-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d115f-112">Not supported.</span></span>|
|<span data-ttu-id="d115f-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d115f-113">Application</span></span>|<span data-ttu-id="d115f-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d115f-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d115f-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d115f-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="d115f-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d115f-116">Request headers</span></span>
|<span data-ttu-id="d115f-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="d115f-117">Header</span></span>|<span data-ttu-id="d115f-118">Wert</span><span class="sxs-lookup"><span data-stu-id="d115f-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d115f-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="d115f-119">Authorization</span></span>|<span data-ttu-id="d115f-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="d115f-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d115f-121">Accept</span><span class="sxs-lookup"><span data-stu-id="d115f-121">Accept</span></span>|<span data-ttu-id="d115f-122">application/json</span><span class="sxs-lookup"><span data-stu-id="d115f-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d115f-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d115f-123">Request body</span></span>
<span data-ttu-id="d115f-124">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md) an.</span><span class="sxs-lookup"><span data-stu-id="d115f-124">In the request body, supply a JSON representation for the [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md) object.</span></span>

<span data-ttu-id="d115f-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="d115f-125">The following table shows the properties that are required when you create the [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md).</span></span>

|<span data-ttu-id="d115f-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d115f-126">Property</span></span>|<span data-ttu-id="d115f-127">Typ</span><span class="sxs-lookup"><span data-stu-id="d115f-127">Type</span></span>|<span data-ttu-id="d115f-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d115f-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d115f-129">id</span><span class="sxs-lookup"><span data-stu-id="d115f-129">id</span></span>|<span data-ttu-id="d115f-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d115f-130">String</span></span>|<span data-ttu-id="d115f-131">UUID für das Objekt. Geerbt von [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="d115f-131">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="d115f-132">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="d115f-132">eventDateTime</span></span>|<span data-ttu-id="d115f-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d115f-133">DateTimeOffset</span></span>|<span data-ttu-id="d115f-134">Uhrzeit, zu der das Ereignis aufgetreten ist.</span><span class="sxs-lookup"><span data-stu-id="d115f-134">Time when the event occurred .</span></span> <span data-ttu-id="d115f-135">Gerbt von [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="d115f-135">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="d115f-136">correlationId</span><span class="sxs-lookup"><span data-stu-id="d115f-136">correlationId</span></span>|<span data-ttu-id="d115f-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d115f-137">String</span></span>|<span data-ttu-id="d115f-138">ID, die für die Verfolgung des Fehlers in dem Dienst verwendet wurde.</span><span class="sxs-lookup"><span data-stu-id="d115f-138">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="d115f-139">Gerbt von [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="d115f-139">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="d115f-140">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="d115f-140">managedDeviceIdentifier</span></span>|<span data-ttu-id="d115f-141">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d115f-141">String</span></span>|<span data-ttu-id="d115f-142">Von Intune erstellter oder erfasster Gerätebezeichner</span><span class="sxs-lookup"><span data-stu-id="d115f-142">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="d115f-143">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="d115f-143">operatingSystem</span></span>|<span data-ttu-id="d115f-144">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d115f-144">String</span></span>|<span data-ttu-id="d115f-145">Betriebssystem</span><span class="sxs-lookup"><span data-stu-id="d115f-145">Operating System.</span></span>|
|<span data-ttu-id="d115f-146">osVersion</span><span class="sxs-lookup"><span data-stu-id="d115f-146">osVersion</span></span>|<span data-ttu-id="d115f-147">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d115f-147">String</span></span>|<span data-ttu-id="d115f-148">Betriebssystemversion</span><span class="sxs-lookup"><span data-stu-id="d115f-148">OS Version.</span></span>|
|<span data-ttu-id="d115f-149">userId</span><span class="sxs-lookup"><span data-stu-id="d115f-149">userId</span></span>|<span data-ttu-id="d115f-150">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d115f-150">String</span></span>|<span data-ttu-id="d115f-151">Bezeichner für den Benutzer, der versucht hat, das Gerät zu registrieren.</span><span class="sxs-lookup"><span data-stu-id="d115f-151">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="d115f-152">deviceId</span><span class="sxs-lookup"><span data-stu-id="d115f-152">deviceId</span></span>|<span data-ttu-id="d115f-153">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d115f-153">String</span></span>|<span data-ttu-id="d115f-154">Azure AD-Gerätebezeichner</span><span class="sxs-lookup"><span data-stu-id="d115f-154">Azure AD device identifier.</span></span>|
|<span data-ttu-id="d115f-155">enrollmentType</span><span class="sxs-lookup"><span data-stu-id="d115f-155">enrollmentType</span></span>|[<span data-ttu-id="d115f-156">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="d115f-156">deviceEnrollmentType</span></span>](../resources/intune_shared_deviceenrollmenttype.md)|<span data-ttu-id="d115f-157">Typ der Registrierung.</span><span class="sxs-lookup"><span data-stu-id="d115f-157">Type of the enrollment.</span></span> <span data-ttu-id="d115f-158">Mögliche Werte: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span><span class="sxs-lookup"><span data-stu-id="d115f-158">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="d115f-159">failureCategory</span><span class="sxs-lookup"><span data-stu-id="d115f-159">failureCategory</span></span>|[<span data-ttu-id="d115f-160">deviceEnrollmentFailureReason</span><span class="sxs-lookup"><span data-stu-id="d115f-160">deviceEnrollmentFailureReason</span></span>](../resources/intune_troubleshooting_deviceenrollmentfailurereason.md)|<span data-ttu-id="d115f-161">Allgemeine Fehlerkategorie.</span><span class="sxs-lookup"><span data-stu-id="d115f-161">Highlevel failure category.</span></span> <span data-ttu-id="d115f-162">Mögliche Werte sind: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected` und `userAbandonment`.</span><span class="sxs-lookup"><span data-stu-id="d115f-162">Possible values are: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`, `userAbandonment`.</span></span>|
|<span data-ttu-id="d115f-163">failureReason</span><span class="sxs-lookup"><span data-stu-id="d115f-163">failureReason</span></span>|<span data-ttu-id="d115f-164">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d115f-164">String</span></span>|<span data-ttu-id="d115f-165">Detaillierte Fehlerursache</span><span class="sxs-lookup"><span data-stu-id="d115f-165">Detailed failure reason.</span></span>|



## <a name="response"></a><span data-ttu-id="d115f-166">Antwort</span><span class="sxs-lookup"><span data-stu-id="d115f-166">Response</span></span>
<span data-ttu-id="d115f-167">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="d115f-167">If successful, this method returns a `200 OK` response code and an updated [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d115f-168">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d115f-168">Example</span></span>
### <a name="request"></a><span data-ttu-id="d115f-169">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d115f-169">Request</span></span>
<span data-ttu-id="d115f-170">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d115f-170">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
Content-type: application/json
Content-length: 440

{
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "correlationId": "Correlation Id value",
  "managedDeviceIdentifier": "Managed Device Identifier value",
  "operatingSystem": "Operating System value",
  "osVersion": "Os Version value",
  "userId": "User Id value",
  "deviceId": "Device Id value",
  "enrollmentType": "userEnrollment",
  "failureCategory": "authentication",
  "failureReason": "Failure Reason value"
}
```

### <a name="response"></a><span data-ttu-id="d115f-171">Antwort</span><span class="sxs-lookup"><span data-stu-id="d115f-171">Response</span></span>
<span data-ttu-id="d115f-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d115f-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 558

{
  "@odata.type": "#microsoft.graph.enrollmentTroubleshootingEvent",
  "id": "c4a623f5-23f5-c4a6-f523-a6c4f523a6c4",
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "correlationId": "Correlation Id value",
  "managedDeviceIdentifier": "Managed Device Identifier value",
  "operatingSystem": "Operating System value",
  "osVersion": "Os Version value",
  "userId": "User Id value",
  "deviceId": "Device Id value",
  "enrollmentType": "userEnrollment",
  "failureCategory": "authentication",
  "failureReason": "Failure Reason value"
}
```



