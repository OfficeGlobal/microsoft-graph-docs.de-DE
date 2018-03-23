# <a name="update-manageddevicemobileappconfigurationassignment"></a><span data-ttu-id="5b3b0-101">Aktualisieren von „managedDeviceMobileAppConfigurationAssignment“</span><span class="sxs-lookup"><span data-stu-id="5b3b0-101">Update managedDeviceMobileAppConfigurationAssignment</span></span>

> <span data-ttu-id="5b3b0-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="5b3b0-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5b3b0-103">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [managedDeviceMobileAppConfigurationAssignment](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="5b3b0-103">Update the properties of a [calendar](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5b3b0-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="5b3b0-104">Prerequisites</span></span>
<span data-ttu-id="5b3b0-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="5b3b0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="5b3b0-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5b3b0-107">Permission type</span></span>|<span data-ttu-id="5b3b0-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5b3b0-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5b3b0-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5b3b0-109">Delegated (work or school account)</span></span>|<span data-ttu-id="5b3b0-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5b3b0-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="5b3b0-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5b3b0-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5b3b0-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5b3b0-112">Not supported.</span></span>|
|<span data-ttu-id="5b3b0-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5b3b0-113">Application</span></span>|<span data-ttu-id="5b3b0-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5b3b0-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5b3b0-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5b3b0-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments/{managedDeviceMobileAppConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="5b3b0-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5b3b0-116">Request headers</span></span>
|<span data-ttu-id="5b3b0-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="5b3b0-117">Header</span></span>|<span data-ttu-id="5b3b0-118">Wert</span><span class="sxs-lookup"><span data-stu-id="5b3b0-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5b3b0-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="5b3b0-119">Authorization</span></span>|<span data-ttu-id="5b3b0-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="5b3b0-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="5b3b0-121">Accept</span><span class="sxs-lookup"><span data-stu-id="5b3b0-121">Accept</span></span>|<span data-ttu-id="5b3b0-122">application/json</span><span class="sxs-lookup"><span data-stu-id="5b3b0-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5b3b0-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5b3b0-123">Request body</span></span>
<span data-ttu-id="5b3b0-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [managedDeviceMobileAppConfigurationAssignment](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md) an.</span><span class="sxs-lookup"><span data-stu-id="5b3b0-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md) object.</span></span>

<span data-ttu-id="5b3b0-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [managedDeviceMobileAppConfigurationAssignment](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="5b3b0-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="5b3b0-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5b3b0-126">Property</span></span>|<span data-ttu-id="5b3b0-127">Typ</span><span class="sxs-lookup"><span data-stu-id="5b3b0-127">Type</span></span>|<span data-ttu-id="5b3b0-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5b3b0-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5b3b0-129">id</span><span class="sxs-lookup"><span data-stu-id="5b3b0-129">id</span></span>|<span data-ttu-id="5b3b0-130">String</span><span class="sxs-lookup"><span data-stu-id="5b3b0-130">String</span></span>|<span data-ttu-id="5b3b0-131">Eindeutiger Bezeichner der Entität</span><span class="sxs-lookup"><span data-stu-id="5b3b0-131">Unique identifier of the folder.</span></span>|
|<span data-ttu-id="5b3b0-132">target</span><span class="sxs-lookup"><span data-stu-id="5b3b0-132">target</span></span>|[<span data-ttu-id="5b3b0-133">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="5b3b0-133">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune_apps_deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="5b3b0-134">Zuweisungsziel, dem die Geschäftsbedingungen-Richtlinie zugewiesen ist</span><span class="sxs-lookup"><span data-stu-id="5b3b0-134">Assignment target that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="5b3b0-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="5b3b0-135">Response</span></span>
<span data-ttu-id="5b3b0-136">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [managedDeviceMobileAppConfigurationAssignment](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="5b3b0-136">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5b3b0-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5b3b0-137">Example</span></span>
### <a name="request"></a><span data-ttu-id="5b3b0-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5b3b0-138">Request</span></span>
<span data-ttu-id="5b3b0-139">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5b3b0-139">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments/{managedDeviceMobileAppConfigurationAssignmentId}
Content-type: application/json
Content-length: 101

{
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="5b3b0-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="5b3b0-140">Response</span></span>
<span data-ttu-id="5b3b0-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5b3b0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



