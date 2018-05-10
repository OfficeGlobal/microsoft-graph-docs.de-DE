# <a name="update-androidmanagedappregistration"></a><span data-ttu-id="0523e-101">Aktualisieren von „androidManagedAppRegistration“</span><span class="sxs-lookup"><span data-stu-id="0523e-101">Update androidManagedAppRegistration</span></span>

> <span data-ttu-id="0523e-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="0523e-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0523e-103">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [androidManagedAppRegistration](../resources/intune_mam_androidmanagedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="0523e-103">Update the properties of a [androidManagedAppRegistration](../resources/intune_mam_androidmanagedappregistration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0523e-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="0523e-104">Prerequisites</span></span>
<span data-ttu-id="0523e-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="0523e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="0523e-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0523e-107">Permission type</span></span>|<span data-ttu-id="0523e-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0523e-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0523e-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0523e-109">Delegated (work or school account)</span></span>|<span data-ttu-id="0523e-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0523e-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0523e-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0523e-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0523e-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0523e-112">Not supported.</span></span>|
|<span data-ttu-id="0523e-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0523e-113">Application</span></span>|<span data-ttu-id="0523e-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0523e-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0523e-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0523e-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}
```

## <a name="request-headers"></a><span data-ttu-id="0523e-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0523e-116">Request headers</span></span>
|<span data-ttu-id="0523e-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="0523e-117">Header</span></span>|<span data-ttu-id="0523e-118">Wert</span><span class="sxs-lookup"><span data-stu-id="0523e-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0523e-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="0523e-119">Authorization</span></span>|<span data-ttu-id="0523e-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="0523e-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0523e-121">Accept</span><span class="sxs-lookup"><span data-stu-id="0523e-121">Accept</span></span>|<span data-ttu-id="0523e-122">application/json</span><span class="sxs-lookup"><span data-stu-id="0523e-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0523e-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0523e-123">Request body</span></span>
<span data-ttu-id="0523e-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [androidManagedAppRegistration](../resources/intune_mam_androidmanagedappregistration.md) an.</span><span class="sxs-lookup"><span data-stu-id="0523e-124">In the request body, supply a JSON representation for the [androidManagedAppRegistration](../resources/intune_mam_androidmanagedappregistration.md) object.</span></span>

<span data-ttu-id="0523e-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [androidManagedAppRegistration](../resources/intune_mam_androidmanagedappregistration.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="0523e-125">The following table shows the properties that are required when you create the [androidManagedAppRegistration](../resources/intune_mam_androidmanagedappregistration.md).</span></span>

|<span data-ttu-id="0523e-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0523e-126">Property</span></span>|<span data-ttu-id="0523e-127">Typ</span><span class="sxs-lookup"><span data-stu-id="0523e-127">Type</span></span>|<span data-ttu-id="0523e-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0523e-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0523e-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0523e-129">createdDateTime</span></span>|<span data-ttu-id="0523e-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0523e-130">DateTimeOffset</span></span>|<span data-ttu-id="0523e-131">Datum und Uhrzeit der Erstellung. Geerbt von [managedAppRegistration](../resources/intune_mam_managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="0523e-131">Date and time of creation Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="0523e-132">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="0523e-132">lastSyncDateTime</span></span>|<span data-ttu-id="0523e-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0523e-133">DateTimeOffset</span></span>|<span data-ttu-id="0523e-134">Datum und Uhrzeit der letzten Synchronisierung der App mit dem Verwaltungsdienst.</span><span class="sxs-lookup"><span data-stu-id="0523e-134">Date and time of last the app synced with management service.</span></span> <span data-ttu-id="0523e-135">Geerbt von [managedAppRegistration](../resources/intune_mam_managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="0523e-135">Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="0523e-136">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="0523e-136">applicationVersion</span></span>|<span data-ttu-id="0523e-137">String</span><span class="sxs-lookup"><span data-stu-id="0523e-137">String</span></span>|<span data-ttu-id="0523e-138">App-Version. Geerbt von [managedAppRegistration](../resources/intune_mam_managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="0523e-138">App version Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="0523e-139">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="0523e-139">managementSdkVersion</span></span>|<span data-ttu-id="0523e-140">String</span><span class="sxs-lookup"><span data-stu-id="0523e-140">String</span></span>|<span data-ttu-id="0523e-141">Version des App-Verwaltungs-SDK. Geerbt von [managedAppRegistration](../resources/intune_mam_managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="0523e-141">App management SDK version Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="0523e-142">platformVersion</span><span class="sxs-lookup"><span data-stu-id="0523e-142">platformVersion</span></span>|<span data-ttu-id="0523e-143">String</span><span class="sxs-lookup"><span data-stu-id="0523e-143">String</span></span>|<span data-ttu-id="0523e-144">Version des Betriebssystems. Geerbt von [managedAppRegistration](../resources/intune_mam_managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="0523e-144">Operating System version Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="0523e-145">deviceType</span><span class="sxs-lookup"><span data-stu-id="0523e-145">deviceType</span></span>|<span data-ttu-id="0523e-146">String</span><span class="sxs-lookup"><span data-stu-id="0523e-146">String</span></span>|<span data-ttu-id="0523e-147">Gerätetyp des Hostgeräts. Geerbt von [managedAppRegistration](../resources/intune_mam_managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="0523e-147">Host device type Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="0523e-148">deviceTag</span><span class="sxs-lookup"><span data-stu-id="0523e-148">deviceTag</span></span>|<span data-ttu-id="0523e-149">String</span><span class="sxs-lookup"><span data-stu-id="0523e-149">String</span></span>|<span data-ttu-id="0523e-150">Vom App-Verwaltungs-SDK generiertes Tag, das bei der Zuordnung von Apps hilft, die auf demselben Gerät gehostet werden.</span><span class="sxs-lookup"><span data-stu-id="0523e-150">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="0523e-151">Es ist nicht garantiert, dass die App-Zuordnung unter allen Bedingungen funktioniert.</span><span class="sxs-lookup"><span data-stu-id="0523e-151">Not guaranteed to relate apps in all conditions.</span></span> <span data-ttu-id="0523e-152">Geerbt von [managedAppRegistration](../resources/intune_mam_managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="0523e-152">Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="0523e-153">deviceName</span><span class="sxs-lookup"><span data-stu-id="0523e-153">deviceName</span></span>|<span data-ttu-id="0523e-154">String</span><span class="sxs-lookup"><span data-stu-id="0523e-154">String</span></span>|<span data-ttu-id="0523e-155">Gerätename des Hostgeräts. Geerbt von [managedAppRegistration](../resources/intune_mam_managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="0523e-155">Host device name Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="0523e-156">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="0523e-156">flaggedReasons</span></span>|<span data-ttu-id="0523e-157">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="0523e-157">String collection</span></span>|<span data-ttu-id="0523e-158">Gründe (0 oder mehr), aus denen eine App-Registrierung gekennzeichnet wurde.</span><span class="sxs-lookup"><span data-stu-id="0523e-158">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="0523e-159">Beispiel:</span><span class="sxs-lookup"><span data-stu-id="0523e-159">E.g.</span></span> <span data-ttu-id="0523e-160">Die App wird auf einem gerooteten Gerät ausgeführt. Geerbt von [managedAppRegistration](../resources/intune_mam_managedappregistration.md). Mögliche Werte sind: `none` und `rootedDevice`.</span><span class="sxs-lookup"><span data-stu-id="0523e-160">app running on rooted device Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md) Possible values are: `none`, `rootedDevice`.</span></span>|
|<span data-ttu-id="0523e-161">userId</span><span class="sxs-lookup"><span data-stu-id="0523e-161">userId</span></span>|<span data-ttu-id="0523e-162">String</span><span class="sxs-lookup"><span data-stu-id="0523e-162">String</span></span>|<span data-ttu-id="0523e-163">Benutzer-ID, zu der die App-Registrierung gehört.</span><span class="sxs-lookup"><span data-stu-id="0523e-163">The user Id to who this app registration belongs.</span></span> <span data-ttu-id="0523e-164">Geerbt von [managedAppRegistration](../resources/intune_mam_managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="0523e-164">Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="0523e-165">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="0523e-165">appIdentifier</span></span>|[<span data-ttu-id="0523e-166">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="0523e-166">mobileAppIdentifier</span></span>](../resources/intune_mam_mobileappidentifier.md)|<span data-ttu-id="0523e-167">Bezeichner des App-Pakets. Geerbt von [managedAppRegistration](../resources/intune_mam_managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="0523e-167">The app package Identifier Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="0523e-168">id</span><span class="sxs-lookup"><span data-stu-id="0523e-168">id</span></span>|<span data-ttu-id="0523e-169">String</span><span class="sxs-lookup"><span data-stu-id="0523e-169">String</span></span>|<span data-ttu-id="0523e-170">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="0523e-170">Key of the entity.</span></span> <span data-ttu-id="0523e-171">Geerbt von [managedAppRegistration](../resources/intune_mam_managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="0523e-171">Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="0523e-172">version</span><span class="sxs-lookup"><span data-stu-id="0523e-172">version</span></span>|<span data-ttu-id="0523e-173">String</span><span class="sxs-lookup"><span data-stu-id="0523e-173">String</span></span>|<span data-ttu-id="0523e-174">Version der Entität.</span><span class="sxs-lookup"><span data-stu-id="0523e-174">Version of the entity.</span></span> <span data-ttu-id="0523e-175">Geerbt von [managedAppRegistration](../resources/intune_mam_managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="0523e-175">Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="0523e-176">Antwort</span><span class="sxs-lookup"><span data-stu-id="0523e-176">Response</span></span>
<span data-ttu-id="0523e-177">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [androidManagedAppRegistration](../resources/intune_mam_androidmanagedappregistration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="0523e-177">If successful, this method returns a `200 OK` response code and an updated [androidManagedAppRegistration](../resources/intune_mam_androidmanagedappregistration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0523e-178">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0523e-178">Example</span></span>
### <a name="request"></a><span data-ttu-id="0523e-179">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0523e-179">Request</span></span>
<span data-ttu-id="0523e-180">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0523e-180">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}
Content-type: application/json
Content-length: 577

{
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "applicationVersion": "Application Version value",
  "managementSdkVersion": "Management Sdk Version value",
  "platformVersion": "Platform Version value",
  "deviceType": "Device Type value",
  "deviceTag": "Device Tag value",
  "deviceName": "Device Name value",
  "flaggedReasons": [
    "rootedDevice"
  ],
  "userId": "User Id value",
  "appIdentifier": {
    "@odata.type": "microsoft.graph.androidMobileAppIdentifier",
    "packageId": "Package Id value"
  },
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="0523e-181">Antwort</span><span class="sxs-lookup"><span data-stu-id="0523e-181">Response</span></span>
<span data-ttu-id="0523e-p108">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0523e-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 753

{
  "@odata.type": "#microsoft.graph.androidManagedAppRegistration",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "applicationVersion": "Application Version value",
  "managementSdkVersion": "Management Sdk Version value",
  "platformVersion": "Platform Version value",
  "deviceType": "Device Type value",
  "deviceTag": "Device Tag value",
  "deviceName": "Device Name value",
  "flaggedReasons": [
    "rootedDevice"
  ],
  "userId": "User Id value",
  "appIdentifier": {
    "@odata.type": "microsoft.graph.androidMobileAppIdentifier",
    "packageId": "Package Id value"
  },
  "id": "0e064997-4997-0e06-9749-060e9749060e",
  "version": "Version value"
}
```



