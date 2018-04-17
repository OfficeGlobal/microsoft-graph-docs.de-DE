# <a name="create-vpptoken"></a><span data-ttu-id="283de-101">VppToken erstellen</span><span class="sxs-lookup"><span data-stu-id="283de-101">Create vppToken</span></span>

> <span data-ttu-id="283de-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="283de-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="283de-103">Erstellen Sie ein neues [VppToken](../resources/intune_onboarding_vpptoken.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="283de-103">Create a new [iosManagedAppRegistration](../resources/intune_onboarding_vpptoken.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="283de-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="283de-104">Prerequisites</span></span>
<span data-ttu-id="283de-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="283de-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="283de-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="283de-107">Permission type</span></span>|<span data-ttu-id="283de-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="283de-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="283de-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="283de-109">Delegated (work or school account)</span></span>|<span data-ttu-id="283de-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="283de-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="283de-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="283de-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="283de-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="283de-112">Not supported.</span></span>|
|<span data-ttu-id="283de-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="283de-113">Application</span></span>|<span data-ttu-id="283de-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="283de-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="283de-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="283de-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/vppTokens
```

## <a name="request-headers"></a><span data-ttu-id="283de-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="283de-116">Request headers</span></span>
|<span data-ttu-id="283de-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="283de-117">Header</span></span>|<span data-ttu-id="283de-118">Wert</span><span class="sxs-lookup"><span data-stu-id="283de-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="283de-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="283de-119">Authorization</span></span>|<span data-ttu-id="283de-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="283de-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="283de-121">Accept</span><span class="sxs-lookup"><span data-stu-id="283de-121">Accept</span></span>|<span data-ttu-id="283de-122">application/json</span><span class="sxs-lookup"><span data-stu-id="283de-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="283de-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="283de-123">Request body</span></span>
<span data-ttu-id="283de-124">Geben Sie im Anforderungstext eine JSON-Darstellung des vppToken-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="283de-124">In the request body, supply a JSON representation for the softwareUpdateStatusSummary object.</span></span>

<span data-ttu-id="283de-125">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen des vppToken erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="283de-125">The following table shows the properties that are required when you create the windows10TeamGeneralConfiguration.</span></span>

|<span data-ttu-id="283de-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="283de-126">Property</span></span>|<span data-ttu-id="283de-127">Typ</span><span class="sxs-lookup"><span data-stu-id="283de-127">Type</span></span>|<span data-ttu-id="283de-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="283de-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="283de-129">id</span><span class="sxs-lookup"><span data-stu-id="283de-129">id</span></span>|<span data-ttu-id="283de-130">String</span><span class="sxs-lookup"><span data-stu-id="283de-130">String</span></span>|<span data-ttu-id="283de-131">Wird automatisch generiert, wenn AppleVolumePurchaseProgramToken erstellt wird.</span><span class="sxs-lookup"><span data-stu-id="283de-131">This is automatically generated when the appleVolumePurchaseProgramToken is created.</span></span> <span data-ttu-id="283de-132">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="283de-132">It is the Key of the entity.</span></span>|
|<span data-ttu-id="283de-133">organizationName</span><span class="sxs-lookup"><span data-stu-id="283de-133">OrganizationName</span></span>|<span data-ttu-id="283de-134">String</span><span class="sxs-lookup"><span data-stu-id="283de-134">String</span></span>|<span data-ttu-id="283de-135">Organisation, die dem Apple Volume Purchase Program-Token zugeordnet ist</span><span class="sxs-lookup"><span data-stu-id="283de-135">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="283de-136">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="283de-136">vppTokenAccountType</span></span>|<span data-ttu-id="283de-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="283de-137">String</span></span>|<span data-ttu-id="283de-138">Volume Purchase Program-Typ, dem das angegebene Apple Volume Purchase Program-Token zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="283de-138">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="283de-139">Mögliche Werte sind: `business` und `education`.</span><span class="sxs-lookup"><span data-stu-id="283de-139">Possible values are: `business`, `education`.</span></span> <span data-ttu-id="283de-140">Mögliche Werte sind: `business` und `education`.</span><span class="sxs-lookup"><span data-stu-id="283de-140">Possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="283de-141">appleId</span><span class="sxs-lookup"><span data-stu-id="283de-141">appleId</span></span>|<span data-ttu-id="283de-142">String</span><span class="sxs-lookup"><span data-stu-id="283de-142">String</span></span>|<span data-ttu-id="283de-143">Apple-ID, die dem Apple Volume Purchase Program-Token zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="283de-143">The Apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="283de-144">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="283de-144">expirationDateTime</span></span>|<span data-ttu-id="283de-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="283de-145">DateTimeOffset</span></span>|<span data-ttu-id="283de-146">Ablaufdatum und -uhrzeit des Apple Volume Purchase Program-Token.</span><span class="sxs-lookup"><span data-stu-id="283de-146">The expiration date time of the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="283de-147">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="283de-147">lastSyncDateTime</span></span>|<span data-ttu-id="283de-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="283de-148">DateTimeOffset</span></span>|<span data-ttu-id="283de-149">Zeitpunkt der letzten Synchronisierung der Anwendung mit dem Apple Volume Purchase Program Service mithilfe des Apple Volume Purchase Program-Token.</span><span class="sxs-lookup"><span data-stu-id="283de-149">The last time when an application sync was done with the Apple volume purchase program service using the the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="283de-150">token</span><span class="sxs-lookup"><span data-stu-id="283de-150">token</span></span>|<span data-ttu-id="283de-151">String</span><span class="sxs-lookup"><span data-stu-id="283de-151">String</span></span>|<span data-ttu-id="283de-152">Aus dem Apple Volume Purchase Program heruntergeladene Zeichenfolge des Apple Volume Purchase Program-Token.</span><span class="sxs-lookup"><span data-stu-id="283de-152">The Apple Volume Purchase Program Token string downloaded from the Apple Volume Purchase Program.</span></span>|
|<span data-ttu-id="283de-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="283de-153">lastModifiedDateTime</span></span>|<span data-ttu-id="283de-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="283de-154">DateTimeOffset</span></span>|<span data-ttu-id="283de-155">Letztes Änderungsdatum und letzter Änderungszeitpunkt des Apple Volume Purchase Program-Token.</span><span class="sxs-lookup"><span data-stu-id="283de-155">Last modification date time associated with the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="283de-156">state</span><span class="sxs-lookup"><span data-stu-id="283de-156">state</span></span>|<span data-ttu-id="283de-157">String</span><span class="sxs-lookup"><span data-stu-id="283de-157">String</span></span>|<span data-ttu-id="283de-158">Aktueller Stand des Apple Volume Purchase Program-Token.</span><span class="sxs-lookup"><span data-stu-id="283de-158">Current state of the Apple Volume Purchase Program Token.</span></span> <span data-ttu-id="283de-159">Mögliche Werte sind: `unknown`, `valid`, `expired`, `invalid`.</span><span class="sxs-lookup"><span data-stu-id="283de-159">Possible values are: `unknown`, `valid`, `expired`, `invalid`.</span></span> <span data-ttu-id="283de-160">Mögliche Werte sind: `unknown`, `valid`, `expired`, `invalid`.</span><span class="sxs-lookup"><span data-stu-id="283de-160">Possible values are: `unknown`, `valid`, `expired`, `invalid`.</span></span>|
|<span data-ttu-id="283de-161">lastSyncStatus</span><span class="sxs-lookup"><span data-stu-id="283de-161">lastSyncStatus</span></span>|<span data-ttu-id="283de-162">String</span><span class="sxs-lookup"><span data-stu-id="283de-162">String</span></span>|<span data-ttu-id="283de-163">Aktueller Synchronisierungsstatus seit der letzten Synchronisierung der Anwendung, die mit dem Apple Volume Purchase Program-Token durchgeführt wurde.</span><span class="sxs-lookup"><span data-stu-id="283de-163">Current sync status of the last application sync which was triggered using the Apple Volume Purchase Program Token.</span></span> <span data-ttu-id="283de-164">Mögliche Werte sind: `none`, `inProgress`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="283de-164">Possible values are: `none`, `inProgress`, `completed`, `failed`.</span></span> <span data-ttu-id="283de-165">Mögliche Werte sind: `none`, `inProgress`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="283de-165">Possible values are: `none`, `inProgress`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="283de-166">automaticallyUpdateApps</span><span class="sxs-lookup"><span data-stu-id="283de-166">automaticallyUpdateApps</span></span>|<span data-ttu-id="283de-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="283de-167">Boolean</span></span>|<span data-ttu-id="283de-168">Angabe, ob Anwendungen für das VPP-Token automatisch aktualisiert werden.</span><span class="sxs-lookup"><span data-stu-id="283de-168">Whether or not apps for the VPP token will be automatically updated.</span></span>|
|<span data-ttu-id="283de-169">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="283de-169">countryOrRegion</span></span>|<span data-ttu-id="283de-170">String</span><span class="sxs-lookup"><span data-stu-id="283de-170">String</span></span>|<span data-ttu-id="283de-171">Angabe, ob Anwendungen für das VPP-Token automatisch aktualisiert werden.</span><span class="sxs-lookup"><span data-stu-id="283de-171">Whether or not apps for the VPP token will be automatically updated.</span></span>|



## <a name="response"></a><span data-ttu-id="283de-172">Antwort</span><span class="sxs-lookup"><span data-stu-id="283de-172">Response</span></span>
<span data-ttu-id="283de-173">Bei Erfolg gibt diese Methode den Antwortcode `201 Created` und ein [vppToken](../resources/intune_onboarding_vpptoken.md)-Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="283de-173">If successful, this method returns a `201 Created` response code and a [managedDevice](../resources/intune_onboarding_vpptoken.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="283de-174">Beispiel</span><span class="sxs-lookup"><span data-stu-id="283de-174">Example</span></span>
### <a name="request"></a><span data-ttu-id="283de-175">Anforderung</span><span class="sxs-lookup"><span data-stu-id="283de-175">Request</span></span>
<span data-ttu-id="283de-176">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="283de-176">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/vppTokens
Content-type: application/json
Content-length: 525

{
  "@odata.type": "#microsoft.graph.vppToken",
  "organizationName": "Organization Name value",
  "vppTokenAccountType": "education",
  "appleId": "Apple Id value",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "token": "Token value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "state": "valid",
  "lastSyncStatus": "inProgress",
  "automaticallyUpdateApps": true,
  "countryOrRegion": "Country Or Region value"
}
```

### <a name="response"></a><span data-ttu-id="283de-177">Antwort</span><span class="sxs-lookup"><span data-stu-id="283de-177">Response</span></span>
<span data-ttu-id="283de-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="283de-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 574

{
  "@odata.type": "#microsoft.graph.vppToken",
  "id": "9ceb2f92-2f92-9ceb-922f-eb9c922feb9c",
  "organizationName": "Organization Name value",
  "vppTokenAccountType": "education",
  "appleId": "Apple Id value",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "token": "Token value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "state": "valid",
  "lastSyncStatus": "inProgress",
  "automaticallyUpdateApps": true,
  "countryOrRegion": "Country Or Region value"
}
```



