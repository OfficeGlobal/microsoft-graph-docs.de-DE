# <a name="create-devicemanagementtroubleshootingevent"></a><span data-ttu-id="b5403-101">deviceManagementTroubleshootingEvent erstellen</span><span class="sxs-lookup"><span data-stu-id="b5403-101">Create deviceManagementTroubleshootingEvent</span></span>

> <span data-ttu-id="b5403-102">**Wichtig:** Die APIs der /beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b5403-102">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b5403-103">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b5403-103">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b5403-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="b5403-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b5403-105">Erstellen eines neuen [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="b5403-105">Create a new [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b5403-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b5403-106">Prerequisites</span></span>
<span data-ttu-id="b5403-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b5403-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b5403-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b5403-109">Permission type</span></span>|<span data-ttu-id="b5403-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b5403-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b5403-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b5403-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b5403-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5403-112">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="b5403-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b5403-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b5403-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b5403-114">Not supported.</span></span>|
|<span data-ttu-id="b5403-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b5403-115">Application</span></span>|<span data-ttu-id="b5403-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b5403-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b5403-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b5403-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="b5403-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b5403-118">Request headers</span></span>
|<span data-ttu-id="b5403-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="b5403-119">Header</span></span>|<span data-ttu-id="b5403-120">Wert</span><span class="sxs-lookup"><span data-stu-id="b5403-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b5403-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b5403-121">Authorization</span></span>|<span data-ttu-id="b5403-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b5403-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b5403-123">Accept</span><span class="sxs-lookup"><span data-stu-id="b5403-123">Accept</span></span>|<span data-ttu-id="b5403-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b5403-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b5403-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b5403-125">Request body</span></span>
<span data-ttu-id="b5403-126">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs deviceManagementTroubleshootingEvent an.</span><span class="sxs-lookup"><span data-stu-id="b5403-126">In the request body, supply a JSON representation for the deviceManagementTroubleshootingEvent object.</span></span>

<span data-ttu-id="b5403-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs deviceManagementTroubleshootingEvent erstellen.</span><span class="sxs-lookup"><span data-stu-id="b5403-127">The following table shows the properties that are required when you create the deviceManagementTroubleshootingEvent.</span></span>

|<span data-ttu-id="b5403-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b5403-128">Property</span></span>|<span data-ttu-id="b5403-129">Typ</span><span class="sxs-lookup"><span data-stu-id="b5403-129">Type</span></span>|<span data-ttu-id="b5403-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b5403-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b5403-131">id</span><span class="sxs-lookup"><span data-stu-id="b5403-131">id</span></span>|<span data-ttu-id="b5403-132">String</span><span class="sxs-lookup"><span data-stu-id="b5403-132">String</span></span>|<span data-ttu-id="b5403-133">UUID für das Objekt</span><span class="sxs-lookup"><span data-stu-id="b5403-133">UUID for the object</span></span>|
|<span data-ttu-id="b5403-134">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="b5403-134">eventDateTime</span></span>|<span data-ttu-id="b5403-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b5403-135">DateTimeOffset</span></span>|<span data-ttu-id="b5403-136">Uhrzeit, zu der das Ereignis aufgetreten ist.</span><span class="sxs-lookup"><span data-stu-id="b5403-136">Time when the event occurred .</span></span>|
|<span data-ttu-id="b5403-137">correlationId</span><span class="sxs-lookup"><span data-stu-id="b5403-137">correlationId</span></span>|<span data-ttu-id="b5403-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b5403-138">String</span></span>|<span data-ttu-id="b5403-139">ID, die für die Verfolgung des Fehlers in dem Dienst verwendet wurde.</span><span class="sxs-lookup"><span data-stu-id="b5403-139">Id used for tracing the failure in the service.</span></span>|



## <a name="response"></a><span data-ttu-id="b5403-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="b5403-140">Response</span></span>
<span data-ttu-id="b5403-141">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b5403-141">If successful, this method returns a `201 Created` response code and a [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b5403-142">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b5403-142">Example</span></span>
### <a name="request"></a><span data-ttu-id="b5403-143">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b5403-143">Request</span></span>
<span data-ttu-id="b5403-144">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b5403-144">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents
Content-type: application/json
Content-length: 179

{
  "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingEvent",
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "correlationId": "Correlation Id value"
}
```

### <a name="response"></a><span data-ttu-id="b5403-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="b5403-145">Response</span></span>
<span data-ttu-id="b5403-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b5403-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 228

{
  "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingEvent",
  "id": "fb26dcee-dcee-fb26-eedc-26fbeedc26fb",
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "correlationId": "Correlation Id value"
}
```



