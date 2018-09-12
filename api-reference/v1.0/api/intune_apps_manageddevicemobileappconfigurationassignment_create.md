# <a name="create-manageddevicemobileappconfigurationassignment"></a><span data-ttu-id="6548f-101">Erstellen von „managedDeviceMobileAppConfigurationAssignment“</span><span class="sxs-lookup"><span data-stu-id="6548f-101">Create managedDeviceMobileAppConfigurationAssignment</span></span>

> <span data-ttu-id="6548f-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="6548f-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6548f-103">Diese Methode erstellt ein neues Objekt des Typs [managedDeviceMobileAppConfigurationAssignment](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="6548f-103">Create a new [managedDeviceMobileAppConfigurationAssignment](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6548f-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="6548f-104">Prerequisites</span></span>
<span data-ttu-id="6548f-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="6548f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="6548f-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6548f-107">Permission type</span></span>|<span data-ttu-id="6548f-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6548f-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6548f-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6548f-109">Delegated (work or school account)</span></span>|<span data-ttu-id="6548f-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6548f-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="6548f-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6548f-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6548f-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6548f-112">Not supported.</span></span>|
|<span data-ttu-id="6548f-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6548f-113">Application</span></span>|<span data-ttu-id="6548f-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6548f-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6548f-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6548f-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="6548f-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6548f-116">Request headers</span></span>
|<span data-ttu-id="6548f-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="6548f-117">Header</span></span>|<span data-ttu-id="6548f-118">Wert</span><span class="sxs-lookup"><span data-stu-id="6548f-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6548f-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="6548f-119">Authorization</span></span>|<span data-ttu-id="6548f-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="6548f-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6548f-121">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="6548f-121">Accept</span></span>|<span data-ttu-id="6548f-122">application/json</span><span class="sxs-lookup"><span data-stu-id="6548f-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6548f-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6548f-123">Request body</span></span>
<span data-ttu-id="6548f-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „managedDeviceMobileAppConfigurationAssignment“ an.</span><span class="sxs-lookup"><span data-stu-id="6548f-124">In the request body, supply a JSON representation for the managedDeviceMobileAppConfigurationAssignment object.</span></span>

<span data-ttu-id="6548f-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „managedDeviceMobileAppConfigurationAssignment“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="6548f-125">The following table shows the properties that are required when you create the managedDeviceMobileAppConfigurationAssignment.</span></span>

|<span data-ttu-id="6548f-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6548f-126">Property</span></span>|<span data-ttu-id="6548f-127">Typ</span><span class="sxs-lookup"><span data-stu-id="6548f-127">Type</span></span>|<span data-ttu-id="6548f-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6548f-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6548f-129">ID</span><span class="sxs-lookup"><span data-stu-id="6548f-129">id</span></span>|<span data-ttu-id="6548f-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6548f-130">String</span></span>|<span data-ttu-id="6548f-131">Eindeutiger Bezeichner der Entität</span><span class="sxs-lookup"><span data-stu-id="6548f-131">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="6548f-132">Ziel</span><span class="sxs-lookup"><span data-stu-id="6548f-132">target</span></span>|[<span data-ttu-id="6548f-133">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="6548f-133">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune_shared_deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="6548f-134">Zuweisungsziel, dem die Geschäftsbedingungen-Richtlinie zugewiesen ist</span><span class="sxs-lookup"><span data-stu-id="6548f-134">Assignment target that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="6548f-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="6548f-135">Response</span></span>
<span data-ttu-id="6548f-136">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [managedDeviceMobileAppConfigurationAssignment](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="6548f-136">If successful, this method returns a `201 Created` response code and a [managedDeviceMobileAppConfigurationAssignment](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6548f-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6548f-137">Example</span></span>
### <a name="request"></a><span data-ttu-id="6548f-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6548f-138">Request</span></span>
<span data-ttu-id="6548f-139">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6548f-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments
Content-type: application/json
Content-length: 185

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="6548f-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="6548f-140">Response</span></span>
<span data-ttu-id="6548f-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6548f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 234

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationAssignment",
  "id": "4df81c9c-1c9c-4df8-9c1c-f84d9c1cf84d",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```








