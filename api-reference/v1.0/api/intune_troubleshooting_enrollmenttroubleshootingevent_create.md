# <a name="create-enrollmenttroubleshootingevent"></a><span data-ttu-id="cd453-101">EnrollmentTroubleshootingEvent erstellen</span><span class="sxs-lookup"><span data-stu-id="cd453-101">Create enrollmentTroubleshootingEvent</span></span>

> <span data-ttu-id="cd453-102">**Wichtig:** Die APIs der /beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="cd453-102">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cd453-103">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="cd453-103">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cd453-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="cd453-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cd453-105">Erstellen eines neuen [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="cd453-105">Create a new [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cd453-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="cd453-106">Prerequisites</span></span>
<span data-ttu-id="cd453-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="cd453-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="cd453-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="cd453-109">Permission type</span></span>|<span data-ttu-id="cd453-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="cd453-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cd453-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="cd453-111">Delegated (work or school account)</span></span>|<span data-ttu-id="cd453-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd453-112">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="cd453-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="cd453-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cd453-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cd453-114">Not supported.</span></span>|
|<span data-ttu-id="cd453-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="cd453-115">Application</span></span>|<span data-ttu-id="cd453-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cd453-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cd453-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="cd453-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="cd453-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="cd453-118">Request headers</span></span>
|<span data-ttu-id="cd453-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="cd453-119">Header</span></span>|<span data-ttu-id="cd453-120">Wert</span><span class="sxs-lookup"><span data-stu-id="cd453-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cd453-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="cd453-121">Authorization</span></span>|<span data-ttu-id="cd453-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="cd453-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cd453-123">Accept</span><span class="sxs-lookup"><span data-stu-id="cd453-123">Accept</span></span>|<span data-ttu-id="cd453-124">application/json</span><span class="sxs-lookup"><span data-stu-id="cd453-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cd453-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="cd453-125">Request body</span></span>
<span data-ttu-id="cd453-126">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs enrollmentTroubleshootingEvent an.</span><span class="sxs-lookup"><span data-stu-id="cd453-126">In the request body, supply a JSON representation for the enrollmentTroubleshootingEvent object.</span></span>

<span data-ttu-id="cd453-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs enrollmentTroubleshootingEvent erstellen.</span><span class="sxs-lookup"><span data-stu-id="cd453-127">The following table shows the properties that are required when you create the enrollmentTroubleshootingEvent.</span></span>

