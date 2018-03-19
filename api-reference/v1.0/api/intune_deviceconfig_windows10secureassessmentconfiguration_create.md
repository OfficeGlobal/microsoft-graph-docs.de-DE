# <a name="create-windows10secureassessmentconfiguration"></a><span data-ttu-id="8d98a-101">Erstellen von „windows10SecureAssessmentConfiguration“</span><span class="sxs-lookup"><span data-stu-id="8d98a-101">Create windows10SecureAssessmentConfiguration</span></span>

> <span data-ttu-id="8d98a-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="8d98a-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8d98a-103">Erstellen eines neuen [windows10SecureAssessmentConfiguration](../resources/intune_deviceconfig_windows10secureassessmentconfiguration.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="8d98a-103">Create a new [plannerBucket](../resources/intune_deviceconfig_windows10secureassessmentconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8d98a-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="8d98a-104">Prerequisites</span></span>
<span data-ttu-id="8d98a-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="8d98a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="8d98a-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8d98a-107">Permission type</span></span>|<span data-ttu-id="8d98a-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8d98a-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8d98a-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8d98a-109">Delegated (work or school account)</span></span>|<span data-ttu-id="8d98a-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d98a-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8d98a-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8d98a-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8d98a-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8d98a-112">Not supported.</span></span>|
|<span data-ttu-id="8d98a-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8d98a-113">Application</span></span>|<span data-ttu-id="8d98a-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8d98a-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8d98a-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8d98a-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="8d98a-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8d98a-116">Request headers</span></span>
|<span data-ttu-id="8d98a-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="8d98a-117">Header</span></span>|<span data-ttu-id="8d98a-118">Wert</span><span class="sxs-lookup"><span data-stu-id="8d98a-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8d98a-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="8d98a-119">Authorization</span></span>|<span data-ttu-id="8d98a-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="8d98a-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="8d98a-121">Annehmen</span><span class="sxs-lookup"><span data-stu-id="8d98a-121">Accept</span></span>|<span data-ttu-id="8d98a-122">application/json</span><span class="sxs-lookup"><span data-stu-id="8d98a-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8d98a-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8d98a-123">Request body</span></span>
<span data-ttu-id="8d98a-124">Geben Sie im Anforderungstext eine JSON-Darstellung des windows10SecureAssessmentConfiguration-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="8d98a-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="8d98a-125">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der windows10SecureAssessmentConfiguration erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="8d98a-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="8d98a-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8d98a-126">Property</span></span>|<span data-ttu-id="8d98a-127">Typ</span><span class="sxs-lookup"><span data-stu-id="8d98a-127">Type</span></span>|<span data-ttu-id="8d98a-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8d98a-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8d98a-129">id</span><span class="sxs-lookup"><span data-stu-id="8d98a-129">id</span></span>|<span data-ttu-id="8d98a-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8d98a-130">String</span></span>|<span data-ttu-id="8d98a-131">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="8d98a-131">Key of the setting.</span></span> <span data-ttu-id="8d98a-132">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8d98a-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8d98a-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8d98a-133">lastModifiedDateTime</span></span>|<span data-ttu-id="8d98a-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8d98a-134">DateTimeOffset</span></span>|<span data-ttu-id="8d98a-135">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="8d98a-135">Indicates the date the object was last modified.</span></span> <span data-ttu-id="8d98a-136">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8d98a-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8d98a-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8d98a-137">createdDateTime</span></span>|<span data-ttu-id="8d98a-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8d98a-138">DateTimeOffset</span></span>|<span data-ttu-id="8d98a-139">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="8d98a-139">DateTime the object was created.</span></span> <span data-ttu-id="8d98a-140">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8d98a-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8d98a-141">description</span><span class="sxs-lookup"><span data-stu-id="8d98a-141">description</span></span>|<span data-ttu-id="8d98a-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8d98a-142">String</span></span>|<span data-ttu-id="8d98a-143">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="8d98a-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="8d98a-144">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8d98a-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8d98a-145">displayName</span><span class="sxs-lookup"><span data-stu-id="8d98a-145">displayName</span></span>|<span data-ttu-id="8d98a-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8d98a-146">String</span></span>|<span data-ttu-id="8d98a-147">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="8d98a-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="8d98a-148">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8d98a-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8d98a-149">Version</span><span class="sxs-lookup"><span data-stu-id="8d98a-149">version</span></span>|<span data-ttu-id="8d98a-150">Int32</span><span class="sxs-lookup"><span data-stu-id="8d98a-150">Int32</span></span>|<span data-ttu-id="8d98a-151">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="8d98a-151">Version of the device configuration.</span></span> <span data-ttu-id="8d98a-152">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8d98a-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8d98a-153">launchUri</span><span class="sxs-lookup"><span data-stu-id="8d98a-153">launchUri</span></span>|<span data-ttu-id="8d98a-154">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8d98a-154">String</span></span>|<span data-ttu-id="8d98a-155">URL zu einer Bewertung, die automatisch geladen wird, sobald der Browser für sichere Bewertungen gestartet wird.</span><span class="sxs-lookup"><span data-stu-id="8d98a-155">Url link to an assessment that's automatically loaded when the secure assessment browser is launched.</span></span> <span data-ttu-id="8d98a-156">Die URL muss eine gültige URL sein (http\[s\]://msdn.microsoft.com/).</span><span class="sxs-lookup"><span data-stu-id="8d98a-156">It has to be a valid Url (http\[s\]://msdn.microsoft.com/).</span></span>|
|<span data-ttu-id="8d98a-157">configurationAccount</span><span class="sxs-lookup"><span data-stu-id="8d98a-157">configurationAccount</span></span>|<span data-ttu-id="8d98a-158">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8d98a-158">String</span></span>|<span data-ttu-id="8d98a-159">Konto, mit dem das Windows-Gerät für den Test konfiguriert wurde.</span><span class="sxs-lookup"><span data-stu-id="8d98a-159">The account used to configure the Windows device for taking the test.</span></span> <span data-ttu-id="8d98a-160">Der Benutzer kann ein Domänenkonto (Domäne\Benutzername), ein AAD-Konto (benutzername@mandant.com) oder ein lokales Konto (Benutzername) sein.</span><span class="sxs-lookup"><span data-stu-id="8d98a-160">The user can be a domain account (domain\user), an AAD account (username@tenant.com) or a local account (username).</span></span>|
|<span data-ttu-id="8d98a-161">allowPrinting</span><span class="sxs-lookup"><span data-stu-id="8d98a-161">allowPrinting</span></span>|<span data-ttu-id="8d98a-162">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="8d98a-162">Boolean</span></span>|<span data-ttu-id="8d98a-163">Gibt an, ob während des Tests über die App gedruckt werden darf.</span><span class="sxs-lookup"><span data-stu-id="8d98a-163">Indicates whether or not to allow the app from printing during the test.</span></span>|
|<span data-ttu-id="8d98a-164">allowScreenCapture</span><span class="sxs-lookup"><span data-stu-id="8d98a-164">allowScreenCapture</span></span>|<span data-ttu-id="8d98a-165">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="8d98a-165">Boolean</span></span>|<span data-ttu-id="8d98a-166">Gibt an, ob während des Tests über die App Screenshots angefertigt werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="8d98a-166">Indicates whether or not to allow screen capture capability during a test.</span></span>|
|<span data-ttu-id="8d98a-167">allowTextSuggestion</span><span class="sxs-lookup"><span data-stu-id="8d98a-167">allowTextSuggestion</span></span>|<span data-ttu-id="8d98a-168">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="8d98a-168">Boolean</span></span>|<span data-ttu-id="8d98a-169">Gibt an, ob während des Tests Wortvorschläge angezeigt werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="8d98a-169">Indicates whether or not to allow text suggestions during the test.</span></span>|



## <a name="response"></a><span data-ttu-id="8d98a-170">Antwort</span><span class="sxs-lookup"><span data-stu-id="8d98a-170">Response</span></span>
<span data-ttu-id="8d98a-171">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [windows10SecureAssessmentConfiguration](../resources/intune_deviceconfig_windows10secureassessmentconfiguration.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8d98a-171">If successful, this method returns a `201 Created` response code and a [section](../resources/intune_deviceconfig_windows10secureassessmentconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8d98a-172">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8d98a-172">Example</span></span>
### <a name="request"></a><span data-ttu-id="8d98a-173">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8d98a-173">Request</span></span>
<span data-ttu-id="8d98a-174">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8d98a-174">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 423

{
  "@odata.type": "#microsoft.graph.windows10SecureAssessmentConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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

### <a name="response"></a><span data-ttu-id="8d98a-175">Antwort</span><span class="sxs-lookup"><span data-stu-id="8d98a-175">Response</span></span>
<span data-ttu-id="8d98a-p110">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8d98a-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



