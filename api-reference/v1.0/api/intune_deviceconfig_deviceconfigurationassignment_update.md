# <a name="update-deviceconfigurationassignment"></a><span data-ttu-id="1b956-101">Aktualisieren von „deviceConfigurationAssignment“</span><span class="sxs-lookup"><span data-stu-id="1b956-101">Update deviceConfigurationAssignment</span></span>

> <span data-ttu-id="1b956-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="1b956-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1b956-103">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="1b956-103">Update the properties of a [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1b956-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="1b956-104">Prerequisites</span></span>
<span data-ttu-id="1b956-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="1b956-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="1b956-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1b956-107">Permission type</span></span>|<span data-ttu-id="1b956-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1b956-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1b956-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1b956-109">Delegated (work or school account)</span></span>|<span data-ttu-id="1b956-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b956-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1b956-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1b956-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1b956-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1b956-112">Not supported.</span></span>|
|<span data-ttu-id="1b956-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1b956-113">Application</span></span>|<span data-ttu-id="1b956-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1b956-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1b956-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1b956-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments/{deviceConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="1b956-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1b956-116">Request headers</span></span>
|<span data-ttu-id="1b956-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="1b956-117">Header</span></span>|<span data-ttu-id="1b956-118">Wert</span><span class="sxs-lookup"><span data-stu-id="1b956-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1b956-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="1b956-119">Authorization</span></span>|<span data-ttu-id="1b956-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="1b956-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1b956-121">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="1b956-121">Accept</span></span>|<span data-ttu-id="1b956-122">Anwendung/json</span><span class="sxs-lookup"><span data-stu-id="1b956-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1b956-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1b956-123">Request body</span></span>
<span data-ttu-id="1b956-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md) an.</span><span class="sxs-lookup"><span data-stu-id="1b956-124">In the request body, supply a JSON representation for the [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md) object.</span></span>

<span data-ttu-id="1b956-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="1b956-125">The following table shows the properties that are required when you create the [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md).</span></span>

|<span data-ttu-id="1b956-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1b956-126">Property</span></span>|<span data-ttu-id="1b956-127">Typ</span><span class="sxs-lookup"><span data-stu-id="1b956-127">Type</span></span>|<span data-ttu-id="1b956-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1b956-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1b956-129">ID</span><span class="sxs-lookup"><span data-stu-id="1b956-129">id</span></span>|<span data-ttu-id="1b956-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1b956-130">String</span></span>|<span data-ttu-id="1b956-131">Schlüssel der Zuweisung</span><span class="sxs-lookup"><span data-stu-id="1b956-131">The key of the assignment.</span></span>|
|<span data-ttu-id="1b956-132">Ziel</span><span class="sxs-lookup"><span data-stu-id="1b956-132">target</span></span>|[<span data-ttu-id="1b956-133">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="1b956-133">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune_shared_deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="1b956-134">Zuweisungsziel für die Gerätekonfiguration</span><span class="sxs-lookup"><span data-stu-id="1b956-134">The assignment target for the device configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="1b956-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="1b956-135">Response</span></span>
<span data-ttu-id="1b956-136">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="1b956-136">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1b956-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1b956-137">Example</span></span>
### <a name="request"></a><span data-ttu-id="1b956-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1b956-138">Request</span></span>
<span data-ttu-id="1b956-139">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1b956-139">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments/{deviceConfigurationAssignmentId}
Content-type: application/json
Content-length: 101

{
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="1b956-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="1b956-140">Response</span></span>
<span data-ttu-id="1b956-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1b956-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 218

{
  "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
  "id": "d59b6342-6342-d59b-4263-9bd542639bd5",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```








