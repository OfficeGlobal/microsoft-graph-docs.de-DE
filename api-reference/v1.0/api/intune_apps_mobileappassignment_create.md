# <a name="create-mobileappassignment"></a><span data-ttu-id="5ebbb-101">Erstellen von „mobileAppAssignment“</span><span class="sxs-lookup"><span data-stu-id="5ebbb-101">Create mobileAppAssignment</span></span>

> <span data-ttu-id="5ebbb-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="5ebbb-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5ebbb-103">Diese Methode erstellt ein neues Objekt des Typs [mobileAppAssignment](../resources/intune_apps_mobileappassignment.md).</span><span class="sxs-lookup"><span data-stu-id="5ebbb-103">Create a new [mobileAppAssignment](../resources/intune_apps_mobileappassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5ebbb-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="5ebbb-104">Prerequisites</span></span>
<span data-ttu-id="5ebbb-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="5ebbb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="5ebbb-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5ebbb-107">Permission type</span></span>|<span data-ttu-id="5ebbb-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5ebbb-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5ebbb-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5ebbb-109">Delegated (work or school account)</span></span>|<span data-ttu-id="5ebbb-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ebbb-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="5ebbb-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5ebbb-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5ebbb-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5ebbb-112">Not supported.</span></span>|
|<span data-ttu-id="5ebbb-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5ebbb-113">Application</span></span>|<span data-ttu-id="5ebbb-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5ebbb-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5ebbb-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5ebbb-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="5ebbb-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5ebbb-116">Request headers</span></span>
|<span data-ttu-id="5ebbb-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="5ebbb-117">Header</span></span>|<span data-ttu-id="5ebbb-118">Wert</span><span class="sxs-lookup"><span data-stu-id="5ebbb-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5ebbb-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="5ebbb-119">Authorization</span></span>|<span data-ttu-id="5ebbb-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="5ebbb-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5ebbb-121">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="5ebbb-121">Accept</span></span>|<span data-ttu-id="5ebbb-122">Anwendung/json</span><span class="sxs-lookup"><span data-stu-id="5ebbb-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5ebbb-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5ebbb-123">Request body</span></span>
<span data-ttu-id="5ebbb-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „mobileAppAssignment“ an.</span><span class="sxs-lookup"><span data-stu-id="5ebbb-124">In the request body, supply a JSON representation for the mobileAppAssignment object.</span></span>

<span data-ttu-id="5ebbb-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „mobileAppAssignment“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="5ebbb-125">The following table shows the properties that are required when you create the mobileAppAssignment.</span></span>

|<span data-ttu-id="5ebbb-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5ebbb-126">Property</span></span>|<span data-ttu-id="5ebbb-127">Typ</span><span class="sxs-lookup"><span data-stu-id="5ebbb-127">Type</span></span>|<span data-ttu-id="5ebbb-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5ebbb-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5ebbb-129">id</span><span class="sxs-lookup"><span data-stu-id="5ebbb-129">id</span></span>|<span data-ttu-id="5ebbb-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5ebbb-130">String</span></span>|<span data-ttu-id="5ebbb-131">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="5ebbb-131">Key of the entity.</span></span>|
|<span data-ttu-id="5ebbb-132">intent</span><span class="sxs-lookup"><span data-stu-id="5ebbb-132">intent</span></span>|[<span data-ttu-id="5ebbb-133">installIntent</span><span class="sxs-lookup"><span data-stu-id="5ebbb-133">installIntent</span></span>](../resources/intune_shared_installintent.md)|<span data-ttu-id="5ebbb-134">Die durch den Administrator definierten Install-Intent. Die möglichen Werte sind: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="5ebbb-134">The install intent defined by the admin. Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|
|<span data-ttu-id="5ebbb-135">Ziel</span><span class="sxs-lookup"><span data-stu-id="5ebbb-135">target</span></span>|[<span data-ttu-id="5ebbb-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="5ebbb-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune_shared_deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="5ebbb-137">Die vom Administrator definierte Zielgruppenzuordnung</span><span class="sxs-lookup"><span data-stu-id="5ebbb-137">The target group assignment defined by the admin.</span></span>|
|<span data-ttu-id="5ebbb-138">Einstellungen</span><span class="sxs-lookup"><span data-stu-id="5ebbb-138">settings</span></span>|[<span data-ttu-id="5ebbb-139">mobileAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="5ebbb-139">mobileAppAssignmentSettings</span></span>](../resources/intune_apps_mobileappassignmentsettings.md)|<span data-ttu-id="5ebbb-140">Die vom Administrator definierten Einstellungen für die Zielgruppenzuordnung</span><span class="sxs-lookup"><span data-stu-id="5ebbb-140">The settings for target assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="5ebbb-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="5ebbb-141">Response</span></span>
<span data-ttu-id="5ebbb-142">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [mobileAppAssignment](../resources/intune_apps_mobileappassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="5ebbb-142">If successful, this method returns a `201 Created` response code and a [mobileAppAssignment](../resources/intune_apps_mobileappassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5ebbb-143">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5ebbb-143">Example</span></span>
### <a name="request"></a><span data-ttu-id="5ebbb-144">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5ebbb-144">Request</span></span>
<span data-ttu-id="5ebbb-145">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5ebbb-145">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5ebbb-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="5ebbb-146">Response</span></span>
<span data-ttu-id="5ebbb-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5ebbb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



