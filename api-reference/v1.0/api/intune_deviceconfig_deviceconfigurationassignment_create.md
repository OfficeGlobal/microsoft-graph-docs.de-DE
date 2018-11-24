# <a name="create-deviceconfigurationassignment"></a><span data-ttu-id="0b3d8-101">Erstellen von „deviceConfigurationAssignment“</span><span class="sxs-lookup"><span data-stu-id="0b3d8-101">Create deviceConfigurationAssignment</span></span>

> <span data-ttu-id="0b3d8-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="0b3d8-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0b3d8-103">Diese Methode erstellt ein neues Objekt des Typs [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="0b3d8-103">Create a new [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0b3d8-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="0b3d8-104">Prerequisites</span></span>
<span data-ttu-id="0b3d8-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="0b3d8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="0b3d8-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0b3d8-107">Permission type</span></span>|<span data-ttu-id="0b3d8-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0b3d8-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0b3d8-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0b3d8-109">Delegated (work or school account)</span></span>|<span data-ttu-id="0b3d8-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b3d8-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0b3d8-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0b3d8-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0b3d8-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0b3d8-112">Not supported.</span></span>|
|<span data-ttu-id="0b3d8-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0b3d8-113">Application</span></span>|<span data-ttu-id="0b3d8-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0b3d8-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0b3d8-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0b3d8-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="0b3d8-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0b3d8-116">Request headers</span></span>
|<span data-ttu-id="0b3d8-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="0b3d8-117">Header</span></span>|<span data-ttu-id="0b3d8-118">Wert</span><span class="sxs-lookup"><span data-stu-id="0b3d8-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0b3d8-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="0b3d8-119">Authorization</span></span>|<span data-ttu-id="0b3d8-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="0b3d8-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0b3d8-121">Accept</span><span class="sxs-lookup"><span data-stu-id="0b3d8-121">Accept</span></span>|<span data-ttu-id="0b3d8-122">application/json</span><span class="sxs-lookup"><span data-stu-id="0b3d8-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0b3d8-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0b3d8-123">Request body</span></span>
<span data-ttu-id="0b3d8-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „deviceConfigurationAssignment“ an.</span><span class="sxs-lookup"><span data-stu-id="0b3d8-124">In the request body, supply a JSON representation for the deviceConfigurationAssignment object.</span></span>

<span data-ttu-id="0b3d8-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „deviceConfigurationAssignment“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="0b3d8-125">The following table shows the properties that are required when you create the deviceConfigurationAssignment.</span></span>

|<span data-ttu-id="0b3d8-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0b3d8-126">Property</span></span>|<span data-ttu-id="0b3d8-127">Typ</span><span class="sxs-lookup"><span data-stu-id="0b3d8-127">Type</span></span>|<span data-ttu-id="0b3d8-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0b3d8-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0b3d8-129">id</span><span class="sxs-lookup"><span data-stu-id="0b3d8-129">id</span></span>|<span data-ttu-id="0b3d8-130">String</span><span class="sxs-lookup"><span data-stu-id="0b3d8-130">String</span></span>|<span data-ttu-id="0b3d8-131">Schlüssel der Zuweisung</span><span class="sxs-lookup"><span data-stu-id="0b3d8-131">The key of the assignment.</span></span>|
|<span data-ttu-id="0b3d8-132">target</span><span class="sxs-lookup"><span data-stu-id="0b3d8-132">target</span></span>|[<span data-ttu-id="0b3d8-133">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="0b3d8-133">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune_shared_deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="0b3d8-134">Zuweisungsziel für die Gerätekonfiguration</span><span class="sxs-lookup"><span data-stu-id="0b3d8-134">The assignment target for the device configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="0b3d8-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="0b3d8-135">Response</span></span>
<span data-ttu-id="0b3d8-136">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="0b3d8-136">If successful, this method returns a `201 Created` response code and a [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0b3d8-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0b3d8-137">Example</span></span>
### <a name="request"></a><span data-ttu-id="0b3d8-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0b3d8-138">Request</span></span>
<span data-ttu-id="0b3d8-139">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0b3d8-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments
Content-type: application/json
Content-length: 169

{
  "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="0b3d8-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="0b3d8-140">Response</span></span>
<span data-ttu-id="0b3d8-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0b3d8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



