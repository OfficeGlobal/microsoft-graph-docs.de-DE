# <a name="update-windows10secureassessmentconfiguration"></a><span data-ttu-id="1a2c6-101">Aktualisieren von „windows10SecureAssessmentConfiguration“</span><span class="sxs-lookup"><span data-stu-id="1a2c6-101">Update windows10SecureAssessmentConfiguration</span></span>

> <span data-ttu-id="1a2c6-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="1a2c6-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1a2c6-103">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [windows10SecureAssessmentConfiguration](../resources/intune_deviceconfig_windows10secureassessmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1a2c6-103">Update the properties of a [windows10SecureAssessmentConfiguration](../resources/intune_deviceconfig_windows10secureassessmentconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1a2c6-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="1a2c6-104">Prerequisites</span></span>
<span data-ttu-id="1a2c6-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="1a2c6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="1a2c6-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1a2c6-107">Permission type</span></span>|<span data-ttu-id="1a2c6-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1a2c6-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1a2c6-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1a2c6-109">Delegated (work or school account)</span></span>|<span data-ttu-id="1a2c6-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a2c6-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1a2c6-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1a2c6-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1a2c6-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1a2c6-112">Not supported.</span></span>|
|<span data-ttu-id="1a2c6-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1a2c6-113">Application</span></span>|<span data-ttu-id="1a2c6-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1a2c6-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1a2c6-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1a2c6-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="1a2c6-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1a2c6-116">Request headers</span></span>
|<span data-ttu-id="1a2c6-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="1a2c6-117">Header</span></span>|<span data-ttu-id="1a2c6-118">Wert</span><span class="sxs-lookup"><span data-stu-id="1a2c6-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1a2c6-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="1a2c6-119">Authorization</span></span>|<span data-ttu-id="1a2c6-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="1a2c6-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1a2c6-121">Accept</span><span class="sxs-lookup"><span data-stu-id="1a2c6-121">Accept</span></span>|<span data-ttu-id="1a2c6-122">application/json</span><span class="sxs-lookup"><span data-stu-id="1a2c6-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1a2c6-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1a2c6-123">Request body</span></span>
<span data-ttu-id="1a2c6-124">Geben Sie als Anforderungstext eine JSON-Darstellung von Objekten des Typs [windows10SecureAssessmentConfiguration](../resources/intune_deviceconfig_windows10secureassessmentconfiguration.md) an.</span><span class="sxs-lookup"><span data-stu-id="1a2c6-124">In the request body, supply a JSON representation for the [windows10SecureAssessmentConfiguration](../resources/intune_deviceconfig_windows10secureassessmentconfiguration.md) object.</span></span>

<span data-ttu-id="1a2c6-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [windows10SecureAssessmentConfiguration](../resources/intune_deviceconfig_windows10secureassessmentconfiguration.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="1a2c6-125">The following table shows the properties that are required when you create the [windows10SecureAssessmentConfiguration](../resources/intune_deviceconfig_windows10secureassessmentconfiguration.md).</span></span>

|<span data-ttu-id="1a2c6-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1a2c6-126">Property</span></span>|<span data-ttu-id="1a2c6-127">Typ</span><span class="sxs-lookup"><span data-stu-id="1a2c6-127">Type</span></span>|<span data-ttu-id="1a2c6-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1a2c6-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a2c6-129">id</span><span class="sxs-lookup"><span data-stu-id="1a2c6-129">id</span></span>|<span data-ttu-id="1a2c6-130">String</span><span class="sxs-lookup"><span data-stu-id="1a2c6-130">String</span></span>|<span data-ttu-id="1a2c6-131">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="1a2c6-131">Key of the entity.</span></span> <span data-ttu-id="1a2c6-132">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1a2c6-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a2c6-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1a2c6-133">lastModifiedDateTime</span></span>|<span data-ttu-id="1a2c6-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1a2c6-134">DateTimeOffset</span></span>|<span data-ttu-id="1a2c6-135">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="1a2c6-135">DateTime the object was last modified.</span></span> <span data-ttu-id="1a2c6-136">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1a2c6-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a2c6-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1a2c6-137">createdDateTime</span></span>|<span data-ttu-id="1a2c6-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1a2c6-138">DateTimeOffset</span></span>|<span data-ttu-id="1a2c6-139">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="1a2c6-139">DateTime the object was created.</span></span> <span data-ttu-id="1a2c6-140">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1a2c6-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a2c6-141">description</span><span class="sxs-lookup"><span data-stu-id="1a2c6-141">description</span></span>|<span data-ttu-id="1a2c6-142">String</span><span class="sxs-lookup"><span data-stu-id="1a2c6-142">String</span></span>|<span data-ttu-id="1a2c6-143">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="1a2c6-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="1a2c6-144">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1a2c6-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a2c6-145">displayName</span><span class="sxs-lookup"><span data-stu-id="1a2c6-145">displayName</span></span>|<span data-ttu-id="1a2c6-146">String</span><span class="sxs-lookup"><span data-stu-id="1a2c6-146">String</span></span>|<span data-ttu-id="1a2c6-147">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="1a2c6-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="1a2c6-148">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1a2c6-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a2c6-149">version</span><span class="sxs-lookup"><span data-stu-id="1a2c6-149">version</span></span>|<span data-ttu-id="1a2c6-150">Int32</span><span class="sxs-lookup"><span data-stu-id="1a2c6-150">Int32</span></span>|<span data-ttu-id="1a2c6-151">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="1a2c6-151">Version of the device configuration.</span></span> <span data-ttu-id="1a2c6-152">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1a2c6-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a2c6-153">launchUri</span><span class="sxs-lookup"><span data-stu-id="1a2c6-153">launchUri</span></span>|<span data-ttu-id="1a2c6-154">String</span><span class="sxs-lookup"><span data-stu-id="1a2c6-154">String</span></span>|<span data-ttu-id="1a2c6-155">URL zu einer Bewertung, die automatisch geladen wird, sobald der Browser für sichere Bewertungen gestartet wird.</span><span class="sxs-lookup"><span data-stu-id="1a2c6-155">Url link to an assessment that's automatically loaded when the secure assessment browser is launched.</span></span> <span data-ttu-id="1a2c6-156">Die URL muss eine gültige URL sein (http\[s\]://msdn.microsoft.com/).</span><span class="sxs-lookup"><span data-stu-id="1a2c6-156">It has to be a valid Url (http\[s\]://msdn.microsoft.com/).</span></span>|
|<span data-ttu-id="1a2c6-157">configurationAccount</span><span class="sxs-lookup"><span data-stu-id="1a2c6-157">configurationAccount</span></span>|<span data-ttu-id="1a2c6-158">String</span><span class="sxs-lookup"><span data-stu-id="1a2c6-158">String</span></span>|<span data-ttu-id="1a2c6-159">Konto, mit dem das Windows-Gerät für den Test konfiguriert wurde.</span><span class="sxs-lookup"><span data-stu-id="1a2c6-159">The account used to configure the Windows device for taking the test.</span></span> <span data-ttu-id="1a2c6-160">Der Benutzer kann ein Domänenkonto (Domäne\Benutzername), ein AAD-Konto (benutzername@mandant.com) oder ein lokales Konto (Benutzername) sein.</span><span class="sxs-lookup"><span data-stu-id="1a2c6-160">The user can be a domain account (domain\user), an AAD account (username@tenant.com) or a local account (username).</span></span>|
|<span data-ttu-id="1a2c6-161">allowPrinting</span><span class="sxs-lookup"><span data-stu-id="1a2c6-161">allowPrinting</span></span>|<span data-ttu-id="1a2c6-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="1a2c6-162">Boolean</span></span>|<span data-ttu-id="1a2c6-163">Gibt an, ob während des Tests über die App gedruckt werden darf.</span><span class="sxs-lookup"><span data-stu-id="1a2c6-163">Indicates whether or not to allow the app from printing during the test.</span></span>|
|<span data-ttu-id="1a2c6-164">allowScreenCapture</span><span class="sxs-lookup"><span data-stu-id="1a2c6-164">allowScreenCapture</span></span>|<span data-ttu-id="1a2c6-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="1a2c6-165">Boolean</span></span>|<span data-ttu-id="1a2c6-166">Gibt an, ob während des Tests über die App Screenshots angefertigt werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="1a2c6-166">Indicates whether or not to allow screen capture capability during a test.</span></span>|
|<span data-ttu-id="1a2c6-167">allowTextSuggestion</span><span class="sxs-lookup"><span data-stu-id="1a2c6-167">allowTextSuggestion</span></span>|<span data-ttu-id="1a2c6-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="1a2c6-168">Boolean</span></span>|<span data-ttu-id="1a2c6-169">Gibt an, ob während des Tests Wortvorschläge angezeigt werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="1a2c6-169">Indicates whether or not to allow text suggestions during the test.</span></span>|



## <a name="response"></a><span data-ttu-id="1a2c6-170">Antwort</span><span class="sxs-lookup"><span data-stu-id="1a2c6-170">Response</span></span>
<span data-ttu-id="1a2c6-171">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [windows10SecureAssessmentConfiguration](../resources/intune_deviceconfig_windows10secureassessmentconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="1a2c6-171">If successful, this method returns a `200 OK` response code and an updated [windows10SecureAssessmentConfiguration](../resources/intune_deviceconfig_windows10secureassessmentconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1a2c6-172">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1a2c6-172">Example</span></span>
### <a name="request"></a><span data-ttu-id="1a2c6-173">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1a2c6-173">Request</span></span>
<span data-ttu-id="1a2c6-174">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1a2c6-174">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 359

{
  "@odata.type": "#microsoft.graph.windows10SecureAssessmentConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "launchUri": "Launch Uri value",
  "configurationAccount": "Configuration Account value",
  "allowPrinting": true,
  "allowScreenCapture": true,
  "allowTextSuggestion": true
}
```

### <a name="response"></a><span data-ttu-id="1a2c6-175">Antwort</span><span class="sxs-lookup"><span data-stu-id="1a2c6-175">Response</span></span>
<span data-ttu-id="1a2c6-p110">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1a2c6-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 531

{
  "@odata.type": "#microsoft.graph.windows10SecureAssessmentConfiguration",
  "id": "f60d71be-71be-f60d-be71-0df6be710df6",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "launchUri": "Launch Uri value",
  "configurationAccount": "Configuration Account value",
  "allowPrinting": true,
  "allowScreenCapture": true,
  "allowTextSuggestion": true
}
```



