# <a name="update-androidforworkenrollmentprofile"></a><span data-ttu-id="77735-101">Aktualisieren von „androidForWorkEnrollmentProfile“</span><span class="sxs-lookup"><span data-stu-id="77735-101">Update androidForWorkEnrollmentProfile</span></span>

> <span data-ttu-id="77735-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="77735-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="77735-103">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [androidForWorkEnrollmentProfile](../resources/intune_androidforwork_androidforworkenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="77735-103">Update the properties of a [calendar](../resources/intune_androidforwork_androidforworkenrollmentprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="77735-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="77735-104">Prerequisites</span></span>
<span data-ttu-id="77735-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="77735-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="77735-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="77735-107">Permission type</span></span>|<span data-ttu-id="77735-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="77735-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="77735-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="77735-109">Delegated (work or school account)</span></span>|<span data-ttu-id="77735-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77735-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="77735-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="77735-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="77735-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="77735-112">Not supported.</span></span>|
|<span data-ttu-id="77735-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="77735-113">Application</span></span>|<span data-ttu-id="77735-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="77735-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="77735-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="77735-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidForWorkEnrollmentProfiles/{androidForWorkEnrollmentProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="77735-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="77735-116">Request headers</span></span>
|<span data-ttu-id="77735-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="77735-117">Header</span></span>|<span data-ttu-id="77735-118">Wert</span><span class="sxs-lookup"><span data-stu-id="77735-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="77735-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="77735-119">Authorization</span></span>|<span data-ttu-id="77735-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="77735-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="77735-121">Accept</span><span class="sxs-lookup"><span data-stu-id="77735-121">Accept</span></span>|<span data-ttu-id="77735-122">application/json</span><span class="sxs-lookup"><span data-stu-id="77735-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="77735-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="77735-123">Request body</span></span>
<span data-ttu-id="77735-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [androidForWorkEnrollmentProfile](../resources/intune_androidforwork_androidforworkenrollmentprofile.md) an.</span><span class="sxs-lookup"><span data-stu-id="77735-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_androidforwork_androidforworkenrollmentprofile.md) object.</span></span>

<span data-ttu-id="77735-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [androidForWorkEnrollmentProfile](../resources/intune_androidforwork_androidforworkenrollmentprofile.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="77735-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="77735-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="77735-126">Property</span></span>|<span data-ttu-id="77735-127">Typ</span><span class="sxs-lookup"><span data-stu-id="77735-127">Type</span></span>|<span data-ttu-id="77735-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="77735-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="77735-129">accountId</span><span class="sxs-lookup"><span data-stu-id="77735-129">accountId</span></span>|<span data-ttu-id="77735-130">String</span><span class="sxs-lookup"><span data-stu-id="77735-130">String</span></span>|<span data-ttu-id="77735-131">Mandanten-GUID, zu der das Registrierungsprofil gehört</span><span class="sxs-lookup"><span data-stu-id="77735-131">Tenant GUID the enrollment profile belongs to.</span></span>|
|<span data-ttu-id="77735-132">id</span><span class="sxs-lookup"><span data-stu-id="77735-132">id</span></span>|<span data-ttu-id="77735-133">String</span><span class="sxs-lookup"><span data-stu-id="77735-133">String</span></span>|<span data-ttu-id="77735-134">Eindeutige GUID des Registrierungsprofils</span><span class="sxs-lookup"><span data-stu-id="77735-134">Unique GUID for the enrollment profile.</span></span>|
|<span data-ttu-id="77735-135">name</span><span class="sxs-lookup"><span data-stu-id="77735-135">name</span></span>|<span data-ttu-id="77735-136">String</span><span class="sxs-lookup"><span data-stu-id="77735-136">String</span></span>|<span data-ttu-id="77735-137">Anzeigename des Registrierungsprofils (veraltet)</span><span class="sxs-lookup"><span data-stu-id="77735-137">(Deprecated) Display name for the enrollment profile.</span></span>|
|<span data-ttu-id="77735-138">displayName</span><span class="sxs-lookup"><span data-stu-id="77735-138">displayName</span></span>|<span data-ttu-id="77735-139">String</span><span class="sxs-lookup"><span data-stu-id="77735-139">String</span></span>|<span data-ttu-id="77735-140">Anzeigename des Registrierungsprofils</span><span class="sxs-lookup"><span data-stu-id="77735-140">Display name for the enrollment profile.</span></span>|
|<span data-ttu-id="77735-141">description</span><span class="sxs-lookup"><span data-stu-id="77735-141">description</span></span>|<span data-ttu-id="77735-142">String</span><span class="sxs-lookup"><span data-stu-id="77735-142">String</span></span>|<span data-ttu-id="77735-143">Beschreibung des Registrierungsprofils</span><span class="sxs-lookup"><span data-stu-id="77735-143">Description for the enrollment profile.</span></span>|
|<span data-ttu-id="77735-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="77735-144">createdDateTime</span></span>|<span data-ttu-id="77735-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="77735-145">DateTimeOffset</span></span>|<span data-ttu-id="77735-146">Datum und Uhrzeit der Erstellung des Registrierungsprofils</span><span class="sxs-lookup"><span data-stu-id="77735-146">Date time the enrollment profile was created.</span></span>|
|<span data-ttu-id="77735-147">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="77735-147">modifiedDateTime</span></span>|<span data-ttu-id="77735-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="77735-148">DateTimeOffset</span></span>|<span data-ttu-id="77735-149">Datum und Uhrzeit der letzten Änderung des Registrierungsprofils (veraltet)</span><span class="sxs-lookup"><span data-stu-id="77735-149">(Deprecated) Date time the enrollment profile was last modified.</span></span>|
|<span data-ttu-id="77735-150">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="77735-150">lastModifiedDateTime</span></span>|<span data-ttu-id="77735-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="77735-151">DateTimeOffset</span></span>|<span data-ttu-id="77735-152">Datum und Uhrzeit der letzten Änderung des Registrierungsprofils</span><span class="sxs-lookup"><span data-stu-id="77735-152">Date time the enrollment profile was last modified.</span></span>|
|<span data-ttu-id="77735-153">tokenValue</span><span class="sxs-lookup"><span data-stu-id="77735-153">tokenValue</span></span>|<span data-ttu-id="77735-154">String</span><span class="sxs-lookup"><span data-stu-id="77735-154">String</span></span>|<span data-ttu-id="77735-155">Wert des zuletzt für das Registrierungsprofil erstellten Tokens</span><span class="sxs-lookup"><span data-stu-id="77735-155">Value of the most recently created token for this enrollment profile.</span></span>|
|<span data-ttu-id="77735-156">tokenExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="77735-156">tokenExpirationDateTime</span></span>|<span data-ttu-id="77735-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="77735-157">DateTimeOffset</span></span>|<span data-ttu-id="77735-158">Datum und Uhrzeit des Ablaufs des zuletzt erstellten Tokens</span><span class="sxs-lookup"><span data-stu-id="77735-158">Date time the most recently created token will expire.</span></span>|
|<span data-ttu-id="77735-159">totalEnrollmentCount</span><span class="sxs-lookup"><span data-stu-id="77735-159">totalEnrollmentCount</span></span>|<span data-ttu-id="77735-160">Int32</span><span class="sxs-lookup"><span data-stu-id="77735-160">Int32</span></span>|<span data-ttu-id="77735-161">Gesamtzahl der mit dem Registrierungsprofil registrierten Android-Geräte (veraltet)</span><span class="sxs-lookup"><span data-stu-id="77735-161">(Deprecated) Total number of Android devices that have enrolled using this enrollment profile.</span></span>|
|<span data-ttu-id="77735-162">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="77735-162">enrolledDeviceCount</span></span>|<span data-ttu-id="77735-163">Int32</span><span class="sxs-lookup"><span data-stu-id="77735-163">Int32</span></span>|<span data-ttu-id="77735-164">Gesamtzahl der mit dem Registrierungsprofil registrierten Android-Geräte</span><span class="sxs-lookup"><span data-stu-id="77735-164">Total number of Android devices that have enrolled using this enrollment profile.</span></span>|
|<span data-ttu-id="77735-165">qrCode</span><span class="sxs-lookup"><span data-stu-id="77735-165">qrCode</span></span>|<span data-ttu-id="77735-166">String</span><span class="sxs-lookup"><span data-stu-id="77735-166">String</span></span>|<span data-ttu-id="77735-167">Zeichenfolge, die zur Generierung eines QR-Codes für das Token verwendet wird (veraltet)</span><span class="sxs-lookup"><span data-stu-id="77735-167">(Deprecated) String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="77735-168">qrCodeContent</span><span class="sxs-lookup"><span data-stu-id="77735-168">qrCodeContent</span></span>|<span data-ttu-id="77735-169">String</span><span class="sxs-lookup"><span data-stu-id="77735-169">String</span></span>|<span data-ttu-id="77735-170">Zeichenfolge, die zur Generierung eines QR-Codes für das Token verwendet wird</span><span class="sxs-lookup"><span data-stu-id="77735-170">String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="77735-171">qrCodeImage</span><span class="sxs-lookup"><span data-stu-id="77735-171">qrCodeImage</span></span>|[<span data-ttu-id="77735-172">mimeContent</span><span class="sxs-lookup"><span data-stu-id="77735-172">mimeContent</span></span>](../resources/intune_androidforwork_mimecontent.md)|<span data-ttu-id="77735-173">Zeichenfolge, die zur Generierung eines QR-Codes für das Token verwendet wird</span><span class="sxs-lookup"><span data-stu-id="77735-173">String used to generate a QR code for the token.</span></span>|



## <a name="response"></a><span data-ttu-id="77735-174">Antwort</span><span class="sxs-lookup"><span data-stu-id="77735-174">Response</span></span>
<span data-ttu-id="77735-175">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [androidForWorkEnrollmentProfile](../resources/intune_androidforwork_androidforworkenrollmentprofile.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="77735-175">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_androidforwork_androidforworkenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="77735-176">Beispiel</span><span class="sxs-lookup"><span data-stu-id="77735-176">Example</span></span>
### <a name="request"></a><span data-ttu-id="77735-177">Anforderung</span><span class="sxs-lookup"><span data-stu-id="77735-177">Request</span></span>
<span data-ttu-id="77735-178">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="77735-178">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/androidForWorkEnrollmentProfiles/{androidForWorkEnrollmentProfileId}
Content-type: application/json
Content-length: 575

{
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

### <a name="response"></a><span data-ttu-id="77735-179">Antwort</span><span class="sxs-lookup"><span data-stu-id="77735-179">Response</span></span>
<span data-ttu-id="77735-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="77735-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