|<span data-ttu-id="cd453-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="cd453-128">Property</span></span>|<span data-ttu-id="cd453-129">Typ</span><span class="sxs-lookup"><span data-stu-id="cd453-129">Type</span></span>|<span data-ttu-id="cd453-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cd453-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cd453-131">id</span><span class="sxs-lookup"><span data-stu-id="cd453-131">id</span></span>|<span data-ttu-id="cd453-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="cd453-132">String</span></span>|<span data-ttu-id="cd453-133">UUID für das Objekt. Geerbt von [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="cd453-133">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="cd453-134">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="cd453-134">eventDateTime</span></span>|<span data-ttu-id="cd453-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cd453-135">DateTimeOffset</span></span>|<span data-ttu-id="cd453-136">Uhrzeit, zu der das Ereignis aufgetreten ist.</span><span class="sxs-lookup"><span data-stu-id="cd453-136">Time when the event occurred .</span></span> <span data-ttu-id="cd453-137">Gerbt von [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="cd453-137">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="cd453-138">correlationId</span><span class="sxs-lookup"><span data-stu-id="cd453-138">correlationId</span></span>|<span data-ttu-id="cd453-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="cd453-139">String</span></span>|<span data-ttu-id="cd453-140">ID, die für die Verfolgung des Fehlers in dem Dienst verwendet wurde.</span><span class="sxs-lookup"><span data-stu-id="cd453-140">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="cd453-141">Gerbt von [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="cd453-141">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="cd453-142">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="cd453-142">managedDeviceIdentifier</span></span>|<span data-ttu-id="cd453-143">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="cd453-143">String</span></span>|<span data-ttu-id="cd453-144">Von Intune erstellter oder erfasster Gerätebezeichner</span><span class="sxs-lookup"><span data-stu-id="cd453-144">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="cd453-145">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="cd453-145">operatingSystem</span></span>|<span data-ttu-id="cd453-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="cd453-146">String</span></span>|<span data-ttu-id="cd453-147">Betriebssystem</span><span class="sxs-lookup"><span data-stu-id="cd453-147">Operating System.</span></span>|
|<span data-ttu-id="cd453-148">osVersion</span><span class="sxs-lookup"><span data-stu-id="cd453-148">osVersion</span></span>|<span data-ttu-id="cd453-149">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="cd453-149">String</span></span>|<span data-ttu-id="cd453-150">Betriebssystemversion</span><span class="sxs-lookup"><span data-stu-id="cd453-150">OS Version.</span></span>|
|<span data-ttu-id="cd453-151">userId</span><span class="sxs-lookup"><span data-stu-id="cd453-151">userId</span></span>|<span data-ttu-id="cd453-152">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="cd453-152">String</span></span>|<span data-ttu-id="cd453-153">Bezeichner für den Benutzer, der versucht hat, das Gerät zu registrieren.</span><span class="sxs-lookup"><span data-stu-id="cd453-153">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="cd453-154">deviceId</span><span class="sxs-lookup"><span data-stu-id="cd453-154">deviceId</span></span>|<span data-ttu-id="cd453-155">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="cd453-155">String</span></span>|<span data-ttu-id="cd453-156">Azure AD-Gerätebezeichner</span><span class="sxs-lookup"><span data-stu-id="cd453-156">Azure AD device identifier.</span></span>|
|<span data-ttu-id="cd453-157">enrollmentType</span><span class="sxs-lookup"><span data-stu-id="cd453-157">enrollmentType</span></span>|<span data-ttu-id="cd453-158">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="cd453-158">String</span></span>|<span data-ttu-id="cd453-159">Typ der Registrierung.</span><span class="sxs-lookup"><span data-stu-id="cd453-159">Type of the enrollment.</span></span> <span data-ttu-id="cd453-160">Mögliche Werte: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span><span class="sxs-lookup"><span data-stu-id="cd453-160">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="cd453-161">failureCategory</span><span class="sxs-lookup"><span data-stu-id="cd453-161">failureCategory</span></span>|<span data-ttu-id="cd453-162">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="cd453-162">String</span></span>|<span data-ttu-id="cd453-163">Allgemeine Fehlerkategorie.</span><span class="sxs-lookup"><span data-stu-id="cd453-163">Highlevel failure category.</span></span> <span data-ttu-id="cd453-164">Mögliche Werte: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`.</span><span class="sxs-lookup"><span data-stu-id="cd453-164">Possible values are: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`.</span></span>|
|<span data-ttu-id="cd453-165">failureReason</span><span class="sxs-lookup"><span data-stu-id="cd453-165">failureReason</span></span>|<span data-ttu-id="cd453-166">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="cd453-166">String</span></span>|<span data-ttu-id="cd453-167">Detaillierte Fehlerursache</span><span class="sxs-lookup"><span data-stu-id="cd453-167">Detailed failure reason.</span></span>|



## <a name="response"></a><span data-ttu-id="cd453-168">Antwort</span><span class="sxs-lookup"><span data-stu-id="cd453-168">Response</span></span>
<span data-ttu-id="cd453-169">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="cd453-169">If successful, this method returns a `201 Created` response code and a [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cd453-170">Beispiel</span><span class="sxs-lookup"><span data-stu-id="cd453-170">Example</span></span>
### <a name="request"></a><span data-ttu-id="cd453-171">Anforderung</span><span class="sxs-lookup"><span data-stu-id="cd453-171">Request</span></span>
<span data-ttu-id="cd453-172">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="cd453-172">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents
Content-type: application/json
Content-length: 509

{
  "@odata.type": "#microsoft.graph.enrollmentTroubleshootingEvent",
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

### <a name="response"></a><span data-ttu-id="cd453-173">Antwort</span><span class="sxs-lookup"><span data-stu-id="cd453-173">Response</span></span>
<span data-ttu-id="cd453-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cd453-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



