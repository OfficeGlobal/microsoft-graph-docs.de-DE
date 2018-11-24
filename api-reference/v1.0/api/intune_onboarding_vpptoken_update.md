# <a name="update-vpptoken"></a><span data-ttu-id="7c261-101">VppToken aktualisieren</span><span class="sxs-lookup"><span data-stu-id="7c261-101">Update vppToken</span></span>

> <span data-ttu-id="7c261-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="7c261-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7c261-103">Aktualisieren der Eigenschaften eines [vppToken](../resources/intune_onboarding_vpptoken.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="7c261-103">Update the properties of a [vppToken](../resources/intune_onboarding_vpptoken.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7c261-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="7c261-104">Prerequisites</span></span>
<span data-ttu-id="7c261-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="7c261-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="7c261-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7c261-107">Permission type</span></span>|<span data-ttu-id="7c261-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7c261-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7c261-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7c261-109">Delegated (work or school account)</span></span>|<span data-ttu-id="7c261-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c261-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="7c261-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7c261-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7c261-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7c261-112">Not supported.</span></span>|
|<span data-ttu-id="7c261-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7c261-113">Application</span></span>|<span data-ttu-id="7c261-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7c261-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7c261-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7c261-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/vppTokens/{vppTokenId}
```

## <a name="request-headers"></a><span data-ttu-id="7c261-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7c261-116">Request headers</span></span>
|<span data-ttu-id="7c261-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="7c261-117">Header</span></span>|<span data-ttu-id="7c261-118">Wert</span><span class="sxs-lookup"><span data-stu-id="7c261-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7c261-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="7c261-119">Authorization</span></span>|<span data-ttu-id="7c261-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="7c261-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7c261-121">Accept</span><span class="sxs-lookup"><span data-stu-id="7c261-121">Accept</span></span>|<span data-ttu-id="7c261-122">application/json</span><span class="sxs-lookup"><span data-stu-id="7c261-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7c261-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7c261-123">Request body</span></span>
<span data-ttu-id="7c261-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [vppToken](../resources/intune_onboarding_vpptoken.md) an.</span><span class="sxs-lookup"><span data-stu-id="7c261-124">In the request body, supply a JSON representation for the [vppToken](../resources/intune_onboarding_vpptoken.md) object.</span></span>

<span data-ttu-id="7c261-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [vppToken](../resources/intune_onboarding_vpptoken.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="7c261-125">The following table shows the properties that are required when you create the [vppToken](../resources/intune_onboarding_vpptoken.md).</span></span>

|<span data-ttu-id="7c261-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7c261-126">Property</span></span>|<span data-ttu-id="7c261-127">Typ</span><span class="sxs-lookup"><span data-stu-id="7c261-127">Type</span></span>|<span data-ttu-id="7c261-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7c261-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7c261-129">id</span><span class="sxs-lookup"><span data-stu-id="7c261-129">id</span></span>|<span data-ttu-id="7c261-130">String</span><span class="sxs-lookup"><span data-stu-id="7c261-130">String</span></span>|<span data-ttu-id="7c261-131">Dies wird automatisch generiert, wenn das appleVolumePurchaseProgramToken erstellt wird.</span><span class="sxs-lookup"><span data-stu-id="7c261-131">This is automatically generated when the appleVolumePurchaseProgramToken is created.</span></span> <span data-ttu-id="7c261-132">Es ist der Schlüssel für die Entität.</span><span class="sxs-lookup"><span data-stu-id="7c261-132">It is the Key of the entity.</span></span>|
|<span data-ttu-id="7c261-133">organizationName</span><span class="sxs-lookup"><span data-stu-id="7c261-133">organizationName</span></span>|<span data-ttu-id="7c261-134">String</span><span class="sxs-lookup"><span data-stu-id="7c261-134">String</span></span>|<span data-ttu-id="7c261-135">Organisation, die dem Apple Volume Purchase Program-Token zugeordnet ist</span><span class="sxs-lookup"><span data-stu-id="7c261-135">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="7c261-136">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="7c261-136">vppTokenAccountType</span></span>|[<span data-ttu-id="7c261-137">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="7c261-137">vppTokenAccountType</span></span>](../resources/intune_shared_vpptokenaccounttype.md)|<span data-ttu-id="7c261-138">Volume Purchase Program-Typ, dem das angegebene Apple Volume Purchase Program-Token zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="7c261-138">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="7c261-139">Mögliche Werte sind: `business` und `education`.</span><span class="sxs-lookup"><span data-stu-id="7c261-139">Possible values are: `business`, `education`.</span></span> <span data-ttu-id="7c261-140">Mögliche Werte sind: `business` und `education`.</span><span class="sxs-lookup"><span data-stu-id="7c261-140">Possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="7c261-141">appleId</span><span class="sxs-lookup"><span data-stu-id="7c261-141">appleId</span></span>|<span data-ttu-id="7c261-142">String</span><span class="sxs-lookup"><span data-stu-id="7c261-142">String</span></span>|<span data-ttu-id="7c261-143">Die Apple-ID, die dem Apple Volume Purchase Program-Token zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="7c261-143">The apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="7c261-144">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="7c261-144">expirationDateTime</span></span>|<span data-ttu-id="7c261-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7c261-145">DateTimeOffset</span></span>|<span data-ttu-id="7c261-146">Ablaufdatum und -Uhrzeit des Apple Volume Purchase Program-Tokens</span><span class="sxs-lookup"><span data-stu-id="7c261-146">The expiration date time of the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="7c261-147">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="7c261-147">lastSyncDateTime</span></span>|<span data-ttu-id="7c261-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7c261-148">DateTimeOffset</span></span>|<span data-ttu-id="7c261-149">Der Zeitpunkt der letzten Anwendungssynchronisierung mit dem Apple Volume Purchase Program-Dienst mithilfe des Apple Volume Purchase Program-Tokens.</span><span class="sxs-lookup"><span data-stu-id="7c261-149">The last time when an application sync was done with the Apple volume purchase program service using the the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="7c261-150">token</span><span class="sxs-lookup"><span data-stu-id="7c261-150">token</span></span>|<span data-ttu-id="7c261-151">String</span><span class="sxs-lookup"><span data-stu-id="7c261-151">String</span></span>|<span data-ttu-id="7c261-152">Die Zeichenfolge des Apple Volume Purchase Program-Tokens, die vom Apple Volume Purchase Program heruntergeladen wurde.</span><span class="sxs-lookup"><span data-stu-id="7c261-152">The Apple Volume Purchase Program Token string downloaded from the Apple Volume Purchase Program.</span></span>|
|<span data-ttu-id="7c261-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7c261-153">lastModifiedDateTime</span></span>|<span data-ttu-id="7c261-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7c261-154">DateTimeOffset</span></span>|<span data-ttu-id="7c261-155">Datum und Uhrzeit der letzten Änderung, die dem Apple Volume Purchase Program-Token zugeordnet sind.</span><span class="sxs-lookup"><span data-stu-id="7c261-155">Last modification date time associated with the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="7c261-156">state</span><span class="sxs-lookup"><span data-stu-id="7c261-156">state</span></span>|[<span data-ttu-id="7c261-157">vppTokenState</span><span class="sxs-lookup"><span data-stu-id="7c261-157">vppTokenState</span></span>](../resources/intune_onboarding_vpptokenstate.md)|<span data-ttu-id="7c261-158">Aktueller Status des Apple Volume Purchase Program-Tokens.</span><span class="sxs-lookup"><span data-stu-id="7c261-158">Current state of the Apple Volume Purchase Program Token.</span></span> <span data-ttu-id="7c261-159">Mögliche Werte sind: `unknown`, `valid`, `expired`, `invalid` und `assignedToExternalMDM`.</span><span class="sxs-lookup"><span data-stu-id="7c261-159">Possible values are: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span></span> <span data-ttu-id="7c261-160">Mögliche Werte sind: `unknown`, `valid`, `expired`, `invalid` und `assignedToExternalMDM`.</span><span class="sxs-lookup"><span data-stu-id="7c261-160">Possible values are: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span></span>|
|<span data-ttu-id="7c261-161">lastSyncStatus</span><span class="sxs-lookup"><span data-stu-id="7c261-161">lastSyncStatus</span></span>|[<span data-ttu-id="7c261-162">vppTokenSyncStatus</span><span class="sxs-lookup"><span data-stu-id="7c261-162">vppTokenSyncStatus</span></span>](../resources/intune_onboarding_vpptokensyncstatus.md)|<span data-ttu-id="7c261-163">Aktueller Synchronisierungsstatus der letzten Anwendungssynchronisierung, die mit dem Apple Volume Purchase Program-Token ausgelöst wurde.</span><span class="sxs-lookup"><span data-stu-id="7c261-163">Current sync status of the last application sync which was triggered using the Apple Volume Purchase Program Token.</span></span> <span data-ttu-id="7c261-164">Mögliche Werte sind: `none`, `inProgress`, `completed` und `failed`.</span><span class="sxs-lookup"><span data-stu-id="7c261-164">Possible values are: `none`, `inProgress`, `completed`, `failed`.</span></span> <span data-ttu-id="7c261-165">Mögliche Werte sind: `none`, `inProgress`, `completed` und `failed`.</span><span class="sxs-lookup"><span data-stu-id="7c261-165">Possible values are: `none`, `inProgress`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="7c261-166">automaticallyUpdateApps</span><span class="sxs-lookup"><span data-stu-id="7c261-166">automaticallyUpdateApps</span></span>|<span data-ttu-id="7c261-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="7c261-167">Boolean</span></span>|<span data-ttu-id="7c261-168">Gibt an, ob Apps für das VPP-Token automatisch aktualisiert werden.</span><span class="sxs-lookup"><span data-stu-id="7c261-168">Whether or not apps for the VPP token will be automatically updated.</span></span>|
|<span data-ttu-id="7c261-169">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="7c261-169">countryOrRegion</span></span>|<span data-ttu-id="7c261-170">String</span><span class="sxs-lookup"><span data-stu-id="7c261-170">String</span></span>|<span data-ttu-id="7c261-171">Gibt an, ob Apps für das VPP-Token automatisch aktualisiert werden.</span><span class="sxs-lookup"><span data-stu-id="7c261-171">Whether or not apps for the VPP token will be automatically updated.</span></span>|



## <a name="response"></a><span data-ttu-id="7c261-172">Antwort</span><span class="sxs-lookup"><span data-stu-id="7c261-172">Response</span></span>
<span data-ttu-id="7c261-173">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [vppToken](../resources/intune_onboarding_vpptoken.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="7c261-173">If successful, this method returns a `200 OK` response code and an updated [vppToken](../resources/intune_onboarding_vpptoken.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7c261-174">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7c261-174">Example</span></span>
### <a name="request"></a><span data-ttu-id="7c261-175">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7c261-175">Request</span></span>
<span data-ttu-id="7c261-176">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7c261-176">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/vppTokens/{vppTokenId}
Content-type: application/json
Content-length: 461

{
  "@odata.type": "#microsoft.graph.vppToken",
  "organizationName": "Organization Name value",
  "vppTokenAccountType": "education",
  "appleId": "Apple Id value",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "token": "Token value",
  "state": "valid",
  "lastSyncStatus": "inProgress",
  "automaticallyUpdateApps": true,
  "countryOrRegion": "Country Or Region value"
}
```

### <a name="response"></a><span data-ttu-id="7c261-177">Antwort</span><span class="sxs-lookup"><span data-stu-id="7c261-177">Response</span></span>
<span data-ttu-id="7c261-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7c261-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



