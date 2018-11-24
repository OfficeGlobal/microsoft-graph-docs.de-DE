# <a name="create-mobileappassignment"></a><span data-ttu-id="578d1-101">Erstellen von „mobileAppAssignment“</span><span class="sxs-lookup"><span data-stu-id="578d1-101">Create mobileAppAssignment</span></span>

> <span data-ttu-id="578d1-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="578d1-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="578d1-103">Diese Methode erstellt ein neues Objekt des Typs [mobileAppAssignment](../resources/intune_apps_mobileappassignment.md).</span><span class="sxs-lookup"><span data-stu-id="578d1-103">Create a new [mobileAppAssignment](../resources/intune_apps_mobileappassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="578d1-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="578d1-104">Prerequisites</span></span>
<span data-ttu-id="578d1-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="578d1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="578d1-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="578d1-107">Permission type</span></span>|<span data-ttu-id="578d1-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="578d1-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="578d1-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="578d1-109">Delegated (work or school account)</span></span>|<span data-ttu-id="578d1-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="578d1-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="578d1-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="578d1-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="578d1-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="578d1-112">Not supported.</span></span>|
|<span data-ttu-id="578d1-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="578d1-113">Application</span></span>|<span data-ttu-id="578d1-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="578d1-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="578d1-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="578d1-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="578d1-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="578d1-116">Request headers</span></span>
|<span data-ttu-id="578d1-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="578d1-117">Header</span></span>|<span data-ttu-id="578d1-118">Wert</span><span class="sxs-lookup"><span data-stu-id="578d1-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="578d1-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="578d1-119">Authorization</span></span>|<span data-ttu-id="578d1-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="578d1-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="578d1-121">Accept</span><span class="sxs-lookup"><span data-stu-id="578d1-121">Accept</span></span>|<span data-ttu-id="578d1-122">application/json</span><span class="sxs-lookup"><span data-stu-id="578d1-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="578d1-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="578d1-123">Request body</span></span>
<span data-ttu-id="578d1-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „mobileAppAssignment“ an.</span><span class="sxs-lookup"><span data-stu-id="578d1-124">In the request body, supply a JSON representation for the mobileAppAssignment object.</span></span>

<span data-ttu-id="578d1-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „mobileAppAssignment“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="578d1-125">The following table shows the properties that are required when you create the mobileAppAssignment.</span></span>

|<span data-ttu-id="578d1-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="578d1-126">Property</span></span>|<span data-ttu-id="578d1-127">Typ</span><span class="sxs-lookup"><span data-stu-id="578d1-127">Type</span></span>|<span data-ttu-id="578d1-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="578d1-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="578d1-129">id</span><span class="sxs-lookup"><span data-stu-id="578d1-129">id</span></span>|<span data-ttu-id="578d1-130">String</span><span class="sxs-lookup"><span data-stu-id="578d1-130">String</span></span>|<span data-ttu-id="578d1-131">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="578d1-131">Key of the entity.</span></span>|
|<span data-ttu-id="578d1-132">intent</span><span class="sxs-lookup"><span data-stu-id="578d1-132">intent</span></span>|[<span data-ttu-id="578d1-133">installIntent</span><span class="sxs-lookup"><span data-stu-id="578d1-133">installIntent</span></span>](../resources/intune_shared_installintent.md)|<span data-ttu-id="578d1-134">Die vom Administrator definierte Installationspriorität. Mögliche Werte sind: `available`, `required`, `uninstall` und `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="578d1-134">The install intent defined by the admin. Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|
|<span data-ttu-id="578d1-135">target</span><span class="sxs-lookup"><span data-stu-id="578d1-135">target</span></span>|[<span data-ttu-id="578d1-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="578d1-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune_shared_deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="578d1-137">Die vom Administrator definierte Zielgruppenzuordnung</span><span class="sxs-lookup"><span data-stu-id="578d1-137">The target group assignment defined by the admin.</span></span>|
|<span data-ttu-id="578d1-138">settings</span><span class="sxs-lookup"><span data-stu-id="578d1-138">settings</span></span>|[<span data-ttu-id="578d1-139">mobileAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="578d1-139">mobileAppAssignmentSettings</span></span>](../resources/intune_apps_mobileappassignmentsettings.md)|<span data-ttu-id="578d1-140">Die vom Administrator definierten Einstellungen für die Zielgruppenzuordnung</span><span class="sxs-lookup"><span data-stu-id="578d1-140">The settings for target assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="578d1-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="578d1-141">Response</span></span>
<span data-ttu-id="578d1-142">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [mobileAppAssignment](../resources/intune_apps_mobileappassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="578d1-142">If successful, this method returns a `201 Created` response code and a [mobileAppAssignment](../resources/intune_apps_mobileappassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="578d1-143">Beispiel</span><span class="sxs-lookup"><span data-stu-id="578d1-143">Example</span></span>
### <a name="request"></a><span data-ttu-id="578d1-144">Anforderung</span><span class="sxs-lookup"><span data-stu-id="578d1-144">Request</span></span>
<span data-ttu-id="578d1-145">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="578d1-145">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/assignments
Content-type: application/json
Content-length: 273

{
  "@odata.type": "#microsoft.graph.mobileAppAssignment",
  "intent": "required",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "settings": {
    "@odata.type": "microsoft.graph.mobileAppAssignmentSettings"
  }
}
```

### <a name="response"></a><span data-ttu-id="578d1-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="578d1-146">Response</span></span>
<span data-ttu-id="578d1-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="578d1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 322

{
  "@odata.type": "#microsoft.graph.mobileAppAssignment",
  "id": "591620b7-20b7-5916-b720-1659b7201659",
  "intent": "required",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "settings": {
    "@odata.type": "microsoft.graph.mobileAppAssignmentSettings"
  }
}
```



