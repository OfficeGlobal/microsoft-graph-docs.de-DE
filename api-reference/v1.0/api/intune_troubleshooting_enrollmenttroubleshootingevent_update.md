# <a name="update-enrollmenttroubleshootingevent"></a><span data-ttu-id="8acd8-101">enrollmentTroubleshootingEvent aktualisieren</span><span class="sxs-lookup"><span data-stu-id="8acd8-101">Update enrollmentTroubleshootingEvent</span></span>

> <span data-ttu-id="8acd8-102">**Wichtig:** Die APIs der /beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="8acd8-102">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8acd8-103">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8acd8-103">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8acd8-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="8acd8-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8acd8-105">Aktualisieren der Eigenschaften eines [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="8acd8-105">Update the properties of a [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8acd8-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="8acd8-106">Prerequisites</span></span>
<span data-ttu-id="8acd8-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="8acd8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="8acd8-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8acd8-109">Permission type</span></span>|<span data-ttu-id="8acd8-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8acd8-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8acd8-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8acd8-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8acd8-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8acd8-112">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="8acd8-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8acd8-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8acd8-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8acd8-114">Not supported.</span></span>|
|<span data-ttu-id="8acd8-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8acd8-115">Application</span></span>|<span data-ttu-id="8acd8-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8acd8-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8acd8-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8acd8-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="8acd8-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8acd8-118">Request headers</span></span>
|<span data-ttu-id="8acd8-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="8acd8-119">Header</span></span>|<span data-ttu-id="8acd8-120">Wert</span><span class="sxs-lookup"><span data-stu-id="8acd8-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8acd8-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="8acd8-121">Authorization</span></span>|<span data-ttu-id="8acd8-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="8acd8-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8acd8-123">Accept</span><span class="sxs-lookup"><span data-stu-id="8acd8-123">Accept</span></span>|<span data-ttu-id="8acd8-124">application/json</span><span class="sxs-lookup"><span data-stu-id="8acd8-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8acd8-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8acd8-125">Request body</span></span>
<span data-ttu-id="8acd8-126">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md) an.</span><span class="sxs-lookup"><span data-stu-id="8acd8-126">In the request body, supply a JSON representation for the [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md) object.</span></span>

<span data-ttu-id="8acd8-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="8acd8-127">The following table shows the properties that are required when you create the [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md).</span></span>

|<span data-ttu-id="8acd8-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8acd8-128">Property</span></span>|<span data-ttu-id="8acd8-129">Typ</span><span class="sxs-lookup"><span data-stu-id="8acd8-129">Type</span></span>|<span data-ttu-id="8acd8-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8acd8-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8acd8-131">id</span><span class="sxs-lookup"><span data-stu-id="8acd8-131">id</span></span>|<span data-ttu-id="8acd8-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8acd8-132">String</span></span>|<span data-ttu-id="8acd8-133">UUID für das Objekt. Geerbt von [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="8acd8-133">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="8acd8-134">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="8acd8-134">eventDateTime</span></span>|<span data-ttu-id="8acd8-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8acd8-135">DateTimeOffset</span></span>|<span data-ttu-id="8acd8-136">Uhrzeit, zu der das Ereignis aufgetreten ist.</span><span class="sxs-lookup"><span data-stu-id="8acd8-136">Time when the event occurred .</span></span> <span data-ttu-id="8acd8-137">Gerbt von [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="8acd8-137">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="8acd8-138">correlationId</span><span class="sxs-lookup"><span data-stu-id="8acd8-138">correlationId</span></span>|<span data-ttu-id="8acd8-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8acd8-139">String</span></span>|<span data-ttu-id="8acd8-140">ID, die für die Verfolgung des Fehlers in dem Dienst verwendet wurde.</span><span class="sxs-lookup"><span data-stu-id="8acd8-140">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="8acd8-141">Gerbt von [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="8acd8-141">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="8acd8-142">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="8acd8-142">managedDeviceIdentifier</span></span>|<span data-ttu-id="8acd8-143">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8acd8-143">String</span></span>|<span data-ttu-id="8acd8-144">Von Intune erstellter oder erfasster Gerätebezeichner</span><span class="sxs-lookup"><span data-stu-id="8acd8-144">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="8acd8-145">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="8acd8-145">operatingSystem</span></span>|<span data-ttu-id="8acd8-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8acd8-146">String</span></span>|<span data-ttu-id="8acd8-147">Betriebssystem</span><span class="sxs-lookup"><span data-stu-id="8acd8-147">Operating System.</span></span>|
|<span data-ttu-id="8acd8-148">osVersion</span><span class="sxs-lookup"><span data-stu-id="8acd8-148">osVersion</span></span>|<span data-ttu-id="8acd8-149">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8acd8-149">String</span></span>|<span data-ttu-id="8acd8-150">Betriebssystemversion</span><span class="sxs-lookup"><span data-stu-id="8acd8-150">OS Version.</span></span>|
|<span data-ttu-id="8acd8-151">userId</span><span class="sxs-lookup"><span data-stu-id="8acd8-151">userId</span></span>|<span data-ttu-id="8acd8-152">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8acd8-152">String</span></span>|<span data-ttu-id="8acd8-153">Bezeichner für den Benutzer, der versucht hat, das Gerät zu registrieren.</span><span class="sxs-lookup"><span data-stu-id="8acd8-153">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="8acd8-154">deviceId</span><span class="sxs-lookup"><span data-stu-id="8acd8-154">deviceId</span></span>|<span data-ttu-id="8acd8-155">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8acd8-155">String</span></span>|<span data-ttu-id="8acd8-156">Azure AD-Gerätebezeichner</span><span class="sxs-lookup"><span data-stu-id="8acd8-156">Azure AD device identifier.</span></span>|
|<span data-ttu-id="8acd8-157">enrollmentType</span><span class="sxs-lookup"><span data-stu-id="8acd8-157">enrollmentType</span></span>|<span data-ttu-id="8acd8-158">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8acd8-158">String</span></span>|<span data-ttu-id="8acd8-159">Typ der Registrierung.</span><span class="sxs-lookup"><span data-stu-id="8acd8-159">Type of the enrollment.</span></span> <span data-ttu-id="8acd8-160">Mögliche Werte: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span><span class="sxs-lookup"><span data-stu-id="8acd8-160">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="8acd8-161">failureCategory</span><span class="sxs-lookup"><span data-stu-id="8acd8-161">failureCategory</span></span>|<span data-ttu-id="8acd8-162">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8acd8-162">String</span></span>|<span data-ttu-id="8acd8-163">Allgemeine Fehlerkategorie.</span><span class="sxs-lookup"><span data-stu-id="8acd8-163">Highlevel failure category.</span></span> <span data-ttu-id="8acd8-164">Mögliche Werte: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`.</span><span class="sxs-lookup"><span data-stu-id="8acd8-164">Possible values are: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`.</span></span>|
|<span data-ttu-id="8acd8-165">failureReason</span><span class="sxs-lookup"><span data-stu-id="8acd8-165">failureReason</span></span>|<span data-ttu-id="8acd8-166">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8acd8-166">String</span></span>|<span data-ttu-id="8acd8-167">Detaillierte Fehlerursache</span><span class="sxs-lookup"><span data-stu-id="8acd8-167">Detailed failure reason.</span></span>|



## <a name="response"></a><span data-ttu-id="8acd8-168">Antwort</span><span class="sxs-lookup"><span data-stu-id="8acd8-168">Response</span></span>
<span data-ttu-id="8acd8-169">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="8acd8-169">If successful, this method returns a `200 OK` response code and an updated [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8acd8-170">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8acd8-170">Example</span></span>
### <a name="request"></a><span data-ttu-id="8acd8-171">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8acd8-171">Request</span></span>
<span data-ttu-id="8acd8-172">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8acd8-172">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
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

### <a name="response"></a><span data-ttu-id="8acd8-173">Antwort</span><span class="sxs-lookup"><span data-stu-id="8acd8-173">Response</span></span>
<span data-ttu-id="8acd8-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8acd8-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



