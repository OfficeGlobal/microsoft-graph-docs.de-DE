# <a name="create-androidmanagedappregistration"></a><span data-ttu-id="d583d-101">Erstellen von „androidManagedAppRegistration“</span><span class="sxs-lookup"><span data-stu-id="d583d-101">Create androidManagedAppRegistration</span></span>

> <span data-ttu-id="d583d-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="d583d-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d583d-103">Diese Methode erstellt ein neues Objekt des Typs [androidManagedAppRegistration](../resources/intune_mam_androidmanagedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="d583d-103">Create a new [androidManagedAppRegistration](../resources/intune_mam_androidmanagedappregistration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d583d-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="d583d-104">Prerequisites</span></span>
<span data-ttu-id="d583d-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="d583d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d583d-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d583d-107">Permission type</span></span>|<span data-ttu-id="d583d-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d583d-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d583d-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d583d-109">Delegated (work or school account)</span></span>|<span data-ttu-id="d583d-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d583d-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d583d-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d583d-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d583d-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d583d-112">Not supported.</span></span>|
|<span data-ttu-id="d583d-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d583d-113">Application</span></span>|<span data-ttu-id="d583d-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d583d-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d583d-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d583d-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppRegistrations
```

## <a name="request-headers"></a><span data-ttu-id="d583d-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d583d-116">Request headers</span></span>
|<span data-ttu-id="d583d-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="d583d-117">Header</span></span>|<span data-ttu-id="d583d-118">Wert</span><span class="sxs-lookup"><span data-stu-id="d583d-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d583d-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="d583d-119">Authorization</span></span>|<span data-ttu-id="d583d-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="d583d-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d583d-121">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="d583d-121">Accept</span></span>|<span data-ttu-id="d583d-122">Anwendung/json</span><span class="sxs-lookup"><span data-stu-id="d583d-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d583d-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d583d-123">Request body</span></span>
<span data-ttu-id="d583d-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „androidManagedAppRegistration“ an.</span><span class="sxs-lookup"><span data-stu-id="d583d-124">In the request body, supply a JSON representation for the androidManagedAppRegistration object.</span></span>

<span data-ttu-id="d583d-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „androidManagedAppRegistration“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="d583d-125">The following table shows the properties that are required when you create the androidManagedAppRegistration.</span></span>

|<span data-ttu-id="d583d-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d583d-126">Property</span></span>|<span data-ttu-id="d583d-127">Typ</span><span class="sxs-lookup"><span data-stu-id="d583d-127">Type</span></span>|<span data-ttu-id="d583d-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d583d-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d583d-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d583d-129">createdDateTime</span></span>|<span data-ttu-id="d583d-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d583d-130">DateTimeOffset</span></span>|<span data-ttu-id="d583d-131">Datum und Uhrzeit der Erstellung. Geerbt von [managedAppRegistration](../resources/intune_mam_managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="d583d-131">Date and time of creation Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="d583d-132">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="d583d-132">lastSyncDateTime</span></span>|<span data-ttu-id="d583d-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d583d-133">DateTimeOffset</span></span>|<span data-ttu-id="d583d-134">Datum und Uhrzeit der letzten Synchronisierung der App mit dem Verwaltungsdienst.</span><span class="sxs-lookup"><span data-stu-id="d583d-134">Date and time of last the app synced with management service.</span></span> <span data-ttu-id="d583d-135">Geerbt von [managedAppRegistration](../resources/intune_mam_managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="d583d-135">Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="d583d-136">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="d583d-136">applicationVersion</span></span>|<span data-ttu-id="d583d-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d583d-137">String</span></span>|<span data-ttu-id="d583d-138">App-Version. Geerbt von [managedAppRegistration](../resources/intune_mam_managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="d583d-138">App version Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="d583d-139">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="d583d-139">managementSdkVersion</span></span>|<span data-ttu-id="d583d-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d583d-140">String</span></span>|<span data-ttu-id="d583d-141">Version des App-Verwaltungs-SDK. Geerbt von [managedAppRegistration](../resources/intune_mam_managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="d583d-141">App management SDK version Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="d583d-142">platformVersion</span><span class="sxs-lookup"><span data-stu-id="d583d-142">platformVersion</span></span>|<span data-ttu-id="d583d-143">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d583d-143">String</span></span>|<span data-ttu-id="d583d-144">Version des Betriebssystems. Geerbt von [managedAppRegistration](../resources/intune_mam_managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="d583d-144">Operating System version Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="d583d-145">deviceType</span><span class="sxs-lookup"><span data-stu-id="d583d-145">deviceType</span></span>|<span data-ttu-id="d583d-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d583d-146">String</span></span>|<span data-ttu-id="d583d-147">Gerätetyp des Hostgeräts. Geerbt von [managedAppRegistration](../resources/intune_mam_managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="d583d-147">Host device type Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="d583d-148">deviceTag</span><span class="sxs-lookup"><span data-stu-id="d583d-148">deviceTag</span></span>|<span data-ttu-id="d583d-149">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d583d-149">String</span></span>|<span data-ttu-id="d583d-150">Vom App-Verwaltungs-SDK generiertes Tag, das bei der Zuordnung von Apps hilft, die auf demselben Gerät gehostet werden.</span><span class="sxs-lookup"><span data-stu-id="d583d-150">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="d583d-151">Es ist nicht garantiert, dass die App-Zuordnung unter allen Bedingungen funktioniert.</span><span class="sxs-lookup"><span data-stu-id="d583d-151">Not guaranteed to relate apps in all conditions.</span></span> <span data-ttu-id="d583d-152">Geerbt von [managedAppRegistration](../resources/intune_mam_managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="d583d-152">Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="d583d-153">deviceName</span><span class="sxs-lookup"><span data-stu-id="d583d-153">deviceName</span></span>|<span data-ttu-id="d583d-154">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d583d-154">String</span></span>|<span data-ttu-id="d583d-155">Gerätename des Hostgeräts. Geerbt von [managedAppRegistration](../resources/intune_mam_managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="d583d-155">Host device name Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="d583d-156">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="d583d-156">flaggedReasons</span></span>|<span data-ttu-id="d583d-157">[managedAppFlaggedReason Enumerations](../resources/intune_mam_managedappflaggedreason.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="d583d-157">[managedAppFlaggedReason enum](../resources/intune_mam_managedappflaggedreason.md) collection</span></span>|<span data-ttu-id="d583d-158">Gründe (0 oder mehr), aus denen eine App-Registrierung gekennzeichnet wurde.</span><span class="sxs-lookup"><span data-stu-id="d583d-158">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="d583d-159">Z.B.</span><span class="sxs-lookup"><span data-stu-id="d583d-159">E.g.</span></span> <span data-ttu-id="d583d-160">Die App wird auf einem gerooteten Gerät ausgeführt. Geerbt von [managedAppRegistration](../resources/intune_mam_managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="d583d-160">app running on rooted device Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span> <span data-ttu-id="d583d-161">Die möglichen Werte sind: `none`, `rootedDevice`.</span><span class="sxs-lookup"><span data-stu-id="d583d-161">The possible values are:</span></span>|
|<span data-ttu-id="d583d-162">userId</span><span class="sxs-lookup"><span data-stu-id="d583d-162">userId</span></span>|<span data-ttu-id="d583d-163">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d583d-163">String</span></span>|<span data-ttu-id="d583d-164">Benutzer-ID, zu der die App-Registrierung gehört.</span><span class="sxs-lookup"><span data-stu-id="d583d-164">The user Id to who this app registration belongs.</span></span> <span data-ttu-id="d583d-165">Geerbt von [managedAppRegistration](../resources/intune_mam_managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="d583d-165">Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="d583d-166">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="d583d-166">appIdentifier</span></span>|[<span data-ttu-id="d583d-167">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="d583d-167">mobileAppIdentifier</span></span>](../resources/intune_mam_mobileappidentifier.md)|<span data-ttu-id="d583d-168">Bezeichner des App-Pakets. Geerbt von [managedAppRegistration](../resources/intune_mam_managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="d583d-168">The app package Identifier Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="d583d-169">id</span><span class="sxs-lookup"><span data-stu-id="d583d-169">id</span></span>|<span data-ttu-id="d583d-170">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d583d-170">String</span></span>|<span data-ttu-id="d583d-171">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="d583d-171">Key of the entity.</span></span> <span data-ttu-id="d583d-172">Geerbt von [managedAppRegistration](../resources/intune_mam_managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="d583d-172">Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="d583d-173">Version</span><span class="sxs-lookup"><span data-stu-id="d583d-173">version</span></span>|<span data-ttu-id="d583d-174">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d583d-174">String</span></span>|<span data-ttu-id="d583d-175">Version der Entität</span><span class="sxs-lookup"><span data-stu-id="d583d-175">Version of the entity.</span></span> <span data-ttu-id="d583d-176">Geerbt von [managedAppRegistration](../resources/intune_mam_managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="d583d-176">Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="d583d-177">Antwort</span><span class="sxs-lookup"><span data-stu-id="d583d-177">Response</span></span>
<span data-ttu-id="d583d-178">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [androidManagedAppRegistration](../resources/intune_mam_androidmanagedappregistration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="d583d-178">If successful, this method returns a `201 Created` response code and a [androidManagedAppRegistration](../resources/intune_mam_androidmanagedappregistration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d583d-179">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d583d-179">Example</span></span>
### <a name="request"></a><span data-ttu-id="d583d-180">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d583d-180">Request</span></span>
<span data-ttu-id="d583d-181">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d583d-181">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppRegistrations
Content-type: application/json
Content-length: 645

{
  "@odata.type": "#microsoft.graph.androidManagedAppRegistration",
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

### <a name="response"></a><span data-ttu-id="d583d-182">Antwort</span><span class="sxs-lookup"><span data-stu-id="d583d-182">Response</span></span>
<span data-ttu-id="d583d-p108">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d583d-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



