# <a name="update-iosupdateconfiguration"></a><span data-ttu-id="5ccdb-101">Aktualisieren von „iosUpdateConfiguration“</span><span class="sxs-lookup"><span data-stu-id="5ccdb-101">Update iosUpdateConfiguration</span></span>

> <span data-ttu-id="5ccdb-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="5ccdb-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5ccdb-103">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [iosUpdateConfiguration](../resources/intune_deviceconfig_iosupdateconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5ccdb-103">Update the properties of a [iosUpdateConfiguration](../resources/intune_deviceconfig_iosupdateconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5ccdb-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="5ccdb-104">Prerequisites</span></span>
<span data-ttu-id="5ccdb-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="5ccdb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="5ccdb-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5ccdb-107">Permission type</span></span>|<span data-ttu-id="5ccdb-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5ccdb-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5ccdb-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5ccdb-109">Delegated (work or school account)</span></span>|<span data-ttu-id="5ccdb-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ccdb-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5ccdb-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5ccdb-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5ccdb-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5ccdb-112">Not supported.</span></span>|
|<span data-ttu-id="5ccdb-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5ccdb-113">Application</span></span>|<span data-ttu-id="5ccdb-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5ccdb-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5ccdb-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5ccdb-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="5ccdb-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5ccdb-116">Request headers</span></span>
|<span data-ttu-id="5ccdb-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="5ccdb-117">Header</span></span>|<span data-ttu-id="5ccdb-118">Wert</span><span class="sxs-lookup"><span data-stu-id="5ccdb-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5ccdb-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="5ccdb-119">Authorization</span></span>|<span data-ttu-id="5ccdb-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="5ccdb-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5ccdb-121">Accept</span><span class="sxs-lookup"><span data-stu-id="5ccdb-121">Accept</span></span>|<span data-ttu-id="5ccdb-122">application/json</span><span class="sxs-lookup"><span data-stu-id="5ccdb-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5ccdb-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5ccdb-123">Request body</span></span>
<span data-ttu-id="5ccdb-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [iosUpdateConfiguration](../resources/intune_deviceconfig_iosupdateconfiguration.md) an.</span><span class="sxs-lookup"><span data-stu-id="5ccdb-124">In the request body, supply a JSON representation for the [iosUpdateConfiguration](../resources/intune_deviceconfig_iosupdateconfiguration.md) object.</span></span>

<span data-ttu-id="5ccdb-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [iosUpdateConfiguration](../resources/intune_deviceconfig_iosupdateconfiguration.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="5ccdb-125">The following table shows the properties that are required when you create the [iosUpdateConfiguration](../resources/intune_deviceconfig_iosupdateconfiguration.md).</span></span>

|<span data-ttu-id="5ccdb-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5ccdb-126">Property</span></span>|<span data-ttu-id="5ccdb-127">Typ</span><span class="sxs-lookup"><span data-stu-id="5ccdb-127">Type</span></span>|<span data-ttu-id="5ccdb-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5ccdb-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5ccdb-129">id</span><span class="sxs-lookup"><span data-stu-id="5ccdb-129">id</span></span>|<span data-ttu-id="5ccdb-130">String</span><span class="sxs-lookup"><span data-stu-id="5ccdb-130">String</span></span>|<span data-ttu-id="5ccdb-131">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="5ccdb-131">Key of the entity.</span></span> <span data-ttu-id="5ccdb-132">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5ccdb-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5ccdb-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5ccdb-133">lastModifiedDateTime</span></span>|<span data-ttu-id="5ccdb-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5ccdb-134">DateTimeOffset</span></span>|<span data-ttu-id="5ccdb-135">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="5ccdb-135">DateTime the object was last modified.</span></span> <span data-ttu-id="5ccdb-136">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5ccdb-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5ccdb-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5ccdb-137">createdDateTime</span></span>|<span data-ttu-id="5ccdb-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5ccdb-138">DateTimeOffset</span></span>|<span data-ttu-id="5ccdb-139">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="5ccdb-139">DateTime the object was created.</span></span> <span data-ttu-id="5ccdb-140">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5ccdb-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5ccdb-141">description</span><span class="sxs-lookup"><span data-stu-id="5ccdb-141">description</span></span>|<span data-ttu-id="5ccdb-142">String</span><span class="sxs-lookup"><span data-stu-id="5ccdb-142">String</span></span>|<span data-ttu-id="5ccdb-143">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="5ccdb-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="5ccdb-144">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5ccdb-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5ccdb-145">displayName</span><span class="sxs-lookup"><span data-stu-id="5ccdb-145">displayName</span></span>|<span data-ttu-id="5ccdb-146">String</span><span class="sxs-lookup"><span data-stu-id="5ccdb-146">String</span></span>|<span data-ttu-id="5ccdb-147">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="5ccdb-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="5ccdb-148">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5ccdb-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5ccdb-149">version</span><span class="sxs-lookup"><span data-stu-id="5ccdb-149">version</span></span>|<span data-ttu-id="5ccdb-150">Int32</span><span class="sxs-lookup"><span data-stu-id="5ccdb-150">Int32</span></span>|<span data-ttu-id="5ccdb-151">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="5ccdb-151">Version of the device configuration.</span></span> <span data-ttu-id="5ccdb-152">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5ccdb-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5ccdb-153">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="5ccdb-153">activeHoursStart</span></span>|<span data-ttu-id="5ccdb-154">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="5ccdb-154">TimeOfDay</span></span>|<span data-ttu-id="5ccdb-155">Beginn der aktiven Stunden (Als aktive Stunden wird das Zeitfenster bezeichnet, in dem keine Updates installiert werden sollen.)</span><span class="sxs-lookup"><span data-stu-id="5ccdb-155">Active Hours Start (active hours mean the time window when updates install should not happen)</span></span>|
|<span data-ttu-id="5ccdb-156">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="5ccdb-156">activeHoursEnd</span></span>|<span data-ttu-id="5ccdb-157">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="5ccdb-157">TimeOfDay</span></span>|<span data-ttu-id="5ccdb-158">Ende der aktiven Stunden (Als aktive Stunden wird das Zeitfenster bezeichnet, in dem keine Updates installiert werden sollen.)</span><span class="sxs-lookup"><span data-stu-id="5ccdb-158">Active Hours End (active hours mean the time window when updates install should not happen)</span></span>|
|<span data-ttu-id="5ccdb-159">scheduledInstallDays</span><span class="sxs-lookup"><span data-stu-id="5ccdb-159">scheduledInstallDays</span></span>|<span data-ttu-id="5ccdb-160">[DayOfWeek](../resources/intune_deviceconfig_dayofweek.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="5ccdb-160">[dayOfWeek](../resources/intune_deviceconfig_dayofweek.md) collection</span></span>|<span data-ttu-id="5ccdb-161">Tage in der Woche, für die aktive Stunden konfiguriert sind.</span><span class="sxs-lookup"><span data-stu-id="5ccdb-161">Days in week for which active hours are configured.</span></span> <span data-ttu-id="5ccdb-162">Diese Sammlung darf maximal 7 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="5ccdb-162">This collection can contain a maximum of 7 elements.</span></span> <span data-ttu-id="5ccdb-163">Mögliche Werte sind: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday` und `saturday`.</span><span class="sxs-lookup"><span data-stu-id="5ccdb-163">Possible values are: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="5ccdb-164">utcTimeOffsetInMinutes</span><span class="sxs-lookup"><span data-stu-id="5ccdb-164">utcTimeOffsetInMinutes</span></span>|<span data-ttu-id="5ccdb-165">Int32</span><span class="sxs-lookup"><span data-stu-id="5ccdb-165">Int32</span></span>|<span data-ttu-id="5ccdb-166">UTC-Zeitversatz in Minuten</span><span class="sxs-lookup"><span data-stu-id="5ccdb-166">UTC Time Offset indicated in minutes</span></span>|



## <a name="response"></a><span data-ttu-id="5ccdb-167">Antwort</span><span class="sxs-lookup"><span data-stu-id="5ccdb-167">Response</span></span>
<span data-ttu-id="5ccdb-168">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [iosUpdateConfiguration](../resources/intune_deviceconfig_iosupdateconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="5ccdb-168">If successful, this method returns a `200 OK` response code and an updated [iosUpdateConfiguration](../resources/intune_deviceconfig_iosupdateconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5ccdb-169">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5ccdb-169">Example</span></span>
### <a name="request"></a><span data-ttu-id="5ccdb-170">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5ccdb-170">Request</span></span>
<span data-ttu-id="5ccdb-171">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5ccdb-171">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 325

{
  "@odata.type": "#microsoft.graph.iosUpdateConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "activeHoursStart": "12:00:05.5020000",
  "activeHoursEnd": "11:59:00.8990000",
  "scheduledInstallDays": [
    "monday"
  ],
  "utcTimeOffsetInMinutes": 6
}
```

### <a name="response"></a><span data-ttu-id="5ccdb-172">Antwort</span><span class="sxs-lookup"><span data-stu-id="5ccdb-172">Response</span></span>
<span data-ttu-id="5ccdb-p109">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5ccdb-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 497

{
  "@odata.type": "#microsoft.graph.iosUpdateConfiguration",
  "id": "321aef09-ef09-321a-09ef-1a3209ef1a32",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "activeHoursStart": "12:00:05.5020000",
  "activeHoursEnd": "11:59:00.8990000",
  "scheduledInstallDays": [
    "monday"
  ],
  "utcTimeOffsetInMinutes": 6
}
```



