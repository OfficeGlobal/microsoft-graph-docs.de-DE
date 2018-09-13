# <a name="update-mobileappassignment"></a><span data-ttu-id="1385c-101">Aktualisieren von „mobileAppAssignment“</span><span class="sxs-lookup"><span data-stu-id="1385c-101">Update mobileAppAssignment</span></span>

> <span data-ttu-id="1385c-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="1385c-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1385c-103">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [mobileAppAssignment](../resources/intune_apps_mobileappassignment.md).</span><span class="sxs-lookup"><span data-stu-id="1385c-103">Update the properties of a [mobileAppAssignment](../resources/intune_apps_mobileappassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1385c-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="1385c-104">Prerequisites</span></span>
<span data-ttu-id="1385c-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="1385c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="1385c-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1385c-107">Permission type</span></span>|<span data-ttu-id="1385c-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1385c-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1385c-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1385c-109">Delegated (work or school account)</span></span>|<span data-ttu-id="1385c-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1385c-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1385c-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1385c-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1385c-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1385c-112">Not supported.</span></span>|
|<span data-ttu-id="1385c-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1385c-113">Application</span></span>|<span data-ttu-id="1385c-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1385c-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1385c-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1385c-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/assignments/{mobileAppAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="1385c-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1385c-116">Request headers</span></span>
|<span data-ttu-id="1385c-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="1385c-117">Header</span></span>|<span data-ttu-id="1385c-118">Wert</span><span class="sxs-lookup"><span data-stu-id="1385c-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1385c-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="1385c-119">Authorization</span></span>|<span data-ttu-id="1385c-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="1385c-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1385c-121">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="1385c-121">Accept</span></span>|<span data-ttu-id="1385c-122">Anwendung/json</span><span class="sxs-lookup"><span data-stu-id="1385c-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1385c-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1385c-123">Request body</span></span>
<span data-ttu-id="1385c-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [mobileAppAssignment](../resources/intune_apps_mobileappassignment.md) an.</span><span class="sxs-lookup"><span data-stu-id="1385c-124">In the request body, supply a JSON representation for the [mobileAppAssignment](../resources/intune_apps_mobileappassignment.md) object.</span></span>

<span data-ttu-id="1385c-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [mobileAppAssignment](../resources/intune_apps_mobileappassignment.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="1385c-125">The following table shows the properties that are required when you create the [mobileAppAssignment](../resources/intune_apps_mobileappassignment.md).</span></span>

|<span data-ttu-id="1385c-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1385c-126">Property</span></span>|<span data-ttu-id="1385c-127">Typ</span><span class="sxs-lookup"><span data-stu-id="1385c-127">Type</span></span>|<span data-ttu-id="1385c-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1385c-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1385c-129">id</span><span class="sxs-lookup"><span data-stu-id="1385c-129">id</span></span>|<span data-ttu-id="1385c-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1385c-130">String</span></span>|<span data-ttu-id="1385c-131">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="1385c-131">Key of the entity.</span></span>|
|<span data-ttu-id="1385c-132">intent</span><span class="sxs-lookup"><span data-stu-id="1385c-132">intent</span></span>|[<span data-ttu-id="1385c-133">installIntent</span><span class="sxs-lookup"><span data-stu-id="1385c-133">installIntent</span></span>](../resources/intune_shared_installintent.md)|<span data-ttu-id="1385c-134">Die vom Administrator definierte Installationspriorität. Mögliche Werte sind: `available`, `required`, `uninstall` und `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="1385c-134">The install intent defined by the admin. Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|
|<span data-ttu-id="1385c-135">target</span><span class="sxs-lookup"><span data-stu-id="1385c-135">target</span></span>|[<span data-ttu-id="1385c-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="1385c-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune_shared_deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="1385c-137">Die vom Administrator definierte Zielgruppenzuordnung</span><span class="sxs-lookup"><span data-stu-id="1385c-137">The target group assignment defined by the admin.</span></span>|
|<span data-ttu-id="1385c-138">Einstellungen</span><span class="sxs-lookup"><span data-stu-id="1385c-138">settings</span></span>|[<span data-ttu-id="1385c-139">mobileAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="1385c-139">mobileAppAssignmentSettings</span></span>](../resources/intune_apps_mobileappassignmentsettings.md)|<span data-ttu-id="1385c-140">Die vom Administrator definierten Einstellungen für die Zielgruppenzuordnung</span><span class="sxs-lookup"><span data-stu-id="1385c-140">The settings for target assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="1385c-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="1385c-141">Response</span></span>
<span data-ttu-id="1385c-142">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [mobileAppAssignment](../resources/intune_apps_mobileappassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="1385c-142">If successful, this method returns a `200 OK` response code and an updated [mobileAppAssignment](../resources/intune_apps_mobileappassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1385c-143">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1385c-143">Example</span></span>
### <a name="request"></a><span data-ttu-id="1385c-144">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1385c-144">Request</span></span>
<span data-ttu-id="1385c-145">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1385c-145">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/assignments/{mobileAppAssignmentId}
Content-type: application/json
Content-length: 215

{
  "intent": "required",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "settings": {
    "@odata.type": "microsoft.graph.mobileAppAssignmentSettings"
  }
}
```

### <a name="response"></a><span data-ttu-id="1385c-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="1385c-146">Response</span></span>
<span data-ttu-id="1385c-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1385c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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








