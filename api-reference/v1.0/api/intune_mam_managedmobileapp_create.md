# <a name="create-managedmobileapp"></a><span data-ttu-id="93896-101">Erstellen von „managedMobileApp“</span><span class="sxs-lookup"><span data-stu-id="93896-101">Create managedMobileApp</span></span>

> <span data-ttu-id="93896-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="93896-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="93896-103">Diese Methode erstellt ein neues Objekt des Typs [managedMobileApp](../resources/intune_mam_managedmobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="93896-103">Create a new [plannerBucket](../resources/intune_mam_managedmobileapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="93896-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="93896-104">Prerequisites</span></span>
<span data-ttu-id="93896-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="93896-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="93896-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="93896-107">Permission type</span></span>|<span data-ttu-id="93896-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="93896-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="93896-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="93896-109">Delegated (work or school account)</span></span>|<span data-ttu-id="93896-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93896-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="93896-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="93896-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="93896-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="93896-112">Not supported.</span></span>|
|<span data-ttu-id="93896-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="93896-113">Application</span></span>|<span data-ttu-id="93896-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="93896-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="93896-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="93896-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/apps
POST /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}/apps
POST /deviceAppManagement/defaultManagedAppProtections/{defaultManagedAppProtectionId}/apps
POST /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/apps
```

## <a name="request-headers"></a><span data-ttu-id="93896-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="93896-116">Request headers</span></span>
|<span data-ttu-id="93896-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="93896-117">Header</span></span>|<span data-ttu-id="93896-118">Wert</span><span class="sxs-lookup"><span data-stu-id="93896-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="93896-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="93896-119">Authorization</span></span>|<span data-ttu-id="93896-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="93896-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="93896-121">Accept</span><span class="sxs-lookup"><span data-stu-id="93896-121">Accept</span></span>|<span data-ttu-id="93896-122">application/json</span><span class="sxs-lookup"><span data-stu-id="93896-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="93896-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="93896-123">Request body</span></span>
<span data-ttu-id="93896-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „managedMobileApp“ an.</span><span class="sxs-lookup"><span data-stu-id="93896-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="93896-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „managedMobileApp“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="93896-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="93896-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="93896-126">Property</span></span>|<span data-ttu-id="93896-127">Typ</span><span class="sxs-lookup"><span data-stu-id="93896-127">Type</span></span>|<span data-ttu-id="93896-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="93896-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="93896-129">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="93896-129">mobileAppIdentifier</span></span>|[<span data-ttu-id="93896-130">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="93896-130">mobileAppIdentifier</span></span>](../resources/intune_mam_mobileappidentifier.md)|<span data-ttu-id="93896-131">Bezeichner der App mit dem zugehörigen Betriebssystemtyp</span><span class="sxs-lookup"><span data-stu-id="93896-131">The identifier for an app with it's operating system type.</span></span>|
|<span data-ttu-id="93896-132">id</span><span class="sxs-lookup"><span data-stu-id="93896-132">id</span></span>|<span data-ttu-id="93896-133">String</span><span class="sxs-lookup"><span data-stu-id="93896-133">String</span></span>|<span data-ttu-id="93896-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="93896-134">Key of the setting.</span></span>|
|<span data-ttu-id="93896-135">version</span><span class="sxs-lookup"><span data-stu-id="93896-135">version</span></span>|<span data-ttu-id="93896-136">String</span><span class="sxs-lookup"><span data-stu-id="93896-136">String</span></span>|<span data-ttu-id="93896-137">Version der Entität</span><span class="sxs-lookup"><span data-stu-id="93896-137">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="93896-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="93896-138">Response</span></span>
<span data-ttu-id="93896-139">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [managedMobileApp](../resources/intune_mam_managedmobileapp.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="93896-139">If successful, this method returns a `201 Created` response code and a [section](../resources/intune_mam_managedmobileapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="93896-140">Beispiel</span><span class="sxs-lookup"><span data-stu-id="93896-140">Example</span></span>
### <a name="request"></a><span data-ttu-id="93896-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="93896-141">Request</span></span>
<span data-ttu-id="93896-142">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="93896-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/apps
Content-type: application/json
Content-length: 181

{
  "@odata.type": "#microsoft.graph.managedMobileApp",
  "mobileAppIdentifier": {
    "@odata.type": "microsoft.graph.mobileAppIdentifier"
  },
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="93896-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="93896-143">Response</span></span>
<span data-ttu-id="93896-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="93896-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 230

{
  "@odata.type": "#microsoft.graph.managedMobileApp",
  "mobileAppIdentifier": {
    "@odata.type": "microsoft.graph.mobileAppIdentifier"
  },
  "id": "0a129715-9715-0a12-1597-120a1597120a",
  "version": "Version value"
}
```



