# <a name="create-androidforworkenrollmentprofile"></a><span data-ttu-id="530e8-101">Erstellen von „androidForWorkEnrollmentProfile“</span><span class="sxs-lookup"><span data-stu-id="530e8-101">Create androidForWorkEnrollmentProfile</span></span>

> <span data-ttu-id="530e8-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="530e8-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="530e8-103">Erstellen eines neuen [androidForWorkEnrollmentProfile](../resources/intune_androidforwork_androidforworkenrollmentprofile.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="530e8-103">Create a new [plannerBucket](../resources/intune_androidforwork_androidforworkenrollmentprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="530e8-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="530e8-104">Prerequisites</span></span>
<span data-ttu-id="530e8-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="530e8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="530e8-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="530e8-107">Permission type</span></span>|<span data-ttu-id="530e8-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="530e8-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="530e8-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="530e8-109">Delegated (work or school account)</span></span>|<span data-ttu-id="530e8-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="530e8-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="530e8-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="530e8-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="530e8-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="530e8-112">Not supported.</span></span>|
|<span data-ttu-id="530e8-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="530e8-113">Application</span></span>|<span data-ttu-id="530e8-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="530e8-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="530e8-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="530e8-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidForWorkEnrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="530e8-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="530e8-116">Request headers</span></span>
|<span data-ttu-id="530e8-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="530e8-117">Header</span></span>|<span data-ttu-id="530e8-118">Wert</span><span class="sxs-lookup"><span data-stu-id="530e8-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="530e8-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="530e8-119">Authorization</span></span>|<span data-ttu-id="530e8-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="530e8-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="530e8-121">Annehmen</span><span class="sxs-lookup"><span data-stu-id="530e8-121">Accept</span></span>|<span data-ttu-id="530e8-122">application/json</span><span class="sxs-lookup"><span data-stu-id="530e8-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="530e8-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="530e8-123">Request body</span></span>
<span data-ttu-id="530e8-124">Geben Sie im Anforderungstext eine JSON-Darstellung des androidForWorkEnrollmentProfile-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="530e8-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="530e8-125">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen des androidForWorkEnrollmentProfile erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="530e8-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="530e8-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="530e8-126">Property</span></span>|<span data-ttu-id="530e8-127">Typ</span><span class="sxs-lookup"><span data-stu-id="530e8-127">Type</span></span>|<span data-ttu-id="530e8-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="530e8-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="530e8-129">accountId</span><span class="sxs-lookup"><span data-stu-id="530e8-129">accountId</span></span>|<span data-ttu-id="530e8-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="530e8-130">String</span></span>|<span data-ttu-id="530e8-131">Mandanten-GUID, zu der das Registrierungsprofil gehört.</span><span class="sxs-lookup"><span data-stu-id="530e8-131">Tenant GUID the enrollment profile belongs to.</span></span>|
|<span data-ttu-id="530e8-132">id</span><span class="sxs-lookup"><span data-stu-id="530e8-132">id</span></span>|<span data-ttu-id="530e8-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="530e8-133">String</span></span>|<span data-ttu-id="530e8-134">Eindeutige GUID des Registrierungsprofils.</span><span class="sxs-lookup"><span data-stu-id="530e8-134">Unique GUID for the enrollment profile.</span></span>|
|<span data-ttu-id="530e8-135">name</span><span class="sxs-lookup"><span data-stu-id="530e8-135">name</span></span>|<span data-ttu-id="530e8-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="530e8-136">String</span></span>|<span data-ttu-id="530e8-137">Anzeigename des Registrierungsprofils (veraltet).</span><span class="sxs-lookup"><span data-stu-id="530e8-137">(Deprecated) Display name for the enrollment profile.</span></span>|
|<span data-ttu-id="530e8-138">displayName</span><span class="sxs-lookup"><span data-stu-id="530e8-138">displayName</span></span>|<span data-ttu-id="530e8-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="530e8-139">String</span></span>|<span data-ttu-id="530e8-140">Anzeigename des Registrierungsprofils.</span><span class="sxs-lookup"><span data-stu-id="530e8-140">Display name for the enrollment profile.</span></span>|
|<span data-ttu-id="530e8-141">description</span><span class="sxs-lookup"><span data-stu-id="530e8-141">description</span></span>|<span data-ttu-id="530e8-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="530e8-142">String</span></span>|<span data-ttu-id="530e8-143">Beschreibung des Registrierungsprofils.</span><span class="sxs-lookup"><span data-stu-id="530e8-143">Description for the enrollment profile.</span></span>|
|<span data-ttu-id="530e8-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="530e8-144">createdDateTime</span></span>|<span data-ttu-id="530e8-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="530e8-145">DateTimeOffset</span></span>|<span data-ttu-id="530e8-146">Datum und Uhrzeit der Erstellung des Registrierungsprofils.</span><span class="sxs-lookup"><span data-stu-id="530e8-146">Date time the enrollment profile was created.</span></span>|
|<span data-ttu-id="530e8-147">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="530e8-147">modifiedDateTime</span></span>|<span data-ttu-id="530e8-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="530e8-148">DateTimeOffset</span></span>|<span data-ttu-id="530e8-149">Datum und Uhrzeit der letzten Änderung des Registrierungsprofils (veraltet).</span><span class="sxs-lookup"><span data-stu-id="530e8-149">(Deprecated) Date time the enrollment profile was last modified.</span></span>|
|<span data-ttu-id="530e8-150">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="530e8-150">lastModifiedDateTime</span></span>|<span data-ttu-id="530e8-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="530e8-151">DateTimeOffset</span></span>|<span data-ttu-id="530e8-152">Datum und Uhrzeit der letzten Änderung des Registrierungsprofils.</span><span class="sxs-lookup"><span data-stu-id="530e8-152">Date time the enrollment profile was last modified.</span></span>|
|<span data-ttu-id="530e8-153">tokenValue</span><span class="sxs-lookup"><span data-stu-id="530e8-153">tokenValue</span></span>|<span data-ttu-id="530e8-154">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="530e8-154">String</span></span>|<span data-ttu-id="530e8-155">Wert des zuletzt für das Registrierungsprofil erstellten Tokens.</span><span class="sxs-lookup"><span data-stu-id="530e8-155">Value of the most recently created token for this enrollment profile.</span></span>|
|<span data-ttu-id="530e8-156">tokenExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="530e8-156">tokenExpirationDateTime</span></span>|<span data-ttu-id="530e8-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="530e8-157">DateTimeOffset</span></span>|<span data-ttu-id="530e8-158">Datum und Uhrzeit des Ablaufs des zuletzt erstellten Tokens.</span><span class="sxs-lookup"><span data-stu-id="530e8-158">Date time the most recently created token will expire.</span></span>|
|<span data-ttu-id="530e8-159">totalEnrollmentCount</span><span class="sxs-lookup"><span data-stu-id="530e8-159">totalEnrollmentCount</span></span>|<span data-ttu-id="530e8-160">Int32</span><span class="sxs-lookup"><span data-stu-id="530e8-160">Int32</span></span>|<span data-ttu-id="530e8-161">Gesamtzahl der mit dem Registrierungsprofil registrierten Android-Geräte (veraltet).</span><span class="sxs-lookup"><span data-stu-id="530e8-161">(Deprecated) Total number of Android devices that have enrolled using this enrollment profile.</span></span>|
|<span data-ttu-id="530e8-162">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="530e8-162">enrolledDeviceCount</span></span>|<span data-ttu-id="530e8-163">Int32</span><span class="sxs-lookup"><span data-stu-id="530e8-163">Int32</span></span>|<span data-ttu-id="530e8-164">Gesamtzahl der mit dem Registrierungsprofil registrierten Android-Geräte.</span><span class="sxs-lookup"><span data-stu-id="530e8-164">Total number of Android devices that have enrolled using this enrollment profile.</span></span>|
|<span data-ttu-id="530e8-165">qrCode</span><span class="sxs-lookup"><span data-stu-id="530e8-165">qrCode</span></span>|<span data-ttu-id="530e8-166">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="530e8-166">String</span></span>|<span data-ttu-id="530e8-167">Zeichenfolge, die zur Generierung eines QR-Codes für das Token verwendet wird (veraltet).</span><span class="sxs-lookup"><span data-stu-id="530e8-167">(Deprecated) String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="530e8-168">qrCodeContent</span><span class="sxs-lookup"><span data-stu-id="530e8-168">qrCodeContent</span></span>|<span data-ttu-id="530e8-169">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="530e8-169">String</span></span>|<span data-ttu-id="530e8-170">Zeichenfolge, die zur Generierung eines QR-Codes für das Token verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="530e8-170">String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="530e8-171">qrCodeImage</span><span class="sxs-lookup"><span data-stu-id="530e8-171">qrCodeImage</span></span>|[<span data-ttu-id="530e8-172">mimeContent</span><span class="sxs-lookup"><span data-stu-id="530e8-172">mimeContent</span></span>](../resources/intune_androidforwork_mimecontent.md)|<span data-ttu-id="530e8-173">Zeichenfolge, die zur Generierung eines QR-Codes für das Token verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="530e8-173">String used to generate a QR code for the token.</span></span>|



## <a name="response"></a><span data-ttu-id="530e8-174">Antwort</span><span class="sxs-lookup"><span data-stu-id="530e8-174">Response</span></span>
<span data-ttu-id="530e8-175">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [androidForWorkEnrollmentProfile](../resources/intune_androidforwork_androidforworkenrollmentprofile.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="530e8-175">If successful, this method returns a `201 Created` response code and a [section](../resources/intune_androidforwork_androidforworkenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="530e8-176">Beispiel</span><span class="sxs-lookup"><span data-stu-id="530e8-176">Example</span></span>
### <a name="request"></a><span data-ttu-id="530e8-177">Anforderung</span><span class="sxs-lookup"><span data-stu-id="530e8-177">Request</span></span>
<span data-ttu-id="530e8-178">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="530e8-178">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/androidForWorkEnrollmentProfiles
Content-type: application/json
Content-length: 645

{
  "@odata.type": "#microsoft.graph.androidForWorkEnrollmentProfile",
  "accountId": "Account Id value",
  "name": "Name value",
  "displayName": "Display Name value",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "tokenValue": "Token Value value",
  "tokenExpirationDateTime": "2016-12-31T23:59:54.0590989-08:00",
  "totalEnrollmentCount": 4,
  "enrolledDeviceCount": 3,
  "qrCode": "Qr Code value",
  "qrCodeContent": "Qr Code Content value",
  "qrCodeImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  }
}
```

### <a name="response"></a><span data-ttu-id="530e8-179">Antwort</span><span class="sxs-lookup"><span data-stu-id="530e8-179">Response</span></span>
<span data-ttu-id="530e8-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="530e8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 813

{
  "@odata.type": "#microsoft.graph.androidForWorkEnrollmentProfile",
  "accountId": "Account Id value",
  "id": "e6742553-2553-e674-5325-74e6532574e6",
  "name": "Name value",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "tokenValue": "Token Value value",
  "tokenExpirationDateTime": "2016-12-31T23:59:54.0590989-08:00",
  "totalEnrollmentCount": 4,
  "enrolledDeviceCount": 3,
  "qrCode": "Qr Code value",
  "qrCodeContent": "Qr Code Content value",
  "qrCodeImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  }
}
```



