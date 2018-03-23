# <a name="create-iosupdateconfiguration"></a><span data-ttu-id="80353-101">iosUpdateConfiguration erstellen</span><span class="sxs-lookup"><span data-stu-id="80353-101">Create iosUpdateConfiguration</span></span>

> <span data-ttu-id="80353-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="80353-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="80353-103">Erstellen eines neuen [iosUpdateConfiguration](../resources/intune_deviceconfig_iosupdateconfiguration.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="80353-103">Create a new [plannerBucket](../resources/intune_deviceconfig_iosupdateconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="80353-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="80353-104">Prerequisites</span></span>
<span data-ttu-id="80353-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="80353-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="80353-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="80353-107">Permission type</span></span>|<span data-ttu-id="80353-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="80353-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="80353-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="80353-109">Delegated (work or school account)</span></span>|<span data-ttu-id="80353-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="80353-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="80353-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="80353-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="80353-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="80353-112">Not supported.</span></span>|
|<span data-ttu-id="80353-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="80353-113">Application</span></span>|<span data-ttu-id="80353-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="80353-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="80353-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="80353-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="80353-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="80353-116">Request headers</span></span>
|<span data-ttu-id="80353-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="80353-117">Header</span></span>|<span data-ttu-id="80353-118">Wert</span><span class="sxs-lookup"><span data-stu-id="80353-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="80353-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="80353-119">Authorization</span></span>|<span data-ttu-id="80353-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="80353-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="80353-121">Annehmen</span><span class="sxs-lookup"><span data-stu-id="80353-121">Accept</span></span>|<span data-ttu-id="80353-122">application/json</span><span class="sxs-lookup"><span data-stu-id="80353-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="80353-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="80353-123">Request body</span></span>
<span data-ttu-id="80353-124">Geben Sie im Anforderungstext eine JSON-Darstellung des iosUpdateConfiguration-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="80353-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="80353-125">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen des iosUpdateConfiguration erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="80353-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="80353-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="80353-126">Property</span></span>|<span data-ttu-id="80353-127">Typ</span><span class="sxs-lookup"><span data-stu-id="80353-127">Type</span></span>|<span data-ttu-id="80353-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="80353-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="80353-129">id</span><span class="sxs-lookup"><span data-stu-id="80353-129">id</span></span>|<span data-ttu-id="80353-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="80353-130">String</span></span>|<span data-ttu-id="80353-131">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="80353-131">Key of the setting.</span></span> <span data-ttu-id="80353-132">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="80353-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="80353-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="80353-133">lastModifiedDateTime</span></span>|<span data-ttu-id="80353-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="80353-134">DateTimeOffset</span></span>|<span data-ttu-id="80353-135">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="80353-135">Indicates the date the object was last modified.</span></span> <span data-ttu-id="80353-136">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="80353-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="80353-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="80353-137">createdDateTime</span></span>|<span data-ttu-id="80353-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="80353-138">DateTimeOffset</span></span>|<span data-ttu-id="80353-139">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="80353-139">DateTime the object was created.</span></span> <span data-ttu-id="80353-140">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="80353-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="80353-141">description</span><span class="sxs-lookup"><span data-stu-id="80353-141">description</span></span>|<span data-ttu-id="80353-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="80353-142">String</span></span>|<span data-ttu-id="80353-143">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="80353-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="80353-144">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="80353-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="80353-145">displayName</span><span class="sxs-lookup"><span data-stu-id="80353-145">displayName</span></span>|<span data-ttu-id="80353-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="80353-146">String</span></span>|<span data-ttu-id="80353-147">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="80353-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="80353-148">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="80353-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="80353-149">Version</span><span class="sxs-lookup"><span data-stu-id="80353-149">version</span></span>|<span data-ttu-id="80353-150">Int32</span><span class="sxs-lookup"><span data-stu-id="80353-150">Int32</span></span>|<span data-ttu-id="80353-151">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="80353-151">Version of the device configuration.</span></span> <span data-ttu-id="80353-152">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="80353-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="80353-153">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="80353-153">activeHoursStart</span></span>|<span data-ttu-id="80353-154">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="80353-154">TimeOfDay</span></span>|<span data-ttu-id="80353-155">Beginn der aktiven Stunden (als aktive Stunden wird das Zeitfenster bezeichnet, in dem keine Installation von Updates ausgeführt werden soll)</span><span class="sxs-lookup"><span data-stu-id="80353-155">Active Hours Start (active hours mean the time window when updates install should not happen)</span></span>|
|<span data-ttu-id="80353-156">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="80353-156">activeHoursEnd</span></span>|<span data-ttu-id="80353-157">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="80353-157">TimeOfDay</span></span>|<span data-ttu-id="80353-158">Ende der aktiven Stunden (als aktive Stunden wird das Zeitfenster bezeichnet, in dem keine Installation von Updates ausgeführt werden soll)</span><span class="sxs-lookup"><span data-stu-id="80353-158">Active Hours End (active hours mean the time window when updates install should not happen)</span></span>|
|<span data-ttu-id="80353-159">scheduledInstallDays</span><span class="sxs-lookup"><span data-stu-id="80353-159">scheduledInstallDays</span></span>|<span data-ttu-id="80353-160">String collection</span><span class="sxs-lookup"><span data-stu-id="80353-160">String collection</span></span>|<span data-ttu-id="80353-161">Tage in der Woche, für die aktive Stunden konfiguriert werden.</span><span class="sxs-lookup"><span data-stu-id="80353-161">Days in week for which active hours are configured.</span></span> <span data-ttu-id="80353-162">Diese Sammlung darf maximal 7 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="80353-162">This collection can contain a maximum of 7 elements.</span></span> <span data-ttu-id="80353-163">Mögliche Werte: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span><span class="sxs-lookup"><span data-stu-id="80353-163">Possible values are: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="80353-164">utcTimeOffsetInMinutes</span><span class="sxs-lookup"><span data-stu-id="80353-164">utcTimeOffsetInMinutes</span></span>|<span data-ttu-id="80353-165">Int32</span><span class="sxs-lookup"><span data-stu-id="80353-165">Int32</span></span>|<span data-ttu-id="80353-166">UTC-Zeitversatz in Minuten</span><span class="sxs-lookup"><span data-stu-id="80353-166">UTC Time Offset indicated in minutes</span></span>|



## <a name="response"></a><span data-ttu-id="80353-167">Antwort</span><span class="sxs-lookup"><span data-stu-id="80353-167">Response</span></span>
<span data-ttu-id="80353-168">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [iosUpdateConfiguration](../resources/intune_deviceconfig_iosupdateconfiguration.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="80353-168">If successful, this method returns a `201 Created` response code and a [section](../resources/intune_deviceconfig_iosupdateconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="80353-169">Beispiel</span><span class="sxs-lookup"><span data-stu-id="80353-169">Example</span></span>
### <a name="request"></a><span data-ttu-id="80353-170">Anforderung</span><span class="sxs-lookup"><span data-stu-id="80353-170">Request</span></span>
<span data-ttu-id="80353-171">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="80353-171">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 389

{
  "@odata.type": "#microsoft.graph.iosUpdateConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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

### <a name="response"></a><span data-ttu-id="80353-172">Antwort</span><span class="sxs-lookup"><span data-stu-id="80353-172">Response</span></span>
<span data-ttu-id="80353-p109">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="80353-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



