# <a name="create-devicemanagementtroubleshootingevent"></a><span data-ttu-id="9fb43-101">deviceManagementTroubleshootingEvent erstellen</span><span class="sxs-lookup"><span data-stu-id="9fb43-101">Create deviceManagementTroubleshootingEvent</span></span>

> <span data-ttu-id="9fb43-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="9fb43-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9fb43-103">Erstellen eines neuen [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="9fb43-103">Create a new [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9fb43-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="9fb43-104">Prerequisites</span></span>
<span data-ttu-id="9fb43-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="9fb43-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="9fb43-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9fb43-107">Permission type</span></span>|<span data-ttu-id="9fb43-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9fb43-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9fb43-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9fb43-109">Delegated (work or school account)</span></span>|<span data-ttu-id="9fb43-110">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9fb43-110">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="9fb43-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9fb43-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9fb43-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9fb43-112">Not supported.</span></span>|
|<span data-ttu-id="9fb43-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9fb43-113">Application</span></span>|<span data-ttu-id="9fb43-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9fb43-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9fb43-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9fb43-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="9fb43-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9fb43-116">Request headers</span></span>
|<span data-ttu-id="9fb43-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="9fb43-117">Header</span></span>|<span data-ttu-id="9fb43-118">Wert</span><span class="sxs-lookup"><span data-stu-id="9fb43-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9fb43-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="9fb43-119">Authorization</span></span>|<span data-ttu-id="9fb43-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="9fb43-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9fb43-121">Accept</span><span class="sxs-lookup"><span data-stu-id="9fb43-121">Accept</span></span>|<span data-ttu-id="9fb43-122">application/json</span><span class="sxs-lookup"><span data-stu-id="9fb43-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9fb43-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9fb43-123">Request body</span></span>
<span data-ttu-id="9fb43-124">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs deviceManagementTroubleshootingEvent an.</span><span class="sxs-lookup"><span data-stu-id="9fb43-124">In the request body, supply a JSON representation for the deviceManagementTroubleshootingEvent object.</span></span>

<span data-ttu-id="9fb43-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs deviceManagementTroubleshootingEvent erstellen.</span><span class="sxs-lookup"><span data-stu-id="9fb43-125">The following table shows the properties that are required when you create the deviceManagementTroubleshootingEvent.</span></span>

|<span data-ttu-id="9fb43-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9fb43-126">Property</span></span>|<span data-ttu-id="9fb43-127">Typ</span><span class="sxs-lookup"><span data-stu-id="9fb43-127">Type</span></span>|<span data-ttu-id="9fb43-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9fb43-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9fb43-129">id</span><span class="sxs-lookup"><span data-stu-id="9fb43-129">id</span></span>|<span data-ttu-id="9fb43-130">String</span><span class="sxs-lookup"><span data-stu-id="9fb43-130">String</span></span>|<span data-ttu-id="9fb43-131">UUID für das Objekt</span><span class="sxs-lookup"><span data-stu-id="9fb43-131">UUID for the object</span></span>|
|<span data-ttu-id="9fb43-132">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="9fb43-132">eventDateTime</span></span>|<span data-ttu-id="9fb43-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9fb43-133">DateTimeOffset</span></span>|<span data-ttu-id="9fb43-134">Uhrzeit, zu der das Ereignis aufgetreten ist.</span><span class="sxs-lookup"><span data-stu-id="9fb43-134">Time when the event occurred .</span></span>|
|<span data-ttu-id="9fb43-135">correlationId</span><span class="sxs-lookup"><span data-stu-id="9fb43-135">correlationId</span></span>|<span data-ttu-id="9fb43-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9fb43-136">String</span></span>|<span data-ttu-id="9fb43-137">ID, die für die Verfolgung des Fehlers in dem Dienst verwendet wurde.</span><span class="sxs-lookup"><span data-stu-id="9fb43-137">Id used for tracing the failure in the service.</span></span>|



## <a name="response"></a><span data-ttu-id="9fb43-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="9fb43-138">Response</span></span>
<span data-ttu-id="9fb43-139">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9fb43-139">If successful, this method returns a `201 Created` response code and a [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9fb43-140">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9fb43-140">Example</span></span>
### <a name="request"></a><span data-ttu-id="9fb43-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9fb43-141">Request</span></span>
<span data-ttu-id="9fb43-142">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9fb43-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/troubleshootingEvents
Content-type: application/json
Content-length: 179

{
  "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingEvent",
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "correlationId": "Correlation Id value"
}
```

### <a name="response"></a><span data-ttu-id="9fb43-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="9fb43-143">Response</span></span>
<span data-ttu-id="9fb43-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9fb43-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



