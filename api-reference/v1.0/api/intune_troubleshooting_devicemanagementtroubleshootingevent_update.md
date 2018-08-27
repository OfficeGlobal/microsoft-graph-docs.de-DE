# <a name="update-devicemanagementtroubleshootingevent"></a><span data-ttu-id="7a237-101">deviceManagementTroubleshootingEvent aktualisieren</span><span class="sxs-lookup"><span data-stu-id="7a237-101">Update deviceManagementTroubleshootingEvent</span></span>

> <span data-ttu-id="7a237-102">**Wichtig:** Die APIs der /beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="7a237-102">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7a237-103">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7a237-103">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7a237-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="7a237-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7a237-105">Aktualisieren der Eigenschaften eines [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="7a237-105">Update the properties of a [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7a237-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="7a237-106">Prerequisites</span></span>
<span data-ttu-id="7a237-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="7a237-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="7a237-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7a237-109">Permission type</span></span>|<span data-ttu-id="7a237-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7a237-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7a237-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7a237-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7a237-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7a237-112">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="7a237-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7a237-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7a237-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7a237-114">Not supported.</span></span>|
|<span data-ttu-id="7a237-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7a237-115">Application</span></span>|<span data-ttu-id="7a237-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7a237-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7a237-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7a237-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="7a237-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7a237-118">Request headers</span></span>
|<span data-ttu-id="7a237-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="7a237-119">Header</span></span>|<span data-ttu-id="7a237-120">Wert</span><span class="sxs-lookup"><span data-stu-id="7a237-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7a237-121">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="7a237-121">Authorization</span></span>|<span data-ttu-id="7a237-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="7a237-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7a237-123">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="7a237-123">Accept</span></span>|<span data-ttu-id="7a237-124">application/json</span><span class="sxs-lookup"><span data-stu-id="7a237-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7a237-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7a237-125">Request body</span></span>
<span data-ttu-id="7a237-126">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md) an.</span><span class="sxs-lookup"><span data-stu-id="7a237-126">In the request body, supply a JSON representation for the [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md) object.</span></span>

<span data-ttu-id="7a237-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="7a237-127">The following table shows the properties that are required when you create the [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md).</span></span>

|<span data-ttu-id="7a237-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7a237-128">Property</span></span>|<span data-ttu-id="7a237-129">Typ</span><span class="sxs-lookup"><span data-stu-id="7a237-129">Type</span></span>|<span data-ttu-id="7a237-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7a237-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7a237-131">ID</span><span class="sxs-lookup"><span data-stu-id="7a237-131">id</span></span>|<span data-ttu-id="7a237-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7a237-132">String</span></span>|<span data-ttu-id="7a237-133">UUID für das Objekt</span><span class="sxs-lookup"><span data-stu-id="7a237-133">UUID for the object</span></span>|
|<span data-ttu-id="7a237-134">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="7a237-134">eventDateTime</span></span>|<span data-ttu-id="7a237-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7a237-135">DateTimeOffset</span></span>|<span data-ttu-id="7a237-136">Uhrzeit, zu der das Ereignis aufgetreten ist.</span><span class="sxs-lookup"><span data-stu-id="7a237-136">Time when the event occurred .</span></span>|
|<span data-ttu-id="7a237-137">correlationId</span><span class="sxs-lookup"><span data-stu-id="7a237-137">correlationId</span></span>|<span data-ttu-id="7a237-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7a237-138">String</span></span>|<span data-ttu-id="7a237-139">ID, die für die Verfolgung des Fehlers in dem Dienst verwendet wurde.</span><span class="sxs-lookup"><span data-stu-id="7a237-139">Id used for tracing the failure in the service.</span></span>|



## <a name="response"></a><span data-ttu-id="7a237-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="7a237-140">Response</span></span>
<span data-ttu-id="7a237-141">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein aktualisiertes [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7a237-141">If successful, this method returns a `200 OK` response code and an updated [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7a237-142">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7a237-142">Example</span></span>
### <a name="request"></a><span data-ttu-id="7a237-143">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7a237-143">Request</span></span>
<span data-ttu-id="7a237-144">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7a237-144">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
Content-type: application/json
Content-length: 104

{
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "correlationId": "Correlation Id value"
}
```

### <a name="response"></a><span data-ttu-id="7a237-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="7a237-145">Response</span></span>
<span data-ttu-id="7a237-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7a237-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 228

{
  "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingEvent",
  "id": "fb26dcee-dcee-fb26-eedc-26fbeedc26fb",
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "correlationId": "Correlation Id value"
}
```



