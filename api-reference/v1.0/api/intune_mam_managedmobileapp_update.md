# <a name="update-managedmobileapp"></a><span data-ttu-id="b43c4-101">Aktualisieren von „managedMobileApp“</span><span class="sxs-lookup"><span data-stu-id="b43c4-101">Update managedMobileApp</span></span>

> <span data-ttu-id="b43c4-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="b43c4-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b43c4-103">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [managedMobileApp](../resources/intune_mam_managedmobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b43c4-103">Update the properties of a [managedMobileApp](../resources/intune_mam_managedmobileapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b43c4-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b43c4-104">Prerequisites</span></span>
<span data-ttu-id="b43c4-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b43c4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b43c4-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b43c4-107">Permission type</span></span>|<span data-ttu-id="b43c4-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b43c4-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b43c4-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b43c4-109">Delegated (work or school account)</span></span>|<span data-ttu-id="b43c4-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b43c4-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b43c4-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b43c4-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b43c4-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b43c4-112">Not supported.</span></span>|
|<span data-ttu-id="b43c4-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b43c4-113">Application</span></span>|<span data-ttu-id="b43c4-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b43c4-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b43c4-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b43c4-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/apps/{managedMobileAppId}
PATCH /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}/apps/{managedMobileAppId}
PATCH /deviceAppManagement/defaultManagedAppProtections/{defaultManagedAppProtectionId}/apps/{managedMobileAppId}
PATCH /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/apps/{managedMobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="b43c4-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b43c4-116">Request headers</span></span>
|<span data-ttu-id="b43c4-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="b43c4-117">Header</span></span>|<span data-ttu-id="b43c4-118">Wert</span><span class="sxs-lookup"><span data-stu-id="b43c4-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b43c4-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="b43c4-119">Authorization</span></span>|<span data-ttu-id="b43c4-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b43c4-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b43c4-121">Accept</span><span class="sxs-lookup"><span data-stu-id="b43c4-121">Accept</span></span>|<span data-ttu-id="b43c4-122">application/json</span><span class="sxs-lookup"><span data-stu-id="b43c4-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b43c4-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b43c4-123">Request body</span></span>
<span data-ttu-id="b43c4-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [managedMobileApp](../resources/intune_mam_managedmobileapp.md) an.</span><span class="sxs-lookup"><span data-stu-id="b43c4-124">In the request body, supply a JSON representation for the [managedMobileApp](../resources/intune_mam_managedmobileapp.md) object.</span></span>

<span data-ttu-id="b43c4-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [managedMobileApp](../resources/intune_mam_managedmobileapp.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="b43c4-125">The following table shows the properties that are required when you create the [managedMobileApp](../resources/intune_mam_managedmobileapp.md).</span></span>

|<span data-ttu-id="b43c4-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b43c4-126">Property</span></span>|<span data-ttu-id="b43c4-127">Typ</span><span class="sxs-lookup"><span data-stu-id="b43c4-127">Type</span></span>|<span data-ttu-id="b43c4-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b43c4-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b43c4-129">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="b43c4-129">mobileAppIdentifier</span></span>|[<span data-ttu-id="b43c4-130">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="b43c4-130">mobileAppIdentifier</span></span>](../resources/intune_mam_mobileappidentifier.md)|<span data-ttu-id="b43c4-131">Bezeichner für eine App mit dem zugehörigen Betriebssystemtyp</span><span class="sxs-lookup"><span data-stu-id="b43c4-131">The identifier for an app with it's operating system type.</span></span>|
|<span data-ttu-id="b43c4-132">id</span><span class="sxs-lookup"><span data-stu-id="b43c4-132">id</span></span>|<span data-ttu-id="b43c4-133">String</span><span class="sxs-lookup"><span data-stu-id="b43c4-133">String</span></span>|<span data-ttu-id="b43c4-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="b43c4-134">Key of the entity.</span></span>|
|<span data-ttu-id="b43c4-135">version</span><span class="sxs-lookup"><span data-stu-id="b43c4-135">version</span></span>|<span data-ttu-id="b43c4-136">String</span><span class="sxs-lookup"><span data-stu-id="b43c4-136">String</span></span>|<span data-ttu-id="b43c4-137">Version der Entität</span><span class="sxs-lookup"><span data-stu-id="b43c4-137">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="b43c4-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="b43c4-138">Response</span></span>
<span data-ttu-id="b43c4-139">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [managedMobileApp](../resources/intune_mam_managedmobileapp.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="b43c4-139">If successful, this method returns a `200 OK` response code and an updated [managedMobileApp](../resources/intune_mam_managedmobileapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b43c4-140">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b43c4-140">Example</span></span>
### <a name="request"></a><span data-ttu-id="b43c4-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b43c4-141">Request</span></span>
<span data-ttu-id="b43c4-142">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b43c4-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/apps/{managedMobileAppId}
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

### <a name="response"></a><span data-ttu-id="b43c4-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="b43c4-143">Response</span></span>
<span data-ttu-id="b43c4-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b43c4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



