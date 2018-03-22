# <a name="update-mobileappcontentfile"></a><span data-ttu-id="db56c-101">mobileAppContentFile aktualisieren</span><span class="sxs-lookup"><span data-stu-id="db56c-101">Update mobileAppContentFile</span></span>

> <span data-ttu-id="db56c-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="db56c-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="db56c-103">Aktualisieren der Eigenschaften eines [MobileAppContentFile](../resources/intune_apps_mobileappcontentfile.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="db56c-103">Update the properties of a [calendar](../resources/intune_apps_mobileappcontentfile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="db56c-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="db56c-104">Prerequisites</span></span>
<span data-ttu-id="db56c-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="db56c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="db56c-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="db56c-107">Permission type</span></span>|<span data-ttu-id="db56c-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="db56c-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="db56c-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="db56c-109">Delegated (work or school account)</span></span>|<span data-ttu-id="db56c-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db56c-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="db56c-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="db56c-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="db56c-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="db56c-112">Not supported.</span></span>|
|<span data-ttu-id="db56c-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="db56c-113">Application</span></span>|<span data-ttu-id="db56c-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="db56c-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="db56c-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="db56c-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files/{mobileAppContentFileId}
```

## <a name="request-headers"></a><span data-ttu-id="db56c-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="db56c-116">Request headers</span></span>
|<span data-ttu-id="db56c-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="db56c-117">Header</span></span>|<span data-ttu-id="db56c-118">Wert</span><span class="sxs-lookup"><span data-stu-id="db56c-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="db56c-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="db56c-119">Authorization</span></span>|<span data-ttu-id="db56c-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="db56c-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="db56c-121">Annehmen</span><span class="sxs-lookup"><span data-stu-id="db56c-121">Accept</span></span>|<span data-ttu-id="db56c-122">application/json</span><span class="sxs-lookup"><span data-stu-id="db56c-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="db56c-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="db56c-123">Request body</span></span>
<span data-ttu-id="db56c-124">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs [mobileAppContentFile](../resources/intune_apps_mobileappcontentfile.md) an.</span><span class="sxs-lookup"><span data-stu-id="db56c-124">In the request body, supply a JSON representation of [ContactFolder](../resources/intune_apps_mobileappcontentfile.md) object.</span></span>

<span data-ttu-id="db56c-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [mobileAppContentFile](../resources/intune_apps_mobileappcontentfile.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="db56c-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="db56c-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="db56c-126">Property</span></span>|<span data-ttu-id="db56c-127">Typ</span><span class="sxs-lookup"><span data-stu-id="db56c-127">Type</span></span>|<span data-ttu-id="db56c-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="db56c-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="db56c-129">azureStorageUri</span><span class="sxs-lookup"><span data-stu-id="db56c-129">azureStorageUri</span></span>|<span data-ttu-id="db56c-130">String</span><span class="sxs-lookup"><span data-stu-id="db56c-130">String</span></span>|<span data-ttu-id="db56c-131">Der Azure Storage-URI.</span><span class="sxs-lookup"><span data-stu-id="db56c-131">The Azure Storage URI.</span></span>|
|<span data-ttu-id="db56c-132">isCommitted</span><span class="sxs-lookup"><span data-stu-id="db56c-132">isCommitted</span></span>|<span data-ttu-id="db56c-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="db56c-133">Boolean</span></span>|<span data-ttu-id="db56c-134">Ein Wert, der angibt, ob für die Datei ein Commit ausgeführt wurde.</span><span class="sxs-lookup"><span data-stu-id="db56c-134">A value indicating whether the file is committed.</span></span>|
|<span data-ttu-id="db56c-135">id</span><span class="sxs-lookup"><span data-stu-id="db56c-135">id</span></span>|<span data-ttu-id="db56c-136">String</span><span class="sxs-lookup"><span data-stu-id="db56c-136">String</span></span>|<span data-ttu-id="db56c-137">Die Datei-ID</span><span class="sxs-lookup"><span data-stu-id="db56c-137">The File Id.</span></span>|
|<span data-ttu-id="db56c-138">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="db56c-138">createdDateTime</span></span>|<span data-ttu-id="db56c-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="db56c-139">DateTimeOffset</span></span>|<span data-ttu-id="db56c-140">Der Zeitpunkt der Erstellung der Datei</span><span class="sxs-lookup"><span data-stu-id="db56c-140">The time the file was created.</span></span>|
|<span data-ttu-id="db56c-141">name</span><span class="sxs-lookup"><span data-stu-id="db56c-141">name</span></span>|<span data-ttu-id="db56c-142">String</span><span class="sxs-lookup"><span data-stu-id="db56c-142">String</span></span>|<span data-ttu-id="db56c-143">Der Dateiname</span><span class="sxs-lookup"><span data-stu-id="db56c-143">The file name.</span></span>|
|<span data-ttu-id="db56c-144">size</span><span class="sxs-lookup"><span data-stu-id="db56c-144">size</span></span>|<span data-ttu-id="db56c-145">Int64</span><span class="sxs-lookup"><span data-stu-id="db56c-145">Int64</span></span>|<span data-ttu-id="db56c-146">Die Größe der Datei vor der Verschlüsselung.</span><span class="sxs-lookup"><span data-stu-id="db56c-146">The size of the file prior to encryption.</span></span>|
|<span data-ttu-id="db56c-147">sizeEncrypted</span><span class="sxs-lookup"><span data-stu-id="db56c-147">sizeEncrypted</span></span>|<span data-ttu-id="db56c-148">Int64</span><span class="sxs-lookup"><span data-stu-id="db56c-148">Int64</span></span>|<span data-ttu-id="db56c-149">Die Größe der Datei nach der Verschlüsselung.</span><span class="sxs-lookup"><span data-stu-id="db56c-149">The size of the file after encryption.</span></span>|
|<span data-ttu-id="db56c-150">azureStorageUriExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="db56c-150">azureStorageUriExpirationDateTime</span></span>|<span data-ttu-id="db56c-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="db56c-151">DateTimeOffset</span></span>|<span data-ttu-id="db56c-152">Die Zeit, zu der der Azure Storage-URI abläuft.</span><span class="sxs-lookup"><span data-stu-id="db56c-152">The time the Azure storage Uri expires.</span></span>|
|<span data-ttu-id="db56c-153">manifest</span><span class="sxs-lookup"><span data-stu-id="db56c-153">manifest</span></span>|<span data-ttu-id="db56c-154">Binär</span><span class="sxs-lookup"><span data-stu-id="db56c-154">Binary</span></span>|<span data-ttu-id="db56c-155">Die Manifestinformationen</span><span class="sxs-lookup"><span data-stu-id="db56c-155">The manifest information.</span></span>|
|<span data-ttu-id="db56c-156">uploadState</span><span class="sxs-lookup"><span data-stu-id="db56c-156">uploadState</span></span>|<span data-ttu-id="db56c-157">String</span><span class="sxs-lookup"><span data-stu-id="db56c-157">String</span></span>|<span data-ttu-id="db56c-158">Der Status der aktuellen Uploadanforderung.</span><span class="sxs-lookup"><span data-stu-id="db56c-158">The state of the current upload request.</span></span> <span data-ttu-id="db56c-159">Mögliche Werte sind: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed` und `commitFileTimedOut`.</span><span class="sxs-lookup"><span data-stu-id="db56c-159">Possible values are: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed`, `commitFileTimedOut`.</span></span>|



## <a name="response"></a><span data-ttu-id="db56c-160">Antwort</span><span class="sxs-lookup"><span data-stu-id="db56c-160">Response</span></span>
<span data-ttu-id="db56c-161">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [mobileAppContentFile](../resources/intune_apps_mobileappcontentfile.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="db56c-161">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_apps_mobileappcontentfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="db56c-162">Beispiel</span><span class="sxs-lookup"><span data-stu-id="db56c-162">Example</span></span>
### <a name="request"></a><span data-ttu-id="db56c-163">Anforderung</span><span class="sxs-lookup"><span data-stu-id="db56c-163">Request</span></span>
<span data-ttu-id="db56c-164">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="db56c-164">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files/{mobileAppContentFileId}
Content-type: application/json
Content-length: 283

{
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

### <a name="response"></a><span data-ttu-id="db56c-165">Antwort</span><span class="sxs-lookup"><span data-stu-id="db56c-165">Response</span></span>
<span data-ttu-id="db56c-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="db56c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



