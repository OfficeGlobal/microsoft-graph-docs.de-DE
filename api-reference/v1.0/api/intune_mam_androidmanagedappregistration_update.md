# <a name="update-androidmanagedappregistration"></a><span data-ttu-id="0645a-101">Aktualisieren von „androidManagedAppRegistration“</span><span class="sxs-lookup"><span data-stu-id="0645a-101">Update androidManagedAppRegistration</span></span>

> <span data-ttu-id="0645a-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="0645a-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0645a-103">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [androidManagedAppRegistration](../resources/intune_mam_androidmanagedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="0645a-103">Update the properties of a [calendar](../resources/intune_mam_androidmanagedappregistration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0645a-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="0645a-104">Prerequisites</span></span>
<span data-ttu-id="0645a-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="0645a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="0645a-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0645a-107">Permission type</span></span>|<span data-ttu-id="0645a-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0645a-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0645a-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0645a-109">Delegated (work or school account)</span></span>|<span data-ttu-id="0645a-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0645a-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0645a-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0645a-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0645a-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0645a-112">Not supported.</span></span>|
|<span data-ttu-id="0645a-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0645a-113">Application</span></span>|<span data-ttu-id="0645a-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0645a-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0645a-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0645a-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}
```

## <a name="request-headers"></a><span data-ttu-id="0645a-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0645a-116">Request headers</span></span>
|<span data-ttu-id="0645a-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="0645a-117">Header</span></span>|<span data-ttu-id="0645a-118">Wert</span><span class="sxs-lookup"><span data-stu-id="0645a-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0645a-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="0645a-119">Authorization</span></span>|<span data-ttu-id="0645a-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="0645a-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="0645a-121">Accept</span><span class="sxs-lookup"><span data-stu-id="0645a-121">Accept</span></span>|<span data-ttu-id="0645a-122">application/json</span><span class="sxs-lookup"><span data-stu-id="0645a-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0645a-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0645a-123">Request body</span></span>
<span data-ttu-id="0645a-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [androidManagedAppRegistration](../resources/intune_mam_androidmanagedappregistration.md) an.</span><span class="sxs-lookup"><span data-stu-id="0645a-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_mam_androidmanagedappregistration.md) object.</span></span>

<span data-ttu-id="0645a-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [androidManagedAppRegistration](../resources/intune_mam_androidmanagedappregistration.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="0645a-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="0645a-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0645a-126">Property</span></span>|<span data-ttu-id="0645a-127">Typ</span><span class="sxs-lookup"><span data-stu-id="0645a-127">Type</span></span>|<span data-ttu-id="0645a-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0645a-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0645a-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0645a-129">createdDateTime</span></span>|<span data-ttu-id="0645a-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0645a-130">DateTimeOffset</span></span>|<span data-ttu-id="0645a-131">Datum und Uhrzeit der Erstellung. Geerbt von [managedAppRegistration](../resources/intune_mam_managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="0645a-131">Date and time of creation Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="0645a-132">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="0645a-132">lastSyncDateTime</span></span>|<span data-ttu-id="0645a-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0645a-133">DateTimeOffset</span></span>|<span data-ttu-id="0645a-134">Datum und Uhrzeit der letzten Synchronisierung der App mit dem Verwaltungsdienst.</span><span class="sxs-lookup"><span data-stu-id="0645a-134">Date and time of last the app synced with management service.</span></span> <span data-ttu-id="0645a-135">Geerbt von [managedAppRegistration](../resources/intune_mam_managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="0645a-135">Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="0645a-136">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="0645a-136">applicationVersion</span></span>|<span data-ttu-id="0645a-137">String</span><span class="sxs-lookup"><span data-stu-id="0645a-137">String</span></span>|<span data-ttu-id="0645a-138">App-Version. Geerbt von [managedAppRegistration](../resources/intune_mam_managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="0645a-138">App version Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="0645a-139">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="0645a-139">managementSdkVersion</span></span>|<span data-ttu-id="0645a-140">String</span><span class="sxs-lookup"><span data-stu-id="0645a-140">String</span></span>|<span data-ttu-id="0645a-141">Version des App-Verwaltungs-SDK. Geerbt von [managedAppRegistration](../resources/intune_mam_managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="0645a-141">App management SDK version Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="0645a-142">platformVersion</span><span class="sxs-lookup"><span data-stu-id="0645a-142">platformVersion</span></span>|<span data-ttu-id="0645a-143">String</span><span class="sxs-lookup"><span data-stu-id="0645a-143">String</span></span>|<span data-ttu-id="0645a-144">Version des Betriebssystems. Geerbt von [managedAppRegistration](../resources/intune_mam_managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="0645a-144">Operating System version Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="0645a-145">deviceType</span><span class="sxs-lookup"><span data-stu-id="0645a-145">deviceType</span></span>|<span data-ttu-id="0645a-146">String</span><span class="sxs-lookup"><span data-stu-id="0645a-146">String</span></span>|<span data-ttu-id="0645a-147">Gerätetyp des Hostgeräts. Geerbt von [managedAppRegistration](../resources/intune_mam_managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="0645a-147">Host device type Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="0645a-148">deviceTag</span><span class="sxs-lookup"><span data-stu-id="0645a-148">deviceTag</span></span>|<span data-ttu-id="0645a-149">String</span><span class="sxs-lookup"><span data-stu-id="0645a-149">String</span></span>|<span data-ttu-id="0645a-150">Vom App-Verwaltungs-SDK generiertes Tag, das bei der Zuordnung von Apps hilft, die auf demselben Gerät gehostet werden.</span><span class="sxs-lookup"><span data-stu-id="0645a-150">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="0645a-151">Es ist nicht garantiert, dass die App-Zuordnung unter allen Bedingungen funktioniert.</span><span class="sxs-lookup"><span data-stu-id="0645a-151">Not guaranteed to relate apps in all conditions.</span></span> <span data-ttu-id="0645a-152">Geerbt von [managedAppRegistration](../resources/intune_mam_managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="0645a-152">Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="0645a-153">deviceName</span><span class="sxs-lookup"><span data-stu-id="0645a-153">deviceName</span></span>|<span data-ttu-id="0645a-154">String</span><span class="sxs-lookup"><span data-stu-id="0645a-154">String</span></span>|<span data-ttu-id="0645a-155">Gerätename des Hostgeräts. Geerbt von [managedAppRegistration](../resources/intune_mam_managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="0645a-155">Host device name Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="0645a-156">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="0645a-156">flaggedReasons</span></span>|<span data-ttu-id="0645a-157">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="0645a-157">String collection</span></span>|<span data-ttu-id="0645a-158">Gründe (0 oder mehr), aus denen eine App-Registrierung gekennzeichnet wurde.</span><span class="sxs-lookup"><span data-stu-id="0645a-158">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="0645a-159">Beispiel:</span><span class="sxs-lookup"><span data-stu-id="0645a-159">E.g.</span></span> <span data-ttu-id="0645a-160">Die App wird auf einem gerooteten Gerät ausgeführt. Geerbt von [managedAppRegistration](../resources/intune_mam_managedappregistration.md). Mögliche Werte sind: `none` und `rootedDevice`.</span><span class="sxs-lookup"><span data-stu-id="0645a-160">app running on rooted device Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md) Possible values are: `none`, `rootedDevice`.</span></span>|
|<span data-ttu-id="0645a-161">userId</span><span class="sxs-lookup"><span data-stu-id="0645a-161">userID</span></span>|<span data-ttu-id="0645a-162">String</span><span class="sxs-lookup"><span data-stu-id="0645a-162">String</span></span>|<span data-ttu-id="0645a-163">Benutzer-ID, zu der die App-Registrierung gehört.</span><span class="sxs-lookup"><span data-stu-id="0645a-163">The user Id to who this app registration belongs.</span></span> <span data-ttu-id="0645a-164">Geerbt von [managedAppRegistration](../resources/intune_mam_managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="0645a-164">Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="0645a-165">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="0645a-165">appIdentifier</span></span>|[<span data-ttu-id="0645a-166">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="0645a-166">mobileAppIdentifier</span></span>](../resources/intune_mam_mobileappidentifier.md)|<span data-ttu-id="0645a-167">Bezeichner des App-Pakets. Geerbt von [managedAppRegistration](../resources/intune_mam_managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="0645a-167">The app package Identifier Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="0645a-168">id</span><span class="sxs-lookup"><span data-stu-id="0645a-168">id</span></span>|<span data-ttu-id="0645a-169">String</span><span class="sxs-lookup"><span data-stu-id="0645a-169">String</span></span>|<span data-ttu-id="0645a-170">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="0645a-170">Key of the setting.</span></span> <span data-ttu-id="0645a-171">Geerbt von [managedAppRegistration](../resources/intune_mam_managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="0645a-171">Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="0645a-172">version</span><span class="sxs-lookup"><span data-stu-id="0645a-172">version</span></span>|<span data-ttu-id="0645a-173">String</span><span class="sxs-lookup"><span data-stu-id="0645a-173">String</span></span>|<span data-ttu-id="0645a-174">Version der Entität.</span><span class="sxs-lookup"><span data-stu-id="0645a-174">Version of the entity.</span></span> <span data-ttu-id="0645a-175">Geerbt von [managedAppRegistration](../resources/intune_mam_managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="0645a-175">Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="0645a-176">Antwort</span><span class="sxs-lookup"><span data-stu-id="0645a-176">Response</span></span>
<span data-ttu-id="0645a-177">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [androidManagedAppRegistration](../resources/intune_mam_androidmanagedappregistration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="0645a-177">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_mam_androidmanagedappregistration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0645a-178">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0645a-178">Example</span></span>
### <a name="request"></a><span data-ttu-id="0645a-179">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0645a-179">Request</span></span>
<span data-ttu-id="0645a-180">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0645a-180">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0645a-181">Antwort</span><span class="sxs-lookup"><span data-stu-id="0645a-181">Response</span></span>
<span data-ttu-id="0645a-p108">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0645a-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



