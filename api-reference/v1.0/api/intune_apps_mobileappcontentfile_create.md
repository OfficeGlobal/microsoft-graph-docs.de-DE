# <a name="create-mobileappcontentfile"></a><span data-ttu-id="7f6f3-101">Erstellen von „mobileAppContentFile“</span><span class="sxs-lookup"><span data-stu-id="7f6f3-101">Create mobileAppContentFile</span></span>

> <span data-ttu-id="7f6f3-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="7f6f3-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7f6f3-103">Diese Methode erstellt ein neues Objekt des Typs [mobileAppContentFile](../resources/intune_apps_mobileappcontentfile.md).</span><span class="sxs-lookup"><span data-stu-id="7f6f3-103">Create a new [mobileAppContentFile](../resources/intune_apps_mobileappcontentfile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7f6f3-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="7f6f3-104">Prerequisites</span></span>
<span data-ttu-id="7f6f3-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="7f6f3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="7f6f3-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7f6f3-107">Permission type</span></span>|<span data-ttu-id="7f6f3-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7f6f3-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7f6f3-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7f6f3-109">Delegated (work or school account)</span></span>|<span data-ttu-id="7f6f3-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f6f3-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7f6f3-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7f6f3-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7f6f3-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7f6f3-112">Not supported.</span></span>|
|<span data-ttu-id="7f6f3-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7f6f3-113">Application</span></span>|<span data-ttu-id="7f6f3-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7f6f3-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7f6f3-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7f6f3-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files
```

## <a name="request-headers"></a><span data-ttu-id="7f6f3-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7f6f3-116">Request headers</span></span>
|<span data-ttu-id="7f6f3-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="7f6f3-117">Header</span></span>|<span data-ttu-id="7f6f3-118">Wert</span><span class="sxs-lookup"><span data-stu-id="7f6f3-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7f6f3-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="7f6f3-119">Authorization</span></span>|<span data-ttu-id="7f6f3-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="7f6f3-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7f6f3-121">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="7f6f3-121">Accept</span></span>|<span data-ttu-id="7f6f3-122">Anwendung/json</span><span class="sxs-lookup"><span data-stu-id="7f6f3-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7f6f3-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7f6f3-123">Request body</span></span>
<span data-ttu-id="7f6f3-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „mobileAppContentFile“ an.</span><span class="sxs-lookup"><span data-stu-id="7f6f3-124">In the request body, supply a JSON representation for the mobileAppContentFile object.</span></span>

<span data-ttu-id="7f6f3-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „mobileAppContentFile“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="7f6f3-125">The following table shows the properties that are required when you create the mobileAppContentFile.</span></span>

|<span data-ttu-id="7f6f3-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7f6f3-126">Property</span></span>|<span data-ttu-id="7f6f3-127">Typ</span><span class="sxs-lookup"><span data-stu-id="7f6f3-127">Type</span></span>|<span data-ttu-id="7f6f3-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7f6f3-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7f6f3-129">azureStorageUri</span><span class="sxs-lookup"><span data-stu-id="7f6f3-129">azureStorageUri</span></span>|<span data-ttu-id="7f6f3-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7f6f3-130">String</span></span>|<span data-ttu-id="7f6f3-131">Azure Storage-URI</span><span class="sxs-lookup"><span data-stu-id="7f6f3-131">The Azure Storage URI.</span></span>|
|<span data-ttu-id="7f6f3-132">isCommitted</span><span class="sxs-lookup"><span data-stu-id="7f6f3-132">isCommitted</span></span>|<span data-ttu-id="7f6f3-133">Boolesch</span><span class="sxs-lookup"><span data-stu-id="7f6f3-133">Boolean</span></span>|<span data-ttu-id="7f6f3-134">Wert, der angibt, ob für die Datei ein Commit ausgeführt wurde</span><span class="sxs-lookup"><span data-stu-id="7f6f3-134">A value indicating whether the file is committed.</span></span>|
|<span data-ttu-id="7f6f3-135">id</span><span class="sxs-lookup"><span data-stu-id="7f6f3-135">id</span></span>|<span data-ttu-id="7f6f3-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7f6f3-136">String</span></span>|<span data-ttu-id="7f6f3-137">ID der Datei</span><span class="sxs-lookup"><span data-stu-id="7f6f3-137">The File Id.</span></span>|
|<span data-ttu-id="7f6f3-138">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7f6f3-138">createdDateTime</span></span>|<span data-ttu-id="7f6f3-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7f6f3-139">DateTimeOffset</span></span>|<span data-ttu-id="7f6f3-140">Datum und Uhrzeit der Erstellung der Datei</span><span class="sxs-lookup"><span data-stu-id="7f6f3-140">The time the file was created.</span></span>|
|<span data-ttu-id="7f6f3-141">name</span><span class="sxs-lookup"><span data-stu-id="7f6f3-141">name</span></span>|<span data-ttu-id="7f6f3-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7f6f3-142">String</span></span>|<span data-ttu-id="7f6f3-143">Name der Datei</span><span class="sxs-lookup"><span data-stu-id="7f6f3-143">the file name.</span></span>|
|<span data-ttu-id="7f6f3-144">size</span><span class="sxs-lookup"><span data-stu-id="7f6f3-144">size</span></span>|<span data-ttu-id="7f6f3-145">Int64</span><span class="sxs-lookup"><span data-stu-id="7f6f3-145">Int64</span></span>|<span data-ttu-id="7f6f3-146">Größe der Datei vor der Verschlüsselung</span><span class="sxs-lookup"><span data-stu-id="7f6f3-146">The size of the file prior to encryption.</span></span>|
|<span data-ttu-id="7f6f3-147">sizeEncrypted</span><span class="sxs-lookup"><span data-stu-id="7f6f3-147">sizeEncrypted</span></span>|<span data-ttu-id="7f6f3-148">Int64</span><span class="sxs-lookup"><span data-stu-id="7f6f3-148">Int64</span></span>|<span data-ttu-id="7f6f3-149">Größe der Datei nach der Verschlüsselung</span><span class="sxs-lookup"><span data-stu-id="7f6f3-149">The size of the file after encryption.</span></span>|
|<span data-ttu-id="7f6f3-150">azureStorageUriExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="7f6f3-150">azureStorageUriExpirationDateTime</span></span>|<span data-ttu-id="7f6f3-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7f6f3-151">DateTimeOffset</span></span>|<span data-ttu-id="7f6f3-152">Datum und Uhrzeit des Ablaufs des Azure Storage-URI</span><span class="sxs-lookup"><span data-stu-id="7f6f3-152">The time the Azure storage Uri expires.</span></span>|
|<span data-ttu-id="7f6f3-153">manifest</span><span class="sxs-lookup"><span data-stu-id="7f6f3-153">manifest</span></span>|<span data-ttu-id="7f6f3-154">Binär</span><span class="sxs-lookup"><span data-stu-id="7f6f3-154">Binary</span></span>|<span data-ttu-id="7f6f3-155">Manifestinformationen</span><span class="sxs-lookup"><span data-stu-id="7f6f3-155">The manifest information.</span></span>|
|<span data-ttu-id="7f6f3-156">uploadState</span><span class="sxs-lookup"><span data-stu-id="7f6f3-156">uploadState</span></span>|[<span data-ttu-id="7f6f3-157">mobileAppContentFileUploadState</span><span class="sxs-lookup"><span data-stu-id="7f6f3-157">mobileAppContentFileUploadState</span></span>](../resources/intune_apps_mobileappcontentfileuploadstate.md)|<span data-ttu-id="7f6f3-158">Status der aktuellen Uploadanforderung.</span><span class="sxs-lookup"><span data-stu-id="7f6f3-158">The state of the current upload request.</span></span> <span data-ttu-id="7f6f3-159">Mögliche Werte sind: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed` und `commitFileTimedOut`.</span><span class="sxs-lookup"><span data-stu-id="7f6f3-159">Possible values are: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed`, `commitFileTimedOut`.</span></span>|



## <a name="response"></a><span data-ttu-id="7f6f3-160">Antwort</span><span class="sxs-lookup"><span data-stu-id="7f6f3-160">Response</span></span>
<span data-ttu-id="7f6f3-161">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [mobileAppContentFile](../resources/intune_apps_mobileappcontentfile.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="7f6f3-161">If successful, this method returns a `201 Created` response code and a [mobileAppContentFile](../resources/intune_apps_mobileappcontentfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7f6f3-162">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7f6f3-162">Example</span></span>
### <a name="request"></a><span data-ttu-id="7f6f3-163">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7f6f3-163">Request</span></span>
<span data-ttu-id="7f6f3-164">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7f6f3-164">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files
Content-type: application/json
Content-length: 342

{
  "@odata.type": "#microsoft.graph.mobileAppContentFile",
  "azureStorageUri": "Azure Storage Uri value",
  "isCommitted": true,
  "name": "Name value",
  "size": 4,
  "sizeEncrypted": 13,
  "azureStorageUriExpirationDateTime": "2017-01-01T00:00:08.4940464-08:00",
  "manifest": "bWFuaWZlc3Q=",
  "uploadState": "transientError"
}
```

### <a name="response"></a><span data-ttu-id="7f6f3-165">Antwort</span><span class="sxs-lookup"><span data-stu-id="7f6f3-165">Response</span></span>
<span data-ttu-id="7f6f3-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7f6f3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 450

{
  "@odata.type": "#microsoft.graph.mobileAppContentFile",
  "azureStorageUri": "Azure Storage Uri value",
  "isCommitted": true,
  "id": "eab2e29b-e29b-eab2-9be2-b2ea9be2b2ea",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "name": "Name value",
  "size": 4,
  "sizeEncrypted": 13,
  "azureStorageUriExpirationDateTime": "2017-01-01T00:00:08.4940464-08:00",
  "manifest": "bWFuaWZlc3Q=",
  "uploadState": "transientError"
}
```








